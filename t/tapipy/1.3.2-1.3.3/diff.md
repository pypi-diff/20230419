# Comparing `tmp/tapipy-1.3.2.tar.gz` & `tmp/tapipy-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapipy-1.3.2.tar", max compression
+gzip compressed data, was "tapipy-1.3.3.tar", max compression
```

## Comparing `tapipy-1.3.2.tar` & `tapipy-1.3.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1539 2022-05-17 23:01:20.810838 tapipy-1.3.2/LICENSE.md
--rw-r--r--   0        0        0     8639 2022-09-27 22:55:39.801480 tapipy-1.3.2/README.md
--rw-r--r--   0        0        0      970 2023-04-14 14:58:36.392257 tapipy-1.3.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-14 14:58:32.612293 tapipy-1.3.2/tapipy/__init__.py
--rw-r--r--   0        0        0    13502 2022-09-27 22:40:07.902909 tapipy-1.3.2/tapipy/actors.py
--rw-r--r--   0        0        0     2071 2022-10-13 22:38:48.858613 tapipy-1.3.2/tapipy/errors.py
--rw-r--r--   0        0        0    38703 2022-05-17 23:01:20.818838 tapipy-1.3.2/tapipy/resources/openapi_v3-actors.yml
--rw-r--r--   0        0        0    65073 2023-04-14 14:57:18.237004 tapipy-1.3.2/tapipy/resources/openapi_v3-apps.yml
--rw-r--r--   0        0        0    23554 2022-10-13 22:47:01.777739 tapipy-1.3.2/tapipy/resources/openapi_v3-authenticator.yml
--rw-r--r--   0        0        0    73300 2023-03-23 16:19:52.690490 tapipy-1.3.2/tapipy/resources/openapi_v3-files.yml
--rw-r--r--   0        0        0    65257 2023-03-22 22:25:39.039342 tapipy-1.3.2/tapipy/resources/openapi_v3-jobs.yml
--rw-r--r--   0        0        0    28625 2022-05-17 23:01:20.822838 tapipy-1.3.2/tapipy/resources/openapi_v3-meta.yml
--rw-r--r--   0        0        0    52031 2023-04-14 14:57:21.296975 tapipy-1.3.2/tapipy/resources/openapi_v3-notifications.yml
--rw-r--r--   0        0        0    33814 2023-03-22 22:25:37.527357 tapipy-1.3.2/tapipy/resources/openapi_v3-pgrest.yml
--rw-r--r--   0        0        0    30728 2022-12-13 18:05:18.840827 tapipy-1.3.2/tapipy/resources/openapi_v3-pods.yml
--rw-r--r--   0        0        0   145319 2022-10-25 21:18:32.853350 tapipy-1.3.2/tapipy/resources/openapi_v3-sk.yml
--rw-r--r--   0        0        0   108752 2023-03-22 22:25:35.307379 tapipy-1.3.2/tapipy/resources/openapi_v3-streams.yml
--rw-r--r--   0        0        0    90114 2023-04-14 14:57:14.489040 tapipy-1.3.2/tapipy/resources/openapi_v3-systems.yml
--rw-r--r--   0        0        0    25448 2022-05-17 23:01:20.826838 tapipy-1.3.2/tapipy/resources/openapi_v3-tenants.yml
--rw-r--r--   0        0        0     8406 2022-10-13 22:47:04.421713 tapipy-1.3.2/tapipy/resources/openapi_v3-tokens.yml
--rw-r--r--   0        0        0    87200 2023-04-14 14:57:20.564982 tapipy-1.3.2/tapipy/resources/openapi_v3-workflows.yml
--rw-r--r--   0        0        0      907 2023-04-14 14:57:21.308975 tapipy-1.3.2/tapipy/resources/resource_etags.json
--rw-r--r--   0        0        0    24325 2023-04-14 14:57:24.052949 tapipy-1.3.2/tapipy/specs/tapis-project-pods_service-prod-docs-openapi_v3-pods.pickle
--rw-r--r--   0        0        0    30512 2023-04-14 14:57:21.852970 tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-actors.pickle
--rw-r--r--   0        0        0    49315 2023-04-14 14:57:24.748942 tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-apps.pickle
--rw-r--r--   0        0        0    19368 2023-04-14 14:57:21.944969 tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-authenticator.pickle
--rw-r--r--   0        0        0    55192 2023-04-14 14:57:22.332965 tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-files.pickle
--rw-r--r--   0        0        0    49485 2023-04-14 14:57:24.408945 tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-jobs.pickle
--rw-r--r--   0        0        0    21718 2023-04-14 14:57:22.052968 tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-meta.pickle
--rw-r--r--   0        0        0    40403 2023-04-14 14:57:24.952940 tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-notifications.pickle
--rw-r--r--   0        0        0    27737 2023-04-14 14:57:23.896950 tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-pgrest.pickle
--rw-r--r--   0        0        0   117394 2023-04-14 14:57:22.792961 tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-sk.pickle
--rw-r--r--   0        0        0    81328 2023-04-14 14:57:23.228956 tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-streams.pickle
--rw-r--r--   0        0        0    69380 2023-04-14 14:57:23.588953 tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-systems.pickle
--rw-r--r--   0        0        0    20570 2023-04-14 14:57:23.708952 tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tenants.pickle
--rw-r--r--   0        0        0     7112 2023-04-14 14:57:23.764951 tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tokens.pickle
--rw-r--r--   0        0        0    64540 2023-04-14 14:57:26.352927 tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-workflows.pickle
--rw-r--r--   0        0        0    14089 2022-05-17 23:01:20.830838 tapipy-1.3.2/tapipy/specs/tapis-project-tapis-client-java-dev-jobs-client-src-main-resources-jobsapi.pickle
--rw-r--r--   0        0        0    70890 2023-04-14 15:12:33.374927 tapipy-1.3.2/tapipy/tapis.py
--rw-r--r--   0        0        0      144 2022-05-17 23:01:20.834838 tapipy-1.3.2/tapipy/util.py
--rw-r--r--   0        0        0    10018 1970-01-01 00:00:00.000000 tapipy-1.3.2/setup.py
--rw-r--r--   0        0        0    10051 1970-01-01 00:00:00.000000 tapipy-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1539 2022-05-17 23:01:20.810838 tapipy-1.3.3/LICENSE.md
+-rw-r--r--   0        0        0     8639 2022-09-27 22:55:39.801480 tapipy-1.3.3/README.md
+-rw-r--r--   0        0        0      970 2023-04-18 21:53:08.470903 tapipy-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-18 21:53:04.234943 tapipy-1.3.3/tapipy/__init__.py
+-rw-r--r--   0        0        0    13502 2022-09-27 22:40:07.902909 tapipy-1.3.3/tapipy/actors.py
+-rw-r--r--   0        0        0     2071 2022-10-13 22:38:48.858613 tapipy-1.3.3/tapipy/errors.py
+-rw-r--r--   0        0        0    38703 2022-05-17 23:01:20.818838 tapipy-1.3.3/tapipy/resources/openapi_v3-actors.yml
+-rw-r--r--   0        0        0    65073 2023-04-14 14:57:18.237004 tapipy-1.3.3/tapipy/resources/openapi_v3-apps.yml
+-rw-r--r--   0        0        0    23554 2022-10-13 22:47:01.777739 tapipy-1.3.3/tapipy/resources/openapi_v3-authenticator.yml
+-rw-r--r--   0        0        0    73801 2023-04-18 21:51:45.271692 tapipy-1.3.3/tapipy/resources/openapi_v3-files.yml
+-rw-r--r--   0        0        0    65257 2023-03-22 22:25:39.039342 tapipy-1.3.3/tapipy/resources/openapi_v3-jobs.yml
+-rw-r--r--   0        0        0    28625 2022-05-17 23:01:20.822838 tapipy-1.3.3/tapipy/resources/openapi_v3-meta.yml
+-rw-r--r--   0        0        0    52031 2023-04-14 14:57:21.296975 tapipy-1.3.3/tapipy/resources/openapi_v3-notifications.yml
+-rw-r--r--   0        0        0    33814 2023-03-22 22:25:37.527357 tapipy-1.3.3/tapipy/resources/openapi_v3-pgrest.yml
+-rw-r--r--   0        0        0    30728 2022-12-13 18:05:18.840827 tapipy-1.3.3/tapipy/resources/openapi_v3-pods.yml
+-rw-r--r--   0        0        0   145319 2022-10-25 21:18:32.853350 tapipy-1.3.3/tapipy/resources/openapi_v3-sk.yml
+-rw-r--r--   0        0        0   108752 2023-03-22 22:25:35.307379 tapipy-1.3.3/tapipy/resources/openapi_v3-streams.yml
+-rw-r--r--   0        0        0    90114 2023-04-14 14:57:14.489040 tapipy-1.3.3/tapipy/resources/openapi_v3-systems.yml
+-rw-r--r--   0        0        0    25448 2022-05-17 23:01:20.826838 tapipy-1.3.3/tapipy/resources/openapi_v3-tenants.yml
+-rw-r--r--   0        0        0     8406 2022-10-13 22:47:04.421713 tapipy-1.3.3/tapipy/resources/openapi_v3-tokens.yml
+-rw-r--r--   0        0        0    87200 2023-04-14 14:57:20.564982 tapipy-1.3.3/tapipy/resources/openapi_v3-workflows.yml
+-rw-r--r--   0        0        0      907 2023-04-18 21:51:51.319634 tapipy-1.3.3/tapipy/resources/resource_etags.json
+-rw-r--r--   0        0        0    24325 2023-04-18 21:51:54.179607 tapipy-1.3.3/tapipy/specs/tapis-project-pods_service-prod-docs-openapi_v3-pods.pickle
+-rw-r--r--   0        0        0    30512 2023-04-18 21:51:51.895629 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-actors.pickle
+-rw-r--r--   0        0        0    49315 2023-04-18 21:51:54.827601 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-apps.pickle
+-rw-r--r--   0        0        0    19368 2023-04-18 21:51:51.995628 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-authenticator.pickle
+-rw-r--r--   0        0        0    55698 2023-04-18 21:51:52.423624 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-files.pickle
+-rw-r--r--   0        0        0    49485 2023-04-18 21:51:54.527604 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-jobs.pickle
+-rw-r--r--   0        0        0    21718 2023-04-18 21:51:52.115627 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-meta.pickle
+-rw-r--r--   0        0        0    40403 2023-04-18 21:51:55.043599 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-notifications.pickle
+-rw-r--r--   0        0        0    27737 2023-04-18 21:51:54.019609 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-pgrest.pickle
+-rw-r--r--   0        0        0   117394 2023-04-18 21:51:52.911619 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-sk.pickle
+-rw-r--r--   0        0        0    81328 2023-04-18 21:51:53.375615 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-streams.pickle
+-rw-r--r--   0        0        0    69380 2023-04-18 21:51:53.715612 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-systems.pickle
+-rw-r--r--   0        0        0    20570 2023-04-18 21:51:53.839611 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tenants.pickle
+-rw-r--r--   0        0        0     7112 2023-04-18 21:51:53.887610 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tokens.pickle
+-rw-r--r--   0        0        0    64540 2023-04-18 21:51:56.747583 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-workflows.pickle
+-rw-r--r--   0        0        0    14089 2022-05-17 23:01:20.830838 tapipy-1.3.3/tapipy/specs/tapis-project-tapis-client-java-dev-jobs-client-src-main-resources-jobsapi.pickle
+-rw-r--r--   0        0        0    70890 2023-04-14 15:12:33.374927 tapipy-1.3.3/tapipy/tapis.py
+-rw-r--r--   0        0        0      144 2022-05-17 23:01:20.834838 tapipy-1.3.3/tapipy/util.py
+-rw-r--r--   0        0        0    10018 1970-01-01 00:00:00.000000 tapipy-1.3.3/setup.py
+-rw-r--r--   0        0        0    10051 1970-01-01 00:00:00.000000 tapipy-1.3.3/PKG-INFO
```

### Comparing `tapipy-1.3.2/LICENSE.md` & `tapipy-1.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/README.md` & `tapipy-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/pyproject.toml` & `tapipy-1.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tapipy"
-version = "1.3.2"
+version = "1.3.3"
 description = "Python lib for interacting with an instance of the Tapis API Framework"
 license = "BSD-4-Clause"
 authors = ["Joe Stubbs <jstubbs@tacc.utexas.edu>"]
 maintainers = ["Joe Stubbs <jstubbs@tacc.utexas.edu>",
 			   "Christian Garcia <cgarcia@tacc.utexas.edu>"]
 readme = "README.md"
 repository = "https://github.com/tapis-project/tapipy"
```

### Comparing `tapipy-1.3.2/tapipy/actors.py` & `tapipy-1.3.3/tapipy/actors.py`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/errors.py` & `tapipy-1.3.3/tapipy/errors.py`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/resources/openapi_v3-actors.yml` & `tapipy-1.3.3/tapipy/resources/openapi_v3-actors.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/resources/openapi_v3-apps.yml` & `tapipy-1.3.3/tapipy/resources/openapi_v3-apps.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/resources/openapi_v3-authenticator.yml` & `tapipy-1.3.3/tapipy/resources/openapi_v3-authenticator.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/resources/openapi_v3-files.yml` & `tapipy-1.3.3/tapipy/resources/openapi_v3-files.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 openapi: 3.0.3
 info:
   title: Tapis Files API
   description: The Tapis Files API provides for management of file resources on Tapis systems
-  version: '1.3.0'
+  version: '1.3.5'
   termsOfService: "https://tapis-project.org"
   contact:
     name: "Files API - CICSupport"
     url: "https://tapis-project.org"
     email: "cicsupport@tacc.utexas.edu"
   license:
     name: 3-Clause BSD License
@@ -39,16 +39,16 @@
   
       Please note that Tapis also supports a higher level approach to granting access known as *Sharing*.
 
       Finally, be aware that Tapis permissions are independent of native permissions enforced by the underlying system host.
   - name: Sharing
     description: |
       In addition to fine grained permissions support, Tapis also supports a higher level approach to granting access.
-      This approach is known simply as *sharing*. The sharing API allows you to share a path with a set of users
-      as well as share publicly with all users in a tenant. Sharing a path grants users READ access to the path.
+      This approach is known simply as *sharing*. The sharing API allows you to share a path with a set of users as
+      well as share publicly with all users in a tenant. Sharing a path grants users READ or MODIFY access to the path.
       
       Please note that the underlying host associated with a system typically also has it's own access controls.
 
 # ------------------------------------------------------------------------------
 # --- Paths -------------------------------------------------------------------
 # ------------------------------------------------------------------------------
 paths:
@@ -81,15 +81,15 @@
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/RespBasic'
         '503':
           description: Service unavailable.
 
-  # --- Paths for /files/ops --------------------------------------- --------------
+  # --- Paths for /files/ops -----------------------------------------------------
   /v3/files/ops/{systemId}/{path}:
     get:
       tags:
         - File Operations
       description: |
         List files or objects on a Tapis system. Type for items will depend on system type. For example, for LINUX
         they will be posix files and for S3 they will be storage objects. For S3 the recurse flag is ignored and all
@@ -100,16 +100,17 @@
         Note that S3 buckets do not have a hierarchical structure. There are no directories. Everything is an object
         associated with a key.
 
         Certain services may use the query parameter *impersonationId* to be used in place of the requesting
         Tapis user. Tapis will use this user Id when performing authorization and resolving the *effectiveUserId*
         for the system.
         
-        Certain services may use the query parameter *sharedAppCtx* to indicate that the request is in a shared
-        application context. Tapis authorization will be bypassed.
+        Certain services may use the query parameter *sharedCtx* to indicate that the request is in a shared
+        context. *sharedCtx* must be set to the share grantor.
+        Tapis will include the share grantor as part of authorization checks.
       operationId: listFiles
       parameters:
         - name: systemId
           in: path
           description: System ID
           required: true
           schema:
@@ -117,15 +118,15 @@
           example: system123
         - name: path
           in: path
           description: Path relative to the system *rootDir*
           required: true
           schema:
             type: string
-          example: /directoryA/directoryB/
+          example: directoryA/directoryB/
         - name: limit
           in: query
           description: pagination limit
           schema:
             type: integer
             format: int32
             default: 1000
@@ -146,20 +147,19 @@
             default: false
           example: false
         - name: impersonationId
           in: query
           description: Restricted. Only certain services may impersonate a Tapis user.
           schema:
             type: string
-        - name: sharedAppCtx
+        - name: sharedCtx
           in: query
-          description: Restricted. Only certain services may indicate that the request is in a shared context.
+          description: Restricted. Only certain services may indicate that the request is in a shared context. Must be set to the share grantor.
           schema:
-            type: boolean
-            default: false
+            $ref: '#/components/schemas/UserNameString'
       responses:
         '200':
           description: A list of files
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/FileListingResponse'
@@ -384,30 +384,31 @@
   /v3/files/ops/{systemId}:
     post:
       tags:
         - File Operations
       description: |
         Create a directory on the system at the given path. Not supported for all system types. Currently supported
         for LINUX and IRODS type systems.
-        Certain services may use the query parameter *sharedAppCtx* to indicate that the request is in a shared
-        application context. Tapis authorization will be bypassed.
+
+        Certain services may use the query parameter *sharedCtx* to indicate that the request is in a shared
+        context. *sharedCtx* must be set to the share grantor.
+        Tapis will include the share grantor as part of authorization checks.
       operationId: mkdir
       parameters:
         - name: systemId
           in: path
           description: System ID
           required: true
           schema:
             type: string
-        - name: sharedAppCtx
+        - name: sharedCtx
           in: query
-          description: Restricted. Only certain services may indicate that the request is in a shared context.
+          description: Restricted. Only certain services may indicate that the request is in a shared context. Must be set to the share grantor.
           schema:
-            type: boolean
-            default: false
+            $ref: '#/components/schemas/UserNameString'
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/MkdirRequest'
       responses:
         '200':
@@ -459,15 +460,15 @@
           example: system123
         - name: path
           in: path
           description: Path relative to the system *rootDir*
           required: true
           schema:
             type: string
-          example: /directoryA/file1
+          example: directoryA/file1
         - name: followLinks
           in: query
           description: When path is a symbolic link whether to get information about the link (false) or the link target (true)
           schema:
             type: boolean
             default: false
           example: true
@@ -714,16 +715,17 @@
         Tapis user. Tapis will use this user Id when performing authorization and resolving the *effectiveUserId*
         for the system.
         
         Use the query parameter *zip* to request a stream compressed using the ZIP file format. This is not allowed
         if system *rootDir* plus *path* would result in all files on the host being included. Please download
         individual directories, files or objects.
         
-        Certain services may use the query parameter *sharedAppCtx* to indicate that the request is in a shared
-        application context. Tapis authorization will be bypassed.
+        Certain services may use the query parameter *sharedCtx* to indicate that the request is in a shared
+        context. *sharedCtx* must be set to the share grantor.
+        Tapis will include the share grantor as part of authorization checks.
       operationId: getContents
       parameters:
         - name: systemId
           in: path
           description: System ID
           required: true
           schema:
@@ -731,15 +733,15 @@
           example: system123
         - name: path
           in: path
           description: Path relative to the system *rootDir*
           required: true
           schema:
             type: string
-          example: /directoryA/directoryB/
+          example: directoryA/directoryB/
         - name: range
           in: header
           description: Optional range of bytes to send. If not specified all content
             will be sent.
           schema:
             $ref: '#/components/schemas/HeaderByteRange'
           example: range=0,999
@@ -756,20 +758,19 @@
             type: integer
             format: int64
         - name: impersonationId
           in: query
           description: Restricted. Only certain services may impersonate a Tapis user.
           schema:
             type: string
-        - name: sharedAppCtx
+        - name: sharedCtx
           in: query
-          description: Restricted. Only certain services may indicate that the request is in a shared context.
+          description: Restricted. Only certain services may indicate that the request is in a shared context. Must be set to the share grantor.
           schema:
-            type: boolean
-            default: false
+            $ref: '#/components/schemas/UserNameString'
       responses:
         '200':
           description: OK
         '400':
           description: Bad Request
         '401':
           description: Not Authenticated
@@ -885,15 +886,15 @@
           description: Transfer task ID
           required: true
           schema:
             type: string
           example: 6491c2a5-acb2-40ef-b2c0-bc1fc4cd7e6c
         - name: impersonationId
           in: query
-          description: Highly restricted. Only certain services may impersonate a Tapis user.
+          description: Restricted. Only certain services may impersonate a Tapis user.
           schema:
             type: string
       responses:
         '200':
           description: OK
           content:
             application/json:
@@ -1612,14 +1613,20 @@
         - name: zip
           in: query
           description: Indicates a zip output stream should be provided.  If zip is not provided it defaults to false unless
             the path is a directory.  In the case of a directory the content will be zipped.
           schema:
             type: boolean
           example: false
+        - name: download
+          in: query
+          description: If set to true, this will force a browser to initiate a file download.  If set to false, the content-disposition header will be set to inline causing the browser to render the document.  If download is not provided it defaults to false. 
+          schema:
+            type: boolean
+          example: false
       responses:
         '200':
           description: Success.
         '400':
           description: Bad Request
           content:
             application/json:
@@ -2055,22 +2062,18 @@
           type: string
         destinationURI:
           type: string
         optional:
           type: boolean
           default: false
           description: Allow the full transfer to succeed even if this element fails.
-        srcSharedAppCtx:
-          type: boolean
-          default: false
-          description: Certain services may indicate that the request is in a shared context.
-        destSharedAppCtx:
-          type: boolean
-          default: false
-          description: Certain services may indicate that the request is in a shared context.
+        srcSharedCtx:
+          $ref: '#/components/schemas/UserNameString'
+        destSharedCtx:
+          $ref: '#/components/schemas/UserNameString'
     NativeLinuxOpRequest:
       required:
         - argument
         - operation
       type: object
       properties:
         operation:
@@ -2121,15 +2124,15 @@
           format: int32
           description: | 
             Number of times that the new PostIt can be redeemed. The
             default is one use.  Setting the value to -1 (negative one)
             will allow the PostIt to be redeemed an unlimited number of
             times.
           default: 1
-        expirationSeconds:
+        validSeconds:
           type: string
           format: int32
           description: | 
             Number of seconds until the PostIt expires.  
             Default is 30 days.
           default: 2592000
```

### Comparing `tapipy-1.3.2/tapipy/resources/openapi_v3-jobs.yml` & `tapipy-1.3.3/tapipy/resources/openapi_v3-jobs.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/resources/openapi_v3-meta.yml` & `tapipy-1.3.3/tapipy/resources/openapi_v3-meta.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/resources/openapi_v3-notifications.yml` & `tapipy-1.3.3/tapipy/resources/openapi_v3-notifications.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/resources/openapi_v3-pgrest.yml` & `tapipy-1.3.3/tapipy/resources/openapi_v3-pgrest.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/resources/openapi_v3-pods.yml` & `tapipy-1.3.3/tapipy/resources/openapi_v3-pods.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/resources/openapi_v3-sk.yml` & `tapipy-1.3.3/tapipy/resources/openapi_v3-sk.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/resources/openapi_v3-streams.yml` & `tapipy-1.3.3/tapipy/resources/openapi_v3-streams.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/resources/openapi_v3-systems.yml` & `tapipy-1.3.3/tapipy/resources/openapi_v3-systems.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/resources/openapi_v3-tenants.yml` & `tapipy-1.3.3/tapipy/resources/openapi_v3-tenants.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/resources/openapi_v3-tokens.yml` & `tapipy-1.3.3/tapipy/resources/openapi_v3-tokens.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/resources/openapi_v3-workflows.yml` & `tapipy-1.3.3/tapipy/resources/openapi_v3-workflows.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/resources/resource_etags.json` & `tapipy-1.3.3/tapipy/resources/resource_etags.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'files'": '\'W/"a5877986f5ce5feefc53dda54f64b913415e32b6"\''}*

```diff
@@ -1,12 +1,12 @@
 {
     "actors": "W/\"790d47ac8c8c65e702080db8e564c154ee3ba420\"",
     "apps": "W/\"a1560cf120d77dcbc4adf9ad31646a2b504d2a96\"",
     "authenticator": "W/\"e81fcd4d421ec0a30d25bcfe7bb039af27c9acd1\"",
-    "files": "W/\"0e75984a5be027eb8b90c2f7d10ae6e69a17b482\"",
+    "files": "W/\"a5877986f5ce5feefc53dda54f64b913415e32b6\"",
     "jobs": "W/\"ed61f6fb359161059940c6eb0a28175b58dc42c9\"",
     "meta": "W/\"e49bc20f1b1e3296278db40fdd6b33d92c44beea\"",
     "notifications": "W/\"93c92b6a473db7d5e02a0cebde5c91b2c706c63a\"",
     "pgrest": "W/\"6494d146379036fdd95de0ed7da22d1bec1335cd\"",
     "pods": "W/\"d0f92c40b0ccec6f194257b75e335bb2352b00dc\"",
     "sk": "W/\"1d60d95dc6576e129817e90c107bd4daf0200e4c\"",
     "streams": "W/\"d48bb1cdc3a01f8b4b42ecacc9f41585c29a660b\"",
```

### Comparing `tapipy-1.3.2/tapipy/specs/tapis-project-pods_service-prod-docs-openapi_v3-pods.pickle` & `tapipy-1.3.3/tapipy/specs/tapis-project-pods_service-prod-docs-openapi_v3-pods.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-actors.pickle` & `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-actors.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-apps.pickle` & `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-apps.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-authenticator.pickle` & `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-authenticator.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-files.pickle` & `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-files.pickle`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-00000000: 8004 958d d700 0000 0000 007d 9428 8c07  ...........}.(..
+00000000: 8004 9587 d900 0000 0000 007d 9428 8c07  ...........}.(..
 00000010: 6f70 656e 6170 6994 8c05 332e 302e 3394  openapi...3.0.3.
 00000020: 8c04 696e 666f 947d 9428 8c05 7469 746c  ..info.}.(..titl
 00000030: 6594 8c0f 5461 7069 7320 4669 6c65 7320  e...Tapis Files 
 00000040: 4150 4994 8c0b 6465 7363 7269 7074 696f  API...descriptio
 00000050: 6e94 8c4e 5468 6520 5461 7069 7320 4669  n..NThe Tapis Fi
 00000060: 6c65 7320 4150 4920 7072 6f76 6964 6573  les API provides
 00000070: 2066 6f72 206d 616e 6167 656d 656e 7420   for management 
 00000080: 6f66 2066 696c 6520 7265 736f 7572 6365  of file resource
 00000090: 7320 6f6e 2054 6170 6973 2073 7973 7465  s on Tapis syste
 000000a0: 6d73 948c 0776 6572 7369 6f6e 948c 0531  ms...version...1
-000000b0: 2e33 2e30 948c 0e74 6572 6d73 4f66 5365  .3.0...termsOfSe
+000000b0: 2e33 2e35 948c 0e74 6572 6d73 4f66 5365  .3.5...termsOfSe
 000000c0: 7276 6963 6594 8c19 6874 7470 733a 2f2f  rvice...https://
 000000d0: 7461 7069 732d 7072 6f6a 6563 742e 6f72  tapis-project.or
 000000e0: 6794 8c07 636f 6e74 6163 7494 7d94 288c  g...contact.}.(.
 000000f0: 046e 616d 6594 8c16 4669 6c65 7320 4150  .name...Files AP
 00000100: 4920 2d20 4349 4353 7570 706f 7274 948c  I - CICSupport..
 00000110: 0375 726c 948c 1968 7474 7073 3a2f 2f74  .url...https://t
 00000120: 6170 6973 2d70 726f 6a65 6374 2e6f 7267  apis-project.org
@@ -95,3356 +95,3388 @@
 000005e0: 2069 6e64 6570 656e 6465 6e74 206f 6620   independent of 
 000005f0: 6e61 7469 7665 2070 6572 6d69 7373 696f  native permissio
 00000600: 6e73 2065 6e66 6f72 6365 6420 6279 2074  ns enforced by t
 00000610: 6865 2075 6e64 6572 6c79 696e 6720 7379  he underlying sy
 00000620: 7374 656d 2068 6f73 742e 0a94 757d 9428  stem host...u}.(
 00000630: 8c04 6e61 6d65 948c 0753 6861 7269 6e67  ..name...Sharing
 00000640: 948c 0b64 6573 6372 6970 7469 6f6e 9458  ...description.X
-00000650: b301 0000 496e 2061 6464 6974 696f 6e20  ....In addition 
+00000650: bd01 0000 496e 2061 6464 6974 696f 6e20  ....In addition 
 00000660: 746f 2066 696e 6520 6772 6169 6e65 6420  to fine grained 
 00000670: 7065 726d 6973 7369 6f6e 7320 7375 7070  permissions supp
 00000680: 6f72 742c 2054 6170 6973 2061 6c73 6f20  ort, Tapis also 
 00000690: 7375 7070 6f72 7473 2061 2068 6967 6865  supports a highe
 000006a0: 7220 6c65 7665 6c20 6170 7072 6f61 6368  r level approach
 000006b0: 2074 6f20 6772 616e 7469 6e67 2061 6363   to granting acc
 000006c0: 6573 732e 0a54 6869 7320 6170 7072 6f61  ess..This approa
 000006d0: 6368 2069 7320 6b6e 6f77 6e20 7369 6d70  ch is known simp
 000006e0: 6c79 2061 7320 2a73 6861 7269 6e67 2a2e  ly as *sharing*.
 000006f0: 2054 6865 2073 6861 7269 6e67 2041 5049   The sharing API
 00000700: 2061 6c6c 6f77 7320 796f 7520 746f 2073   allows you to s
 00000710: 6861 7265 2061 2070 6174 6820 7769 7468  hare a path with
-00000720: 2061 2073 6574 206f 6620 7573 6572 730a   a set of users.
-00000730: 6173 2077 656c 6c20 6173 2073 6861 7265  as well as share
+00000720: 2061 2073 6574 206f 6620 7573 6572 7320   a set of users 
+00000730: 6173 0a77 656c 6c20 6173 2073 6861 7265  as.well as share
 00000740: 2070 7562 6c69 636c 7920 7769 7468 2061   publicly with a
 00000750: 6c6c 2075 7365 7273 2069 6e20 6120 7465  ll users in a te
 00000760: 6e61 6e74 2e20 5368 6172 696e 6720 6120  nant. Sharing a 
 00000770: 7061 7468 2067 7261 6e74 7320 7573 6572  path grants user
-00000780: 7320 5245 4144 2061 6363 6573 7320 746f  s READ access to
-00000790: 2074 6865 2070 6174 682e 0a0a 506c 6561   the path...Plea
-000007a0: 7365 206e 6f74 6520 7468 6174 2074 6865  se note that the
-000007b0: 2075 6e64 6572 6c79 696e 6720 686f 7374   underlying host
-000007c0: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-000007d0: 2061 2073 7973 7465 6d20 7479 7069 6361   a system typica
-000007e0: 6c6c 7920 616c 736f 2068 6173 2069 7427  lly also has it'
-000007f0: 7320 6f77 6e20 6163 6365 7373 2063 6f6e  s own access con
-00000800: 7472 6f6c 732e 0a94 7565 8c05 7061 7468  trols...ue..path
-00000810: 7394 7d94 288c 152f 7633 2f66 696c 6573  s.}.(../v3/files
-00000820: 2f68 6561 6c74 6863 6865 636b 947d 948c  /healthcheck.}..
-00000830: 0367 6574 947d 9428 8c04 7461 6773 945d  .get.}.(..tags.]
-00000840: 948c 0747 656e 6572 616c 9461 8c0b 6465  ...General.a..de
-00000850: 7363 7269 7074 696f 6e94 8c0c 4865 616c  scription...Heal
-00000860: 7468 2063 6865 636b 948c 0b6f 7065 7261  th check...opera
-00000870: 7469 6f6e 4964 948c 0b68 6561 6c74 6843  tionId...healthC
-00000880: 6865 636b 948c 0972 6573 706f 6e73 6573  heck...responses
-00000890: 947d 9428 8c03 3230 3094 7d94 288c 0b64  .}.(..200.}.(..d
-000008a0: 6573 6372 6970 7469 6f6e 948c 114d 6573  escription...Mes
-000008b0: 7361 6765 2072 6563 6569 7665 642e 948c  sage received...
-000008c0: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
-000008d0: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
-000008e0: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
-000008f0: 6694 8c1e 232f 636f 6d70 6f6e 656e 7473  f...#/components
-00000900: 2f73 6368 656d 6173 2f52 6573 7042 6173  /schemas/RespBas
-00000910: 6963 9473 7373 758c 0335 3030 947d 948c  ic.sssu..500.}..
-00000920: 0b64 6573 6372 6970 7469 6f6e 948c 0d53  .description...S
-00000930: 6572 7665 7220 6572 726f 722e 9473 7575  erver error..suu
-00000940: 738c 142f 7633 2f66 696c 6573 2f72 6561  s../v3/files/rea
-00000950: 6479 6368 6563 6b94 7d94 8c03 6765 7494  dycheck.}...get.
-00000960: 7d94 288c 0474 6167 7394 5d94 8c07 4765  }.(..tags.]...Ge
-00000970: 6e65 7261 6c94 618c 0b64 6573 6372 6970  neral.a..descrip
-00000980: 7469 6f6e 948c 0b52 6561 6479 2063 6865  tion...Ready che
-00000990: 636b 948c 0b6f 7065 7261 7469 6f6e 4964  ck...operationId
-000009a0: 948c 0a72 6561 6479 4368 6563 6b94 8c09  ...readyCheck...
-000009b0: 7265 7370 6f6e 7365 7394 7d94 288c 0332  responses.}.(..2
-000009c0: 3030 947d 9428 8c0b 6465 7363 7269 7074  00.}.(..descript
-000009d0: 696f 6e94 8c0e 5365 7276 6963 6520 7265  ion...Service re
-000009e0: 6164 792e 948c 0763 6f6e 7465 6e74 947d  ady....content.}
-000009f0: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
-00000a00: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
-00000a10: 948c 0424 7265 6694 8c1e 232f 636f 6d70  ...$ref...#/comp
-00000a20: 6f6e 656e 7473 2f73 6368 656d 6173 2f52  onents/schemas/R
-00000a30: 6573 7042 6173 6963 9473 7373 758c 0335  espBasic.sssu..5
-00000a40: 3033 947d 948c 0b64 6573 6372 6970 7469  03.}...descripti
-00000a50: 6f6e 948c 1453 6572 7669 6365 2075 6e61  on...Service una
-00000a60: 7661 696c 6162 6c65 2e94 7375 7573 8c1f  vailable..suus..
-00000a70: 2f76 332f 6669 6c65 732f 6f70 732f 7b73  /v3/files/ops/{s
-00000a80: 7973 7465 6d49 647d 2f7b 7061 7468 7d94  ystemId}/{path}.
-00000a90: 7d94 288c 0367 6574 947d 9428 8c04 7461  }.(..get.}.(..ta
-00000aa0: 6773 945d 948c 0f46 696c 6520 4f70 6572  gs.]...File Oper
-00000ab0: 6174 696f 6e73 9461 8c0b 6465 7363 7269  ations.a..descri
-00000ac0: 7074 696f 6e94 5877 0300 004c 6973 7420  ption.Xw...List 
-00000ad0: 6669 6c65 7320 6f72 206f 626a 6563 7473  files or objects
-00000ae0: 206f 6e20 6120 5461 7069 7320 7379 7374   on a Tapis syst
-00000af0: 656d 2e20 5479 7065 2066 6f72 2069 7465  em. Type for ite
-00000b00: 6d73 2077 696c 6c20 6465 7065 6e64 206f  ms will depend o
-00000b10: 6e20 7379 7374 656d 2074 7970 652e 2046  n system type. F
-00000b20: 6f72 2065 7861 6d70 6c65 2c20 666f 7220  or example, for 
-00000b30: 4c49 4e55 580a 7468 6579 2077 696c 6c20  LINUX.they will 
-00000b40: 6265 2070 6f73 6978 2066 696c 6573 2061  be posix files a
-00000b50: 6e64 2066 6f72 2053 3320 7468 6579 2077  nd for S3 they w
-00000b60: 696c 6c20 6265 2073 746f 7261 6765 206f  ill be storage o
-00000b70: 626a 6563 7473 2e20 466f 7220 5333 2074  bjects. For S3 t
-00000b80: 6865 2072 6563 7572 7365 2066 6c61 6720  he recurse flag 
-00000b90: 6973 2069 676e 6f72 6564 2061 6e64 2061  is ignored and a
-00000ba0: 6c6c 0a6f 626a 6563 7473 2077 6974 6820  ll.objects with 
-00000bb0: 6b65 7973 206d 6174 6368 696e 6720 7468  keys matching th
-00000bc0: 6520 7061 7468 2061 7320 6120 7072 6566  e path as a pref
-00000bd0: 6978 2061 7265 2069 6e63 6c75 6465 642e  ix are included.
-00000be0: 0a0a 466f 7220 7379 7374 656d 2074 7970  ..For system typ
-00000bf0: 6573 2074 6861 7420 7375 7070 6f72 7420  es that support 
-00000c00: 6469 7265 6374 6f72 7920 6869 6572 6172  directory hierar
-00000c10: 6368 6965 7320 7468 6520 6d61 7869 6d75  chies the maximu
-00000c20: 6d20 7265 6375 7273 696f 6e20 6465 7074  m recursion dept
-00000c30: 6820 6973 2032 302e 0a0a 4e6f 7465 2074  h is 20...Note t
-00000c40: 6861 7420 5333 2062 7563 6b65 7473 2064  hat S3 buckets d
-00000c50: 6f20 6e6f 7420 6861 7665 2061 2068 6965  o not have a hie
-00000c60: 7261 7263 6869 6361 6c20 7374 7275 6374  rarchical struct
-00000c70: 7572 652e 2054 6865 7265 2061 7265 206e  ure. There are n
-00000c80: 6f20 6469 7265 6374 6f72 6965 732e 2045  o directories. E
-00000c90: 7665 7279 7468 696e 6720 6973 2061 6e20  verything is an 
-00000ca0: 6f62 6a65 6374 0a61 7373 6f63 6961 7465  object.associate
-00000cb0: 6420 7769 7468 2061 206b 6579 2e0a 0a43  d with a key...C
-00000cc0: 6572 7461 696e 2073 6572 7669 6365 7320  ertain services 
-00000cd0: 6d61 7920 7573 6520 7468 6520 7175 6572  may use the quer
-00000ce0: 7920 7061 7261 6d65 7465 7220 2a69 6d70  y parameter *imp
-00000cf0: 6572 736f 6e61 7469 6f6e 4964 2a20 746f  ersonationId* to
-00000d00: 2062 6520 7573 6564 2069 6e20 706c 6163   be used in plac
-00000d10: 6520 6f66 2074 6865 2072 6571 7565 7374  e of the request
-00000d20: 696e 670a 5461 7069 7320 7573 6572 2e20  ing.Tapis user. 
-00000d30: 5461 7069 7320 7769 6c6c 2075 7365 2074  Tapis will use t
-00000d40: 6869 7320 7573 6572 2049 6420 7768 656e  his user Id when
-00000d50: 2070 6572 666f 726d 696e 6720 6175 7468   performing auth
-00000d60: 6f72 697a 6174 696f 6e20 616e 6420 7265  orization and re
-00000d70: 736f 6c76 696e 6720 7468 6520 2a65 6666  solving the *eff
-00000d80: 6563 7469 7665 5573 6572 4964 2a0a 666f  ectiveUserId*.fo
-00000d90: 7220 7468 6520 7379 7374 656d 2e0a 0a43  r the system...C
-00000da0: 6572 7461 696e 2073 6572 7669 6365 7320  ertain services 
-00000db0: 6d61 7920 7573 6520 7468 6520 7175 6572  may use the quer
-00000dc0: 7920 7061 7261 6d65 7465 7220 2a73 6861  y parameter *sha
-00000dd0: 7265 6441 7070 4374 782a 2074 6f20 696e  redAppCtx* to in
-00000de0: 6469 6361 7465 2074 6861 7420 7468 6520  dicate that the 
-00000df0: 7265 7175 6573 7420 6973 2069 6e20 6120  request is in a 
-00000e00: 7368 6172 6564 0a61 7070 6c69 6361 7469  shared.applicati
-00000e10: 6f6e 2063 6f6e 7465 7874 2e20 5461 7069  on context. Tapi
-00000e20: 7320 6175 7468 6f72 697a 6174 696f 6e20  s authorization 
-00000e30: 7769 6c6c 2062 6520 6279 7061 7373 6564  will be bypassed
-00000e40: 2e0a 948c 0b6f 7065 7261 7469 6f6e 4964  .....operationId
-00000e50: 948c 096c 6973 7446 696c 6573 948c 0a70  ...listFiles...p
-00000e60: 6172 616d 6574 6572 7394 5d94 287d 9428  arameters.].(}.(
-00000e70: 8c04 6e61 6d65 948c 0873 7973 7465 6d49  ..name...systemI
-00000e80: 6494 8c02 696e 948c 0470 6174 6894 8c0b  d...in...path...
-00000e90: 6465 7363 7269 7074 696f 6e94 8c09 5379  description...Sy
-00000ea0: 7374 656d 2049 4494 8c08 7265 7175 6972  stem ID...requir
-00000eb0: 6564 9488 8c06 7363 6865 6d61 947d 948c  ed....schema.}..
-00000ec0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-00000ed0: 8c07 6578 616d 706c 6594 8c09 7379 7374  ..example...syst
-00000ee0: 656d 3132 3394 757d 9428 8c04 6e61 6d65  em123.u}.(..name
-00000ef0: 948c 0470 6174 6894 8c02 696e 948c 0470  ...path...in...p
-00000f00: 6174 6894 8c0b 6465 7363 7269 7074 696f  ath...descriptio
-00000f10: 6e94 8c25 5061 7468 2072 656c 6174 6976  n..%Path relativ
-00000f20: 6520 746f 2074 6865 2073 7973 7465 6d20  e to the system 
-00000f30: 2a72 6f6f 7444 6972 2a94 8c08 7265 7175  *rootDir*...requ
-00000f40: 6972 6564 9488 8c06 7363 6865 6d61 947d  ired....schema.}
-00000f50: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-00000f60: 9473 8c07 6578 616d 706c 6594 8c17 2f64  .s..example.../d
-00000f70: 6972 6563 746f 7279 412f 6469 7265 6374  irectoryA/direct
-00000f80: 6f72 7942 2f94 757d 9428 8c04 6e61 6d65  oryB/.u}.(..name
-00000f90: 948c 056c 696d 6974 948c 0269 6e94 8c05  ...limit...in...
-00000fa0: 7175 6572 7994 8c0b 6465 7363 7269 7074  query...descript
-00000fb0: 696f 6e94 8c10 7061 6769 6e61 7469 6f6e  ion...pagination
-00000fc0: 206c 696d 6974 948c 0673 6368 656d 6194   limit...schema.
-00000fd0: 7d94 288c 0474 7970 6594 8c07 696e 7465  }.(..type...inte
-00000fe0: 6765 7294 8c06 666f 726d 6174 948c 0569  ger...format...i
-00000ff0: 6e74 3332 948c 0764 6566 6175 6c74 944d  nt32...default.M
-00001000: e803 758c 0765 7861 6d70 6c65 944b 6475  ..u..example.Kdu
-00001010: 7d94 288c 046e 616d 6594 8c06 6f66 6673  }.(..name...offs
-00001020: 6574 948c 0269 6e94 8c05 7175 6572 7994  et...in...query.
-00001030: 8c0b 6465 7363 7269 7074 696f 6e94 8c11  ..description...
-00001040: 7061 6769 6e61 7469 6f6e 206f 6666 7365  pagination offse
-00001050: 7494 8c06 7363 6865 6d61 947d 9428 8c04  t...schema.}.(..
-00001060: 7479 7065 948c 0769 6e74 6567 6572 948c  type...integer..
-00001070: 0666 6f72 6d61 7494 8c05 696e 7436 3494  .format...int64.
-00001080: 8c07 6465 6661 756c 7494 4b00 758c 0765  ..default.K.u..e
-00001090: 7861 6d70 6c65 944d e803 757d 9428 8c04  xample.M..u}.(..
-000010a0: 6e61 6d65 948c 0772 6563 7572 7365 948c  name...recurse..
-000010b0: 0269 6e94 8c05 7175 6572 7994 8c0b 6465  .in...query...de
-000010c0: 7363 7269 7074 696f 6e94 8c31 5265 6375  scription..1Recu
-000010d0: 7273 6976 6520 6c69 7374 696e 672e 204d  rsive listing. M
-000010e0: 6178 696d 756d 2072 6563 7572 7369 6f6e  aximum recursion
-000010f0: 2064 6570 7468 2069 7320 3230 2e94 8c06   depth is 20....
-00001100: 7363 6865 6d61 947d 9428 8c04 7479 7065  schema.}.(..type
-00001110: 948c 0762 6f6f 6c65 616e 948c 0764 6566  ...boolean...def
-00001120: 6175 6c74 9489 758c 0765 7861 6d70 6c65  ault..u..example
-00001130: 9489 757d 9428 8c04 6e61 6d65 948c 0f69  ..u}.(..name...i
-00001140: 6d70 6572 736f 6e61 7469 6f6e 4964 948c  mpersonationId..
-00001150: 0269 6e94 8c05 7175 6572 7994 8c0b 6465  .in...query...de
-00001160: 7363 7269 7074 696f 6e94 8c3f 5265 7374  scription..?Rest
-00001170: 7269 6374 6564 2e20 4f6e 6c79 2063 6572  ricted. Only cer
-00001180: 7461 696e 2073 6572 7669 6365 7320 6d61  tain services ma
-00001190: 7920 696d 7065 7273 6f6e 6174 6520 6120  y impersonate a 
-000011a0: 5461 7069 7320 7573 6572 2e94 8c06 7363  Tapis user....sc
-000011b0: 6865 6d61 947d 948c 0474 7970 6594 8c06  hema.}...type...
-000011c0: 7374 7269 6e67 9473 757d 9428 8c04 6e61  string.su}.(..na
-000011d0: 6d65 948c 0c73 6861 7265 6441 7070 4374  me...sharedAppCt
-000011e0: 7894 8c02 696e 948c 0571 7565 7279 948c  x...in...query..
-000011f0: 0b64 6573 6372 6970 7469 6f6e 948c 5752  .description..WR
-00001200: 6573 7472 6963 7465 642e 204f 6e6c 7920  estricted. Only 
-00001210: 6365 7274 6169 6e20 7365 7276 6963 6573  certain services
-00001220: 206d 6179 2069 6e64 6963 6174 6520 7468   may indicate th
-00001230: 6174 2074 6865 2072 6571 7565 7374 2069  at the request i
-00001240: 7320 696e 2061 2073 6861 7265 6420 636f  s in a shared co
-00001250: 6e74 6578 742e 948c 0673 6368 656d 6194  ntext....schema.
-00001260: 7d94 288c 0474 7970 6594 8c07 626f 6f6c  }.(..type...bool
-00001270: 6561 6e94 8c07 6465 6661 756c 7494 8975  ean...default..u
-00001280: 7565 8c09 7265 7370 6f6e 7365 7394 7d94  ue..responses.}.
-00001290: 288c 0332 3030 947d 9428 8c0b 6465 7363  (..200.}.(..desc
-000012a0: 7269 7074 696f 6e94 8c0f 4120 6c69 7374  ription...A list
-000012b0: 206f 6620 6669 6c65 7394 8c07 636f 6e74   of files...cont
-000012c0: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
-000012d0: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
-000012e0: 656d 6194 7d94 8c04 2472 6566 948c 2823  ema.}...$ref..(#
-000012f0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-00001300: 6d61 732f 4669 6c65 4c69 7374 696e 6752  mas/FileListingR
-00001310: 6573 706f 6e73 6594 7373 7375 8c03 3430  esponse.sssu..40
-00001320: 3094 7d94 288c 0b64 6573 6372 6970 7469  0.}.(..descripti
-00001330: 6f6e 948c 0b42 6164 2052 6571 7565 7374  on...Bad Request
-00001340: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
-00001350: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
-00001360: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
-00001370: 7265 6694 8c27 232f 636f 6d70 6f6e 656e  ref..'#/componen
-00001380: 7473 2f73 6368 656d 6173 2f46 696c 6553  ts/schemas/FileS
-00001390: 7472 696e 6752 6573 706f 6e73 6594 7373  tringResponse.ss
-000013a0: 7375 8c03 3430 3194 7d94 288c 0b64 6573  su..401.}.(..des
-000013b0: 6372 6970 7469 6f6e 948c 114e 6f74 2041  cription...Not A
-000013c0: 7574 6865 6e74 6963 6174 6564 948c 0763  uthenticated...c
-000013d0: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
-000013e0: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
-000013f0: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
-00001400: 8c27 232f 636f 6d70 6f6e 656e 7473 2f73  .'#/components/s
-00001410: 6368 656d 6173 2f46 696c 6553 7472 696e  chemas/FileStrin
-00001420: 6752 6573 706f 6e73 6594 7373 7375 8c03  gResponse.sssu..
-00001430: 3430 3394 7d94 288c 0b64 6573 6372 6970  403.}.(..descrip
-00001440: 7469 6f6e 948c 1150 6572 6d69 7373 696f  tion...Permissio
-00001450: 6e20 4465 6e69 6564 948c 0763 6f6e 7465  n Denied...conte
-00001460: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
-00001470: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
-00001480: 6d61 947d 948c 0424 7265 6694 8c27 232f  ma.}...$ref..'#/
-00001490: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-000014a0: 6173 2f46 696c 6553 7472 696e 6752 6573  as/FileStringRes
-000014b0: 706f 6e73 6594 7373 7375 8c03 3430 3494  ponse.sssu..404.
-000014c0: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
-000014d0: 948c 094e 6f74 2046 6f75 6e64 948c 0763  ...Not Found...c
-000014e0: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
-000014f0: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
-00001500: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
-00001510: 8c27 232f 636f 6d70 6f6e 656e 7473 2f73  .'#/components/s
-00001520: 6368 656d 6173 2f46 696c 6553 7472 696e  chemas/FileStrin
-00001530: 6752 6573 706f 6e73 6594 7373 7375 8c03  gResponse.sssu..
-00001540: 3530 3094 7d94 288c 0b64 6573 6372 6970  500.}.(..descrip
-00001550: 7469 6f6e 948c 0e49 6e74 6572 6e61 6c20  tion...Internal 
-00001560: 4572 726f 7294 8c07 636f 6e74 656e 7494  Error...content.
-00001570: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
-00001580: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
-00001590: 7d94 8c04 2472 6566 948c 2723 2f63 6f6d  }...$ref..'#/com
-000015a0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-000015b0: 4669 6c65 5374 7269 6e67 5265 7370 6f6e  FileStringRespon
-000015c0: 7365 9473 7373 7575 758c 0370 7574 947d  se.sssuuu..put.}
-000015d0: 9428 8c04 7461 6773 945d 948c 0f46 696c  .(..tags.]...Fil
-000015e0: 6520 4f70 6572 6174 696f 6e73 9461 8c0b  e Operations.a..
-000015f0: 6465 7363 7269 7074 696f 6e94 8c7a 4d6f  description..zMo
-00001600: 7665 206f 7220 636f 7079 2061 2066 696c  ve or copy a fil
-00001610: 652c 2064 6972 6563 746f 7279 206f 7220  e, directory or 
-00001620: 6f62 6a65 6374 206f 6e20 7b73 7973 7465  object on {syste
-00001630: 6d49 447d 2061 7420 7061 7468 207b 7061  mID} at path {pa
-00001640: 7468 7d2e 204e 6f74 2061 6c6c 206f 7065  th}. Not all ope
-00001650: 7261 7469 6f6e 7320 7375 7070 6f72 7465  rations supporte
-00001660: 6420 666f 7220 616c 6c0a 7379 7374 656d  d for all.system
-00001670: 2074 7970 6573 2e0a 948c 0b6f 7065 7261   types.....opera
-00001680: 7469 6f6e 4964 948c 086d 6f76 6543 6f70  tionId...moveCop
-00001690: 7994 8c0a 7061 7261 6d65 7465 7273 945d  y...parameters.]
-000016a0: 9428 7d94 288c 046e 616d 6594 8c08 7379  .(}.(..name...sy
-000016b0: 7374 656d 4964 948c 0269 6e94 8c04 7061  stemId...in...pa
-000016c0: 7468 948c 0b64 6573 6372 6970 7469 6f6e  th...description
-000016d0: 948c 0953 7973 7465 6d20 4944 948c 0872  ...System ID...r
-000016e0: 6571 7569 7265 6494 888c 0673 6368 656d  equired....schem
-000016f0: 6194 7d94 8c04 7479 7065 948c 0673 7472  a.}...type...str
-00001700: 696e 6794 7375 7d94 288c 046e 616d 6594  ing.su}.(..name.
-00001710: 8c04 7061 7468 948c 0269 6e94 8c04 7061  ..path...in...pa
-00001720: 7468 948c 0b64 6573 6372 6970 7469 6f6e  th...description
-00001730: 948c 2550 6174 6820 7265 6c61 7469 7665  ..%Path relative
-00001740: 2074 6f20 7468 6520 7379 7374 656d 202a   to the system *
-00001750: 726f 6f74 4469 722a 948c 0872 6571 7569  rootDir*...requi
-00001760: 7265 6494 888c 0673 6368 656d 6194 7d94  red....schema.}.
-00001770: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-00001780: 7375 658c 0b72 6571 7565 7374 426f 6479  sue..requestBody
-00001790: 947d 948c 0763 6f6e 7465 6e74 947d 948c  .}...content.}..
-000017a0: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
-000017b0: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
-000017c0: 0424 7265 6694 8c24 232f 636f 6d70 6f6e  .$ref..$#/compon
-000017d0: 656e 7473 2f73 6368 656d 6173 2f4d 6f76  ents/schemas/Mov
-000017e0: 6543 6f70 7952 6571 7565 7374 9473 7373  eCopyRequest.sss
-000017f0: 738c 0972 6573 706f 6e73 6573 947d 9428  s..responses.}.(
-00001800: 8c03 3230 3094 7d94 288c 0b64 6573 6372  ..200.}.(..descr
-00001810: 6970 7469 6f6e 948c 024f 4b94 8c07 636f  iption...OK...co
-00001820: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
-00001830: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
-00001840: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
-00001850: 2723 2f63 6f6d 706f 6e65 6e74 732f 7363  '#/components/sc
-00001860: 6865 6d61 732f 4669 6c65 5374 7269 6e67  hemas/FileString
-00001870: 5265 7370 6f6e 7365 9473 7373 758c 0334  Response.sssu..4
-00001880: 3030 947d 9428 8c0b 6465 7363 7269 7074  00.}.(..descript
-00001890: 696f 6e94 8c0b 4261 6420 5265 7175 6573  ion...Bad Reques
-000018a0: 7494 8c07 636f 6e74 656e 7494 7d94 8c10  t...content.}...
-000018b0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-000018c0: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
-000018d0: 2472 6566 948c 2723 2f63 6f6d 706f 6e65  $ref..'#/compone
-000018e0: 6e74 732f 7363 6865 6d61 732f 4669 6c65  nts/schemas/File
-000018f0: 5374 7269 6e67 5265 7370 6f6e 7365 9473  StringResponse.s
-00001900: 7373 758c 0334 3031 947d 9428 8c0b 6465  ssu..401.}.(..de
-00001910: 7363 7269 7074 696f 6e94 8c11 4e6f 7420  scription...Not 
-00001920: 4175 7468 656e 7469 6361 7465 6494 8c07  Authenticated...
-00001930: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
-00001940: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
-00001950: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
-00001960: 948c 2723 2f63 6f6d 706f 6e65 6e74 732f  ..'#/components/
-00001970: 7363 6865 6d61 732f 4669 6c65 5374 7269  schemas/FileStri
-00001980: 6e67 5265 7370 6f6e 7365 9473 7373 758c  ngResponse.sssu.
-00001990: 0334 3033 947d 9428 8c0b 6465 7363 7269  .403.}.(..descri
-000019a0: 7074 696f 6e94 8c11 5065 726d 6973 7369  ption...Permissi
-000019b0: 6f6e 2044 656e 6965 6494 8c07 636f 6e74  on Denied...cont
-000019c0: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
-000019d0: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
-000019e0: 656d 6194 7d94 8c04 2472 6566 948c 2723  ema.}...$ref..'#
-000019f0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-00001a00: 6d61 732f 4669 6c65 5374 7269 6e67 5265  mas/FileStringRe
-00001a10: 7370 6f6e 7365 9473 7373 758c 0334 3034  sponse.sssu..404
-00001a20: 947d 9428 8c0b 6465 7363 7269 7074 696f  .}.(..descriptio
-00001a30: 6e94 8c09 4e6f 7420 466f 756e 6494 8c07  n...Not Found...
-00001a40: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
-00001a50: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
-00001a60: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
-00001a70: 948c 2723 2f63 6f6d 706f 6e65 6e74 732f  ..'#/components/
-00001a80: 7363 6865 6d61 732f 4669 6c65 5374 7269  schemas/FileStri
-00001a90: 6e67 5265 7370 6f6e 7365 9473 7373 758c  ngResponse.sssu.
-00001aa0: 0335 3030 947d 9428 8c0b 6465 7363 7269  .500.}.(..descri
-00001ab0: 7074 696f 6e94 8c0e 496e 7465 726e 616c  ption...Internal
-00001ac0: 2045 7272 6f72 948c 0763 6f6e 7465 6e74   Error...content
-00001ad0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
-00001ae0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
-00001af0: 947d 948c 0424 7265 6694 8c27 232f 636f  .}...$ref..'#/co
-00001b00: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-00001b10: 2f46 696c 6553 7472 696e 6752 6573 706f  /FileStringRespo
-00001b20: 6e73 6594 7373 7375 7575 8c04 706f 7374  nse.sssuuu..post
-00001b30: 947d 9428 8c04 7461 6773 945d 948c 0f46  .}.(..tags.]...F
-00001b40: 696c 6520 4f70 6572 6174 696f 6e73 9461  ile Operations.a
-00001b50: 8c0b 6465 7363 7269 7074 696f 6e94 8c54  ..description..T
-00001b60: 5468 6520 6669 6c65 206f 7220 6f62 6a65  The file or obje
-00001b70: 6374 2077 696c 6c20 6265 2075 706c 6f61  ct will be uploa
-00001b80: 6465 6420 6174 2074 6865 207b 7061 7468  ded at the {path
-00001b90: 7d20 696e 6465 7065 6e64 656e 7420 6f66  } independent of
-00001ba0: 2074 6865 206f 7269 6769 6e61 6c20 6e61   the original na
-00001bb0: 6d65 2e0a 948c 0b6f 7065 7261 7469 6f6e  me.....operation
-00001bc0: 4964 948c 0669 6e73 6572 7494 8c0a 7061  Id...insert...pa
-00001bd0: 7261 6d65 7465 7273 945d 9428 7d94 288c  rameters.].(}.(.
-00001be0: 046e 616d 6594 8c08 7379 7374 656d 4964  .name...systemId
-00001bf0: 948c 0269 6e94 8c04 7061 7468 948c 0b64  ...in...path...d
-00001c00: 6573 6372 6970 7469 6f6e 948c 0953 7973  escription...Sys
-00001c10: 7465 6d20 4944 948c 0872 6571 7569 7265  tem ID...require
-00001c20: 6494 888c 0673 6368 656d 6194 7d94 8c04  d....schema.}...
-00001c30: 7479 7065 948c 0673 7472 696e 6794 7375  type...string.su
-00001c40: 7d94 288c 046e 616d 6594 8c04 7061 7468  }.(..name...path
-00001c50: 948c 0269 6e94 8c04 7061 7468 948c 0b64  ...in...path...d
-00001c60: 6573 6372 6970 7469 6f6e 948c 2550 6174  escription..%Pat
-00001c70: 6820 7265 6c61 7469 7665 2074 6f20 7468  h relative to th
-00001c80: 6520 7379 7374 656d 202a 726f 6f74 4469  e system *rootDi
-00001c90: 722a 948c 0872 6571 7569 7265 6494 888c  r*...required...
-00001ca0: 0673 6368 656d 6194 7d94 8c04 7479 7065  .schema.}...type
-00001cb0: 948c 0673 7472 696e 6794 7375 658c 0b72  ...string.sue..r
-00001cc0: 6571 7565 7374 426f 6479 947d 948c 0763  equestBody.}...c
-00001cd0: 6f6e 7465 6e74 947d 948c 136d 756c 7469  ontent.}...multi
-00001ce0: 7061 7274 2f66 6f72 6d2d 6461 7461 947d  part/form-data.}
-00001cf0: 948c 0673 6368 656d 6194 7d94 288c 0872  ...schema.}.(..r
-00001d00: 6571 7569 7265 6494 5d94 8c04 6669 6c65  equired.]...file
-00001d10: 9461 8c04 7479 7065 948c 066f 626a 6563  .a..type...objec
-00001d20: 7494 8c0a 7072 6f70 6572 7469 6573 947d  t...properties.}
-00001d30: 948c 0466 696c 6594 7d94 288c 0474 7970  ...file.}.(..typ
-00001d40: 6594 8c06 7374 7269 6e67 948c 0666 6f72  e...string...for
-00001d50: 6d61 7494 8c06 6269 6e61 7279 9475 7375  mat...binary.usu
-00001d60: 7373 738c 0972 6573 706f 6e73 6573 947d  sss..responses.}
-00001d70: 9428 8c03 3230 3094 7d94 288c 0b64 6573  .(..200.}.(..des
-00001d80: 6372 6970 7469 6f6e 948c 024f 4b94 8c07  cription...OK...
-00001d90: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
-00001da0: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
-00001db0: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
-00001dc0: 948c 2723 2f63 6f6d 706f 6e65 6e74 732f  ..'#/components/
-00001dd0: 7363 6865 6d61 732f 4669 6c65 5374 7269  schemas/FileStri
-00001de0: 6e67 5265 7370 6f6e 7365 9473 7373 758c  ngResponse.sssu.
-00001df0: 0334 3030 947d 9428 8c0b 6465 7363 7269  .400.}.(..descri
-00001e00: 7074 696f 6e94 8c0b 4261 6420 5265 7175  ption...Bad Requ
-00001e10: 6573 7494 8c07 636f 6e74 656e 7494 7d94  est...content.}.
-00001e20: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
-00001e30: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
-00001e40: 8c04 2472 6566 948c 2723 2f63 6f6d 706f  ..$ref..'#/compo
-00001e50: 6e65 6e74 732f 7363 6865 6d61 732f 4669  nents/schemas/Fi
-00001e60: 6c65 5374 7269 6e67 5265 7370 6f6e 7365  leStringResponse
-00001e70: 9473 7373 758c 0334 3031 947d 9428 8c0b  .sssu..401.}.(..
-00001e80: 6465 7363 7269 7074 696f 6e94 8c11 4e6f  description...No
-00001e90: 7420 4175 7468 656e 7469 6361 7465 6494  t Authenticated.
-00001ea0: 8c07 636f 6e74 656e 7494 7d94 8c10 6170  ..content.}...ap
-00001eb0: 706c 6963 6174 696f 6e2f 6a73 6f6e 947d  plication/json.}
-00001ec0: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
-00001ed0: 6566 948c 2723 2f63 6f6d 706f 6e65 6e74  ef..'#/component
-00001ee0: 732f 7363 6865 6d61 732f 4669 6c65 5374  s/schemas/FileSt
-00001ef0: 7269 6e67 5265 7370 6f6e 7365 9473 7373  ringResponse.sss
-00001f00: 758c 0334 3033 947d 9428 8c0b 6465 7363  u..403.}.(..desc
-00001f10: 7269 7074 696f 6e94 8c11 5065 726d 6973  ription...Permis
-00001f20: 7369 6f6e 2044 656e 6965 6494 8c07 636f  sion Denied...co
-00001f30: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
-00001f40: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
-00001f50: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
-00001f60: 2723 2f63 6f6d 706f 6e65 6e74 732f 7363  '#/components/sc
-00001f70: 6865 6d61 732f 4669 6c65 5374 7269 6e67  hemas/FileString
-00001f80: 5265 7370 6f6e 7365 9473 7373 758c 0335  Response.sssu..5
-00001f90: 3030 947d 9428 8c0b 6465 7363 7269 7074  00.}.(..descript
-00001fa0: 696f 6e94 8c0e 496e 7465 726e 616c 2045  ion...Internal E
-00001fb0: 7272 6f72 948c 0763 6f6e 7465 6e74 947d  rror...content.}
-00001fc0: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
-00001fd0: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
-00001fe0: 948c 0424 7265 6694 8c27 232f 636f 6d70  ...$ref..'#/comp
-00001ff0: 6f6e 656e 7473 2f73 6368 656d 6173 2f46  onents/schemas/F
-00002000: 696c 6553 7472 696e 6752 6573 706f 6e73  ileStringRespons
-00002010: 6594 7373 7375 7575 8c06 6465 6c65 7465  e.sssuuu..delete
-00002020: 947d 9428 8c04 7461 6773 945d 948c 0f46  .}.(..tags.]...F
-00002030: 696c 6520 4f70 6572 6174 696f 6e73 9461  ile Operations.a
-00002040: 8c0b 6465 7363 7269 7074 696f 6e94 581b  ..description.X.
-00002050: 0200 0044 656c 6574 6520 6120 6669 6c65  ...Delete a file
-00002060: 2c20 6469 7265 6374 6f72 7920 6f72 206f  , directory or o
-00002070: 626a 6563 7420 6f6e 207b 7379 7374 656d  bject on {system
-00002080: 4944 7d20 6174 2070 6174 6820 7b70 6174  ID} at path {pat
-00002090: 687d 2e0a 0a46 6f72 2061 204c 494e 5558  h}...For a LINUX
-000020a0: 2064 6972 6563 746f 7279 2074 6869 7320   directory this 
-000020b0: 7769 6c6c 2062 6520 6120 7265 6375 7273  will be a recurs
-000020c0: 6976 6520 6465 6c65 7465 2e0a 0a46 6f72  ive delete...For
-000020d0: 2061 6e20 5333 2073 7973 7465 6d2c 2074   an S3 system, t
-000020e0: 6865 2070 6174 6820 7769 6c6c 2072 6570  he path will rep
-000020f0: 7265 7365 6e74 2065 6974 6865 7220 6120  resent either a 
-00002100: 7369 6e67 6c65 206f 626a 6563 7420 6f72  single object or
-00002110: 2061 6c6c 206f 626a 6563 7473 2069 6e20   all objects in 
-00002120: 7468 6520 6275 636b 6574 2077 6974 6820  the bucket with 
-00002130: 6120 7072 6566 6978 0a6d 6174 6368 696e  a prefix.matchin
-00002140: 6720 7468 6520 7379 7374 656d 202a 726f  g the system *ro
-00002150: 6f74 4469 722a 2069 6620 7468 6520 7061  otDir* if the pa
-00002160: 7468 2069 7320 7468 6520 656d 7074 7920  th is the empty 
-00002170: 7374 7269 6e67 2e0a 0a2a 2a57 4152 4e49  string...**WARNI
-00002180: 4e47 2a2a 2046 6f72 2061 6e20 5333 2073  NG** For an S3 s
-00002190: 7973 7465 6d20 6966 2074 6865 2070 6174  ystem if the pat
-000021a0: 6820 6973 2074 6865 2065 6d70 7479 2073  h is the empty s
-000021b0: 7472 696e 672c 2074 6865 6e20 616c 6c20  tring, then all 
-000021c0: 6f62 6a65 6374 7320 696e 2074 6865 2062  objects in the b
-000021d0: 7563 6b65 7420 7769 7468 2061 206b 6579  ucket with a key
-000021e0: 206d 6174 6368 696e 670a 7468 6520 7072   matching.the pr
-000021f0: 6566 6978 202a 726f 6f74 4469 722a 2077  efix *rootDir* w
-00002200: 696c 6c20 6265 2064 656c 6574 6564 2e20  ill be deleted. 
-00002210: 536f 2069 6620 7468 6520 2a72 6f6f 7444  So if the *rootD
-00002220: 6972 2a20 6973 2061 6c73 6f20 7468 6520  ir* is also the 
-00002230: 656d 7074 7920 7374 7269 6e67 2c20 7468  empty string, th
-00002240: 656e 2061 6c6c 206f 626a 6563 7473 2069  en all objects i
-00002250: 6e20 7468 6520 6275 636b 6574 0a77 696c  n the bucket.wil
-00002260: 6c20 6265 2072 656d 6f76 6564 2e0a 948c  l be removed....
-00002270: 0b6f 7065 7261 7469 6f6e 4964 948c 0664  .operationId...d
-00002280: 656c 6574 6594 8c0a 7061 7261 6d65 7465  elete...paramete
-00002290: 7273 945d 9428 7d94 288c 046e 616d 6594  rs.].(}.(..name.
-000022a0: 8c08 7379 7374 656d 4964 948c 0269 6e94  ..systemId...in.
-000022b0: 8c04 7061 7468 948c 0b64 6573 6372 6970  ..path...descrip
-000022c0: 7469 6f6e 948c 0953 7973 7465 6d20 4944  tion...System ID
-000022d0: 948c 0872 6571 7569 7265 6494 888c 0673  ...required....s
-000022e0: 6368 656d 6194 7d94 8c04 7479 7065 948c  chema.}...type..
-000022f0: 0673 7472 696e 6794 7375 7d94 288c 046e  .string.su}.(..n
-00002300: 616d 6594 8c04 7061 7468 948c 0269 6e94  ame...path...in.
-00002310: 8c04 7061 7468 948c 0b64 6573 6372 6970  ..path...descrip
-00002320: 7469 6f6e 948c 2550 6174 6820 7265 6c61  tion..%Path rela
-00002330: 7469 7665 2074 6f20 7468 6520 7379 7374  tive to the syst
-00002340: 656d 202a 726f 6f74 4469 722a 948c 0872  em *rootDir*...r
-00002350: 6571 7569 7265 6494 888c 0673 6368 656d  equired....schem
-00002360: 6194 7d94 8c04 7479 7065 948c 0673 7472  a.}...type...str
-00002370: 696e 6794 7375 658c 0972 6573 706f 6e73  ing.sue..respons
-00002380: 6573 947d 9428 8c03 3230 3094 7d94 288c  es.}.(..200.}.(.
-00002390: 0b64 6573 6372 6970 7469 6f6e 948c 024f  .description...O
-000023a0: 4b94 8c07 636f 6e74 656e 7494 7d94 8c10  K...content.}...
-000023b0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-000023c0: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
-000023d0: 2472 6566 948c 2723 2f63 6f6d 706f 6e65  $ref..'#/compone
-000023e0: 6e74 732f 7363 6865 6d61 732f 4669 6c65  nts/schemas/File
-000023f0: 5374 7269 6e67 5265 7370 6f6e 7365 9473  StringResponse.s
-00002400: 7373 758c 0334 3030 947d 9428 8c0b 6465  ssu..400.}.(..de
-00002410: 7363 7269 7074 696f 6e94 8c0b 4261 6420  scription...Bad 
-00002420: 5265 7175 6573 7494 8c07 636f 6e74 656e  Request...conten
-00002430: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
-00002440: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
-00002450: 6194 7d94 8c04 2472 6566 948c 2723 2f63  a.}...$ref..'#/c
-00002460: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
-00002470: 732f 4669 6c65 5374 7269 6e67 5265 7370  s/FileStringResp
-00002480: 6f6e 7365 9473 7373 758c 0334 3031 947d  onse.sssu..401.}
-00002490: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
-000024a0: 8c11 4e6f 7420 4175 7468 656e 7469 6361  ..Not Authentica
-000024b0: 7465 6494 8c07 636f 6e74 656e 7494 7d94  ted...content.}.
-000024c0: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
-000024d0: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
-000024e0: 8c04 2472 6566 948c 2723 2f63 6f6d 706f  ..$ref..'#/compo
-000024f0: 6e65 6e74 732f 7363 6865 6d61 732f 4669  nents/schemas/Fi
-00002500: 6c65 5374 7269 6e67 5265 7370 6f6e 7365  leStringResponse
-00002510: 9473 7373 758c 0334 3033 947d 9428 8c0b  .sssu..403.}.(..
-00002520: 6465 7363 7269 7074 696f 6e94 8c11 5065  description...Pe
-00002530: 726d 6973 7369 6f6e 2044 656e 6965 6494  rmission Denied.
-00002540: 8c07 636f 6e74 656e 7494 7d94 8c10 6170  ..content.}...ap
-00002550: 706c 6963 6174 696f 6e2f 6a73 6f6e 947d  plication/json.}
-00002560: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
-00002570: 6566 948c 2723 2f63 6f6d 706f 6e65 6e74  ef..'#/component
-00002580: 732f 7363 6865 6d61 732f 4669 6c65 5374  s/schemas/FileSt
-00002590: 7269 6e67 5265 7370 6f6e 7365 9473 7373  ringResponse.sss
-000025a0: 758c 0334 3034 947d 9428 8c0b 6465 7363  u..404.}.(..desc
-000025b0: 7269 7074 696f 6e94 8c09 4e6f 7420 466f  ription...Not Fo
-000025c0: 756e 6494 8c07 636f 6e74 656e 7494 7d94  und...content.}.
-000025d0: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
-000025e0: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
-000025f0: 8c04 2472 6566 948c 2723 2f63 6f6d 706f  ..$ref..'#/compo
-00002600: 6e65 6e74 732f 7363 6865 6d61 732f 4669  nents/schemas/Fi
-00002610: 6c65 5374 7269 6e67 5265 7370 6f6e 7365  leStringResponse
-00002620: 9473 7373 758c 0335 3030 947d 9428 8c0b  .sssu..500.}.(..
-00002630: 6465 7363 7269 7074 696f 6e94 8c0e 496e  description...In
-00002640: 7465 726e 616c 2045 7272 6f72 948c 0763  ternal Error...c
-00002650: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
-00002660: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
-00002670: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
-00002680: 8c27 232f 636f 6d70 6f6e 656e 7473 2f73  .'#/components/s
-00002690: 6368 656d 6173 2f46 696c 6553 7472 696e  chemas/FileStrin
-000026a0: 6752 6573 706f 6e73 6594 7373 7375 7575  gResponse.sssuuu
-000026b0: 758c 182f 7633 2f66 696c 6573 2f6f 7073  u../v3/files/ops
-000026c0: 2f7b 7379 7374 656d 4964 7d94 7d94 8c04  /{systemId}.}...
-000026d0: 706f 7374 947d 9428 8c04 7461 6773 945d  post.}.(..tags.]
-000026e0: 948c 0f46 696c 6520 4f70 6572 6174 696f  ...File Operatio
-000026f0: 6e73 9461 8c0b 6465 7363 7269 7074 696f  ns.a..descriptio
-00002700: 6e94 5831 0100 0043 7265 6174 6520 6120  n.X1...Create a 
-00002710: 6469 7265 6374 6f72 7920 6f6e 2074 6865  directory on the
-00002720: 2073 7973 7465 6d20 6174 2074 6865 2067   system at the g
-00002730: 6976 656e 2070 6174 682e 204e 6f74 2073  iven path. Not s
-00002740: 7570 706f 7274 6564 2066 6f72 2061 6c6c  upported for all
-00002750: 2073 7973 7465 6d20 7479 7065 732e 2043   system types. C
-00002760: 7572 7265 6e74 6c79 2073 7570 706f 7274  urrently support
-00002770: 6564 0a66 6f72 204c 494e 5558 2061 6e64  ed.for LINUX and
-00002780: 2049 524f 4453 2074 7970 6520 7379 7374   IRODS type syst
-00002790: 656d 732e 0a43 6572 7461 696e 2073 6572  ems..Certain ser
-000027a0: 7669 6365 7320 6d61 7920 7573 6520 7468  vices may use th
-000027b0: 6520 7175 6572 7920 7061 7261 6d65 7465  e query paramete
-000027c0: 7220 2a73 6861 7265 6441 7070 4374 782a  r *sharedAppCtx*
-000027d0: 2074 6f20 696e 6469 6361 7465 2074 6861   to indicate tha
-000027e0: 7420 7468 6520 7265 7175 6573 7420 6973  t the request is
-000027f0: 2069 6e20 6120 7368 6172 6564 0a61 7070   in a shared.app
-00002800: 6c69 6361 7469 6f6e 2063 6f6e 7465 7874  lication context
-00002810: 2e20 5461 7069 7320 6175 7468 6f72 697a  . Tapis authoriz
-00002820: 6174 696f 6e20 7769 6c6c 2062 6520 6279  ation will be by
-00002830: 7061 7373 6564 2e0a 948c 0b6f 7065 7261  passed.....opera
-00002840: 7469 6f6e 4964 948c 056d 6b64 6972 948c  tionId...mkdir..
-00002850: 0a70 6172 616d 6574 6572 7394 5d94 287d  .parameters.].(}
-00002860: 9428 8c04 6e61 6d65 948c 0873 7973 7465  .(..name...syste
-00002870: 6d49 6494 8c02 696e 948c 0470 6174 6894  mId...in...path.
-00002880: 8c0b 6465 7363 7269 7074 696f 6e94 8c09  ..description...
-00002890: 5379 7374 656d 2049 4494 8c08 7265 7175  System ID...requ
-000028a0: 6972 6564 9488 8c06 7363 6865 6d61 947d  ired....schema.}
-000028b0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-000028c0: 9473 757d 9428 8c04 6e61 6d65 948c 0c73  .su}.(..name...s
-000028d0: 6861 7265 6441 7070 4374 7894 8c02 696e  haredAppCtx...in
-000028e0: 948c 0571 7565 7279 948c 0b64 6573 6372  ...query...descr
-000028f0: 6970 7469 6f6e 948c 5752 6573 7472 6963  iption..WRestric
-00002900: 7465 642e 204f 6e6c 7920 6365 7274 6169  ted. Only certai
-00002910: 6e20 7365 7276 6963 6573 206d 6179 2069  n services may i
-00002920: 6e64 6963 6174 6520 7468 6174 2074 6865  ndicate that the
-00002930: 2072 6571 7565 7374 2069 7320 696e 2061   request is in a
-00002940: 2073 6861 7265 6420 636f 6e74 6578 742e   shared context.
-00002950: 948c 0673 6368 656d 6194 7d94 288c 0474  ...schema.}.(..t
-00002960: 7970 6594 8c07 626f 6f6c 6561 6e94 8c07  ype...boolean...
-00002970: 6465 6661 756c 7494 8975 7565 8c0b 7265  default..uue..re
-00002980: 7175 6573 7442 6f64 7994 7d94 8c07 636f  questBody.}...co
-00002990: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
-000029a0: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
-000029b0: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
-000029c0: 2123 2f63 6f6d 706f 6e65 6e74 732f 7363  !#/components/sc
-000029d0: 6865 6d61 732f 4d6b 6469 7252 6571 7565  hemas/MkdirReque
-000029e0: 7374 9473 7373 738c 0972 6573 706f 6e73  st.ssss..respons
-000029f0: 6573 947d 9428 8c03 3230 3094 7d94 288c  es.}.(..200.}.(.
-00002a00: 0b64 6573 6372 6970 7469 6f6e 948c 024f  .description...O
-00002a10: 4b94 8c07 636f 6e74 656e 7494 7d94 8c10  K...content.}...
-00002a20: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-00002a30: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
-00002a40: 2472 6566 948c 2723 2f63 6f6d 706f 6e65  $ref..'#/compone
-00002a50: 6e74 732f 7363 6865 6d61 732f 4669 6c65  nts/schemas/File
-00002a60: 5374 7269 6e67 5265 7370 6f6e 7365 9473  StringResponse.s
-00002a70: 7373 758c 0334 3030 947d 9428 8c0b 6465  ssu..400.}.(..de
-00002a80: 7363 7269 7074 696f 6e94 8c0b 4261 6420  scription...Bad 
-00002a90: 5265 7175 6573 7494 8c07 636f 6e74 656e  Request...conten
-00002aa0: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
-00002ab0: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
-00002ac0: 6194 7d94 8c04 2472 6566 948c 2723 2f63  a.}...$ref..'#/c
-00002ad0: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
-00002ae0: 732f 4669 6c65 5374 7269 6e67 5265 7370  s/FileStringResp
-00002af0: 6f6e 7365 9473 7373 758c 0334 3031 947d  onse.sssu..401.}
-00002b00: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
-00002b10: 8c11 4e6f 7420 4175 7468 656e 7469 6361  ..Not Authentica
-00002b20: 7465 6494 8c07 636f 6e74 656e 7494 7d94  ted...content.}.
-00002b30: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
-00002b40: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
-00002b50: 8c04 2472 6566 948c 2723 2f63 6f6d 706f  ..$ref..'#/compo
-00002b60: 6e65 6e74 732f 7363 6865 6d61 732f 4669  nents/schemas/Fi
-00002b70: 6c65 5374 7269 6e67 5265 7370 6f6e 7365  leStringResponse
-00002b80: 9473 7373 758c 0334 3033 947d 9428 8c0b  .sssu..403.}.(..
-00002b90: 6465 7363 7269 7074 696f 6e94 8c11 5065  description...Pe
-00002ba0: 726d 6973 7369 6f6e 2044 656e 6965 6494  rmission Denied.
-00002bb0: 8c07 636f 6e74 656e 7494 7d94 8c10 6170  ..content.}...ap
-00002bc0: 706c 6963 6174 696f 6e2f 6a73 6f6e 947d  plication/json.}
-00002bd0: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
-00002be0: 6566 948c 2723 2f63 6f6d 706f 6e65 6e74  ef..'#/component
-00002bf0: 732f 7363 6865 6d61 732f 4669 6c65 5374  s/schemas/FileSt
-00002c00: 7269 6e67 5265 7370 6f6e 7365 9473 7373  ringResponse.sss
-00002c10: 758c 0335 3030 947d 9428 8c0b 6465 7363  u..500.}.(..desc
-00002c20: 7269 7074 696f 6e94 8c0e 496e 7465 726e  ription...Intern
-00002c30: 616c 2045 7272 6f72 948c 0763 6f6e 7465  al Error...conte
-00002c40: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
-00002c50: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
-00002c60: 6d61 947d 948c 0424 7265 6694 8c27 232f  ma.}...$ref..'#/
-00002c70: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-00002c80: 6173 2f46 696c 6553 7472 696e 6752 6573  as/FileStringRes
-00002c90: 706f 6e73 6594 7373 7375 7575 738c 272f  ponse.sssuuus.'/
-00002ca0: 7633 2f66 696c 6573 2f75 7469 6c73 2f6c  v3/files/utils/l
-00002cb0: 696e 7578 2f7b 7379 7374 656d 4964 7d2f  inux/{systemId}/
-00002cc0: 7b70 6174 687d 947d 9428 8c03 6765 7494  {path}.}.(..get.
-00002cd0: 7d94 288c 0474 6167 7394 5d94 8c0f 4669  }.(..tags.]...Fi
-00002ce0: 6c65 204f 7065 7261 7469 6f6e 7394 618c  le Operations.a.
-00002cf0: 0b64 6573 6372 6970 7469 6f6e 948c 5047  .description..PG
-00002d00: 6574 206e 6174 6976 6520 7374 6174 2069  et native stat i
-00002d10: 6e66 6f72 6d61 7469 6f6e 2066 6f72 2061  nformation for a
-00002d20: 2066 696c 6520 6f72 2064 6972 6563 746f   file or directo
-00002d30: 7279 2066 6f72 2061 2073 7973 7465 6d20  ry for a system 
-00002d40: 6f66 2074 7970 6520 4c49 4e55 582e 0a94  of type LINUX...
-00002d50: 8c0b 6f70 6572 6174 696f 6e49 6494 8c0b  ..operationId...
-00002d60: 6765 7453 7461 7449 6e66 6f94 8c0a 7061  getStatInfo...pa
-00002d70: 7261 6d65 7465 7273 945d 9428 7d94 288c  rameters.].(}.(.
-00002d80: 046e 616d 6594 8c08 7379 7374 656d 4964  .name...systemId
-00002d90: 948c 0269 6e94 8c04 7061 7468 948c 0b64  ...in...path...d
-00002da0: 6573 6372 6970 7469 6f6e 948c 0953 7973  escription...Sys
-00002db0: 7465 6d20 4944 948c 0872 6571 7569 7265  tem ID...require
-00002dc0: 6494 888c 0673 6368 656d 6194 7d94 8c04  d....schema.}...
-00002dd0: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-00002de0: 0765 7861 6d70 6c65 948c 0973 7973 7465  .example...syste
-00002df0: 6d31 3233 9475 7d94 288c 046e 616d 6594  m123.u}.(..name.
-00002e00: 8c04 7061 7468 948c 0269 6e94 8c04 7061  ..path...in...pa
-00002e10: 7468 948c 0b64 6573 6372 6970 7469 6f6e  th...description
-00002e20: 948c 2550 6174 6820 7265 6c61 7469 7665  ..%Path relative
-00002e30: 2074 6f20 7468 6520 7379 7374 656d 202a   to the system *
-00002e40: 726f 6f74 4469 722a 948c 0872 6571 7569  rootDir*...requi
-00002e50: 7265 6494 888c 0673 6368 656d 6194 7d94  red....schema.}.
-00002e60: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-00002e70: 738c 0765 7861 6d70 6c65 948c 112f 6469  s..example.../di
-00002e80: 7265 6374 6f72 7941 2f66 696c 6531 9475  rectoryA/file1.u
-00002e90: 7d94 288c 046e 616d 6594 8c0b 666f 6c6c  }.(..name...foll
-00002ea0: 6f77 4c69 6e6b 7394 8c02 696e 948c 0571  owLinks...in...q
-00002eb0: 7565 7279 948c 0b64 6573 6372 6970 7469  uery...descripti
-00002ec0: 6f6e 948c 6857 6865 6e20 7061 7468 2069  on..hWhen path i
-00002ed0: 7320 6120 7379 6d62 6f6c 6963 206c 696e  s a symbolic lin
-00002ee0: 6b20 7768 6574 6865 7220 746f 2067 6574  k whether to get
-00002ef0: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
-00002f00: 7574 2074 6865 206c 696e 6b20 2866 616c  ut the link (fal
-00002f10: 7365 2920 6f72 2074 6865 206c 696e 6b20  se) or the link 
-00002f20: 7461 7267 6574 2028 7472 7565 2994 8c06  target (true)...
-00002f30: 7363 6865 6d61 947d 9428 8c04 7479 7065  schema.}.(..type
-00002f40: 948c 0762 6f6f 6c65 616e 948c 0764 6566  ...boolean...def
-00002f50: 6175 6c74 9489 758c 0765 7861 6d70 6c65  ault..u..example
-00002f60: 9488 7565 8c09 7265 7370 6f6e 7365 7394  ..ue..responses.
-00002f70: 7d94 288c 0332 3030 947d 9428 8c0b 6465  }.(..200.}.(..de
-00002f80: 7363 7269 7074 696f 6e94 8c31 4c69 6e75  scription..1Linu
-00002f90: 7820 7374 6174 2069 6e66 6f72 6d61 7469  x stat informati
-00002fa0: 6f6e 2066 6f72 2074 6865 2066 696c 6520  on for the file 
-00002fb0: 6f72 2064 6972 6563 746f 7279 2e94 8c07  or directory....
-00002fc0: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
-00002fd0: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
-00002fe0: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
-00002ff0: 948c 2923 2f63 6f6d 706f 6e65 6e74 732f  ..)#/components/
-00003000: 7363 6865 6d61 732f 4669 6c65 5374 6174  schemas/FileStat
-00003010: 496e 666f 5265 7370 6f6e 7365 9473 7373  InfoResponse.sss
-00003020: 758c 0334 3030 947d 9428 8c0b 6465 7363  u..400.}.(..desc
-00003030: 7269 7074 696f 6e94 8c0b 4261 6420 5265  ription...Bad Re
-00003040: 7175 6573 7494 8c07 636f 6e74 656e 7494  quest...content.
-00003050: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
-00003060: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
-00003070: 7d94 8c04 2472 6566 948c 2723 2f63 6f6d  }...$ref..'#/com
-00003080: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-00003090: 4669 6c65 5374 7269 6e67 5265 7370 6f6e  FileStringRespon
-000030a0: 7365 9473 7373 758c 0334 3031 947d 9428  se.sssu..401.}.(
-000030b0: 8c0b 6465 7363 7269 7074 696f 6e94 8c11  ..description...
-000030c0: 4e6f 7420 4175 7468 656e 7469 6361 7465  Not Authenticate
-000030d0: 6494 8c07 636f 6e74 656e 7494 7d94 8c10  d...content.}...
-000030e0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-000030f0: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
-00003100: 2472 6566 948c 2723 2f63 6f6d 706f 6e65  $ref..'#/compone
-00003110: 6e74 732f 7363 6865 6d61 732f 4669 6c65  nts/schemas/File
-00003120: 5374 7269 6e67 5265 7370 6f6e 7365 9473  StringResponse.s
-00003130: 7373 758c 0334 3033 947d 9428 8c0b 6465  ssu..403.}.(..de
-00003140: 7363 7269 7074 696f 6e94 8c11 5065 726d  scription...Perm
-00003150: 6973 7369 6f6e 2044 656e 6965 6494 8c07  ission Denied...
-00003160: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
-00003170: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
-00003180: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
-00003190: 948c 2723 2f63 6f6d 706f 6e65 6e74 732f  ..'#/components/
-000031a0: 7363 6865 6d61 732f 4669 6c65 5374 7269  schemas/FileStri
-000031b0: 6e67 5265 7370 6f6e 7365 9473 7373 758c  ngResponse.sssu.
-000031c0: 0334 3034 947d 9428 8c0b 6465 7363 7269  .404.}.(..descri
-000031d0: 7074 696f 6e94 8c09 4e6f 7420 466f 756e  ption...Not Foun
-000031e0: 6494 8c07 636f 6e74 656e 7494 7d94 8c10  d...content.}...
-000031f0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-00003200: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
-00003210: 2472 6566 948c 2723 2f63 6f6d 706f 6e65  $ref..'#/compone
-00003220: 6e74 732f 7363 6865 6d61 732f 4669 6c65  nts/schemas/File
-00003230: 5374 7269 6e67 5265 7370 6f6e 7365 9473  StringResponse.s
-00003240: 7373 758c 0335 3030 947d 9428 8c0b 6465  ssu..500.}.(..de
-00003250: 7363 7269 7074 696f 6e94 8c0e 496e 7465  scription...Inte
-00003260: 726e 616c 2045 7272 6f72 948c 0763 6f6e  rnal Error...con
-00003270: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
-00003280: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
-00003290: 6865 6d61 947d 948c 0424 7265 6694 8c27  hema.}...$ref..'
-000032a0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
-000032b0: 656d 6173 2f46 696c 6553 7472 696e 6752  emas/FileStringR
-000032c0: 6573 706f 6e73 6594 7373 7375 7575 8c04  esponse.sssuuu..
-000032d0: 706f 7374 947d 9428 8c04 7461 6773 945d  post.}.(..tags.]
-000032e0: 948c 0f46 696c 6520 4f70 6572 6174 696f  ...File Operatio
-000032f0: 6e73 9461 8c0b 6465 7363 7269 7074 696f  ns.a..descriptio
-00003300: 6e94 8c64 5275 6e20 6120 6e61 7469 7665  n..dRun a native
-00003310: 206f 7065 7261 7469 6f6e 206f 6e20 6120   operation on a 
-00003320: 7061 7468 2e20 4f70 6572 6174 696f 6e73  path. Operations
-00003330: 2061 7265 2063 686d 6f64 2c20 6368 6f77   are chmod, chow
-00003340: 6e20 6f72 2063 6867 7270 2e20 466f 7220  n or chgrp. For 
-00003350: 6120 7379 7374 656d 206f 6620 7479 7065  a system of type
-00003360: 204c 494e 5558 2e0a 948c 0b6f 7065 7261   LINUX.....opera
-00003370: 7469 6f6e 4964 948c 1072 756e 4c69 6e75  tionId...runLinu
-00003380: 784e 6174 6976 654f 7094 8c0a 7061 7261  xNativeOp...para
-00003390: 6d65 7465 7273 945d 9428 7d94 288c 046e  meters.].(}.(..n
-000033a0: 616d 6594 8c08 7379 7374 656d 4964 948c  ame...systemId..
-000033b0: 0269 6e94 8c04 7061 7468 948c 0b64 6573  .in...path...des
-000033c0: 6372 6970 7469 6f6e 948c 0953 7973 7465  cription...Syste
-000033d0: 6d20 4944 948c 0872 6571 7569 7265 6494  m ID...required.
-000033e0: 888c 0673 6368 656d 6194 7d94 8c04 7479  ...schema.}...ty
-000033f0: 7065 948c 0673 7472 696e 6794 7375 7d94  pe...string.su}.
-00003400: 288c 046e 616d 6594 8c04 7061 7468 948c  (..name...path..
-00003410: 0269 6e94 8c04 7061 7468 948c 0b64 6573  .in...path...des
-00003420: 6372 6970 7469 6f6e 948c 2550 6174 6820  cription..%Path 
-00003430: 7265 6c61 7469 7665 2074 6f20 7468 6520  relative to the 
-00003440: 7379 7374 656d 202a 726f 6f74 4469 722a  system *rootDir*
-00003450: 948c 0872 6571 7569 7265 6494 888c 0673  ...required....s
-00003460: 6368 656d 6194 7d94 8c04 7479 7065 948c  chema.}...type..
-00003470: 0673 7472 696e 6794 7375 7d94 288c 046e  .string.su}.(..n
-00003480: 616d 6594 8c09 7265 6375 7273 6976 6594  ame...recursive.
-00003490: 8c02 696e 948c 0571 7565 7279 948c 0b64  ..in...query...d
-000034a0: 6573 6372 6970 7469 6f6e 948c 5549 6620  escription..UIf 
-000034b0: 7061 7468 2069 7320 6120 6469 7265 6374  path is a direct
-000034c0: 6f72 7920 7468 6973 2069 6e64 6963 6174  ory this indicat
-000034d0: 6573 2077 6865 7468 6572 206f 7220 6e6f  es whether or no
-000034e0: 7420 746f 2061 7070 6c79 2074 6865 2063  t to apply the c
-000034f0: 6861 6e67 6573 2072 6563 7572 7369 7665  hanges recursive
-00003500: 6c79 948c 0673 6368 656d 6194 7d94 288c  ly...schema.}.(.
-00003510: 0474 7970 6594 8c07 626f 6f6c 6561 6e94  .type...boolean.
-00003520: 8c07 6465 6661 756c 7494 8975 8c07 6578  ..default..u..ex
-00003530: 616d 706c 6594 8875 658c 0b72 6571 7565  ample..ue..reque
-00003540: 7374 426f 6479 947d 948c 0763 6f6e 7465  stBody.}...conte
-00003550: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
-00003560: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
-00003570: 6d61 947d 948c 0424 7265 6694 8c29 232f  ma.}...$ref..)#/
-00003580: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-00003590: 6173 2f4e 6174 6976 654c 696e 7578 4f70  as/NativeLinuxOp
-000035a0: 5265 7175 6573 7494 7373 7373 8c09 7265  Request.ssss..re
-000035b0: 7370 6f6e 7365 7394 7d94 288c 0332 3030  sponses.}.(..200
-000035c0: 947d 9428 8c0b 6465 7363 7269 7074 696f  .}.(..descriptio
-000035d0: 6e94 8c02 4f4b 948c 0763 6f6e 7465 6e74  n...OK...content
-000035e0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
-000035f0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
-00003600: 947d 948c 0424 7265 6694 8c30 232f 636f  .}...$ref..0#/co
-00003610: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-00003620: 2f4e 6174 6976 654c 696e 7578 4f70 5265  /NativeLinuxOpRe
-00003630: 7375 6c74 5265 7370 6f6e 7365 9473 7373  sultResponse.sss
-00003640: 758c 0334 3030 947d 9428 8c0b 6465 7363  u..400.}.(..desc
-00003650: 7269 7074 696f 6e94 8c0b 4261 6420 5265  ription...Bad Re
-00003660: 7175 6573 7494 8c07 636f 6e74 656e 7494  quest...content.
-00003670: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
-00003680: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
-00003690: 7d94 8c04 2472 6566 948c 2723 2f63 6f6d  }...$ref..'#/com
-000036a0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-000036b0: 4669 6c65 5374 7269 6e67 5265 7370 6f6e  FileStringRespon
-000036c0: 7365 9473 7373 758c 0334 3031 947d 9428  se.sssu..401.}.(
-000036d0: 8c0b 6465 7363 7269 7074 696f 6e94 8c11  ..description...
-000036e0: 4e6f 7420 4175 7468 656e 7469 6361 7465  Not Authenticate
-000036f0: 6494 8c07 636f 6e74 656e 7494 7d94 8c10  d...content.}...
-00003700: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-00003710: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
-00003720: 2472 6566 948c 2723 2f63 6f6d 706f 6e65  $ref..'#/compone
-00003730: 6e74 732f 7363 6865 6d61 732f 4669 6c65  nts/schemas/File
-00003740: 5374 7269 6e67 5265 7370 6f6e 7365 9473  StringResponse.s
-00003750: 7373 758c 0334 3033 947d 9428 8c0b 6465  ssu..403.}.(..de
-00003760: 7363 7269 7074 696f 6e94 8c11 5065 726d  scription...Perm
-00003770: 6973 7369 6f6e 2044 656e 6965 6494 8c07  ission Denied...
-00003780: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
-00003790: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
-000037a0: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
-000037b0: 948c 2723 2f63 6f6d 706f 6e65 6e74 732f  ..'#/components/
-000037c0: 7363 6865 6d61 732f 4669 6c65 5374 7269  schemas/FileStri
-000037d0: 6e67 5265 7370 6f6e 7365 9473 7373 758c  ngResponse.sssu.
-000037e0: 0334 3034 947d 9428 8c0b 6465 7363 7269  .404.}.(..descri
-000037f0: 7074 696f 6e94 8c09 4e6f 7420 466f 756e  ption...Not Foun
-00003800: 6494 8c07 636f 6e74 656e 7494 7d94 8c10  d...content.}...
-00003810: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-00003820: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
-00003830: 2472 6566 948c 2723 2f63 6f6d 706f 6e65  $ref..'#/compone
-00003840: 6e74 732f 7363 6865 6d61 732f 4669 6c65  nts/schemas/File
-00003850: 5374 7269 6e67 5265 7370 6f6e 7365 9473  StringResponse.s
-00003860: 7373 758c 0335 3030 947d 9428 8c0b 6465  ssu..500.}.(..de
-00003870: 7363 7269 7074 696f 6e94 8c0e 496e 7465  scription...Inte
-00003880: 726e 616c 2045 7272 6f72 948c 0763 6f6e  rnal Error...con
-00003890: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
-000038a0: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
-000038b0: 6865 6d61 947d 948c 0424 7265 6694 8c27  hema.}...$ref..'
-000038c0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
-000038d0: 656d 6173 2f46 696c 6553 7472 696e 6752  emas/FileStringR
-000038e0: 6573 706f 6e73 6594 7373 7375 7575 758c  esponse.sssuuuu.
-000038f0: 2c2f 7633 2f66 696c 6573 2f75 7469 6c73  ,/v3/files/utils
-00003900: 2f6c 696e 7578 2f66 6163 6c2f 7b73 7973  /linux/facl/{sys
-00003910: 7465 6d49 647d 2f7b 7061 7468 7d94 7d94  temId}/{path}.}.
-00003920: 288c 0367 6574 947d 9428 8c04 7461 6773  (..get.}.(..tags
-00003930: 945d 948c 0f46 696c 6520 4f70 6572 6174  .]...File Operat
-00003940: 696f 6e73 9461 8c0b 6465 7363 7269 7074  ions.a..descript
-00003950: 696f 6e94 8c28 4765 7420 6669 6c65 2041  ion..(Get file A
-00003960: 434c 7320 666f 7220 6669 6c65 7320 6f72  CLs for files or
-00003970: 2064 6972 6563 746f 7269 6573 2e0a 948c   directories....
-00003980: 0b6f 7065 7261 7469 6f6e 4964 948c 0767  .operationId...g
-00003990: 6574 4661 636c 948c 0a70 6172 616d 6574  etFacl...paramet
-000039a0: 6572 7394 5d94 287d 9428 8c04 6e61 6d65  ers.].(}.(..name
-000039b0: 948c 0873 7973 7465 6d49 6494 8c02 696e  ...systemId...in
-000039c0: 948c 0470 6174 6894 8c0b 6465 7363 7269  ...path...descri
-000039d0: 7074 696f 6e94 8c09 5379 7374 656d 2049  ption...System I
-000039e0: 4494 8c08 7265 7175 6972 6564 9488 8c06  D...required....
-000039f0: 7363 6865 6d61 947d 948c 0474 7970 6594  schema.}...type.
-00003a00: 8c06 7374 7269 6e67 9473 8c07 6578 616d  ..string.s..exam
-00003a10: 706c 6594 8c09 7379 7374 656d 3132 3394  ple...system123.
-00003a20: 757d 9428 8c04 6e61 6d65 948c 0470 6174  u}.(..name...pat
-00003a30: 6894 8c02 696e 948c 0470 6174 6894 8c0b  h...in...path...
-00003a40: 6465 7363 7269 7074 696f 6e94 8c25 5061  description..%Pa
-00003a50: 7468 2072 656c 6174 6976 6520 746f 2074  th relative to t
-00003a60: 6865 2073 7973 7465 6d20 2a72 6f6f 7444  he system *rootD
-00003a70: 6972 2a94 8c08 7265 7175 6972 6564 9488  ir*...required..
-00003a80: 8c06 7363 6865 6d61 947d 948c 0474 7970  ..schema.}...typ
-00003a90: 6594 8c06 7374 7269 6e67 9473 8c07 6578  e...string.s..ex
-00003aa0: 616d 706c 6594 8c17 2f64 6972 6563 746f  ample.../directo
-00003ab0: 7279 412f 6469 7265 6374 6f72 7942 2f94  ryA/directoryB/.
-00003ac0: 7565 8c09 7265 7370 6f6e 7365 7394 7d94  ue..responses.}.
-00003ad0: 288c 0332 3030 947d 9428 8c0b 6465 7363  (..200.}.(..desc
-00003ae0: 7269 7074 696f 6e94 8c02 4f4b 948c 0763  ription...OK...c
-00003af0: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
-00003b00: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
-00003b10: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
-00003b20: 8c2f 232f 636f 6d70 6f6e 656e 7473 2f73  ./#/components/s
-00003b30: 6368 656d 6173 2f4e 6174 6976 654c 696e  chemas/NativeLin
-00003b40: 7578 4765 7446 6163 6c52 6573 706f 6e73  uxGetFaclRespons
-00003b50: 6594 7373 7375 8c03 3430 3194 7d94 288c  e.sssu..401.}.(.
-00003b60: 0b64 6573 6372 6970 7469 6f6e 948c 114e  .description...N
-00003b70: 6f74 2041 7574 6865 6e74 6963 6174 6564  ot Authenticated
-00003b80: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
-00003b90: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
-00003ba0: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
-00003bb0: 7265 6694 8c27 232f 636f 6d70 6f6e 656e  ref..'#/componen
-00003bc0: 7473 2f73 6368 656d 6173 2f46 696c 6553  ts/schemas/FileS
-00003bd0: 7472 696e 6752 6573 706f 6e73 6594 7373  tringResponse.ss
-00003be0: 7375 8c03 3430 3394 7d94 288c 0b64 6573  su..403.}.(..des
-00003bf0: 6372 6970 7469 6f6e 948c 1150 6572 6d69  cription...Permi
-00003c00: 7373 696f 6e20 4465 6e69 6564 948c 0763  ssion Denied...c
-00003c10: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
-00003c20: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
-00003c30: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
-00003c40: 8c27 232f 636f 6d70 6f6e 656e 7473 2f73  .'#/components/s
-00003c50: 6368 656d 6173 2f46 696c 6553 7472 696e  chemas/FileStrin
-00003c60: 6752 6573 706f 6e73 6594 7373 7375 8c03  gResponse.sssu..
-00003c70: 3430 3494 7d94 288c 0b64 6573 6372 6970  404.}.(..descrip
-00003c80: 7469 6f6e 948c 094e 6f74 2046 6f75 6e64  tion...Not Found
-00003c90: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
-00003ca0: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
-00003cb0: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
-00003cc0: 7265 6694 8c27 232f 636f 6d70 6f6e 656e  ref..'#/componen
-00003cd0: 7473 2f73 6368 656d 6173 2f46 696c 6553  ts/schemas/FileS
-00003ce0: 7472 696e 6752 6573 706f 6e73 6594 7373  tringResponse.ss
-00003cf0: 7375 8c03 3530 3094 7d94 288c 0b64 6573  su..500.}.(..des
-00003d00: 6372 6970 7469 6f6e 948c 0e49 6e74 6572  cription...Inter
-00003d10: 6e61 6c20 4572 726f 7294 8c07 636f 6e74  nal Error...cont
-00003d20: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
-00003d30: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
-00003d40: 656d 6194 7d94 8c04 2472 6566 948c 2723  ema.}...$ref..'#
-00003d50: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-00003d60: 6d61 732f 4669 6c65 5374 7269 6e67 5265  mas/FileStringRe
-00003d70: 7370 6f6e 7365 9473 7373 7575 758c 0470  sponse.sssuuu..p
-00003d80: 6f73 7494 7d94 288c 0474 6167 7394 5d94  ost.}.(..tags.].
-00003d90: 8c0f 4669 6c65 204f 7065 7261 7469 6f6e  ..File Operation
-00003da0: 7394 618c 0b64 6573 6372 6970 7469 6f6e  s.a..description
-00003db0: 9458 2901 0000 5365 7420 6669 6c65 2041  .X)...Set file A
-00003dc0: 434c 7320 666f 7220 6669 6c65 7320 6f72  CLs for files or
-00003dd0: 2064 6972 6563 746f 7269 6573 2e0a 0a54   directories...T
-00003de0: 6869 7320 6361 6e20 6265 2075 7365 6420  his can be used 
-00003df0: 666f 7220 6120 7369 6e67 6c65 2066 696c  for a single fil
-00003e00: 6520 6f72 2064 6972 6563 746f 7279 2c20  e or directory, 
-00003e10: 6f72 2063 616e 2062 6520 7265 6375 7273  or can be recurs
-00003e20: 6976 652e 2020 4966 2072 6563 7572 7369  ive.  If recursi
-00003e30: 6f6e 2069 730a 7573 6564 2c20 6974 2063  on is.used, it c
-00003e40: 616e 2062 6520 6d61 6465 2074 6f20 666f  an be made to fo
-00003e50: 6c6c 6f77 2073 796d 6c69 6e6b 732c 206f  llow symlinks, o
-00003e60: 7220 6e6f 7420 666f 6c6c 6f77 2073 796d  r not follow sym
-00003e70: 6c69 6e6b 732e 0a0a 5468 6520 6f70 6572  links...The oper
-00003e80: 6174 696f 6e73 2073 7570 706f 7274 2061  ations support a
-00003e90: 6464 696e 6720 6f72 2072 656d 6f76 696e  dding or removin
-00003ea0: 6720 4163 6c20 456e 7472 6965 7320 6173  g Acl Entries as
-00003eb0: 2077 656c 6c20 6173 2072 656d 6f76 696e   well as removin
-00003ec0: 6720 616c 6c20 6163 6c73 206f 7220 616c  g all acls or al
-00003ed0: 6c0a 6465 6661 756c 7420 6163 6c73 0a94  l.default acls..
-00003ee0: 8c0b 6f70 6572 6174 696f 6e49 6494 8c07  ..operationId...
-00003ef0: 7365 7446 6163 6c94 8c0a 7061 7261 6d65  setFacl...parame
-00003f00: 7465 7273 945d 9428 7d94 288c 046e 616d  ters.].(}.(..nam
-00003f10: 6594 8c08 7379 7374 656d 4964 948c 0269  e...systemId...i
-00003f20: 6e94 8c04 7061 7468 948c 0872 6571 7569  n...path...requi
-00003f30: 7265 6494 888c 0b64 6573 6372 6970 7469  red....descripti
-00003f40: 6f6e 948c 0953 7973 7465 6d20 4944 948c  on...System ID..
-00003f50: 0673 6368 656d 6194 7d94 8c04 7479 7065  .schema.}...type
-00003f60: 948c 0673 7472 696e 6794 738c 0765 7861  ...string.s..exa
-00003f70: 6d70 6c65 948c 0973 7973 7465 6d31 3233  mple...system123
-00003f80: 9475 7d94 288c 046e 616d 6594 8c04 7061  .u}.(..name...pa
-00003f90: 7468 948c 0269 6e94 8c04 7061 7468 948c  th...in...path..
-00003fa0: 0b64 6573 6372 6970 7469 6f6e 948c 2550  .description..%P
-00003fb0: 6174 6820 7265 6c61 7469 7665 2074 6f20  ath relative to 
-00003fc0: 7468 6520 7379 7374 656d 202a 726f 6f74  the system *root
-00003fd0: 4469 722a 948c 0872 6571 7569 7265 6494  Dir*...required.
-00003fe0: 888c 0673 6368 656d 6194 7d94 8c04 7479  ...schema.}...ty
-00003ff0: 7065 948c 0673 7472 696e 6794 738c 0765  pe...string.s..e
-00004000: 7861 6d70 6c65 948c 172f 6469 7265 6374  xample.../direct
-00004010: 6f72 7941 2f64 6972 6563 746f 7279 422f  oryA/directoryB/
-00004020: 9475 658c 0b72 6571 7565 7374 426f 6479  .ue..requestBody
-00004030: 947d 9428 8c08 7265 7175 6972 6564 9488  .}.(..required..
-00004040: 8c0b 6465 7363 7269 7074 696f 6e94 8c35  ..description..5
-00004050: 4120 4a53 4f4e 206f 626a 6563 7420 7370  A JSON object sp
-00004060: 6563 6966 7969 6e67 2075 7064 6174 6564  ecifying updated
-00004070: 2073 6861 7269 6e67 2069 6e66 6f72 6d61   sharing informa
-00004080: 7469 6f6e 2e94 8c07 636f 6e74 656e 7494  tion....content.
-00004090: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
-000040a0: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
-000040b0: 7d94 8c04 2472 6566 948c 2e23 2f63 6f6d  }...$ref...#/com
-000040c0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-000040d0: 4e61 7469 7665 4c69 6e75 7853 6574 4661  NativeLinuxSetFa
-000040e0: 636c 5265 7175 6573 7494 7373 7375 8c09  clRequest.sssu..
-000040f0: 7265 7370 6f6e 7365 7394 7d94 288c 0332  responses.}.(..2
-00004100: 3030 947d 9428 8c0b 6465 7363 7269 7074  00.}.(..descript
-00004110: 696f 6e94 8c02 4f4b 948c 0763 6f6e 7465  ion...OK...conte
-00004120: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
-00004130: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
-00004140: 6d61 947d 948c 0424 7265 6694 8c2f 232f  ma.}...$ref../#/
-00004150: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-00004160: 6173 2f4e 6174 6976 654c 696e 7578 5365  as/NativeLinuxSe
-00004170: 7446 6163 6c52 6573 706f 6e73 6594 7373  tFaclResponse.ss
-00004180: 7375 8c03 3430 3094 7d94 288c 0b64 6573  su..400.}.(..des
-00004190: 6372 6970 7469 6f6e 948c 0b42 6164 2052  cription...Bad R
-000041a0: 6571 7565 7374 948c 0763 6f6e 7465 6e74  equest...content
-000041b0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
-000041c0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
-000041d0: 947d 948c 0424 7265 6694 8c27 232f 636f  .}...$ref..'#/co
-000041e0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-000041f0: 2f46 696c 6553 7472 696e 6752 6573 706f  /FileStringRespo
-00004200: 6e73 6594 7373 7375 8c03 3430 3194 7d94  nse.sssu..401.}.
-00004210: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
-00004220: 114e 6f74 2041 7574 6865 6e74 6963 6174  .Not Authenticat
-00004230: 6564 948c 0763 6f6e 7465 6e74 947d 948c  ed...content.}..
-00004240: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
-00004250: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
-00004260: 0424 7265 6694 8c27 232f 636f 6d70 6f6e  .$ref..'#/compon
-00004270: 656e 7473 2f73 6368 656d 6173 2f46 696c  ents/schemas/Fil
-00004280: 6553 7472 696e 6752 6573 706f 6e73 6594  eStringResponse.
-00004290: 7373 7375 8c03 3430 3394 7d94 288c 0b64  sssu..403.}.(..d
-000042a0: 6573 6372 6970 7469 6f6e 948c 1150 6572  escription...Per
-000042b0: 6d69 7373 696f 6e20 4465 6e69 6564 948c  mission Denied..
-000042c0: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
-000042d0: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
-000042e0: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
-000042f0: 6694 8c27 232f 636f 6d70 6f6e 656e 7473  f..'#/components
-00004300: 2f73 6368 656d 6173 2f46 696c 6553 7472  /schemas/FileStr
-00004310: 696e 6752 6573 706f 6e73 6594 7373 7375  ingResponse.sssu
-00004320: 8c03 3430 3494 7d94 288c 0b64 6573 6372  ..404.}.(..descr
-00004330: 6970 7469 6f6e 948c 094e 6f74 2046 6f75  iption...Not Fou
-00004340: 6e64 948c 0763 6f6e 7465 6e74 947d 948c  nd...content.}..
-00004350: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
-00004360: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
-00004370: 0424 7265 6694 8c27 232f 636f 6d70 6f6e  .$ref..'#/compon
-00004380: 656e 7473 2f73 6368 656d 6173 2f46 696c  ents/schemas/Fil
-00004390: 6553 7472 696e 6752 6573 706f 6e73 6594  eStringResponse.
-000043a0: 7373 7375 8c03 3530 3094 7d94 288c 0b64  sssu..500.}.(..d
-000043b0: 6573 6372 6970 7469 6f6e 948c 0e49 6e74  escription...Int
-000043c0: 6572 6e61 6c20 4572 726f 7294 8c07 636f  ernal Error...co
-000043d0: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
-000043e0: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
-000043f0: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
-00004400: 2723 2f63 6f6d 706f 6e65 6e74 732f 7363  '#/components/sc
-00004410: 6865 6d61 732f 4669 6c65 5374 7269 6e67  hemas/FileString
-00004420: 5265 7370 6f6e 7365 9473 7373 7575 7575  Response.sssuuuu
-00004430: 8c23 2f76 332f 6669 6c65 732f 636f 6e74  .#/v3/files/cont
-00004440: 656e 742f 7b73 7973 7465 6d49 647d 2f7b  ent/{systemId}/{
-00004450: 7061 7468 7d94 7d94 8c03 6765 7494 7d94  path}.}...get.}.
-00004460: 288c 0474 6167 7394 5d94 8c07 436f 6e74  (..tags.]...Cont
-00004470: 656e 7494 618c 0b64 6573 6372 6970 7469  ent.a..descripti
-00004480: 6f6e 9458 b502 0000 4765 7420 6669 6c65  on.X....Get file
-00004490: 206f 7220 6469 7265 6374 6f72 7920 636f   or directory co
-000044a0: 6e74 656e 7473 2061 7320 6120 7374 7265  ntents as a stre
-000044b0: 616d 206f 6620 6461 7461 2e0a 0a43 6572  am of data...Cer
-000044c0: 7461 696e 2073 6572 7669 6365 7320 6d61  tain services ma
-000044d0: 7920 7573 6520 7468 6520 7175 6572 7920  y use the query 
-000044e0: 7061 7261 6d65 7465 7220 2a69 6d70 6572  parameter *imper
-000044f0: 736f 6e61 7469 6f6e 4964 2a20 746f 2062  sonationId* to b
-00004500: 6520 7573 6564 2069 6e20 706c 6163 6520  e used in place 
-00004510: 6f66 2074 6865 2072 6571 7565 7374 696e  of the requestin
-00004520: 670a 5461 7069 7320 7573 6572 2e20 5461  g.Tapis user. Ta
-00004530: 7069 7320 7769 6c6c 2075 7365 2074 6869  pis will use thi
-00004540: 7320 7573 6572 2049 6420 7768 656e 2070  s user Id when p
-00004550: 6572 666f 726d 696e 6720 6175 7468 6f72  erforming author
-00004560: 697a 6174 696f 6e20 616e 6420 7265 736f  ization and reso
-00004570: 6c76 696e 6720 7468 6520 2a65 6666 6563  lving the *effec
-00004580: 7469 7665 5573 6572 4964 2a0a 666f 7220  tiveUserId*.for 
-00004590: 7468 6520 7379 7374 656d 2e0a 0a55 7365  the system...Use
-000045a0: 2074 6865 2071 7565 7279 2070 6172 616d   the query param
-000045b0: 6574 6572 202a 7a69 702a 2074 6f20 7265  eter *zip* to re
-000045c0: 7175 6573 7420 6120 7374 7265 616d 2063  quest a stream c
-000045d0: 6f6d 7072 6573 7365 6420 7573 696e 6720  ompressed using 
-000045e0: 7468 6520 5a49 5020 6669 6c65 2066 6f72  the ZIP file for
-000045f0: 6d61 742e 2054 6869 7320 6973 206e 6f74  mat. This is not
-00004600: 2061 6c6c 6f77 6564 0a69 6620 7379 7374   allowed.if syst
-00004610: 656d 202a 726f 6f74 4469 722a 2070 6c75  em *rootDir* plu
-00004620: 7320 2a70 6174 682a 2077 6f75 6c64 2072  s *path* would r
-00004630: 6573 756c 7420 696e 2061 6c6c 2066 696c  esult in all fil
-00004640: 6573 206f 6e20 7468 6520 686f 7374 2062  es on the host b
-00004650: 6569 6e67 2069 6e63 6c75 6465 642e 2050  eing included. P
-00004660: 6c65 6173 6520 646f 776e 6c6f 6164 0a69  lease download.i
-00004670: 6e64 6976 6964 7561 6c20 6469 7265 6374  ndividual direct
-00004680: 6f72 6965 732c 2066 696c 6573 206f 7220  ories, files or 
-00004690: 6f62 6a65 6374 732e 0a0a 4365 7274 6169  objects...Certai
-000046a0: 6e20 7365 7276 6963 6573 206d 6179 2075  n services may u
-000046b0: 7365 2074 6865 2071 7565 7279 2070 6172  se the query par
-000046c0: 616d 6574 6572 202a 7368 6172 6564 4170  ameter *sharedAp
-000046d0: 7043 7478 2a20 746f 2069 6e64 6963 6174  pCtx* to indicat
-000046e0: 6520 7468 6174 2074 6865 2072 6571 7565  e that the reque
-000046f0: 7374 2069 7320 696e 2061 2073 6861 7265  st is in a share
-00004700: 640a 6170 706c 6963 6174 696f 6e20 636f  d.application co
-00004710: 6e74 6578 742e 2054 6170 6973 2061 7574  ntext. Tapis aut
-00004720: 686f 7269 7a61 7469 6f6e 2077 696c 6c20  horization will 
-00004730: 6265 2062 7970 6173 7365 642e 0a94 8c0b  be bypassed.....
-00004740: 6f70 6572 6174 696f 6e49 6494 8c0b 6765  operationId...ge
-00004750: 7443 6f6e 7465 6e74 7394 8c0a 7061 7261  tContents...para
-00004760: 6d65 7465 7273 945d 9428 7d94 288c 046e  meters.].(}.(..n
-00004770: 616d 6594 8c08 7379 7374 656d 4964 948c  ame...systemId..
-00004780: 0269 6e94 8c04 7061 7468 948c 0b64 6573  .in...path...des
-00004790: 6372 6970 7469 6f6e 948c 0953 7973 7465  cription...Syste
-000047a0: 6d20 4944 948c 0872 6571 7569 7265 6494  m ID...required.
-000047b0: 888c 0673 6368 656d 6194 7d94 8c04 7479  ...schema.}...ty
-000047c0: 7065 948c 0673 7472 696e 6794 738c 0765  pe...string.s..e
-000047d0: 7861 6d70 6c65 948c 0973 7973 7465 6d31  xample...system1
-000047e0: 3233 9475 7d94 288c 046e 616d 6594 8c04  23.u}.(..name...
-000047f0: 7061 7468 948c 0269 6e94 8c04 7061 7468  path...in...path
-00004800: 948c 0b64 6573 6372 6970 7469 6f6e 948c  ...description..
-00004810: 2550 6174 6820 7265 6c61 7469 7665 2074  %Path relative t
-00004820: 6f20 7468 6520 7379 7374 656d 202a 726f  o the system *ro
-00004830: 6f74 4469 722a 948c 0872 6571 7569 7265  otDir*...require
-00004840: 6494 888c 0673 6368 656d 6194 7d94 8c04  d....schema.}...
-00004850: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-00004860: 0765 7861 6d70 6c65 948c 172f 6469 7265  .example.../dire
-00004870: 6374 6f72 7941 2f64 6972 6563 746f 7279  ctoryA/directory
-00004880: 422f 9475 7d94 288c 046e 616d 6594 8c05  B/.u}.(..name...
-00004890: 7261 6e67 6594 8c02 696e 948c 0668 6561  range...in...hea
-000048a0: 6465 7294 8c0b 6465 7363 7269 7074 696f  der...descriptio
-000048b0: 6e94 8c4b 4f70 7469 6f6e 616c 2072 616e  n..KOptional ran
-000048c0: 6765 206f 6620 6279 7465 7320 746f 2073  ge of bytes to s
-000048d0: 656e 642e 2049 6620 6e6f 7420 7370 6563  end. If not spec
-000048e0: 6966 6965 6420 616c 6c20 636f 6e74 656e  ified all conten
-000048f0: 7420 7769 6c6c 2062 6520 7365 6e74 2e94  t will be sent..
-00004900: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
-00004910: 6694 8c24 232f 636f 6d70 6f6e 656e 7473  f..$#/components
-00004920: 2f73 6368 656d 6173 2f48 6561 6465 7242  /schemas/HeaderB
-00004930: 7974 6552 616e 6765 9473 8c07 6578 616d  yteRange.s..exam
-00004940: 706c 6594 8c0b 7261 6e67 653d 302c 3939  ple...range=0,99
-00004950: 3994 757d 9428 8c04 6e61 6d65 948c 037a  9.u}.(..name...z
-00004960: 6970 948c 0269 6e94 8c05 7175 6572 7994  ip...in...query.
-00004970: 8c0b 6465 7363 7269 7074 696f 6e94 8c31  ..description..1
-00004980: 496e 6469 6361 7465 7320 6120 7a69 7020  Indicates a zip 
-00004990: 6f75 7470 7574 2073 7472 6561 6d20 7368  output stream sh
-000049a0: 6f75 6c64 2062 6520 7072 6f76 6964 6564  ould be provided
-000049b0: 2e94 8c06 7363 6865 6d61 947d 948c 0474  ....schema.}...t
-000049c0: 7970 6594 8c07 626f 6f6c 6561 6e94 738c  ype...boolean.s.
-000049d0: 0765 7861 6d70 6c65 9489 757d 9428 8c04  .example..u}.(..
-000049e0: 6e61 6d65 948c 046d 6f72 6594 8c02 696e  name...more...in
-000049f0: 948c 0668 6561 6465 7294 8c0b 6465 7363  ...header...desc
-00004a00: 7269 7074 696f 6e94 8c46 5365 6e64 2031  ription..FSend 1
-00004a10: 6b20 6f66 2055 5446 2d38 2065 6e63 6f64  k of UTF-8 encod
-00004a20: 6564 2073 7472 696e 6720 6261 636b 2073  ed string back s
-00004a30: 7461 7274 696e 6720 6174 2027 7061 6765  tarting at 'page
-00004a40: 2720 312c 2065 2e67 2e20 6d6f 7265 3d31  ' 1, e.g. more=1
-00004a50: 948c 0673 6368 656d 6194 7d94 288c 0474  ...schema.}.(..t
-00004a60: 7970 6594 8c07 696e 7465 6765 7294 8c06  ype...integer...
-00004a70: 666f 726d 6174 948c 0569 6e74 3634 9475  format...int64.u
-00004a80: 757d 9428 8c04 6e61 6d65 948c 0f69 6d70  u}.(..name...imp
-00004a90: 6572 736f 6e61 7469 6f6e 4964 948c 0269  ersonationId...i
-00004aa0: 6e94 8c05 7175 6572 7994 8c0b 6465 7363  n...query...desc
-00004ab0: 7269 7074 696f 6e94 8c3f 5265 7374 7269  ription..?Restri
-00004ac0: 6374 6564 2e20 4f6e 6c79 2063 6572 7461  cted. Only certa
-00004ad0: 696e 2073 6572 7669 6365 7320 6d61 7920  in services may 
-00004ae0: 696d 7065 7273 6f6e 6174 6520 6120 5461  impersonate a Ta
-00004af0: 7069 7320 7573 6572 2e94 8c06 7363 6865  pis user....sche
-00004b00: 6d61 947d 948c 0474 7970 6594 8c06 7374  ma.}...type...st
-00004b10: 7269 6e67 9473 757d 9428 8c04 6e61 6d65  ring.su}.(..name
-00004b20: 948c 0c73 6861 7265 6441 7070 4374 7894  ...sharedAppCtx.
-00004b30: 8c02 696e 948c 0571 7565 7279 948c 0b64  ..in...query...d
-00004b40: 6573 6372 6970 7469 6f6e 948c 5752 6573  escription..WRes
-00004b50: 7472 6963 7465 642e 204f 6e6c 7920 6365  tricted. Only ce
-00004b60: 7274 6169 6e20 7365 7276 6963 6573 206d  rtain services m
-00004b70: 6179 2069 6e64 6963 6174 6520 7468 6174  ay indicate that
-00004b80: 2074 6865 2072 6571 7565 7374 2069 7320   the request is 
-00004b90: 696e 2061 2073 6861 7265 6420 636f 6e74  in a shared cont
-00004ba0: 6578 742e 948c 0673 6368 656d 6194 7d94  ext....schema.}.
-00004bb0: 288c 0474 7970 6594 8c07 626f 6f6c 6561  (..type...boolea
-00004bc0: 6e94 8c07 6465 6661 756c 7494 8975 7565  n...default..uue
-00004bd0: 8c09 7265 7370 6f6e 7365 7394 7d94 288c  ..responses.}.(.
-00004be0: 0332 3030 947d 948c 0b64 6573 6372 6970  .200.}...descrip
-00004bf0: 7469 6f6e 948c 024f 4b94 738c 0334 3030  tion...OK.s..400
-00004c00: 947d 948c 0b64 6573 6372 6970 7469 6f6e  .}...description
-00004c10: 948c 0b42 6164 2052 6571 7565 7374 9473  ...Bad Request.s
-00004c20: 8c03 3430 3194 7d94 8c0b 6465 7363 7269  ..401.}...descri
-00004c30: 7074 696f 6e94 8c11 4e6f 7420 4175 7468  ption...Not Auth
-00004c40: 656e 7469 6361 7465 6494 738c 0334 3034  enticated.s..404
-00004c50: 947d 948c 0b64 6573 6372 6970 7469 6f6e  .}...description
-00004c60: 948c 094e 6f74 2046 6f75 6e64 9473 8c03  ...Not Found.s..
-00004c70: 3430 3394 7d94 8c0b 6465 7363 7269 7074  403.}...descript
-00004c80: 696f 6e94 8c11 5065 726d 6973 7369 6f6e  ion...Permission
-00004c90: 2044 656e 6965 6494 7375 7573 8c13 2f76   Denied.suus../v
-00004ca0: 332f 6669 6c65 732f 7472 616e 7366 6572  3/files/transfer
-00004cb0: 7394 7d94 288c 0367 6574 947d 9428 8c04  s.}.(..get.}.(..
-00004cc0: 7461 6773 945d 948c 0954 7261 6e73 6665  tags.]...Transfe
-00004cd0: 7273 9461 8c0b 6465 7363 7269 7074 696f  rs.a..descriptio
-00004ce0: 6e94 8c3c 4765 7420 6120 6c69 7374 206f  n..<Get a list o
-00004cf0: 6620 7472 616e 7366 6572 2074 6173 6b73  f transfer tasks
-00004d00: 2073 7461 7274 696e 6720 7769 7468 2074   starting with t
-00004d10: 6865 206d 6f73 7420 7265 6365 6e74 2e0a  he most recent..
-00004d20: 948c 0b6f 7065 7261 7469 6f6e 4964 948c  ...operationId..
-00004d30: 1667 6574 5265 6365 6e74 5472 616e 7366  .getRecentTransf
-00004d40: 6572 5461 736b 7394 8c0a 7061 7261 6d65  erTasks...parame
-00004d50: 7465 7273 945d 9428 7d94 288c 046e 616d  ters.].(}.(..nam
-00004d60: 6594 8c05 6c69 6d69 7494 8c02 696e 948c  e...limit...in..
-00004d70: 0571 7565 7279 948c 0b64 6573 6372 6970  .query...descrip
-00004d80: 7469 6f6e 948c 1070 6167 696e 6174 696f  tion...paginatio
-00004d90: 6e20 6c69 6d69 7494 8c06 7363 6865 6d61  n limit...schema
-00004da0: 947d 9428 8c04 7479 7065 948c 0769 6e74  .}.(..type...int
-00004db0: 6567 6572 948c 0666 6f72 6d61 7494 8c05  eger...format...
-00004dc0: 696e 7433 3294 8c07 6465 6661 756c 7494  int32...default.
-00004dd0: 4de8 0375 8c07 6578 616d 706c 6594 4b64  M..u..example.Kd
-00004de0: 757d 9428 8c04 6e61 6d65 948c 066f 6666  u}.(..name...off
-00004df0: 7365 7494 8c02 696e 948c 0571 7565 7279  set...in...query
-00004e00: 948c 0b64 6573 6372 6970 7469 6f6e 948c  ...description..
-00004e10: 1170 6167 696e 6174 696f 6e20 6f66 6673  .pagination offs
-00004e20: 6574 948c 0673 6368 656d 6194 7d94 288c  et...schema.}.(.
-00004e30: 0474 7970 6594 8c07 696e 7465 6765 7294  .type...integer.
-00004e40: 8c06 666f 726d 6174 948c 0569 6e74 3332  ..format...int32
-00004e50: 948c 0764 6566 6175 6c74 944b 0075 8c07  ...default.K.u..
-00004e60: 6578 616d 706c 6594 4de8 0375 658c 0972  example.M..ue..r
-00004e70: 6573 706f 6e73 6573 947d 948c 0332 3030  esponses.}...200
-00004e80: 947d 9428 8c0b 6465 7363 7269 7074 696f  .}.(..descriptio
-00004e90: 6e94 8c02 4f4b 948c 0763 6f6e 7465 6e74  n...OK...content
-00004ea0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
-00004eb0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
-00004ec0: 947d 948c 0424 7265 6694 8c2d 232f 636f  .}...$ref..-#/co
-00004ed0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-00004ee0: 2f54 7261 6e73 6665 7254 6173 6b4c 6973  /TransferTaskLis
-00004ef0: 7452 6573 706f 6e73 6594 7373 7375 7375  tResponse.sssusu
-00004f00: 8c04 706f 7374 947d 9428 8c04 7461 6773  ..post.}.(..tags
-00004f10: 945d 948c 0954 7261 6e73 6665 7273 9461  .]...Transfers.a
-00004f20: 8c0b 6465 7363 7269 7074 696f 6e94 8c44  ..description..D
-00004f30: 4372 6561 7465 2061 2062 6163 6b67 726f  Create a backgro
-00004f40: 756e 6420 7461 736b 2077 6869 6368 2077  und task which w
-00004f50: 696c 6c20 7472 616e 7366 6572 2066 696c  ill transfer fil
-00004f60: 6573 2062 6574 7765 656e 2073 7973 7465  es between syste
-00004f70: 6d73 2e0a 948c 0b6f 7065 7261 7469 6f6e  ms.....operation
-00004f80: 4964 948c 1263 7265 6174 6554 7261 6e73  Id...createTrans
-00004f90: 6665 7254 6173 6b94 8c0b 7265 7175 6573  ferTask...reques
-00004fa0: 7442 6f64 7994 7d94 288c 0763 6f6e 7465  tBody.}.(..conte
-00004fb0: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
-00004fc0: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
-00004fd0: 6d61 947d 948c 0424 7265 6694 8c20 232f  ma.}...$ref.. #/
-00004fe0: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-00004ff0: 6173 2f52 6571 5472 616e 7366 6572 9473  as/ReqTransfer.s
-00005000: 7373 8c08 7265 7175 6972 6564 9488 758c  ss..required..u.
-00005010: 0972 6573 706f 6e73 6573 947d 948c 0332  .responses.}...2
-00005020: 3030 947d 9428 8c0b 6465 7363 7269 7074  00.}.(..descript
-00005030: 696f 6e94 8c02 4f4b 948c 0763 6f6e 7465  ion...OK...conte
-00005040: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
-00005050: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
-00005060: 6d61 947d 948c 0424 7265 6694 8c29 232f  ma.}...$ref..)#/
-00005070: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-00005080: 6173 2f54 7261 6e73 6665 7254 6173 6b52  as/TransferTaskR
-00005090: 6573 706f 6e73 6594 7373 7375 7375 758c  esponse.sssusuu.
-000050a0: 242f 7633 2f66 696c 6573 2f74 7261 6e73  $/v3/files/trans
-000050b0: 6665 7273 2f7b 7472 616e 7366 6572 5461  fers/{transferTa
-000050c0: 736b 4964 7d94 7d94 288c 0367 6574 947d  skId}.}.(..get.}
-000050d0: 9428 8c04 7461 6773 945d 948c 0954 7261  .(..tags.]...Tra
-000050e0: 6e73 6665 7273 9461 8c0b 6465 7363 7269  nsfers.a..descri
-000050f0: 7074 696f 6e94 8c1a 5265 7472 6965 7665  ption...Retrieve
-00005100: 2061 2074 7261 6e73 6665 7220 7461 736b   a transfer task
-00005110: 2e0a 948c 0b6f 7065 7261 7469 6f6e 4964  .....operationId
-00005120: 948c 0f67 6574 5472 616e 7366 6572 5461  ...getTransferTa
-00005130: 736b 948c 0a70 6172 616d 6574 6572 7394  sk...parameters.
-00005140: 5d94 7d94 288c 046e 616d 6594 8c0e 7472  ].}.(..name...tr
-00005150: 616e 7366 6572 5461 736b 4964 948c 0269  ansferTaskId...i
-00005160: 6e94 8c04 7061 7468 948c 0b64 6573 6372  n...path...descr
-00005170: 6970 7469 6f6e 948c 1054 7261 6e73 6665  iption...Transfe
-00005180: 7220 7461 736b 2049 4494 8c08 7265 7175  r task ID...requ
-00005190: 6972 6564 9488 8c06 7363 6865 6d61 947d  ired....schema.}
-000051a0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-000051b0: 9473 8c07 6578 616d 706c 6594 8c24 3634  .s..example..$64
-000051c0: 3931 6332 6135 2d61 6362 322d 3430 6566  91c2a5-acb2-40ef
-000051d0: 2d62 3263 302d 6263 3166 6334 6364 3765  -b2c0-bc1fc4cd7e
-000051e0: 3663 9475 618c 0972 6573 706f 6e73 6573  6c.ua..responses
-000051f0: 947d 948c 0332 3030 947d 9428 8c0b 6465  .}...200.}.(..de
-00005200: 7363 7269 7074 696f 6e94 8c02 4f4b 948c  scription...OK..
-00005210: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
-00005220: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
-00005230: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
-00005240: 6694 8c29 232f 636f 6d70 6f6e 656e 7473  f..)#/components
-00005250: 2f73 6368 656d 6173 2f54 7261 6e73 6665  /schemas/Transfe
-00005260: 7254 6173 6b52 6573 706f 6e73 6594 7373  rTaskResponse.ss
-00005270: 7375 7375 8c06 6465 6c65 7465 947d 9428  susu..delete.}.(
-00005280: 8c04 7461 6773 945d 948c 0954 7261 6e73  ..tags.]...Trans
-00005290: 6665 7273 9461 8c0b 6465 7363 7269 7074  fers.a..descript
-000052a0: 696f 6e94 8c2b 5265 7175 6573 7420 7468  ion..+Request th
-000052b0: 6174 2061 2074 7261 6e73 6665 7220 7461  at a transfer ta
-000052c0: 736b 2062 6520 6361 6e63 656c 6c65 642e  sk be cancelled.
-000052d0: 0a94 8c0b 6f70 6572 6174 696f 6e49 6494  ....operationId.
-000052e0: 8c12 6361 6e63 656c 5472 616e 7366 6572  ..cancelTransfer
-000052f0: 5461 736b 948c 0a70 6172 616d 6574 6572  Task...parameter
-00005300: 7394 5d94 7d94 288c 046e 616d 6594 8c0e  s.].}.(..name...
-00005310: 7472 616e 7366 6572 5461 736b 4964 948c  transferTaskId..
-00005320: 0269 6e94 8c04 7061 7468 948c 0b64 6573  .in...path...des
-00005330: 6372 6970 7469 6f6e 948c 1054 7261 6e73  cription...Trans
-00005340: 6665 7220 7461 736b 2049 4494 8c08 7265  fer task ID...re
-00005350: 7175 6972 6564 9488 8c06 7363 6865 6d61  quired....schema
-00005360: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-00005370: 6e67 9473 8c07 6578 616d 706c 6594 8c24  ng.s..example..$
-00005380: 3634 3931 6332 6135 2d61 6362 322d 3430  6491c2a5-acb2-40
-00005390: 6566 2d62 3263 302d 6263 3166 6334 6364  ef-b2c0-bc1fc4cd
-000053a0: 3765 3663 9475 618c 0972 6573 706f 6e73  7e6c.ua..respons
-000053b0: 6573 947d 948c 0332 3030 947d 9428 8c0b  es.}...200.}.(..
-000053c0: 6465 7363 7269 7074 696f 6e94 8c02 4f4b  description...OK
-000053d0: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
-000053e0: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
-000053f0: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
-00005400: 7265 6694 8c23 232f 636f 6d70 6f6e 656e  ref..##/componen
-00005410: 7473 2f73 6368 656d 6173 2f53 7472 696e  ts/schemas/Strin
-00005420: 6752 6573 706f 6e73 6594 7373 7375 7375  gResponse.sssusu
-00005430: 758c 2c2f 7633 2f66 696c 6573 2f74 7261  u.,/v3/files/tra
-00005440: 6e73 6665 7273 2f7b 7472 616e 7366 6572  nsfers/{transfer
-00005450: 5461 736b 4964 7d2f 6465 7461 696c 7394  TaskId}/details.
-00005460: 7d94 8c03 6765 7494 7d94 288c 0474 6167  }...get.}.(..tag
-00005470: 7394 5d94 8c09 5472 616e 7366 6572 7394  s.]...Transfers.
-00005480: 618c 0b64 6573 6372 6970 7469 6f6e 948c  a..description..
-00005490: 3352 6574 7269 6576 6520 6465 7461 696c  3Retrieve detail
-000054a0: 6564 2069 6e66 6f72 6d61 7469 6f6e 2066  ed information f
-000054b0: 6f72 2061 2074 7261 6e73 6665 7220 7461  or a transfer ta
-000054c0: 736b 2e0a 948c 0b6f 7065 7261 7469 6f6e  sk.....operation
-000054d0: 4964 948c 1667 6574 5472 616e 7366 6572  Id...getTransfer
-000054e0: 5461 736b 4465 7461 696c 7394 8c0a 7061  TaskDetails...pa
-000054f0: 7261 6d65 7465 7273 945d 9428 7d94 288c  rameters.].(}.(.
-00005500: 046e 616d 6594 8c0e 7472 616e 7366 6572  .name...transfer
-00005510: 5461 736b 4964 948c 0269 6e94 8c04 7061  TaskId...in...pa
-00005520: 7468 948c 0b64 6573 6372 6970 7469 6f6e  th...description
-00005530: 948c 1054 7261 6e73 6665 7220 7461 736b  ...Transfer task
-00005540: 2049 4494 8c08 7265 7175 6972 6564 9488   ID...required..
-00005550: 8c06 7363 6865 6d61 947d 948c 0474 7970  ..schema.}...typ
-00005560: 6594 8c06 7374 7269 6e67 9473 8c07 6578  e...string.s..ex
-00005570: 616d 706c 6594 8c24 3634 3931 6332 6135  ample..$6491c2a5
-00005580: 2d61 6362 322d 3430 6566 2d62 3263 302d  -acb2-40ef-b2c0-
-00005590: 6263 3166 6334 6364 3765 3663 9475 7d94  bc1fc4cd7e6c.u}.
-000055a0: 288c 046e 616d 6594 8c0f 696d 7065 7273  (..name...impers
-000055b0: 6f6e 6174 696f 6e49 6494 8c02 696e 948c  onationId...in..
-000055c0: 0571 7565 7279 948c 0b64 6573 6372 6970  .query...descrip
-000055d0: 7469 6f6e 948c 4648 6967 686c 7920 7265  tion..FHighly re
-000055e0: 7374 7269 6374 6564 2e20 4f6e 6c79 2063  stricted. Only c
-000055f0: 6572 7461 696e 2073 6572 7669 6365 7320  ertain services 
-00005600: 6d61 7920 696d 7065 7273 6f6e 6174 6520  may impersonate 
-00005610: 6120 5461 7069 7320 7573 6572 2e94 8c06  a Tapis user....
-00005620: 7363 6865 6d61 947d 948c 0474 7970 6594  schema.}...type.
-00005630: 8c06 7374 7269 6e67 9473 7565 8c09 7265  ..string.sue..re
-00005640: 7370 6f6e 7365 7394 7d94 8c03 3230 3094  sponses.}...200.
-00005650: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
-00005660: 948c 024f 4b94 8c07 636f 6e74 656e 7494  ...OK...content.
-00005670: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
-00005680: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
-00005690: 7d94 8c04 2472 6566 948c 2923 2f63 6f6d  }...$ref..)#/com
-000056a0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-000056b0: 5472 616e 7366 6572 5461 736b 5265 7370  TransferTaskResp
-000056c0: 6f6e 7365 9473 7373 7573 7573 8c27 2f76  onse.sssusus.'/v
-000056d0: 332f 6669 6c65 732f 7065 726d 6973 7369  3/files/permissi
-000056e0: 6f6e 732f 7b73 7973 7465 6d49 647d 2f7b  ons/{systemId}/{
-000056f0: 7061 7468 7d94 7d94 288c 0367 6574 947d  path}.}.(..get.}
-00005700: 9428 8c04 7461 6773 945d 948c 0b50 6572  .(..tags.]...Per
-00005710: 6d69 7373 696f 6e73 9461 8c0b 6465 7363  missions.a..desc
-00005720: 7269 7074 696f 6e94 8c93 4765 7420 7468  ription...Get th
-00005730: 6520 5461 7069 7320 7065 726d 6973 7369  e Tapis permissi
-00005740: 6f6e 7320 666f 7220 6120 7573 6572 2066  ons for a user f
-00005750: 6f72 2074 6865 2073 7973 7465 6d20 616e  or the system an
-00005760: 6420 7061 7468 2e0a 4966 206e 6f20 7573  d path..If no us
-00005770: 6572 2073 7065 6369 6669 6564 2074 6865  er specified the
-00005780: 6e20 7065 726d 6973 7369 6f6e 7320 6172  n permissions ar
-00005790: 6520 7265 7472 6965 7665 6420 666f 7220  e retrieved for 
-000057a0: 7468 6520 7573 6572 206d 616b 696e 6720  the user making 
-000057b0: 7468 6520 7265 7175 6573 742e 0a94 8c0b  the request.....
-000057c0: 6f70 6572 6174 696f 6e49 6494 8c0e 6765  operationId...ge
-000057d0: 7450 6572 6d69 7373 696f 6e73 948c 0a70  tPermissions...p
-000057e0: 6172 616d 6574 6572 7394 5d94 287d 9428  arameters.].(}.(
-000057f0: 8c04 6e61 6d65 948c 0873 7973 7465 6d49  ..name...systemI
-00005800: 6494 8c02 696e 948c 0470 6174 6894 8c0b  d...in...path...
-00005810: 6465 7363 7269 7074 696f 6e94 8c09 5379  description...Sy
-00005820: 7374 656d 2049 4494 8c08 7265 7175 6972  stem ID...requir
-00005830: 6564 9488 8c06 7363 6865 6d61 947d 948c  ed....schema.}..
-00005840: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-00005850: 757d 9428 8c04 6e61 6d65 948c 0470 6174  u}.(..name...pat
-00005860: 6894 8c02 696e 948c 0470 6174 6894 8c0b  h...in...path...
-00005870: 6465 7363 7269 7074 696f 6e94 8c25 5061  description..%Pa
-00005880: 7468 2072 656c 6174 6976 6520 746f 2074  th relative to t
-00005890: 6865 2073 7973 7465 6d20 2a72 6f6f 7444  he system *rootD
-000058a0: 6972 2a94 8c08 7265 7175 6972 6564 9488  ir*...required..
-000058b0: 8c06 7363 6865 6d61 947d 948c 0474 7970  ..schema.}...typ
-000058c0: 6594 8c06 7374 7269 6e67 9473 757d 9428  e...string.su}.(
-000058d0: 8c04 6e61 6d65 948c 0875 7365 726e 616d  ..name...usernam
-000058e0: 6594 8c02 696e 948c 0571 7565 7279 948c  e...in...query..
-000058f0: 0b64 6573 6372 6970 7469 6f6e 948c 1055  .description...U
-00005900: 7365 726e 616d 6520 746f 206c 6973 7494  sername to list.
-00005910: 8c06 7363 6865 6d61 947d 948c 0474 7970  ..schema.}...typ
-00005920: 6594 8c06 7374 7269 6e67 9473 7565 8c09  e...string.sue..
-00005930: 7265 7370 6f6e 7365 7394 7d94 8c03 3230  responses.}...20
-00005940: 3094 7d94 288c 0b64 6573 6372 6970 7469  0.}.(..descripti
-00005950: 6f6e 948c 0e46 696c 6550 6572 6d69 7373  on...FilePermiss
-00005960: 696f 6e94 8c07 636f 6e74 656e 7494 7d94  ion...content.}.
-00005970: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
-00005980: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
-00005990: 8c04 2472 6566 948c 2b23 2f63 6f6d 706f  ..$ref..+#/compo
-000059a0: 6e65 6e74 732f 7363 6865 6d61 732f 4669  nents/schemas/Fi
-000059b0: 6c65 5065 726d 6973 7369 6f6e 5265 7370  lePermissionResp
-000059c0: 6f6e 7365 9473 7373 7573 758c 0470 6f73  onse.sssusu..pos
-000059d0: 7494 7d94 288c 0474 6167 7394 5d94 8c0b  t.}.(..tags.]...
-000059e0: 5065 726d 6973 7369 6f6e 7394 618c 0b64  Permissions.a..d
-000059f0: 6573 6372 6970 7469 6f6e 948c 5647 7261  escription..VGra
-00005a00: 6e74 2061 6363 6573 7320 746f 2061 2070  nt access to a p
-00005a10: 6174 6820 666f 7220 6120 7573 6572 2e20  ath for a user. 
-00005a20: 4163 6365 7373 206d 6179 2062 6520 5245  Access may be RE
-00005a30: 4144 206f 7220 4d4f 4449 4659 2e20 4d4f  AD or MODIFY. MO
-00005a40: 4449 4659 2069 6d70 6c69 6573 2052 4541  DIFY implies REA
-00005a50: 442e 0a94 8c0b 6f70 6572 6174 696f 6e49  D.....operationI
-00005a60: 6494 8c10 6772 616e 7450 6572 6d69 7373  d...grantPermiss
-00005a70: 696f 6e73 948c 0a70 6172 616d 6574 6572  ions...parameter
-00005a80: 7394 5d94 287d 9428 8c04 6e61 6d65 948c  s.].(}.(..name..
-00005a90: 0873 7973 7465 6d49 6494 8c02 696e 948c  .systemId...in..
-00005aa0: 0470 6174 6894 8c0b 6465 7363 7269 7074  .path...descript
-00005ab0: 696f 6e94 8c09 5379 7374 656d 2049 4494  ion...System ID.
-00005ac0: 8c08 7265 7175 6972 6564 9488 8c06 7363  ..required....sc
-00005ad0: 6865 6d61 947d 948c 0474 7970 6594 8c06  hema.}...type...
-00005ae0: 7374 7269 6e67 9473 757d 9428 8c04 6e61  string.su}.(..na
-00005af0: 6d65 948c 0470 6174 6894 8c02 696e 948c  me...path...in..
-00005b00: 0470 6174 6894 8c0b 6465 7363 7269 7074  .path...descript
-00005b10: 696f 6e94 8c25 5061 7468 2072 656c 6174  ion..%Path relat
-00005b20: 6976 6520 746f 2074 6865 2073 7973 7465  ive to the syste
-00005b30: 6d20 2a72 6f6f 7444 6972 2a94 8c08 7265  m *rootDir*...re
-00005b40: 7175 6972 6564 9488 8c06 7363 6865 6d61  quired....schema
-00005b50: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-00005b60: 6e67 9473 7565 8c0b 7265 7175 6573 7442  ng.sue..requestB
-00005b70: 6f64 7994 7d94 288c 0763 6f6e 7465 6e74  ody.}.(..content
-00005b80: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
-00005b90: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
-00005ba0: 947d 948c 0424 7265 6694 8c2c 232f 636f  .}...$ref..,#/co
-00005bb0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-00005bc0: 2f43 7265 6174 6550 6572 6d69 7373 696f  /CreatePermissio
-00005bd0: 6e52 6571 7565 7374 9473 7373 8c08 7265  nRequest.sss..re
-00005be0: 7175 6972 6564 9488 758c 0972 6573 706f  quired..u..respo
-00005bf0: 6e73 6573 947d 948c 0332 3030 947d 9428  nses.}...200.}.(
-00005c00: 8c0b 6465 7363 7269 7074 696f 6e94 8c0e  ..description...
-00005c10: 4669 6c65 5065 726d 6973 7369 6f6e 948c  FilePermission..
-00005c20: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
-00005c30: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
-00005c40: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
-00005c50: 6694 8c2b 232f 636f 6d70 6f6e 656e 7473  f..+#/components
-00005c60: 2f73 6368 656d 6173 2f46 696c 6550 6572  /schemas/FilePer
-00005c70: 6d69 7373 696f 6e52 6573 706f 6e73 6594  missionResponse.
-00005c80: 7373 7375 7375 8c06 6465 6c65 7465 947d  sssusu..delete.}
-00005c90: 9428 8c04 7461 6773 945d 948c 0b50 6572  .(..tags.]...Per
-00005ca0: 6d69 7373 696f 6e73 9461 8c0b 6465 7363  missions.a..desc
-00005cb0: 7269 7074 696f 6e94 8c49 5265 766f 6b65  ription..IRevoke
-00005cc0: 2061 6363 6573 7320 666f 7220 6120 7573   access for a us
-00005cd0: 6572 2066 6f72 2074 6865 2073 7973 7465  er for the syste
-00005ce0: 6d20 616e 6420 7061 7468 2e20 416c 6c20  m and path. All 
-00005cf0: 6163 6365 7373 2069 7320 7265 766f 6b65  access is revoke
-00005d00: 642e 0a94 8c0b 6f70 6572 6174 696f 6e49  d.....operationI
-00005d10: 6494 8c11 6465 6c65 7465 5065 726d 6973  d...deletePermis
-00005d20: 7369 6f6e 7394 8c0a 7061 7261 6d65 7465  sions...paramete
-00005d30: 7273 945d 9428 7d94 288c 046e 616d 6594  rs.].(}.(..name.
-00005d40: 8c08 7379 7374 656d 4964 948c 0269 6e94  ..systemId...in.
-00005d50: 8c04 7061 7468 948c 0b64 6573 6372 6970  ..path...descrip
-00005d60: 7469 6f6e 948c 0953 7973 7465 6d20 4944  tion...System ID
-00005d70: 948c 0872 6571 7569 7265 6494 888c 0673  ...required....s
-00005d80: 6368 656d 6194 7d94 8c04 7479 7065 948c  chema.}...type..
-00005d90: 0673 7472 696e 6794 7375 7d94 288c 046e  .string.su}.(..n
-00005da0: 616d 6594 8c04 7061 7468 948c 0269 6e94  ame...path...in.
-00005db0: 8c04 7061 7468 948c 0b64 6573 6372 6970  ..path...descrip
-00005dc0: 7469 6f6e 948c 2550 6174 6820 7265 6c61  tion..%Path rela
-00005dd0: 7469 7665 2074 6f20 7468 6520 7379 7374  tive to the syst
-00005de0: 656d 202a 726f 6f74 4469 722a 948c 0872  em *rootDir*...r
-00005df0: 6571 7569 7265 6494 888c 0673 6368 656d  equired....schem
-00005e00: 6194 7d94 8c04 7479 7065 948c 0673 7472  a.}...type...str
-00005e10: 696e 6794 7375 7d94 288c 046e 616d 6594  ing.su}.(..name.
-00005e20: 8c08 7573 6572 6e61 6d65 948c 0269 6e94  ..username...in.
-00005e30: 8c05 7175 6572 7994 8c0b 6465 7363 7269  ..query...descri
-00005e40: 7074 696f 6e94 8c12 5573 6572 6e61 6d65  ption...Username
-00005e50: 2074 6f20 7265 6d6f 7665 948c 0872 6571   to remove...req
-00005e60: 7569 7265 6494 888c 0673 6368 656d 6194  uired....schema.
-00005e70: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
-00005e80: 6794 7375 658c 0972 6573 706f 6e73 6573  g.sue..responses
-00005e90: 947d 948c 0332 3030 947d 9428 8c0b 6465  .}...200.}.(..de
-00005ea0: 7363 7269 7074 696f 6e94 8c0e 4669 6c65  scription...File
-00005eb0: 5065 726d 6973 7369 6f6e 948c 0763 6f6e  Permission...con
-00005ec0: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
-00005ed0: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
-00005ee0: 6865 6d61 947d 948c 0424 7265 6694 8c23  hema.}...$ref..#
-00005ef0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
-00005f00: 656d 6173 2f53 7472 696e 6752 6573 706f  emas/StringRespo
-00005f10: 6e73 6594 7373 7375 7375 758c 212f 7633  nse.sssusuu.!/v3
-00005f20: 2f66 696c 6573 2f73 6861 7265 2f7b 7379  /files/share/{sy
-00005f30: 7374 656d 4964 7d2f 7b70 6174 687d 947d  stemId}/{path}.}
-00005f40: 9428 8c03 6765 7494 7d94 288c 0474 6167  .(..get.}.(..tag
-00005f50: 7394 5d94 8c07 5368 6172 696e 6794 618c  s.]...Sharing.a.
-00005f60: 0773 756d 6d61 7279 948c 3752 6574 7269  .summary..7Retri
-00005f70: 6576 6520 616c 6c20 7368 6172 696e 6720  eve all sharing 
-00005f80: 696e 666f 726d 6174 696f 6e20 666f 7220  information for 
-00005f90: 6120 7061 7468 206f 6e20 6120 7379 7374  a path on a syst
-00005fa0: 656d 948c 0b64 6573 6372 6970 7469 6f6e  em...description
-00005fb0: 948c b252 6574 7269 6576 6520 616c 6c20  ...Retrieve all 
-00005fc0: 7368 6172 696e 6720 696e 666f 726d 6174  sharing informat
-00005fd0: 696f 6e20 666f 7220 6120 7061 7468 206f  ion for a path o
-00005fe0: 6e20 6120 7379 7374 656d 2e20 5468 6973  n a system. This
-00005ff0: 2069 6e63 6c75 6465 7320 616c 6c20 7573   includes all us
-00006000: 6572 7320 7769 7468 2077 686f 6d20 7468  ers with whom th
-00006010: 6520 7061 7468 0a68 6173 2062 6565 6e20  e path.has been 
-00006020: 7368 6172 6564 2061 6e64 2077 6865 7468  shared and wheth
-00006030: 6572 206f 7220 6e6f 7420 7468 6520 7061  er or not the pa
-00006040: 7468 2068 6173 2062 6565 6e20 6d61 6465  th has been made
-00006050: 2070 7562 6c69 636c 7920 6176 6169 6c61   publicly availa
-00006060: 626c 652e 0a94 8c0b 6f70 6572 6174 696f  ble.....operatio
-00006070: 6e49 6494 8c0c 6765 7453 6861 7265 496e  nId...getShareIn
-00006080: 666f 948c 0a70 6172 616d 6574 6572 7394  fo...parameters.
-00006090: 5d94 287d 9428 8c04 6e61 6d65 948c 0873  ].(}.(..name...s
-000060a0: 7973 7465 6d49 6494 8c02 696e 948c 0470  ystemId...in...p
-000060b0: 6174 6894 8c08 7265 7175 6972 6564 9488  ath...required..
-000060c0: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
-000060d0: 6694 8c1d 232f 636f 6d70 6f6e 656e 7473  f...#/components
-000060e0: 2f73 6368 656d 6173 2f49 6453 7472 696e  /schemas/IdStrin
-000060f0: 6794 7375 7d94 288c 046e 616d 6594 8c04  g.su}.(..name...
-00006100: 7061 7468 948c 0269 6e94 8c04 7061 7468  path...in...path
-00006110: 948c 0872 6571 7569 7265 6494 888c 0673  ...required....s
-00006120: 6368 656d 6194 7d94 8c04 7479 7065 948c  chema.}...type..
-00006130: 0673 7472 696e 6794 7375 658c 0972 6573  .string.sue..res
-00006140: 706f 6e73 6573 947d 9428 8c03 3230 3094  ponses.}.(..200.
-00006150: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
-00006160: 948c 0853 7563 6365 7373 2e94 8c07 636f  ...Success....co
-00006170: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
-00006180: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
-00006190: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
-000061a0: 2223 2f63 6f6d 706f 6e65 6e74 732f 7363  "#/components/sc
-000061b0: 6865 6d61 732f 5265 7370 5368 6172 6549  hemas/RespShareI
-000061c0: 6e66 6f94 7373 7375 8c03 3430 3094 7d94  nfo.sssu..400.}.
-000061d0: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
-000061e0: 0c49 6e70 7574 2065 7272 6f72 2e94 8c07  .Input error....
-000061f0: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
-00006200: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
-00006210: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
-00006220: 948c 1e23 2f63 6f6d 706f 6e65 6e74 732f  ...#/components/
-00006230: 7363 6865 6d61 732f 5265 7370 4261 7369  schemas/RespBasi
-00006240: 6394 7373 7375 8c03 3430 3394 7d94 288c  c.sssu..403.}.(.
-00006250: 0b64 6573 6372 6970 7469 6f6e 948c 1150  .description...P
-00006260: 6572 6d69 7373 696f 6e20 4465 6e69 6564  ermission Denied
-00006270: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
-00006280: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
-00006290: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
-000062a0: 7265 6694 8c1e 232f 636f 6d70 6f6e 656e  ref...#/componen
-000062b0: 7473 2f73 6368 656d 6173 2f52 6573 7042  ts/schemas/RespB
-000062c0: 6173 6963 9473 7373 758c 0334 3034 947d  asic.sssu..404.}
-000062d0: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
-000062e0: 8c11 5379 7374 656d 206e 6f74 2066 6f75  ..System not fou
-000062f0: 6e64 2e94 8c07 636f 6e74 656e 7494 7d94  nd....content.}.
-00006300: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
-00006310: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
-00006320: 8c04 2472 6566 948c 1e23 2f63 6f6d 706f  ..$ref...#/compo
-00006330: 6e65 6e74 732f 7363 6865 6d61 732f 5265  nents/schemas/Re
-00006340: 7370 4261 7369 6394 7373 7375 8c03 3530  spBasic.sssu..50
-00006350: 3094 7d94 288c 0b64 6573 6372 6970 7469  0.}.(..descripti
-00006360: 6f6e 948c 0d53 6572 7665 7220 6572 726f  on...Server erro
-00006370: 722e 948c 0763 6f6e 7465 6e74 947d 948c  r....content.}..
-00006380: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
-00006390: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
-000063a0: 0424 7265 6694 8c1e 232f 636f 6d70 6f6e  .$ref...#/compon
-000063b0: 656e 7473 2f73 6368 656d 6173 2f52 6573  ents/schemas/Res
-000063c0: 7042 6173 6963 9473 7373 7575 758c 0470  pBasic.sssuuu..p
-000063d0: 6f73 7494 7d94 288c 0474 6167 7394 5d94  ost.}.(..tags.].
-000063e0: 8c07 5368 6172 696e 6794 618c 0773 756d  ..Sharing.a..sum
-000063f0: 6d61 7279 948c 3053 6861 7265 2061 2070  mary..0Share a p
-00006400: 6174 6820 6f6e 2061 2073 7973 7465 6d20  ath on a system 
-00006410: 7769 7468 206f 6e65 206f 7220 6d6f 7265  with one or more
-00006420: 2075 7365 7273 2e94 8c0b 6465 7363 7269   users....descri
-00006430: 7074 696f 6e94 8ce1 4372 6561 7465 206f  ption...Create o
-00006440: 7220 7570 6461 7465 2073 6861 7269 6e67  r update sharing
-00006450: 2069 6e66 6f72 6d61 7469 6f6e 2066 6f72   information for
-00006460: 2061 2070 6174 6820 6f6e 2061 2073 7973   a path on a sys
-00006470: 7465 6d2e 2054 6865 2070 6174 6820 7769  tem. The path wi
-00006480: 6c6c 2062 6520 7368 6172 6564 2077 6974  ll be shared wit
-00006490: 6820 7468 6520 6c69 7374 206f 6620 7573  h the list of us
-000064a0: 6572 730a 7072 6f76 6964 6564 2069 6e20  ers.provided in 
-000064b0: 7468 6520 7265 7175 6573 7420 626f 6479  the request body
-000064c0: 2e20 5265 7175 6573 7465 7220 6d75 7374  . Requester must
-000064d0: 2062 6520 6f77 6e65 7220 6f66 2074 6865   be owner of the
-000064e0: 2073 7973 7465 6d2e 2046 6f72 204c 494e   system. For LIN
-000064f0: 5558 2073 7973 7465 6d73 2070 6174 6820  UX systems path 
-00006500: 7368 6172 696e 6720 6973 0a68 6965 7261  sharing is.hiera
-00006510: 7263 6869 6361 6c2e 0a94 8c0b 6f70 6572  rchical.....oper
-00006520: 6174 696f 6e49 6494 8c09 7368 6172 6550  ationId...shareP
-00006530: 6174 6894 8c0a 7061 7261 6d65 7465 7273  ath...parameters
-00006540: 945d 9428 7d94 288c 046e 616d 6594 8c08  .].(}.(..name...
-00006550: 7379 7374 656d 4964 948c 0269 6e94 8c04  systemId...in...
-00006560: 7061 7468 948c 0872 6571 7569 7265 6494  path...required.
-00006570: 888c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
-00006580: 6566 948c 1d23 2f63 6f6d 706f 6e65 6e74  ef...#/component
-00006590: 732f 7363 6865 6d61 732f 4964 5374 7269  s/schemas/IdStri
-000065a0: 6e67 9473 757d 9428 8c04 6e61 6d65 948c  ng.su}.(..name..
-000065b0: 0470 6174 6894 8c02 696e 948c 0470 6174  .path...in...pat
-000065c0: 6894 8c08 7265 7175 6972 6564 9488 8c06  h...required....
-000065d0: 7363 6865 6d61 947d 948c 0474 7970 6594  schema.}...type.
-000065e0: 8c06 7374 7269 6e67 9473 7565 8c0b 7265  ..string.sue..re
-000065f0: 7175 6573 7442 6f64 7994 7d94 288c 0872  questBody.}.(..r
-00006600: 6571 7569 7265 6494 888c 0b64 6573 6372  equired....descr
-00006610: 6970 7469 6f6e 948c 3541 204a 534f 4e20  iption..5A JSON 
-00006620: 6f62 6a65 6374 2073 7065 6369 6679 696e  object specifyin
-00006630: 6720 7570 6461 7465 6420 7368 6172 696e  g updated sharin
-00006640: 6720 696e 666f 726d 6174 696f 6e2e 948c  g information...
-00006650: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
-00006660: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
-00006670: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
-00006680: 6694 8c23 232f 636f 6d70 6f6e 656e 7473  f..##/components
-00006690: 2f73 6368 656d 6173 2f52 6571 5368 6172  /schemas/ReqShar
-000066a0: 6555 7064 6174 6594 7373 7375 8c09 7265  eUpdate.sssu..re
-000066b0: 7370 6f6e 7365 7394 7d94 288c 0332 3030  sponses.}.(..200
-000066c0: 947d 9428 8c0b 6465 7363 7269 7074 696f  .}.(..descriptio
-000066d0: 6e94 8c1c 5368 6172 696e 6720 696e 666f  n...Sharing info
-000066e0: 726d 6174 696f 6e20 7570 6461 7465 642e  rmation updated.
-000066f0: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
-00006700: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
-00006710: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
-00006720: 7265 6694 8c1e 232f 636f 6d70 6f6e 656e  ref...#/componen
-00006730: 7473 2f73 6368 656d 6173 2f52 6573 7042  ts/schemas/RespB
-00006740: 6173 6963 9473 7373 758c 0334 3030 947d  asic.sssu..400.}
-00006750: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
-00006760: 8c1a 496e 7075 7420 6572 726f 722e 2049  ..Input error. I
-00006770: 6e76 616c 6964 204a 534f 4e2e 948c 0763  nvalid JSON....c
-00006780: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
-00006790: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
-000067a0: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
-000067b0: 8c1e 232f 636f 6d70 6f6e 656e 7473 2f73  ..#/components/s
-000067c0: 6368 656d 6173 2f52 6573 7042 6173 6963  chemas/RespBasic
-000067d0: 9473 7373 758c 0334 3033 947d 9428 8c0b  .sssu..403.}.(..
-000067e0: 6465 7363 7269 7074 696f 6e94 8c11 5065  description...Pe
-000067f0: 726d 6973 7369 6f6e 2044 656e 6965 6494  rmission Denied.
-00006800: 8c07 636f 6e74 656e 7494 7d94 8c10 6170  ..content.}...ap
-00006810: 706c 6963 6174 696f 6e2f 6a73 6f6e 947d  plication/json.}
-00006820: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
-00006830: 6566 948c 1e23 2f63 6f6d 706f 6e65 6e74  ef...#/component
-00006840: 732f 7363 6865 6d61 732f 5265 7370 4261  s/schemas/RespBa
-00006850: 7369 6394 7373 7375 8c03 3530 3094 7d94  sic.sssu..500.}.
-00006860: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
-00006870: 0d53 6572 7665 7220 6572 726f 722e 948c  .Server error...
-00006880: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
-00006890: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
-000068a0: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
-000068b0: 6694 8c1e 232f 636f 6d70 6f6e 656e 7473  f...#/components
-000068c0: 2f73 6368 656d 6173 2f52 6573 7042 6173  /schemas/RespBas
-000068d0: 6963 9473 7373 7575 7575 8c28 2f76 332f  ic.sssuuuu.(/v3/
-000068e0: 6669 6c65 732f 7368 6172 655f 7075 626c  files/share_publ
-000068f0: 6963 2f7b 7379 7374 656d 4964 7d2f 7b70  ic/{systemId}/{p
-00006900: 6174 687d 947d 948c 0470 6f73 7494 7d94  ath}.}...post.}.
-00006910: 288c 0474 6167 7394 5d94 8c07 5368 6172  (..tags.]...Shar
-00006920: 696e 6794 618c 0773 756d 6d61 7279 948c  ing.a..summary..
-00006930: 3f53 6861 7265 2061 2070 6174 6820 6f6e  ?Share a path on
-00006940: 2061 2073 7973 7465 6d20 7075 626c 6963   a system public
-00006950: 6c79 2077 6974 6820 616c 6c20 7573 6572  ly with all user
-00006960: 7320 696e 2074 6865 2074 656e 616e 742e  s in the tenant.
-00006970: 948c 0b64 6573 6372 6970 7469 6f6e 948c  ...description..
-00006980: 5e53 6861 7265 2061 2070 6174 6820 6f6e  ^Share a path on
-00006990: 2061 2073 7973 7465 6d20 7769 7468 2061   a system with a
-000069a0: 6c6c 2075 7365 7273 2069 6e20 7468 6520  ll users in the 
-000069b0: 7465 6e61 6e74 2e20 5265 7175 6573 7465  tenant. Requeste
-000069c0: 7220 6d75 7374 2062 6520 6f77 6e65 7220  r must be owner 
-000069d0: 6f66 2074 6865 2073 7973 7465 6d2e 0a94  of the system...
-000069e0: 8c0b 6f70 6572 6174 696f 6e49 6494 8c0f  ..operationId...
-000069f0: 7368 6172 6550 6174 6850 7562 6c69 6394  sharePathPublic.
-00006a00: 8c0a 7061 7261 6d65 7465 7273 945d 9428  ..parameters.].(
-00006a10: 7d94 288c 046e 616d 6594 8c08 7379 7374  }.(..name...syst
-00006a20: 656d 4964 948c 0269 6e94 8c04 7061 7468  emId...in...path
-00006a30: 948c 0872 6571 7569 7265 6494 888c 0673  ...required....s
-00006a40: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
-00006a50: 1d23 2f63 6f6d 706f 6e65 6e74 732f 7363  .#/components/sc
-00006a60: 6865 6d61 732f 4964 5374 7269 6e67 9473  hemas/IdString.s
-00006a70: 757d 9428 8c04 6e61 6d65 948c 0470 6174  u}.(..name...pat
-00006a80: 6894 8c02 696e 948c 0470 6174 6894 8c08  h...in...path...
-00006a90: 7265 7175 6972 6564 9488 8c06 7363 6865  required....sche
-00006aa0: 6d61 947d 948c 0474 7970 6594 8c06 7374  ma.}...type...st
-00006ab0: 7269 6e67 9473 7565 8c09 7265 7370 6f6e  ring.sue..respon
-00006ac0: 7365 7394 7d94 288c 0332 3030 947d 9428  ses.}.(..200.}.(
-00006ad0: 8c0b 6465 7363 7269 7074 696f 6e94 8c15  ..description...
-00006ae0: 5061 7468 2073 6861 7265 6420 7075 626c  Path shared publ
-00006af0: 6963 6c79 2e94 8c07 636f 6e74 656e 7494  icly....content.
-00006b00: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
-00006b10: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
-00006b20: 7d94 8c04 2472 6566 948c 1e23 2f63 6f6d  }...$ref...#/com
-00006b30: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-00006b40: 5265 7370 4261 7369 6394 7373 7375 8c03  RespBasic.sssu..
-00006b50: 3430 3394 7d94 288c 0b64 6573 6372 6970  403.}.(..descrip
-00006b60: 7469 6f6e 948c 1150 6572 6d69 7373 696f  tion...Permissio
-00006b70: 6e20 4465 6e69 6564 948c 0763 6f6e 7465  n Denied...conte
-00006b80: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
-00006b90: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
-00006ba0: 6d61 947d 948c 0424 7265 6694 8c1e 232f  ma.}...$ref...#/
-00006bb0: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-00006bc0: 6173 2f52 6573 7042 6173 6963 9473 7373  as/RespBasic.sss
-00006bd0: 758c 0335 3030 947d 9428 8c0b 6465 7363  u..500.}.(..desc
-00006be0: 7269 7074 696f 6e94 8c0d 5365 7276 6572  ription...Server
-00006bf0: 2065 7272 6f72 2e94 8c07 636f 6e74 656e   error....conten
-00006c00: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
-00006c10: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
-00006c20: 6194 7d94 8c04 2472 6566 948c 1e23 2f63  a.}...$ref...#/c
-00006c30: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
-00006c40: 732f 5265 7370 4261 7369 6394 7373 7375  s/RespBasic.sssu
-00006c50: 7575 738c 232f 7633 2f66 696c 6573 2f75  uus.#/v3/files/u
-00006c60: 6e73 6861 7265 2f7b 7379 7374 656d 4964  nshare/{systemId
-00006c70: 7d2f 7b70 6174 687d 947d 948c 0470 6f73  }/{path}.}...pos
-00006c80: 7494 7d94 288c 0474 6167 7394 5d94 8c07  t.}.(..tags.]...
-00006c90: 5368 6172 696e 6794 618c 0773 756d 6d61  Sharing.a..summa
-00006ca0: 7279 948c 3255 6e73 6861 7265 2061 2070  ry..2Unshare a p
-00006cb0: 6174 6820 6f6e 2061 2073 7973 7465 6d20  ath on a system 
-00006cc0: 7769 7468 206f 6e65 206f 7220 6d6f 7265  with one or more
-00006cd0: 2075 7365 7273 2e94 8c0b 6465 7363 7269   users....descri
-00006ce0: 7074 696f 6e94 8cb3 4372 6561 7465 206f  ption...Create o
-00006cf0: 7220 7570 6461 7465 2073 6861 7269 6e67  r update sharing
-00006d00: 2069 6e66 6f72 6d61 7469 6f6e 2066 6f72   information for
-00006d10: 2061 2070 6174 6820 6f6e 2061 2073 7973   a path on a sys
-00006d20: 7465 6d2e 2054 6865 2070 6174 6820 7769  tem. The path wi
-00006d30: 6c6c 2062 6520 756e 7368 6172 6564 2077  ll be unshared w
-00006d40: 6974 6820 7468 6520 6c69 7374 206f 6620  ith the list of 
-00006d50: 7573 6572 730a 7072 6f76 6964 6564 2069  users.provided i
-00006d60: 6e20 7468 6520 7265 7175 6573 7420 626f  n the request bo
-00006d70: 6479 2e20 5265 7175 6573 7465 7220 6d75  dy. Requester mu
-00006d80: 7374 2062 6520 6f77 6e65 7220 6f66 2074  st be owner of t
-00006d90: 6865 2073 7973 7465 6d2e 0a94 8c0b 6f70  he system.....op
-00006da0: 6572 6174 696f 6e49 6494 8c0b 756e 5368  erationId...unSh
-00006db0: 6172 6550 6174 6894 8c0a 7061 7261 6d65  arePath...parame
-00006dc0: 7465 7273 945d 9428 7d94 288c 046e 616d  ters.].(}.(..nam
-00006dd0: 6594 8c08 7379 7374 656d 4964 948c 0269  e...systemId...i
-00006de0: 6e94 8c04 7061 7468 948c 0872 6571 7569  n...path...requi
-00006df0: 7265 6494 888c 0673 6368 656d 6194 7d94  red....schema.}.
-00006e00: 8c04 2472 6566 948c 1d23 2f63 6f6d 706f  ..$ref...#/compo
-00006e10: 6e65 6e74 732f 7363 6865 6d61 732f 4964  nents/schemas/Id
-00006e20: 5374 7269 6e67 9473 757d 9428 8c04 6e61  String.su}.(..na
-00006e30: 6d65 948c 0470 6174 6894 8c02 696e 948c  me...path...in..
-00006e40: 0470 6174 6894 8c08 7265 7175 6972 6564  .path...required
-00006e50: 9488 8c06 7363 6865 6d61 947d 948c 0474  ....schema.}...t
-00006e60: 7970 6594 8c06 7374 7269 6e67 9473 7565  ype...string.sue
-00006e70: 8c0b 7265 7175 6573 7442 6f64 7994 7d94  ..requestBody.}.
-00006e80: 288c 0872 6571 7569 7265 6494 888c 0b64  (..required....d
-00006e90: 6573 6372 6970 7469 6f6e 948c 3541 204a  escription..5A J
-00006ea0: 534f 4e20 6f62 6a65 6374 2073 7065 6369  SON object speci
-00006eb0: 6679 696e 6720 7570 6461 7465 6420 7368  fying updated sh
-00006ec0: 6172 696e 6720 696e 666f 726d 6174 696f  aring informatio
-00006ed0: 6e2e 948c 0763 6f6e 7465 6e74 947d 948c  n....content.}..
-00006ee0: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
-00006ef0: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
-00006f00: 0424 7265 6694 8c23 232f 636f 6d70 6f6e  .$ref..##/compon
-00006f10: 656e 7473 2f73 6368 656d 6173 2f52 6571  ents/schemas/Req
-00006f20: 5368 6172 6555 7064 6174 6594 7373 7375  ShareUpdate.sssu
-00006f30: 8c09 7265 7370 6f6e 7365 7394 7d94 288c  ..responses.}.(.
-00006f40: 0332 3030 947d 9428 8c0b 6465 7363 7269  .200.}.(..descri
-00006f50: 7074 696f 6e94 8c1c 5368 6172 696e 6720  ption...Sharing 
-00006f60: 696e 666f 726d 6174 696f 6e20 7570 6461  information upda
-00006f70: 7465 642e 948c 0763 6f6e 7465 6e74 947d  ted....content.}
-00006f80: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
-00006f90: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
-00006fa0: 948c 0424 7265 6694 8c1e 232f 636f 6d70  ...$ref...#/comp
-00006fb0: 6f6e 656e 7473 2f73 6368 656d 6173 2f52  onents/schemas/R
-00006fc0: 6573 7042 6173 6963 9473 7373 758c 0334  espBasic.sssu..4
-00006fd0: 3030 947d 9428 8c0b 6465 7363 7269 7074  00.}.(..descript
-00006fe0: 696f 6e94 8c1a 496e 7075 7420 6572 726f  ion...Input erro
-00006ff0: 722e 2049 6e76 616c 6964 204a 534f 4e2e  r. Invalid JSON.
-00007000: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
-00007010: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
-00007020: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
-00007030: 7265 6694 8c1e 232f 636f 6d70 6f6e 656e  ref...#/componen
-00007040: 7473 2f73 6368 656d 6173 2f52 6573 7042  ts/schemas/RespB
-00007050: 6173 6963 9473 7373 758c 0334 3033 947d  asic.sssu..403.}
-00007060: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
-00007070: 8c11 5065 726d 6973 7369 6f6e 2044 656e  ..Permission Den
-00007080: 6965 6494 8c07 636f 6e74 656e 7494 7d94  ied...content.}.
-00007090: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
-000070a0: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
-000070b0: 8c04 2472 6566 948c 1e23 2f63 6f6d 706f  ..$ref...#/compo
-000070c0: 6e65 6e74 732f 7363 6865 6d61 732f 5265  nents/schemas/Re
-000070d0: 7370 4261 7369 6394 7373 7375 8c03 3530  spBasic.sssu..50
-000070e0: 3094 7d94 288c 0b64 6573 6372 6970 7469  0.}.(..descripti
-000070f0: 6f6e 948c 0d53 6572 7665 7220 6572 726f  on...Server erro
-00007100: 722e 948c 0763 6f6e 7465 6e74 947d 948c  r....content.}..
-00007110: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
-00007120: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
-00007130: 0424 7265 6694 8c1e 232f 636f 6d70 6f6e  .$ref...#/compon
-00007140: 656e 7473 2f73 6368 656d 6173 2f52 6573  ents/schemas/Res
-00007150: 7042 6173 6963 9473 7373 7575 7573 8c2a  pBasic.sssuuus.*
-00007160: 2f76 332f 6669 6c65 732f 756e 7368 6172  /v3/files/unshar
-00007170: 655f 7075 626c 6963 2f7b 7379 7374 656d  e_public/{system
-00007180: 4964 7d2f 7b70 6174 687d 947d 948c 0470  Id}/{path}.}...p
-00007190: 6f73 7494 7d94 288c 0474 6167 7394 5d94  ost.}.(..tags.].
-000071a0: 8c07 5368 6172 696e 6794 618c 0773 756d  ..Sharing.a..sum
-000071b0: 6d61 7279 948c 2c52 656d 6f76 6520 7075  mary..,Remove pu
-000071c0: 626c 6963 2061 6363 6573 7320 666f 7220  blic access for 
-000071d0: 6120 7061 7468 206f 6e20 6120 7379 7374  a path on a syst
-000071e0: 656d 2e94 8c0b 6465 7363 7269 7074 696f  em....descriptio
-000071f0: 6e94 8c55 5265 6d6f 7665 2070 7562 6c69  n..URemove publi
-00007200: 6320 7368 6172 696e 6720 666f 7220 6120  c sharing for a 
-00007210: 7061 7468 206f 6e20 6120 7379 7374 656d  path on a system
-00007220: 2e20 5265 7175 6573 7465 7220 6d75 7374  . Requester must
-00007230: 2062 6520 6f77 6e65 7220 6f66 2074 6865   be owner of the
-00007240: 2073 7973 7465 6d2e 0a94 8c0b 6f70 6572   system.....oper
-00007250: 6174 696f 6e49 6494 8c11 756e 5368 6172  ationId...unShar
-00007260: 6550 6174 6850 7562 6c69 6394 8c0a 7061  ePathPublic...pa
-00007270: 7261 6d65 7465 7273 945d 9428 7d94 288c  rameters.].(}.(.
-00007280: 046e 616d 6594 8c08 7379 7374 656d 4964  .name...systemId
-00007290: 948c 0269 6e94 8c04 7061 7468 948c 0872  ...in...path...r
-000072a0: 6571 7569 7265 6494 888c 0673 6368 656d  equired....schem
-000072b0: 6194 7d94 8c04 2472 6566 948c 1d23 2f63  a.}...$ref...#/c
-000072c0: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
-000072d0: 732f 4964 5374 7269 6e67 9473 757d 9428  s/IdString.su}.(
-000072e0: 8c04 6e61 6d65 948c 0470 6174 6894 8c02  ..name...path...
-000072f0: 696e 948c 0470 6174 6894 8c08 7265 7175  in...path...requ
-00007300: 6972 6564 9488 8c06 7363 6865 6d61 947d  ired....schema.}
-00007310: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-00007320: 9473 7565 8c09 7265 7370 6f6e 7365 7394  .sue..responses.
-00007330: 7d94 288c 0332 3030 947d 9428 8c0b 6465  }.(..200.}.(..de
-00007340: 7363 7269 7074 696f 6e94 8c1b 5061 7468  scription...Path
-00007350: 2070 7562 6c69 6320 6163 6365 7373 2072   public access r
-00007360: 656d 6f76 6564 2e94 8c07 636f 6e74 656e  emoved....conten
-00007370: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
-00007380: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
-00007390: 6194 7d94 8c04 2472 6566 948c 1e23 2f63  a.}...$ref...#/c
-000073a0: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
-000073b0: 732f 5265 7370 4261 7369 6394 7373 7375  s/RespBasic.sssu
-000073c0: 8c03 3430 3394 7d94 288c 0b64 6573 6372  ..403.}.(..descr
-000073d0: 6970 7469 6f6e 948c 1150 6572 6d69 7373  iption...Permiss
-000073e0: 696f 6e20 4465 6e69 6564 948c 0763 6f6e  ion Denied...con
-000073f0: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
-00007400: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
-00007410: 6865 6d61 947d 948c 0424 7265 6694 8c1e  hema.}...$ref...
-00007420: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
-00007430: 656d 6173 2f52 6573 7042 6173 6963 9473  emas/RespBasic.s
-00007440: 7373 758c 0335 3030 947d 9428 8c0b 6465  ssu..500.}.(..de
-00007450: 7363 7269 7074 696f 6e94 8c0d 5365 7276  scription...Serv
-00007460: 6572 2065 7272 6f72 2e94 8c07 636f 6e74  er error....cont
-00007470: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
-00007480: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
-00007490: 656d 6194 7d94 8c04 2472 6566 948c 1e23  ema.}...$ref...#
-000074a0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-000074b0: 6d61 732f 5265 7370 4261 7369 6394 7373  mas/RespBasic.ss
-000074c0: 7375 7575 738c 272f 7633 2f66 696c 6573  suuus.'/v3/files
-000074d0: 2f75 6e73 6861 7265 5f61 6c6c 2f7b 7379  /unshare_all/{sy
-000074e0: 7374 656d 4964 7d2f 7b70 6174 687d 947d  stemId}/{path}.}
-000074f0: 948c 0470 6f73 7494 7d94 288c 0474 6167  ...post.}.(..tag
-00007500: 7394 5d94 8c07 5368 6172 696e 6794 618c  s.]...Sharing.a.
-00007510: 0773 756d 6d61 7279 948c 4152 656d 6f76  .summary..ARemov
-00007520: 6520 616c 6c20 7368 6172 6573 2066 6f72  e all shares for
-00007530: 2061 2070 6174 6820 6f6e 2061 2073 7973   a path on a sys
-00007540: 7465 6d20 696e 636c 7564 696e 6720 7075  tem including pu
-00007550: 626c 6963 2061 6363 6573 732e 948c 0b64  blic access....d
-00007560: 6573 6372 6970 7469 6f6e 948c 6c52 656d  escription..lRem
-00007570: 6f76 6520 616c 6c20 7368 6172 6573 2066  ove all shares f
-00007580: 6f72 2061 2070 6174 6820 6f6e 2061 2073  or a path on a s
-00007590: 7973 7465 6d20 696e 636c 7564 696e 6720  ystem including 
-000075a0: 7075 626c 6963 2061 6363 6573 732e 2054  public access. T
-000075b0: 6869 7320 7769 6c6c 2061 6c73 6f20 6265  his will also be
-000075c0: 2064 6f6e 6520 666f 7220 616c 6c20 7375   done for all su
-000075d0: 622d 7061 7468 732e 0a94 8c0b 6f70 6572  b-paths.....oper
-000075e0: 6174 696f 6e49 6494 8c0e 756e 5368 6172  ationId...unShar
-000075f0: 6550 6174 6841 6c6c 948c 0a70 6172 616d  ePathAll...param
-00007600: 6574 6572 7394 5d94 287d 9428 8c04 6e61  eters.].(}.(..na
-00007610: 6d65 948c 0873 7973 7465 6d49 6494 8c02  me...systemId...
-00007620: 696e 948c 0470 6174 6894 8c08 7265 7175  in...path...requ
-00007630: 6972 6564 9488 8c06 7363 6865 6d61 947d  ired....schema.}
-00007640: 948c 0424 7265 6694 8c1d 232f 636f 6d70  ...$ref...#/comp
-00007650: 6f6e 656e 7473 2f73 6368 656d 6173 2f49  onents/schemas/I
-00007660: 6453 7472 696e 6794 7375 7d94 288c 046e  dString.su}.(..n
-00007670: 616d 6594 8c04 7061 7468 948c 0269 6e94  ame...path...in.
-00007680: 8c04 7061 7468 948c 0872 6571 7569 7265  ..path...require
-00007690: 6494 888c 0673 6368 656d 6194 7d94 8c04  d....schema.}...
-000076a0: 7479 7065 948c 0673 7472 696e 6794 7375  type...string.su
-000076b0: 7d94 288c 046e 616d 6594 8c07 7265 6375  }.(..name...recu
-000076c0: 7273 6594 8c02 696e 948c 0571 7565 7279  rse...in...query
-000076d0: 948c 0872 6571 7569 7265 6494 898c 0673  ...required....s
-000076e0: 6368 656d 6194 7d94 288c 0474 7970 6594  chema.}.(..type.
-000076f0: 8c07 626f 6f6c 6561 6e94 8c07 6465 6661  ..boolean...defa
-00007700: 756c 7494 8975 7565 8c09 7265 7370 6f6e  ult..uue..respon
-00007710: 7365 7394 7d94 288c 0332 3030 947d 9428  ses.}.(..200.}.(
-00007720: 8c0b 6465 7363 7269 7074 696f 6e94 8c19  ..description...
-00007730: 416c 6c20 7368 6172 6520 6163 6365 7373  All share access
-00007740: 2072 656d 6f76 6564 2e94 8c07 636f 6e74   removed....cont
-00007750: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
-00007760: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
-00007770: 656d 6194 7d94 8c04 2472 6566 948c 1e23  ema.}...$ref...#
-00007780: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-00007790: 6d61 732f 5265 7370 4261 7369 6394 7373  mas/RespBasic.ss
-000077a0: 7375 8c03 3430 3394 7d94 288c 0b64 6573  su..403.}.(..des
-000077b0: 6372 6970 7469 6f6e 948c 1150 6572 6d69  cription...Permi
-000077c0: 7373 696f 6e20 4465 6e69 6564 948c 0763  ssion Denied...c
-000077d0: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
-000077e0: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
-000077f0: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
-00007800: 8c1e 232f 636f 6d70 6f6e 656e 7473 2f73  ..#/components/s
-00007810: 6368 656d 6173 2f52 6573 7042 6173 6963  chemas/RespBasic
-00007820: 9473 7373 758c 0335 3030 947d 9428 8c0b  .sssu..500.}.(..
-00007830: 6465 7363 7269 7074 696f 6e94 8c0d 5365  description...Se
-00007840: 7276 6572 2065 7272 6f72 2e94 8c07 636f  rver error....co
-00007850: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
-00007860: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
-00007870: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
-00007880: 1e23 2f63 6f6d 706f 6e65 6e74 732f 7363  .#/components/sc
-00007890: 6865 6d61 732f 5265 7370 4261 7369 6394  hemas/RespBasic.
-000078a0: 7373 7375 7575 738c 232f 7633 2f66 696c  sssuuus.#/v3/fil
-000078b0: 6573 2f70 6f73 7469 7473 2f7b 7379 7374  es/postits/{syst
-000078c0: 656d 4964 7d2f 7b70 6174 687d 947d 948c  emId}/{path}.}..
-000078d0: 0470 6f73 7494 7d94 288c 0773 756d 6d61  .post.}.(..summa
-000078e0: 7279 948c 0f43 7265 6174 6520 6120 506f  ry...Create a Po
-000078f0: 7374 4974 948c 0474 6167 7394 5d94 8c07  stIt...tags.]...
-00007900: 506f 7374 4974 7394 618c 0b64 6573 6372  PostIts.a..descr
-00007910: 6970 7469 6f6e 948c e043 7265 6174 6520  iption...Create 
-00007920: 6120 506f 7374 4974 2e20 2054 6865 2050  a PostIt.  The P
-00007930: 6f73 7449 7420 7769 6c6c 2067 7261 6e74  ostIt will grant
-00007940: 2061 6363 6573 7320 746f 2061 2066 696c   access to a fil
-00007950: 6520 7572 6c2e 0a54 6865 206e 6577 6c79  e url..The newly
-00007960: 2063 7265 6174 6564 2050 6f73 7449 7420   created PostIt 
-00007970: 6361 6e20 6265 2072 6564 6565 6d65 6420  can be redeemed 
-00007980: 6279 2061 6e79 6f6e 6520 7769 7468 6f75  by anyone withou
-00007990: 7420 0a66 7572 7468 6572 2061 7574 686f  t .further autho
-000079a0: 7269 7a61 7469 6f6e 2e20 2054 6869 7320  rization.  This 
-000079b0: 7769 6c6c 206e 6561 726c 7920 6964 656e  will nearly iden
-000079c0: 7469 6361 6c20 746f 2063 616c 6c69 6e67  tical to calling
-000079d0: 0a74 6865 2066 696c 6573 2073 6572 7669  .the files servi
-000079e0: 6365 2067 6574 436f 6e74 656e 7473 2065  ce getContents e
-000079f0: 6e64 706f 696e 742e 0a94 8c0b 6f70 6572  ndpoint.....oper
-00007a00: 6174 696f 6e49 6494 8c0c 6372 6561 7465  ationId...create
-00007a10: 506f 7374 4974 948c 0a70 6172 616d 6574  PostIt...paramet
-00007a20: 6572 7394 5d94 287d 9428 8c04 6e61 6d65  ers.].(}.(..name
-00007a30: 948c 0873 7973 7465 6d49 6494 8c0b 6465  ...systemId...de
-00007a40: 7363 7269 7074 696f 6e94 8c30 5468 6520  scription..0The 
-00007a50: 6e61 6d65 206f 6620 7468 6520 7379 7374  name of the syst
-00007a60: 656d 2074 6f20 6372 6561 7465 2074 6865  em to create the
-00007a70: 2050 6f73 7449 7420 666f 722e 948c 0269   PostIt for....i
-00007a80: 6e94 8c04 7061 7468 948c 0872 6571 7569  n...path...requi
-00007a90: 7265 6494 888c 0673 6368 656d 6194 7d94  red....schema.}.
-00007aa0: 8c04 2472 6566 948c 1d23 2f63 6f6d 706f  ..$ref...#/compo
-00007ab0: 6e65 6e74 732f 7363 6865 6d61 732f 4964  nents/schemas/Id
-00007ac0: 5374 7269 6e67 9473 757d 9428 8c04 6e61  String.su}.(..na
-00007ad0: 6d65 948c 0470 6174 6894 8c02 696e 948c  me...path...in..
-00007ae0: 0470 6174 6894 8c08 7265 7175 6972 6564  .path...required
-00007af0: 9488 8c0b 6465 7363 7269 7074 696f 6e94  ....description.
-00007b00: 8c25 5061 7468 2072 656c 6174 6976 6520  .%Path relative 
-00007b10: 746f 2074 6865 2073 7973 7465 6d20 2a72  to the system *r
-00007b20: 6f6f 7444 6972 2a94 8c07 6578 616d 706c  ootDir*...exampl
-00007b30: 6594 8c1f 2f44 6972 6563 746f 7279 412f  e.../DirectoryA/
-00007b40: 4469 7265 6374 6f72 7942 2f66 696c 652e  DirectoryB/file.
-00007b50: 7478 7494 8c06 7363 6865 6d61 947d 948c  txt...schema.}..
-00007b60: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-00007b70: 7565 8c0b 7265 7175 6573 7442 6f64 7994  ue..requestBody.
-00007b80: 7d94 288c 0872 6571 7569 7265 6494 888c  }.(..required...
-00007b90: 0b64 6573 6372 6970 7469 6f6e 948c 3441  .description..4A
-00007ba0: 204a 534f 4e20 646f 6375 6d65 6e74 2064   JSON document d
-00007bb0: 6573 6372 6962 696e 6720 7468 6520 506f  escribing the Po
-00007bc0: 7374 4974 2074 6f20 6265 2063 7265 6174  stIt to be creat
-00007bd0: 6564 2e94 8c07 636f 6e74 656e 7494 7d94  ed....content.}.
-00007be0: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
-00007bf0: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
-00007c00: 8c04 2472 6566 948c 2823 2f63 6f6d 706f  ..$ref..(#/compo
-00007c10: 6e65 6e74 732f 7363 6865 6d61 732f 4372  nents/schemas/Cr
-00007c20: 6561 7465 506f 7374 4974 5265 7175 6573  eatePostItReques
-00007c30: 7494 7373 7375 8c09 7265 7370 6f6e 7365  t.sssu..response
-00007c40: 7394 7d94 288c 0332 3030 947d 9428 8c0b  s.}.(..200.}.(..
-00007c50: 6465 7363 7269 7074 696f 6e94 8c08 5375  description...Su
-00007c60: 6363 6573 732e 948c 0763 6f6e 7465 6e74  ccess....content
-00007c70: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
-00007c80: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
-00007c90: 947d 948c 0424 7265 6694 8c23 232f 636f  .}...$ref..##/co
-00007ca0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-00007cb0: 2f50 6f73 7449 7452 6573 706f 6e73 6594  /PostItResponse.
-00007cc0: 7373 7375 8c03 3430 3094 7d94 288c 0b64  sssu..400.}.(..d
-00007cd0: 6573 6372 6970 7469 6f6e 948c 0b42 6164  escription...Bad
-00007ce0: 2052 6571 7565 7374 948c 0763 6f6e 7465   Request...conte
-00007cf0: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
-00007d00: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
-00007d10: 6d61 947d 948c 0424 7265 6694 8c27 232f  ma.}...$ref..'#/
-00007d20: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-00007d30: 6173 2f46 696c 6553 7472 696e 6752 6573  as/FileStringRes
-00007d40: 706f 6e73 6594 7373 7375 8c03 3430 3194  ponse.sssu..401.
-00007d50: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
-00007d60: 948c 114e 6f74 2041 7574 6865 6e74 6963  ...Not Authentic
-00007d70: 6174 6564 948c 0763 6f6e 7465 6e74 947d  ated...content.}
-00007d80: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
-00007d90: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
-00007da0: 948c 0424 7265 6694 8c27 232f 636f 6d70  ...$ref..'#/comp
-00007db0: 6f6e 656e 7473 2f73 6368 656d 6173 2f46  onents/schemas/F
-00007dc0: 696c 6553 7472 696e 6752 6573 706f 6e73  ileStringRespons
-00007dd0: 6594 7373 7375 8c03 3430 3394 7d94 288c  e.sssu..403.}.(.
-00007de0: 0b64 6573 6372 6970 7469 6f6e 948c 1150  .description...P
-00007df0: 6572 6d69 7373 696f 6e20 4465 6e69 6564  ermission Denied
-00007e00: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
-00007e10: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
-00007e20: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
-00007e30: 7265 6694 8c27 232f 636f 6d70 6f6e 656e  ref..'#/componen
-00007e40: 7473 2f73 6368 656d 6173 2f46 696c 6553  ts/schemas/FileS
-00007e50: 7472 696e 6752 6573 706f 6e73 6594 7373  tringResponse.ss
-00007e60: 7375 8c03 3430 3494 7d94 288c 0b64 6573  su..404.}.(..des
-00007e70: 6372 6970 7469 6f6e 948c 094e 6f74 2046  cription...Not F
-00007e80: 6f75 6e64 948c 0763 6f6e 7465 6e74 947d  ound...content.}
-00007e90: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
-00007ea0: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
-00007eb0: 948c 0424 7265 6694 8c27 232f 636f 6d70  ...$ref..'#/comp
-00007ec0: 6f6e 656e 7473 2f73 6368 656d 6173 2f46  onents/schemas/F
-00007ed0: 696c 6553 7472 696e 6752 6573 706f 6e73  ileStringRespons
-00007ee0: 6594 7373 7375 8c03 3530 3094 7d94 288c  e.sssu..500.}.(.
-00007ef0: 0b64 6573 6372 6970 7469 6f6e 948c 0e49  .description...I
-00007f00: 6e74 6572 6e61 6c20 4572 726f 7294 8c07  nternal Error...
-00007f10: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
-00007f20: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
-00007f30: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
-00007f40: 948c 2723 2f63 6f6d 706f 6e65 6e74 732f  ..'#/components/
-00007f50: 7363 6865 6d61 732f 4669 6c65 5374 7269  schemas/FileStri
-00007f60: 6e67 5265 7370 6f6e 7365 9473 7373 7575  ngResponse.sssuu
-00007f70: 7573 8c11 2f76 332f 6669 6c65 732f 706f  us../v3/files/po
-00007f80: 7374 6974 7394 7d94 8c03 6765 7494 7d94  stits.}...get.}.
-00007f90: 288c 0773 756d 6d61 7279 948c 0d4c 6973  (..summary...Lis
-00007fa0: 7420 506f 7374 4974 732e 948c 0474 6167  t PostIts....tag
-00007fb0: 7394 5d94 8c07 506f 7374 4974 7394 618c  s.]...PostIts.a.
-00007fc0: 0b64 6573 6372 6970 7469 6f6e 9458 7c01  .description.X|.
-00007fd0: 0000 5265 7472 6965 7665 2061 206c 6973  ..Retrieve a lis
-00007fe0: 7420 6f66 2061 6c6c 2050 6f73 7449 7473  t of all PostIts
-00007ff0: 2e20 2055 7365 202a 6c69 7374 5479 7065  .  Use *listType
-00008000: 2a20 616e 6420 2a73 656c 6563 742a 2071  * and *select* q
-00008010: 7565 7279 200a 7061 7261 6d65 7465 7273  uery .parameters
-00008020: 2074 6f20 6c69 6d69 7420 7265 7375 6c74   to limit result
-00008030: 732e 2051 7565 7279 2070 6172 616d 6574  s. Query paramet
-00008040: 6572 202a 6c69 7374 5479 7065 2a20 616c  er *listType* al
-00008050: 6c6f 7773 2066 6f72 2066 696c 7465 7269  lows for filteri
-00008060: 6e67 200a 7265 7375 6c74 7320 6261 7365  ng .results base
-00008070: 6420 6f6e 2061 7574 686f 7269 7a61 7469  d on authorizati
-00008080: 6f6e 2e20 4f70 7469 6f6e 7320 666f 7220  on. Options for 
-00008090: 2a6c 6973 7454 7970 652a 2061 7265 0a20  *listType* are. 
-000080a0: 202d 202a 4f57 4e45 442a 2049 6e63 6c75   - *OWNED* Inclu
-000080b0: 6465 206f 6e6c 7920 6974 656d 7320 6f77  de only items ow
-000080c0: 6e65 6420 6279 2072 6571 7565 7374 6572  ned by requester
-000080d0: 2028 4465 6661 756c 7429 0a20 202d 202a   (Default).  - *
-000080e0: 414c 4c2a 2049 6e63 6c75 6465 2061 6c6c  ALL* Include all
-000080f0: 2069 7465 6d73 2072 6571 7565 7374 6572   items requester
-00008100: 2069 7320 6175 7468 6f72 697a 6564 2074   is authorized t
-00008110: 6f20 7669 6577 2e20 2854 656e 616e 7420  o view. (Tenant 
-00008120: 6164 6d69 6e73 2063 616e 2076 6965 7720  admins can view 
-00008130: 616c 6c20 506f 7374 4974 7320 696e 2074  all PostIts in t
-00008140: 6865 6972 2074 656e 616e 7429 2e0a 948c  heir tenant)....
-00008150: 0b6f 7065 7261 7469 6f6e 4964 948c 0b6c  .operationId...l
-00008160: 6973 7450 6f73 7449 7473 948c 0a70 6172  istPostIts...par
-00008170: 616d 6574 6572 7394 5d94 287d 9428 8c04  ameters.].(}.(..
-00008180: 6e61 6d65 948c 086c 6973 7454 7970 6594  name...listType.
-00008190: 8c02 696e 948c 0571 7565 7279 948c 0673  ..in...query...s
-000081a0: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
-000081b0: 2123 2f63 6f6d 706f 6e65 6e74 732f 7363  !#/components/sc
-000081c0: 6865 6d61 732f 4c69 7374 5479 7065 456e  hemas/ListTypeEn
-000081d0: 756d 9473 757d 9428 8c04 6e61 6d65 948c  um.su}.(..name..
-000081e0: 056c 696d 6974 948c 0269 6e94 8c05 7175  .limit...in...qu
-000081f0: 6572 7994 8c0b 6465 7363 7269 7074 696f  ery...descriptio
-00008200: 6e94 8c5b 4c69 6d69 7420 6e75 6d62 6572  n..[Limit number
-00008210: 206f 6620 6974 656d 7320 7265 7475 726e   of items return
-00008220: 6564 2e20 466f 7220 6578 616d 706c 6520  ed. For example 
-00008230: 6c69 6d69 743d 3130 2e20 5573 6520 2d31  limit=10. Use -1
-00008240: 2066 6f72 2075 6e6c 696d 6974 6564 2e20   for unlimited. 
-00008250: 4465 6661 756c 7420 6973 2031 3030 2e94  Default is 100..
-00008260: 8c06 7363 6865 6d61 947d 9428 8c04 7479  ..schema.}.(..ty
-00008270: 7065 948c 0769 6e74 6567 6572 948c 0764  pe...integer...d
-00008280: 6566 6175 6c74 944b 6475 757d 9428 8c04  efault.Kduu}.(..
-00008290: 6e61 6d65 948c 076f 7264 6572 4279 948c  name...orderBy..
-000082a0: 0269 6e94 8c05 7175 6572 7994 8c0b 6465  .in...query...de
-000082b0: 7363 7269 7074 696f 6e94 8c6b 4174 7472  scription..kAttr
-000082c0: 6962 7574 6520 666f 7220 736f 7274 696e  ibute for sortin
-000082d0: 672e 2044 6972 6563 7469 6f6e 206d 6179  g. Direction may
-000082e0: 2062 6520 696e 636c 7564 6564 2e20 466f   be included. Fo
-000082f0: 7220 6578 616d 706c 6520 6f72 6465 7242  r example orderB
-00008300: 793d 6964 2864 6573 6329 2e20 4465 6661  y=id(desc). Defa
-00008310: 756c 7420 6469 7265 6374 696f 6e20 6973  ult direction is
-00008320: 2028 6173 6329 2e94 8c06 7363 6865 6d61   (asc)....schema
-00008330: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-00008340: 6e67 9473 757d 9428 8c04 6e61 6d65 948c  ng.su}.(..name..
-00008350: 0473 6b69 7094 8c02 696e 948c 0571 7565  .skip...in...que
-00008360: 7279 948c 0b64 6573 6372 6970 7469 6f6e  ry...description
-00008370: 948c 5a4e 756d 6265 7220 6f66 2069 7465  ..ZNumber of ite
-00008380: 6d73 2074 6f20 736b 6970 2e20 5573 6520  ms to skip. Use 
-00008390: 6f6e 6520 6f66 2073 6b69 7020 6f72 2073  one of skip or s
-000083a0: 7461 7274 4166 7465 722e 2046 6f72 2065  tartAfter. For e
-000083b0: 7861 6d70 6c65 2073 6b69 703d 3130 2e20  xample skip=10. 
-000083c0: 4465 6661 756c 7420 6973 2030 2e94 8c06  Default is 0....
-000083d0: 7363 6865 6d61 947d 948c 0474 7970 6594  schema.}...type.
-000083e0: 8c07 696e 7465 6765 7294 7375 7d94 288c  ..integer.su}.(.
-000083f0: 046e 616d 6594 8c0a 7374 6172 7441 6674  .name...startAft
-00008400: 6572 948c 0269 6e94 8c05 7175 6572 7994  er...in...query.
-00008410: 8c0b 6465 7363 7269 7074 696f 6e94 8c98  ..description...
-00008420: 5768 6572 6520 746f 2073 7461 7274 2077  Where to start w
-00008430: 6865 6e20 736f 7274 696e 672e 2055 7365  hen sorting. Use
-00008440: 206f 6e65 206f 6620 736b 6970 206f 7220   one of skip or 
-00008450: 7374 6172 7441 6674 6572 2e20 4d75 7374  startAfter. Must
-00008460: 2061 6c73 6f20 7370 6563 6966 7920 6f72   also specify or
-00008470: 6465 7242 792e 2046 6f72 2065 7861 6d70  derBy. For examp
-00008480: 6c65 2c20 6c69 6d69 743d 3130 266f 7264  le, limit=10&ord
-00008490: 6572 4279 3d69 6428 6173 6329 2673 7461  erBy=id(asc)&sta
-000084a0: 7274 4166 7465 723d 266c 743b 706f 7374  rtAfter=&lt;post
-000084b0: 6974 6964 2667 743b 948c 0673 6368 656d  itid&gt;...schem
-000084c0: 6194 7d94 8c04 7479 7065 948c 0673 7472  a.}...type...str
-000084d0: 696e 6794 7375 7d94 288c 046e 616d 6594  ing.su}.(..name.
-000084e0: 8c06 7365 6c65 6374 948c 0269 6e94 8c05  ..select...in...
-000084f0: 7175 6572 7994 8c0b 6465 7363 7269 7074  query...descript
-00008500: 696f 6e94 8c9f 4c69 7374 206f 6620 6174  ion...List of at
-00008510: 7472 6962 7574 6573 2074 6f20 6265 2069  tributes to be i
-00008520: 6e63 6c75 6465 6420 6173 2070 6172 7420  ncluded as part 
-00008530: 6f66 2065 6163 6820 7265 7375 6c74 2069  of each result i
-00008540: 7465 6d2e 204b 6579 776f 7264 7320 2a61  tem. Keywords *a
-00008550: 6c6c 4174 7472 6962 7574 6573 2a20 616e  llAttributes* an
-00008560: 6420 2a73 756d 6d61 7279 4174 7472 6962  d *summaryAttrib
-00008570: 7574 6573 2a20 6172 6520 7375 7070 6f72  utes* are suppor
-00008580: 7465 642e 2046 6f72 2065 7861 6d70 6c65  ted. For example
-00008590: 2073 656c 6563 743d 6964 2c6f 776e 6572   select=id,owner
-000085a0: 2c70 6174 6894 8c06 7363 6865 6d61 947d  ,path...schema.}
-000085b0: 9428 8c04 7479 7065 948c 0673 7472 696e  .(..type...strin
-000085c0: 6794 8c07 6465 6661 756c 7494 8c11 7375  g...default...su
-000085d0: 6d6d 6172 7941 7474 7269 6275 7465 7394  mmaryAttributes.
-000085e0: 7575 658c 0972 6573 706f 6e73 6573 947d  uue..responses.}
-000085f0: 9428 8c03 3230 3094 7d94 288c 0b64 6573  .(..200.}.(..des
-00008600: 6372 6970 7469 6f6e 948c 0853 7563 6365  cription...Succe
-00008610: 7373 2e94 8c07 636f 6e74 656e 7494 7d94  ss....content.}.
-00008620: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
-00008630: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
-00008640: 8c04 2472 6566 948c 2723 2f63 6f6d 706f  ..$ref..'#/compo
-00008650: 6e65 6e74 732f 7363 6865 6d61 732f 506f  nents/schemas/Po
-00008660: 7374 4974 4c69 7374 5265 7370 6f6e 7365  stItListResponse
-00008670: 9473 7373 758c 0334 3030 947d 9428 8c0b  .sssu..400.}.(..
-00008680: 6465 7363 7269 7074 696f 6e94 8c0b 4261  description...Ba
-00008690: 6420 5265 7175 6573 7494 8c07 636f 6e74  d Request...cont
-000086a0: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
-000086b0: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
-000086c0: 656d 6194 7d94 8c04 2472 6566 948c 2723  ema.}...$ref..'#
-000086d0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-000086e0: 6d61 732f 4669 6c65 5374 7269 6e67 5265  mas/FileStringRe
-000086f0: 7370 6f6e 7365 9473 7373 758c 0334 3031  sponse.sssu..401
-00008700: 947d 9428 8c0b 6465 7363 7269 7074 696f  .}.(..descriptio
-00008710: 6e94 8c11 4e6f 7420 4175 7468 656e 7469  n...Not Authenti
-00008720: 6361 7465 6494 8c07 636f 6e74 656e 7494  cated...content.
-00008730: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
-00008740: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
-00008750: 7d94 8c04 2472 6566 948c 2723 2f63 6f6d  }...$ref..'#/com
-00008760: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-00008770: 4669 6c65 5374 7269 6e67 5265 7370 6f6e  FileStringRespon
-00008780: 7365 9473 7373 758c 0334 3033 947d 9428  se.sssu..403.}.(
-00008790: 8c0b 6465 7363 7269 7074 696f 6e94 8c11  ..description...
-000087a0: 5065 726d 6973 7369 6f6e 2044 656e 6965  Permission Denie
-000087b0: 6494 8c07 636f 6e74 656e 7494 7d94 8c10  d...content.}...
-000087c0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-000087d0: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
-000087e0: 2472 6566 948c 2723 2f63 6f6d 706f 6e65  $ref..'#/compone
-000087f0: 6e74 732f 7363 6865 6d61 732f 4669 6c65  nts/schemas/File
-00008800: 5374 7269 6e67 5265 7370 6f6e 7365 9473  StringResponse.s
-00008810: 7373 758c 0334 3034 947d 9428 8c0b 6465  ssu..404.}.(..de
-00008820: 7363 7269 7074 696f 6e94 8c09 4e6f 7420  scription...Not 
-00008830: 466f 756e 6494 8c07 636f 6e74 656e 7494  Found...content.
-00008840: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
-00008850: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
-00008860: 7d94 8c04 2472 6566 948c 2723 2f63 6f6d  }...$ref..'#/com
-00008870: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-00008880: 4669 6c65 5374 7269 6e67 5265 7370 6f6e  FileStringRespon
-00008890: 7365 9473 7373 758c 0335 3030 947d 9428  se.sssu..500.}.(
-000088a0: 8c0b 6465 7363 7269 7074 696f 6e94 8c0e  ..description...
-000088b0: 496e 7465 726e 616c 2045 7272 6f72 948c  Internal Error..
-000088c0: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
-000088d0: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
-000088e0: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
-000088f0: 6694 8c27 232f 636f 6d70 6f6e 656e 7473  f..'#/components
-00008900: 2f73 6368 656d 6173 2f46 696c 6553 7472  /schemas/FileStr
-00008910: 696e 6752 6573 706f 6e73 6594 7373 7375  ingResponse.sssu
-00008920: 7575 738c 1c2f 7633 2f66 696c 6573 2f70  uus../v3/files/p
-00008930: 6f73 7469 7473 2f7b 706f 7374 6974 4964  ostits/{postitId
-00008940: 7d94 7d94 288c 0367 6574 947d 9428 8c07  }.}.(..get.}.(..
-00008950: 7375 6d6d 6172 7994 8c0b 4765 7420 506f  summary...Get Po
-00008960: 7374 4974 2e94 8c04 7461 6773 945d 948c  stIt....tags.]..
-00008970: 0750 6f73 7449 7473 9461 8c0b 6465 7363  .PostIts.a..desc
-00008980: 7269 7074 696f 6e94 8c36 4765 7420 6120  ription..6Get a 
-00008990: 7369 6e67 6c65 2050 6f73 7449 742e 2020  single PostIt.  
-000089a0: 5468 6973 2064 6f65 7320 6e6f 7420 7265  This does not re
-000089b0: 6465 656d 2074 6865 2050 6f73 7449 742e  deem the PostIt.
-000089c0: 948c 0b6f 7065 7261 7469 6f6e 4964 948c  ...operationId..
-000089d0: 0967 6574 506f 7374 4974 948c 0a70 6172  .getPostIt...par
-000089e0: 616d 6574 6572 7394 5d94 7d94 288c 046e  ameters.].}.(..n
-000089f0: 616d 6594 8c08 706f 7374 6974 4964 948c  ame...postitId..
-00008a00: 0269 6e94 8c04 7061 7468 948c 0872 6571  .in...path...req
-00008a10: 7569 7265 6494 888c 0673 6368 656d 6194  uired....schema.
-00008a20: 7d94 288c 0474 7970 6594 8c06 7374 7269  }.(..type...stri
-00008a30: 6e67 948c 0666 6f72 6d61 7494 8c04 7575  ng...format...uu
-00008a40: 6964 9475 7561 8c09 7265 7370 6f6e 7365  id.uua..response
-00008a50: 7394 7d94 288c 0332 3030 947d 9428 8c0b  s.}.(..200.}.(..
-00008a60: 6465 7363 7269 7074 696f 6e94 8c08 5375  description...Su
-00008a70: 6363 6573 732e 948c 0763 6f6e 7465 6e74  ccess....content
-00008a80: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
-00008a90: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
-00008aa0: 947d 948c 0424 7265 6694 8c23 232f 636f  .}...$ref..##/co
-00008ab0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-00008ac0: 2f50 6f73 7449 7452 6573 706f 6e73 6594  /PostItResponse.
-00008ad0: 7373 7375 8c03 3430 3094 7d94 288c 0b64  sssu..400.}.(..d
-00008ae0: 6573 6372 6970 7469 6f6e 948c 0b42 6164  escription...Bad
-00008af0: 2052 6571 7565 7374 948c 0763 6f6e 7465   Request...conte
-00008b00: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
-00008b10: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
-00008b20: 6d61 947d 948c 0424 7265 6694 8c27 232f  ma.}...$ref..'#/
-00008b30: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-00008b40: 6173 2f46 696c 6553 7472 696e 6752 6573  as/FileStringRes
-00008b50: 706f 6e73 6594 7373 7375 8c03 3430 3194  ponse.sssu..401.
-00008b60: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
-00008b70: 948c 114e 6f74 2041 7574 6865 6e74 6963  ...Not Authentic
-00008b80: 6174 6564 948c 0763 6f6e 7465 6e74 947d  ated...content.}
-00008b90: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
-00008ba0: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
-00008bb0: 948c 0424 7265 6694 8c27 232f 636f 6d70  ...$ref..'#/comp
-00008bc0: 6f6e 656e 7473 2f73 6368 656d 6173 2f46  onents/schemas/F
-00008bd0: 696c 6553 7472 696e 6752 6573 706f 6e73  ileStringRespons
-00008be0: 6594 7373 7375 8c03 3430 3394 7d94 288c  e.sssu..403.}.(.
-00008bf0: 0b64 6573 6372 6970 7469 6f6e 948c 1150  .description...P
-00008c00: 6572 6d69 7373 696f 6e20 4465 6e69 6564  ermission Denied
-00008c10: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
-00008c20: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
-00008c30: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
-00008c40: 7265 6694 8c27 232f 636f 6d70 6f6e 656e  ref..'#/componen
-00008c50: 7473 2f73 6368 656d 6173 2f46 696c 6553  ts/schemas/FileS
-00008c60: 7472 696e 6752 6573 706f 6e73 6594 7373  tringResponse.ss
-00008c70: 7375 8c03 3430 3494 7d94 288c 0b64 6573  su..404.}.(..des
-00008c80: 6372 6970 7469 6f6e 948c 094e 6f74 2046  cription...Not F
-00008c90: 6f75 6e64 948c 0763 6f6e 7465 6e74 947d  ound...content.}
-00008ca0: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
-00008cb0: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
-00008cc0: 948c 0424 7265 6694 8c27 232f 636f 6d70  ...$ref..'#/comp
-00008cd0: 6f6e 656e 7473 2f73 6368 656d 6173 2f46  onents/schemas/F
-00008ce0: 696c 6553 7472 696e 6752 6573 706f 6e73  ileStringRespons
-00008cf0: 6594 7373 7375 8c03 3530 3094 7d94 288c  e.sssu..500.}.(.
-00008d00: 0b64 6573 6372 6970 7469 6f6e 948c 0e49  .description...I
-00008d10: 6e74 6572 6e61 6c20 4572 726f 7294 8c07  nternal Error...
-00008d20: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
-00008d30: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
-00008d40: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
-00008d50: 948c 2723 2f63 6f6d 706f 6e65 6e74 732f  ..'#/components/
-00008d60: 7363 6865 6d61 732f 4669 6c65 5374 7269  schemas/FileStri
-00008d70: 6e67 5265 7370 6f6e 7365 9473 7373 7575  ngResponse.sssuu
-00008d80: 758c 0570 6174 6368 947d 9428 8c07 7375  u..patch.}.(..su
-00008d90: 6d6d 6172 7994 8c0f 4d6f 6469 6679 2061  mmary...Modify a
-00008da0: 2050 6f73 7449 7494 8c04 7461 6773 945d   PostIt...tags.]
-00008db0: 948c 0750 6f73 7449 7473 9461 8c0b 6465  ...PostIts.a..de
-00008dc0: 7363 7269 7074 696f 6e94 8c25 5570 6461  scription..%Upda
-00008dd0: 7465 2073 656c 6563 7465 6420 6669 656c  te selected fiel
-00008de0: 6473 206f 6620 6120 506f 7374 4974 2e20  ds of a PostIt. 
-00008df0: 0a94 8c0b 6f70 6572 6174 696f 6e49 6494  ....operationId.
-00008e00: 8c0c 7570 6461 7465 506f 7374 4974 948c  ..updatePostIt..
-00008e10: 0a70 6172 616d 6574 6572 7394 5d94 7d94  .parameters.].}.
-00008e20: 288c 046e 616d 6594 8c08 706f 7374 6974  (..name...postit
-00008e30: 4964 948c 0269 6e94 8c04 7061 7468 948c  Id...in...path..
-00008e40: 0872 6571 7569 7265 6494 888c 0673 6368  .required....sch
-00008e50: 656d 6194 7d94 288c 0474 7970 6594 8c06  ema.}.(..type...
-00008e60: 7374 7269 6e67 948c 0666 6f72 6d61 7494  string...format.
-00008e70: 8c04 7575 6964 9475 7561 8c0b 7265 7175  ..uuid.uua..requ
-00008e80: 6573 7442 6f64 7994 7d94 288c 0872 6571  estBody.}.(..req
-00008e90: 7569 7265 6494 888c 0b64 6573 6372 6970  uired....descrip
-00008ea0: 7469 6f6e 948c 3441 204a 534f 4e20 646f  tion..4A JSON do
-00008eb0: 6375 6d65 6e74 2064 6573 6372 6962 696e  cument describin
-00008ec0: 6720 7468 6520 506f 7374 4974 2074 6f20  g the PostIt to 
-00008ed0: 6265 2075 7064 6174 6564 2e94 8c07 636f  be updated....co
-00008ee0: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
-00008ef0: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
-00008f00: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
-00008f10: 2823 2f63 6f6d 706f 6e65 6e74 732f 7363  (#/components/sc
-00008f20: 6865 6d61 732f 5570 6461 7465 506f 7374  hemas/UpdatePost
-00008f30: 4974 5265 7175 6573 7494 7373 7375 8c09  ItRequest.sssu..
-00008f40: 7265 7370 6f6e 7365 7394 7d94 288c 0332  responses.}.(..2
-00008f50: 3030 947d 9428 8c0b 6465 7363 7269 7074  00.}.(..descript
-00008f60: 696f 6e94 8c08 5375 6363 6573 732e 948c  ion...Success...
-00008f70: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
-00008f80: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
-00008f90: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
-00008fa0: 6694 8c23 232f 636f 6d70 6f6e 656e 7473  f..##/components
-00008fb0: 2f73 6368 656d 6173 2f50 6f73 7449 7452  /schemas/PostItR
-00008fc0: 6573 706f 6e73 6594 7373 7375 8c03 3430  esponse.sssu..40
-00008fd0: 3094 7d94 288c 0b64 6573 6372 6970 7469  0.}.(..descripti
-00008fe0: 6f6e 948c 0b42 6164 2052 6571 7565 7374  on...Bad Request
-00008ff0: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
-00009000: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
-00009010: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
-00009020: 7265 6694 8c27 232f 636f 6d70 6f6e 656e  ref..'#/componen
-00009030: 7473 2f73 6368 656d 6173 2f46 696c 6553  ts/schemas/FileS
-00009040: 7472 696e 6752 6573 706f 6e73 6594 7373  tringResponse.ss
-00009050: 7375 8c03 3430 3194 7d94 288c 0b64 6573  su..401.}.(..des
-00009060: 6372 6970 7469 6f6e 948c 114e 6f74 2041  cription...Not A
-00009070: 7574 6865 6e74 6963 6174 6564 948c 0763  uthenticated...c
-00009080: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
-00009090: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
-000090a0: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
-000090b0: 8c27 232f 636f 6d70 6f6e 656e 7473 2f73  .'#/components/s
-000090c0: 6368 656d 6173 2f46 696c 6553 7472 696e  chemas/FileStrin
-000090d0: 6752 6573 706f 6e73 6594 7373 7375 8c03  gResponse.sssu..
-000090e0: 3430 3394 7d94 288c 0b64 6573 6372 6970  403.}.(..descrip
-000090f0: 7469 6f6e 948c 1150 6572 6d69 7373 696f  tion...Permissio
-00009100: 6e20 4465 6e69 6564 948c 0763 6f6e 7465  n Denied...conte
-00009110: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
-00009120: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
-00009130: 6d61 947d 948c 0424 7265 6694 8c27 232f  ma.}...$ref..'#/
-00009140: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-00009150: 6173 2f46 696c 6553 7472 696e 6752 6573  as/FileStringRes
-00009160: 706f 6e73 6594 7373 7375 8c03 3430 3494  ponse.sssu..404.
-00009170: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
-00009180: 948c 094e 6f74 2046 6f75 6e64 948c 0763  ...Not Found...c
-00009190: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
-000091a0: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
-000091b0: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
-000091c0: 8c27 232f 636f 6d70 6f6e 656e 7473 2f73  .'#/components/s
-000091d0: 6368 656d 6173 2f46 696c 6553 7472 696e  chemas/FileStrin
-000091e0: 6752 6573 706f 6e73 6594 7373 7375 8c03  gResponse.sssu..
-000091f0: 3530 3094 7d94 288c 0b64 6573 6372 6970  500.}.(..descrip
-00009200: 7469 6f6e 948c 0e49 6e74 6572 6e61 6c20  tion...Internal 
-00009210: 4572 726f 7294 8c07 636f 6e74 656e 7494  Error...content.
-00009220: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
-00009230: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
-00009240: 7d94 8c04 2472 6566 948c 2723 2f63 6f6d  }...$ref..'#/com
-00009250: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-00009260: 4669 6c65 5374 7269 6e67 5265 7370 6f6e  FileStringRespon
-00009270: 7365 9473 7373 7575 758c 0664 656c 6574  se.sssuuu..delet
-00009280: 6594 7d94 288c 0773 756d 6d61 7279 948c  e.}.(..summary..
-00009290: 0f44 656c 6574 6520 6120 506f 7374 4974  .Delete a PostIt
-000092a0: 948c 0474 6167 7394 5d94 8c07 506f 7374  ...tags.]...Post
-000092b0: 4974 7394 618c 0b64 6573 6372 6970 7469  Its.a..descripti
-000092c0: 6f6e 948c 1044 656c 6574 6520 6120 506f  on...Delete a Po
-000092d0: 7374 4974 2e94 8c0b 6f70 6572 6174 696f  stIt....operatio
-000092e0: 6e49 6494 8c0c 6465 6c65 7465 506f 7374  nId...deletePost
-000092f0: 4974 948c 0a70 6172 616d 6574 6572 7394  It...parameters.
-00009300: 5d94 7d94 288c 046e 616d 6594 8c08 706f  ].}.(..name...po
-00009310: 7374 6974 4964 948c 0269 6e94 8c04 7061  stitId...in...pa
-00009320: 7468 948c 0872 6571 7569 7265 6494 888c  th...required...
-00009330: 0673 6368 656d 6194 7d94 288c 0474 7970  .schema.}.(..typ
-00009340: 6594 8c06 7374 7269 6e67 948c 0666 6f72  e...string...for
-00009350: 6d61 7494 8c04 7575 6964 9475 7561 8c09  mat...uuid.uua..
-00009360: 7265 7370 6f6e 7365 7394 7d94 288c 0332  responses.}.(..2
-00009370: 3030 947d 9428 8c0b 6465 7363 7269 7074  00.}.(..descript
-00009380: 696f 6e94 8c08 5375 6363 6573 732e 948c  ion...Success...
-00009390: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
-000093a0: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
-000093b0: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
-000093c0: 6694 8c24 232f 636f 6d70 6f6e 656e 7473  f..$#/components
-000093d0: 2f73 6368 656d 6173 2f52 6573 7043 6861  /schemas/RespCha
-000093e0: 6e67 6543 6f75 6e74 9473 7373 758c 0334  ngeCount.sssu..4
-000093f0: 3030 947d 9428 8c0b 6465 7363 7269 7074  00.}.(..descript
-00009400: 696f 6e94 8c0b 4261 6420 5265 7175 6573  ion...Bad Reques
-00009410: 7494 8c07 636f 6e74 656e 7494 7d94 8c10  t...content.}...
-00009420: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-00009430: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
-00009440: 2472 6566 948c 2723 2f63 6f6d 706f 6e65  $ref..'#/compone
-00009450: 6e74 732f 7363 6865 6d61 732f 4669 6c65  nts/schemas/File
-00009460: 5374 7269 6e67 5265 7370 6f6e 7365 9473  StringResponse.s
-00009470: 7373 758c 0334 3031 947d 9428 8c0b 6465  ssu..401.}.(..de
-00009480: 7363 7269 7074 696f 6e94 8c11 4e6f 7420  scription...Not 
-00009490: 4175 7468 656e 7469 6361 7465 6494 8c07  Authenticated...
-000094a0: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
-000094b0: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
-000094c0: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
-000094d0: 948c 2723 2f63 6f6d 706f 6e65 6e74 732f  ..'#/components/
-000094e0: 7363 6865 6d61 732f 4669 6c65 5374 7269  schemas/FileStri
-000094f0: 6e67 5265 7370 6f6e 7365 9473 7373 758c  ngResponse.sssu.
-00009500: 0334 3033 947d 9428 8c0b 6465 7363 7269  .403.}.(..descri
-00009510: 7074 696f 6e94 8c11 5065 726d 6973 7369  ption...Permissi
-00009520: 6f6e 2044 656e 6965 6494 8c07 636f 6e74  on Denied...cont
-00009530: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
-00009540: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
-00009550: 656d 6194 7d94 8c04 2472 6566 948c 2723  ema.}...$ref..'#
-00009560: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-00009570: 6d61 732f 4669 6c65 5374 7269 6e67 5265  mas/FileStringRe
-00009580: 7370 6f6e 7365 9473 7373 758c 0334 3034  sponse.sssu..404
-00009590: 947d 9428 8c0b 6465 7363 7269 7074 696f  .}.(..descriptio
-000095a0: 6e94 8c09 4e6f 7420 466f 756e 6494 8c07  n...Not Found...
-000095b0: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
-000095c0: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
-000095d0: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
-000095e0: 948c 2723 2f63 6f6d 706f 6e65 6e74 732f  ..'#/components/
-000095f0: 7363 6865 6d61 732f 4669 6c65 5374 7269  schemas/FileStri
-00009600: 6e67 5265 7370 6f6e 7365 9473 7373 758c  ngResponse.sssu.
-00009610: 0335 3030 947d 9428 8c0b 6465 7363 7269  .500.}.(..descri
-00009620: 7074 696f 6e94 8c0e 496e 7465 726e 616c  ption...Internal
-00009630: 2045 7272 6f72 948c 0763 6f6e 7465 6e74   Error...content
-00009640: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
-00009650: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
-00009660: 947d 948c 0424 7265 6694 8c27 232f 636f  .}...$ref..'#/co
-00009670: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-00009680: 2f46 696c 6553 7472 696e 6752 6573 706f  /FileStringRespo
-00009690: 6e73 6594 7373 7375 7575 758c 232f 7633  nse.sssuuuu.#/v3
-000096a0: 2f66 696c 6573 2f70 6f73 7469 7473 2f72  /files/postits/r
-000096b0: 6564 6565 6d2f 7b70 6f73 7469 7449 647d  edeem/{postitId}
-000096c0: 947d 948c 0367 6574 947d 9428 8c07 7375  .}...get.}.(..su
-000096d0: 6d6d 6172 7994 8c0e 5265 6465 656d 2050  mmary...Redeem P
-000096e0: 6f73 7449 742e 948c 0474 6167 7394 5d94  ostIt....tags.].
-000096f0: 8c07 506f 7374 4974 7394 618c 0b64 6573  ..PostIts.a..des
-00009700: 6372 6970 7469 6f6e 9458 be01 0000 5265  cription.X....Re
-00009710: 6465 656d 2061 2050 6f73 7449 742e 2020  deem a PostIt.  
-00009720: 5468 6973 2077 696c 6c20 7265 7475 726e  This will return
-00009730: 2074 6865 2066 696c 6520 7468 6174 2069   the file that i
-00009740: 7320 706f 696e 7465 6420 746f 2062 7920  s pointed to by 
-00009750: 7468 6520 506f 7374 4974 2e20 204e 6f20  the PostIt.  No 
-00009760: 6175 7468 656e 7469 6361 7469 6f6e 2069  authentication i
-00009770: 7320 7265 7175 6972 6564 2e20 4966 2074  s required. If t
-00009780: 6865 202a 7a69 702a 2071 7565 7279 2070  he *zip* query p
-00009790: 6172 616d 2069 7320 7072 6f76 6964 6564  aram is provided
-000097a0: 2069 7420 636f 6e74 726f 6c73 2069 6620   it controls if 
-000097b0: 7468 6520 636f 6e74 656e 7420 6973 207a  the content is z
-000097c0: 6970 7065 6420 6f72 206e 6f74 2e20 2049  ipped or not.  I
-000097d0: 6620 7a69 7020 6973 206e 6f74 2070 726f  f zip is not pro
-000097e0: 7669 6465 642c 2069 7420 6465 6661 756c  vided, it defaul
-000097f0: 7473 2074 6f20 6661 6c73 6520 756e 6c65  ts to false unle
-00009800: 7373 2074 6865 2070 6174 6820 706f 696e  ss the path poin
-00009810: 7465 6420 746f 2062 7920 7468 6520 506f  ted to by the Po
-00009820: 7374 4974 2069 7320 6120 6469 7265 6374  stIt is a direct
-00009830: 6f72 792e 2020 496e 2074 6865 2063 6173  ory.  In the cas
-00009840: 6520 6f66 2061 2064 6972 6563 746f 7279  e of a directory
-00009850: 2c20 7468 6520 6465 6661 756c 7420 6973  , the default is
-00009860: 207a 6970 3d74 7275 652e 2044 6972 6563   zip=true. Direc
-00009870: 746f 7269 6573 206d 7573 7420 6279 2072  tories must by r
-00009880: 6564 6565 6d65 6420 696e 207a 6970 7065  edeemed in zippe
-00009890: 6420 666f 726d 6174 2c20 736f 2065 6974  d format, so eit
-000098a0: 6865 7220 6163 6365 7074 2074 6865 2064  her accept the d
-000098b0: 6566 6175 6c74 2c20 6f72 2073 7065 6369  efault, or speci
-000098c0: 6679 207a 6970 3d74 7275 652e 948c 0b6f  fy zip=true....o
-000098d0: 7065 7261 7469 6f6e 4964 948c 0c72 6564  perationId...red
-000098e0: 6565 6d50 6f73 7449 7494 8c0a 7061 7261  eemPostIt...para
-000098f0: 6d65 7465 7273 945d 9428 7d94 288c 046e  meters.].(}.(..n
-00009900: 616d 6594 8c08 706f 7374 6974 4964 948c  ame...postitId..
-00009910: 0269 6e94 8c04 7061 7468 948c 0872 6571  .in...path...req
-00009920: 7569 7265 6494 888c 0673 6368 656d 6194  uired....schema.
-00009930: 7d94 288c 0474 7970 6594 8c06 7374 7269  }.(..type...stri
-00009940: 6e67 948c 0666 6f72 6d61 7494 8c04 7575  ng...format...uu
-00009950: 6964 9475 757d 9428 8c04 6e61 6d65 948c  id.uu}.(..name..
-00009960: 037a 6970 948c 0269 6e94 8c05 7175 6572  .zip...in...quer
-00009970: 7994 8c0b 6465 7363 7269 7074 696f 6e94  y...description.
-00009980: 8cb6 496e 6469 6361 7465 7320 6120 7a69  ..Indicates a zi
-00009990: 7020 6f75 7470 7574 2073 7472 6561 6d20  p output stream 
-000099a0: 7368 6f75 6c64 2062 6520 7072 6f76 6964  should be provid
-000099b0: 6564 2e20 2049 6620 7a69 7020 6973 206e  ed.  If zip is n
-000099c0: 6f74 2070 726f 7669 6465 6420 6974 2064  ot provided it d
-000099d0: 6566 6175 6c74 7320 746f 2066 616c 7365  efaults to false
-000099e0: 2075 6e6c 6573 7320 7468 6520 7061 7468   unless the path
-000099f0: 2069 7320 6120 6469 7265 6374 6f72 792e   is a directory.
-00009a00: 2020 496e 2074 6865 2063 6173 6520 6f66    In the case of
-00009a10: 2061 2064 6972 6563 746f 7279 2074 6865   a directory the
-00009a20: 2063 6f6e 7465 6e74 2077 696c 6c20 6265   content will be
-00009a30: 207a 6970 7065 642e 948c 0673 6368 656d   zipped....schem
-00009a40: 6194 7d94 8c04 7479 7065 948c 0762 6f6f  a.}...type...boo
-00009a50: 6c65 616e 9473 8c07 6578 616d 706c 6594  lean.s..example.
-00009a60: 8975 658c 0972 6573 706f 6e73 6573 947d  .ue..responses.}
-00009a70: 9428 8c03 3230 3094 7d94 8c0b 6465 7363  .(..200.}...desc
-00009a80: 7269 7074 696f 6e94 8c08 5375 6363 6573  ription...Succes
-00009a90: 732e 9473 8c03 3430 3094 7d94 288c 0b64  s..s..400.}.(..d
-00009aa0: 6573 6372 6970 7469 6f6e 948c 0b42 6164  escription...Bad
-00009ab0: 2052 6571 7565 7374 948c 0763 6f6e 7465   Request...conte
-00009ac0: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
-00009ad0: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
-00009ae0: 6d61 947d 948c 0424 7265 6694 8c27 232f  ma.}...$ref..'#/
-00009af0: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-00009b00: 6173 2f46 696c 6553 7472 696e 6752 6573  as/FileStringRes
-00009b10: 706f 6e73 6594 7373 7375 8c03 3430 3394  ponse.sssu..403.
-00009b20: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
-00009b30: 948c 1150 6572 6d69 7373 696f 6e20 4465  ...Permission De
-00009b40: 6e69 6564 948c 0763 6f6e 7465 6e74 947d  nied...content.}
-00009b50: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
-00009b60: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
-00009b70: 948c 0424 7265 6694 8c27 232f 636f 6d70  ...$ref..'#/comp
-00009b80: 6f6e 656e 7473 2f73 6368 656d 6173 2f46  onents/schemas/F
-00009b90: 696c 6553 7472 696e 6752 6573 706f 6e73  ileStringRespons
-00009ba0: 6594 7373 7375 8c03 3430 3494 7d94 288c  e.sssu..404.}.(.
-00009bb0: 0b64 6573 6372 6970 7469 6f6e 948c 094e  .description...N
-00009bc0: 6f74 2046 6f75 6e64 948c 0763 6f6e 7465  ot Found...conte
-00009bd0: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
-00009be0: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
-00009bf0: 6d61 947d 948c 0424 7265 6694 8c27 232f  ma.}...$ref..'#/
-00009c00: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-00009c10: 6173 2f46 696c 6553 7472 696e 6752 6573  as/FileStringRes
-00009c20: 706f 6e73 6594 7373 7375 8c03 3530 3094  ponse.sssu..500.
-00009c30: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
-00009c40: 948c 0e49 6e74 6572 6e61 6c20 4572 726f  ...Internal Erro
-00009c50: 7294 8c07 636f 6e74 656e 7494 7d94 8c10  r...content.}...
-00009c60: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-00009c70: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
-00009c80: 2472 6566 948c 2723 2f63 6f6d 706f 6e65  $ref..'#/compone
-00009c90: 6e74 732f 7363 6865 6d61 732f 4669 6c65  nts/schemas/File
-00009ca0: 5374 7269 6e67 5265 7370 6f6e 7365 9473  StringResponse.s
-00009cb0: 7373 7575 7573 758c 0a63 6f6d 706f 6e65  ssuuusu..compone
-00009cc0: 6e74 7394 7d94 8c07 7363 6865 6d61 7394  nts.}...schemas.
-00009cd0: 7d94 288c 0f48 6561 6465 7242 7974 6552  }.(..HeaderByteR
-00009ce0: 616e 6765 947d 9428 8c04 7479 7065 948c  ange.}.(..type..
-00009cf0: 066f 626a 6563 7494 8c0a 7072 6f70 6572  .object...proper
-00009d00: 7469 6573 947d 9428 8c03 6d69 6e94 7d94  ties.}.(..min.}.
-00009d10: 288c 0474 7970 6594 8c07 696e 7465 6765  (..type...intege
-00009d20: 7294 8c06 666f 726d 6174 948c 0569 6e74  r...format...int
-00009d30: 3634 9475 8c03 6d61 7894 7d94 288c 0474  64.u..max.}.(..t
-00009d40: 7970 6594 8c07 696e 7465 6765 7294 8c06  ype...integer...
-00009d50: 666f 726d 6174 948c 0569 6e74 3634 9475  format...int64.u
-00009d60: 7575 8c08 4669 6c65 496e 666f 947d 9428  uu..FileInfo.}.(
-00009d70: 8c04 7479 7065 948c 066f 626a 6563 7494  ..type...object.
-00009d80: 8c0a 7072 6f70 6572 7469 6573 947d 9428  ..properties.}.(
-00009d90: 8c08 6d69 6d65 5479 7065 947d 948c 0474  ..mimeType.}...t
-00009da0: 7970 6594 8c06 7374 7269 6e67 9473 8c04  ype...string.s..
-00009db0: 7479 7065 947d 948c 0474 7970 6594 8c06  type.}...type...
-00009dc0: 7374 7269 6e67 9473 8c05 6f77 6e65 7294  string.s..owner.
-00009dd0: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
-00009de0: 6794 738c 0567 726f 7570 947d 948c 0474  g.s..group.}...t
-00009df0: 7970 6594 8c06 7374 7269 6e67 9473 8c11  ype...string.s..
-00009e00: 6e61 7469 7665 5065 726d 6973 7369 6f6e  nativePermission
-00009e10: 7394 7d94 8c04 7479 7065 948c 0673 7472  s.}...type...str
-00009e20: 696e 6794 738c 0375 726c 947d 948c 0474  ing.s..url.}...t
-00009e30: 7970 6594 8c06 7374 7269 6e67 9473 8c0c  ype...string.s..
-00009e40: 6c61 7374 4d6f 6469 6669 6564 947d 9428  lastModified.}.(
-00009e50: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-00009e60: 8c06 666f 726d 6174 948c 0964 6174 652d  ..format...date-
-00009e70: 7469 6d65 9475 8c04 6e61 6d65 947d 948c  time.u..name.}..
-00009e80: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-00009e90: 8c04 7061 7468 947d 948c 0474 7970 6594  ..path.}...type.
-00009ea0: 8c06 7374 7269 6e67 9473 8c04 7369 7a65  ..string.s..size
-00009eb0: 947d 9428 8c04 7479 7065 948c 0769 6e74  .}.(..type...int
-00009ec0: 6567 6572 948c 0b64 6573 6372 6970 7469  eger...descripti
-00009ed0: 6f6e 948c 0a73 697a 6520 696e 206b 4294  on...size in kB.
-00009ee0: 8c06 666f 726d 6174 948c 0569 6e74 3634  ..format...int64
-00009ef0: 9475 7575 8c0c 4669 6c65 5374 6174 496e  .uuu..FileStatIn
-00009f00: 666f 947d 9428 8c04 7479 7065 948c 066f  fo.}.(..type...o
-00009f10: 626a 6563 7494 8c0a 7072 6f70 6572 7469  bject...properti
-00009f20: 6573 947d 9428 8c0c 6162 736f 6c75 7465  es.}.(..absolute
-00009f30: 5061 7468 947d 948c 0474 7970 6594 8c06  Path.}...type...
-00009f40: 7374 7269 6e67 9473 8c03 7569 6494 7d94  string.s..uid.}.
-00009f50: 288c 0474 7970 6594 8c07 696e 7465 6765  (..type...intege
-00009f60: 7294 8c06 666f 726d 6174 948c 0569 6e74  r...format...int
-00009f70: 3332 9475 8c03 6769 6494 7d94 288c 0474  32.u..gid.}.(..t
-00009f80: 7970 6594 8c07 696e 7465 6765 7294 8c06  ype...integer...
-00009f90: 666f 726d 6174 948c 0569 6e74 3332 9475  format...int32.u
-00009fa0: 8c04 7369 7a65 947d 9428 8c04 7479 7065  ..size.}.(..type
-00009fb0: 948c 0769 6e74 6567 6572 948c 0666 6f72  ...integer...for
-00009fc0: 6d61 7494 8c05 696e 7436 3494 758c 0570  mat...int64.u..p
-00009fd0: 6572 6d73 947d 948c 0474 7970 6594 8c06  erms.}...type...
-00009fe0: 7374 7269 6e67 9473 8c0a 6163 6365 7373  string.s..access
-00009ff0: 5469 6d65 947d 9428 8c04 7479 7065 948c  Time.}.(..type..
-0000a000: 0769 6e74 6567 6572 948c 0666 6f72 6d61  .integer...forma
-0000a010: 7494 8c05 696e 7436 3494 758c 0a6d 6f64  t...int64.u..mod
-0000a020: 6966 7954 696d 6594 7d94 288c 0474 7970  ifyTime.}.(..typ
-0000a030: 6594 8c07 696e 7465 6765 7294 8c06 666f  e...integer...fo
-0000a040: 726d 6174 948c 0569 6e74 3634 9475 8c03  rmat...int64.u..
-0000a050: 6469 7294 7d94 8c04 7479 7065 948c 0762  dir.}...type...b
-0000a060: 6f6f 6c65 616e 9473 8c04 6c69 6e6b 947d  oolean.s..link.}
-0000a070: 948c 0474 7970 6594 8c07 626f 6f6c 6561  ...type...boolea
-0000a080: 6e94 7375 758c 0c41 636c 456e 7472 7949  n.suu..AclEntryI
-0000a090: 6e66 6f94 7d94 288c 0474 7970 6594 8c06  nfo.}.(..type...
-0000a0a0: 6f62 6a65 6374 948c 0a70 726f 7065 7274  object...propert
-0000a0b0: 6965 7394 7d94 288c 0a64 6566 6175 6c74  ies.}.(..default
-0000a0c0: 4163 6c94 7d94 8c04 7479 7065 948c 0762  Acl.}...type...b
-0000a0d0: 6f6f 6c65 616e 9473 8c04 7479 7065 947d  oolean.s..type.}
-0000a0e0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-0000a0f0: 9473 8c09 7072 696e 6369 7061 6c94 7d94  .s..principal.}.
-0000a100: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-0000a110: 738c 0b70 6572 6d69 7373 696f 6e73 947d  s..permissions.}
-0000a120: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-0000a130: 9473 7575 8c13 4669 6c65 4c69 7374 696e  .suu..FileListin
-0000a140: 6752 6573 706f 6e73 6594 7d94 288c 0474  gResponse.}.(..t
-0000a150: 7970 6594 8c06 6f62 6a65 6374 948c 0a70  ype...object...p
-0000a160: 726f 7065 7274 6965 7394 7d94 288c 0673  roperties.}.(..s
-0000a170: 7461 7475 7394 7d94 8c04 7479 7065 948c  tatus.}...type..
-0000a180: 0673 7472 696e 6794 738c 076d 6573 7361  .string.s..messa
-0000a190: 6765 947d 948c 0474 7970 6594 8c06 7374  ge.}...type...st
-0000a1a0: 7269 6e67 9473 8c06 7265 7375 6c74 947d  ring.s..result.}
-0000a1b0: 9428 8c04 7479 7065 948c 0561 7272 6179  .(..type...array
-0000a1c0: 948c 0569 7465 6d73 947d 948c 0424 7265  ...items.}...$re
-0000a1d0: 6694 8c1d 232f 636f 6d70 6f6e 656e 7473  f...#/components
-0000a1e0: 2f73 6368 656d 6173 2f46 696c 6549 6e66  /schemas/FileInf
-0000a1f0: 6f94 7375 8c07 7665 7273 696f 6e94 7d94  o.su..version.}.
-0000a200: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-0000a210: 738c 086d 6574 6164 6174 6194 7d94 8c04  s..metadata.}...
-0000a220: 7479 7065 948c 066f 626a 6563 7494 7375  type...object.su
-0000a230: 758c 0e46 696c 6550 6572 6d69 7373 696f  u..FilePermissio
-0000a240: 6e94 7d94 288c 0474 7970 6594 8c06 6f62  n.}.(..type...ob
-0000a250: 6a65 6374 948c 0a70 726f 7065 7274 6965  ject...propertie
-0000a260: 7394 7d94 288c 0874 656e 616e 7449 6494  s.}.(..tenantId.
-0000a270: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
-0000a280: 6794 738c 0875 7365 726e 616d 6594 7d94  g.s..username.}.
-0000a290: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-0000a2a0: 738c 0873 7973 7465 6d49 6494 7d94 8c04  s..systemId.}...
-0000a2b0: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-0000a2c0: 0470 6174 6894 7d94 8c04 7479 7065 948c  .path.}...type..
-0000a2d0: 0673 7472 696e 6794 738c 0a70 6572 6d69  .string.s..permi
-0000a2e0: 7373 696f 6e94 7d94 8c04 2472 6566 948c  ssion.}...$ref..
-0000a2f0: 1d23 2f63 6f6d 706f 6e65 6e74 732f 7363  .#/components/sc
-0000a300: 6865 6d61 732f 5065 726d 456e 756d 9473  hemas/PermEnum.s
-0000a310: 7575 8c10 5368 6172 6564 4669 6c65 4f62  uu..SharedFileOb
-0000a320: 6a65 6374 947d 9428 8c04 7479 7065 948c  ject.}.(..type..
-0000a330: 066f 626a 6563 7494 8c0a 7072 6f70 6572  .object...proper
-0000a340: 7469 6573 947d 9428 8c07 6372 6561 746f  ties.}.(..creato
-0000a350: 7294 7d94 288c 0474 7970 6594 8c06 7374  r.}.(..type...st
-0000a360: 7269 6e67 948c 0b64 6573 6372 6970 7469  ring...descripti
-0000a370: 6f6e 948c 2655 7365 726e 616d 6520 7768  on..&Username wh
-0000a380: 6f20 7368 6172 6564 2074 6865 2066 696c  o shared the fil
-0000a390: 652f 6469 7265 6374 6f72 7994 758c 0a73  e/directory.u..s
-0000a3a0: 6861 7265 6457 6974 6894 7d94 288c 0474  haredWith.}.(..t
-0000a3b0: 7970 6594 8c06 7374 7269 6e67 948c 0b64  ype...string...d
-0000a3c0: 6573 6372 6970 7469 6f6e 948c 1f55 7365  escription...Use
-0000a3d0: 726e 616d 6520 7768 6f20 7761 7320 6772  rname who was gr
-0000a3e0: 616e 7465 6420 6163 6365 7373 9475 8c07  anted access.u..
-0000a3f0: 6372 6561 7465 6494 7d94 288c 0474 7970  created.}.(..typ
-0000a400: 6594 8c06 7374 7269 6e67 948c 0b64 6573  e...string...des
-0000a410: 6372 6970 7469 6f6e 948c 1943 7265 6174  cription...Creat
-0000a420: 696f 6e20 7469 6d65 7374 616d 7020 696e  ion timestamp in
-0000a430: 2055 5443 9475 8c09 6578 7069 7265 7349   UTC.u..expiresI
-0000a440: 6e94 7d94 288c 0474 7970 6594 8c07 696e  n.}.(..type...in
-0000a450: 7465 6765 7294 8c0b 6465 7363 7269 7074  teger...descript
-0000a460: 696f 6e94 8c37 4e75 6d62 6572 206f 6620  ion..7Number of 
-0000a470: 7365 636f 6e64 7320 696e 2077 6869 6368  seconds in which
-0000a480: 2074 6865 2073 6861 7265 2077 6173 2073   the share was s
-0000a490: 6574 2074 6f20 6578 7069 7265 2e94 8c06  et to expire....
-0000a4a0: 666f 726d 6174 948c 0569 6e74 3332 9475  format...int32.u
-0000a4b0: 8c03 7572 6c94 7d94 288c 0474 7970 6594  ..url.}.(..type.
-0000a4c0: 8c06 7374 7269 6e67 948c 0b64 6573 6372  ..string...descr
-0000a4d0: 6970 7469 6f6e 948c 184c 696e 6b20 746f  iption...Link to
-0000a4e0: 2074 6865 2073 6861 7265 6420 6669 6c65   the shared file
-0000a4f0: 2e94 7575 758c 1053 6861 7265 4669 6c65  ..uuu..ShareFile
-0000a500: 5265 7175 6573 7494 7d94 288c 0872 6571  Request.}.(..req
-0000a510: 7569 7265 6494 5d94 288c 0965 7870 6972  uired.].(..expir
-0000a520: 6573 496e 948c 0875 7365 726e 616d 6594  esIn...username.
-0000a530: 658c 0474 7970 6594 8c06 6f62 6a65 6374  e..type...object
-0000a540: 948c 0a70 726f 7065 7274 6965 7394 7d94  ...properties.}.
-0000a550: 288c 0875 7365 726e 616d 6594 7d94 288c  (..username.}.(.
-0000a560: 0474 7970 6594 8c06 7374 7269 6e67 948c  .type...string..
-0000a570: 0b64 6573 6372 6970 7469 6f6e 948c 1c54  .description...T
-0000a580: 6865 2075 7365 7220 7769 7468 2077 6869  he user with whi
-0000a590: 6368 2074 6f20 7368 6172 6594 758c 0965  ch to share.u..e
-0000a5a0: 7870 6972 6573 496e 947d 9428 8c07 6d61  xpiresIn.}.(..ma
-0000a5b0: 7869 6d75 6d94 4a80 3a09 008c 076d 696e  ximum.J.:....min
-0000a5c0: 696d 756d 944b 018c 0474 7970 6594 8c07  imum.K...type...
-0000a5d0: 696e 7465 6765 7294 8c0b 6465 7363 7269  integer...descri
-0000a5e0: 7074 696f 6e94 8c41 5469 6d65 2069 6e20  ption..ATime in 
-0000a5f0: 7365 636f 6e64 7320 6f66 2065 7870 6972  seconds of expir
-0000a600: 6174 696f 6e2e 206d 696e 696d 756d 3d31  ation. minimum=1
-0000a610: 2c20 6d61 7869 6d75 6d3d 3630 3438 3030  , maximum=604800
-0000a620: 2028 3120 7765 656b 2994 8c06 666f 726d   (1 week)...form
-0000a630: 6174 948c 0569 6e74 3332 9475 7575 8c0c  at...int32.uuu..
-0000a640: 5472 616e 7366 6572 5461 736b 947d 9428  TransferTask.}.(
-0000a650: 8c04 7479 7065 948c 066f 626a 6563 7494  ..type...object.
-0000a660: 8c0a 7072 6f70 6572 7469 6573 947d 9428  ..properties.}.(
-0000a670: 8c02 6964 947d 9428 8c04 7479 7065 948c  ..id.}.(..type..
-0000a680: 0769 6e74 6567 6572 948c 0666 6f72 6d61  .integer...forma
-0000a690: 7494 8c05 696e 7433 3294 758c 0875 7365  t...int32.u..use
-0000a6a0: 726e 616d 6594 7d94 8c04 7479 7065 948c  rname.}...type..
-0000a6b0: 0673 7472 696e 6794 738c 0874 656e 616e  .string.s..tenan
-0000a6c0: 7449 6494 7d94 8c04 7479 7065 948c 0673  tId.}...type...s
-0000a6d0: 7472 696e 6794 738c 0374 6167 947d 948c  tring.s..tag.}..
-0000a6e0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-0000a6f0: 8c04 7575 6964 947d 9428 8c04 7479 7065  ..uuid.}.(..type
-0000a700: 948c 0673 7472 696e 6794 8c06 666f 726d  ...string...form
-0000a710: 6174 948c 0475 7569 6494 758c 0673 7461  at...uuid.u..sta
-0000a720: 7475 7394 7d94 8c04 2472 6566 948c 2723  tus.}...$ref..'#
-0000a730: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-0000a740: 6d61 732f 5472 616e 7366 6572 5374 6174  mas/TransferStat
-0000a750: 7573 456e 756d 9473 8c0b 7061 7265 6e74  usEnum.s..parent
-0000a760: 5461 736b 7394 7d94 288c 0474 7970 6594  Tasks.}.(..type.
-0000a770: 8c05 6172 7261 7994 8c05 6974 656d 7394  ..array...items.
-0000a780: 7d94 8c04 2472 6566 948c 2723 2f63 6f6d  }...$ref..'#/com
-0000a790: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-0000a7a0: 5472 616e 7366 6572 5461 736b 5061 7265  TransferTaskPare
-0000a7b0: 6e74 9473 758c 1365 7374 696d 6174 6564  nt.su..estimated
-0000a7c0: 546f 7461 6c42 7974 6573 947d 9428 8c04  TotalBytes.}.(..
-0000a7d0: 7479 7065 948c 0769 6e74 6567 6572 948c  type...integer..
-0000a7e0: 0666 6f72 6d61 7494 8c05 696e 7436 3494  .format...int64.
-0000a7f0: 758c 1574 6f74 616c 4279 7465 7354 7261  u..totalBytesTra
-0000a800: 6e73 6665 7272 6564 947d 9428 8c04 7479  nsferred.}.(..ty
-0000a810: 7065 948c 0769 6e74 6567 6572 948c 0666  pe...integer...f
-0000a820: 6f72 6d61 7494 8c05 696e 7436 3494 758c  ormat...int64.u.
-0000a830: 0e74 6f74 616c 5472 616e 7366 6572 7394  .totalTransfers.
-0000a840: 7d94 288c 0474 7970 6594 8c07 696e 7465  }.(..type...inte
-0000a850: 6765 7294 8c06 666f 726d 6174 948c 0569  ger...format...i
-0000a860: 6e74 3332 9475 8c11 636f 6d70 6c65 7465  nt32.u..complete
-0000a870: 5472 616e 7366 6572 7394 7d94 288c 0474  Transfers.}.(..t
-0000a880: 7970 6594 8c07 696e 7465 6765 7294 8c06  ype...integer...
-0000a890: 666f 726d 6174 948c 0569 6e74 3332 9475  format...int32.u
-0000a8a0: 8c0c 6572 726f 724d 6573 7361 6765 947d  ..errorMessage.}
-0000a8b0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-0000a8c0: 9473 8c07 6372 6561 7465 6494 7d94 288c  .s..created.}.(.
-0000a8d0: 0474 7970 6594 8c06 7374 7269 6e67 948c  .type...string..
-0000a8e0: 0666 6f72 6d61 7494 8c09 6461 7465 2d74  .format...date-t
-0000a8f0: 696d 6594 758c 0973 7461 7274 5469 6d65  ime.u..startTime
-0000a900: 947d 9428 8c04 7479 7065 948c 0673 7472  .}.(..type...str
-0000a910: 696e 6794 8c06 666f 726d 6174 948c 0964  ing...format...d
-0000a920: 6174 652d 7469 6d65 9475 8c07 656e 6454  ate-time.u..endT
-0000a930: 696d 6594 7d94 288c 0474 7970 6594 8c06  ime.}.(..type...
-0000a940: 7374 7269 6e67 948c 0666 6f72 6d61 7494  string...format.
-0000a950: 8c09 6461 7465 2d74 696d 6594 7575 758c  ..date-time.uuu.
-0000a960: 1254 7261 6e73 6665 7254 6173 6b50 6172  .TransferTaskPar
-0000a970: 656e 7494 7d94 288c 0474 7970 6594 8c06  ent.}.(..type...
-0000a980: 6f62 6a65 6374 948c 0a70 726f 7065 7274  object...propert
-0000a990: 6965 7394 7d94 288c 0269 6494 7d94 288c  ies.}.(..id.}.(.
-0000a9a0: 0474 7970 6594 8c07 696e 7465 6765 7294  .type...integer.
-0000a9b0: 8c06 666f 726d 6174 948c 0569 6e74 3332  ..format...int32
-0000a9c0: 9475 8c08 7465 6e61 6e74 4964 947d 948c  .u..tenantId.}..
-0000a9d0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-0000a9e0: 8c08 7573 6572 6e61 6d65 947d 948c 0474  ..username.}...t
-0000a9f0: 7970 6594 8c06 7374 7269 6e67 9473 8c09  ype...string.s..
-0000aa00: 736f 7572 6365 5552 4994 7d94 8c04 7479  sourceURI.}...ty
-0000aa10: 7065 948c 0673 7472 696e 6794 738c 0e64  pe...string.s..d
-0000aa20: 6573 7469 6e61 7469 6f6e 5552 4994 7d94  estinationURI.}.
-0000aa30: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-0000aa40: 738c 0a74 6f74 616c 4279 7465 7394 7d94  s..totalBytes.}.
-0000aa50: 288c 0474 7970 6594 8c07 696e 7465 6765  (..type...intege
-0000aa60: 7294 8c06 666f 726d 6174 948c 0569 6e74  r...format...int
-0000aa70: 3634 9475 8c10 6279 7465 7354 7261 6e73  64.u..bytesTrans
-0000aa80: 6665 7272 6564 947d 9428 8c04 7479 7065  ferred.}.(..type
-0000aa90: 948c 0769 6e74 6567 6572 948c 0666 6f72  ...integer...for
-0000aaa0: 6d61 7494 8c05 696e 7436 3494 758c 0674  mat...int64.u..t
-0000aab0: 6173 6b49 6494 7d94 288c 0474 7970 6594  askId.}.(..type.
-0000aac0: 8c07 696e 7465 6765 7294 8c06 666f 726d  ..integer...form
-0000aad0: 6174 948c 0569 6e74 3332 9475 8c08 6368  at...int32.u..ch
-0000aae0: 696c 6472 656e 947d 9428 8c04 7479 7065  ildren.}.(..type
-0000aaf0: 948c 0561 7272 6179 948c 0569 7465 6d73  ...array...items
-0000ab00: 947d 948c 0424 7265 6694 8c26 232f 636f  .}...$ref..&#/co
-0000ab10: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-0000ab20: 2f54 7261 6e73 6665 7254 6173 6b43 6869  /TransferTaskChi
-0000ab30: 6c64 9473 758c 0c65 7272 6f72 4d65 7373  ld.su..errorMess
-0000ab40: 6167 6594 7d94 8c04 7479 7065 948c 0673  age.}...type...s
-0000ab50: 7472 696e 6794 738c 0475 7569 6494 7d94  tring.s..uuid.}.
-0000ab60: 288c 0474 7970 6594 8c06 7374 7269 6e67  (..type...string
-0000ab70: 948c 0b64 6573 6372 6970 7469 6f6e 948c  ...description..
-0000ab80: 1655 6e69 7175 6520 4944 206f 6620 7468  .Unique ID of th
-0000ab90: 6520 7461 736b 2e94 8c06 666f 726d 6174  e task....format
-0000aba0: 948c 0475 7569 6494 758c 0673 7461 7475  ...uuid.u..statu
-0000abb0: 7394 7d94 8c04 2472 6566 948c 2723 2f63  s.}...$ref..'#/c
-0000abc0: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
-0000abd0: 732f 5472 616e 7366 6572 5374 6174 7573  s/TransferStatus
-0000abe0: 456e 756d 9473 8c07 6372 6561 7465 6494  Enum.s..created.
-0000abf0: 7d94 288c 0474 7970 6594 8c06 7374 7269  }.(..type...stri
-0000ac00: 6e67 948c 0666 6f72 6d61 7494 8c09 6461  ng...format...da
-0000ac10: 7465 2d74 696d 6594 758c 0973 7461 7274  te-time.u..start
-0000ac20: 5469 6d65 947d 9428 8c04 7479 7065 948c  Time.}.(..type..
-0000ac30: 0673 7472 696e 6794 8c06 666f 726d 6174  .string...format
-0000ac40: 948c 0964 6174 652d 7469 6d65 9475 8c07  ...date-time.u..
-0000ac50: 656e 6454 696d 6594 7d94 288c 0474 7970  endTime.}.(..typ
-0000ac60: 6594 8c06 7374 7269 6e67 948c 0666 6f72  e...string...for
-0000ac70: 6d61 7494 8c09 6461 7465 2d74 696d 6594  mat...date-time.
-0000ac80: 7575 758c 1154 7261 6e73 6665 7254 6173  uuu..TransferTas
-0000ac90: 6b43 6869 6c64 947d 9428 8c04 7479 7065  kChild.}.(..type
-0000aca0: 948c 066f 626a 6563 7494 8c0a 7072 6f70  ...object...prop
-0000acb0: 6572 7469 6573 947d 9428 8c02 6964 947d  erties.}.(..id.}
-0000acc0: 9428 8c04 7479 7065 948c 0769 6e74 6567  .(..type...integ
-0000acd0: 6572 948c 0666 6f72 6d61 7494 8c05 696e  er...format...in
-0000ace0: 7433 3294 758c 0874 656e 616e 7449 6494  t32.u..tenantId.
-0000acf0: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
-0000ad00: 6794 738c 0875 7365 726e 616d 6594 7d94  g.s..username.}.
-0000ad10: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-0000ad20: 738c 0973 6f75 7263 6555 5249 947d 948c  s..sourceURI.}..
-0000ad30: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-0000ad40: 8c0e 6465 7374 696e 6174 696f 6e55 5249  ..destinationURI
-0000ad50: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-0000ad60: 6e67 9473 8c0a 746f 7461 6c42 7974 6573  ng.s..totalBytes
-0000ad70: 947d 9428 8c04 7479 7065 948c 0769 6e74  .}.(..type...int
-0000ad80: 6567 6572 948c 0666 6f72 6d61 7494 8c05  eger...format...
-0000ad90: 696e 7436 3494 758c 1062 7974 6573 5472  int64.u..bytesTr
-0000ada0: 616e 7366 6572 7265 6494 7d94 288c 0474  ansferred.}.(..t
-0000adb0: 7970 6594 8c07 696e 7465 6765 7294 8c06  ype...integer...
-0000adc0: 666f 726d 6174 948c 0569 6e74 3634 9475  format...int64.u
-0000add0: 8c06 7461 736b 4964 947d 9428 8c04 7479  ..taskId.}.(..ty
-0000ade0: 7065 948c 0769 6e74 6567 6572 948c 0666  pe...integer...f
-0000adf0: 6f72 6d61 7494 8c05 696e 7433 3294 758c  ormat...int32.u.
-0000ae00: 0c65 7272 6f72 4d65 7373 6167 6594 7d94  .errorMessage.}.
-0000ae10: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-0000ae20: 738c 0c70 6172 656e 7454 6173 6b49 6494  s..parentTaskId.
-0000ae30: 7d94 288c 0474 7970 6594 8c07 696e 7465  }.(..type...inte
-0000ae40: 6765 7294 8c06 666f 726d 6174 948c 0569  ger...format...i
-0000ae50: 6e74 3332 9475 8c07 7265 7472 6965 7394  nt32.u..retries.
-0000ae60: 7d94 288c 0474 7970 6594 8c07 696e 7465  }.(..type...inte
-0000ae70: 6765 7294 8c06 666f 726d 6174 948c 0569  ger...format...i
-0000ae80: 6e74 3332 9475 8c03 6469 7294 7d94 8c04  nt32.u..dir.}...
-0000ae90: 7479 7065 948c 0762 6f6f 6c65 616e 9473  type...boolean.s
-0000aea0: 8c04 7575 6964 947d 9428 8c04 7479 7065  ..uuid.}.(..type
-0000aeb0: 948c 0673 7472 696e 6794 8c0b 6465 7363  ...string...desc
-0000aec0: 7269 7074 696f 6e94 8c16 556e 6971 7565  ription...Unique
-0000aed0: 2049 4420 6f66 2074 6865 2074 6173 6b2e   ID of the task.
-0000aee0: 948c 0666 6f72 6d61 7494 8c04 7575 6964  ...format...uuid
-0000aef0: 9475 8c06 7374 6174 7573 947d 948c 0424  .u..status.}...$
-0000af00: 7265 6694 8c27 232f 636f 6d70 6f6e 656e  ref..'#/componen
-0000af10: 7473 2f73 6368 656d 6173 2f54 7261 6e73  ts/schemas/Trans
-0000af20: 6665 7253 7461 7475 7345 6e75 6d94 738c  ferStatusEnum.s.
-0000af30: 0763 7265 6174 6564 947d 9428 8c04 7479  .created.}.(..ty
-0000af40: 7065 948c 0673 7472 696e 6794 8c06 666f  pe...string...fo
-0000af50: 726d 6174 948c 0964 6174 652d 7469 6d65  rmat...date-time
-0000af60: 9475 8c09 7374 6172 7454 696d 6594 7d94  .u..startTime.}.
-0000af70: 288c 0474 7970 6594 8c06 7374 7269 6e67  (..type...string
-0000af80: 948c 0666 6f72 6d61 7494 8c09 6461 7465  ...format...date
-0000af90: 2d74 696d 6594 758c 0765 6e64 5469 6d65  -time.u..endTime
-0000afa0: 947d 9428 8c04 7479 7065 948c 0673 7472  .}.(..type...str
-0000afb0: 696e 6794 8c06 666f 726d 6174 948c 0964  ing...format...d
-0000afc0: 6174 652d 7469 6d65 9475 7575 8c06 506f  ate-time.uuu..Po
-0000afd0: 7374 4974 947d 9428 8c04 7479 7065 948c  stIt.}.(..type..
-0000afe0: 066f 626a 6563 7494 8c0a 7072 6f70 6572  .object...proper
-0000aff0: 7469 6573 947d 9428 8c08 706f 7374 6974  ties.}.(..postit
-0000b000: 4964 947d 9428 8c04 7479 7065 948c 0673  Id.}.(..type...s
-0000b010: 7472 696e 6794 8c06 666f 726d 6174 948c  tring...format..
-0000b020: 0475 7569 6494 8c0b 6465 7363 7269 7074  .uuid...descript
-0000b030: 696f 6e94 8c1c 5468 6520 756e 6971 7565  ion...The unique
-0000b040: 2049 4420 6f66 2074 6865 2050 6f73 7449   ID of the PostI
-0000b050: 742e 9475 8c08 7379 7374 656d 4964 947d  t..u..systemId.}
-0000b060: 9428 8c04 7479 7065 948c 0673 7472 696e  .(..type...strin
-0000b070: 6794 8c0b 6465 7363 7269 7074 696f 6e94  g...description.
-0000b080: 8c45 5468 6520 4944 206f 6620 7468 6520  .EThe ID of the 
-0000b090: 7379 7374 656d 2077 6865 7265 2074 6865  system where the
-0000b0a0: 2066 696c 6520 706f 696e 7465 6420 746f   file pointed to
-0000b0b0: 2062 7920 7468 6520 506f 7374 4974 2072   by the PostIt r
-0000b0c0: 6573 6964 6573 2e94 758c 056f 776e 6572  esides..u..owner
-0000b0d0: 947d 9428 8c04 7479 7065 948c 0673 7472  .}.(..type...str
-0000b0e0: 696e 6794 8c0b 6465 7363 7269 7074 696f  ing...descriptio
-0000b0f0: 6e94 8c18 5468 6520 6f77 6e65 7220 6f66  n...The owner of
-0000b100: 2074 6865 2050 6f73 7449 742e 9475 8c08   the PostIt..u..
-0000b110: 7465 6e61 6e74 4964 947d 9428 8c04 7479  tenantId.}.(..ty
-0000b120: 7065 948c 0673 7472 696e 6794 8c0b 6465  pe...string...de
-0000b130: 7363 7269 7074 696f 6e94 8c27 7468 6520  scription..'the 
-0000b140: 7465 6e61 6e74 2074 6861 7420 7474 6865  tenant that tthe
-0000b150: 2050 6f73 7449 7420 6265 6c6f 6e67 7320   PostIt belongs 
-0000b160: 746f 2e94 758c 0470 6174 6894 7d94 288c  to..u..path.}.(.
-0000b170: 0474 7970 6594 8c06 7374 7269 6e67 948c  .type...string..
-0000b180: 0b64 6573 6372 6970 7469 6f6e 948c 2550  .description..%P
-0000b190: 6174 6820 7265 6c61 7469 7665 2074 6f20  ath relative to 
-0000b1a0: 7468 6520 7379 7374 656d 202a 726f 6f74  the system *root
-0000b1b0: 4469 722a 9475 8c0b 616c 6c6f 7765 6455  Dir*.u..allowedU
-0000b1c0: 7365 7394 7d94 288c 0474 7970 6594 8c07  ses.}.(..type...
-0000b1d0: 696e 7465 6765 7294 8c06 666f 726d 6174  integer...format
-0000b1e0: 948c 0569 6e74 3332 948c 0b64 6573 6372  ...int32...descr
-0000b1f0: 6970 7469 6f6e 948c 6a54 6865 206e 756d  iption..jThe num
-0000b200: 6265 7220 6f66 2074 696d 6573 2074 6865  ber of times the
-0000b210: 2050 6f73 7449 7420 6d61 7920 6265 2072   PostIt may be r
-0000b220: 6564 6565 6d65 642e 2020 5468 6973 206e  edeemed.  This n
-0000b230: 756d 6265 7220 6d69 6e75 7320 2a75 7365  umber minus *use
-0000b240: 732a 2069 7320 7468 6520 6e75 6d62 6572  s* is the number
-0000b250: 206f 6620 7573 6573 2072 656d 6169 6e69   of uses remaini
-0000b260: 6e67 2e94 758c 0974 696d 6573 5573 6564  ng..u..timesUsed
-0000b270: 947d 9428 8c04 7479 7065 948c 0769 6e74  .}.(..type...int
-0000b280: 6567 6572 948c 0666 6f72 6d61 7494 8c05  eger...format...
-0000b290: 696e 7433 3294 8c0b 6465 7363 7269 7074  int32...descript
-0000b2a0: 696f 6e94 8c3a 5468 6520 6e75 6d62 6572  ion..:The number
-0000b2b0: 206f 6620 7469 6d65 7320 7468 6520 506f   of times the Po
-0000b2c0: 7374 4974 2068 6173 2061 6c72 6561 6479  stIt has already
-0000b2d0: 2062 6565 6e20 7265 7472 6965 7665 642e   been retrieved.
-0000b2e0: 9475 8c07 6a77 7455 7365 7294 7d94 288c  .u..jwtUser.}.(.
-0000b2f0: 0474 7970 6594 8c06 7374 7269 6e67 948c  .type...string..
-0000b300: 0b64 6573 6372 6970 7469 6f6e 948c 4141  .description..AA
-0000b310: 7574 6865 6e74 6963 6174 6564 2075 7365  uthenticated use
-0000b320: 7220 6672 6f6d 2074 6865 204a 5754 2028  r from the JWT (
-0000b330: 6d61 7920 6265 2064 6966 6665 7265 6e74  may be different
-0000b340: 2074 6861 6e20 4f42 4f20 7573 6572 292e   than OBO user).
-0000b350: 9475 8c0b 6a77 7454 656e 616e 7449 6494  .u..jwtTenantId.
-0000b360: 7d94 288c 0474 7970 6594 8c06 7374 7269  }.(..type...stri
-0000b370: 6e67 948c 0b64 6573 6372 6970 7469 6f6e  ng...description
-0000b380: 948c 5454 656e 616e 7420 6f66 2061 7574  ..TTenant of aut
-0000b390: 6865 6e74 6963 6174 6564 2075 7365 7220  henticated user 
-0000b3a0: 6672 6f6d 2074 6865 204a 5754 2028 6d61  from the JWT (ma
-0000b3b0: 7920 6265 2064 6966 6665 7265 6e74 2074  y be different t
-0000b3c0: 6861 6e20 4f42 4f20 7573 6572 2773 2074  han OBO user's t
-0000b3d0: 656e 616e 7429 2e94 758c 0972 6564 6565  enant)..u..redee
-0000b3e0: 6d55 726c 947d 9428 8c04 7479 7065 948c  mUrl.}.(..type..
-0000b3f0: 0673 7472 696e 6794 8c0b 6465 7363 7269  .string...descri
-0000b400: 7074 696f 6e94 8c3d 5468 6520 7572 6c20  ption..=The url 
-0000b410: 746f 2075 7365 2074 6f20 7265 7472 6965  to use to retrie
-0000b420: 7665 2074 6865 2066 696c 6520 706f 696e  ve the file poin
-0000b430: 7465 6420 746f 2062 7920 7468 6520 506f  ted to by the Po
-0000b440: 7374 4974 2e94 758c 0a65 7870 6972 6174  stIt..u..expirat
-0000b450: 696f 6e94 7d94 288c 0474 7970 6594 8c06  ion.}.(..type...
-0000b460: 7374 7269 6e67 948c 0666 6f72 6d61 7494  string...format.
-0000b470: 8c09 6461 7465 2d74 696d 6594 8c0b 6465  ..date-time...de
-0000b480: 7363 7269 7074 696f 6e94 8c27 5468 6520  scription..'The 
-0000b490: 6578 7069 7261 7469 6f6e 2064 6174 652f  expiration date/
-0000b4a0: 7469 6d65 206f 6620 7468 6520 506f 7374  time of the Post
-0000b4b0: 4974 2e94 758c 0763 7265 6174 6564 947d  It..u..created.}
-0000b4c0: 9428 8c04 7479 7065 948c 0673 7472 696e  .(..type...strin
-0000b4d0: 6794 8c06 666f 726d 6174 948c 0964 6174  g...format...dat
-0000b4e0: 652d 7469 6d65 948c 0b64 6573 6372 6970  e-time...descrip
-0000b4f0: 7469 6f6e 948c 1943 7265 6174 696f 6e20  tion...Creation 
-0000b500: 7469 6d65 7374 616d 7020 696e 2055 5443  timestamp in UTC
-0000b510: 9475 8c07 7570 6461 7465 6494 7d94 288c  .u..updated.}.(.
-0000b520: 0474 7970 6594 8c06 7374 7269 6e67 948c  .type...string..
-0000b530: 0666 6f72 6d61 7494 8c09 6461 7465 2d74  .format...date-t
-0000b540: 696d 6594 8c0b 6465 7363 7269 7074 696f  ime...descriptio
-0000b550: 6e94 8c1c 4c61 7374 2075 7064 6174 6520  n...Last update 
-0000b560: 7469 6d65 7374 616d 7020 696e 2055 5443  timestamp in UTC
-0000b570: 9475 7575 8c08 4964 5374 7269 6e67 947d  .uuu..IdString.}
+00000780: 7320 5245 4144 206f 7220 4d4f 4449 4659  s READ or MODIFY
+00000790: 2061 6363 6573 7320 746f 2074 6865 2070   access to the p
+000007a0: 6174 682e 0a0a 506c 6561 7365 206e 6f74  ath...Please not
+000007b0: 6520 7468 6174 2074 6865 2075 6e64 6572  e that the under
+000007c0: 6c79 696e 6720 686f 7374 2061 7373 6f63  lying host assoc
+000007d0: 6961 7465 6420 7769 7468 2061 2073 7973  iated with a sys
+000007e0: 7465 6d20 7479 7069 6361 6c6c 7920 616c  tem typically al
+000007f0: 736f 2068 6173 2069 7427 7320 6f77 6e20  so has it's own 
+00000800: 6163 6365 7373 2063 6f6e 7472 6f6c 732e  access controls.
+00000810: 0a94 7565 8c05 7061 7468 7394 7d94 288c  ..ue..paths.}.(.
+00000820: 152f 7633 2f66 696c 6573 2f68 6561 6c74  ./v3/files/healt
+00000830: 6863 6865 636b 947d 948c 0367 6574 947d  hcheck.}...get.}
+00000840: 9428 8c04 7461 6773 945d 948c 0747 656e  .(..tags.]...Gen
+00000850: 6572 616c 9461 8c0b 6465 7363 7269 7074  eral.a..descript
+00000860: 696f 6e94 8c0c 4865 616c 7468 2063 6865  ion...Health che
+00000870: 636b 948c 0b6f 7065 7261 7469 6f6e 4964  ck...operationId
+00000880: 948c 0b68 6561 6c74 6843 6865 636b 948c  ...healthCheck..
+00000890: 0972 6573 706f 6e73 6573 947d 9428 8c03  .responses.}.(..
+000008a0: 3230 3094 7d94 288c 0b64 6573 6372 6970  200.}.(..descrip
+000008b0: 7469 6f6e 948c 114d 6573 7361 6765 2072  tion...Message r
+000008c0: 6563 6569 7665 642e 948c 0763 6f6e 7465  eceived....conte
+000008d0: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
+000008e0: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
+000008f0: 6d61 947d 948c 0424 7265 6694 8c1e 232f  ma.}...$ref...#/
+00000900: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+00000910: 6173 2f52 6573 7042 6173 6963 9473 7373  as/RespBasic.sss
+00000920: 758c 0335 3030 947d 948c 0b64 6573 6372  u..500.}...descr
+00000930: 6970 7469 6f6e 948c 0d53 6572 7665 7220  iption...Server 
+00000940: 6572 726f 722e 9473 7575 738c 142f 7633  error..suus../v3
+00000950: 2f66 696c 6573 2f72 6561 6479 6368 6563  /files/readychec
+00000960: 6b94 7d94 8c03 6765 7494 7d94 288c 0474  k.}...get.}.(..t
+00000970: 6167 7394 5d94 8c07 4765 6e65 7261 6c94  ags.]...General.
+00000980: 618c 0b64 6573 6372 6970 7469 6f6e 948c  a..description..
+00000990: 0b52 6561 6479 2063 6865 636b 948c 0b6f  .Ready check...o
+000009a0: 7065 7261 7469 6f6e 4964 948c 0a72 6561  perationId...rea
+000009b0: 6479 4368 6563 6b94 8c09 7265 7370 6f6e  dyCheck...respon
+000009c0: 7365 7394 7d94 288c 0332 3030 947d 9428  ses.}.(..200.}.(
+000009d0: 8c0b 6465 7363 7269 7074 696f 6e94 8c0e  ..description...
+000009e0: 5365 7276 6963 6520 7265 6164 792e 948c  Service ready...
+000009f0: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
+00000a00: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
+00000a10: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
+00000a20: 6694 8c1e 232f 636f 6d70 6f6e 656e 7473  f...#/components
+00000a30: 2f73 6368 656d 6173 2f52 6573 7042 6173  /schemas/RespBas
+00000a40: 6963 9473 7373 758c 0335 3033 947d 948c  ic.sssu..503.}..
+00000a50: 0b64 6573 6372 6970 7469 6f6e 948c 1453  .description...S
+00000a60: 6572 7669 6365 2075 6e61 7661 696c 6162  ervice unavailab
+00000a70: 6c65 2e94 7375 7573 8c1f 2f76 332f 6669  le..suus../v3/fi
+00000a80: 6c65 732f 6f70 732f 7b73 7973 7465 6d49  les/ops/{systemI
+00000a90: 647d 2f7b 7061 7468 7d94 7d94 288c 0367  d}/{path}.}.(..g
+00000aa0: 6574 947d 9428 8c04 7461 6773 945d 948c  et.}.(..tags.]..
+00000ab0: 0f46 696c 6520 4f70 6572 6174 696f 6e73  .File Operations
+00000ac0: 9461 8c0b 6465 7363 7269 7074 696f 6e94  .a..description.
+00000ad0: 58b6 0300 004c 6973 7420 6669 6c65 7320  X....List files 
+00000ae0: 6f72 206f 626a 6563 7473 206f 6e20 6120  or objects on a 
+00000af0: 5461 7069 7320 7379 7374 656d 2e20 5479  Tapis system. Ty
+00000b00: 7065 2066 6f72 2069 7465 6d73 2077 696c  pe for items wil
+00000b10: 6c20 6465 7065 6e64 206f 6e20 7379 7374  l depend on syst
+00000b20: 656d 2074 7970 652e 2046 6f72 2065 7861  em type. For exa
+00000b30: 6d70 6c65 2c20 666f 7220 4c49 4e55 580a  mple, for LINUX.
+00000b40: 7468 6579 2077 696c 6c20 6265 2070 6f73  they will be pos
+00000b50: 6978 2066 696c 6573 2061 6e64 2066 6f72  ix files and for
+00000b60: 2053 3320 7468 6579 2077 696c 6c20 6265   S3 they will be
+00000b70: 2073 746f 7261 6765 206f 626a 6563 7473   storage objects
+00000b80: 2e20 466f 7220 5333 2074 6865 2072 6563  . For S3 the rec
+00000b90: 7572 7365 2066 6c61 6720 6973 2069 676e  urse flag is ign
+00000ba0: 6f72 6564 2061 6e64 2061 6c6c 0a6f 626a  ored and all.obj
+00000bb0: 6563 7473 2077 6974 6820 6b65 7973 206d  ects with keys m
+00000bc0: 6174 6368 696e 6720 7468 6520 7061 7468  atching the path
+00000bd0: 2061 7320 6120 7072 6566 6978 2061 7265   as a prefix are
+00000be0: 2069 6e63 6c75 6465 642e 0a0a 466f 7220   included...For 
+00000bf0: 7379 7374 656d 2074 7970 6573 2074 6861  system types tha
+00000c00: 7420 7375 7070 6f72 7420 6469 7265 6374  t support direct
+00000c10: 6f72 7920 6869 6572 6172 6368 6965 7320  ory hierarchies 
+00000c20: 7468 6520 6d61 7869 6d75 6d20 7265 6375  the maximum recu
+00000c30: 7273 696f 6e20 6465 7074 6820 6973 2032  rsion depth is 2
+00000c40: 302e 0a0a 4e6f 7465 2074 6861 7420 5333  0...Note that S3
+00000c50: 2062 7563 6b65 7473 2064 6f20 6e6f 7420   buckets do not 
+00000c60: 6861 7665 2061 2068 6965 7261 7263 6869  have a hierarchi
+00000c70: 6361 6c20 7374 7275 6374 7572 652e 2054  cal structure. T
+00000c80: 6865 7265 2061 7265 206e 6f20 6469 7265  here are no dire
+00000c90: 6374 6f72 6965 732e 2045 7665 7279 7468  ctories. Everyth
+00000ca0: 696e 6720 6973 2061 6e20 6f62 6a65 6374  ing is an object
+00000cb0: 0a61 7373 6f63 6961 7465 6420 7769 7468  .associated with
+00000cc0: 2061 206b 6579 2e0a 0a43 6572 7461 696e   a key...Certain
+00000cd0: 2073 6572 7669 6365 7320 6d61 7920 7573   services may us
+00000ce0: 6520 7468 6520 7175 6572 7920 7061 7261  e the query para
+00000cf0: 6d65 7465 7220 2a69 6d70 6572 736f 6e61  meter *impersona
+00000d00: 7469 6f6e 4964 2a20 746f 2062 6520 7573  tionId* to be us
+00000d10: 6564 2069 6e20 706c 6163 6520 6f66 2074  ed in place of t
+00000d20: 6865 2072 6571 7565 7374 696e 670a 5461  he requesting.Ta
+00000d30: 7069 7320 7573 6572 2e20 5461 7069 7320  pis user. Tapis 
+00000d40: 7769 6c6c 2075 7365 2074 6869 7320 7573  will use this us
+00000d50: 6572 2049 6420 7768 656e 2070 6572 666f  er Id when perfo
+00000d60: 726d 696e 6720 6175 7468 6f72 697a 6174  rming authorizat
+00000d70: 696f 6e20 616e 6420 7265 736f 6c76 696e  ion and resolvin
+00000d80: 6720 7468 6520 2a65 6666 6563 7469 7665  g the *effective
+00000d90: 5573 6572 4964 2a0a 666f 7220 7468 6520  UserId*.for the 
+00000da0: 7379 7374 656d 2e0a 0a43 6572 7461 696e  system...Certain
+00000db0: 2073 6572 7669 6365 7320 6d61 7920 7573   services may us
+00000dc0: 6520 7468 6520 7175 6572 7920 7061 7261  e the query para
+00000dd0: 6d65 7465 7220 2a73 6861 7265 6443 7478  meter *sharedCtx
+00000de0: 2a20 746f 2069 6e64 6963 6174 6520 7468  * to indicate th
+00000df0: 6174 2074 6865 2072 6571 7565 7374 2069  at the request i
+00000e00: 7320 696e 2061 2073 6861 7265 640a 636f  s in a shared.co
+00000e10: 6e74 6578 742e 202a 7368 6172 6564 4374  ntext. *sharedCt
+00000e20: 782a 206d 7573 7420 6265 2073 6574 2074  x* must be set t
+00000e30: 6f20 7468 6520 7368 6172 6520 6772 616e  o the share gran
+00000e40: 746f 722e 0a54 6170 6973 2077 696c 6c20  tor..Tapis will 
+00000e50: 696e 636c 7564 6520 7468 6520 7368 6172  include the shar
+00000e60: 6520 6772 616e 746f 7220 6173 2070 6172  e grantor as par
+00000e70: 7420 6f66 2061 7574 686f 7269 7a61 7469  t of authorizati
+00000e80: 6f6e 2063 6865 636b 732e 0a94 8c0b 6f70  on checks.....op
+00000e90: 6572 6174 696f 6e49 6494 8c09 6c69 7374  erationId...list
+00000ea0: 4669 6c65 7394 8c0a 7061 7261 6d65 7465  Files...paramete
+00000eb0: 7273 945d 9428 7d94 288c 046e 616d 6594  rs.].(}.(..name.
+00000ec0: 8c08 7379 7374 656d 4964 948c 0269 6e94  ..systemId...in.
+00000ed0: 8c04 7061 7468 948c 0b64 6573 6372 6970  ..path...descrip
+00000ee0: 7469 6f6e 948c 0953 7973 7465 6d20 4944  tion...System ID
+00000ef0: 948c 0872 6571 7569 7265 6494 888c 0673  ...required....s
+00000f00: 6368 656d 6194 7d94 8c04 7479 7065 948c  chema.}...type..
+00000f10: 0673 7472 696e 6794 738c 0765 7861 6d70  .string.s..examp
+00000f20: 6c65 948c 0973 7973 7465 6d31 3233 9475  le...system123.u
+00000f30: 7d94 288c 046e 616d 6594 8c04 7061 7468  }.(..name...path
+00000f40: 948c 0269 6e94 8c04 7061 7468 948c 0b64  ...in...path...d
+00000f50: 6573 6372 6970 7469 6f6e 948c 2550 6174  escription..%Pat
+00000f60: 6820 7265 6c61 7469 7665 2074 6f20 7468  h relative to th
+00000f70: 6520 7379 7374 656d 202a 726f 6f74 4469  e system *rootDi
+00000f80: 722a 948c 0872 6571 7569 7265 6494 888c  r*...required...
+00000f90: 0673 6368 656d 6194 7d94 8c04 7479 7065  .schema.}...type
+00000fa0: 948c 0673 7472 696e 6794 738c 0765 7861  ...string.s..exa
+00000fb0: 6d70 6c65 948c 1664 6972 6563 746f 7279  mple...directory
+00000fc0: 412f 6469 7265 6374 6f72 7942 2f94 757d  A/directoryB/.u}
+00000fd0: 9428 8c04 6e61 6d65 948c 056c 696d 6974  .(..name...limit
+00000fe0: 948c 0269 6e94 8c05 7175 6572 7994 8c0b  ...in...query...
+00000ff0: 6465 7363 7269 7074 696f 6e94 8c10 7061  description...pa
+00001000: 6769 6e61 7469 6f6e 206c 696d 6974 948c  gination limit..
+00001010: 0673 6368 656d 6194 7d94 288c 0474 7970  .schema.}.(..typ
+00001020: 6594 8c07 696e 7465 6765 7294 8c06 666f  e...integer...fo
+00001030: 726d 6174 948c 0569 6e74 3332 948c 0764  rmat...int32...d
+00001040: 6566 6175 6c74 944d e803 758c 0765 7861  efault.M..u..exa
+00001050: 6d70 6c65 944b 6475 7d94 288c 046e 616d  mple.Kdu}.(..nam
+00001060: 6594 8c06 6f66 6673 6574 948c 0269 6e94  e...offset...in.
+00001070: 8c05 7175 6572 7994 8c0b 6465 7363 7269  ..query...descri
+00001080: 7074 696f 6e94 8c11 7061 6769 6e61 7469  ption...paginati
+00001090: 6f6e 206f 6666 7365 7494 8c06 7363 6865  on offset...sche
+000010a0: 6d61 947d 9428 8c04 7479 7065 948c 0769  ma.}.(..type...i
+000010b0: 6e74 6567 6572 948c 0666 6f72 6d61 7494  nteger...format.
+000010c0: 8c05 696e 7436 3494 8c07 6465 6661 756c  ..int64...defaul
+000010d0: 7494 4b00 758c 0765 7861 6d70 6c65 944d  t.K.u..example.M
+000010e0: e803 757d 9428 8c04 6e61 6d65 948c 0772  ..u}.(..name...r
+000010f0: 6563 7572 7365 948c 0269 6e94 8c05 7175  ecurse...in...qu
+00001100: 6572 7994 8c0b 6465 7363 7269 7074 696f  ery...descriptio
+00001110: 6e94 8c31 5265 6375 7273 6976 6520 6c69  n..1Recursive li
+00001120: 7374 696e 672e 204d 6178 696d 756d 2072  sting. Maximum r
+00001130: 6563 7572 7369 6f6e 2064 6570 7468 2069  ecursion depth i
+00001140: 7320 3230 2e94 8c06 7363 6865 6d61 947d  s 20....schema.}
+00001150: 9428 8c04 7479 7065 948c 0762 6f6f 6c65  .(..type...boole
+00001160: 616e 948c 0764 6566 6175 6c74 9489 758c  an...default..u.
+00001170: 0765 7861 6d70 6c65 9489 757d 9428 8c04  .example..u}.(..
+00001180: 6e61 6d65 948c 0f69 6d70 6572 736f 6e61  name...impersona
+00001190: 7469 6f6e 4964 948c 0269 6e94 8c05 7175  tionId...in...qu
+000011a0: 6572 7994 8c0b 6465 7363 7269 7074 696f  ery...descriptio
+000011b0: 6e94 8c3f 5265 7374 7269 6374 6564 2e20  n..?Restricted. 
+000011c0: 4f6e 6c79 2063 6572 7461 696e 2073 6572  Only certain ser
+000011d0: 7669 6365 7320 6d61 7920 696d 7065 7273  vices may impers
+000011e0: 6f6e 6174 6520 6120 5461 7069 7320 7573  onate a Tapis us
+000011f0: 6572 2e94 8c06 7363 6865 6d61 947d 948c  er....schema.}..
+00001200: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+00001210: 757d 9428 8c04 6e61 6d65 948c 0973 6861  u}.(..name...sha
+00001220: 7265 6443 7478 948c 0269 6e94 8c05 7175  redCtx...in...qu
+00001230: 6572 7994 8c0b 6465 7363 7269 7074 696f  ery...descriptio
+00001240: 6e94 8c79 5265 7374 7269 6374 6564 2e20  n..yRestricted. 
+00001250: 4f6e 6c79 2063 6572 7461 696e 2073 6572  Only certain ser
+00001260: 7669 6365 7320 6d61 7920 696e 6469 6361  vices may indica
+00001270: 7465 2074 6861 7420 7468 6520 7265 7175  te that the requ
+00001280: 6573 7420 6973 2069 6e20 6120 7368 6172  est is in a shar
+00001290: 6564 2063 6f6e 7465 7874 2e20 4d75 7374  ed context. Must
+000012a0: 2062 6520 7365 7420 746f 2074 6865 2073   be set to the s
+000012b0: 6861 7265 2067 7261 6e74 6f72 2e94 8c06  hare grantor....
+000012c0: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
+000012d0: 8c23 232f 636f 6d70 6f6e 656e 7473 2f73  .##/components/s
+000012e0: 6368 656d 6173 2f55 7365 724e 616d 6553  chemas/UserNameS
+000012f0: 7472 696e 6794 7375 658c 0972 6573 706f  tring.sue..respo
+00001300: 6e73 6573 947d 9428 8c03 3230 3094 7d94  nses.}.(..200.}.
+00001310: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
+00001320: 0f41 206c 6973 7420 6f66 2066 696c 6573  .A list of files
+00001330: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
+00001340: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
+00001350: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
+00001360: 7265 6694 8c28 232f 636f 6d70 6f6e 656e  ref..(#/componen
+00001370: 7473 2f73 6368 656d 6173 2f46 696c 654c  ts/schemas/FileL
+00001380: 6973 7469 6e67 5265 7370 6f6e 7365 9473  istingResponse.s
+00001390: 7373 758c 0334 3030 947d 9428 8c0b 6465  ssu..400.}.(..de
+000013a0: 7363 7269 7074 696f 6e94 8c0b 4261 6420  scription...Bad 
+000013b0: 5265 7175 6573 7494 8c07 636f 6e74 656e  Request...conten
+000013c0: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
+000013d0: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
+000013e0: 6194 7d94 8c04 2472 6566 948c 2723 2f63  a.}...$ref..'#/c
+000013f0: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+00001400: 732f 4669 6c65 5374 7269 6e67 5265 7370  s/FileStringResp
+00001410: 6f6e 7365 9473 7373 758c 0334 3031 947d  onse.sssu..401.}
+00001420: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
+00001430: 8c11 4e6f 7420 4175 7468 656e 7469 6361  ..Not Authentica
+00001440: 7465 6494 8c07 636f 6e74 656e 7494 7d94  ted...content.}.
+00001450: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
+00001460: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
+00001470: 8c04 2472 6566 948c 2723 2f63 6f6d 706f  ..$ref..'#/compo
+00001480: 6e65 6e74 732f 7363 6865 6d61 732f 4669  nents/schemas/Fi
+00001490: 6c65 5374 7269 6e67 5265 7370 6f6e 7365  leStringResponse
+000014a0: 9473 7373 758c 0334 3033 947d 9428 8c0b  .sssu..403.}.(..
+000014b0: 6465 7363 7269 7074 696f 6e94 8c11 5065  description...Pe
+000014c0: 726d 6973 7369 6f6e 2044 656e 6965 6494  rmission Denied.
+000014d0: 8c07 636f 6e74 656e 7494 7d94 8c10 6170  ..content.}...ap
+000014e0: 706c 6963 6174 696f 6e2f 6a73 6f6e 947d  plication/json.}
+000014f0: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
+00001500: 6566 948c 2723 2f63 6f6d 706f 6e65 6e74  ef..'#/component
+00001510: 732f 7363 6865 6d61 732f 4669 6c65 5374  s/schemas/FileSt
+00001520: 7269 6e67 5265 7370 6f6e 7365 9473 7373  ringResponse.sss
+00001530: 758c 0334 3034 947d 9428 8c0b 6465 7363  u..404.}.(..desc
+00001540: 7269 7074 696f 6e94 8c09 4e6f 7420 466f  ription...Not Fo
+00001550: 756e 6494 8c07 636f 6e74 656e 7494 7d94  und...content.}.
+00001560: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
+00001570: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
+00001580: 8c04 2472 6566 948c 2723 2f63 6f6d 706f  ..$ref..'#/compo
+00001590: 6e65 6e74 732f 7363 6865 6d61 732f 4669  nents/schemas/Fi
+000015a0: 6c65 5374 7269 6e67 5265 7370 6f6e 7365  leStringResponse
+000015b0: 9473 7373 758c 0335 3030 947d 9428 8c0b  .sssu..500.}.(..
+000015c0: 6465 7363 7269 7074 696f 6e94 8c0e 496e  description...In
+000015d0: 7465 726e 616c 2045 7272 6f72 948c 0763  ternal Error...c
+000015e0: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
+000015f0: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
+00001600: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
+00001610: 8c27 232f 636f 6d70 6f6e 656e 7473 2f73  .'#/components/s
+00001620: 6368 656d 6173 2f46 696c 6553 7472 696e  chemas/FileStrin
+00001630: 6752 6573 706f 6e73 6594 7373 7375 7575  gResponse.sssuuu
+00001640: 8c03 7075 7494 7d94 288c 0474 6167 7394  ..put.}.(..tags.
+00001650: 5d94 8c0f 4669 6c65 204f 7065 7261 7469  ]...File Operati
+00001660: 6f6e 7394 618c 0b64 6573 6372 6970 7469  ons.a..descripti
+00001670: 6f6e 948c 7a4d 6f76 6520 6f72 2063 6f70  on..zMove or cop
+00001680: 7920 6120 6669 6c65 2c20 6469 7265 6374  y a file, direct
+00001690: 6f72 7920 6f72 206f 626a 6563 7420 6f6e  ory or object on
+000016a0: 207b 7379 7374 656d 4944 7d20 6174 2070   {systemID} at p
+000016b0: 6174 6820 7b70 6174 687d 2e20 4e6f 7420  ath {path}. Not 
+000016c0: 616c 6c20 6f70 6572 6174 696f 6e73 2073  all operations s
+000016d0: 7570 706f 7274 6564 2066 6f72 2061 6c6c  upported for all
+000016e0: 0a73 7973 7465 6d20 7479 7065 732e 0a94  .system types...
+000016f0: 8c0b 6f70 6572 6174 696f 6e49 6494 8c08  ..operationId...
+00001700: 6d6f 7665 436f 7079 948c 0a70 6172 616d  moveCopy...param
+00001710: 6574 6572 7394 5d94 287d 9428 8c04 6e61  eters.].(}.(..na
+00001720: 6d65 948c 0873 7973 7465 6d49 6494 8c02  me...systemId...
+00001730: 696e 948c 0470 6174 6894 8c0b 6465 7363  in...path...desc
+00001740: 7269 7074 696f 6e94 8c09 5379 7374 656d  ription...System
+00001750: 2049 4494 8c08 7265 7175 6972 6564 9488   ID...required..
+00001760: 8c06 7363 6865 6d61 947d 948c 0474 7970  ..schema.}...typ
+00001770: 6594 8c06 7374 7269 6e67 9473 757d 9428  e...string.su}.(
+00001780: 8c04 6e61 6d65 948c 0470 6174 6894 8c02  ..name...path...
+00001790: 696e 948c 0470 6174 6894 8c0b 6465 7363  in...path...desc
+000017a0: 7269 7074 696f 6e94 8c25 5061 7468 2072  ription..%Path r
+000017b0: 656c 6174 6976 6520 746f 2074 6865 2073  elative to the s
+000017c0: 7973 7465 6d20 2a72 6f6f 7444 6972 2a94  ystem *rootDir*.
+000017d0: 8c08 7265 7175 6972 6564 9488 8c06 7363  ..required....sc
+000017e0: 6865 6d61 947d 948c 0474 7970 6594 8c06  hema.}...type...
+000017f0: 7374 7269 6e67 9473 7565 8c0b 7265 7175  string.sue..requ
+00001800: 6573 7442 6f64 7994 7d94 8c07 636f 6e74  estBody.}...cont
+00001810: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
+00001820: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
+00001830: 656d 6194 7d94 8c04 2472 6566 948c 2423  ema.}...$ref..$#
+00001840: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+00001850: 6d61 732f 4d6f 7665 436f 7079 5265 7175  mas/MoveCopyRequ
+00001860: 6573 7494 7373 7373 8c09 7265 7370 6f6e  est.ssss..respon
+00001870: 7365 7394 7d94 288c 0332 3030 947d 9428  ses.}.(..200.}.(
+00001880: 8c0b 6465 7363 7269 7074 696f 6e94 8c02  ..description...
+00001890: 4f4b 948c 0763 6f6e 7465 6e74 947d 948c  OK...content.}..
+000018a0: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
+000018b0: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
+000018c0: 0424 7265 6694 8c27 232f 636f 6d70 6f6e  .$ref..'#/compon
+000018d0: 656e 7473 2f73 6368 656d 6173 2f46 696c  ents/schemas/Fil
+000018e0: 6553 7472 696e 6752 6573 706f 6e73 6594  eStringResponse.
+000018f0: 7373 7375 8c03 3430 3094 7d94 288c 0b64  sssu..400.}.(..d
+00001900: 6573 6372 6970 7469 6f6e 948c 0b42 6164  escription...Bad
+00001910: 2052 6571 7565 7374 948c 0763 6f6e 7465   Request...conte
+00001920: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
+00001930: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
+00001940: 6d61 947d 948c 0424 7265 6694 8c27 232f  ma.}...$ref..'#/
+00001950: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+00001960: 6173 2f46 696c 6553 7472 696e 6752 6573  as/FileStringRes
+00001970: 706f 6e73 6594 7373 7375 8c03 3430 3194  ponse.sssu..401.
+00001980: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
+00001990: 948c 114e 6f74 2041 7574 6865 6e74 6963  ...Not Authentic
+000019a0: 6174 6564 948c 0763 6f6e 7465 6e74 947d  ated...content.}
+000019b0: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
+000019c0: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
+000019d0: 948c 0424 7265 6694 8c27 232f 636f 6d70  ...$ref..'#/comp
+000019e0: 6f6e 656e 7473 2f73 6368 656d 6173 2f46  onents/schemas/F
+000019f0: 696c 6553 7472 696e 6752 6573 706f 6e73  ileStringRespons
+00001a00: 6594 7373 7375 8c03 3430 3394 7d94 288c  e.sssu..403.}.(.
+00001a10: 0b64 6573 6372 6970 7469 6f6e 948c 1150  .description...P
+00001a20: 6572 6d69 7373 696f 6e20 4465 6e69 6564  ermission Denied
+00001a30: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
+00001a40: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
+00001a50: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
+00001a60: 7265 6694 8c27 232f 636f 6d70 6f6e 656e  ref..'#/componen
+00001a70: 7473 2f73 6368 656d 6173 2f46 696c 6553  ts/schemas/FileS
+00001a80: 7472 696e 6752 6573 706f 6e73 6594 7373  tringResponse.ss
+00001a90: 7375 8c03 3430 3494 7d94 288c 0b64 6573  su..404.}.(..des
+00001aa0: 6372 6970 7469 6f6e 948c 094e 6f74 2046  cription...Not F
+00001ab0: 6f75 6e64 948c 0763 6f6e 7465 6e74 947d  ound...content.}
+00001ac0: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
+00001ad0: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
+00001ae0: 948c 0424 7265 6694 8c27 232f 636f 6d70  ...$ref..'#/comp
+00001af0: 6f6e 656e 7473 2f73 6368 656d 6173 2f46  onents/schemas/F
+00001b00: 696c 6553 7472 696e 6752 6573 706f 6e73  ileStringRespons
+00001b10: 6594 7373 7375 8c03 3530 3094 7d94 288c  e.sssu..500.}.(.
+00001b20: 0b64 6573 6372 6970 7469 6f6e 948c 0e49  .description...I
+00001b30: 6e74 6572 6e61 6c20 4572 726f 7294 8c07  nternal Error...
+00001b40: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
+00001b50: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
+00001b60: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
+00001b70: 948c 2723 2f63 6f6d 706f 6e65 6e74 732f  ..'#/components/
+00001b80: 7363 6865 6d61 732f 4669 6c65 5374 7269  schemas/FileStri
+00001b90: 6e67 5265 7370 6f6e 7365 9473 7373 7575  ngResponse.sssuu
+00001ba0: 758c 0470 6f73 7494 7d94 288c 0474 6167  u..post.}.(..tag
+00001bb0: 7394 5d94 8c0f 4669 6c65 204f 7065 7261  s.]...File Opera
+00001bc0: 7469 6f6e 7394 618c 0b64 6573 6372 6970  tions.a..descrip
+00001bd0: 7469 6f6e 948c 5454 6865 2066 696c 6520  tion..TThe file 
+00001be0: 6f72 206f 626a 6563 7420 7769 6c6c 2062  or object will b
+00001bf0: 6520 7570 6c6f 6164 6564 2061 7420 7468  e uploaded at th
+00001c00: 6520 7b70 6174 687d 2069 6e64 6570 656e  e {path} indepen
+00001c10: 6465 6e74 206f 6620 7468 6520 6f72 6967  dent of the orig
+00001c20: 696e 616c 206e 616d 652e 0a94 8c0b 6f70  inal name.....op
+00001c30: 6572 6174 696f 6e49 6494 8c06 696e 7365  erationId...inse
+00001c40: 7274 948c 0a70 6172 616d 6574 6572 7394  rt...parameters.
+00001c50: 5d94 287d 9428 8c04 6e61 6d65 948c 0873  ].(}.(..name...s
+00001c60: 7973 7465 6d49 6494 8c02 696e 948c 0470  ystemId...in...p
+00001c70: 6174 6894 8c0b 6465 7363 7269 7074 696f  ath...descriptio
+00001c80: 6e94 8c09 5379 7374 656d 2049 4494 8c08  n...System ID...
+00001c90: 7265 7175 6972 6564 9488 8c06 7363 6865  required....sche
+00001ca0: 6d61 947d 948c 0474 7970 6594 8c06 7374  ma.}...type...st
+00001cb0: 7269 6e67 9473 757d 9428 8c04 6e61 6d65  ring.su}.(..name
+00001cc0: 948c 0470 6174 6894 8c02 696e 948c 0470  ...path...in...p
+00001cd0: 6174 6894 8c0b 6465 7363 7269 7074 696f  ath...descriptio
+00001ce0: 6e94 8c25 5061 7468 2072 656c 6174 6976  n..%Path relativ
+00001cf0: 6520 746f 2074 6865 2073 7973 7465 6d20  e to the system 
+00001d00: 2a72 6f6f 7444 6972 2a94 8c08 7265 7175  *rootDir*...requ
+00001d10: 6972 6564 9488 8c06 7363 6865 6d61 947d  ired....schema.}
+00001d20: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+00001d30: 9473 7565 8c0b 7265 7175 6573 7442 6f64  .sue..requestBod
+00001d40: 7994 7d94 8c07 636f 6e74 656e 7494 7d94  y.}...content.}.
+00001d50: 8c13 6d75 6c74 6970 6172 742f 666f 726d  ..multipart/form
+00001d60: 2d64 6174 6194 7d94 8c06 7363 6865 6d61  -data.}...schema
+00001d70: 947d 9428 8c08 7265 7175 6972 6564 945d  .}.(..required.]
+00001d80: 948c 0466 696c 6594 618c 0474 7970 6594  ...file.a..type.
+00001d90: 8c06 6f62 6a65 6374 948c 0a70 726f 7065  ..object...prope
+00001da0: 7274 6965 7394 7d94 8c04 6669 6c65 947d  rties.}...file.}
+00001db0: 9428 8c04 7479 7065 948c 0673 7472 696e  .(..type...strin
+00001dc0: 6794 8c06 666f 726d 6174 948c 0662 696e  g...format...bin
+00001dd0: 6172 7994 7573 7573 7373 8c09 7265 7370  ary.ususss..resp
+00001de0: 6f6e 7365 7394 7d94 288c 0332 3030 947d  onses.}.(..200.}
+00001df0: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
+00001e00: 8c02 4f4b 948c 0763 6f6e 7465 6e74 947d  ..OK...content.}
+00001e10: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
+00001e20: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
+00001e30: 948c 0424 7265 6694 8c27 232f 636f 6d70  ...$ref..'#/comp
+00001e40: 6f6e 656e 7473 2f73 6368 656d 6173 2f46  onents/schemas/F
+00001e50: 696c 6553 7472 696e 6752 6573 706f 6e73  ileStringRespons
+00001e60: 6594 7373 7375 8c03 3430 3094 7d94 288c  e.sssu..400.}.(.
+00001e70: 0b64 6573 6372 6970 7469 6f6e 948c 0b42  .description...B
+00001e80: 6164 2052 6571 7565 7374 948c 0763 6f6e  ad Request...con
+00001e90: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
+00001ea0: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
+00001eb0: 6865 6d61 947d 948c 0424 7265 6694 8c27  hema.}...$ref..'
+00001ec0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+00001ed0: 656d 6173 2f46 696c 6553 7472 696e 6752  emas/FileStringR
+00001ee0: 6573 706f 6e73 6594 7373 7375 8c03 3430  esponse.sssu..40
+00001ef0: 3194 7d94 288c 0b64 6573 6372 6970 7469  1.}.(..descripti
+00001f00: 6f6e 948c 114e 6f74 2041 7574 6865 6e74  on...Not Authent
+00001f10: 6963 6174 6564 948c 0763 6f6e 7465 6e74  icated...content
+00001f20: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
+00001f30: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
+00001f40: 947d 948c 0424 7265 6694 8c27 232f 636f  .}...$ref..'#/co
+00001f50: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00001f60: 2f46 696c 6553 7472 696e 6752 6573 706f  /FileStringRespo
+00001f70: 6e73 6594 7373 7375 8c03 3430 3394 7d94  nse.sssu..403.}.
+00001f80: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
+00001f90: 1150 6572 6d69 7373 696f 6e20 4465 6e69  .Permission Deni
+00001fa0: 6564 948c 0763 6f6e 7465 6e74 947d 948c  ed...content.}..
+00001fb0: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
+00001fc0: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
+00001fd0: 0424 7265 6694 8c27 232f 636f 6d70 6f6e  .$ref..'#/compon
+00001fe0: 656e 7473 2f73 6368 656d 6173 2f46 696c  ents/schemas/Fil
+00001ff0: 6553 7472 696e 6752 6573 706f 6e73 6594  eStringResponse.
+00002000: 7373 7375 8c03 3530 3094 7d94 288c 0b64  sssu..500.}.(..d
+00002010: 6573 6372 6970 7469 6f6e 948c 0e49 6e74  escription...Int
+00002020: 6572 6e61 6c20 4572 726f 7294 8c07 636f  ernal Error...co
+00002030: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
+00002040: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
+00002050: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
+00002060: 2723 2f63 6f6d 706f 6e65 6e74 732f 7363  '#/components/sc
+00002070: 6865 6d61 732f 4669 6c65 5374 7269 6e67  hemas/FileString
+00002080: 5265 7370 6f6e 7365 9473 7373 7575 758c  Response.sssuuu.
+00002090: 0664 656c 6574 6594 7d94 288c 0474 6167  .delete.}.(..tag
+000020a0: 7394 5d94 8c0f 4669 6c65 204f 7065 7261  s.]...File Opera
+000020b0: 7469 6f6e 7394 618c 0b64 6573 6372 6970  tions.a..descrip
+000020c0: 7469 6f6e 9458 1b02 0000 4465 6c65 7465  tion.X....Delete
+000020d0: 2061 2066 696c 652c 2064 6972 6563 746f   a file, directo
+000020e0: 7279 206f 7220 6f62 6a65 6374 206f 6e20  ry or object on 
+000020f0: 7b73 7973 7465 6d49 447d 2061 7420 7061  {systemID} at pa
+00002100: 7468 207b 7061 7468 7d2e 0a0a 466f 7220  th {path}...For 
+00002110: 6120 4c49 4e55 5820 6469 7265 6374 6f72  a LINUX director
+00002120: 7920 7468 6973 2077 696c 6c20 6265 2061  y this will be a
+00002130: 2072 6563 7572 7369 7665 2064 656c 6574   recursive delet
+00002140: 652e 0a0a 466f 7220 616e 2053 3320 7379  e...For an S3 sy
+00002150: 7374 656d 2c20 7468 6520 7061 7468 2077  stem, the path w
+00002160: 696c 6c20 7265 7072 6573 656e 7420 6569  ill represent ei
+00002170: 7468 6572 2061 2073 696e 676c 6520 6f62  ther a single ob
+00002180: 6a65 6374 206f 7220 616c 6c20 6f62 6a65  ject or all obje
+00002190: 6374 7320 696e 2074 6865 2062 7563 6b65  cts in the bucke
+000021a0: 7420 7769 7468 2061 2070 7265 6669 780a  t with a prefix.
+000021b0: 6d61 7463 6869 6e67 2074 6865 2073 7973  matching the sys
+000021c0: 7465 6d20 2a72 6f6f 7444 6972 2a20 6966  tem *rootDir* if
+000021d0: 2074 6865 2070 6174 6820 6973 2074 6865   the path is the
+000021e0: 2065 6d70 7479 2073 7472 696e 672e 0a0a   empty string...
+000021f0: 2a2a 5741 524e 494e 472a 2a20 466f 7220  **WARNING** For 
+00002200: 616e 2053 3320 7379 7374 656d 2069 6620  an S3 system if 
+00002210: 7468 6520 7061 7468 2069 7320 7468 6520  the path is the 
+00002220: 656d 7074 7920 7374 7269 6e67 2c20 7468  empty string, th
+00002230: 656e 2061 6c6c 206f 626a 6563 7473 2069  en all objects i
+00002240: 6e20 7468 6520 6275 636b 6574 2077 6974  n the bucket wit
+00002250: 6820 6120 6b65 7920 6d61 7463 6869 6e67  h a key matching
+00002260: 0a74 6865 2070 7265 6669 7820 2a72 6f6f  .the prefix *roo
+00002270: 7444 6972 2a20 7769 6c6c 2062 6520 6465  tDir* will be de
+00002280: 6c65 7465 642e 2053 6f20 6966 2074 6865  leted. So if the
+00002290: 202a 726f 6f74 4469 722a 2069 7320 616c   *rootDir* is al
+000022a0: 736f 2074 6865 2065 6d70 7479 2073 7472  so the empty str
+000022b0: 696e 672c 2074 6865 6e20 616c 6c20 6f62  ing, then all ob
+000022c0: 6a65 6374 7320 696e 2074 6865 2062 7563  jects in the buc
+000022d0: 6b65 740a 7769 6c6c 2062 6520 7265 6d6f  ket.will be remo
+000022e0: 7665 642e 0a94 8c0b 6f70 6572 6174 696f  ved.....operatio
+000022f0: 6e49 6494 8c06 6465 6c65 7465 948c 0a70  nId...delete...p
+00002300: 6172 616d 6574 6572 7394 5d94 287d 9428  arameters.].(}.(
+00002310: 8c04 6e61 6d65 948c 0873 7973 7465 6d49  ..name...systemI
+00002320: 6494 8c02 696e 948c 0470 6174 6894 8c0b  d...in...path...
+00002330: 6465 7363 7269 7074 696f 6e94 8c09 5379  description...Sy
+00002340: 7374 656d 2049 4494 8c08 7265 7175 6972  stem ID...requir
+00002350: 6564 9488 8c06 7363 6865 6d61 947d 948c  ed....schema.}..
+00002360: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+00002370: 757d 9428 8c04 6e61 6d65 948c 0470 6174  u}.(..name...pat
+00002380: 6894 8c02 696e 948c 0470 6174 6894 8c0b  h...in...path...
+00002390: 6465 7363 7269 7074 696f 6e94 8c25 5061  description..%Pa
+000023a0: 7468 2072 656c 6174 6976 6520 746f 2074  th relative to t
+000023b0: 6865 2073 7973 7465 6d20 2a72 6f6f 7444  he system *rootD
+000023c0: 6972 2a94 8c08 7265 7175 6972 6564 9488  ir*...required..
+000023d0: 8c06 7363 6865 6d61 947d 948c 0474 7970  ..schema.}...typ
+000023e0: 6594 8c06 7374 7269 6e67 9473 7565 8c09  e...string.sue..
+000023f0: 7265 7370 6f6e 7365 7394 7d94 288c 0332  responses.}.(..2
+00002400: 3030 947d 9428 8c0b 6465 7363 7269 7074  00.}.(..descript
+00002410: 696f 6e94 8c02 4f4b 948c 0763 6f6e 7465  ion...OK...conte
+00002420: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
+00002430: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
+00002440: 6d61 947d 948c 0424 7265 6694 8c27 232f  ma.}...$ref..'#/
+00002450: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+00002460: 6173 2f46 696c 6553 7472 696e 6752 6573  as/FileStringRes
+00002470: 706f 6e73 6594 7373 7375 8c03 3430 3094  ponse.sssu..400.
+00002480: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
+00002490: 948c 0b42 6164 2052 6571 7565 7374 948c  ...Bad Request..
+000024a0: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
+000024b0: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
+000024c0: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
+000024d0: 6694 8c27 232f 636f 6d70 6f6e 656e 7473  f..'#/components
+000024e0: 2f73 6368 656d 6173 2f46 696c 6553 7472  /schemas/FileStr
+000024f0: 696e 6752 6573 706f 6e73 6594 7373 7375  ingResponse.sssu
+00002500: 8c03 3430 3194 7d94 288c 0b64 6573 6372  ..401.}.(..descr
+00002510: 6970 7469 6f6e 948c 114e 6f74 2041 7574  iption...Not Aut
+00002520: 6865 6e74 6963 6174 6564 948c 0763 6f6e  henticated...con
+00002530: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
+00002540: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
+00002550: 6865 6d61 947d 948c 0424 7265 6694 8c27  hema.}...$ref..'
+00002560: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+00002570: 656d 6173 2f46 696c 6553 7472 696e 6752  emas/FileStringR
+00002580: 6573 706f 6e73 6594 7373 7375 8c03 3430  esponse.sssu..40
+00002590: 3394 7d94 288c 0b64 6573 6372 6970 7469  3.}.(..descripti
+000025a0: 6f6e 948c 1150 6572 6d69 7373 696f 6e20  on...Permission 
+000025b0: 4465 6e69 6564 948c 0763 6f6e 7465 6e74  Denied...content
+000025c0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
+000025d0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
+000025e0: 947d 948c 0424 7265 6694 8c27 232f 636f  .}...$ref..'#/co
+000025f0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00002600: 2f46 696c 6553 7472 696e 6752 6573 706f  /FileStringRespo
+00002610: 6e73 6594 7373 7375 8c03 3430 3494 7d94  nse.sssu..404.}.
+00002620: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
+00002630: 094e 6f74 2046 6f75 6e64 948c 0763 6f6e  .Not Found...con
+00002640: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
+00002650: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
+00002660: 6865 6d61 947d 948c 0424 7265 6694 8c27  hema.}...$ref..'
+00002670: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+00002680: 656d 6173 2f46 696c 6553 7472 696e 6752  emas/FileStringR
+00002690: 6573 706f 6e73 6594 7373 7375 8c03 3530  esponse.sssu..50
+000026a0: 3094 7d94 288c 0b64 6573 6372 6970 7469  0.}.(..descripti
+000026b0: 6f6e 948c 0e49 6e74 6572 6e61 6c20 4572  on...Internal Er
+000026c0: 726f 7294 8c07 636f 6e74 656e 7494 7d94  ror...content.}.
+000026d0: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
+000026e0: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
+000026f0: 8c04 2472 6566 948c 2723 2f63 6f6d 706f  ..$ref..'#/compo
+00002700: 6e65 6e74 732f 7363 6865 6d61 732f 4669  nents/schemas/Fi
+00002710: 6c65 5374 7269 6e67 5265 7370 6f6e 7365  leStringResponse
+00002720: 9473 7373 7575 7575 8c18 2f76 332f 6669  .sssuuuu../v3/fi
+00002730: 6c65 732f 6f70 732f 7b73 7973 7465 6d49  les/ops/{systemI
+00002740: 647d 947d 948c 0470 6f73 7494 7d94 288c  d}.}...post.}.(.
+00002750: 0474 6167 7394 5d94 8c0f 4669 6c65 204f  .tags.]...File O
+00002760: 7065 7261 7469 6f6e 7394 618c 0b64 6573  perations.a..des
+00002770: 6372 6970 7469 6f6e 9458 7101 0000 4372  cription.Xq...Cr
+00002780: 6561 7465 2061 2064 6972 6563 746f 7279  eate a directory
+00002790: 206f 6e20 7468 6520 7379 7374 656d 2061   on the system a
+000027a0: 7420 7468 6520 6769 7665 6e20 7061 7468  t the given path
+000027b0: 2e20 4e6f 7420 7375 7070 6f72 7465 6420  . Not supported 
+000027c0: 666f 7220 616c 6c20 7379 7374 656d 2074  for all system t
+000027d0: 7970 6573 2e20 4375 7272 656e 746c 7920  ypes. Currently 
+000027e0: 7375 7070 6f72 7465 640a 666f 7220 4c49  supported.for LI
+000027f0: 4e55 5820 616e 6420 4952 4f44 5320 7479  NUX and IRODS ty
+00002800: 7065 2073 7973 7465 6d73 2e0a 0a43 6572  pe systems...Cer
+00002810: 7461 696e 2073 6572 7669 6365 7320 6d61  tain services ma
+00002820: 7920 7573 6520 7468 6520 7175 6572 7920  y use the query 
+00002830: 7061 7261 6d65 7465 7220 2a73 6861 7265  parameter *share
+00002840: 6443 7478 2a20 746f 2069 6e64 6963 6174  dCtx* to indicat
+00002850: 6520 7468 6174 2074 6865 2072 6571 7565  e that the reque
+00002860: 7374 2069 7320 696e 2061 2073 6861 7265  st is in a share
+00002870: 640a 636f 6e74 6578 742e 202a 7368 6172  d.context. *shar
+00002880: 6564 4374 782a 206d 7573 7420 6265 2073  edCtx* must be s
+00002890: 6574 2074 6f20 7468 6520 7368 6172 6520  et to the share 
+000028a0: 6772 616e 746f 722e 0a54 6170 6973 2077  grantor..Tapis w
+000028b0: 696c 6c20 696e 636c 7564 6520 7468 6520  ill include the 
+000028c0: 7368 6172 6520 6772 616e 746f 7220 6173  share grantor as
+000028d0: 2070 6172 7420 6f66 2061 7574 686f 7269   part of authori
+000028e0: 7a61 7469 6f6e 2063 6865 636b 732e 0a94  zation checks...
+000028f0: 8c0b 6f70 6572 6174 696f 6e49 6494 8c05  ..operationId...
+00002900: 6d6b 6469 7294 8c0a 7061 7261 6d65 7465  mkdir...paramete
+00002910: 7273 945d 9428 7d94 288c 046e 616d 6594  rs.].(}.(..name.
+00002920: 8c08 7379 7374 656d 4964 948c 0269 6e94  ..systemId...in.
+00002930: 8c04 7061 7468 948c 0b64 6573 6372 6970  ..path...descrip
+00002940: 7469 6f6e 948c 0953 7973 7465 6d20 4944  tion...System ID
+00002950: 948c 0872 6571 7569 7265 6494 888c 0673  ...required....s
+00002960: 6368 656d 6194 7d94 8c04 7479 7065 948c  chema.}...type..
+00002970: 0673 7472 696e 6794 7375 7d94 288c 046e  .string.su}.(..n
+00002980: 616d 6594 8c09 7368 6172 6564 4374 7894  ame...sharedCtx.
+00002990: 8c02 696e 948c 0571 7565 7279 948c 0b64  ..in...query...d
+000029a0: 6573 6372 6970 7469 6f6e 948c 7952 6573  escription..yRes
+000029b0: 7472 6963 7465 642e 204f 6e6c 7920 6365  tricted. Only ce
+000029c0: 7274 6169 6e20 7365 7276 6963 6573 206d  rtain services m
+000029d0: 6179 2069 6e64 6963 6174 6520 7468 6174  ay indicate that
+000029e0: 2074 6865 2072 6571 7565 7374 2069 7320   the request is 
+000029f0: 696e 2061 2073 6861 7265 6420 636f 6e74  in a shared cont
+00002a00: 6578 742e 204d 7573 7420 6265 2073 6574  ext. Must be set
+00002a10: 2074 6f20 7468 6520 7368 6172 6520 6772   to the share gr
+00002a20: 616e 746f 722e 948c 0673 6368 656d 6194  antor....schema.
+00002a30: 7d94 8c04 2472 6566 948c 2323 2f63 6f6d  }...$ref..##/com
+00002a40: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+00002a50: 5573 6572 4e61 6d65 5374 7269 6e67 9473  UserNameString.s
+00002a60: 7565 8c0b 7265 7175 6573 7442 6f64 7994  ue..requestBody.
+00002a70: 7d94 8c07 636f 6e74 656e 7494 7d94 8c10  }...content.}...
+00002a80: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+00002a90: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
+00002aa0: 2472 6566 948c 2123 2f63 6f6d 706f 6e65  $ref..!#/compone
+00002ab0: 6e74 732f 7363 6865 6d61 732f 4d6b 6469  nts/schemas/Mkdi
+00002ac0: 7252 6571 7565 7374 9473 7373 738c 0972  rRequest.ssss..r
+00002ad0: 6573 706f 6e73 6573 947d 9428 8c03 3230  esponses.}.(..20
+00002ae0: 3094 7d94 288c 0b64 6573 6372 6970 7469  0.}.(..descripti
+00002af0: 6f6e 948c 024f 4b94 8c07 636f 6e74 656e  on...OK...conten
+00002b00: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
+00002b10: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
+00002b20: 6194 7d94 8c04 2472 6566 948c 2723 2f63  a.}...$ref..'#/c
+00002b30: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+00002b40: 732f 4669 6c65 5374 7269 6e67 5265 7370  s/FileStringResp
+00002b50: 6f6e 7365 9473 7373 758c 0334 3030 947d  onse.sssu..400.}
+00002b60: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
+00002b70: 8c0b 4261 6420 5265 7175 6573 7494 8c07  ..Bad Request...
+00002b80: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
+00002b90: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
+00002ba0: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
+00002bb0: 948c 2723 2f63 6f6d 706f 6e65 6e74 732f  ..'#/components/
+00002bc0: 7363 6865 6d61 732f 4669 6c65 5374 7269  schemas/FileStri
+00002bd0: 6e67 5265 7370 6f6e 7365 9473 7373 758c  ngResponse.sssu.
+00002be0: 0334 3031 947d 9428 8c0b 6465 7363 7269  .401.}.(..descri
+00002bf0: 7074 696f 6e94 8c11 4e6f 7420 4175 7468  ption...Not Auth
+00002c00: 656e 7469 6361 7465 6494 8c07 636f 6e74  enticated...cont
+00002c10: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
+00002c20: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
+00002c30: 656d 6194 7d94 8c04 2472 6566 948c 2723  ema.}...$ref..'#
+00002c40: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+00002c50: 6d61 732f 4669 6c65 5374 7269 6e67 5265  mas/FileStringRe
+00002c60: 7370 6f6e 7365 9473 7373 758c 0334 3033  sponse.sssu..403
+00002c70: 947d 9428 8c0b 6465 7363 7269 7074 696f  .}.(..descriptio
+00002c80: 6e94 8c11 5065 726d 6973 7369 6f6e 2044  n...Permission D
+00002c90: 656e 6965 6494 8c07 636f 6e74 656e 7494  enied...content.
+00002ca0: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
+00002cb0: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
+00002cc0: 7d94 8c04 2472 6566 948c 2723 2f63 6f6d  }...$ref..'#/com
+00002cd0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+00002ce0: 4669 6c65 5374 7269 6e67 5265 7370 6f6e  FileStringRespon
+00002cf0: 7365 9473 7373 758c 0335 3030 947d 9428  se.sssu..500.}.(
+00002d00: 8c0b 6465 7363 7269 7074 696f 6e94 8c0e  ..description...
+00002d10: 496e 7465 726e 616c 2045 7272 6f72 948c  Internal Error..
+00002d20: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
+00002d30: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
+00002d40: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
+00002d50: 6694 8c27 232f 636f 6d70 6f6e 656e 7473  f..'#/components
+00002d60: 2f73 6368 656d 6173 2f46 696c 6553 7472  /schemas/FileStr
+00002d70: 696e 6752 6573 706f 6e73 6594 7373 7375  ingResponse.sssu
+00002d80: 7575 738c 272f 7633 2f66 696c 6573 2f75  uus.'/v3/files/u
+00002d90: 7469 6c73 2f6c 696e 7578 2f7b 7379 7374  tils/linux/{syst
+00002da0: 656d 4964 7d2f 7b70 6174 687d 947d 9428  emId}/{path}.}.(
+00002db0: 8c03 6765 7494 7d94 288c 0474 6167 7394  ..get.}.(..tags.
+00002dc0: 5d94 8c0f 4669 6c65 204f 7065 7261 7469  ]...File Operati
+00002dd0: 6f6e 7394 618c 0b64 6573 6372 6970 7469  ons.a..descripti
+00002de0: 6f6e 948c 5047 6574 206e 6174 6976 6520  on..PGet native 
+00002df0: 7374 6174 2069 6e66 6f72 6d61 7469 6f6e  stat information
+00002e00: 2066 6f72 2061 2066 696c 6520 6f72 2064   for a file or d
+00002e10: 6972 6563 746f 7279 2066 6f72 2061 2073  irectory for a s
+00002e20: 7973 7465 6d20 6f66 2074 7970 6520 4c49  ystem of type LI
+00002e30: 4e55 582e 0a94 8c0b 6f70 6572 6174 696f  NUX.....operatio
+00002e40: 6e49 6494 8c0b 6765 7453 7461 7449 6e66  nId...getStatInf
+00002e50: 6f94 8c0a 7061 7261 6d65 7465 7273 945d  o...parameters.]
+00002e60: 9428 7d94 288c 046e 616d 6594 8c08 7379  .(}.(..name...sy
+00002e70: 7374 656d 4964 948c 0269 6e94 8c04 7061  stemId...in...pa
+00002e80: 7468 948c 0b64 6573 6372 6970 7469 6f6e  th...description
+00002e90: 948c 0953 7973 7465 6d20 4944 948c 0872  ...System ID...r
+00002ea0: 6571 7569 7265 6494 888c 0673 6368 656d  equired....schem
+00002eb0: 6194 7d94 8c04 7479 7065 948c 0673 7472  a.}...type...str
+00002ec0: 696e 6794 738c 0765 7861 6d70 6c65 948c  ing.s..example..
+00002ed0: 0973 7973 7465 6d31 3233 9475 7d94 288c  .system123.u}.(.
+00002ee0: 046e 616d 6594 8c04 7061 7468 948c 0269  .name...path...i
+00002ef0: 6e94 8c04 7061 7468 948c 0b64 6573 6372  n...path...descr
+00002f00: 6970 7469 6f6e 948c 2550 6174 6820 7265  iption..%Path re
+00002f10: 6c61 7469 7665 2074 6f20 7468 6520 7379  lative to the sy
+00002f20: 7374 656d 202a 726f 6f74 4469 722a 948c  stem *rootDir*..
+00002f30: 0872 6571 7569 7265 6494 888c 0673 6368  .required....sch
+00002f40: 656d 6194 7d94 8c04 7479 7065 948c 0673  ema.}...type...s
+00002f50: 7472 696e 6794 738c 0765 7861 6d70 6c65  tring.s..example
+00002f60: 948c 1064 6972 6563 746f 7279 412f 6669  ...directoryA/fi
+00002f70: 6c65 3194 757d 9428 8c04 6e61 6d65 948c  le1.u}.(..name..
+00002f80: 0b66 6f6c 6c6f 774c 696e 6b73 948c 0269  .followLinks...i
+00002f90: 6e94 8c05 7175 6572 7994 8c0b 6465 7363  n...query...desc
+00002fa0: 7269 7074 696f 6e94 8c68 5768 656e 2070  ription..hWhen p
+00002fb0: 6174 6820 6973 2061 2073 796d 626f 6c69  ath is a symboli
+00002fc0: 6320 6c69 6e6b 2077 6865 7468 6572 2074  c link whether t
+00002fd0: 6f20 6765 7420 696e 666f 726d 6174 696f  o get informatio
+00002fe0: 6e20 6162 6f75 7420 7468 6520 6c69 6e6b  n about the link
+00002ff0: 2028 6661 6c73 6529 206f 7220 7468 6520   (false) or the 
+00003000: 6c69 6e6b 2074 6172 6765 7420 2874 7275  link target (tru
+00003010: 6529 948c 0673 6368 656d 6194 7d94 288c  e)...schema.}.(.
+00003020: 0474 7970 6594 8c07 626f 6f6c 6561 6e94  .type...boolean.
+00003030: 8c07 6465 6661 756c 7494 8975 8c07 6578  ..default..u..ex
+00003040: 616d 706c 6594 8875 658c 0972 6573 706f  ample..ue..respo
+00003050: 6e73 6573 947d 9428 8c03 3230 3094 7d94  nses.}.(..200.}.
+00003060: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
+00003070: 314c 696e 7578 2073 7461 7420 696e 666f  1Linux stat info
+00003080: 726d 6174 696f 6e20 666f 7220 7468 6520  rmation for the 
+00003090: 6669 6c65 206f 7220 6469 7265 6374 6f72  file or director
+000030a0: 792e 948c 0763 6f6e 7465 6e74 947d 948c  y....content.}..
+000030b0: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
+000030c0: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
+000030d0: 0424 7265 6694 8c29 232f 636f 6d70 6f6e  .$ref..)#/compon
+000030e0: 656e 7473 2f73 6368 656d 6173 2f46 696c  ents/schemas/Fil
+000030f0: 6553 7461 7449 6e66 6f52 6573 706f 6e73  eStatInfoRespons
+00003100: 6594 7373 7375 8c03 3430 3094 7d94 288c  e.sssu..400.}.(.
+00003110: 0b64 6573 6372 6970 7469 6f6e 948c 0b42  .description...B
+00003120: 6164 2052 6571 7565 7374 948c 0763 6f6e  ad Request...con
+00003130: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
+00003140: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
+00003150: 6865 6d61 947d 948c 0424 7265 6694 8c27  hema.}...$ref..'
+00003160: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+00003170: 656d 6173 2f46 696c 6553 7472 696e 6752  emas/FileStringR
+00003180: 6573 706f 6e73 6594 7373 7375 8c03 3430  esponse.sssu..40
+00003190: 3194 7d94 288c 0b64 6573 6372 6970 7469  1.}.(..descripti
+000031a0: 6f6e 948c 114e 6f74 2041 7574 6865 6e74  on...Not Authent
+000031b0: 6963 6174 6564 948c 0763 6f6e 7465 6e74  icated...content
+000031c0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
+000031d0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
+000031e0: 947d 948c 0424 7265 6694 8c27 232f 636f  .}...$ref..'#/co
+000031f0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00003200: 2f46 696c 6553 7472 696e 6752 6573 706f  /FileStringRespo
+00003210: 6e73 6594 7373 7375 8c03 3430 3394 7d94  nse.sssu..403.}.
+00003220: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
+00003230: 1150 6572 6d69 7373 696f 6e20 4465 6e69  .Permission Deni
+00003240: 6564 948c 0763 6f6e 7465 6e74 947d 948c  ed...content.}..
+00003250: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
+00003260: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
+00003270: 0424 7265 6694 8c27 232f 636f 6d70 6f6e  .$ref..'#/compon
+00003280: 656e 7473 2f73 6368 656d 6173 2f46 696c  ents/schemas/Fil
+00003290: 6553 7472 696e 6752 6573 706f 6e73 6594  eStringResponse.
+000032a0: 7373 7375 8c03 3430 3494 7d94 288c 0b64  sssu..404.}.(..d
+000032b0: 6573 6372 6970 7469 6f6e 948c 094e 6f74  escription...Not
+000032c0: 2046 6f75 6e64 948c 0763 6f6e 7465 6e74   Found...content
+000032d0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
+000032e0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
+000032f0: 947d 948c 0424 7265 6694 8c27 232f 636f  .}...$ref..'#/co
+00003300: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00003310: 2f46 696c 6553 7472 696e 6752 6573 706f  /FileStringRespo
+00003320: 6e73 6594 7373 7375 8c03 3530 3094 7d94  nse.sssu..500.}.
+00003330: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
+00003340: 0e49 6e74 6572 6e61 6c20 4572 726f 7294  .Internal Error.
+00003350: 8c07 636f 6e74 656e 7494 7d94 8c10 6170  ..content.}...ap
+00003360: 706c 6963 6174 696f 6e2f 6a73 6f6e 947d  plication/json.}
+00003370: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
+00003380: 6566 948c 2723 2f63 6f6d 706f 6e65 6e74  ef..'#/component
+00003390: 732f 7363 6865 6d61 732f 4669 6c65 5374  s/schemas/FileSt
+000033a0: 7269 6e67 5265 7370 6f6e 7365 9473 7373  ringResponse.sss
+000033b0: 7575 758c 0470 6f73 7494 7d94 288c 0474  uuu..post.}.(..t
+000033c0: 6167 7394 5d94 8c0f 4669 6c65 204f 7065  ags.]...File Ope
+000033d0: 7261 7469 6f6e 7394 618c 0b64 6573 6372  rations.a..descr
+000033e0: 6970 7469 6f6e 948c 6452 756e 2061 206e  iption..dRun a n
+000033f0: 6174 6976 6520 6f70 6572 6174 696f 6e20  ative operation 
+00003400: 6f6e 2061 2070 6174 682e 204f 7065 7261  on a path. Opera
+00003410: 7469 6f6e 7320 6172 6520 6368 6d6f 642c  tions are chmod,
+00003420: 2063 686f 776e 206f 7220 6368 6772 702e   chown or chgrp.
+00003430: 2046 6f72 2061 2073 7973 7465 6d20 6f66   For a system of
+00003440: 2074 7970 6520 4c49 4e55 582e 0a94 8c0b   type LINUX.....
+00003450: 6f70 6572 6174 696f 6e49 6494 8c10 7275  operationId...ru
+00003460: 6e4c 696e 7578 4e61 7469 7665 4f70 948c  nLinuxNativeOp..
+00003470: 0a70 6172 616d 6574 6572 7394 5d94 287d  .parameters.].(}
+00003480: 9428 8c04 6e61 6d65 948c 0873 7973 7465  .(..name...syste
+00003490: 6d49 6494 8c02 696e 948c 0470 6174 6894  mId...in...path.
+000034a0: 8c0b 6465 7363 7269 7074 696f 6e94 8c09  ..description...
+000034b0: 5379 7374 656d 2049 4494 8c08 7265 7175  System ID...requ
+000034c0: 6972 6564 9488 8c06 7363 6865 6d61 947d  ired....schema.}
+000034d0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+000034e0: 9473 757d 9428 8c04 6e61 6d65 948c 0470  .su}.(..name...p
+000034f0: 6174 6894 8c02 696e 948c 0470 6174 6894  ath...in...path.
+00003500: 8c0b 6465 7363 7269 7074 696f 6e94 8c25  ..description..%
+00003510: 5061 7468 2072 656c 6174 6976 6520 746f  Path relative to
+00003520: 2074 6865 2073 7973 7465 6d20 2a72 6f6f   the system *roo
+00003530: 7444 6972 2a94 8c08 7265 7175 6972 6564  tDir*...required
+00003540: 9488 8c06 7363 6865 6d61 947d 948c 0474  ....schema.}...t
+00003550: 7970 6594 8c06 7374 7269 6e67 9473 757d  ype...string.su}
+00003560: 9428 8c04 6e61 6d65 948c 0972 6563 7572  .(..name...recur
+00003570: 7369 7665 948c 0269 6e94 8c05 7175 6572  sive...in...quer
+00003580: 7994 8c0b 6465 7363 7269 7074 696f 6e94  y...description.
+00003590: 8c55 4966 2070 6174 6820 6973 2061 2064  .UIf path is a d
+000035a0: 6972 6563 746f 7279 2074 6869 7320 696e  irectory this in
+000035b0: 6469 6361 7465 7320 7768 6574 6865 7220  dicates whether 
+000035c0: 6f72 206e 6f74 2074 6f20 6170 706c 7920  or not to apply 
+000035d0: 7468 6520 6368 616e 6765 7320 7265 6375  the changes recu
+000035e0: 7273 6976 656c 7994 8c06 7363 6865 6d61  rsively...schema
+000035f0: 947d 9428 8c04 7479 7065 948c 0762 6f6f  .}.(..type...boo
+00003600: 6c65 616e 948c 0764 6566 6175 6c74 9489  lean...default..
+00003610: 758c 0765 7861 6d70 6c65 9488 7565 8c0b  u..example..ue..
+00003620: 7265 7175 6573 7442 6f64 7994 7d94 8c07  requestBody.}...
+00003630: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
+00003640: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
+00003650: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
+00003660: 948c 2923 2f63 6f6d 706f 6e65 6e74 732f  ..)#/components/
+00003670: 7363 6865 6d61 732f 4e61 7469 7665 4c69  schemas/NativeLi
+00003680: 6e75 784f 7052 6571 7565 7374 9473 7373  nuxOpRequest.sss
+00003690: 738c 0972 6573 706f 6e73 6573 947d 9428  s..responses.}.(
+000036a0: 8c03 3230 3094 7d94 288c 0b64 6573 6372  ..200.}.(..descr
+000036b0: 6970 7469 6f6e 948c 024f 4b94 8c07 636f  iption...OK...co
+000036c0: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
+000036d0: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
+000036e0: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
+000036f0: 3023 2f63 6f6d 706f 6e65 6e74 732f 7363  0#/components/sc
+00003700: 6865 6d61 732f 4e61 7469 7665 4c69 6e75  hemas/NativeLinu
+00003710: 784f 7052 6573 756c 7452 6573 706f 6e73  xOpResultRespons
+00003720: 6594 7373 7375 8c03 3430 3094 7d94 288c  e.sssu..400.}.(.
+00003730: 0b64 6573 6372 6970 7469 6f6e 948c 0b42  .description...B
+00003740: 6164 2052 6571 7565 7374 948c 0763 6f6e  ad Request...con
+00003750: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
+00003760: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
+00003770: 6865 6d61 947d 948c 0424 7265 6694 8c27  hema.}...$ref..'
+00003780: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+00003790: 656d 6173 2f46 696c 6553 7472 696e 6752  emas/FileStringR
+000037a0: 6573 706f 6e73 6594 7373 7375 8c03 3430  esponse.sssu..40
+000037b0: 3194 7d94 288c 0b64 6573 6372 6970 7469  1.}.(..descripti
+000037c0: 6f6e 948c 114e 6f74 2041 7574 6865 6e74  on...Not Authent
+000037d0: 6963 6174 6564 948c 0763 6f6e 7465 6e74  icated...content
+000037e0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
+000037f0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
+00003800: 947d 948c 0424 7265 6694 8c27 232f 636f  .}...$ref..'#/co
+00003810: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00003820: 2f46 696c 6553 7472 696e 6752 6573 706f  /FileStringRespo
+00003830: 6e73 6594 7373 7375 8c03 3430 3394 7d94  nse.sssu..403.}.
+00003840: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
+00003850: 1150 6572 6d69 7373 696f 6e20 4465 6e69  .Permission Deni
+00003860: 6564 948c 0763 6f6e 7465 6e74 947d 948c  ed...content.}..
+00003870: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
+00003880: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
+00003890: 0424 7265 6694 8c27 232f 636f 6d70 6f6e  .$ref..'#/compon
+000038a0: 656e 7473 2f73 6368 656d 6173 2f46 696c  ents/schemas/Fil
+000038b0: 6553 7472 696e 6752 6573 706f 6e73 6594  eStringResponse.
+000038c0: 7373 7375 8c03 3430 3494 7d94 288c 0b64  sssu..404.}.(..d
+000038d0: 6573 6372 6970 7469 6f6e 948c 094e 6f74  escription...Not
+000038e0: 2046 6f75 6e64 948c 0763 6f6e 7465 6e74   Found...content
+000038f0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
+00003900: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
+00003910: 947d 948c 0424 7265 6694 8c27 232f 636f  .}...$ref..'#/co
+00003920: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00003930: 2f46 696c 6553 7472 696e 6752 6573 706f  /FileStringRespo
+00003940: 6e73 6594 7373 7375 8c03 3530 3094 7d94  nse.sssu..500.}.
+00003950: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
+00003960: 0e49 6e74 6572 6e61 6c20 4572 726f 7294  .Internal Error.
+00003970: 8c07 636f 6e74 656e 7494 7d94 8c10 6170  ..content.}...ap
+00003980: 706c 6963 6174 696f 6e2f 6a73 6f6e 947d  plication/json.}
+00003990: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
+000039a0: 6566 948c 2723 2f63 6f6d 706f 6e65 6e74  ef..'#/component
+000039b0: 732f 7363 6865 6d61 732f 4669 6c65 5374  s/schemas/FileSt
+000039c0: 7269 6e67 5265 7370 6f6e 7365 9473 7373  ringResponse.sss
+000039d0: 7575 7575 8c2c 2f76 332f 6669 6c65 732f  uuuu.,/v3/files/
+000039e0: 7574 696c 732f 6c69 6e75 782f 6661 636c  utils/linux/facl
+000039f0: 2f7b 7379 7374 656d 4964 7d2f 7b70 6174  /{systemId}/{pat
+00003a00: 687d 947d 9428 8c03 6765 7494 7d94 288c  h}.}.(..get.}.(.
+00003a10: 0474 6167 7394 5d94 8c0f 4669 6c65 204f  .tags.]...File O
+00003a20: 7065 7261 7469 6f6e 7394 618c 0b64 6573  perations.a..des
+00003a30: 6372 6970 7469 6f6e 948c 2847 6574 2066  cription..(Get f
+00003a40: 696c 6520 4143 4c73 2066 6f72 2066 696c  ile ACLs for fil
+00003a50: 6573 206f 7220 6469 7265 6374 6f72 6965  es or directorie
+00003a60: 732e 0a94 8c0b 6f70 6572 6174 696f 6e49  s.....operationI
+00003a70: 6494 8c07 6765 7446 6163 6c94 8c0a 7061  d...getFacl...pa
+00003a80: 7261 6d65 7465 7273 945d 9428 7d94 288c  rameters.].(}.(.
+00003a90: 046e 616d 6594 8c08 7379 7374 656d 4964  .name...systemId
+00003aa0: 948c 0269 6e94 8c04 7061 7468 948c 0b64  ...in...path...d
+00003ab0: 6573 6372 6970 7469 6f6e 948c 0953 7973  escription...Sys
+00003ac0: 7465 6d20 4944 948c 0872 6571 7569 7265  tem ID...require
+00003ad0: 6494 888c 0673 6368 656d 6194 7d94 8c04  d....schema.}...
+00003ae0: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
+00003af0: 0765 7861 6d70 6c65 948c 0973 7973 7465  .example...syste
+00003b00: 6d31 3233 9475 7d94 288c 046e 616d 6594  m123.u}.(..name.
+00003b10: 8c04 7061 7468 948c 0269 6e94 8c04 7061  ..path...in...pa
+00003b20: 7468 948c 0b64 6573 6372 6970 7469 6f6e  th...description
+00003b30: 948c 2550 6174 6820 7265 6c61 7469 7665  ..%Path relative
+00003b40: 2074 6f20 7468 6520 7379 7374 656d 202a   to the system *
+00003b50: 726f 6f74 4469 722a 948c 0872 6571 7569  rootDir*...requi
+00003b60: 7265 6494 888c 0673 6368 656d 6194 7d94  red....schema.}.
+00003b70: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+00003b80: 738c 0765 7861 6d70 6c65 948c 172f 6469  s..example.../di
+00003b90: 7265 6374 6f72 7941 2f64 6972 6563 746f  rectoryA/directo
+00003ba0: 7279 422f 9475 658c 0972 6573 706f 6e73  ryB/.ue..respons
+00003bb0: 6573 947d 9428 8c03 3230 3094 7d94 288c  es.}.(..200.}.(.
+00003bc0: 0b64 6573 6372 6970 7469 6f6e 948c 024f  .description...O
+00003bd0: 4b94 8c07 636f 6e74 656e 7494 7d94 8c10  K...content.}...
+00003be0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+00003bf0: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
+00003c00: 2472 6566 948c 2f23 2f63 6f6d 706f 6e65  $ref../#/compone
+00003c10: 6e74 732f 7363 6865 6d61 732f 4e61 7469  nts/schemas/Nati
+00003c20: 7665 4c69 6e75 7847 6574 4661 636c 5265  veLinuxGetFaclRe
+00003c30: 7370 6f6e 7365 9473 7373 758c 0334 3031  sponse.sssu..401
+00003c40: 947d 9428 8c0b 6465 7363 7269 7074 696f  .}.(..descriptio
+00003c50: 6e94 8c11 4e6f 7420 4175 7468 656e 7469  n...Not Authenti
+00003c60: 6361 7465 6494 8c07 636f 6e74 656e 7494  cated...content.
+00003c70: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
+00003c80: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
+00003c90: 7d94 8c04 2472 6566 948c 2723 2f63 6f6d  }...$ref..'#/com
+00003ca0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+00003cb0: 4669 6c65 5374 7269 6e67 5265 7370 6f6e  FileStringRespon
+00003cc0: 7365 9473 7373 758c 0334 3033 947d 9428  se.sssu..403.}.(
+00003cd0: 8c0b 6465 7363 7269 7074 696f 6e94 8c11  ..description...
+00003ce0: 5065 726d 6973 7369 6f6e 2044 656e 6965  Permission Denie
+00003cf0: 6494 8c07 636f 6e74 656e 7494 7d94 8c10  d...content.}...
+00003d00: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+00003d10: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
+00003d20: 2472 6566 948c 2723 2f63 6f6d 706f 6e65  $ref..'#/compone
+00003d30: 6e74 732f 7363 6865 6d61 732f 4669 6c65  nts/schemas/File
+00003d40: 5374 7269 6e67 5265 7370 6f6e 7365 9473  StringResponse.s
+00003d50: 7373 758c 0334 3034 947d 9428 8c0b 6465  ssu..404.}.(..de
+00003d60: 7363 7269 7074 696f 6e94 8c09 4e6f 7420  scription...Not 
+00003d70: 466f 756e 6494 8c07 636f 6e74 656e 7494  Found...content.
+00003d80: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
+00003d90: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
+00003da0: 7d94 8c04 2472 6566 948c 2723 2f63 6f6d  }...$ref..'#/com
+00003db0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+00003dc0: 4669 6c65 5374 7269 6e67 5265 7370 6f6e  FileStringRespon
+00003dd0: 7365 9473 7373 758c 0335 3030 947d 9428  se.sssu..500.}.(
+00003de0: 8c0b 6465 7363 7269 7074 696f 6e94 8c0e  ..description...
+00003df0: 496e 7465 726e 616c 2045 7272 6f72 948c  Internal Error..
+00003e00: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
+00003e10: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
+00003e20: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
+00003e30: 6694 8c27 232f 636f 6d70 6f6e 656e 7473  f..'#/components
+00003e40: 2f73 6368 656d 6173 2f46 696c 6553 7472  /schemas/FileStr
+00003e50: 696e 6752 6573 706f 6e73 6594 7373 7375  ingResponse.sssu
+00003e60: 7575 8c04 706f 7374 947d 9428 8c04 7461  uu..post.}.(..ta
+00003e70: 6773 945d 948c 0f46 696c 6520 4f70 6572  gs.]...File Oper
+00003e80: 6174 696f 6e73 9461 8c0b 6465 7363 7269  ations.a..descri
+00003e90: 7074 696f 6e94 5829 0100 0053 6574 2066  ption.X)...Set f
+00003ea0: 696c 6520 4143 4c73 2066 6f72 2066 696c  ile ACLs for fil
+00003eb0: 6573 206f 7220 6469 7265 6374 6f72 6965  es or directorie
+00003ec0: 732e 0a0a 5468 6973 2063 616e 2062 6520  s...This can be 
+00003ed0: 7573 6564 2066 6f72 2061 2073 696e 676c  used for a singl
+00003ee0: 6520 6669 6c65 206f 7220 6469 7265 6374  e file or direct
+00003ef0: 6f72 792c 206f 7220 6361 6e20 6265 2072  ory, or can be r
+00003f00: 6563 7572 7369 7665 2e20 2049 6620 7265  ecursive.  If re
+00003f10: 6375 7273 696f 6e20 6973 0a75 7365 642c  cursion is.used,
+00003f20: 2069 7420 6361 6e20 6265 206d 6164 6520   it can be made 
+00003f30: 746f 2066 6f6c 6c6f 7720 7379 6d6c 696e  to follow symlin
+00003f40: 6b73 2c20 6f72 206e 6f74 2066 6f6c 6c6f  ks, or not follo
+00003f50: 7720 7379 6d6c 696e 6b73 2e0a 0a54 6865  w symlinks...The
+00003f60: 206f 7065 7261 7469 6f6e 7320 7375 7070   operations supp
+00003f70: 6f72 7420 6164 6469 6e67 206f 7220 7265  ort adding or re
+00003f80: 6d6f 7669 6e67 2041 636c 2045 6e74 7269  moving Acl Entri
+00003f90: 6573 2061 7320 7765 6c6c 2061 7320 7265  es as well as re
+00003fa0: 6d6f 7669 6e67 2061 6c6c 2061 636c 7320  moving all acls 
+00003fb0: 6f72 2061 6c6c 0a64 6566 6175 6c74 2061  or all.default a
+00003fc0: 636c 730a 948c 0b6f 7065 7261 7469 6f6e  cls....operation
+00003fd0: 4964 948c 0773 6574 4661 636c 948c 0a70  Id...setFacl...p
+00003fe0: 6172 616d 6574 6572 7394 5d94 287d 9428  arameters.].(}.(
+00003ff0: 8c04 6e61 6d65 948c 0873 7973 7465 6d49  ..name...systemI
+00004000: 6494 8c02 696e 948c 0470 6174 6894 8c08  d...in...path...
+00004010: 7265 7175 6972 6564 9488 8c0b 6465 7363  required....desc
+00004020: 7269 7074 696f 6e94 8c09 5379 7374 656d  ription...System
+00004030: 2049 4494 8c06 7363 6865 6d61 947d 948c   ID...schema.}..
+00004040: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+00004050: 8c07 6578 616d 706c 6594 8c09 7379 7374  ..example...syst
+00004060: 656d 3132 3394 757d 9428 8c04 6e61 6d65  em123.u}.(..name
+00004070: 948c 0470 6174 6894 8c02 696e 948c 0470  ...path...in...p
+00004080: 6174 6894 8c0b 6465 7363 7269 7074 696f  ath...descriptio
+00004090: 6e94 8c25 5061 7468 2072 656c 6174 6976  n..%Path relativ
+000040a0: 6520 746f 2074 6865 2073 7973 7465 6d20  e to the system 
+000040b0: 2a72 6f6f 7444 6972 2a94 8c08 7265 7175  *rootDir*...requ
+000040c0: 6972 6564 9488 8c06 7363 6865 6d61 947d  ired....schema.}
+000040d0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+000040e0: 9473 8c07 6578 616d 706c 6594 8c17 2f64  .s..example.../d
+000040f0: 6972 6563 746f 7279 412f 6469 7265 6374  irectoryA/direct
+00004100: 6f72 7942 2f94 7565 8c0b 7265 7175 6573  oryB/.ue..reques
+00004110: 7442 6f64 7994 7d94 288c 0872 6571 7569  tBody.}.(..requi
+00004120: 7265 6494 888c 0b64 6573 6372 6970 7469  red....descripti
+00004130: 6f6e 948c 3541 204a 534f 4e20 6f62 6a65  on..5A JSON obje
+00004140: 6374 2073 7065 6369 6679 696e 6720 7570  ct specifying up
+00004150: 6461 7465 6420 7368 6172 696e 6720 696e  dated sharing in
+00004160: 666f 726d 6174 696f 6e2e 948c 0763 6f6e  formation....con
+00004170: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
+00004180: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
+00004190: 6865 6d61 947d 948c 0424 7265 6694 8c2e  hema.}...$ref...
+000041a0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+000041b0: 656d 6173 2f4e 6174 6976 654c 696e 7578  emas/NativeLinux
+000041c0: 5365 7446 6163 6c52 6571 7565 7374 9473  SetFaclRequest.s
+000041d0: 7373 758c 0972 6573 706f 6e73 6573 947d  ssu..responses.}
+000041e0: 9428 8c03 3230 3094 7d94 288c 0b64 6573  .(..200.}.(..des
+000041f0: 6372 6970 7469 6f6e 948c 024f 4b94 8c07  cription...OK...
+00004200: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
+00004210: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
+00004220: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
+00004230: 948c 2f23 2f63 6f6d 706f 6e65 6e74 732f  ../#/components/
+00004240: 7363 6865 6d61 732f 4e61 7469 7665 4c69  schemas/NativeLi
+00004250: 6e75 7853 6574 4661 636c 5265 7370 6f6e  nuxSetFaclRespon
+00004260: 7365 9473 7373 758c 0334 3030 947d 9428  se.sssu..400.}.(
+00004270: 8c0b 6465 7363 7269 7074 696f 6e94 8c0b  ..description...
+00004280: 4261 6420 5265 7175 6573 7494 8c07 636f  Bad Request...co
+00004290: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
+000042a0: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
+000042b0: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
+000042c0: 2723 2f63 6f6d 706f 6e65 6e74 732f 7363  '#/components/sc
+000042d0: 6865 6d61 732f 4669 6c65 5374 7269 6e67  hemas/FileString
+000042e0: 5265 7370 6f6e 7365 9473 7373 758c 0334  Response.sssu..4
+000042f0: 3031 947d 9428 8c0b 6465 7363 7269 7074  01.}.(..descript
+00004300: 696f 6e94 8c11 4e6f 7420 4175 7468 656e  ion...Not Authen
+00004310: 7469 6361 7465 6494 8c07 636f 6e74 656e  ticated...conten
+00004320: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
+00004330: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
+00004340: 6194 7d94 8c04 2472 6566 948c 2723 2f63  a.}...$ref..'#/c
+00004350: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+00004360: 732f 4669 6c65 5374 7269 6e67 5265 7370  s/FileStringResp
+00004370: 6f6e 7365 9473 7373 758c 0334 3033 947d  onse.sssu..403.}
+00004380: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
+00004390: 8c11 5065 726d 6973 7369 6f6e 2044 656e  ..Permission Den
+000043a0: 6965 6494 8c07 636f 6e74 656e 7494 7d94  ied...content.}.
+000043b0: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
+000043c0: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
+000043d0: 8c04 2472 6566 948c 2723 2f63 6f6d 706f  ..$ref..'#/compo
+000043e0: 6e65 6e74 732f 7363 6865 6d61 732f 4669  nents/schemas/Fi
+000043f0: 6c65 5374 7269 6e67 5265 7370 6f6e 7365  leStringResponse
+00004400: 9473 7373 758c 0334 3034 947d 9428 8c0b  .sssu..404.}.(..
+00004410: 6465 7363 7269 7074 696f 6e94 8c09 4e6f  description...No
+00004420: 7420 466f 756e 6494 8c07 636f 6e74 656e  t Found...conten
+00004430: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
+00004440: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
+00004450: 6194 7d94 8c04 2472 6566 948c 2723 2f63  a.}...$ref..'#/c
+00004460: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+00004470: 732f 4669 6c65 5374 7269 6e67 5265 7370  s/FileStringResp
+00004480: 6f6e 7365 9473 7373 758c 0335 3030 947d  onse.sssu..500.}
+00004490: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
+000044a0: 8c0e 496e 7465 726e 616c 2045 7272 6f72  ..Internal Error
+000044b0: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
+000044c0: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
+000044d0: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
+000044e0: 7265 6694 8c27 232f 636f 6d70 6f6e 656e  ref..'#/componen
+000044f0: 7473 2f73 6368 656d 6173 2f46 696c 6553  ts/schemas/FileS
+00004500: 7472 696e 6752 6573 706f 6e73 6594 7373  tringResponse.ss
+00004510: 7375 7575 758c 232f 7633 2f66 696c 6573  suuuu.#/v3/files
+00004520: 2f63 6f6e 7465 6e74 2f7b 7379 7374 656d  /content/{system
+00004530: 4964 7d2f 7b70 6174 687d 947d 948c 0367  Id}/{path}.}...g
+00004540: 6574 947d 9428 8c04 7461 6773 945d 948c  et.}.(..tags.]..
+00004550: 0743 6f6e 7465 6e74 9461 8c0b 6465 7363  .Content.a..desc
+00004560: 7269 7074 696f 6e94 58f4 0200 0047 6574  ription.X....Get
+00004570: 2066 696c 6520 6f72 2064 6972 6563 746f   file or directo
+00004580: 7279 2063 6f6e 7465 6e74 7320 6173 2061  ry contents as a
+00004590: 2073 7472 6561 6d20 6f66 2064 6174 612e   stream of data.
+000045a0: 0a0a 4365 7274 6169 6e20 7365 7276 6963  ..Certain servic
+000045b0: 6573 206d 6179 2075 7365 2074 6865 2071  es may use the q
+000045c0: 7565 7279 2070 6172 616d 6574 6572 202a  uery parameter *
+000045d0: 696d 7065 7273 6f6e 6174 696f 6e49 642a  impersonationId*
+000045e0: 2074 6f20 6265 2075 7365 6420 696e 2070   to be used in p
+000045f0: 6c61 6365 206f 6620 7468 6520 7265 7175  lace of the requ
+00004600: 6573 7469 6e67 0a54 6170 6973 2075 7365  esting.Tapis use
+00004610: 722e 2054 6170 6973 2077 696c 6c20 7573  r. Tapis will us
+00004620: 6520 7468 6973 2075 7365 7220 4964 2077  e this user Id w
+00004630: 6865 6e20 7065 7266 6f72 6d69 6e67 2061  hen performing a
+00004640: 7574 686f 7269 7a61 7469 6f6e 2061 6e64  uthorization and
+00004650: 2072 6573 6f6c 7669 6e67 2074 6865 202a   resolving the *
+00004660: 6566 6665 6374 6976 6555 7365 7249 642a  effectiveUserId*
+00004670: 0a66 6f72 2074 6865 2073 7973 7465 6d2e  .for the system.
+00004680: 0a0a 5573 6520 7468 6520 7175 6572 7920  ..Use the query 
+00004690: 7061 7261 6d65 7465 7220 2a7a 6970 2a20  parameter *zip* 
+000046a0: 746f 2072 6571 7565 7374 2061 2073 7472  to request a str
+000046b0: 6561 6d20 636f 6d70 7265 7373 6564 2075  eam compressed u
+000046c0: 7369 6e67 2074 6865 205a 4950 2066 696c  sing the ZIP fil
+000046d0: 6520 666f 726d 6174 2e20 5468 6973 2069  e format. This i
+000046e0: 7320 6e6f 7420 616c 6c6f 7765 640a 6966  s not allowed.if
+000046f0: 2073 7973 7465 6d20 2a72 6f6f 7444 6972   system *rootDir
+00004700: 2a20 706c 7573 202a 7061 7468 2a20 776f  * plus *path* wo
+00004710: 756c 6420 7265 7375 6c74 2069 6e20 616c  uld result in al
+00004720: 6c20 6669 6c65 7320 6f6e 2074 6865 2068  l files on the h
+00004730: 6f73 7420 6265 696e 6720 696e 636c 7564  ost being includ
+00004740: 6564 2e20 506c 6561 7365 2064 6f77 6e6c  ed. Please downl
+00004750: 6f61 640a 696e 6469 7669 6475 616c 2064  oad.individual d
+00004760: 6972 6563 746f 7269 6573 2c20 6669 6c65  irectories, file
+00004770: 7320 6f72 206f 626a 6563 7473 2e0a 0a43  s or objects...C
+00004780: 6572 7461 696e 2073 6572 7669 6365 7320  ertain services 
+00004790: 6d61 7920 7573 6520 7468 6520 7175 6572  may use the quer
+000047a0: 7920 7061 7261 6d65 7465 7220 2a73 6861  y parameter *sha
+000047b0: 7265 6443 7478 2a20 746f 2069 6e64 6963  redCtx* to indic
+000047c0: 6174 6520 7468 6174 2074 6865 2072 6571  ate that the req
+000047d0: 7565 7374 2069 7320 696e 2061 2073 6861  uest is in a sha
+000047e0: 7265 640a 636f 6e74 6578 742e 202a 7368  red.context. *sh
+000047f0: 6172 6564 4374 782a 206d 7573 7420 6265  aredCtx* must be
+00004800: 2073 6574 2074 6f20 7468 6520 7368 6172   set to the shar
+00004810: 6520 6772 616e 746f 722e 0a54 6170 6973  e grantor..Tapis
+00004820: 2077 696c 6c20 696e 636c 7564 6520 7468   will include th
+00004830: 6520 7368 6172 6520 6772 616e 746f 7220  e share grantor 
+00004840: 6173 2070 6172 7420 6f66 2061 7574 686f  as part of autho
+00004850: 7269 7a61 7469 6f6e 2063 6865 636b 732e  rization checks.
+00004860: 0a94 8c0b 6f70 6572 6174 696f 6e49 6494  ....operationId.
+00004870: 8c0b 6765 7443 6f6e 7465 6e74 7394 8c0a  ..getContents...
+00004880: 7061 7261 6d65 7465 7273 945d 9428 7d94  parameters.].(}.
+00004890: 288c 046e 616d 6594 8c08 7379 7374 656d  (..name...system
+000048a0: 4964 948c 0269 6e94 8c04 7061 7468 948c  Id...in...path..
+000048b0: 0b64 6573 6372 6970 7469 6f6e 948c 0953  .description...S
+000048c0: 7973 7465 6d20 4944 948c 0872 6571 7569  ystem ID...requi
+000048d0: 7265 6494 888c 0673 6368 656d 6194 7d94  red....schema.}.
+000048e0: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+000048f0: 738c 0765 7861 6d70 6c65 948c 0973 7973  s..example...sys
+00004900: 7465 6d31 3233 9475 7d94 288c 046e 616d  tem123.u}.(..nam
+00004910: 6594 8c04 7061 7468 948c 0269 6e94 8c04  e...path...in...
+00004920: 7061 7468 948c 0b64 6573 6372 6970 7469  path...descripti
+00004930: 6f6e 948c 2550 6174 6820 7265 6c61 7469  on..%Path relati
+00004940: 7665 2074 6f20 7468 6520 7379 7374 656d  ve to the system
+00004950: 202a 726f 6f74 4469 722a 948c 0872 6571   *rootDir*...req
+00004960: 7569 7265 6494 888c 0673 6368 656d 6194  uired....schema.
+00004970: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+00004980: 6794 738c 0765 7861 6d70 6c65 948c 1664  g.s..example...d
+00004990: 6972 6563 746f 7279 412f 6469 7265 6374  irectoryA/direct
+000049a0: 6f72 7942 2f94 757d 9428 8c04 6e61 6d65  oryB/.u}.(..name
+000049b0: 948c 0572 616e 6765 948c 0269 6e94 8c06  ...range...in...
+000049c0: 6865 6164 6572 948c 0b64 6573 6372 6970  header...descrip
+000049d0: 7469 6f6e 948c 4b4f 7074 696f 6e61 6c20  tion..KOptional 
+000049e0: 7261 6e67 6520 6f66 2062 7974 6573 2074  range of bytes t
+000049f0: 6f20 7365 6e64 2e20 4966 206e 6f74 2073  o send. If not s
+00004a00: 7065 6369 6669 6564 2061 6c6c 2063 6f6e  pecified all con
+00004a10: 7465 6e74 2077 696c 6c20 6265 2073 656e  tent will be sen
+00004a20: 742e 948c 0673 6368 656d 6194 7d94 8c04  t....schema.}...
+00004a30: 2472 6566 948c 2423 2f63 6f6d 706f 6e65  $ref..$#/compone
+00004a40: 6e74 732f 7363 6865 6d61 732f 4865 6164  nts/schemas/Head
+00004a50: 6572 4279 7465 5261 6e67 6594 738c 0765  erByteRange.s..e
+00004a60: 7861 6d70 6c65 948c 0b72 616e 6765 3d30  xample...range=0
+00004a70: 2c39 3939 9475 7d94 288c 046e 616d 6594  ,999.u}.(..name.
+00004a80: 8c03 7a69 7094 8c02 696e 948c 0571 7565  ..zip...in...que
+00004a90: 7279 948c 0b64 6573 6372 6970 7469 6f6e  ry...description
+00004aa0: 948c 3149 6e64 6963 6174 6573 2061 207a  ..1Indicates a z
+00004ab0: 6970 206f 7574 7075 7420 7374 7265 616d  ip output stream
+00004ac0: 2073 686f 756c 6420 6265 2070 726f 7669   should be provi
+00004ad0: 6465 642e 948c 0673 6368 656d 6194 7d94  ded....schema.}.
+00004ae0: 8c04 7479 7065 948c 0762 6f6f 6c65 616e  ..type...boolean
+00004af0: 9473 8c07 6578 616d 706c 6594 8975 7d94  .s..example..u}.
+00004b00: 288c 046e 616d 6594 8c04 6d6f 7265 948c  (..name...more..
+00004b10: 0269 6e94 8c06 6865 6164 6572 948c 0b64  .in...header...d
+00004b20: 6573 6372 6970 7469 6f6e 948c 4653 656e  escription..FSen
+00004b30: 6420 316b 206f 6620 5554 462d 3820 656e  d 1k of UTF-8 en
+00004b40: 636f 6465 6420 7374 7269 6e67 2062 6163  coded string bac
+00004b50: 6b20 7374 6172 7469 6e67 2061 7420 2770  k starting at 'p
+00004b60: 6167 6527 2031 2c20 652e 672e 206d 6f72  age' 1, e.g. mor
+00004b70: 653d 3194 8c06 7363 6865 6d61 947d 9428  e=1...schema.}.(
+00004b80: 8c04 7479 7065 948c 0769 6e74 6567 6572  ..type...integer
+00004b90: 948c 0666 6f72 6d61 7494 8c05 696e 7436  ...format...int6
+00004ba0: 3494 7575 7d94 288c 046e 616d 6594 8c0f  4.uu}.(..name...
+00004bb0: 696d 7065 7273 6f6e 6174 696f 6e49 6494  impersonationId.
+00004bc0: 8c02 696e 948c 0571 7565 7279 948c 0b64  ..in...query...d
+00004bd0: 6573 6372 6970 7469 6f6e 948c 3f52 6573  escription..?Res
+00004be0: 7472 6963 7465 642e 204f 6e6c 7920 6365  tricted. Only ce
+00004bf0: 7274 6169 6e20 7365 7276 6963 6573 206d  rtain services m
+00004c00: 6179 2069 6d70 6572 736f 6e61 7465 2061  ay impersonate a
+00004c10: 2054 6170 6973 2075 7365 722e 948c 0673   Tapis user....s
+00004c20: 6368 656d 6194 7d94 8c04 7479 7065 948c  chema.}...type..
+00004c30: 0673 7472 696e 6794 7375 7d94 288c 046e  .string.su}.(..n
+00004c40: 616d 6594 8c09 7368 6172 6564 4374 7894  ame...sharedCtx.
+00004c50: 8c02 696e 948c 0571 7565 7279 948c 0b64  ..in...query...d
+00004c60: 6573 6372 6970 7469 6f6e 948c 7952 6573  escription..yRes
+00004c70: 7472 6963 7465 642e 204f 6e6c 7920 6365  tricted. Only ce
+00004c80: 7274 6169 6e20 7365 7276 6963 6573 206d  rtain services m
+00004c90: 6179 2069 6e64 6963 6174 6520 7468 6174  ay indicate that
+00004ca0: 2074 6865 2072 6571 7565 7374 2069 7320   the request is 
+00004cb0: 696e 2061 2073 6861 7265 6420 636f 6e74  in a shared cont
+00004cc0: 6578 742e 204d 7573 7420 6265 2073 6574  ext. Must be set
+00004cd0: 2074 6f20 7468 6520 7368 6172 6520 6772   to the share gr
+00004ce0: 616e 746f 722e 948c 0673 6368 656d 6194  antor....schema.
+00004cf0: 7d94 8c04 2472 6566 948c 2323 2f63 6f6d  }...$ref..##/com
+00004d00: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+00004d10: 5573 6572 4e61 6d65 5374 7269 6e67 9473  UserNameString.s
+00004d20: 7565 8c09 7265 7370 6f6e 7365 7394 7d94  ue..responses.}.
+00004d30: 288c 0332 3030 947d 948c 0b64 6573 6372  (..200.}...descr
+00004d40: 6970 7469 6f6e 948c 024f 4b94 738c 0334  iption...OK.s..4
+00004d50: 3030 947d 948c 0b64 6573 6372 6970 7469  00.}...descripti
+00004d60: 6f6e 948c 0b42 6164 2052 6571 7565 7374  on...Bad Request
+00004d70: 9473 8c03 3430 3194 7d94 8c0b 6465 7363  .s..401.}...desc
+00004d80: 7269 7074 696f 6e94 8c11 4e6f 7420 4175  ription...Not Au
+00004d90: 7468 656e 7469 6361 7465 6494 738c 0334  thenticated.s..4
+00004da0: 3034 947d 948c 0b64 6573 6372 6970 7469  04.}...descripti
+00004db0: 6f6e 948c 094e 6f74 2046 6f75 6e64 9473  on...Not Found.s
+00004dc0: 8c03 3430 3394 7d94 8c0b 6465 7363 7269  ..403.}...descri
+00004dd0: 7074 696f 6e94 8c11 5065 726d 6973 7369  ption...Permissi
+00004de0: 6f6e 2044 656e 6965 6494 7375 7573 8c13  on Denied.suus..
+00004df0: 2f76 332f 6669 6c65 732f 7472 616e 7366  /v3/files/transf
+00004e00: 6572 7394 7d94 288c 0367 6574 947d 9428  ers.}.(..get.}.(
+00004e10: 8c04 7461 6773 945d 948c 0954 7261 6e73  ..tags.]...Trans
+00004e20: 6665 7273 9461 8c0b 6465 7363 7269 7074  fers.a..descript
+00004e30: 696f 6e94 8c3c 4765 7420 6120 6c69 7374  ion..<Get a list
+00004e40: 206f 6620 7472 616e 7366 6572 2074 6173   of transfer tas
+00004e50: 6b73 2073 7461 7274 696e 6720 7769 7468  ks starting with
+00004e60: 2074 6865 206d 6f73 7420 7265 6365 6e74   the most recent
+00004e70: 2e0a 948c 0b6f 7065 7261 7469 6f6e 4964  .....operationId
+00004e80: 948c 1667 6574 5265 6365 6e74 5472 616e  ...getRecentTran
+00004e90: 7366 6572 5461 736b 7394 8c0a 7061 7261  sferTasks...para
+00004ea0: 6d65 7465 7273 945d 9428 7d94 288c 046e  meters.].(}.(..n
+00004eb0: 616d 6594 8c05 6c69 6d69 7494 8c02 696e  ame...limit...in
+00004ec0: 948c 0571 7565 7279 948c 0b64 6573 6372  ...query...descr
+00004ed0: 6970 7469 6f6e 948c 1070 6167 696e 6174  iption...paginat
+00004ee0: 696f 6e20 6c69 6d69 7494 8c06 7363 6865  ion limit...sche
+00004ef0: 6d61 947d 9428 8c04 7479 7065 948c 0769  ma.}.(..type...i
+00004f00: 6e74 6567 6572 948c 0666 6f72 6d61 7494  nteger...format.
+00004f10: 8c05 696e 7433 3294 8c07 6465 6661 756c  ..int32...defaul
+00004f20: 7494 4de8 0375 8c07 6578 616d 706c 6594  t.M..u..example.
+00004f30: 4b64 757d 9428 8c04 6e61 6d65 948c 066f  Kdu}.(..name...o
+00004f40: 6666 7365 7494 8c02 696e 948c 0571 7565  ffset...in...que
+00004f50: 7279 948c 0b64 6573 6372 6970 7469 6f6e  ry...description
+00004f60: 948c 1170 6167 696e 6174 696f 6e20 6f66  ...pagination of
+00004f70: 6673 6574 948c 0673 6368 656d 6194 7d94  fset...schema.}.
+00004f80: 288c 0474 7970 6594 8c07 696e 7465 6765  (..type...intege
+00004f90: 7294 8c06 666f 726d 6174 948c 0569 6e74  r...format...int
+00004fa0: 3332 948c 0764 6566 6175 6c74 944b 0075  32...default.K.u
+00004fb0: 8c07 6578 616d 706c 6594 4de8 0375 658c  ..example.M..ue.
+00004fc0: 0972 6573 706f 6e73 6573 947d 948c 0332  .responses.}...2
+00004fd0: 3030 947d 9428 8c0b 6465 7363 7269 7074  00.}.(..descript
+00004fe0: 696f 6e94 8c02 4f4b 948c 0763 6f6e 7465  ion...OK...conte
+00004ff0: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
+00005000: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
+00005010: 6d61 947d 948c 0424 7265 6694 8c2d 232f  ma.}...$ref..-#/
+00005020: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+00005030: 6173 2f54 7261 6e73 6665 7254 6173 6b4c  as/TransferTaskL
+00005040: 6973 7452 6573 706f 6e73 6594 7373 7375  istResponse.sssu
+00005050: 7375 8c04 706f 7374 947d 9428 8c04 7461  su..post.}.(..ta
+00005060: 6773 945d 948c 0954 7261 6e73 6665 7273  gs.]...Transfers
+00005070: 9461 8c0b 6465 7363 7269 7074 696f 6e94  .a..description.
+00005080: 8c44 4372 6561 7465 2061 2062 6163 6b67  .DCreate a backg
+00005090: 726f 756e 6420 7461 736b 2077 6869 6368  round task which
+000050a0: 2077 696c 6c20 7472 616e 7366 6572 2066   will transfer f
+000050b0: 696c 6573 2062 6574 7765 656e 2073 7973  iles between sys
+000050c0: 7465 6d73 2e0a 948c 0b6f 7065 7261 7469  tems.....operati
+000050d0: 6f6e 4964 948c 1263 7265 6174 6554 7261  onId...createTra
+000050e0: 6e73 6665 7254 6173 6b94 8c0b 7265 7175  nsferTask...requ
+000050f0: 6573 7442 6f64 7994 7d94 288c 0763 6f6e  estBody.}.(..con
+00005100: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
+00005110: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
+00005120: 6865 6d61 947d 948c 0424 7265 6694 8c20  hema.}...$ref.. 
+00005130: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+00005140: 656d 6173 2f52 6571 5472 616e 7366 6572  emas/ReqTransfer
+00005150: 9473 7373 8c08 7265 7175 6972 6564 9488  .sss..required..
+00005160: 758c 0972 6573 706f 6e73 6573 947d 948c  u..responses.}..
+00005170: 0332 3030 947d 9428 8c0b 6465 7363 7269  .200.}.(..descri
+00005180: 7074 696f 6e94 8c02 4f4b 948c 0763 6f6e  ption...OK...con
+00005190: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
+000051a0: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
+000051b0: 6865 6d61 947d 948c 0424 7265 6694 8c29  hema.}...$ref..)
+000051c0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+000051d0: 656d 6173 2f54 7261 6e73 6665 7254 6173  emas/TransferTas
+000051e0: 6b52 6573 706f 6e73 6594 7373 7375 7375  kResponse.sssusu
+000051f0: 758c 242f 7633 2f66 696c 6573 2f74 7261  u.$/v3/files/tra
+00005200: 6e73 6665 7273 2f7b 7472 616e 7366 6572  nsfers/{transfer
+00005210: 5461 736b 4964 7d94 7d94 288c 0367 6574  TaskId}.}.(..get
+00005220: 947d 9428 8c04 7461 6773 945d 948c 0954  .}.(..tags.]...T
+00005230: 7261 6e73 6665 7273 9461 8c0b 6465 7363  ransfers.a..desc
+00005240: 7269 7074 696f 6e94 8c1a 5265 7472 6965  ription...Retrie
+00005250: 7665 2061 2074 7261 6e73 6665 7220 7461  ve a transfer ta
+00005260: 736b 2e0a 948c 0b6f 7065 7261 7469 6f6e  sk.....operation
+00005270: 4964 948c 0f67 6574 5472 616e 7366 6572  Id...getTransfer
+00005280: 5461 736b 948c 0a70 6172 616d 6574 6572  Task...parameter
+00005290: 7394 5d94 7d94 288c 046e 616d 6594 8c0e  s.].}.(..name...
+000052a0: 7472 616e 7366 6572 5461 736b 4964 948c  transferTaskId..
+000052b0: 0269 6e94 8c04 7061 7468 948c 0b64 6573  .in...path...des
+000052c0: 6372 6970 7469 6f6e 948c 1054 7261 6e73  cription...Trans
+000052d0: 6665 7220 7461 736b 2049 4494 8c08 7265  fer task ID...re
+000052e0: 7175 6972 6564 9488 8c06 7363 6865 6d61  quired....schema
+000052f0: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+00005300: 6e67 9473 8c07 6578 616d 706c 6594 8c24  ng.s..example..$
+00005310: 3634 3931 6332 6135 2d61 6362 322d 3430  6491c2a5-acb2-40
+00005320: 6566 2d62 3263 302d 6263 3166 6334 6364  ef-b2c0-bc1fc4cd
+00005330: 3765 3663 9475 618c 0972 6573 706f 6e73  7e6c.ua..respons
+00005340: 6573 947d 948c 0332 3030 947d 9428 8c0b  es.}...200.}.(..
+00005350: 6465 7363 7269 7074 696f 6e94 8c02 4f4b  description...OK
+00005360: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
+00005370: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
+00005380: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
+00005390: 7265 6694 8c29 232f 636f 6d70 6f6e 656e  ref..)#/componen
+000053a0: 7473 2f73 6368 656d 6173 2f54 7261 6e73  ts/schemas/Trans
+000053b0: 6665 7254 6173 6b52 6573 706f 6e73 6594  ferTaskResponse.
+000053c0: 7373 7375 7375 8c06 6465 6c65 7465 947d  sssusu..delete.}
+000053d0: 9428 8c04 7461 6773 945d 948c 0954 7261  .(..tags.]...Tra
+000053e0: 6e73 6665 7273 9461 8c0b 6465 7363 7269  nsfers.a..descri
+000053f0: 7074 696f 6e94 8c2b 5265 7175 6573 7420  ption..+Request 
+00005400: 7468 6174 2061 2074 7261 6e73 6665 7220  that a transfer 
+00005410: 7461 736b 2062 6520 6361 6e63 656c 6c65  task be cancelle
+00005420: 642e 0a94 8c0b 6f70 6572 6174 696f 6e49  d.....operationI
+00005430: 6494 8c12 6361 6e63 656c 5472 616e 7366  d...cancelTransf
+00005440: 6572 5461 736b 948c 0a70 6172 616d 6574  erTask...paramet
+00005450: 6572 7394 5d94 7d94 288c 046e 616d 6594  ers.].}.(..name.
+00005460: 8c0e 7472 616e 7366 6572 5461 736b 4964  ..transferTaskId
+00005470: 948c 0269 6e94 8c04 7061 7468 948c 0b64  ...in...path...d
+00005480: 6573 6372 6970 7469 6f6e 948c 1054 7261  escription...Tra
+00005490: 6e73 6665 7220 7461 736b 2049 4494 8c08  nsfer task ID...
+000054a0: 7265 7175 6972 6564 9488 8c06 7363 6865  required....sche
+000054b0: 6d61 947d 948c 0474 7970 6594 8c06 7374  ma.}...type...st
+000054c0: 7269 6e67 9473 8c07 6578 616d 706c 6594  ring.s..example.
+000054d0: 8c24 3634 3931 6332 6135 2d61 6362 322d  .$6491c2a5-acb2-
+000054e0: 3430 6566 2d62 3263 302d 6263 3166 6334  40ef-b2c0-bc1fc4
+000054f0: 6364 3765 3663 9475 618c 0972 6573 706f  cd7e6c.ua..respo
+00005500: 6e73 6573 947d 948c 0332 3030 947d 9428  nses.}...200.}.(
+00005510: 8c0b 6465 7363 7269 7074 696f 6e94 8c02  ..description...
+00005520: 4f4b 948c 0763 6f6e 7465 6e74 947d 948c  OK...content.}..
+00005530: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
+00005540: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
+00005550: 0424 7265 6694 8c23 232f 636f 6d70 6f6e  .$ref..##/compon
+00005560: 656e 7473 2f73 6368 656d 6173 2f53 7472  ents/schemas/Str
+00005570: 696e 6752 6573 706f 6e73 6594 7373 7375  ingResponse.sssu
+00005580: 7375 758c 2c2f 7633 2f66 696c 6573 2f74  suu.,/v3/files/t
+00005590: 7261 6e73 6665 7273 2f7b 7472 616e 7366  ransfers/{transf
+000055a0: 6572 5461 736b 4964 7d2f 6465 7461 696c  erTaskId}/detail
+000055b0: 7394 7d94 8c03 6765 7494 7d94 288c 0474  s.}...get.}.(..t
+000055c0: 6167 7394 5d94 8c09 5472 616e 7366 6572  ags.]...Transfer
+000055d0: 7394 618c 0b64 6573 6372 6970 7469 6f6e  s.a..description
+000055e0: 948c 3352 6574 7269 6576 6520 6465 7461  ..3Retrieve deta
+000055f0: 696c 6564 2069 6e66 6f72 6d61 7469 6f6e  iled information
+00005600: 2066 6f72 2061 2074 7261 6e73 6665 7220   for a transfer 
+00005610: 7461 736b 2e0a 948c 0b6f 7065 7261 7469  task.....operati
+00005620: 6f6e 4964 948c 1667 6574 5472 616e 7366  onId...getTransf
+00005630: 6572 5461 736b 4465 7461 696c 7394 8c0a  erTaskDetails...
+00005640: 7061 7261 6d65 7465 7273 945d 9428 7d94  parameters.].(}.
+00005650: 288c 046e 616d 6594 8c0e 7472 616e 7366  (..name...transf
+00005660: 6572 5461 736b 4964 948c 0269 6e94 8c04  erTaskId...in...
+00005670: 7061 7468 948c 0b64 6573 6372 6970 7469  path...descripti
+00005680: 6f6e 948c 1054 7261 6e73 6665 7220 7461  on...Transfer ta
+00005690: 736b 2049 4494 8c08 7265 7175 6972 6564  sk ID...required
+000056a0: 9488 8c06 7363 6865 6d61 947d 948c 0474  ....schema.}...t
+000056b0: 7970 6594 8c06 7374 7269 6e67 9473 8c07  ype...string.s..
+000056c0: 6578 616d 706c 6594 8c24 3634 3931 6332  example..$6491c2
+000056d0: 6135 2d61 6362 322d 3430 6566 2d62 3263  a5-acb2-40ef-b2c
+000056e0: 302d 6263 3166 6334 6364 3765 3663 9475  0-bc1fc4cd7e6c.u
+000056f0: 7d94 288c 046e 616d 6594 8c0f 696d 7065  }.(..name...impe
+00005700: 7273 6f6e 6174 696f 6e49 6494 8c02 696e  rsonationId...in
+00005710: 948c 0571 7565 7279 948c 0b64 6573 6372  ...query...descr
+00005720: 6970 7469 6f6e 948c 3f52 6573 7472 6963  iption..?Restric
+00005730: 7465 642e 204f 6e6c 7920 6365 7274 6169  ted. Only certai
+00005740: 6e20 7365 7276 6963 6573 206d 6179 2069  n services may i
+00005750: 6d70 6572 736f 6e61 7465 2061 2054 6170  mpersonate a Tap
+00005760: 6973 2075 7365 722e 948c 0673 6368 656d  is user....schem
+00005770: 6194 7d94 8c04 7479 7065 948c 0673 7472  a.}...type...str
+00005780: 696e 6794 7375 658c 0972 6573 706f 6e73  ing.sue..respons
+00005790: 6573 947d 948c 0332 3030 947d 9428 8c0b  es.}...200.}.(..
+000057a0: 6465 7363 7269 7074 696f 6e94 8c02 4f4b  description...OK
+000057b0: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
+000057c0: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
+000057d0: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
+000057e0: 7265 6694 8c29 232f 636f 6d70 6f6e 656e  ref..)#/componen
+000057f0: 7473 2f73 6368 656d 6173 2f54 7261 6e73  ts/schemas/Trans
+00005800: 6665 7254 6173 6b52 6573 706f 6e73 6594  ferTaskResponse.
+00005810: 7373 7375 7375 738c 272f 7633 2f66 696c  sssusus.'/v3/fil
+00005820: 6573 2f70 6572 6d69 7373 696f 6e73 2f7b  es/permissions/{
+00005830: 7379 7374 656d 4964 7d2f 7b70 6174 687d  systemId}/{path}
+00005840: 947d 9428 8c03 6765 7494 7d94 288c 0474  .}.(..get.}.(..t
+00005850: 6167 7394 5d94 8c0b 5065 726d 6973 7369  ags.]...Permissi
+00005860: 6f6e 7394 618c 0b64 6573 6372 6970 7469  ons.a..descripti
+00005870: 6f6e 948c 9347 6574 2074 6865 2054 6170  on...Get the Tap
+00005880: 6973 2070 6572 6d69 7373 696f 6e73 2066  is permissions f
+00005890: 6f72 2061 2075 7365 7220 666f 7220 7468  or a user for th
+000058a0: 6520 7379 7374 656d 2061 6e64 2070 6174  e system and pat
+000058b0: 682e 0a49 6620 6e6f 2075 7365 7220 7370  h..If no user sp
+000058c0: 6563 6966 6965 6420 7468 656e 2070 6572  ecified then per
+000058d0: 6d69 7373 696f 6e73 2061 7265 2072 6574  missions are ret
+000058e0: 7269 6576 6564 2066 6f72 2074 6865 2075  rieved for the u
+000058f0: 7365 7220 6d61 6b69 6e67 2074 6865 2072  ser making the r
+00005900: 6571 7565 7374 2e0a 948c 0b6f 7065 7261  equest.....opera
+00005910: 7469 6f6e 4964 948c 0e67 6574 5065 726d  tionId...getPerm
+00005920: 6973 7369 6f6e 7394 8c0a 7061 7261 6d65  issions...parame
+00005930: 7465 7273 945d 9428 7d94 288c 046e 616d  ters.].(}.(..nam
+00005940: 6594 8c08 7379 7374 656d 4964 948c 0269  e...systemId...i
+00005950: 6e94 8c04 7061 7468 948c 0b64 6573 6372  n...path...descr
+00005960: 6970 7469 6f6e 948c 0953 7973 7465 6d20  iption...System 
+00005970: 4944 948c 0872 6571 7569 7265 6494 888c  ID...required...
+00005980: 0673 6368 656d 6194 7d94 8c04 7479 7065  .schema.}...type
+00005990: 948c 0673 7472 696e 6794 7375 7d94 288c  ...string.su}.(.
+000059a0: 046e 616d 6594 8c04 7061 7468 948c 0269  .name...path...i
+000059b0: 6e94 8c04 7061 7468 948c 0b64 6573 6372  n...path...descr
+000059c0: 6970 7469 6f6e 948c 2550 6174 6820 7265  iption..%Path re
+000059d0: 6c61 7469 7665 2074 6f20 7468 6520 7379  lative to the sy
+000059e0: 7374 656d 202a 726f 6f74 4469 722a 948c  stem *rootDir*..
+000059f0: 0872 6571 7569 7265 6494 888c 0673 6368  .required....sch
+00005a00: 656d 6194 7d94 8c04 7479 7065 948c 0673  ema.}...type...s
+00005a10: 7472 696e 6794 7375 7d94 288c 046e 616d  tring.su}.(..nam
+00005a20: 6594 8c08 7573 6572 6e61 6d65 948c 0269  e...username...i
+00005a30: 6e94 8c05 7175 6572 7994 8c0b 6465 7363  n...query...desc
+00005a40: 7269 7074 696f 6e94 8c10 5573 6572 6e61  ription...Userna
+00005a50: 6d65 2074 6f20 6c69 7374 948c 0673 6368  me to list...sch
+00005a60: 656d 6194 7d94 8c04 7479 7065 948c 0673  ema.}...type...s
+00005a70: 7472 696e 6794 7375 658c 0972 6573 706f  tring.sue..respo
+00005a80: 6e73 6573 947d 948c 0332 3030 947d 9428  nses.}...200.}.(
+00005a90: 8c0b 6465 7363 7269 7074 696f 6e94 8c0e  ..description...
+00005aa0: 4669 6c65 5065 726d 6973 7369 6f6e 948c  FilePermission..
+00005ab0: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
+00005ac0: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
+00005ad0: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
+00005ae0: 6694 8c2b 232f 636f 6d70 6f6e 656e 7473  f..+#/components
+00005af0: 2f73 6368 656d 6173 2f46 696c 6550 6572  /schemas/FilePer
+00005b00: 6d69 7373 696f 6e52 6573 706f 6e73 6594  missionResponse.
+00005b10: 7373 7375 7375 8c04 706f 7374 947d 9428  sssusu..post.}.(
+00005b20: 8c04 7461 6773 945d 948c 0b50 6572 6d69  ..tags.]...Permi
+00005b30: 7373 696f 6e73 9461 8c0b 6465 7363 7269  ssions.a..descri
+00005b40: 7074 696f 6e94 8c56 4772 616e 7420 6163  ption..VGrant ac
+00005b50: 6365 7373 2074 6f20 6120 7061 7468 2066  cess to a path f
+00005b60: 6f72 2061 2075 7365 722e 2041 6363 6573  or a user. Acces
+00005b70: 7320 6d61 7920 6265 2052 4541 4420 6f72  s may be READ or
+00005b80: 204d 4f44 4946 592e 204d 4f44 4946 5920   MODIFY. MODIFY 
+00005b90: 696d 706c 6965 7320 5245 4144 2e0a 948c  implies READ....
+00005ba0: 0b6f 7065 7261 7469 6f6e 4964 948c 1067  .operationId...g
+00005bb0: 7261 6e74 5065 726d 6973 7369 6f6e 7394  rantPermissions.
+00005bc0: 8c0a 7061 7261 6d65 7465 7273 945d 9428  ..parameters.].(
+00005bd0: 7d94 288c 046e 616d 6594 8c08 7379 7374  }.(..name...syst
+00005be0: 656d 4964 948c 0269 6e94 8c04 7061 7468  emId...in...path
+00005bf0: 948c 0b64 6573 6372 6970 7469 6f6e 948c  ...description..
+00005c00: 0953 7973 7465 6d20 4944 948c 0872 6571  .System ID...req
+00005c10: 7569 7265 6494 888c 0673 6368 656d 6194  uired....schema.
+00005c20: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+00005c30: 6794 7375 7d94 288c 046e 616d 6594 8c04  g.su}.(..name...
+00005c40: 7061 7468 948c 0269 6e94 8c04 7061 7468  path...in...path
+00005c50: 948c 0b64 6573 6372 6970 7469 6f6e 948c  ...description..
+00005c60: 2550 6174 6820 7265 6c61 7469 7665 2074  %Path relative t
+00005c70: 6f20 7468 6520 7379 7374 656d 202a 726f  o the system *ro
+00005c80: 6f74 4469 722a 948c 0872 6571 7569 7265  otDir*...require
+00005c90: 6494 888c 0673 6368 656d 6194 7d94 8c04  d....schema.}...
+00005ca0: 7479 7065 948c 0673 7472 696e 6794 7375  type...string.su
+00005cb0: 658c 0b72 6571 7565 7374 426f 6479 947d  e..requestBody.}
+00005cc0: 9428 8c07 636f 6e74 656e 7494 7d94 8c10  .(..content.}...
+00005cd0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+00005ce0: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
+00005cf0: 2472 6566 948c 2c23 2f63 6f6d 706f 6e65  $ref..,#/compone
+00005d00: 6e74 732f 7363 6865 6d61 732f 4372 6561  nts/schemas/Crea
+00005d10: 7465 5065 726d 6973 7369 6f6e 5265 7175  tePermissionRequ
+00005d20: 6573 7494 7373 738c 0872 6571 7569 7265  est.sss..require
+00005d30: 6494 8875 8c09 7265 7370 6f6e 7365 7394  d..u..responses.
+00005d40: 7d94 8c03 3230 3094 7d94 288c 0b64 6573  }...200.}.(..des
+00005d50: 6372 6970 7469 6f6e 948c 0e46 696c 6550  cription...FileP
+00005d60: 6572 6d69 7373 696f 6e94 8c07 636f 6e74  ermission...cont
+00005d70: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
+00005d80: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
+00005d90: 656d 6194 7d94 8c04 2472 6566 948c 2b23  ema.}...$ref..+#
+00005da0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+00005db0: 6d61 732f 4669 6c65 5065 726d 6973 7369  mas/FilePermissi
+00005dc0: 6f6e 5265 7370 6f6e 7365 9473 7373 7573  onResponse.sssus
+00005dd0: 758c 0664 656c 6574 6594 7d94 288c 0474  u..delete.}.(..t
+00005de0: 6167 7394 5d94 8c0b 5065 726d 6973 7369  ags.]...Permissi
+00005df0: 6f6e 7394 618c 0b64 6573 6372 6970 7469  ons.a..descripti
+00005e00: 6f6e 948c 4952 6576 6f6b 6520 6163 6365  on..IRevoke acce
+00005e10: 7373 2066 6f72 2061 2075 7365 7220 666f  ss for a user fo
+00005e20: 7220 7468 6520 7379 7374 656d 2061 6e64  r the system and
+00005e30: 2070 6174 682e 2041 6c6c 2061 6363 6573   path. All acces
+00005e40: 7320 6973 2072 6576 6f6b 6564 2e0a 948c  s is revoked....
+00005e50: 0b6f 7065 7261 7469 6f6e 4964 948c 1164  .operationId...d
+00005e60: 656c 6574 6550 6572 6d69 7373 696f 6e73  eletePermissions
+00005e70: 948c 0a70 6172 616d 6574 6572 7394 5d94  ...parameters.].
+00005e80: 287d 9428 8c04 6e61 6d65 948c 0873 7973  (}.(..name...sys
+00005e90: 7465 6d49 6494 8c02 696e 948c 0470 6174  temId...in...pat
+00005ea0: 6894 8c0b 6465 7363 7269 7074 696f 6e94  h...description.
+00005eb0: 8c09 5379 7374 656d 2049 4494 8c08 7265  ..System ID...re
+00005ec0: 7175 6972 6564 9488 8c06 7363 6865 6d61  quired....schema
+00005ed0: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+00005ee0: 6e67 9473 757d 9428 8c04 6e61 6d65 948c  ng.su}.(..name..
+00005ef0: 0470 6174 6894 8c02 696e 948c 0470 6174  .path...in...pat
+00005f00: 6894 8c0b 6465 7363 7269 7074 696f 6e94  h...description.
+00005f10: 8c25 5061 7468 2072 656c 6174 6976 6520  .%Path relative 
+00005f20: 746f 2074 6865 2073 7973 7465 6d20 2a72  to the system *r
+00005f30: 6f6f 7444 6972 2a94 8c08 7265 7175 6972  ootDir*...requir
+00005f40: 6564 9488 8c06 7363 6865 6d61 947d 948c  ed....schema.}..
+00005f50: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+00005f60: 757d 9428 8c04 6e61 6d65 948c 0875 7365  u}.(..name...use
+00005f70: 726e 616d 6594 8c02 696e 948c 0571 7565  rname...in...que
+00005f80: 7279 948c 0b64 6573 6372 6970 7469 6f6e  ry...description
+00005f90: 948c 1255 7365 726e 616d 6520 746f 2072  ...Username to r
+00005fa0: 656d 6f76 6594 8c08 7265 7175 6972 6564  emove...required
+00005fb0: 9488 8c06 7363 6865 6d61 947d 948c 0474  ....schema.}...t
+00005fc0: 7970 6594 8c06 7374 7269 6e67 9473 7565  ype...string.sue
+00005fd0: 8c09 7265 7370 6f6e 7365 7394 7d94 8c03  ..responses.}...
+00005fe0: 3230 3094 7d94 288c 0b64 6573 6372 6970  200.}.(..descrip
+00005ff0: 7469 6f6e 948c 0e46 696c 6550 6572 6d69  tion...FilePermi
+00006000: 7373 696f 6e94 8c07 636f 6e74 656e 7494  ssion...content.
+00006010: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
+00006020: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
+00006030: 7d94 8c04 2472 6566 948c 2323 2f63 6f6d  }...$ref..##/com
+00006040: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+00006050: 5374 7269 6e67 5265 7370 6f6e 7365 9473  StringResponse.s
+00006060: 7373 7573 7575 8c21 2f76 332f 6669 6c65  ssusuu.!/v3/file
+00006070: 732f 7368 6172 652f 7b73 7973 7465 6d49  s/share/{systemI
+00006080: 647d 2f7b 7061 7468 7d94 7d94 288c 0367  d}/{path}.}.(..g
+00006090: 6574 947d 9428 8c04 7461 6773 945d 948c  et.}.(..tags.]..
+000060a0: 0753 6861 7269 6e67 9461 8c07 7375 6d6d  .Sharing.a..summ
+000060b0: 6172 7994 8c37 5265 7472 6965 7665 2061  ary..7Retrieve a
+000060c0: 6c6c 2073 6861 7269 6e67 2069 6e66 6f72  ll sharing infor
+000060d0: 6d61 7469 6f6e 2066 6f72 2061 2070 6174  mation for a pat
+000060e0: 6820 6f6e 2061 2073 7973 7465 6d94 8c0b  h on a system...
+000060f0: 6465 7363 7269 7074 696f 6e94 8cb2 5265  description...Re
+00006100: 7472 6965 7665 2061 6c6c 2073 6861 7269  trieve all shari
+00006110: 6e67 2069 6e66 6f72 6d61 7469 6f6e 2066  ng information f
+00006120: 6f72 2061 2070 6174 6820 6f6e 2061 2073  or a path on a s
+00006130: 7973 7465 6d2e 2054 6869 7320 696e 636c  ystem. This incl
+00006140: 7564 6573 2061 6c6c 2075 7365 7273 2077  udes all users w
+00006150: 6974 6820 7768 6f6d 2074 6865 2070 6174  ith whom the pat
+00006160: 680a 6861 7320 6265 656e 2073 6861 7265  h.has been share
+00006170: 6420 616e 6420 7768 6574 6865 7220 6f72  d and whether or
+00006180: 206e 6f74 2074 6865 2070 6174 6820 6861   not the path ha
+00006190: 7320 6265 656e 206d 6164 6520 7075 626c  s been made publ
+000061a0: 6963 6c79 2061 7661 696c 6162 6c65 2e0a  icly available..
+000061b0: 948c 0b6f 7065 7261 7469 6f6e 4964 948c  ...operationId..
+000061c0: 0c67 6574 5368 6172 6549 6e66 6f94 8c0a  .getShareInfo...
+000061d0: 7061 7261 6d65 7465 7273 945d 9428 7d94  parameters.].(}.
+000061e0: 288c 046e 616d 6594 8c08 7379 7374 656d  (..name...system
+000061f0: 4964 948c 0269 6e94 8c04 7061 7468 948c  Id...in...path..
+00006200: 0872 6571 7569 7265 6494 888c 0673 6368  .required....sch
+00006210: 656d 6194 7d94 8c04 2472 6566 948c 1d23  ema.}...$ref...#
+00006220: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+00006230: 6d61 732f 4964 5374 7269 6e67 9473 757d  mas/IdString.su}
+00006240: 9428 8c04 6e61 6d65 948c 0470 6174 6894  .(..name...path.
+00006250: 8c02 696e 948c 0470 6174 6894 8c08 7265  ..in...path...re
+00006260: 7175 6972 6564 9488 8c06 7363 6865 6d61  quired....schema
+00006270: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+00006280: 6e67 9473 7565 8c09 7265 7370 6f6e 7365  ng.sue..response
+00006290: 7394 7d94 288c 0332 3030 947d 9428 8c0b  s.}.(..200.}.(..
+000062a0: 6465 7363 7269 7074 696f 6e94 8c08 5375  description...Su
+000062b0: 6363 6573 732e 948c 0763 6f6e 7465 6e74  ccess....content
+000062c0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
+000062d0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
+000062e0: 947d 948c 0424 7265 6694 8c22 232f 636f  .}...$ref.."#/co
+000062f0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00006300: 2f52 6573 7053 6861 7265 496e 666f 9473  /RespShareInfo.s
+00006310: 7373 758c 0334 3030 947d 9428 8c0b 6465  ssu..400.}.(..de
+00006320: 7363 7269 7074 696f 6e94 8c0c 496e 7075  scription...Inpu
+00006330: 7420 6572 726f 722e 948c 0763 6f6e 7465  t error....conte
+00006340: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
+00006350: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
+00006360: 6d61 947d 948c 0424 7265 6694 8c1e 232f  ma.}...$ref...#/
+00006370: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+00006380: 6173 2f52 6573 7042 6173 6963 9473 7373  as/RespBasic.sss
+00006390: 758c 0334 3033 947d 9428 8c0b 6465 7363  u..403.}.(..desc
+000063a0: 7269 7074 696f 6e94 8c11 5065 726d 6973  ription...Permis
+000063b0: 7369 6f6e 2044 656e 6965 6494 8c07 636f  sion Denied...co
+000063c0: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
+000063d0: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
+000063e0: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
+000063f0: 1e23 2f63 6f6d 706f 6e65 6e74 732f 7363  .#/components/sc
+00006400: 6865 6d61 732f 5265 7370 4261 7369 6394  hemas/RespBasic.
+00006410: 7373 7375 8c03 3430 3494 7d94 288c 0b64  sssu..404.}.(..d
+00006420: 6573 6372 6970 7469 6f6e 948c 1153 7973  escription...Sys
+00006430: 7465 6d20 6e6f 7420 666f 756e 642e 948c  tem not found...
+00006440: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
+00006450: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
+00006460: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
+00006470: 6694 8c1e 232f 636f 6d70 6f6e 656e 7473  f...#/components
+00006480: 2f73 6368 656d 6173 2f52 6573 7042 6173  /schemas/RespBas
+00006490: 6963 9473 7373 758c 0335 3030 947d 9428  ic.sssu..500.}.(
+000064a0: 8c0b 6465 7363 7269 7074 696f 6e94 8c0d  ..description...
+000064b0: 5365 7276 6572 2065 7272 6f72 2e94 8c07  Server error....
+000064c0: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
+000064d0: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
+000064e0: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
+000064f0: 948c 1e23 2f63 6f6d 706f 6e65 6e74 732f  ...#/components/
+00006500: 7363 6865 6d61 732f 5265 7370 4261 7369  schemas/RespBasi
+00006510: 6394 7373 7375 7575 8c04 706f 7374 947d  c.sssuuu..post.}
+00006520: 9428 8c04 7461 6773 945d 948c 0753 6861  .(..tags.]...Sha
+00006530: 7269 6e67 9461 8c07 7375 6d6d 6172 7994  ring.a..summary.
+00006540: 8c30 5368 6172 6520 6120 7061 7468 206f  .0Share a path o
+00006550: 6e20 6120 7379 7374 656d 2077 6974 6820  n a system with 
+00006560: 6f6e 6520 6f72 206d 6f72 6520 7573 6572  one or more user
+00006570: 732e 948c 0b64 6573 6372 6970 7469 6f6e  s....description
+00006580: 948c e143 7265 6174 6520 6f72 2075 7064  ...Create or upd
+00006590: 6174 6520 7368 6172 696e 6720 696e 666f  ate sharing info
+000065a0: 726d 6174 696f 6e20 666f 7220 6120 7061  rmation for a pa
+000065b0: 7468 206f 6e20 6120 7379 7374 656d 2e20  th on a system. 
+000065c0: 5468 6520 7061 7468 2077 696c 6c20 6265  The path will be
+000065d0: 2073 6861 7265 6420 7769 7468 2074 6865   shared with the
+000065e0: 206c 6973 7420 6f66 2075 7365 7273 0a70   list of users.p
+000065f0: 726f 7669 6465 6420 696e 2074 6865 2072  rovided in the r
+00006600: 6571 7565 7374 2062 6f64 792e 2052 6571  equest body. Req
+00006610: 7565 7374 6572 206d 7573 7420 6265 206f  uester must be o
+00006620: 776e 6572 206f 6620 7468 6520 7379 7374  wner of the syst
+00006630: 656d 2e20 466f 7220 4c49 4e55 5820 7379  em. For LINUX sy
+00006640: 7374 656d 7320 7061 7468 2073 6861 7269  stems path shari
+00006650: 6e67 2069 730a 6869 6572 6172 6368 6963  ng is.hierarchic
+00006660: 616c 2e0a 948c 0b6f 7065 7261 7469 6f6e  al.....operation
+00006670: 4964 948c 0973 6861 7265 5061 7468 948c  Id...sharePath..
+00006680: 0a70 6172 616d 6574 6572 7394 5d94 287d  .parameters.].(}
+00006690: 9428 8c04 6e61 6d65 948c 0873 7973 7465  .(..name...syste
+000066a0: 6d49 6494 8c02 696e 948c 0470 6174 6894  mId...in...path.
+000066b0: 8c08 7265 7175 6972 6564 9488 8c06 7363  ..required....sc
+000066c0: 6865 6d61 947d 948c 0424 7265 6694 8c1d  hema.}...$ref...
+000066d0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+000066e0: 656d 6173 2f49 6453 7472 696e 6794 7375  emas/IdString.su
+000066f0: 7d94 288c 046e 616d 6594 8c04 7061 7468  }.(..name...path
+00006700: 948c 0269 6e94 8c04 7061 7468 948c 0872  ...in...path...r
+00006710: 6571 7569 7265 6494 888c 0673 6368 656d  equired....schem
+00006720: 6194 7d94 8c04 7479 7065 948c 0673 7472  a.}...type...str
+00006730: 696e 6794 7375 658c 0b72 6571 7565 7374  ing.sue..request
+00006740: 426f 6479 947d 9428 8c08 7265 7175 6972  Body.}.(..requir
+00006750: 6564 9488 8c0b 6465 7363 7269 7074 696f  ed....descriptio
+00006760: 6e94 8c35 4120 4a53 4f4e 206f 626a 6563  n..5A JSON objec
+00006770: 7420 7370 6563 6966 7969 6e67 2075 7064  t specifying upd
+00006780: 6174 6564 2073 6861 7269 6e67 2069 6e66  ated sharing inf
+00006790: 6f72 6d61 7469 6f6e 2e94 8c07 636f 6e74  ormation....cont
+000067a0: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
+000067b0: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
+000067c0: 656d 6194 7d94 8c04 2472 6566 948c 2323  ema.}...$ref..##
+000067d0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+000067e0: 6d61 732f 5265 7153 6861 7265 5570 6461  mas/ReqShareUpda
+000067f0: 7465 9473 7373 758c 0972 6573 706f 6e73  te.sssu..respons
+00006800: 6573 947d 9428 8c03 3230 3094 7d94 288c  es.}.(..200.}.(.
+00006810: 0b64 6573 6372 6970 7469 6f6e 948c 1c53  .description...S
+00006820: 6861 7269 6e67 2069 6e66 6f72 6d61 7469  haring informati
+00006830: 6f6e 2075 7064 6174 6564 2e94 8c07 636f  on updated....co
+00006840: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
+00006850: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
+00006860: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
+00006870: 1e23 2f63 6f6d 706f 6e65 6e74 732f 7363  .#/components/sc
+00006880: 6865 6d61 732f 5265 7370 4261 7369 6394  hemas/RespBasic.
+00006890: 7373 7375 8c03 3430 3094 7d94 288c 0b64  sssu..400.}.(..d
+000068a0: 6573 6372 6970 7469 6f6e 948c 1a49 6e70  escription...Inp
+000068b0: 7574 2065 7272 6f72 2e20 496e 7661 6c69  ut error. Invali
+000068c0: 6420 4a53 4f4e 2e94 8c07 636f 6e74 656e  d JSON....conten
+000068d0: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
+000068e0: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
+000068f0: 6194 7d94 8c04 2472 6566 948c 1e23 2f63  a.}...$ref...#/c
+00006900: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+00006910: 732f 5265 7370 4261 7369 6394 7373 7375  s/RespBasic.sssu
+00006920: 8c03 3430 3394 7d94 288c 0b64 6573 6372  ..403.}.(..descr
+00006930: 6970 7469 6f6e 948c 1150 6572 6d69 7373  iption...Permiss
+00006940: 696f 6e20 4465 6e69 6564 948c 0763 6f6e  ion Denied...con
+00006950: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
+00006960: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
+00006970: 6865 6d61 947d 948c 0424 7265 6694 8c1e  hema.}...$ref...
+00006980: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+00006990: 656d 6173 2f52 6573 7042 6173 6963 9473  emas/RespBasic.s
+000069a0: 7373 758c 0335 3030 947d 9428 8c0b 6465  ssu..500.}.(..de
+000069b0: 7363 7269 7074 696f 6e94 8c0d 5365 7276  scription...Serv
+000069c0: 6572 2065 7272 6f72 2e94 8c07 636f 6e74  er error....cont
+000069d0: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
+000069e0: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
+000069f0: 656d 6194 7d94 8c04 2472 6566 948c 1e23  ema.}...$ref...#
+00006a00: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+00006a10: 6d61 732f 5265 7370 4261 7369 6394 7373  mas/RespBasic.ss
+00006a20: 7375 7575 758c 282f 7633 2f66 696c 6573  suuuu.(/v3/files
+00006a30: 2f73 6861 7265 5f70 7562 6c69 632f 7b73  /share_public/{s
+00006a40: 7973 7465 6d49 647d 2f7b 7061 7468 7d94  ystemId}/{path}.
+00006a50: 7d94 8c04 706f 7374 947d 9428 8c04 7461  }...post.}.(..ta
+00006a60: 6773 945d 948c 0753 6861 7269 6e67 9461  gs.]...Sharing.a
+00006a70: 8c07 7375 6d6d 6172 7994 8c3f 5368 6172  ..summary..?Shar
+00006a80: 6520 6120 7061 7468 206f 6e20 6120 7379  e a path on a sy
+00006a90: 7374 656d 2070 7562 6c69 636c 7920 7769  stem publicly wi
+00006aa0: 7468 2061 6c6c 2075 7365 7273 2069 6e20  th all users in 
+00006ab0: 7468 6520 7465 6e61 6e74 2e94 8c0b 6465  the tenant....de
+00006ac0: 7363 7269 7074 696f 6e94 8c5e 5368 6172  scription..^Shar
+00006ad0: 6520 6120 7061 7468 206f 6e20 6120 7379  e a path on a sy
+00006ae0: 7374 656d 2077 6974 6820 616c 6c20 7573  stem with all us
+00006af0: 6572 7320 696e 2074 6865 2074 656e 616e  ers in the tenan
+00006b00: 742e 2052 6571 7565 7374 6572 206d 7573  t. Requester mus
+00006b10: 7420 6265 206f 776e 6572 206f 6620 7468  t be owner of th
+00006b20: 6520 7379 7374 656d 2e0a 948c 0b6f 7065  e system.....ope
+00006b30: 7261 7469 6f6e 4964 948c 0f73 6861 7265  rationId...share
+00006b40: 5061 7468 5075 626c 6963 948c 0a70 6172  PathPublic...par
+00006b50: 616d 6574 6572 7394 5d94 287d 9428 8c04  ameters.].(}.(..
+00006b60: 6e61 6d65 948c 0873 7973 7465 6d49 6494  name...systemId.
+00006b70: 8c02 696e 948c 0470 6174 6894 8c08 7265  ..in...path...re
+00006b80: 7175 6972 6564 9488 8c06 7363 6865 6d61  quired....schema
+00006b90: 947d 948c 0424 7265 6694 8c1d 232f 636f  .}...$ref...#/co
+00006ba0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00006bb0: 2f49 6453 7472 696e 6794 7375 7d94 288c  /IdString.su}.(.
+00006bc0: 046e 616d 6594 8c04 7061 7468 948c 0269  .name...path...i
+00006bd0: 6e94 8c04 7061 7468 948c 0872 6571 7569  n...path...requi
+00006be0: 7265 6494 888c 0673 6368 656d 6194 7d94  red....schema.}.
+00006bf0: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+00006c00: 7375 658c 0972 6573 706f 6e73 6573 947d  sue..responses.}
+00006c10: 9428 8c03 3230 3094 7d94 288c 0b64 6573  .(..200.}.(..des
+00006c20: 6372 6970 7469 6f6e 948c 1550 6174 6820  cription...Path 
+00006c30: 7368 6172 6564 2070 7562 6c69 636c 792e  shared publicly.
+00006c40: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
+00006c50: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
+00006c60: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
+00006c70: 7265 6694 8c1e 232f 636f 6d70 6f6e 656e  ref...#/componen
+00006c80: 7473 2f73 6368 656d 6173 2f52 6573 7042  ts/schemas/RespB
+00006c90: 6173 6963 9473 7373 758c 0334 3033 947d  asic.sssu..403.}
+00006ca0: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
+00006cb0: 8c11 5065 726d 6973 7369 6f6e 2044 656e  ..Permission Den
+00006cc0: 6965 6494 8c07 636f 6e74 656e 7494 7d94  ied...content.}.
+00006cd0: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
+00006ce0: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
+00006cf0: 8c04 2472 6566 948c 1e23 2f63 6f6d 706f  ..$ref...#/compo
+00006d00: 6e65 6e74 732f 7363 6865 6d61 732f 5265  nents/schemas/Re
+00006d10: 7370 4261 7369 6394 7373 7375 8c03 3530  spBasic.sssu..50
+00006d20: 3094 7d94 288c 0b64 6573 6372 6970 7469  0.}.(..descripti
+00006d30: 6f6e 948c 0d53 6572 7665 7220 6572 726f  on...Server erro
+00006d40: 722e 948c 0763 6f6e 7465 6e74 947d 948c  r....content.}..
+00006d50: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
+00006d60: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
+00006d70: 0424 7265 6694 8c1e 232f 636f 6d70 6f6e  .$ref...#/compon
+00006d80: 656e 7473 2f73 6368 656d 6173 2f52 6573  ents/schemas/Res
+00006d90: 7042 6173 6963 9473 7373 7575 7573 8c23  pBasic.sssuuus.#
+00006da0: 2f76 332f 6669 6c65 732f 756e 7368 6172  /v3/files/unshar
+00006db0: 652f 7b73 7973 7465 6d49 647d 2f7b 7061  e/{systemId}/{pa
+00006dc0: 7468 7d94 7d94 8c04 706f 7374 947d 9428  th}.}...post.}.(
+00006dd0: 8c04 7461 6773 945d 948c 0753 6861 7269  ..tags.]...Shari
+00006de0: 6e67 9461 8c07 7375 6d6d 6172 7994 8c32  ng.a..summary..2
+00006df0: 556e 7368 6172 6520 6120 7061 7468 206f  Unshare a path o
+00006e00: 6e20 6120 7379 7374 656d 2077 6974 6820  n a system with 
+00006e10: 6f6e 6520 6f72 206d 6f72 6520 7573 6572  one or more user
+00006e20: 732e 948c 0b64 6573 6372 6970 7469 6f6e  s....description
+00006e30: 948c b343 7265 6174 6520 6f72 2075 7064  ...Create or upd
+00006e40: 6174 6520 7368 6172 696e 6720 696e 666f  ate sharing info
+00006e50: 726d 6174 696f 6e20 666f 7220 6120 7061  rmation for a pa
+00006e60: 7468 206f 6e20 6120 7379 7374 656d 2e20  th on a system. 
+00006e70: 5468 6520 7061 7468 2077 696c 6c20 6265  The path will be
+00006e80: 2075 6e73 6861 7265 6420 7769 7468 2074   unshared with t
+00006e90: 6865 206c 6973 7420 6f66 2075 7365 7273  he list of users
+00006ea0: 0a70 726f 7669 6465 6420 696e 2074 6865  .provided in the
+00006eb0: 2072 6571 7565 7374 2062 6f64 792e 2052   request body. R
+00006ec0: 6571 7565 7374 6572 206d 7573 7420 6265  equester must be
+00006ed0: 206f 776e 6572 206f 6620 7468 6520 7379   owner of the sy
+00006ee0: 7374 656d 2e0a 948c 0b6f 7065 7261 7469  stem.....operati
+00006ef0: 6f6e 4964 948c 0b75 6e53 6861 7265 5061  onId...unSharePa
+00006f00: 7468 948c 0a70 6172 616d 6574 6572 7394  th...parameters.
+00006f10: 5d94 287d 9428 8c04 6e61 6d65 948c 0873  ].(}.(..name...s
+00006f20: 7973 7465 6d49 6494 8c02 696e 948c 0470  ystemId...in...p
+00006f30: 6174 6894 8c08 7265 7175 6972 6564 9488  ath...required..
+00006f40: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
+00006f50: 6694 8c1d 232f 636f 6d70 6f6e 656e 7473  f...#/components
+00006f60: 2f73 6368 656d 6173 2f49 6453 7472 696e  /schemas/IdStrin
+00006f70: 6794 7375 7d94 288c 046e 616d 6594 8c04  g.su}.(..name...
+00006f80: 7061 7468 948c 0269 6e94 8c04 7061 7468  path...in...path
+00006f90: 948c 0872 6571 7569 7265 6494 888c 0673  ...required....s
+00006fa0: 6368 656d 6194 7d94 8c04 7479 7065 948c  chema.}...type..
+00006fb0: 0673 7472 696e 6794 7375 658c 0b72 6571  .string.sue..req
+00006fc0: 7565 7374 426f 6479 947d 9428 8c08 7265  uestBody.}.(..re
+00006fd0: 7175 6972 6564 9488 8c0b 6465 7363 7269  quired....descri
+00006fe0: 7074 696f 6e94 8c35 4120 4a53 4f4e 206f  ption..5A JSON o
+00006ff0: 626a 6563 7420 7370 6563 6966 7969 6e67  bject specifying
+00007000: 2075 7064 6174 6564 2073 6861 7269 6e67   updated sharing
+00007010: 2069 6e66 6f72 6d61 7469 6f6e 2e94 8c07   information....
+00007020: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
+00007030: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
+00007040: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
+00007050: 948c 2323 2f63 6f6d 706f 6e65 6e74 732f  ..##/components/
+00007060: 7363 6865 6d61 732f 5265 7153 6861 7265  schemas/ReqShare
+00007070: 5570 6461 7465 9473 7373 758c 0972 6573  Update.sssu..res
+00007080: 706f 6e73 6573 947d 9428 8c03 3230 3094  ponses.}.(..200.
+00007090: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
+000070a0: 948c 1c53 6861 7269 6e67 2069 6e66 6f72  ...Sharing infor
+000070b0: 6d61 7469 6f6e 2075 7064 6174 6564 2e94  mation updated..
+000070c0: 8c07 636f 6e74 656e 7494 7d94 8c10 6170  ..content.}...ap
+000070d0: 706c 6963 6174 696f 6e2f 6a73 6f6e 947d  plication/json.}
+000070e0: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
+000070f0: 6566 948c 1e23 2f63 6f6d 706f 6e65 6e74  ef...#/component
+00007100: 732f 7363 6865 6d61 732f 5265 7370 4261  s/schemas/RespBa
+00007110: 7369 6394 7373 7375 8c03 3430 3094 7d94  sic.sssu..400.}.
+00007120: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
+00007130: 1a49 6e70 7574 2065 7272 6f72 2e20 496e  .Input error. In
+00007140: 7661 6c69 6420 4a53 4f4e 2e94 8c07 636f  valid JSON....co
+00007150: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
+00007160: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
+00007170: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
+00007180: 1e23 2f63 6f6d 706f 6e65 6e74 732f 7363  .#/components/sc
+00007190: 6865 6d61 732f 5265 7370 4261 7369 6394  hemas/RespBasic.
+000071a0: 7373 7375 8c03 3430 3394 7d94 288c 0b64  sssu..403.}.(..d
+000071b0: 6573 6372 6970 7469 6f6e 948c 1150 6572  escription...Per
+000071c0: 6d69 7373 696f 6e20 4465 6e69 6564 948c  mission Denied..
+000071d0: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
+000071e0: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
+000071f0: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
+00007200: 6694 8c1e 232f 636f 6d70 6f6e 656e 7473  f...#/components
+00007210: 2f73 6368 656d 6173 2f52 6573 7042 6173  /schemas/RespBas
+00007220: 6963 9473 7373 758c 0335 3030 947d 9428  ic.sssu..500.}.(
+00007230: 8c0b 6465 7363 7269 7074 696f 6e94 8c0d  ..description...
+00007240: 5365 7276 6572 2065 7272 6f72 2e94 8c07  Server error....
+00007250: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
+00007260: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
+00007270: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
+00007280: 948c 1e23 2f63 6f6d 706f 6e65 6e74 732f  ...#/components/
+00007290: 7363 6865 6d61 732f 5265 7370 4261 7369  schemas/RespBasi
+000072a0: 6394 7373 7375 7575 738c 2a2f 7633 2f66  c.sssuuus.*/v3/f
+000072b0: 696c 6573 2f75 6e73 6861 7265 5f70 7562  iles/unshare_pub
+000072c0: 6c69 632f 7b73 7973 7465 6d49 647d 2f7b  lic/{systemId}/{
+000072d0: 7061 7468 7d94 7d94 8c04 706f 7374 947d  path}.}...post.}
+000072e0: 9428 8c04 7461 6773 945d 948c 0753 6861  .(..tags.]...Sha
+000072f0: 7269 6e67 9461 8c07 7375 6d6d 6172 7994  ring.a..summary.
+00007300: 8c2c 5265 6d6f 7665 2070 7562 6c69 6320  .,Remove public 
+00007310: 6163 6365 7373 2066 6f72 2061 2070 6174  access for a pat
+00007320: 6820 6f6e 2061 2073 7973 7465 6d2e 948c  h on a system...
+00007330: 0b64 6573 6372 6970 7469 6f6e 948c 5552  .description..UR
+00007340: 656d 6f76 6520 7075 626c 6963 2073 6861  emove public sha
+00007350: 7269 6e67 2066 6f72 2061 2070 6174 6820  ring for a path 
+00007360: 6f6e 2061 2073 7973 7465 6d2e 2052 6571  on a system. Req
+00007370: 7565 7374 6572 206d 7573 7420 6265 206f  uester must be o
+00007380: 776e 6572 206f 6620 7468 6520 7379 7374  wner of the syst
+00007390: 656d 2e0a 948c 0b6f 7065 7261 7469 6f6e  em.....operation
+000073a0: 4964 948c 1175 6e53 6861 7265 5061 7468  Id...unSharePath
+000073b0: 5075 626c 6963 948c 0a70 6172 616d 6574  Public...paramet
+000073c0: 6572 7394 5d94 287d 9428 8c04 6e61 6d65  ers.].(}.(..name
+000073d0: 948c 0873 7973 7465 6d49 6494 8c02 696e  ...systemId...in
+000073e0: 948c 0470 6174 6894 8c08 7265 7175 6972  ...path...requir
+000073f0: 6564 9488 8c06 7363 6865 6d61 947d 948c  ed....schema.}..
+00007400: 0424 7265 6694 8c1d 232f 636f 6d70 6f6e  .$ref...#/compon
+00007410: 656e 7473 2f73 6368 656d 6173 2f49 6453  ents/schemas/IdS
+00007420: 7472 696e 6794 7375 7d94 288c 046e 616d  tring.su}.(..nam
+00007430: 6594 8c04 7061 7468 948c 0269 6e94 8c04  e...path...in...
+00007440: 7061 7468 948c 0872 6571 7569 7265 6494  path...required.
+00007450: 888c 0673 6368 656d 6194 7d94 8c04 7479  ...schema.}...ty
+00007460: 7065 948c 0673 7472 696e 6794 7375 658c  pe...string.sue.
+00007470: 0972 6573 706f 6e73 6573 947d 9428 8c03  .responses.}.(..
+00007480: 3230 3094 7d94 288c 0b64 6573 6372 6970  200.}.(..descrip
+00007490: 7469 6f6e 948c 1b50 6174 6820 7075 626c  tion...Path publ
+000074a0: 6963 2061 6363 6573 7320 7265 6d6f 7665  ic access remove
+000074b0: 642e 948c 0763 6f6e 7465 6e74 947d 948c  d....content.}..
+000074c0: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
+000074d0: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
+000074e0: 0424 7265 6694 8c1e 232f 636f 6d70 6f6e  .$ref...#/compon
+000074f0: 656e 7473 2f73 6368 656d 6173 2f52 6573  ents/schemas/Res
+00007500: 7042 6173 6963 9473 7373 758c 0334 3033  pBasic.sssu..403
+00007510: 947d 9428 8c0b 6465 7363 7269 7074 696f  .}.(..descriptio
+00007520: 6e94 8c11 5065 726d 6973 7369 6f6e 2044  n...Permission D
+00007530: 656e 6965 6494 8c07 636f 6e74 656e 7494  enied...content.
+00007540: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
+00007550: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
+00007560: 7d94 8c04 2472 6566 948c 1e23 2f63 6f6d  }...$ref...#/com
+00007570: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+00007580: 5265 7370 4261 7369 6394 7373 7375 8c03  RespBasic.sssu..
+00007590: 3530 3094 7d94 288c 0b64 6573 6372 6970  500.}.(..descrip
+000075a0: 7469 6f6e 948c 0d53 6572 7665 7220 6572  tion...Server er
+000075b0: 726f 722e 948c 0763 6f6e 7465 6e74 947d  ror....content.}
+000075c0: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
+000075d0: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
+000075e0: 948c 0424 7265 6694 8c1e 232f 636f 6d70  ...$ref...#/comp
+000075f0: 6f6e 656e 7473 2f73 6368 656d 6173 2f52  onents/schemas/R
+00007600: 6573 7042 6173 6963 9473 7373 7575 7573  espBasic.sssuuus
+00007610: 8c27 2f76 332f 6669 6c65 732f 756e 7368  .'/v3/files/unsh
+00007620: 6172 655f 616c 6c2f 7b73 7973 7465 6d49  are_all/{systemI
+00007630: 647d 2f7b 7061 7468 7d94 7d94 8c04 706f  d}/{path}.}...po
+00007640: 7374 947d 9428 8c04 7461 6773 945d 948c  st.}.(..tags.]..
+00007650: 0753 6861 7269 6e67 9461 8c07 7375 6d6d  .Sharing.a..summ
+00007660: 6172 7994 8c41 5265 6d6f 7665 2061 6c6c  ary..ARemove all
+00007670: 2073 6861 7265 7320 666f 7220 6120 7061   shares for a pa
+00007680: 7468 206f 6e20 6120 7379 7374 656d 2069  th on a system i
+00007690: 6e63 6c75 6469 6e67 2070 7562 6c69 6320  ncluding public 
+000076a0: 6163 6365 7373 2e94 8c0b 6465 7363 7269  access....descri
+000076b0: 7074 696f 6e94 8c6c 5265 6d6f 7665 2061  ption..lRemove a
+000076c0: 6c6c 2073 6861 7265 7320 666f 7220 6120  ll shares for a 
+000076d0: 7061 7468 206f 6e20 6120 7379 7374 656d  path on a system
+000076e0: 2069 6e63 6c75 6469 6e67 2070 7562 6c69   including publi
+000076f0: 6320 6163 6365 7373 2e20 5468 6973 2077  c access. This w
+00007700: 696c 6c20 616c 736f 2062 6520 646f 6e65  ill also be done
+00007710: 2066 6f72 2061 6c6c 2073 7562 2d70 6174   for all sub-pat
+00007720: 6873 2e0a 948c 0b6f 7065 7261 7469 6f6e  hs.....operation
+00007730: 4964 948c 0e75 6e53 6861 7265 5061 7468  Id...unSharePath
+00007740: 416c 6c94 8c0a 7061 7261 6d65 7465 7273  All...parameters
+00007750: 945d 9428 7d94 288c 046e 616d 6594 8c08  .].(}.(..name...
+00007760: 7379 7374 656d 4964 948c 0269 6e94 8c04  systemId...in...
+00007770: 7061 7468 948c 0872 6571 7569 7265 6494  path...required.
+00007780: 888c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
+00007790: 6566 948c 1d23 2f63 6f6d 706f 6e65 6e74  ef...#/component
+000077a0: 732f 7363 6865 6d61 732f 4964 5374 7269  s/schemas/IdStri
+000077b0: 6e67 9473 757d 9428 8c04 6e61 6d65 948c  ng.su}.(..name..
+000077c0: 0470 6174 6894 8c02 696e 948c 0470 6174  .path...in...pat
+000077d0: 6894 8c08 7265 7175 6972 6564 9488 8c06  h...required....
+000077e0: 7363 6865 6d61 947d 948c 0474 7970 6594  schema.}...type.
+000077f0: 8c06 7374 7269 6e67 9473 757d 9428 8c04  ..string.su}.(..
+00007800: 6e61 6d65 948c 0772 6563 7572 7365 948c  name...recurse..
+00007810: 0269 6e94 8c05 7175 6572 7994 8c08 7265  .in...query...re
+00007820: 7175 6972 6564 9489 8c06 7363 6865 6d61  quired....schema
+00007830: 947d 9428 8c04 7479 7065 948c 0762 6f6f  .}.(..type...boo
+00007840: 6c65 616e 948c 0764 6566 6175 6c74 9489  lean...default..
+00007850: 7575 658c 0972 6573 706f 6e73 6573 947d  uue..responses.}
+00007860: 9428 8c03 3230 3094 7d94 288c 0b64 6573  .(..200.}.(..des
+00007870: 6372 6970 7469 6f6e 948c 1941 6c6c 2073  cription...All s
+00007880: 6861 7265 2061 6363 6573 7320 7265 6d6f  hare access remo
+00007890: 7665 642e 948c 0763 6f6e 7465 6e74 947d  ved....content.}
+000078a0: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
+000078b0: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
+000078c0: 948c 0424 7265 6694 8c1e 232f 636f 6d70  ...$ref...#/comp
+000078d0: 6f6e 656e 7473 2f73 6368 656d 6173 2f52  onents/schemas/R
+000078e0: 6573 7042 6173 6963 9473 7373 758c 0334  espBasic.sssu..4
+000078f0: 3033 947d 9428 8c0b 6465 7363 7269 7074  03.}.(..descript
+00007900: 696f 6e94 8c11 5065 726d 6973 7369 6f6e  ion...Permission
+00007910: 2044 656e 6965 6494 8c07 636f 6e74 656e   Denied...conten
+00007920: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
+00007930: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
+00007940: 6194 7d94 8c04 2472 6566 948c 1e23 2f63  a.}...$ref...#/c
+00007950: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+00007960: 732f 5265 7370 4261 7369 6394 7373 7375  s/RespBasic.sssu
+00007970: 8c03 3530 3094 7d94 288c 0b64 6573 6372  ..500.}.(..descr
+00007980: 6970 7469 6f6e 948c 0d53 6572 7665 7220  iption...Server 
+00007990: 6572 726f 722e 948c 0763 6f6e 7465 6e74  error....content
+000079a0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
+000079b0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
+000079c0: 947d 948c 0424 7265 6694 8c1e 232f 636f  .}...$ref...#/co
+000079d0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+000079e0: 2f52 6573 7042 6173 6963 9473 7373 7575  /RespBasic.sssuu
+000079f0: 7573 8c23 2f76 332f 6669 6c65 732f 706f  us.#/v3/files/po
+00007a00: 7374 6974 732f 7b73 7973 7465 6d49 647d  stits/{systemId}
+00007a10: 2f7b 7061 7468 7d94 7d94 8c04 706f 7374  /{path}.}...post
+00007a20: 947d 9428 8c07 7375 6d6d 6172 7994 8c0f  .}.(..summary...
+00007a30: 4372 6561 7465 2061 2050 6f73 7449 7494  Create a PostIt.
+00007a40: 8c04 7461 6773 945d 948c 0750 6f73 7449  ..tags.]...PostI
+00007a50: 7473 9461 8c0b 6465 7363 7269 7074 696f  ts.a..descriptio
+00007a60: 6e94 8ce0 4372 6561 7465 2061 2050 6f73  n...Create a Pos
+00007a70: 7449 742e 2020 5468 6520 506f 7374 4974  tIt.  The PostIt
+00007a80: 2077 696c 6c20 6772 616e 7420 6163 6365   will grant acce
+00007a90: 7373 2074 6f20 6120 6669 6c65 2075 726c  ss to a file url
+00007aa0: 2e0a 5468 6520 6e65 776c 7920 6372 6561  ..The newly crea
+00007ab0: 7465 6420 506f 7374 4974 2063 616e 2062  ted PostIt can b
+00007ac0: 6520 7265 6465 656d 6564 2062 7920 616e  e redeemed by an
+00007ad0: 796f 6e65 2077 6974 686f 7574 200a 6675  yone without .fu
+00007ae0: 7274 6865 7220 6175 7468 6f72 697a 6174  rther authorizat
+00007af0: 696f 6e2e 2020 5468 6973 2077 696c 6c20  ion.  This will 
+00007b00: 6e65 6172 6c79 2069 6465 6e74 6963 616c  nearly identical
+00007b10: 2074 6f20 6361 6c6c 696e 670a 7468 6520   to calling.the 
+00007b20: 6669 6c65 7320 7365 7276 6963 6520 6765  files service ge
+00007b30: 7443 6f6e 7465 6e74 7320 656e 6470 6f69  tContents endpoi
+00007b40: 6e74 2e0a 948c 0b6f 7065 7261 7469 6f6e  nt.....operation
+00007b50: 4964 948c 0c63 7265 6174 6550 6f73 7449  Id...createPostI
+00007b60: 7494 8c0a 7061 7261 6d65 7465 7273 945d  t...parameters.]
+00007b70: 9428 7d94 288c 046e 616d 6594 8c08 7379  .(}.(..name...sy
+00007b80: 7374 656d 4964 948c 0b64 6573 6372 6970  stemId...descrip
+00007b90: 7469 6f6e 948c 3054 6865 206e 616d 6520  tion..0The name 
+00007ba0: 6f66 2074 6865 2073 7973 7465 6d20 746f  of the system to
+00007bb0: 2063 7265 6174 6520 7468 6520 506f 7374   create the Post
+00007bc0: 4974 2066 6f72 2e94 8c02 696e 948c 0470  It for....in...p
+00007bd0: 6174 6894 8c08 7265 7175 6972 6564 9488  ath...required..
+00007be0: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
+00007bf0: 6694 8c1d 232f 636f 6d70 6f6e 656e 7473  f...#/components
+00007c00: 2f73 6368 656d 6173 2f49 6453 7472 696e  /schemas/IdStrin
+00007c10: 6794 7375 7d94 288c 046e 616d 6594 8c04  g.su}.(..name...
+00007c20: 7061 7468 948c 0269 6e94 8c04 7061 7468  path...in...path
+00007c30: 948c 0872 6571 7569 7265 6494 888c 0b64  ...required....d
+00007c40: 6573 6372 6970 7469 6f6e 948c 2550 6174  escription..%Pat
+00007c50: 6820 7265 6c61 7469 7665 2074 6f20 7468  h relative to th
+00007c60: 6520 7379 7374 656d 202a 726f 6f74 4469  e system *rootDi
+00007c70: 722a 948c 0765 7861 6d70 6c65 948c 1f2f  r*...example.../
+00007c80: 4469 7265 6374 6f72 7941 2f44 6972 6563  DirectoryA/Direc
+00007c90: 746f 7279 422f 6669 6c65 2e74 7874 948c  toryB/file.txt..
+00007ca0: 0673 6368 656d 6194 7d94 8c04 7479 7065  .schema.}...type
+00007cb0: 948c 0673 7472 696e 6794 7375 658c 0b72  ...string.sue..r
+00007cc0: 6571 7565 7374 426f 6479 947d 9428 8c08  equestBody.}.(..
+00007cd0: 7265 7175 6972 6564 9488 8c0b 6465 7363  required....desc
+00007ce0: 7269 7074 696f 6e94 8c34 4120 4a53 4f4e  ription..4A JSON
+00007cf0: 2064 6f63 756d 656e 7420 6465 7363 7269   document descri
+00007d00: 6269 6e67 2074 6865 2050 6f73 7449 7420  bing the PostIt 
+00007d10: 746f 2062 6520 6372 6561 7465 642e 948c  to be created...
+00007d20: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
+00007d30: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
+00007d40: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
+00007d50: 6694 8c28 232f 636f 6d70 6f6e 656e 7473  f..(#/components
+00007d60: 2f73 6368 656d 6173 2f43 7265 6174 6550  /schemas/CreateP
+00007d70: 6f73 7449 7452 6571 7565 7374 9473 7373  ostItRequest.sss
+00007d80: 758c 0972 6573 706f 6e73 6573 947d 9428  u..responses.}.(
+00007d90: 8c03 3230 3094 7d94 288c 0b64 6573 6372  ..200.}.(..descr
+00007da0: 6970 7469 6f6e 948c 0853 7563 6365 7373  iption...Success
+00007db0: 2e94 8c07 636f 6e74 656e 7494 7d94 8c10  ....content.}...
+00007dc0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+00007dd0: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
+00007de0: 2472 6566 948c 2323 2f63 6f6d 706f 6e65  $ref..##/compone
+00007df0: 6e74 732f 7363 6865 6d61 732f 506f 7374  nts/schemas/Post
+00007e00: 4974 5265 7370 6f6e 7365 9473 7373 758c  ItResponse.sssu.
+00007e10: 0334 3030 947d 9428 8c0b 6465 7363 7269  .400.}.(..descri
+00007e20: 7074 696f 6e94 8c0b 4261 6420 5265 7175  ption...Bad Requ
+00007e30: 6573 7494 8c07 636f 6e74 656e 7494 7d94  est...content.}.
+00007e40: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
+00007e50: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
+00007e60: 8c04 2472 6566 948c 2723 2f63 6f6d 706f  ..$ref..'#/compo
+00007e70: 6e65 6e74 732f 7363 6865 6d61 732f 4669  nents/schemas/Fi
+00007e80: 6c65 5374 7269 6e67 5265 7370 6f6e 7365  leStringResponse
+00007e90: 9473 7373 758c 0334 3031 947d 9428 8c0b  .sssu..401.}.(..
+00007ea0: 6465 7363 7269 7074 696f 6e94 8c11 4e6f  description...No
+00007eb0: 7420 4175 7468 656e 7469 6361 7465 6494  t Authenticated.
+00007ec0: 8c07 636f 6e74 656e 7494 7d94 8c10 6170  ..content.}...ap
+00007ed0: 706c 6963 6174 696f 6e2f 6a73 6f6e 947d  plication/json.}
+00007ee0: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
+00007ef0: 6566 948c 2723 2f63 6f6d 706f 6e65 6e74  ef..'#/component
+00007f00: 732f 7363 6865 6d61 732f 4669 6c65 5374  s/schemas/FileSt
+00007f10: 7269 6e67 5265 7370 6f6e 7365 9473 7373  ringResponse.sss
+00007f20: 758c 0334 3033 947d 9428 8c0b 6465 7363  u..403.}.(..desc
+00007f30: 7269 7074 696f 6e94 8c11 5065 726d 6973  ription...Permis
+00007f40: 7369 6f6e 2044 656e 6965 6494 8c07 636f  sion Denied...co
+00007f50: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
+00007f60: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
+00007f70: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
+00007f80: 2723 2f63 6f6d 706f 6e65 6e74 732f 7363  '#/components/sc
+00007f90: 6865 6d61 732f 4669 6c65 5374 7269 6e67  hemas/FileString
+00007fa0: 5265 7370 6f6e 7365 9473 7373 758c 0334  Response.sssu..4
+00007fb0: 3034 947d 9428 8c0b 6465 7363 7269 7074  04.}.(..descript
+00007fc0: 696f 6e94 8c09 4e6f 7420 466f 756e 6494  ion...Not Found.
+00007fd0: 8c07 636f 6e74 656e 7494 7d94 8c10 6170  ..content.}...ap
+00007fe0: 706c 6963 6174 696f 6e2f 6a73 6f6e 947d  plication/json.}
+00007ff0: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
+00008000: 6566 948c 2723 2f63 6f6d 706f 6e65 6e74  ef..'#/component
+00008010: 732f 7363 6865 6d61 732f 4669 6c65 5374  s/schemas/FileSt
+00008020: 7269 6e67 5265 7370 6f6e 7365 9473 7373  ringResponse.sss
+00008030: 758c 0335 3030 947d 9428 8c0b 6465 7363  u..500.}.(..desc
+00008040: 7269 7074 696f 6e94 8c0e 496e 7465 726e  ription...Intern
+00008050: 616c 2045 7272 6f72 948c 0763 6f6e 7465  al Error...conte
+00008060: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
+00008070: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
+00008080: 6d61 947d 948c 0424 7265 6694 8c27 232f  ma.}...$ref..'#/
+00008090: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+000080a0: 6173 2f46 696c 6553 7472 696e 6752 6573  as/FileStringRes
+000080b0: 706f 6e73 6594 7373 7375 7575 738c 112f  ponse.sssuuus../
+000080c0: 7633 2f66 696c 6573 2f70 6f73 7469 7473  v3/files/postits
+000080d0: 947d 948c 0367 6574 947d 9428 8c07 7375  .}...get.}.(..su
+000080e0: 6d6d 6172 7994 8c0d 4c69 7374 2050 6f73  mmary...List Pos
+000080f0: 7449 7473 2e94 8c04 7461 6773 945d 948c  tIts....tags.]..
+00008100: 0750 6f73 7449 7473 9461 8c0b 6465 7363  .PostIts.a..desc
+00008110: 7269 7074 696f 6e94 587c 0100 0052 6574  ription.X|...Ret
+00008120: 7269 6576 6520 6120 6c69 7374 206f 6620  rieve a list of 
+00008130: 616c 6c20 506f 7374 4974 732e 2020 5573  all PostIts.  Us
+00008140: 6520 2a6c 6973 7454 7970 652a 2061 6e64  e *listType* and
+00008150: 202a 7365 6c65 6374 2a20 7175 6572 7920   *select* query 
+00008160: 0a70 6172 616d 6574 6572 7320 746f 206c  .parameters to l
+00008170: 696d 6974 2072 6573 756c 7473 2e20 5175  imit results. Qu
+00008180: 6572 7920 7061 7261 6d65 7465 7220 2a6c  ery parameter *l
+00008190: 6973 7454 7970 652a 2061 6c6c 6f77 7320  istType* allows 
+000081a0: 666f 7220 6669 6c74 6572 696e 6720 0a72  for filtering .r
+000081b0: 6573 756c 7473 2062 6173 6564 206f 6e20  esults based on 
+000081c0: 6175 7468 6f72 697a 6174 696f 6e2e 204f  authorization. O
+000081d0: 7074 696f 6e73 2066 6f72 202a 6c69 7374  ptions for *list
+000081e0: 5479 7065 2a20 6172 650a 2020 2d20 2a4f  Type* are.  - *O
+000081f0: 574e 4544 2a20 496e 636c 7564 6520 6f6e  WNED* Include on
+00008200: 6c79 2069 7465 6d73 206f 776e 6564 2062  ly items owned b
+00008210: 7920 7265 7175 6573 7465 7220 2844 6566  y requester (Def
+00008220: 6175 6c74 290a 2020 2d20 2a41 4c4c 2a20  ault).  - *ALL* 
+00008230: 496e 636c 7564 6520 616c 6c20 6974 656d  Include all item
+00008240: 7320 7265 7175 6573 7465 7220 6973 2061  s requester is a
+00008250: 7574 686f 7269 7a65 6420 746f 2076 6965  uthorized to vie
+00008260: 772e 2028 5465 6e61 6e74 2061 646d 696e  w. (Tenant admin
+00008270: 7320 6361 6e20 7669 6577 2061 6c6c 2050  s can view all P
+00008280: 6f73 7449 7473 2069 6e20 7468 6569 7220  ostIts in their 
+00008290: 7465 6e61 6e74 292e 0a94 8c0b 6f70 6572  tenant).....oper
+000082a0: 6174 696f 6e49 6494 8c0b 6c69 7374 506f  ationId...listPo
+000082b0: 7374 4974 7394 8c0a 7061 7261 6d65 7465  stIts...paramete
+000082c0: 7273 945d 9428 7d94 288c 046e 616d 6594  rs.].(}.(..name.
+000082d0: 8c08 6c69 7374 5479 7065 948c 0269 6e94  ..listType...in.
+000082e0: 8c05 7175 6572 7994 8c06 7363 6865 6d61  ..query...schema
+000082f0: 947d 948c 0424 7265 6694 8c21 232f 636f  .}...$ref..!#/co
+00008300: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00008310: 2f4c 6973 7454 7970 6545 6e75 6d94 7375  /ListTypeEnum.su
+00008320: 7d94 288c 046e 616d 6594 8c05 6c69 6d69  }.(..name...limi
+00008330: 7494 8c02 696e 948c 0571 7565 7279 948c  t...in...query..
+00008340: 0b64 6573 6372 6970 7469 6f6e 948c 5b4c  .description..[L
+00008350: 696d 6974 206e 756d 6265 7220 6f66 2069  imit number of i
+00008360: 7465 6d73 2072 6574 7572 6e65 642e 2046  tems returned. F
+00008370: 6f72 2065 7861 6d70 6c65 206c 696d 6974  or example limit
+00008380: 3d31 302e 2055 7365 202d 3120 666f 7220  =10. Use -1 for 
+00008390: 756e 6c69 6d69 7465 642e 2044 6566 6175  unlimited. Defau
+000083a0: 6c74 2069 7320 3130 302e 948c 0673 6368  lt is 100....sch
+000083b0: 656d 6194 7d94 288c 0474 7970 6594 8c07  ema.}.(..type...
+000083c0: 696e 7465 6765 7294 8c07 6465 6661 756c  integer...defaul
+000083d0: 7494 4b64 7575 7d94 288c 046e 616d 6594  t.Kduu}.(..name.
+000083e0: 8c07 6f72 6465 7242 7994 8c02 696e 948c  ..orderBy...in..
+000083f0: 0571 7565 7279 948c 0b64 6573 6372 6970  .query...descrip
+00008400: 7469 6f6e 948c 6b41 7474 7269 6275 7465  tion..kAttribute
+00008410: 2066 6f72 2073 6f72 7469 6e67 2e20 4469   for sorting. Di
+00008420: 7265 6374 696f 6e20 6d61 7920 6265 2069  rection may be i
+00008430: 6e63 6c75 6465 642e 2046 6f72 2065 7861  ncluded. For exa
+00008440: 6d70 6c65 206f 7264 6572 4279 3d69 6428  mple orderBy=id(
+00008450: 6465 7363 292e 2044 6566 6175 6c74 2064  desc). Default d
+00008460: 6972 6563 7469 6f6e 2069 7320 2861 7363  irection is (asc
+00008470: 292e 948c 0673 6368 656d 6194 7d94 8c04  )....schema.}...
+00008480: 7479 7065 948c 0673 7472 696e 6794 7375  type...string.su
+00008490: 7d94 288c 046e 616d 6594 8c04 736b 6970  }.(..name...skip
+000084a0: 948c 0269 6e94 8c05 7175 6572 7994 8c0b  ...in...query...
+000084b0: 6465 7363 7269 7074 696f 6e94 8c5a 4e75  description..ZNu
+000084c0: 6d62 6572 206f 6620 6974 656d 7320 746f  mber of items to
+000084d0: 2073 6b69 702e 2055 7365 206f 6e65 206f   skip. Use one o
+000084e0: 6620 736b 6970 206f 7220 7374 6172 7441  f skip or startA
+000084f0: 6674 6572 2e20 466f 7220 6578 616d 706c  fter. For exampl
+00008500: 6520 736b 6970 3d31 302e 2044 6566 6175  e skip=10. Defau
+00008510: 6c74 2069 7320 302e 948c 0673 6368 656d  lt is 0....schem
+00008520: 6194 7d94 8c04 7479 7065 948c 0769 6e74  a.}...type...int
+00008530: 6567 6572 9473 757d 9428 8c04 6e61 6d65  eger.su}.(..name
+00008540: 948c 0a73 7461 7274 4166 7465 7294 8c02  ...startAfter...
+00008550: 696e 948c 0571 7565 7279 948c 0b64 6573  in...query...des
+00008560: 6372 6970 7469 6f6e 948c 9857 6865 7265  cription...Where
+00008570: 2074 6f20 7374 6172 7420 7768 656e 2073   to start when s
+00008580: 6f72 7469 6e67 2e20 5573 6520 6f6e 6520  orting. Use one 
+00008590: 6f66 2073 6b69 7020 6f72 2073 7461 7274  of skip or start
+000085a0: 4166 7465 722e 204d 7573 7420 616c 736f  After. Must also
+000085b0: 2073 7065 6369 6679 206f 7264 6572 4279   specify orderBy
+000085c0: 2e20 466f 7220 6578 616d 706c 652c 206c  . For example, l
+000085d0: 696d 6974 3d31 3026 6f72 6465 7242 793d  imit=10&orderBy=
+000085e0: 6964 2861 7363 2926 7374 6172 7441 6674  id(asc)&startAft
+000085f0: 6572 3d26 6c74 3b70 6f73 7469 7469 6426  er=&lt;postitid&
+00008600: 6774 3b94 8c06 7363 6865 6d61 947d 948c  gt;...schema.}..
+00008610: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+00008620: 757d 9428 8c04 6e61 6d65 948c 0673 656c  u}.(..name...sel
+00008630: 6563 7494 8c02 696e 948c 0571 7565 7279  ect...in...query
+00008640: 948c 0b64 6573 6372 6970 7469 6f6e 948c  ...description..
+00008650: 9f4c 6973 7420 6f66 2061 7474 7269 6275  .List of attribu
+00008660: 7465 7320 746f 2062 6520 696e 636c 7564  tes to be includ
+00008670: 6564 2061 7320 7061 7274 206f 6620 6561  ed as part of ea
+00008680: 6368 2072 6573 756c 7420 6974 656d 2e20  ch result item. 
+00008690: 4b65 7977 6f72 6473 202a 616c 6c41 7474  Keywords *allAtt
+000086a0: 7269 6275 7465 732a 2061 6e64 202a 7375  ributes* and *su
+000086b0: 6d6d 6172 7941 7474 7269 6275 7465 732a  mmaryAttributes*
+000086c0: 2061 7265 2073 7570 706f 7274 6564 2e20   are supported. 
+000086d0: 466f 7220 6578 616d 706c 6520 7365 6c65  For example sele
+000086e0: 6374 3d69 642c 6f77 6e65 722c 7061 7468  ct=id,owner,path
+000086f0: 948c 0673 6368 656d 6194 7d94 288c 0474  ...schema.}.(..t
+00008700: 7970 6594 8c06 7374 7269 6e67 948c 0764  ype...string...d
+00008710: 6566 6175 6c74 948c 1173 756d 6d61 7279  efault...summary
+00008720: 4174 7472 6962 7574 6573 9475 7565 8c09  Attributes.uue..
+00008730: 7265 7370 6f6e 7365 7394 7d94 288c 0332  responses.}.(..2
+00008740: 3030 947d 9428 8c0b 6465 7363 7269 7074  00.}.(..descript
+00008750: 696f 6e94 8c08 5375 6363 6573 732e 948c  ion...Success...
+00008760: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
+00008770: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
+00008780: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
+00008790: 6694 8c27 232f 636f 6d70 6f6e 656e 7473  f..'#/components
+000087a0: 2f73 6368 656d 6173 2f50 6f73 7449 744c  /schemas/PostItL
+000087b0: 6973 7452 6573 706f 6e73 6594 7373 7375  istResponse.sssu
+000087c0: 8c03 3430 3094 7d94 288c 0b64 6573 6372  ..400.}.(..descr
+000087d0: 6970 7469 6f6e 948c 0b42 6164 2052 6571  iption...Bad Req
+000087e0: 7565 7374 948c 0763 6f6e 7465 6e74 947d  uest...content.}
+000087f0: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
+00008800: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
+00008810: 948c 0424 7265 6694 8c27 232f 636f 6d70  ...$ref..'#/comp
+00008820: 6f6e 656e 7473 2f73 6368 656d 6173 2f46  onents/schemas/F
+00008830: 696c 6553 7472 696e 6752 6573 706f 6e73  ileStringRespons
+00008840: 6594 7373 7375 8c03 3430 3194 7d94 288c  e.sssu..401.}.(.
+00008850: 0b64 6573 6372 6970 7469 6f6e 948c 114e  .description...N
+00008860: 6f74 2041 7574 6865 6e74 6963 6174 6564  ot Authenticated
+00008870: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
+00008880: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
+00008890: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
+000088a0: 7265 6694 8c27 232f 636f 6d70 6f6e 656e  ref..'#/componen
+000088b0: 7473 2f73 6368 656d 6173 2f46 696c 6553  ts/schemas/FileS
+000088c0: 7472 696e 6752 6573 706f 6e73 6594 7373  tringResponse.ss
+000088d0: 7375 8c03 3430 3394 7d94 288c 0b64 6573  su..403.}.(..des
+000088e0: 6372 6970 7469 6f6e 948c 1150 6572 6d69  cription...Permi
+000088f0: 7373 696f 6e20 4465 6e69 6564 948c 0763  ssion Denied...c
+00008900: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
+00008910: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
+00008920: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
+00008930: 8c27 232f 636f 6d70 6f6e 656e 7473 2f73  .'#/components/s
+00008940: 6368 656d 6173 2f46 696c 6553 7472 696e  chemas/FileStrin
+00008950: 6752 6573 706f 6e73 6594 7373 7375 8c03  gResponse.sssu..
+00008960: 3430 3494 7d94 288c 0b64 6573 6372 6970  404.}.(..descrip
+00008970: 7469 6f6e 948c 094e 6f74 2046 6f75 6e64  tion...Not Found
+00008980: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
+00008990: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
+000089a0: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
+000089b0: 7265 6694 8c27 232f 636f 6d70 6f6e 656e  ref..'#/componen
+000089c0: 7473 2f73 6368 656d 6173 2f46 696c 6553  ts/schemas/FileS
+000089d0: 7472 696e 6752 6573 706f 6e73 6594 7373  tringResponse.ss
+000089e0: 7375 8c03 3530 3094 7d94 288c 0b64 6573  su..500.}.(..des
+000089f0: 6372 6970 7469 6f6e 948c 0e49 6e74 6572  cription...Inter
+00008a00: 6e61 6c20 4572 726f 7294 8c07 636f 6e74  nal Error...cont
+00008a10: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
+00008a20: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
+00008a30: 656d 6194 7d94 8c04 2472 6566 948c 2723  ema.}...$ref..'#
+00008a40: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+00008a50: 6d61 732f 4669 6c65 5374 7269 6e67 5265  mas/FileStringRe
+00008a60: 7370 6f6e 7365 9473 7373 7575 7573 8c1c  sponse.sssuuus..
+00008a70: 2f76 332f 6669 6c65 732f 706f 7374 6974  /v3/files/postit
+00008a80: 732f 7b70 6f73 7469 7449 647d 947d 9428  s/{postitId}.}.(
+00008a90: 8c03 6765 7494 7d94 288c 0773 756d 6d61  ..get.}.(..summa
+00008aa0: 7279 948c 0b47 6574 2050 6f73 7449 742e  ry...Get PostIt.
+00008ab0: 948c 0474 6167 7394 5d94 8c07 506f 7374  ...tags.]...Post
+00008ac0: 4974 7394 618c 0b64 6573 6372 6970 7469  Its.a..descripti
+00008ad0: 6f6e 948c 3647 6574 2061 2073 696e 676c  on..6Get a singl
+00008ae0: 6520 506f 7374 4974 2e20 2054 6869 7320  e PostIt.  This 
+00008af0: 646f 6573 206e 6f74 2072 6564 6565 6d20  does not redeem 
+00008b00: 7468 6520 506f 7374 4974 2e94 8c0b 6f70  the PostIt....op
+00008b10: 6572 6174 696f 6e49 6494 8c09 6765 7450  erationId...getP
+00008b20: 6f73 7449 7494 8c0a 7061 7261 6d65 7465  ostIt...paramete
+00008b30: 7273 945d 947d 9428 8c04 6e61 6d65 948c  rs.].}.(..name..
+00008b40: 0870 6f73 7469 7449 6494 8c02 696e 948c  .postitId...in..
+00008b50: 0470 6174 6894 8c08 7265 7175 6972 6564  .path...required
+00008b60: 9488 8c06 7363 6865 6d61 947d 9428 8c04  ....schema.}.(..
+00008b70: 7479 7065 948c 0673 7472 696e 6794 8c06  type...string...
+00008b80: 666f 726d 6174 948c 0475 7569 6494 7575  format...uuid.uu
+00008b90: 618c 0972 6573 706f 6e73 6573 947d 9428  a..responses.}.(
+00008ba0: 8c03 3230 3094 7d94 288c 0b64 6573 6372  ..200.}.(..descr
+00008bb0: 6970 7469 6f6e 948c 0853 7563 6365 7373  iption...Success
+00008bc0: 2e94 8c07 636f 6e74 656e 7494 7d94 8c10  ....content.}...
+00008bd0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+00008be0: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
+00008bf0: 2472 6566 948c 2323 2f63 6f6d 706f 6e65  $ref..##/compone
+00008c00: 6e74 732f 7363 6865 6d61 732f 506f 7374  nts/schemas/Post
+00008c10: 4974 5265 7370 6f6e 7365 9473 7373 758c  ItResponse.sssu.
+00008c20: 0334 3030 947d 9428 8c0b 6465 7363 7269  .400.}.(..descri
+00008c30: 7074 696f 6e94 8c0b 4261 6420 5265 7175  ption...Bad Requ
+00008c40: 6573 7494 8c07 636f 6e74 656e 7494 7d94  est...content.}.
+00008c50: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
+00008c60: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
+00008c70: 8c04 2472 6566 948c 2723 2f63 6f6d 706f  ..$ref..'#/compo
+00008c80: 6e65 6e74 732f 7363 6865 6d61 732f 4669  nents/schemas/Fi
+00008c90: 6c65 5374 7269 6e67 5265 7370 6f6e 7365  leStringResponse
+00008ca0: 9473 7373 758c 0334 3031 947d 9428 8c0b  .sssu..401.}.(..
+00008cb0: 6465 7363 7269 7074 696f 6e94 8c11 4e6f  description...No
+00008cc0: 7420 4175 7468 656e 7469 6361 7465 6494  t Authenticated.
+00008cd0: 8c07 636f 6e74 656e 7494 7d94 8c10 6170  ..content.}...ap
+00008ce0: 706c 6963 6174 696f 6e2f 6a73 6f6e 947d  plication/json.}
+00008cf0: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
+00008d00: 6566 948c 2723 2f63 6f6d 706f 6e65 6e74  ef..'#/component
+00008d10: 732f 7363 6865 6d61 732f 4669 6c65 5374  s/schemas/FileSt
+00008d20: 7269 6e67 5265 7370 6f6e 7365 9473 7373  ringResponse.sss
+00008d30: 758c 0334 3033 947d 9428 8c0b 6465 7363  u..403.}.(..desc
+00008d40: 7269 7074 696f 6e94 8c11 5065 726d 6973  ription...Permis
+00008d50: 7369 6f6e 2044 656e 6965 6494 8c07 636f  sion Denied...co
+00008d60: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
+00008d70: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
+00008d80: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
+00008d90: 2723 2f63 6f6d 706f 6e65 6e74 732f 7363  '#/components/sc
+00008da0: 6865 6d61 732f 4669 6c65 5374 7269 6e67  hemas/FileString
+00008db0: 5265 7370 6f6e 7365 9473 7373 758c 0334  Response.sssu..4
+00008dc0: 3034 947d 9428 8c0b 6465 7363 7269 7074  04.}.(..descript
+00008dd0: 696f 6e94 8c09 4e6f 7420 466f 756e 6494  ion...Not Found.
+00008de0: 8c07 636f 6e74 656e 7494 7d94 8c10 6170  ..content.}...ap
+00008df0: 706c 6963 6174 696f 6e2f 6a73 6f6e 947d  plication/json.}
+00008e00: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
+00008e10: 6566 948c 2723 2f63 6f6d 706f 6e65 6e74  ef..'#/component
+00008e20: 732f 7363 6865 6d61 732f 4669 6c65 5374  s/schemas/FileSt
+00008e30: 7269 6e67 5265 7370 6f6e 7365 9473 7373  ringResponse.sss
+00008e40: 758c 0335 3030 947d 9428 8c0b 6465 7363  u..500.}.(..desc
+00008e50: 7269 7074 696f 6e94 8c0e 496e 7465 726e  ription...Intern
+00008e60: 616c 2045 7272 6f72 948c 0763 6f6e 7465  al Error...conte
+00008e70: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
+00008e80: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
+00008e90: 6d61 947d 948c 0424 7265 6694 8c27 232f  ma.}...$ref..'#/
+00008ea0: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+00008eb0: 6173 2f46 696c 6553 7472 696e 6752 6573  as/FileStringRes
+00008ec0: 706f 6e73 6594 7373 7375 7575 8c05 7061  ponse.sssuuu..pa
+00008ed0: 7463 6894 7d94 288c 0773 756d 6d61 7279  tch.}.(..summary
+00008ee0: 948c 0f4d 6f64 6966 7920 6120 506f 7374  ...Modify a Post
+00008ef0: 4974 948c 0474 6167 7394 5d94 8c07 506f  It...tags.]...Po
+00008f00: 7374 4974 7394 618c 0b64 6573 6372 6970  stIts.a..descrip
+00008f10: 7469 6f6e 948c 2555 7064 6174 6520 7365  tion..%Update se
+00008f20: 6c65 6374 6564 2066 6965 6c64 7320 6f66  lected fields of
+00008f30: 2061 2050 6f73 7449 742e 200a 948c 0b6f   a PostIt. ....o
+00008f40: 7065 7261 7469 6f6e 4964 948c 0c75 7064  perationId...upd
+00008f50: 6174 6550 6f73 7449 7494 8c0a 7061 7261  atePostIt...para
+00008f60: 6d65 7465 7273 945d 947d 9428 8c04 6e61  meters.].}.(..na
+00008f70: 6d65 948c 0870 6f73 7469 7449 6494 8c02  me...postitId...
+00008f80: 696e 948c 0470 6174 6894 8c08 7265 7175  in...path...requ
+00008f90: 6972 6564 9488 8c06 7363 6865 6d61 947d  ired....schema.}
+00008fa0: 9428 8c04 7479 7065 948c 0673 7472 696e  .(..type...strin
+00008fb0: 6794 8c06 666f 726d 6174 948c 0475 7569  g...format...uui
+00008fc0: 6494 7575 618c 0b72 6571 7565 7374 426f  d.uua..requestBo
+00008fd0: 6479 947d 9428 8c08 7265 7175 6972 6564  dy.}.(..required
+00008fe0: 9488 8c0b 6465 7363 7269 7074 696f 6e94  ....description.
+00008ff0: 8c34 4120 4a53 4f4e 2064 6f63 756d 656e  .4A JSON documen
+00009000: 7420 6465 7363 7269 6269 6e67 2074 6865  t describing the
+00009010: 2050 6f73 7449 7420 746f 2062 6520 7570   PostIt to be up
+00009020: 6461 7465 642e 948c 0763 6f6e 7465 6e74  dated....content
+00009030: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
+00009040: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
+00009050: 947d 948c 0424 7265 6694 8c28 232f 636f  .}...$ref..(#/co
+00009060: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00009070: 2f55 7064 6174 6550 6f73 7449 7452 6571  /UpdatePostItReq
+00009080: 7565 7374 9473 7373 758c 0972 6573 706f  uest.sssu..respo
+00009090: 6e73 6573 947d 9428 8c03 3230 3094 7d94  nses.}.(..200.}.
+000090a0: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
+000090b0: 0853 7563 6365 7373 2e94 8c07 636f 6e74  .Success....cont
+000090c0: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
+000090d0: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
+000090e0: 656d 6194 7d94 8c04 2472 6566 948c 2323  ema.}...$ref..##
+000090f0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+00009100: 6d61 732f 506f 7374 4974 5265 7370 6f6e  mas/PostItRespon
+00009110: 7365 9473 7373 758c 0334 3030 947d 9428  se.sssu..400.}.(
+00009120: 8c0b 6465 7363 7269 7074 696f 6e94 8c0b  ..description...
+00009130: 4261 6420 5265 7175 6573 7494 8c07 636f  Bad Request...co
+00009140: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
+00009150: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
+00009160: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
+00009170: 2723 2f63 6f6d 706f 6e65 6e74 732f 7363  '#/components/sc
+00009180: 6865 6d61 732f 4669 6c65 5374 7269 6e67  hemas/FileString
+00009190: 5265 7370 6f6e 7365 9473 7373 758c 0334  Response.sssu..4
+000091a0: 3031 947d 9428 8c0b 6465 7363 7269 7074  01.}.(..descript
+000091b0: 696f 6e94 8c11 4e6f 7420 4175 7468 656e  ion...Not Authen
+000091c0: 7469 6361 7465 6494 8c07 636f 6e74 656e  ticated...conten
+000091d0: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
+000091e0: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
+000091f0: 6194 7d94 8c04 2472 6566 948c 2723 2f63  a.}...$ref..'#/c
+00009200: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+00009210: 732f 4669 6c65 5374 7269 6e67 5265 7370  s/FileStringResp
+00009220: 6f6e 7365 9473 7373 758c 0334 3033 947d  onse.sssu..403.}
+00009230: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
+00009240: 8c11 5065 726d 6973 7369 6f6e 2044 656e  ..Permission Den
+00009250: 6965 6494 8c07 636f 6e74 656e 7494 7d94  ied...content.}.
+00009260: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
+00009270: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
+00009280: 8c04 2472 6566 948c 2723 2f63 6f6d 706f  ..$ref..'#/compo
+00009290: 6e65 6e74 732f 7363 6865 6d61 732f 4669  nents/schemas/Fi
+000092a0: 6c65 5374 7269 6e67 5265 7370 6f6e 7365  leStringResponse
+000092b0: 9473 7373 758c 0334 3034 947d 9428 8c0b  .sssu..404.}.(..
+000092c0: 6465 7363 7269 7074 696f 6e94 8c09 4e6f  description...No
+000092d0: 7420 466f 756e 6494 8c07 636f 6e74 656e  t Found...conten
+000092e0: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
+000092f0: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
+00009300: 6194 7d94 8c04 2472 6566 948c 2723 2f63  a.}...$ref..'#/c
+00009310: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+00009320: 732f 4669 6c65 5374 7269 6e67 5265 7370  s/FileStringResp
+00009330: 6f6e 7365 9473 7373 758c 0335 3030 947d  onse.sssu..500.}
+00009340: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
+00009350: 8c0e 496e 7465 726e 616c 2045 7272 6f72  ..Internal Error
+00009360: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
+00009370: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
+00009380: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
+00009390: 7265 6694 8c27 232f 636f 6d70 6f6e 656e  ref..'#/componen
+000093a0: 7473 2f73 6368 656d 6173 2f46 696c 6553  ts/schemas/FileS
+000093b0: 7472 696e 6752 6573 706f 6e73 6594 7373  tringResponse.ss
+000093c0: 7375 7575 8c06 6465 6c65 7465 947d 9428  suuu..delete.}.(
+000093d0: 8c07 7375 6d6d 6172 7994 8c0f 4465 6c65  ..summary...Dele
+000093e0: 7465 2061 2050 6f73 7449 7494 8c04 7461  te a PostIt...ta
+000093f0: 6773 945d 948c 0750 6f73 7449 7473 9461  gs.]...PostIts.a
+00009400: 8c0b 6465 7363 7269 7074 696f 6e94 8c10  ..description...
+00009410: 4465 6c65 7465 2061 2050 6f73 7449 742e  Delete a PostIt.
+00009420: 948c 0b6f 7065 7261 7469 6f6e 4964 948c  ...operationId..
+00009430: 0c64 656c 6574 6550 6f73 7449 7494 8c0a  .deletePostIt...
+00009440: 7061 7261 6d65 7465 7273 945d 947d 9428  parameters.].}.(
+00009450: 8c04 6e61 6d65 948c 0870 6f73 7469 7449  ..name...postitI
+00009460: 6494 8c02 696e 948c 0470 6174 6894 8c08  d...in...path...
+00009470: 7265 7175 6972 6564 9488 8c06 7363 6865  required....sche
+00009480: 6d61 947d 9428 8c04 7479 7065 948c 0673  ma.}.(..type...s
+00009490: 7472 696e 6794 8c06 666f 726d 6174 948c  tring...format..
+000094a0: 0475 7569 6494 7575 618c 0972 6573 706f  .uuid.uua..respo
+000094b0: 6e73 6573 947d 9428 8c03 3230 3094 7d94  nses.}.(..200.}.
+000094c0: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
+000094d0: 0853 7563 6365 7373 2e94 8c07 636f 6e74  .Success....cont
+000094e0: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
+000094f0: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
+00009500: 656d 6194 7d94 8c04 2472 6566 948c 2423  ema.}...$ref..$#
+00009510: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+00009520: 6d61 732f 5265 7370 4368 616e 6765 436f  mas/RespChangeCo
+00009530: 756e 7494 7373 7375 8c03 3430 3094 7d94  unt.sssu..400.}.
+00009540: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
+00009550: 0b42 6164 2052 6571 7565 7374 948c 0763  .Bad Request...c
+00009560: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
+00009570: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
+00009580: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
+00009590: 8c27 232f 636f 6d70 6f6e 656e 7473 2f73  .'#/components/s
+000095a0: 6368 656d 6173 2f46 696c 6553 7472 696e  chemas/FileStrin
+000095b0: 6752 6573 706f 6e73 6594 7373 7375 8c03  gResponse.sssu..
+000095c0: 3430 3194 7d94 288c 0b64 6573 6372 6970  401.}.(..descrip
+000095d0: 7469 6f6e 948c 114e 6f74 2041 7574 6865  tion...Not Authe
+000095e0: 6e74 6963 6174 6564 948c 0763 6f6e 7465  nticated...conte
+000095f0: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
+00009600: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
+00009610: 6d61 947d 948c 0424 7265 6694 8c27 232f  ma.}...$ref..'#/
+00009620: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+00009630: 6173 2f46 696c 6553 7472 696e 6752 6573  as/FileStringRes
+00009640: 706f 6e73 6594 7373 7375 8c03 3430 3394  ponse.sssu..403.
+00009650: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
+00009660: 948c 1150 6572 6d69 7373 696f 6e20 4465  ...Permission De
+00009670: 6e69 6564 948c 0763 6f6e 7465 6e74 947d  nied...content.}
+00009680: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
+00009690: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
+000096a0: 948c 0424 7265 6694 8c27 232f 636f 6d70  ...$ref..'#/comp
+000096b0: 6f6e 656e 7473 2f73 6368 656d 6173 2f46  onents/schemas/F
+000096c0: 696c 6553 7472 696e 6752 6573 706f 6e73  ileStringRespons
+000096d0: 6594 7373 7375 8c03 3430 3494 7d94 288c  e.sssu..404.}.(.
+000096e0: 0b64 6573 6372 6970 7469 6f6e 948c 094e  .description...N
+000096f0: 6f74 2046 6f75 6e64 948c 0763 6f6e 7465  ot Found...conte
+00009700: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
+00009710: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
+00009720: 6d61 947d 948c 0424 7265 6694 8c27 232f  ma.}...$ref..'#/
+00009730: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+00009740: 6173 2f46 696c 6553 7472 696e 6752 6573  as/FileStringRes
+00009750: 706f 6e73 6594 7373 7375 8c03 3530 3094  ponse.sssu..500.
+00009760: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
+00009770: 948c 0e49 6e74 6572 6e61 6c20 4572 726f  ...Internal Erro
+00009780: 7294 8c07 636f 6e74 656e 7494 7d94 8c10  r...content.}...
+00009790: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+000097a0: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
+000097b0: 2472 6566 948c 2723 2f63 6f6d 706f 6e65  $ref..'#/compone
+000097c0: 6e74 732f 7363 6865 6d61 732f 4669 6c65  nts/schemas/File
+000097d0: 5374 7269 6e67 5265 7370 6f6e 7365 9473  StringResponse.s
+000097e0: 7373 7575 7575 8c23 2f76 332f 6669 6c65  ssuuuu.#/v3/file
+000097f0: 732f 706f 7374 6974 732f 7265 6465 656d  s/postits/redeem
+00009800: 2f7b 706f 7374 6974 4964 7d94 7d94 8c03  /{postitId}.}...
+00009810: 6765 7494 7d94 288c 0773 756d 6d61 7279  get.}.(..summary
+00009820: 948c 0e52 6564 6565 6d20 506f 7374 4974  ...Redeem PostIt
+00009830: 2e94 8c04 7461 6773 945d 948c 0750 6f73  ....tags.]...Pos
+00009840: 7449 7473 9461 8c0b 6465 7363 7269 7074  tIts.a..descript
+00009850: 696f 6e94 58be 0100 0052 6564 6565 6d20  ion.X....Redeem 
+00009860: 6120 506f 7374 4974 2e20 2054 6869 7320  a PostIt.  This 
+00009870: 7769 6c6c 2072 6574 7572 6e20 7468 6520  will return the 
+00009880: 6669 6c65 2074 6861 7420 6973 2070 6f69  file that is poi
+00009890: 6e74 6564 2074 6f20 6279 2074 6865 2050  nted to by the P
+000098a0: 6f73 7449 742e 2020 4e6f 2061 7574 6865  ostIt.  No authe
+000098b0: 6e74 6963 6174 696f 6e20 6973 2072 6571  ntication is req
+000098c0: 7569 7265 642e 2049 6620 7468 6520 2a7a  uired. If the *z
+000098d0: 6970 2a20 7175 6572 7920 7061 7261 6d20  ip* query param 
+000098e0: 6973 2070 726f 7669 6465 6420 6974 2063  is provided it c
+000098f0: 6f6e 7472 6f6c 7320 6966 2074 6865 2063  ontrols if the c
+00009900: 6f6e 7465 6e74 2069 7320 7a69 7070 6564  ontent is zipped
+00009910: 206f 7220 6e6f 742e 2020 4966 207a 6970   or not.  If zip
+00009920: 2069 7320 6e6f 7420 7072 6f76 6964 6564   is not provided
+00009930: 2c20 6974 2064 6566 6175 6c74 7320 746f  , it defaults to
+00009940: 2066 616c 7365 2075 6e6c 6573 7320 7468   false unless th
+00009950: 6520 7061 7468 2070 6f69 6e74 6564 2074  e path pointed t
+00009960: 6f20 6279 2074 6865 2050 6f73 7449 7420  o by the PostIt 
+00009970: 6973 2061 2064 6972 6563 746f 7279 2e20  is a directory. 
+00009980: 2049 6e20 7468 6520 6361 7365 206f 6620   In the case of 
+00009990: 6120 6469 7265 6374 6f72 792c 2074 6865  a directory, the
+000099a0: 2064 6566 6175 6c74 2069 7320 7a69 703d   default is zip=
+000099b0: 7472 7565 2e20 4469 7265 6374 6f72 6965  true. Directorie
+000099c0: 7320 6d75 7374 2062 7920 7265 6465 656d  s must by redeem
+000099d0: 6564 2069 6e20 7a69 7070 6564 2066 6f72  ed in zipped for
+000099e0: 6d61 742c 2073 6f20 6569 7468 6572 2061  mat, so either a
+000099f0: 6363 6570 7420 7468 6520 6465 6661 756c  ccept the defaul
+00009a00: 742c 206f 7220 7370 6563 6966 7920 7a69  t, or specify zi
+00009a10: 703d 7472 7565 2e94 8c0b 6f70 6572 6174  p=true....operat
+00009a20: 696f 6e49 6494 8c0c 7265 6465 656d 506f  ionId...redeemPo
+00009a30: 7374 4974 948c 0a70 6172 616d 6574 6572  stIt...parameter
+00009a40: 7394 5d94 287d 9428 8c04 6e61 6d65 948c  s.].(}.(..name..
+00009a50: 0870 6f73 7469 7449 6494 8c02 696e 948c  .postitId...in..
+00009a60: 0470 6174 6894 8c08 7265 7175 6972 6564  .path...required
+00009a70: 9488 8c06 7363 6865 6d61 947d 9428 8c04  ....schema.}.(..
+00009a80: 7479 7065 948c 0673 7472 696e 6794 8c06  type...string...
+00009a90: 666f 726d 6174 948c 0475 7569 6494 7575  format...uuid.uu
+00009aa0: 7d94 288c 046e 616d 6594 8c03 7a69 7094  }.(..name...zip.
+00009ab0: 8c02 696e 948c 0571 7565 7279 948c 0b64  ..in...query...d
+00009ac0: 6573 6372 6970 7469 6f6e 948c b649 6e64  escription...Ind
+00009ad0: 6963 6174 6573 2061 207a 6970 206f 7574  icates a zip out
+00009ae0: 7075 7420 7374 7265 616d 2073 686f 756c  put stream shoul
+00009af0: 6420 6265 2070 726f 7669 6465 642e 2020  d be provided.  
+00009b00: 4966 207a 6970 2069 7320 6e6f 7420 7072  If zip is not pr
+00009b10: 6f76 6964 6564 2069 7420 6465 6661 756c  ovided it defaul
+00009b20: 7473 2074 6f20 6661 6c73 6520 756e 6c65  ts to false unle
+00009b30: 7373 2074 6865 2070 6174 6820 6973 2061  ss the path is a
+00009b40: 2064 6972 6563 746f 7279 2e20 2049 6e20   directory.  In 
+00009b50: 7468 6520 6361 7365 206f 6620 6120 6469  the case of a di
+00009b60: 7265 6374 6f72 7920 7468 6520 636f 6e74  rectory the cont
+00009b70: 656e 7420 7769 6c6c 2062 6520 7a69 7070  ent will be zipp
+00009b80: 6564 2e94 8c06 7363 6865 6d61 947d 948c  ed....schema.}..
+00009b90: 0474 7970 6594 8c07 626f 6f6c 6561 6e94  .type...boolean.
+00009ba0: 738c 0765 7861 6d70 6c65 9489 757d 9428  s..example..u}.(
+00009bb0: 8c04 6e61 6d65 948c 0864 6f77 6e6c 6f61  ..name...downloa
+00009bc0: 6494 8c02 696e 948c 0571 7565 7279 948c  d...in...query..
+00009bd0: 0b64 6573 6372 6970 7469 6f6e 948c ec49  .description...I
+00009be0: 6620 7365 7420 746f 2074 7275 652c 2074  f set to true, t
+00009bf0: 6869 7320 7769 6c6c 2066 6f72 6365 2061  his will force a
+00009c00: 2062 726f 7773 6572 2074 6f20 696e 6974   browser to init
+00009c10: 6961 7465 2061 2066 696c 6520 646f 776e  iate a file down
+00009c20: 6c6f 6164 2e20 2049 6620 7365 7420 746f  load.  If set to
+00009c30: 2066 616c 7365 2c20 7468 6520 636f 6e74   false, the cont
+00009c40: 656e 742d 6469 7370 6f73 6974 696f 6e20  ent-disposition 
+00009c50: 6865 6164 6572 2077 696c 6c20 6265 2073  header will be s
+00009c60: 6574 2074 6f20 696e 6c69 6e65 2063 6175  et to inline cau
+00009c70: 7369 6e67 2074 6865 2062 726f 7773 6572  sing the browser
+00009c80: 2074 6f20 7265 6e64 6572 2074 6865 2064   to render the d
+00009c90: 6f63 756d 656e 742e 2020 4966 2064 6f77  ocument.  If dow
+00009ca0: 6e6c 6f61 6420 6973 206e 6f74 2070 726f  nload is not pro
+00009cb0: 7669 6465 6420 6974 2064 6566 6175 6c74  vided it default
+00009cc0: 7320 746f 2066 616c 7365 2e94 8c06 7363  s to false....sc
+00009cd0: 6865 6d61 947d 948c 0474 7970 6594 8c07  hema.}...type...
+00009ce0: 626f 6f6c 6561 6e94 738c 0765 7861 6d70  boolean.s..examp
+00009cf0: 6c65 9489 7565 8c09 7265 7370 6f6e 7365  le..ue..response
+00009d00: 7394 7d94 288c 0332 3030 947d 948c 0b64  s.}.(..200.}...d
+00009d10: 6573 6372 6970 7469 6f6e 948c 0853 7563  escription...Suc
+00009d20: 6365 7373 2e94 738c 0334 3030 947d 9428  cess..s..400.}.(
+00009d30: 8c0b 6465 7363 7269 7074 696f 6e94 8c0b  ..description...
+00009d40: 4261 6420 5265 7175 6573 7494 8c07 636f  Bad Request...co
+00009d50: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
+00009d60: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
+00009d70: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
+00009d80: 2723 2f63 6f6d 706f 6e65 6e74 732f 7363  '#/components/sc
+00009d90: 6865 6d61 732f 4669 6c65 5374 7269 6e67  hemas/FileString
+00009da0: 5265 7370 6f6e 7365 9473 7373 758c 0334  Response.sssu..4
+00009db0: 3033 947d 9428 8c0b 6465 7363 7269 7074  03.}.(..descript
+00009dc0: 696f 6e94 8c11 5065 726d 6973 7369 6f6e  ion...Permission
+00009dd0: 2044 656e 6965 6494 8c07 636f 6e74 656e   Denied...conten
+00009de0: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
+00009df0: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
+00009e00: 6194 7d94 8c04 2472 6566 948c 2723 2f63  a.}...$ref..'#/c
+00009e10: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+00009e20: 732f 4669 6c65 5374 7269 6e67 5265 7370  s/FileStringResp
+00009e30: 6f6e 7365 9473 7373 758c 0334 3034 947d  onse.sssu..404.}
+00009e40: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
+00009e50: 8c09 4e6f 7420 466f 756e 6494 8c07 636f  ..Not Found...co
+00009e60: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
+00009e70: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
+00009e80: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
+00009e90: 2723 2f63 6f6d 706f 6e65 6e74 732f 7363  '#/components/sc
+00009ea0: 6865 6d61 732f 4669 6c65 5374 7269 6e67  hemas/FileString
+00009eb0: 5265 7370 6f6e 7365 9473 7373 758c 0335  Response.sssu..5
+00009ec0: 3030 947d 9428 8c0b 6465 7363 7269 7074  00.}.(..descript
+00009ed0: 696f 6e94 8c0e 496e 7465 726e 616c 2045  ion...Internal E
+00009ee0: 7272 6f72 948c 0763 6f6e 7465 6e74 947d  rror...content.}
+00009ef0: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
+00009f00: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
+00009f10: 948c 0424 7265 6694 8c27 232f 636f 6d70  ...$ref..'#/comp
+00009f20: 6f6e 656e 7473 2f73 6368 656d 6173 2f46  onents/schemas/F
+00009f30: 696c 6553 7472 696e 6752 6573 706f 6e73  ileStringRespons
+00009f40: 6594 7373 7375 7575 7375 8c0a 636f 6d70  e.sssuuusu..comp
+00009f50: 6f6e 656e 7473 947d 948c 0773 6368 656d  onents.}...schem
+00009f60: 6173 947d 9428 8c0f 4865 6164 6572 4279  as.}.(..HeaderBy
+00009f70: 7465 5261 6e67 6594 7d94 288c 0474 7970  teRange.}.(..typ
+00009f80: 6594 8c06 6f62 6a65 6374 948c 0a70 726f  e...object...pro
+00009f90: 7065 7274 6965 7394 7d94 288c 036d 696e  perties.}.(..min
+00009fa0: 947d 9428 8c04 7479 7065 948c 0769 6e74  .}.(..type...int
+00009fb0: 6567 6572 948c 0666 6f72 6d61 7494 8c05  eger...format...
+00009fc0: 696e 7436 3494 758c 036d 6178 947d 9428  int64.u..max.}.(
+00009fd0: 8c04 7479 7065 948c 0769 6e74 6567 6572  ..type...integer
+00009fe0: 948c 0666 6f72 6d61 7494 8c05 696e 7436  ...format...int6
+00009ff0: 3494 7575 758c 0846 696c 6549 6e66 6f94  4.uuu..FileInfo.
+0000a000: 7d94 288c 0474 7970 6594 8c06 6f62 6a65  }.(..type...obje
+0000a010: 6374 948c 0a70 726f 7065 7274 6965 7394  ct...properties.
+0000a020: 7d94 288c 086d 696d 6554 7970 6594 7d94  }.(..mimeType.}.
+0000a030: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000a040: 738c 0474 7970 6594 7d94 8c04 7479 7065  s..type.}...type
+0000a050: 948c 0673 7472 696e 6794 738c 056f 776e  ...string.s..own
+0000a060: 6572 947d 948c 0474 7970 6594 8c06 7374  er.}...type...st
+0000a070: 7269 6e67 9473 8c05 6772 6f75 7094 7d94  ring.s..group.}.
+0000a080: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000a090: 738c 116e 6174 6976 6550 6572 6d69 7373  s..nativePermiss
+0000a0a0: 696f 6e73 947d 948c 0474 7970 6594 8c06  ions.}...type...
+0000a0b0: 7374 7269 6e67 9473 8c03 7572 6c94 7d94  string.s..url.}.
+0000a0c0: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000a0d0: 738c 0c6c 6173 744d 6f64 6966 6965 6494  s..lastModified.
+0000a0e0: 7d94 288c 0474 7970 6594 8c06 7374 7269  }.(..type...stri
+0000a0f0: 6e67 948c 0666 6f72 6d61 7494 8c09 6461  ng...format...da
+0000a100: 7465 2d74 696d 6594 758c 046e 616d 6594  te-time.u..name.
+0000a110: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+0000a120: 6794 738c 0470 6174 6894 7d94 8c04 7479  g.s..path.}...ty
+0000a130: 7065 948c 0673 7472 696e 6794 738c 0473  pe...string.s..s
+0000a140: 697a 6594 7d94 288c 0474 7970 6594 8c07  ize.}.(..type...
+0000a150: 696e 7465 6765 7294 8c0b 6465 7363 7269  integer...descri
+0000a160: 7074 696f 6e94 8c0a 7369 7a65 2069 6e20  ption...size in 
+0000a170: 6b42 948c 0666 6f72 6d61 7494 8c05 696e  kB...format...in
+0000a180: 7436 3494 7575 758c 0c46 696c 6553 7461  t64.uuu..FileSta
+0000a190: 7449 6e66 6f94 7d94 288c 0474 7970 6594  tInfo.}.(..type.
+0000a1a0: 8c06 6f62 6a65 6374 948c 0a70 726f 7065  ..object...prope
+0000a1b0: 7274 6965 7394 7d94 288c 0c61 6273 6f6c  rties.}.(..absol
+0000a1c0: 7574 6550 6174 6894 7d94 8c04 7479 7065  utePath.}...type
+0000a1d0: 948c 0673 7472 696e 6794 738c 0375 6964  ...string.s..uid
+0000a1e0: 947d 9428 8c04 7479 7065 948c 0769 6e74  .}.(..type...int
+0000a1f0: 6567 6572 948c 0666 6f72 6d61 7494 8c05  eger...format...
+0000a200: 696e 7433 3294 758c 0367 6964 947d 9428  int32.u..gid.}.(
+0000a210: 8c04 7479 7065 948c 0769 6e74 6567 6572  ..type...integer
+0000a220: 948c 0666 6f72 6d61 7494 8c05 696e 7433  ...format...int3
+0000a230: 3294 758c 0473 697a 6594 7d94 288c 0474  2.u..size.}.(..t
+0000a240: 7970 6594 8c07 696e 7465 6765 7294 8c06  ype...integer...
+0000a250: 666f 726d 6174 948c 0569 6e74 3634 9475  format...int64.u
+0000a260: 8c05 7065 726d 7394 7d94 8c04 7479 7065  ..perms.}...type
+0000a270: 948c 0673 7472 696e 6794 738c 0a61 6363  ...string.s..acc
+0000a280: 6573 7354 696d 6594 7d94 288c 0474 7970  essTime.}.(..typ
+0000a290: 6594 8c07 696e 7465 6765 7294 8c06 666f  e...integer...fo
+0000a2a0: 726d 6174 948c 0569 6e74 3634 9475 8c0a  rmat...int64.u..
+0000a2b0: 6d6f 6469 6679 5469 6d65 947d 9428 8c04  modifyTime.}.(..
+0000a2c0: 7479 7065 948c 0769 6e74 6567 6572 948c  type...integer..
+0000a2d0: 0666 6f72 6d61 7494 8c05 696e 7436 3494  .format...int64.
+0000a2e0: 758c 0364 6972 947d 948c 0474 7970 6594  u..dir.}...type.
+0000a2f0: 8c07 626f 6f6c 6561 6e94 738c 046c 696e  ..boolean.s..lin
+0000a300: 6b94 7d94 8c04 7479 7065 948c 0762 6f6f  k.}...type...boo
+0000a310: 6c65 616e 9473 7575 8c0c 4163 6c45 6e74  lean.suu..AclEnt
+0000a320: 7279 496e 666f 947d 9428 8c04 7479 7065  ryInfo.}.(..type
+0000a330: 948c 066f 626a 6563 7494 8c0a 7072 6f70  ...object...prop
+0000a340: 6572 7469 6573 947d 9428 8c0a 6465 6661  erties.}.(..defa
+0000a350: 756c 7441 636c 947d 948c 0474 7970 6594  ultAcl.}...type.
+0000a360: 8c07 626f 6f6c 6561 6e94 738c 0474 7970  ..boolean.s..typ
+0000a370: 6594 7d94 8c04 7479 7065 948c 0673 7472  e.}...type...str
+0000a380: 696e 6794 738c 0970 7269 6e63 6970 616c  ing.s..principal
+0000a390: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000a3a0: 6e67 9473 8c0b 7065 726d 6973 7369 6f6e  ng.s..permission
+0000a3b0: 7394 7d94 8c04 7479 7065 948c 0673 7472  s.}...type...str
+0000a3c0: 696e 6794 7375 758c 1346 696c 654c 6973  ing.suu..FileLis
+0000a3d0: 7469 6e67 5265 7370 6f6e 7365 947d 9428  tingResponse.}.(
+0000a3e0: 8c04 7479 7065 948c 066f 626a 6563 7494  ..type...object.
+0000a3f0: 8c0a 7072 6f70 6572 7469 6573 947d 9428  ..properties.}.(
+0000a400: 8c06 7374 6174 7573 947d 948c 0474 7970  ..status.}...typ
+0000a410: 6594 8c06 7374 7269 6e67 9473 8c07 6d65  e...string.s..me
+0000a420: 7373 6167 6594 7d94 8c04 7479 7065 948c  ssage.}...type..
+0000a430: 0673 7472 696e 6794 738c 0672 6573 756c  .string.s..resul
+0000a440: 7494 7d94 288c 0474 7970 6594 8c05 6172  t.}.(..type...ar
+0000a450: 7261 7994 8c05 6974 656d 7394 7d94 8c04  ray...items.}...
+0000a460: 2472 6566 948c 1d23 2f63 6f6d 706f 6e65  $ref...#/compone
+0000a470: 6e74 732f 7363 6865 6d61 732f 4669 6c65  nts/schemas/File
+0000a480: 496e 666f 9473 758c 0776 6572 7369 6f6e  Info.su..version
+0000a490: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000a4a0: 6e67 9473 8c08 6d65 7461 6461 7461 947d  ng.s..metadata.}
+0000a4b0: 948c 0474 7970 6594 8c06 6f62 6a65 6374  ...type...object
+0000a4c0: 9473 7575 8c0e 4669 6c65 5065 726d 6973  .suu..FilePermis
+0000a4d0: 7369 6f6e 947d 9428 8c04 7479 7065 948c  sion.}.(..type..
+0000a4e0: 066f 626a 6563 7494 8c0a 7072 6f70 6572  .object...proper
+0000a4f0: 7469 6573 947d 9428 8c08 7465 6e61 6e74  ties.}.(..tenant
+0000a500: 4964 947d 948c 0474 7970 6594 8c06 7374  Id.}...type...st
+0000a510: 7269 6e67 9473 8c08 7573 6572 6e61 6d65  ring.s..username
+0000a520: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000a530: 6e67 9473 8c08 7379 7374 656d 4964 947d  ng.s..systemId.}
+0000a540: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+0000a550: 9473 8c04 7061 7468 947d 948c 0474 7970  .s..path.}...typ
+0000a560: 6594 8c06 7374 7269 6e67 9473 8c0a 7065  e...string.s..pe
+0000a570: 726d 6973 7369 6f6e 947d 948c 0424 7265  rmission.}...$re
+0000a580: 6694 8c1d 232f 636f 6d70 6f6e 656e 7473  f...#/components
+0000a590: 2f73 6368 656d 6173 2f50 6572 6d45 6e75  /schemas/PermEnu
+0000a5a0: 6d94 7375 758c 1053 6861 7265 6446 696c  m.suu..SharedFil
+0000a5b0: 654f 626a 6563 7494 7d94 288c 0474 7970  eObject.}.(..typ
+0000a5c0: 6594 8c06 6f62 6a65 6374 948c 0a70 726f  e...object...pro
+0000a5d0: 7065 7274 6965 7394 7d94 288c 0763 7265  perties.}.(..cre
+0000a5e0: 6174 6f72 947d 9428 8c04 7479 7065 948c  ator.}.(..type..
+0000a5f0: 0673 7472 696e 6794 8c0b 6465 7363 7269  .string...descri
+0000a600: 7074 696f 6e94 8c26 5573 6572 6e61 6d65  ption..&Username
+0000a610: 2077 686f 2073 6861 7265 6420 7468 6520   who shared the 
+0000a620: 6669 6c65 2f64 6972 6563 746f 7279 9475  file/directory.u
+0000a630: 8c0a 7368 6172 6564 5769 7468 947d 9428  ..sharedWith.}.(
+0000a640: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000a650: 8c0b 6465 7363 7269 7074 696f 6e94 8c1f  ..description...
+0000a660: 5573 6572 6e61 6d65 2077 686f 2077 6173  Username who was
+0000a670: 2067 7261 6e74 6564 2061 6363 6573 7394   granted access.
+0000a680: 758c 0763 7265 6174 6564 947d 9428 8c04  u..created.}.(..
+0000a690: 7479 7065 948c 0673 7472 696e 6794 8c0b  type...string...
+0000a6a0: 6465 7363 7269 7074 696f 6e94 8c19 4372  description...Cr
+0000a6b0: 6561 7469 6f6e 2074 696d 6573 7461 6d70  eation timestamp
+0000a6c0: 2069 6e20 5554 4394 758c 0965 7870 6972   in UTC.u..expir
+0000a6d0: 6573 496e 947d 9428 8c04 7479 7065 948c  esIn.}.(..type..
+0000a6e0: 0769 6e74 6567 6572 948c 0b64 6573 6372  .integer...descr
+0000a6f0: 6970 7469 6f6e 948c 374e 756d 6265 7220  iption..7Number 
+0000a700: 6f66 2073 6563 6f6e 6473 2069 6e20 7768  of seconds in wh
+0000a710: 6963 6820 7468 6520 7368 6172 6520 7761  ich the share wa
+0000a720: 7320 7365 7420 746f 2065 7870 6972 652e  s set to expire.
+0000a730: 948c 0666 6f72 6d61 7494 8c05 696e 7433  ...format...int3
+0000a740: 3294 758c 0375 726c 947d 9428 8c04 7479  2.u..url.}.(..ty
+0000a750: 7065 948c 0673 7472 696e 6794 8c0b 6465  pe...string...de
+0000a760: 7363 7269 7074 696f 6e94 8c18 4c69 6e6b  scription...Link
+0000a770: 2074 6f20 7468 6520 7368 6172 6564 2066   to the shared f
+0000a780: 696c 652e 9475 7575 8c10 5368 6172 6546  ile..uuu..ShareF
+0000a790: 696c 6552 6571 7565 7374 947d 9428 8c08  ileRequest.}.(..
+0000a7a0: 7265 7175 6972 6564 945d 9428 8c09 6578  required.].(..ex
+0000a7b0: 7069 7265 7349 6e94 8c08 7573 6572 6e61  piresIn...userna
+0000a7c0: 6d65 9465 8c04 7479 7065 948c 066f 626a  me.e..type...obj
+0000a7d0: 6563 7494 8c0a 7072 6f70 6572 7469 6573  ect...properties
+0000a7e0: 947d 9428 8c08 7573 6572 6e61 6d65 947d  .}.(..username.}
+0000a7f0: 9428 8c04 7479 7065 948c 0673 7472 696e  .(..type...strin
+0000a800: 6794 8c0b 6465 7363 7269 7074 696f 6e94  g...description.
+0000a810: 8c1c 5468 6520 7573 6572 2077 6974 6820  ..The user with 
+0000a820: 7768 6963 6820 746f 2073 6861 7265 9475  which to share.u
+0000a830: 8c09 6578 7069 7265 7349 6e94 7d94 288c  ..expiresIn.}.(.
+0000a840: 076d 6178 696d 756d 944a 803a 0900 8c07  .maximum.J.:....
+0000a850: 6d69 6e69 6d75 6d94 4b01 8c04 7479 7065  minimum.K...type
+0000a860: 948c 0769 6e74 6567 6572 948c 0b64 6573  ...integer...des
+0000a870: 6372 6970 7469 6f6e 948c 4154 696d 6520  cription..ATime 
+0000a880: 696e 2073 6563 6f6e 6473 206f 6620 6578  in seconds of ex
+0000a890: 7069 7261 7469 6f6e 2e20 6d69 6e69 6d75  piration. minimu
+0000a8a0: 6d3d 312c 206d 6178 696d 756d 3d36 3034  m=1, maximum=604
+0000a8b0: 3830 3020 2831 2077 6565 6b29 948c 0666  800 (1 week)...f
+0000a8c0: 6f72 6d61 7494 8c05 696e 7433 3294 7575  ormat...int32.uu
+0000a8d0: 758c 0c54 7261 6e73 6665 7254 6173 6b94  u..TransferTask.
+0000a8e0: 7d94 288c 0474 7970 6594 8c06 6f62 6a65  }.(..type...obje
+0000a8f0: 6374 948c 0a70 726f 7065 7274 6965 7394  ct...properties.
+0000a900: 7d94 288c 0269 6494 7d94 288c 0474 7970  }.(..id.}.(..typ
+0000a910: 6594 8c07 696e 7465 6765 7294 8c06 666f  e...integer...fo
+0000a920: 726d 6174 948c 0569 6e74 3332 9475 8c08  rmat...int32.u..
+0000a930: 7573 6572 6e61 6d65 947d 948c 0474 7970  username.}...typ
+0000a940: 6594 8c06 7374 7269 6e67 9473 8c08 7465  e...string.s..te
+0000a950: 6e61 6e74 4964 947d 948c 0474 7970 6594  nantId.}...type.
+0000a960: 8c06 7374 7269 6e67 9473 8c03 7461 6794  ..string.s..tag.
+0000a970: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+0000a980: 6794 738c 0475 7569 6494 7d94 288c 0474  g.s..uuid.}.(..t
+0000a990: 7970 6594 8c06 7374 7269 6e67 948c 0666  ype...string...f
+0000a9a0: 6f72 6d61 7494 8c04 7575 6964 9475 8c06  ormat...uuid.u..
+0000a9b0: 7374 6174 7573 947d 948c 0424 7265 6694  status.}...$ref.
+0000a9c0: 8c27 232f 636f 6d70 6f6e 656e 7473 2f73  .'#/components/s
+0000a9d0: 6368 656d 6173 2f54 7261 6e73 6665 7253  chemas/TransferS
+0000a9e0: 7461 7475 7345 6e75 6d94 738c 0b70 6172  tatusEnum.s..par
+0000a9f0: 656e 7454 6173 6b73 947d 9428 8c04 7479  entTasks.}.(..ty
+0000aa00: 7065 948c 0561 7272 6179 948c 0569 7465  pe...array...ite
+0000aa10: 6d73 947d 948c 0424 7265 6694 8c27 232f  ms.}...$ref..'#/
+0000aa20: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+0000aa30: 6173 2f54 7261 6e73 6665 7254 6173 6b50  as/TransferTaskP
+0000aa40: 6172 656e 7494 7375 8c13 6573 7469 6d61  arent.su..estima
+0000aa50: 7465 6454 6f74 616c 4279 7465 7394 7d94  tedTotalBytes.}.
+0000aa60: 288c 0474 7970 6594 8c07 696e 7465 6765  (..type...intege
+0000aa70: 7294 8c06 666f 726d 6174 948c 0569 6e74  r...format...int
+0000aa80: 3634 9475 8c15 746f 7461 6c42 7974 6573  64.u..totalBytes
+0000aa90: 5472 616e 7366 6572 7265 6494 7d94 288c  Transferred.}.(.
+0000aaa0: 0474 7970 6594 8c07 696e 7465 6765 7294  .type...integer.
+0000aab0: 8c06 666f 726d 6174 948c 0569 6e74 3634  ..format...int64
+0000aac0: 9475 8c0e 746f 7461 6c54 7261 6e73 6665  .u..totalTransfe
+0000aad0: 7273 947d 9428 8c04 7479 7065 948c 0769  rs.}.(..type...i
+0000aae0: 6e74 6567 6572 948c 0666 6f72 6d61 7494  nteger...format.
+0000aaf0: 8c05 696e 7433 3294 758c 1163 6f6d 706c  ..int32.u..compl
+0000ab00: 6574 6554 7261 6e73 6665 7273 947d 9428  eteTransfers.}.(
+0000ab10: 8c04 7479 7065 948c 0769 6e74 6567 6572  ..type...integer
+0000ab20: 948c 0666 6f72 6d61 7494 8c05 696e 7433  ...format...int3
+0000ab30: 3294 758c 0c65 7272 6f72 4d65 7373 6167  2.u..errorMessag
+0000ab40: 6594 7d94 8c04 7479 7065 948c 0673 7472  e.}...type...str
+0000ab50: 696e 6794 738c 0763 7265 6174 6564 947d  ing.s..created.}
+0000ab60: 9428 8c04 7479 7065 948c 0673 7472 696e  .(..type...strin
+0000ab70: 6794 8c06 666f 726d 6174 948c 0964 6174  g...format...dat
+0000ab80: 652d 7469 6d65 9475 8c09 7374 6172 7454  e-time.u..startT
+0000ab90: 696d 6594 7d94 288c 0474 7970 6594 8c06  ime.}.(..type...
+0000aba0: 7374 7269 6e67 948c 0666 6f72 6d61 7494  string...format.
+0000abb0: 8c09 6461 7465 2d74 696d 6594 758c 0765  ..date-time.u..e
+0000abc0: 6e64 5469 6d65 947d 9428 8c04 7479 7065  ndTime.}.(..type
+0000abd0: 948c 0673 7472 696e 6794 8c06 666f 726d  ...string...form
+0000abe0: 6174 948c 0964 6174 652d 7469 6d65 9475  at...date-time.u
+0000abf0: 7575 8c12 5472 616e 7366 6572 5461 736b  uu..TransferTask
+0000ac00: 5061 7265 6e74 947d 9428 8c04 7479 7065  Parent.}.(..type
+0000ac10: 948c 066f 626a 6563 7494 8c0a 7072 6f70  ...object...prop
+0000ac20: 6572 7469 6573 947d 9428 8c02 6964 947d  erties.}.(..id.}
+0000ac30: 9428 8c04 7479 7065 948c 0769 6e74 6567  .(..type...integ
+0000ac40: 6572 948c 0666 6f72 6d61 7494 8c05 696e  er...format...in
+0000ac50: 7433 3294 758c 0874 656e 616e 7449 6494  t32.u..tenantId.
+0000ac60: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+0000ac70: 6794 738c 0875 7365 726e 616d 6594 7d94  g.s..username.}.
+0000ac80: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000ac90: 738c 0973 6f75 7263 6555 5249 947d 948c  s..sourceURI.}..
+0000aca0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+0000acb0: 8c0e 6465 7374 696e 6174 696f 6e55 5249  ..destinationURI
+0000acc0: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000acd0: 6e67 9473 8c0a 746f 7461 6c42 7974 6573  ng.s..totalBytes
+0000ace0: 947d 9428 8c04 7479 7065 948c 0769 6e74  .}.(..type...int
+0000acf0: 6567 6572 948c 0666 6f72 6d61 7494 8c05  eger...format...
+0000ad00: 696e 7436 3494 758c 1062 7974 6573 5472  int64.u..bytesTr
+0000ad10: 616e 7366 6572 7265 6494 7d94 288c 0474  ansferred.}.(..t
+0000ad20: 7970 6594 8c07 696e 7465 6765 7294 8c06  ype...integer...
+0000ad30: 666f 726d 6174 948c 0569 6e74 3634 9475  format...int64.u
+0000ad40: 8c06 7461 736b 4964 947d 9428 8c04 7479  ..taskId.}.(..ty
+0000ad50: 7065 948c 0769 6e74 6567 6572 948c 0666  pe...integer...f
+0000ad60: 6f72 6d61 7494 8c05 696e 7433 3294 758c  ormat...int32.u.
+0000ad70: 0863 6869 6c64 7265 6e94 7d94 288c 0474  .children.}.(..t
+0000ad80: 7970 6594 8c05 6172 7261 7994 8c05 6974  ype...array...it
+0000ad90: 656d 7394 7d94 8c04 2472 6566 948c 2623  ems.}...$ref..&#
+0000ada0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+0000adb0: 6d61 732f 5472 616e 7366 6572 5461 736b  mas/TransferTask
+0000adc0: 4368 696c 6494 7375 8c0c 6572 726f 724d  Child.su..errorM
+0000add0: 6573 7361 6765 947d 948c 0474 7970 6594  essage.}...type.
+0000ade0: 8c06 7374 7269 6e67 9473 8c04 7575 6964  ..string.s..uuid
+0000adf0: 947d 9428 8c04 7479 7065 948c 0673 7472  .}.(..type...str
+0000ae00: 696e 6794 8c0b 6465 7363 7269 7074 696f  ing...descriptio
+0000ae10: 6e94 8c16 556e 6971 7565 2049 4420 6f66  n...Unique ID of
+0000ae20: 2074 6865 2074 6173 6b2e 948c 0666 6f72   the task....for
+0000ae30: 6d61 7494 8c04 7575 6964 9475 8c06 7374  mat...uuid.u..st
+0000ae40: 6174 7573 947d 948c 0424 7265 6694 8c27  atus.}...$ref..'
+0000ae50: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+0000ae60: 656d 6173 2f54 7261 6e73 6665 7253 7461  emas/TransferSta
+0000ae70: 7475 7345 6e75 6d94 738c 0763 7265 6174  tusEnum.s..creat
+0000ae80: 6564 947d 9428 8c04 7479 7065 948c 0673  ed.}.(..type...s
+0000ae90: 7472 696e 6794 8c06 666f 726d 6174 948c  tring...format..
+0000aea0: 0964 6174 652d 7469 6d65 9475 8c09 7374  .date-time.u..st
+0000aeb0: 6172 7454 696d 6594 7d94 288c 0474 7970  artTime.}.(..typ
+0000aec0: 6594 8c06 7374 7269 6e67 948c 0666 6f72  e...string...for
+0000aed0: 6d61 7494 8c09 6461 7465 2d74 696d 6594  mat...date-time.
+0000aee0: 758c 0765 6e64 5469 6d65 947d 9428 8c04  u..endTime.}.(..
+0000aef0: 7479 7065 948c 0673 7472 696e 6794 8c06  type...string...
+0000af00: 666f 726d 6174 948c 0964 6174 652d 7469  format...date-ti
+0000af10: 6d65 9475 7575 8c11 5472 616e 7366 6572  me.uuu..Transfer
+0000af20: 5461 736b 4368 696c 6494 7d94 288c 0474  TaskChild.}.(..t
+0000af30: 7970 6594 8c06 6f62 6a65 6374 948c 0a70  ype...object...p
+0000af40: 726f 7065 7274 6965 7394 7d94 288c 0269  roperties.}.(..i
+0000af50: 6494 7d94 288c 0474 7970 6594 8c07 696e  d.}.(..type...in
+0000af60: 7465 6765 7294 8c06 666f 726d 6174 948c  teger...format..
+0000af70: 0569 6e74 3332 9475 8c08 7465 6e61 6e74  .int32.u..tenant
+0000af80: 4964 947d 948c 0474 7970 6594 8c06 7374  Id.}...type...st
+0000af90: 7269 6e67 9473 8c08 7573 6572 6e61 6d65  ring.s..username
+0000afa0: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000afb0: 6e67 9473 8c09 736f 7572 6365 5552 4994  ng.s..sourceURI.
+0000afc0: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+0000afd0: 6794 738c 0e64 6573 7469 6e61 7469 6f6e  g.s..destination
+0000afe0: 5552 4994 7d94 8c04 7479 7065 948c 0673  URI.}...type...s
+0000aff0: 7472 696e 6794 738c 0a74 6f74 616c 4279  tring.s..totalBy
+0000b000: 7465 7394 7d94 288c 0474 7970 6594 8c07  tes.}.(..type...
+0000b010: 696e 7465 6765 7294 8c06 666f 726d 6174  integer...format
+0000b020: 948c 0569 6e74 3634 9475 8c10 6279 7465  ...int64.u..byte
+0000b030: 7354 7261 6e73 6665 7272 6564 947d 9428  sTransferred.}.(
+0000b040: 8c04 7479 7065 948c 0769 6e74 6567 6572  ..type...integer
+0000b050: 948c 0666 6f72 6d61 7494 8c05 696e 7436  ...format...int6
+0000b060: 3494 758c 0674 6173 6b49 6494 7d94 288c  4.u..taskId.}.(.
+0000b070: 0474 7970 6594 8c07 696e 7465 6765 7294  .type...integer.
+0000b080: 8c06 666f 726d 6174 948c 0569 6e74 3332  ..format...int32
+0000b090: 9475 8c0c 6572 726f 724d 6573 7361 6765  .u..errorMessage
+0000b0a0: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000b0b0: 6e67 9473 8c0c 7061 7265 6e74 5461 736b  ng.s..parentTask
+0000b0c0: 4964 947d 9428 8c04 7479 7065 948c 0769  Id.}.(..type...i
+0000b0d0: 6e74 6567 6572 948c 0666 6f72 6d61 7494  nteger...format.
+0000b0e0: 8c05 696e 7433 3294 758c 0772 6574 7269  ..int32.u..retri
+0000b0f0: 6573 947d 9428 8c04 7479 7065 948c 0769  es.}.(..type...i
+0000b100: 6e74 6567 6572 948c 0666 6f72 6d61 7494  nteger...format.
+0000b110: 8c05 696e 7433 3294 758c 0364 6972 947d  ..int32.u..dir.}
+0000b120: 948c 0474 7970 6594 8c07 626f 6f6c 6561  ...type...boolea
+0000b130: 6e94 738c 0475 7569 6494 7d94 288c 0474  n.s..uuid.}.(..t
+0000b140: 7970 6594 8c06 7374 7269 6e67 948c 0b64  ype...string...d
+0000b150: 6573 6372 6970 7469 6f6e 948c 1655 6e69  escription...Uni
+0000b160: 7175 6520 4944 206f 6620 7468 6520 7461  que ID of the ta
+0000b170: 736b 2e94 8c06 666f 726d 6174 948c 0475  sk....format...u
+0000b180: 7569 6494 758c 0673 7461 7475 7394 7d94  uid.u..status.}.
+0000b190: 8c04 2472 6566 948c 2723 2f63 6f6d 706f  ..$ref..'#/compo
+0000b1a0: 6e65 6e74 732f 7363 6865 6d61 732f 5472  nents/schemas/Tr
+0000b1b0: 616e 7366 6572 5374 6174 7573 456e 756d  ansferStatusEnum
+0000b1c0: 9473 8c07 6372 6561 7465 6494 7d94 288c  .s..created.}.(.
+0000b1d0: 0474 7970 6594 8c06 7374 7269 6e67 948c  .type...string..
+0000b1e0: 0666 6f72 6d61 7494 8c09 6461 7465 2d74  .format...date-t
+0000b1f0: 696d 6594 758c 0973 7461 7274 5469 6d65  ime.u..startTime
+0000b200: 947d 9428 8c04 7479 7065 948c 0673 7472  .}.(..type...str
+0000b210: 696e 6794 8c06 666f 726d 6174 948c 0964  ing...format...d
+0000b220: 6174 652d 7469 6d65 9475 8c07 656e 6454  ate-time.u..endT
+0000b230: 696d 6594 7d94 288c 0474 7970 6594 8c06  ime.}.(..type...
+0000b240: 7374 7269 6e67 948c 0666 6f72 6d61 7494  string...format.
+0000b250: 8c09 6461 7465 2d74 696d 6594 7575 758c  ..date-time.uuu.
+0000b260: 0650 6f73 7449 7494 7d94 288c 0474 7970  .PostIt.}.(..typ
+0000b270: 6594 8c06 6f62 6a65 6374 948c 0a70 726f  e...object...pro
+0000b280: 7065 7274 6965 7394 7d94 288c 0870 6f73  perties.}.(..pos
+0000b290: 7469 7449 6494 7d94 288c 0474 7970 6594  titId.}.(..type.
+0000b2a0: 8c06 7374 7269 6e67 948c 0666 6f72 6d61  ..string...forma
+0000b2b0: 7494 8c04 7575 6964 948c 0b64 6573 6372  t...uuid...descr
+0000b2c0: 6970 7469 6f6e 948c 1c54 6865 2075 6e69  iption...The uni
+0000b2d0: 7175 6520 4944 206f 6620 7468 6520 506f  que ID of the Po
+0000b2e0: 7374 4974 2e94 758c 0873 7973 7465 6d49  stIt..u..systemI
+0000b2f0: 6494 7d94 288c 0474 7970 6594 8c06 7374  d.}.(..type...st
+0000b300: 7269 6e67 948c 0b64 6573 6372 6970 7469  ring...descripti
+0000b310: 6f6e 948c 4554 6865 2049 4420 6f66 2074  on..EThe ID of t
+0000b320: 6865 2073 7973 7465 6d20 7768 6572 6520  he system where 
+0000b330: 7468 6520 6669 6c65 2070 6f69 6e74 6564  the file pointed
+0000b340: 2074 6f20 6279 2074 6865 2050 6f73 7449   to by the PostI
+0000b350: 7420 7265 7369 6465 732e 9475 8c05 6f77  t resides..u..ow
+0000b360: 6e65 7294 7d94 288c 0474 7970 6594 8c06  ner.}.(..type...
+0000b370: 7374 7269 6e67 948c 0b64 6573 6372 6970  string...descrip
+0000b380: 7469 6f6e 948c 1854 6865 206f 776e 6572  tion...The owner
+0000b390: 206f 6620 7468 6520 506f 7374 4974 2e94   of the PostIt..
+0000b3a0: 758c 0874 656e 616e 7449 6494 7d94 288c  u..tenantId.}.(.
+0000b3b0: 0474 7970 6594 8c06 7374 7269 6e67 948c  .type...string..
+0000b3c0: 0b64 6573 6372 6970 7469 6f6e 948c 2774  .description..'t
+0000b3d0: 6865 2074 656e 616e 7420 7468 6174 2074  he tenant that t
+0000b3e0: 7468 6520 506f 7374 4974 2062 656c 6f6e  the PostIt belon
+0000b3f0: 6773 2074 6f2e 9475 8c04 7061 7468 947d  gs to..u..path.}
+0000b400: 9428 8c04 7479 7065 948c 0673 7472 696e  .(..type...strin
+0000b410: 6794 8c0b 6465 7363 7269 7074 696f 6e94  g...description.
+0000b420: 8c25 5061 7468 2072 656c 6174 6976 6520  .%Path relative 
+0000b430: 746f 2074 6865 2073 7973 7465 6d20 2a72  to the system *r
+0000b440: 6f6f 7444 6972 2a94 758c 0b61 6c6c 6f77  ootDir*.u..allow
+0000b450: 6564 5573 6573 947d 9428 8c04 7479 7065  edUses.}.(..type
+0000b460: 948c 0769 6e74 6567 6572 948c 0666 6f72  ...integer...for
+0000b470: 6d61 7494 8c05 696e 7433 3294 8c0b 6465  mat...int32...de
+0000b480: 7363 7269 7074 696f 6e94 8c6a 5468 6520  scription..jThe 
+0000b490: 6e75 6d62 6572 206f 6620 7469 6d65 7320  number of times 
+0000b4a0: 7468 6520 506f 7374 4974 206d 6179 2062  the PostIt may b
+0000b4b0: 6520 7265 6465 656d 6564 2e20 2054 6869  e redeemed.  Thi
+0000b4c0: 7320 6e75 6d62 6572 206d 696e 7573 202a  s number minus *
+0000b4d0: 7573 6573 2a20 6973 2074 6865 206e 756d  uses* is the num
+0000b4e0: 6265 7220 6f66 2075 7365 7320 7265 6d61  ber of uses rema
+0000b4f0: 696e 696e 672e 9475 8c09 7469 6d65 7355  ining..u..timesU
+0000b500: 7365 6494 7d94 288c 0474 7970 6594 8c07  sed.}.(..type...
+0000b510: 696e 7465 6765 7294 8c06 666f 726d 6174  integer...format
+0000b520: 948c 0569 6e74 3332 948c 0b64 6573 6372  ...int32...descr
+0000b530: 6970 7469 6f6e 948c 3a54 6865 206e 756d  iption..:The num
+0000b540: 6265 7220 6f66 2074 696d 6573 2074 6865  ber of times the
+0000b550: 2050 6f73 7449 7420 6861 7320 616c 7265   PostIt has alre
+0000b560: 6164 7920 6265 656e 2072 6574 7269 6576  ady been retriev
+0000b570: 6564 2e94 758c 076a 7774 5573 6572 947d  ed..u..jwtUser.}
 0000b580: 9428 8c04 7479 7065 948c 0673 7472 696e  .(..type...strin
-0000b590: 6794 8c09 6d69 6e4c 656e 6774 6894 4b01  g...minLength.K.
-0000b5a0: 8c09 6d61 784c 656e 6774 6894 4b50 758c  ..maxLength.KPu.
-0000b5b0: 0e55 7365 724e 616d 6553 7472 696e 6794  .UserNameString.
-0000b5c0: 7d94 288c 0474 7970 6594 8c06 7374 7269  }.(..type...stri
-0000b5d0: 6e67 948c 096d 696e 4c65 6e67 7468 944b  ng...minLength.K
-0000b5e0: 018c 096d 6178 4c65 6e67 7468 944b 3c75  ...maxLength.K<u
-0000b5f0: 8c0c 4d6b 6469 7252 6571 7565 7374 947d  ..MkdirRequest.}
-0000b600: 9428 8c08 7265 7175 6972 6564 945d 948c  .(..required.]..
-0000b610: 0470 6174 6894 618c 0474 7970 6594 8c06  .path.a..type...
-0000b620: 6f62 6a65 6374 948c 0a70 726f 7065 7274  object...propert
-0000b630: 6965 7394 7d94 8c04 7061 7468 947d 9428  ies.}...path.}.(
-0000b640: 8c07 7061 7474 6572 6e94 8c0d 5e28 3f21  ..pattern...^(?!
-0000b650: 2e2a 5c2e 5c2e 292e 2a94 8c04 7479 7065  .*\.\.).*...type
-0000b660: 948c 0673 7472 696e 6794 7573 758c 0f4d  ...string.usu..M
-0000b670: 6f76 6543 6f70 7952 6571 7565 7374 947d  oveCopyRequest.}
-0000b680: 9428 8c08 7265 7175 6972 6564 945d 9428  .(..required.].(
-0000b690: 8c07 6e65 7750 6174 6894 8c09 6f70 6572  ..newPath...oper
-0000b6a0: 6174 696f 6e94 658c 0474 7970 6594 8c06  ation.e..type...
-0000b6b0: 6f62 6a65 6374 948c 0a70 726f 7065 7274  object...propert
-0000b6c0: 6965 7394 7d94 288c 096f 7065 7261 7469  ies.}.(..operati
-0000b6d0: 6f6e 947d 9428 8c04 7479 7065 948c 0673  on.}.(..type...s
-0000b6e0: 7472 696e 6794 8c04 656e 756d 945d 9428  tring...enum.].(
-0000b6f0: 8c04 4d4f 5645 948c 0443 4f50 5994 6575  ..MOVE...COPY.eu
-0000b700: 8c07 6e65 7750 6174 6894 7d94 288c 0474  ..newPath.}.(..t
-0000b710: 7970 6594 8c06 7374 7269 6e67 948c 0b64  ype...string...d
-0000b720: 6573 6372 6970 7469 6f6e 948c 2c50 6174  escription..,Pat
-0000b730: 6873 206d 7573 7420 6265 2061 6273 6f6c  hs must be absol
-0000b740: 7574 652c 202e 2e2f 2e2e 2069 7320 6e6f  ute, ../.. is no
-0000b750: 7420 616c 6c6f 7765 6494 7575 758c 1743  t allowed.uuu..C
-0000b760: 7265 6174 6550 6572 6d69 7373 696f 6e52  reatePermissionR
-0000b770: 6571 7565 7374 947d 9428 8c08 7265 7175  equest.}.(..requ
-0000b780: 6972 6564 945d 9428 8c0a 7065 726d 6973  ired.].(..permis
-0000b790: 7369 6f6e 948c 0875 7365 726e 616d 6594  sion...username.
-0000b7a0: 658c 0474 7970 6594 8c06 6f62 6a65 6374  e..type...object
-0000b7b0: 948c 0a70 726f 7065 7274 6965 7394 7d94  ...properties.}.
-0000b7c0: 288c 0875 7365 726e 616d 6594 7d94 8c04  (..username.}...
-0000b7d0: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-0000b7e0: 0a70 6572 6d69 7373 696f 6e94 7d94 8c04  .permission.}...
-0000b7f0: 2472 6566 948c 1d23 2f63 6f6d 706f 6e65  $ref...#/compone
-0000b800: 6e74 732f 7363 6865 6d61 732f 5065 726d  nts/schemas/Perm
-0000b810: 456e 756d 9473 7575 8c0e 5265 7153 6861  Enum.suu..ReqSha
-0000b820: 7265 5570 6461 7465 947d 9428 8c04 7479  reUpdate.}.(..ty
-0000b830: 7065 948c 066f 626a 6563 7494 8c08 7265  pe...object...re
-0000b840: 7175 6972 6564 945d 948c 0575 7365 7273  quired.]...users
-0000b850: 9461 8c0a 7072 6f70 6572 7469 6573 947d  .a..properties.}
-0000b860: 948c 0575 7365 7273 947d 9428 8c04 7479  ...users.}.(..ty
-0000b870: 7065 948c 0561 7272 6179 948c 086d 696e  pe...array...min
-0000b880: 4974 656d 7394 4b01 8c05 6974 656d 7394  Items.K...items.
-0000b890: 7d94 8c04 2472 6566 948c 2323 2f63 6f6d  }...$ref..##/com
-0000b8a0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-0000b8b0: 5573 6572 4e61 6d65 5374 7269 6e67 9473  UserNameString.s
-0000b8c0: 7573 758c 0b52 6571 5472 616e 7366 6572  usu..ReqTransfer
-0000b8d0: 947d 9428 8c08 7265 7175 6972 6564 945d  .}.(..required.]
-0000b8e0: 948c 0865 6c65 6d65 6e74 7394 618c 0474  ...elements.a..t
-0000b8f0: 7970 6594 8c06 6f62 6a65 6374 948c 0a70  ype...object...p
-0000b900: 726f 7065 7274 6965 7394 7d94 288c 0374  roperties.}.(..t
-0000b910: 6167 947d 948c 0474 7970 6594 8c06 7374  ag.}...type...st
-0000b920: 7269 6e67 9473 8c08 656c 656d 656e 7473  ring.s..elements
-0000b930: 947d 9428 8c04 7479 7065 948c 0561 7272  .}.(..type...arr
-0000b940: 6179 948c 0569 7465 6d73 947d 948c 0424  ay...items.}...$
-0000b950: 7265 6694 8c27 232f 636f 6d70 6f6e 656e  ref..'#/componen
-0000b960: 7473 2f73 6368 656d 6173 2f52 6571 5472  ts/schemas/ReqTr
-0000b970: 616e 7366 6572 456c 656d 656e 7494 7375  ansferElement.su
-0000b980: 7575 8c12 5265 7154 7261 6e73 6665 7245  uu..ReqTransferE
-0000b990: 6c65 6d65 6e74 947d 9428 8c08 7265 7175  lement.}.(..requ
-0000b9a0: 6972 6564 945d 9428 8c0e 6465 7374 696e  ired.].(..destin
-0000b9b0: 6174 696f 6e55 5249 948c 0973 6f75 7263  ationURI...sourc
-0000b9c0: 6555 5249 9465 8c04 7479 7065 948c 066f  eURI.e..type...o
-0000b9d0: 626a 6563 7494 8c0a 7072 6f70 6572 7469  bject...properti
-0000b9e0: 6573 947d 9428 8c09 736f 7572 6365 5552  es.}.(..sourceUR
-0000b9f0: 4994 7d94 8c04 7479 7065 948c 0673 7472  I.}...type...str
-0000ba00: 696e 6794 738c 0e64 6573 7469 6e61 7469  ing.s..destinati
-0000ba10: 6f6e 5552 4994 7d94 8c04 7479 7065 948c  onURI.}...type..
-0000ba20: 0673 7472 696e 6794 738c 086f 7074 696f  .string.s..optio
-0000ba30: 6e61 6c94 7d94 288c 0474 7970 6594 8c07  nal.}.(..type...
-0000ba40: 626f 6f6c 6561 6e94 8c07 6465 6661 756c  boolean...defaul
-0000ba50: 7494 898c 0b64 6573 6372 6970 7469 6f6e  t....description
-0000ba60: 948c 3e41 6c6c 6f77 2074 6865 2066 756c  ..>Allow the ful
-0000ba70: 6c20 7472 616e 7366 6572 2074 6f20 7375  l transfer to su
-0000ba80: 6363 6565 6420 6576 656e 2069 6620 7468  cceed even if th
-0000ba90: 6973 2065 6c65 6d65 6e74 2066 6169 6c73  is element fails
-0000baa0: 2e94 758c 0f73 7263 5368 6172 6564 4170  ..u..srcSharedAp
-0000bab0: 7043 7478 947d 9428 8c04 7479 7065 948c  pCtx.}.(..type..
-0000bac0: 0762 6f6f 6c65 616e 948c 0764 6566 6175  .boolean...defau
-0000bad0: 6c74 9489 8c0b 6465 7363 7269 7074 696f  lt....descriptio
-0000bae0: 6e94 8c46 4365 7274 6169 6e20 7365 7276  n..FCertain serv
-0000baf0: 6963 6573 206d 6179 2069 6e64 6963 6174  ices may indicat
-0000bb00: 6520 7468 6174 2074 6865 2072 6571 7565  e that the reque
-0000bb10: 7374 2069 7320 696e 2061 2073 6861 7265  st is in a share
-0000bb20: 6420 636f 6e74 6578 742e 9475 8c10 6465  d context..u..de
-0000bb30: 7374 5368 6172 6564 4170 7043 7478 947d  stSharedAppCtx.}
-0000bb40: 9428 8c04 7479 7065 948c 0762 6f6f 6c65  .(..type...boole
-0000bb50: 616e 948c 0764 6566 6175 6c74 9489 8c0b  an...default....
-0000bb60: 6465 7363 7269 7074 696f 6e94 8c46 4365  description..FCe
-0000bb70: 7274 6169 6e20 7365 7276 6963 6573 206d  rtain services m
-0000bb80: 6179 2069 6e64 6963 6174 6520 7468 6174  ay indicate that
-0000bb90: 2074 6865 2072 6571 7565 7374 2069 7320   the request is 
-0000bba0: 696e 2061 2073 6861 7265 6420 636f 6e74  in a shared cont
-0000bbb0: 6578 742e 9475 7575 8c14 4e61 7469 7665  ext..uuu..Native
-0000bbc0: 4c69 6e75 784f 7052 6571 7565 7374 947d  LinuxOpRequest.}
-0000bbd0: 9428 8c08 7265 7175 6972 6564 945d 9428  .(..required.].(
-0000bbe0: 8c08 6172 6775 6d65 6e74 948c 096f 7065  ..argument...ope
-0000bbf0: 7261 7469 6f6e 9465 8c04 7479 7065 948c  ration.e..type..
-0000bc00: 066f 626a 6563 7494 8c0a 7072 6f70 6572  .object...proper
-0000bc10: 7469 6573 947d 9428 8c09 6f70 6572 6174  ties.}.(..operat
-0000bc20: 696f 6e94 7d94 288c 0474 7970 6594 8c06  ion.}.(..type...
-0000bc30: 7374 7269 6e67 948c 0465 6e75 6d94 5d94  string...enum.].
-0000bc40: 288c 0543 484d 4f44 948c 0543 484f 574e  (..CHMOD...CHOWN
-0000bc50: 948c 0543 4847 5250 9465 758c 0861 7267  ...CHGRP.eu..arg
-0000bc60: 756d 656e 7494 7d94 288c 0474 7970 6594  ument.}.(..type.
-0000bc70: 8c06 7374 7269 6e67 948c 0b64 6573 6372  ..string...descr
-0000bc80: 6970 7469 6f6e 948c 2341 7267 756d 656e  iption..#Argumen
-0000bc90: 7420 666f 7220 6e61 7469 7665 206c 696e  t for native lin
-0000bca0: 7578 206f 7065 7261 7469 6f6e 9475 7575  ux operation.uuu
-0000bcb0: 8c19 4e61 7469 7665 4c69 6e75 7853 6574  ..NativeLinuxSet
-0000bcc0: 4661 636c 5265 7175 6573 7494 7d94 288c  FaclRequest.}.(.
-0000bcd0: 0872 6571 7569 7265 6494 5d94 288c 096f  .required.].(..o
-0000bce0: 7065 7261 7469 6f6e 948c 0961 636c 5374  peration...aclSt
-0000bcf0: 7269 6e67 9465 8c04 7479 7065 948c 066f  ring.e..type...o
-0000bd00: 626a 6563 7494 8c0a 7072 6f70 6572 7469  bject...properti
-0000bd10: 6573 947d 9428 8c09 6f70 6572 6174 696f  es.}.(..operatio
-0000bd20: 6e94 7d94 288c 0474 7970 6594 8c06 7374  n.}.(..type...st
-0000bd30: 7269 6e67 948c 0465 6e75 6d94 5d94 288c  ring...enum.].(.
-0000bd40: 0341 4444 948c 0652 454d 4f56 4594 8c0e  .ADD...REMOVE...
-0000bd50: 5245 4d4f 5645 5f44 4546 4155 4c54 948c  REMOVE_DEFAULT..
-0000bd60: 0a52 454d 4f56 455f 414c 4c94 6575 8c0f  .REMOVE_ALL.eu..
-0000bd70: 7265 6375 7273 696f 6e4d 6574 686f 6494  recursionMethod.
-0000bd80: 7d94 288c 0474 7970 6594 8c06 7374 7269  }.(..type...stri
-0000bd90: 6e67 948c 0465 6e75 6d94 5d94 288c 044e  ng...enum.].(..N
-0000bda0: 4f4e 4594 8c08 5048 5953 4943 414c 948c  ONE...PHYSICAL..
-0000bdb0: 074c 4f47 4943 414c 9465 8c07 6465 6661  .LOGICAL.e..defa
-0000bdc0: 756c 7494 8c04 4e4f 4e45 948c 0b64 6573  ult...NONE...des
-0000bdd0: 6372 6970 7469 6f6e 948c 7052 6563 7572  cription..pRecur
-0000bde0: 7369 6f6e 206d 6179 2062 6520 7365 7420  sion may be set 
-0000bdf0: 746f 2070 6879 7369 6361 6c20 2864 6f6e  to physical (don
-0000be00: 2774 2066 6f6c 6c6f 7720 7379 6d6c 696e  't follow symlin
-0000be10: 6b73 2920 6f72 0a6c 6f67 6963 616c 2028  ks) or.logical (
-0000be20: 666f 6c6c 6f77 2073 796d 6c69 6e6b 7329  follow symlinks)
-0000be30: 2c20 6f72 206e 6f6e 6520 2864 6f6e 2774  , or none (don't
-0000be40: 2072 6563 7572 7365 292e 0a94 758c 0961   recurse)...u..a
-0000be50: 636c 5374 7269 6e67 947d 9428 8c04 7479  clString.}.(..ty
-0000be60: 7065 948c 0673 7472 696e 6794 8c0b 6465  pe...string...de
-0000be70: 7363 7269 7074 696f 6e94 8cc6 7370 6563  scription...spec
-0000be80: 6966 6965 7320 7468 6520 6163 7475 616c  ifies the actual
-0000be90: 2061 636c 2073 7472 696e 6720 746f 2073   acl string to s
-0000bea0: 6574 2e20 204d 756c 7469 706c 6520 6163  et.  Multiple ac
-0000beb0: 6c73 206d 6179 2062 6520 7365 7061 7261  ls may be separa
-0000bec0: 7465 6420 6279 200a 636f 6d6d 6173 2e0a  ted by .commas..
-0000bed0: 4578 616d 706c 6573 202d 2075 7365 723a  Examples - user:
-0000bee0: 6d79 7573 6572 3a72 7778 2c67 726f 7570  myuser:rwx,group
-0000bef0: 200a 2020 2020 2020 2020 2020 2067 726f   .           gro
-0000bf00: 7570 3a6d 7967 726f 7570 3a72 7720 0a20  up:mygroup:rw . 
-0000bf10: 2020 2020 2020 2020 2020 7573 6572 3a6d            user:m
-0000bf20: 7975 7365 723a 7277 782c 6772 6f75 702c  yuser:rwx,group,
-0000bf30: 6772 6f75 703a 6d79 6772 6f75 703a 7277  group:mygroup:rw
-0000bf40: 200a 9475 7575 8c13 4372 6561 7465 506f   ..uuu..CreatePo
-0000bf50: 7374 4974 5265 7175 6573 7494 7d94 288c  stItRequest.}.(.
-0000bf60: 0474 7970 6594 8c06 6f62 6a65 6374 948c  .type...object..
-0000bf70: 0a70 726f 7065 7274 6965 7394 7d94 288c  .properties.}.(.
-0000bf80: 0b61 6c6c 6f77 6564 5573 6573 947d 9428  .allowedUses.}.(
-0000bf90: 8c04 7479 7065 948c 0769 6e74 6567 6572  ..type...integer
-0000bfa0: 948c 0666 6f72 6d61 7494 8c05 696e 7433  ...format...int3
-0000bfb0: 3294 8c0b 6465 7363 7269 7074 696f 6e94  2...description.
-0000bfc0: 8cb8 4e75 6d62 6572 206f 6620 7469 6d65  ..Number of time
-0000bfd0: 7320 7468 6174 2074 6865 206e 6577 2050  s that the new P
-0000bfe0: 6f73 7449 7420 6361 6e20 6265 2072 6564  ostIt can be red
-0000bff0: 6565 6d65 642e 2054 6865 0a64 6566 6175  eemed. The.defau
-0000c000: 6c74 2069 7320 6f6e 6520 7573 652e 2020  lt is one use.  
-0000c010: 5365 7474 696e 6720 7468 6520 7661 6c75  Setting the valu
-0000c020: 6520 746f 202d 3120 286e 6567 6174 6976  e to -1 (negativ
-0000c030: 6520 6f6e 6529 0a77 696c 6c20 616c 6c6f  e one).will allo
-0000c040: 7720 7468 6520 506f 7374 4974 2074 6f20  w the PostIt to 
-0000c050: 6265 2072 6564 6565 6d65 6420 616e 2075  be redeemed an u
-0000c060: 6e6c 696d 6974 6564 206e 756d 6265 7220  nlimited number 
-0000c070: 6f66 0a74 696d 6573 2e0a 948c 0764 6566  of.times.....def
-0000c080: 6175 6c74 944b 0175 8c11 6578 7069 7261  ault.K.u..expira
-0000c090: 7469 6f6e 5365 636f 6e64 7394 7d94 288c  tionSeconds.}.(.
-0000c0a0: 0474 7970 6594 8c06 7374 7269 6e67 948c  .type...string..
-0000c0b0: 0666 6f72 6d61 7494 8c05 696e 7433 3294  .format...int32.
-0000c0c0: 8c0b 6465 7363 7269 7074 696f 6e94 8c42  ..description..B
-0000c0d0: 4e75 6d62 6572 206f 6620 7365 636f 6e64  Number of second
-0000c0e0: 7320 756e 7469 6c20 7468 6520 506f 7374  s until the Post
-0000c0f0: 4974 2065 7870 6972 6573 2e20 200a 4465  It expires.  .De
-0000c100: 6661 756c 7420 6973 2033 3020 6461 7973  fault is 30 days
-0000c110: 2e0a 948c 0764 6566 6175 6c74 944a 008d  .....default.J..
-0000c120: 2700 7575 758c 1355 7064 6174 6550 6f73  '.uuu..UpdatePos
-0000c130: 7449 7452 6571 7565 7374 947d 9428 8c04  tItRequest.}.(..
-0000c140: 7479 7065 948c 066f 626a 6563 7494 8c0a  type...object...
-0000c150: 7072 6f70 6572 7469 6573 947d 9428 8c0b  properties.}.(..
-0000c160: 616c 6c6f 7765 6455 7365 7394 7d94 288c  allowedUses.}.(.
-0000c170: 0474 7970 6594 8c07 696e 7465 6765 7294  .type...integer.
-0000c180: 8c06 666f 726d 6174 948c 0569 6e74 3332  ..format...int32
-0000c190: 948c 0b64 6573 6372 6970 7469 6f6e 948c  ...description..
-0000c1a0: 344e 756d 6265 7220 6f66 2074 696d 6573  4Number of times
-0000c1b0: 2074 6861 7420 7468 6520 6e65 7720 506f   that the new Po
-0000c1c0: 7374 4974 2063 616e 2062 6520 7265 6465  stIt can be rede
-0000c1d0: 656d 6564 2e94 758c 0a65 7870 6972 6174  emed..u..expirat
-0000c1e0: 696f 6e94 7d94 288c 0474 7970 6594 8c06  ion.}.(..type...
-0000c1f0: 7374 7269 6e67 948c 0666 6f72 6d61 7494  string...format.
-0000c200: 8c09 6461 7465 2d74 696d 6594 8c0b 6465  ..date-time...de
-0000c210: 7363 7269 7074 696f 6e94 8c1e 4578 7069  scription...Expi
-0000c220: 7261 7469 6f6e 2064 6174 6520 6f66 2074  ration date of t
-0000c230: 6865 2050 6f73 7449 742e 9475 8c09 756e  he PostIt..u..un
-0000c240: 6c69 6d69 7465 6494 7d94 288c 0474 7970  limited.}.(..typ
-0000c250: 6594 8c07 626f 6f6c 6561 6e94 8c0b 6465  e...boolean...de
-0000c260: 7363 7269 7074 696f 6e94 8c44 4966 2073  scription..DIf s
-0000c270: 6574 2074 6f20 7472 7565 2c20 7468 6973  et to true, this
-0000c280: 2050 6f73 7449 7420 7769 6c6c 2068 6176   PostIt will hav
-0000c290: 6520 756e 6c69 6d69 7465 6420 7573 6573  e unlimited uses
-0000c2a0: 2061 6e64 206e 6f74 2065 7870 6972 652e   and not expire.
-0000c2b0: 9475 7575 8c09 5265 7370 4261 7369 6394  .uuu..RespBasic.
-0000c2c0: 7d94 288c 0474 7970 6594 8c06 6f62 6a65  }.(..type...obje
-0000c2d0: 6374 948c 0a70 726f 7065 7274 6965 7394  ct...properties.
-0000c2e0: 7d94 288c 0673 7461 7475 7394 7d94 8c04  }.(..status.}...
-0000c2f0: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-0000c300: 076d 6573 7361 6765 947d 948c 0474 7970  .message.}...typ
-0000c310: 6594 8c06 7374 7269 6e67 9473 8c07 7665  e...string.s..ve
-0000c320: 7273 696f 6e94 7d94 8c04 7479 7065 948c  rsion.}...type..
-0000c330: 0673 7472 696e 6794 738c 0672 6573 756c  .string.s..resul
-0000c340: 7494 7d94 8c04 7479 7065 948c 066f 626a  t.}...type...obj
-0000c350: 6563 7494 738c 086d 6574 6164 6174 6194  ect.s..metadata.
-0000c360: 7d94 8c04 7479 7065 948c 066f 626a 6563  }...type...objec
-0000c370: 7494 7375 758c 1246 696c 6553 7472 696e  t.suu..FileStrin
-0000c380: 6752 6573 706f 6e73 6594 7d94 288c 0474  gResponse.}.(..t
-0000c390: 7970 6594 8c06 6f62 6a65 6374 948c 0a70  ype...object...p
-0000c3a0: 726f 7065 7274 6965 7394 7d94 288c 0673  roperties.}.(..s
-0000c3b0: 7461 7475 7394 7d94 8c04 7479 7065 948c  tatus.}...type..
-0000c3c0: 0673 7472 696e 6794 738c 076d 6573 7361  .string.s..messa
-0000c3d0: 6765 947d 948c 0474 7970 6594 8c06 7374  ge.}...type...st
-0000c3e0: 7269 6e67 9473 8c06 7265 7375 6c74 947d  ring.s..result.}
-0000c3f0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-0000c400: 9473 8c07 7665 7273 696f 6e94 7d94 8c04  .s..version.}...
-0000c410: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-0000c420: 086d 6574 6164 6174 6194 7d94 8c04 7479  .metadata.}...ty
-0000c430: 7065 948c 066f 626a 6563 7494 7375 758c  pe...object.suu.
-0000c440: 0e53 7472 696e 6752 6573 706f 6e73 6594  .StringResponse.
-0000c450: 7d94 288c 0474 7970 6594 8c06 6f62 6a65  }.(..type...obje
-0000c460: 6374 948c 0a70 726f 7065 7274 6965 7394  ct...properties.
-0000c470: 7d94 288c 0673 7461 7475 7394 7d94 8c04  }.(..status.}...
-0000c480: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-0000c490: 076d 6573 7361 6765 947d 948c 0474 7970  .message.}...typ
-0000c4a0: 6594 8c06 7374 7269 6e67 9473 8c06 7265  e...string.s..re
-0000c4b0: 7375 6c74 947d 948c 0474 7970 6594 8c06  sult.}...type...
-0000c4c0: 7374 7269 6e67 9473 8c07 7665 7273 696f  string.s..versio
-0000c4d0: 6e94 7d94 8c04 7479 7065 948c 0673 7472  n.}...type...str
-0000c4e0: 696e 6794 738c 086d 6574 6164 6174 6194  ing.s..metadata.
-0000c4f0: 7d94 8c04 7479 7065 948c 066f 626a 6563  }...type...objec
-0000c500: 7494 7375 758c 0a52 6573 7053 7472 696e  t.suu..RespStrin
-0000c510: 6794 7d94 288c 0474 7970 6594 8c06 6f62  g.}.(..type...ob
-0000c520: 6a65 6374 948c 0a70 726f 7065 7274 6965  ject...propertie
-0000c530: 7394 7d94 288c 0673 7461 7475 7394 7d94  s.}.(..status.}.
-0000c540: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-0000c550: 738c 076d 6573 7361 6765 947d 948c 0474  s..message.}...t
-0000c560: 7970 6594 8c06 7374 7269 6e67 9473 8c06  ype...string.s..
-0000c570: 7265 7375 6c74 947d 948c 0474 7970 6594  result.}...type.
-0000c580: 8c06 7374 7269 6e67 9473 8c07 7665 7273  ..string.s..vers
-0000c590: 696f 6e94 7d94 8c04 7479 7065 948c 0673  ion.}...type...s
-0000c5a0: 7472 696e 6794 738c 086d 6574 6164 6174  tring.s..metadat
-0000c5b0: 6194 7d94 8c04 7479 7065 948c 066f 626a  a.}...type...obj
-0000c5c0: 6563 7494 7375 758c 0f52 6573 7043 6861  ect.suu..RespCha
-0000c5d0: 6e67 6543 6f75 6e74 947d 9428 8c04 7479  ngeCount.}.(..ty
-0000c5e0: 7065 948c 066f 626a 6563 7494 8c0a 7072  pe...object...pr
-0000c5f0: 6f70 6572 7469 6573 947d 9428 8c06 7374  operties.}.(..st
-0000c600: 6174 7573 947d 948c 0474 7970 6594 8c06  atus.}...type...
-0000c610: 7374 7269 6e67 9473 8c07 6d65 7373 6167  string.s..messag
-0000c620: 6594 7d94 8c04 7479 7065 948c 0673 7472  e.}...type...str
-0000c630: 696e 6794 738c 0776 6572 7369 6f6e 947d  ing.s..version.}
-0000c640: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-0000c650: 9473 8c06 7265 7375 6c74 947d 948c 0424  .s..result.}...$
-0000c660: 7265 6694 8c26 232f 636f 6d70 6f6e 656e  ref..&#/componen
-0000c670: 7473 2f73 6368 656d 6173 2f52 6573 756c  ts/schemas/Resul
-0000c680: 7443 6861 6e67 6543 6f75 6e74 9473 8c08  tChangeCount.s..
-0000c690: 6d65 7461 6461 7461 947d 948c 0474 7970  metadata.}...typ
-0000c6a0: 6594 8c06 6f62 6a65 6374 9473 7575 8c11  e...object.suu..
-0000c6b0: 5265 7375 6c74 4368 616e 6765 436f 756e  ResultChangeCoun
-0000c6c0: 7494 7d94 288c 0474 7970 6594 8c06 6f62  t.}.(..type...ob
-0000c6d0: 6a65 6374 948c 0a70 726f 7065 7274 6965  ject...propertie
-0000c6e0: 7394 7d94 8c07 6368 616e 6765 7394 7d94  s.}...changes.}.
-0000c6f0: 288c 0474 7970 6594 8c07 696e 7465 6765  (..type...intege
-0000c700: 7294 8c06 666f 726d 6174 948c 0569 6e74  r...format...int
-0000c710: 3332 948c 0765 7861 6d70 6c65 944b 0175  32...example.K.u
-0000c720: 7375 8c0c 5265 7370 4669 6c65 4c69 7374  su..RespFileList
-0000c730: 947d 9428 8c04 7479 7065 948c 066f 626a  .}.(..type...obj
-0000c740: 6563 7494 8c0a 7072 6f70 6572 7469 6573  ect...properties
-0000c750: 947d 9428 8c06 7374 6174 7573 947d 948c  .}.(..status.}..
-0000c760: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-0000c770: 8c07 6d65 7373 6167 6594 7d94 8c04 7479  ..message.}...ty
-0000c780: 7065 948c 0673 7472 696e 6794 738c 0672  pe...string.s..r
-0000c790: 6573 756c 7494 7d94 288c 0474 7970 6594  esult.}.(..type.
-0000c7a0: 8c05 6172 7261 7994 8c05 6974 656d 7394  ..array...items.
-0000c7b0: 7d94 8c04 2472 6566 948c 1d23 2f63 6f6d  }...$ref...#/com
-0000c7c0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-0000c7d0: 4669 6c65 496e 666f 9473 758c 0776 6572  FileInfo.su..ver
-0000c7e0: 7369 6f6e 947d 948c 0474 7970 6594 8c06  sion.}...type...
-0000c7f0: 7374 7269 6e67 9473 8c08 6d65 7461 6461  string.s..metada
-0000c800: 7461 947d 948c 0474 7970 6594 8c06 6f62  ta.}...type...ob
-0000c810: 6a65 6374 9473 7575 8c14 4669 6c65 5374  ject.suu..FileSt
-0000c820: 6174 496e 666f 5265 7370 6f6e 7365 947d  atInfoResponse.}
-0000c830: 9428 8c04 7479 7065 948c 066f 626a 6563  .(..type...objec
-0000c840: 7494 8c0a 7072 6f70 6572 7469 6573 947d  t...properties.}
-0000c850: 9428 8c06 7374 6174 7573 947d 948c 0474  .(..status.}...t
-0000c860: 7970 6594 8c06 7374 7269 6e67 9473 8c07  ype...string.s..
-0000c870: 6d65 7373 6167 6594 7d94 8c04 7479 7065  message.}...type
-0000c880: 948c 0673 7472 696e 6794 738c 0672 6573  ...string.s..res
-0000c890: 756c 7494 7d94 8c04 2472 6566 948c 2123  ult.}...$ref..!#
-0000c8a0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-0000c8b0: 6d61 732f 4669 6c65 5374 6174 496e 666f  mas/FileStatInfo
-0000c8c0: 9473 8c07 7665 7273 696f 6e94 7d94 8c04  .s..version.}...
-0000c8d0: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-0000c8e0: 086d 6574 6164 6174 6194 7d94 8c04 7479  .metadata.}...ty
-0000c8f0: 7065 948c 066f 626a 6563 7494 7375 758c  pe...object.suu.
-0000c900: 154e 6174 6976 654c 696e 7578 4f70 5265  .NativeLinuxOpRe
-0000c910: 7370 6f6e 7365 947d 9428 8c04 7479 7065  sponse.}.(..type
-0000c920: 948c 066f 626a 6563 7494 8c0a 7072 6f70  ...object...prop
-0000c930: 6572 7469 6573 947d 9428 8c06 7374 6174  erties.}.(..stat
-0000c940: 7573 947d 948c 0474 7970 6594 8c06 7374  us.}...type...st
-0000c950: 7269 6e67 9473 8c07 6d65 7373 6167 6594  ring.s..message.
-0000c960: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
-0000c970: 6794 738c 0672 6573 756c 7494 7d94 8c04  g.s..result.}...
-0000c980: 2472 6566 948c 3023 2f63 6f6d 706f 6e65  $ref..0#/compone
-0000c990: 6e74 732f 7363 6865 6d61 732f 4e61 7469  nts/schemas/Nati
-0000c9a0: 7665 4c69 6e75 784f 7052 6573 756c 7452  veLinuxOpResultR
-0000c9b0: 6573 706f 6e73 6594 738c 0776 6572 7369  esponse.s..versi
-0000c9c0: 6f6e 947d 948c 0474 7970 6594 8c06 7374  on.}...type...st
-0000c9d0: 7269 6e67 9473 8c08 6d65 7461 6461 7461  ring.s..metadata
-0000c9e0: 947d 948c 0474 7970 6594 8c06 6f62 6a65  .}...type...obje
-0000c9f0: 6374 9473 7575 8c1b 4e61 7469 7665 4c69  ct.suu..NativeLi
-0000ca00: 6e75 784f 7052 6573 756c 7452 6573 706f  nuxOpResultRespo
-0000ca10: 6e73 6594 7d94 288c 0474 7970 6594 8c06  nse.}.(..type...
-0000ca20: 6f62 6a65 6374 948c 0a70 726f 7065 7274  object...propert
-0000ca30: 6965 7394 7d94 288c 0763 6f6d 6d61 6e64  ies.}.(..command
-0000ca40: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-0000ca50: 6e67 9473 8c08 6578 6974 436f 6465 947d  ng.s..exitCode.}
-0000ca60: 9428 8c04 7479 7065 948c 0769 6e74 6567  .(..type...integ
-0000ca70: 6572 948c 0666 6f72 6d61 7494 8c05 696e  er...format...in
-0000ca80: 7433 3294 758c 0673 7464 4f75 7494 7d94  t32.u..stdOut.}.
-0000ca90: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-0000caa0: 738c 0673 7464 4572 7294 7d94 8c04 7479  s..stdErr.}...ty
-0000cab0: 7065 948c 0673 7472 696e 6794 7375 758c  pe...string.suu.
-0000cac0: 1a4e 6174 6976 654c 696e 7578 5365 7446  .NativeLinuxSetF
-0000cad0: 6163 6c52 6573 706f 6e73 6594 7d94 288c  aclResponse.}.(.
-0000cae0: 0474 7970 6594 8c06 6f62 6a65 6374 948c  .type...object..
-0000caf0: 0a70 726f 7065 7274 6965 7394 7d94 288c  .properties.}.(.
-0000cb00: 0673 7461 7475 7394 7d94 8c04 7479 7065  .status.}...type
-0000cb10: 948c 0673 7472 696e 6794 738c 076d 6573  ...string.s..mes
-0000cb20: 7361 6765 947d 948c 0474 7970 6594 8c06  sage.}...type...
-0000cb30: 7374 7269 6e67 9473 8c06 7265 7375 6c74  string.s..result
-0000cb40: 947d 948c 0424 7265 6694 8c2d 232f 636f  .}...$ref..-#/co
-0000cb50: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-0000cb60: 2f4e 6174 6976 654c 696e 7578 5365 7446  /NativeLinuxSetF
-0000cb70: 6163 6c52 6573 756c 7494 738c 0776 6572  aclResult.s..ver
-0000cb80: 7369 6f6e 947d 948c 0474 7970 6594 8c06  sion.}...type...
-0000cb90: 7374 7269 6e67 9473 8c08 6d65 7461 6461  string.s..metada
-0000cba0: 7461 947d 948c 0474 7970 6594 8c06 6f62  ta.}...type...ob
-0000cbb0: 6a65 6374 9473 7575 8c18 4e61 7469 7665  ject.suu..Native
-0000cbc0: 4c69 6e75 7853 6574 4661 636c 5265 7375  LinuxSetFaclResu
-0000cbd0: 6c74 947d 9428 8c04 7479 7065 948c 066f  lt.}.(..type...o
-0000cbe0: 626a 6563 7494 8c0a 7072 6f70 6572 7469  bject...properti
-0000cbf0: 6573 947d 9428 8c07 636f 6d6d 616e 6494  es.}.(..command.
-0000cc00: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
-0000cc10: 6794 738c 0865 7869 7443 6f64 6594 7d94  g.s..exitCode.}.
-0000cc20: 288c 0474 7970 6594 8c07 696e 7465 6765  (..type...intege
-0000cc30: 7294 8c06 666f 726d 6174 948c 0569 6e74  r...format...int
-0000cc40: 3332 9475 8c06 7374 644f 7574 947d 948c  32.u..stdOut.}..
-0000cc50: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-0000cc60: 8c06 7374 6445 7272 947d 948c 0474 7970  ..stdErr.}...typ
-0000cc70: 6594 8c06 7374 7269 6e67 9473 7575 8c1a  e...string.suu..
-0000cc80: 4e61 7469 7665 4c69 6e75 7847 6574 4661  NativeLinuxGetFa
-0000cc90: 636c 5265 7370 6f6e 7365 947d 9428 8c04  clResponse.}.(..
-0000cca0: 7479 7065 948c 066f 626a 6563 7494 8c0a  type...object...
-0000ccb0: 7072 6f70 6572 7469 6573 947d 9428 8c06  properties.}.(..
-0000ccc0: 7374 6174 7573 947d 948c 0474 7970 6594  status.}...type.
-0000ccd0: 8c06 7374 7269 6e67 9473 8c07 6d65 7373  ..string.s..mess
-0000cce0: 6167 6594 7d94 8c04 7479 7065 948c 0673  age.}...type...s
-0000ccf0: 7472 696e 6794 738c 0672 6573 756c 7494  tring.s..result.
-0000cd00: 7d94 8c05 6974 656d 7394 7d94 8c04 2472  }...items.}...$r
-0000cd10: 6566 948c 2123 2f63 6f6d 706f 6e65 6e74  ef..!#/component
-0000cd20: 732f 7363 6865 6d61 732f 4163 6c45 6e74  s/schemas/AclEnt
-0000cd30: 7279 496e 666f 9473 738c 0776 6572 7369  ryInfo.ss..versi
-0000cd40: 6f6e 947d 948c 0474 7970 6594 8c06 7374  on.}...type...st
-0000cd50: 7269 6e67 9473 8c08 6d65 7461 6461 7461  ring.s..metadata
-0000cd60: 947d 948c 0474 7970 6594 8c06 6f62 6a65  .}...type...obje
-0000cd70: 6374 9473 7575 8c16 4669 6c65 5065 726d  ct.suu..FilePerm
-0000cd80: 6973 7369 6f6e 5265 7370 6f6e 7365 947d  issionResponse.}
-0000cd90: 9428 8c04 7479 7065 948c 066f 626a 6563  .(..type...objec
-0000cda0: 7494 8c0a 7072 6f70 6572 7469 6573 947d  t...properties.}
-0000cdb0: 9428 8c06 7374 6174 7573 947d 948c 0474  .(..status.}...t
-0000cdc0: 7970 6594 8c06 7374 7269 6e67 9473 8c07  ype...string.s..
-0000cdd0: 6d65 7373 6167 6594 7d94 8c04 7479 7065  message.}...type
-0000cde0: 948c 0673 7472 696e 6794 738c 0672 6573  ...string.s..res
-0000cdf0: 756c 7494 7d94 8c04 2472 6566 948c 2323  ult.}...$ref..##
-0000ce00: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-0000ce10: 6d61 732f 4669 6c65 5065 726d 6973 7369  mas/FilePermissi
-0000ce20: 6f6e 9473 8c07 7665 7273 696f 6e94 7d94  on.s..version.}.
-0000ce30: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-0000ce40: 738c 086d 6574 6164 6174 6194 7d94 8c04  s..metadata.}...
-0000ce50: 7479 7065 948c 066f 626a 6563 7494 7375  type...object.su
-0000ce60: 758c 0d52 6573 7053 6861 7265 496e 666f  u..RespShareInfo
-0000ce70: 947d 9428 8c04 7479 7065 948c 066f 626a  .}.(..type...obj
-0000ce80: 6563 7494 8c0a 7072 6f70 6572 7469 6573  ect...properties
-0000ce90: 947d 9428 8c06 7374 6174 7573 947d 948c  .}.(..status.}..
-0000cea0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-0000ceb0: 8c07 6d65 7373 6167 6594 7d94 8c04 7479  ..message.}...ty
-0000cec0: 7065 948c 0673 7472 696e 6794 738c 0776  pe...string.s..v
-0000ced0: 6572 7369 6f6e 947d 948c 0474 7970 6594  ersion.}...type.
-0000cee0: 8c06 7374 7269 6e67 9473 8c06 7265 7375  ..string.s..resu
-0000cef0: 6c74 947d 948c 0424 7265 6694 8c24 232f  lt.}...$ref..$#/
-0000cf00: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-0000cf10: 6173 2f52 6573 756c 7453 6861 7265 496e  as/ResultShareIn
-0000cf20: 666f 9473 8c08 6d65 7461 6461 7461 947d  fo.s..metadata.}
-0000cf30: 948c 0474 7970 6594 8c06 6f62 6a65 6374  ...type...object
-0000cf40: 9473 7575 8c0f 5265 7375 6c74 5368 6172  .suu..ResultShar
-0000cf50: 6549 6e66 6f94 7d94 288c 0474 7970 6594  eInfo.}.(..type.
-0000cf60: 8c06 6f62 6a65 6374 948c 0a70 726f 7065  ..object...prope
-0000cf70: 7274 6965 7394 7d94 288c 0869 7350 7562  rties.}.(..isPub
-0000cf80: 6c69 6394 7d94 288c 0474 7970 6594 8c07  lic.}.(..type...
-0000cf90: 626f 6f6c 6561 6e94 8c0b 6465 7363 7269  boolean...descri
-0000cfa0: 7074 696f 6e94 8c27 496e 6469 6361 7465  ption..'Indicate
-0000cfb0: 7320 6769 7665 6e20 7061 7468 2069 7320  s given path is 
-0000cfc0: 7368 6172 6564 2070 7562 6c69 636c 7994  shared publicly.
-0000cfd0: 758c 0c69 7350 7562 6c69 6350 6174 6894  u..isPublicPath.
-0000cfe0: 7d94 288c 0474 7970 6594 8c06 7374 7269  }.(..type...stri
-0000cff0: 6e67 948c 0b64 6573 6372 6970 7469 6f6e  ng...description
-0000d000: 948c 3a50 6174 6820 7468 6174 2072 6573  ..:Path that res
-0000d010: 756c 7465 6420 696e 2073 7065 6369 6669  ulted in specifi
-0000d020: 6564 2070 6174 6820 6265 696e 6720 7368  ed path being sh
-0000d030: 6172 6564 2070 7562 6c69 636c 7994 758c  ared publicly.u.
-0000d040: 0775 7365 7253 6574 947d 9428 8c04 7479  .userSet.}.(..ty
-0000d050: 7065 948c 0561 7272 6179 948c 0b64 6573  pe...array...des
-0000d060: 6372 6970 7469 6f6e 948c 2a53 6574 206f  cription..*Set o
-0000d070: 6620 7573 6572 7320 7769 7468 2077 686f  f users with who
-0000d080: 6d20 7468 6520 7061 7468 2069 7320 7368  m the path is sh
-0000d090: 6172 6564 2e94 8c05 6974 656d 7394 7d94  ared....items.}.
-0000d0a0: 8c04 2472 6566 948c 2323 2f63 6f6d 706f  ..$ref..##/compo
-0000d0b0: 6e65 6e74 732f 7363 6865 6d61 732f 5573  nents/schemas/Us
-0000d0c0: 6572 4e61 6d65 5374 7269 6e67 9473 758c  erNameString.su.
-0000d0d0: 1075 7365 7253 6861 7265 496e 666f 5365  .userShareInfoSe
-0000d0e0: 7494 7d94 288c 0474 7970 6594 8c05 6172  t.}.(..type...ar
-0000d0f0: 7261 7994 8c0b 6465 7363 7269 7074 696f  ray...descriptio
-0000d100: 6e94 8c33 4c69 7374 206f 6620 6164 6469  n..3List of addi
-0000d110: 7469 6f6e 616c 2073 6861 7265 2069 6e66  tional share inf
-0000d120: 6f72 6d61 7469 6f6e 2066 6f72 2065 6163  ormation for eac
-0000d130: 6820 7573 6572 2e94 8c05 6974 656d 7394  h user....items.
-0000d140: 7d94 8c04 2472 6566 948c 2223 2f63 6f6d  }...$ref.."#/com
-0000d150: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-0000d160: 5573 6572 5368 6172 6549 6e66 6f94 7375  UserShareInfo.su
-0000d170: 7575 8c0d 5573 6572 5368 6172 6549 6e66  uu..UserShareInf
-0000d180: 6f94 7d94 288c 0474 7970 6594 8c06 6f62  o.}.(..type...ob
-0000d190: 6a65 6374 948c 0a70 726f 7065 7274 6965  ject...propertie
-0000d1a0: 7394 7d94 288c 0875 7365 726e 616d 6594  s.}.(..username.
-0000d1b0: 7d94 8c04 2472 6566 948c 2323 2f63 6f6d  }...$ref..##/com
-0000d1c0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-0000d1d0: 5573 6572 4e61 6d65 5374 7269 6e67 9473  UserNameString.s
-0000d1e0: 8c04 7061 7468 947d 9428 8c04 7479 7065  ..path.}.(..type
-0000d1f0: 948c 0673 7472 696e 6794 8c0b 6465 7363  ...string...desc
-0000d200: 7269 7074 696f 6e94 8c3f 5061 7468 2074  ription..?Path t
-0000d210: 6861 7420 7265 7375 6c74 6564 2069 6e20  hat resulted in 
-0000d220: 7370 6563 6966 6965 6420 7061 7468 2062  specified path b
-0000d230: 6569 6e67 2073 6861 7265 6420 7769 7468  eing shared with
-0000d240: 2074 6865 2075 7365 7294 7575 758c 1454   the user.uuu..T
-0000d250: 7261 6e73 6665 7254 6173 6b52 6573 706f  ransferTaskRespo
-0000d260: 6e73 6594 7d94 288c 0474 7970 6594 8c06  nse.}.(..type...
-0000d270: 6f62 6a65 6374 948c 0a70 726f 7065 7274  object...propert
-0000d280: 6965 7394 7d94 288c 0673 7461 7475 7394  ies.}.(..status.
-0000d290: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
-0000d2a0: 6794 738c 076d 6573 7361 6765 947d 948c  g.s..message.}..
-0000d2b0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-0000d2c0: 8c06 7265 7375 6c74 947d 948c 0424 7265  ..result.}...$re
-0000d2d0: 6694 8c21 232f 636f 6d70 6f6e 656e 7473  f..!#/components
-0000d2e0: 2f73 6368 656d 6173 2f54 7261 6e73 6665  /schemas/Transfe
-0000d2f0: 7254 6173 6b94 738c 0776 6572 7369 6f6e  rTask.s..version
-0000d300: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-0000d310: 6e67 9473 8c08 6d65 7461 6461 7461 947d  ng.s..metadata.}
-0000d320: 948c 0474 7970 6594 8c06 6f62 6a65 6374  ...type...object
-0000d330: 9473 7575 8c18 5472 616e 7366 6572 5461  .suu..TransferTa
-0000d340: 736b 4c69 7374 5265 7370 6f6e 7365 947d  skListResponse.}
-0000d350: 9428 8c04 7479 7065 948c 066f 626a 6563  .(..type...objec
-0000d360: 7494 8c0a 7072 6f70 6572 7469 6573 947d  t...properties.}
-0000d370: 9428 8c06 7374 6174 7573 947d 948c 0474  .(..status.}...t
-0000d380: 7970 6594 8c06 7374 7269 6e67 9473 8c07  ype...string.s..
-0000d390: 6d65 7373 6167 6594 7d94 8c04 7479 7065  message.}...type
-0000d3a0: 948c 0673 7472 696e 6794 738c 0672 6573  ...string.s..res
-0000d3b0: 756c 7494 7d94 288c 0474 7970 6594 8c05  ult.}.(..type...
-0000d3c0: 6172 7261 7994 8c05 6974 656d 7394 7d94  array...items.}.
-0000d3d0: 8c04 2472 6566 948c 2123 2f63 6f6d 706f  ..$ref..!#/compo
-0000d3e0: 6e65 6e74 732f 7363 6865 6d61 732f 5472  nents/schemas/Tr
-0000d3f0: 616e 7366 6572 5461 736b 9473 758c 0776  ansferTask.su..v
-0000d400: 6572 7369 6f6e 947d 948c 0474 7970 6594  ersion.}...type.
-0000d410: 8c06 7374 7269 6e67 9473 8c08 6d65 7461  ..string.s..meta
-0000d420: 6461 7461 947d 948c 0474 7970 6594 8c06  data.}...type...
-0000d430: 6f62 6a65 6374 9473 7575 8c0e 506f 7374  object.suu..Post
-0000d440: 4974 5265 7370 6f6e 7365 947d 9428 8c04  ItResponse.}.(..
-0000d450: 7479 7065 948c 066f 626a 6563 7494 8c0a  type...object...
-0000d460: 7072 6f70 6572 7469 6573 947d 9428 8c06  properties.}.(..
-0000d470: 7374 6174 7573 947d 948c 0474 7970 6594  status.}...type.
-0000d480: 8c06 7374 7269 6e67 9473 8c07 6d65 7373  ..string.s..mess
-0000d490: 6167 6594 7d94 8c04 7479 7065 948c 0673  age.}...type...s
-0000d4a0: 7472 696e 6794 738c 0672 6573 756c 7494  tring.s..result.
-0000d4b0: 7d94 8c04 2472 6566 948c 1b23 2f63 6f6d  }...$ref...#/com
-0000d4c0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-0000d4d0: 506f 7374 4974 9473 8c07 7665 7273 696f  PostIt.s..versio
-0000d4e0: 6e94 7d94 8c04 7479 7065 948c 0673 7472  n.}...type...str
-0000d4f0: 696e 6794 738c 086d 6574 6164 6174 6194  ing.s..metadata.
-0000d500: 7d94 8c04 7479 7065 948c 066f 626a 6563  }...type...objec
-0000d510: 7494 7375 758c 1250 6f73 7449 744c 6973  t.suu..PostItLis
-0000d520: 7452 6573 706f 6e73 6594 7d94 288c 0474  tResponse.}.(..t
-0000d530: 7970 6594 8c06 6f62 6a65 6374 948c 0a70  ype...object...p
-0000d540: 726f 7065 7274 6965 7394 7d94 288c 0673  roperties.}.(..s
-0000d550: 7461 7475 7394 7d94 8c04 7479 7065 948c  tatus.}...type..
-0000d560: 0673 7472 696e 6794 738c 076d 6573 7361  .string.s..messa
-0000d570: 6765 947d 948c 0474 7970 6594 8c06 7374  ge.}...type...st
-0000d580: 7269 6e67 9473 8c06 7265 7375 6c74 947d  ring.s..result.}
-0000d590: 9428 8c04 7479 7065 948c 0561 7272 6179  .(..type...array
-0000d5a0: 948c 0569 7465 6d73 947d 948c 0424 7265  ...items.}...$re
-0000d5b0: 6694 8c1b 232f 636f 6d70 6f6e 656e 7473  f...#/components
-0000d5c0: 2f73 6368 656d 6173 2f50 6f73 7449 7494  /schemas/PostIt.
-0000d5d0: 7375 8c07 7665 7273 696f 6e94 7d94 8c04  su..version.}...
-0000d5e0: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-0000d5f0: 086d 6574 6164 6174 6194 7d94 8c04 7479  .metadata.}...ty
-0000d600: 7065 948c 066f 626a 6563 7494 7375 758c  pe...object.suu.
-0000d610: 1254 7261 6e73 6665 7253 7461 7475 7345  .TransferStatusE
-0000d620: 6e75 6d94 7d94 288c 0474 7970 6594 8c06  num.}.(..type...
-0000d630: 7374 7269 6e67 948c 0b64 6573 6372 6970  string...descrip
-0000d640: 7469 6f6e 948c 4b54 6865 2073 7461 7475  tion..KThe statu
-0000d650: 7320 6f66 2074 6865 2074 6173 6b2c 2073  s of the task, s
-0000d660: 7563 6820 6173 2041 4343 4550 5445 442c  uch as ACCEPTED,
-0000d670: 2049 4e5f 5052 4f47 5245 5353 2c20 434f   IN_PROGRESS, CO
-0000d680: 4d50 4c45 5445 442c 2043 414e 4345 4c4c  MPLETED, CANCELL
-0000d690: 4544 948c 0765 7861 6d70 6c65 948c 0750  ED...example...P
-0000d6a0: 454e 4449 4e47 948c 0465 6e75 6d94 5d94  ENDING...enum.].
-0000d6b0: 288c 0841 4343 4550 5445 4494 8c06 5354  (..ACCEPTED...ST
-0000d6c0: 4147 4544 948c 0b49 4e5f 5052 4f47 5245  AGED...IN_PROGRE
-0000d6d0: 5353 948c 0943 4f4d 504c 4554 4544 948c  SS...COMPLETED..
-0000d6e0: 0943 414e 4345 4c4c 4544 948c 0646 4149  .CANCELLED...FAI
-0000d6f0: 4c45 4494 8c0a 4641 494c 4544 5f4f 5054  LED...FAILED_OPT
-0000d700: 948c 0650 4155 5345 4494 6575 8c08 5065  ...PAUSED.eu..Pe
-0000d710: 726d 456e 756d 947d 9428 8c04 7479 7065  rmEnum.}.(..type
-0000d720: 948c 0673 7472 696e 6794 8c04 656e 756d  ...string...enum
-0000d730: 945d 9428 8c04 5245 4144 948c 064d 4f44  .].(..READ...MOD
-0000d740: 4946 5994 6575 8c0c 4c69 7374 5479 7065  IFY.eu..ListType
-0000d750: 456e 756d 947d 9428 8c04 7479 7065 948c  Enum.}.(..type..
-0000d760: 0673 7472 696e 6794 8c07 6465 6661 756c  .string...defaul
-0000d770: 7494 8c05 4f57 4e45 4494 8c04 656e 756d  t...OWNED...enum
-0000d780: 945d 9428 8c05 4f57 4e45 4494 8c03 414c  .].(..OWNED...AL
-0000d790: 4c94 6575 7573 752e                      L.euusu.
+0000b590: 6794 8c0b 6465 7363 7269 7074 696f 6e94  g...description.
+0000b5a0: 8c41 4175 7468 656e 7469 6361 7465 6420  .AAuthenticated 
+0000b5b0: 7573 6572 2066 726f 6d20 7468 6520 4a57  user from the JW
+0000b5c0: 5420 286d 6179 2062 6520 6469 6666 6572  T (may be differ
+0000b5d0: 656e 7420 7468 616e 204f 424f 2075 7365  ent than OBO use
+0000b5e0: 7229 2e94 758c 0b6a 7774 5465 6e61 6e74  r)..u..jwtTenant
+0000b5f0: 4964 947d 9428 8c04 7479 7065 948c 0673  Id.}.(..type...s
+0000b600: 7472 696e 6794 8c0b 6465 7363 7269 7074  tring...descript
+0000b610: 696f 6e94 8c54 5465 6e61 6e74 206f 6620  ion..TTenant of 
+0000b620: 6175 7468 656e 7469 6361 7465 6420 7573  authenticated us
+0000b630: 6572 2066 726f 6d20 7468 6520 4a57 5420  er from the JWT 
+0000b640: 286d 6179 2062 6520 6469 6666 6572 656e  (may be differen
+0000b650: 7420 7468 616e 204f 424f 2075 7365 7227  t than OBO user'
+0000b660: 7320 7465 6e61 6e74 292e 9475 8c09 7265  s tenant)..u..re
+0000b670: 6465 656d 5572 6c94 7d94 288c 0474 7970  deemUrl.}.(..typ
+0000b680: 6594 8c06 7374 7269 6e67 948c 0b64 6573  e...string...des
+0000b690: 6372 6970 7469 6f6e 948c 3d54 6865 2075  cription..=The u
+0000b6a0: 726c 2074 6f20 7573 6520 746f 2072 6574  rl to use to ret
+0000b6b0: 7269 6576 6520 7468 6520 6669 6c65 2070  rieve the file p
+0000b6c0: 6f69 6e74 6564 2074 6f20 6279 2074 6865  ointed to by the
+0000b6d0: 2050 6f73 7449 742e 9475 8c0a 6578 7069   PostIt..u..expi
+0000b6e0: 7261 7469 6f6e 947d 9428 8c04 7479 7065  ration.}.(..type
+0000b6f0: 948c 0673 7472 696e 6794 8c06 666f 726d  ...string...form
+0000b700: 6174 948c 0964 6174 652d 7469 6d65 948c  at...date-time..
+0000b710: 0b64 6573 6372 6970 7469 6f6e 948c 2754  .description..'T
+0000b720: 6865 2065 7870 6972 6174 696f 6e20 6461  he expiration da
+0000b730: 7465 2f74 696d 6520 6f66 2074 6865 2050  te/time of the P
+0000b740: 6f73 7449 742e 9475 8c07 6372 6561 7465  ostIt..u..create
+0000b750: 6494 7d94 288c 0474 7970 6594 8c06 7374  d.}.(..type...st
+0000b760: 7269 6e67 948c 0666 6f72 6d61 7494 8c09  ring...format...
+0000b770: 6461 7465 2d74 696d 6594 8c0b 6465 7363  date-time...desc
+0000b780: 7269 7074 696f 6e94 8c19 4372 6561 7469  ription...Creati
+0000b790: 6f6e 2074 696d 6573 7461 6d70 2069 6e20  on timestamp in 
+0000b7a0: 5554 4394 758c 0775 7064 6174 6564 947d  UTC.u..updated.}
+0000b7b0: 9428 8c04 7479 7065 948c 0673 7472 696e  .(..type...strin
+0000b7c0: 6794 8c06 666f 726d 6174 948c 0964 6174  g...format...dat
+0000b7d0: 652d 7469 6d65 948c 0b64 6573 6372 6970  e-time...descrip
+0000b7e0: 7469 6f6e 948c 1c4c 6173 7420 7570 6461  tion...Last upda
+0000b7f0: 7465 2074 696d 6573 7461 6d70 2069 6e20  te timestamp in 
+0000b800: 5554 4394 7575 758c 0849 6453 7472 696e  UTC.uuu..IdStrin
+0000b810: 6794 7d94 288c 0474 7970 6594 8c06 7374  g.}.(..type...st
+0000b820: 7269 6e67 948c 096d 696e 4c65 6e67 7468  ring...minLength
+0000b830: 944b 018c 096d 6178 4c65 6e67 7468 944b  .K...maxLength.K
+0000b840: 5075 8c0e 5573 6572 4e61 6d65 5374 7269  Pu..UserNameStri
+0000b850: 6e67 947d 9428 8c04 7479 7065 948c 0673  ng.}.(..type...s
+0000b860: 7472 696e 6794 8c09 6d69 6e4c 656e 6774  tring...minLengt
+0000b870: 6894 4b01 8c09 6d61 784c 656e 6774 6894  h.K...maxLength.
+0000b880: 4b3c 758c 0c4d 6b64 6972 5265 7175 6573  K<u..MkdirReques
+0000b890: 7494 7d94 288c 0872 6571 7569 7265 6494  t.}.(..required.
+0000b8a0: 5d94 8c04 7061 7468 9461 8c04 7479 7065  ]...path.a..type
+0000b8b0: 948c 066f 626a 6563 7494 8c0a 7072 6f70  ...object...prop
+0000b8c0: 6572 7469 6573 947d 948c 0470 6174 6894  erties.}...path.
+0000b8d0: 7d94 288c 0770 6174 7465 726e 948c 0d5e  }.(..pattern...^
+0000b8e0: 283f 212e 2a5c 2e5c 2e29 2e2a 948c 0474  (?!.*\.\.).*...t
+0000b8f0: 7970 6594 8c06 7374 7269 6e67 9475 7375  ype...string.usu
+0000b900: 8c0f 4d6f 7665 436f 7079 5265 7175 6573  ..MoveCopyReques
+0000b910: 7494 7d94 288c 0872 6571 7569 7265 6494  t.}.(..required.
+0000b920: 5d94 288c 076e 6577 5061 7468 948c 096f  ].(..newPath...o
+0000b930: 7065 7261 7469 6f6e 9465 8c04 7479 7065  peration.e..type
+0000b940: 948c 066f 626a 6563 7494 8c0a 7072 6f70  ...object...prop
+0000b950: 6572 7469 6573 947d 9428 8c09 6f70 6572  erties.}.(..oper
+0000b960: 6174 696f 6e94 7d94 288c 0474 7970 6594  ation.}.(..type.
+0000b970: 8c06 7374 7269 6e67 948c 0465 6e75 6d94  ..string...enum.
+0000b980: 5d94 288c 044d 4f56 4594 8c04 434f 5059  ].(..MOVE...COPY
+0000b990: 9465 758c 076e 6577 5061 7468 947d 9428  .eu..newPath.}.(
+0000b9a0: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000b9b0: 8c0b 6465 7363 7269 7074 696f 6e94 8c2c  ..description..,
+0000b9c0: 5061 7468 7320 6d75 7374 2062 6520 6162  Paths must be ab
+0000b9d0: 736f 6c75 7465 2c20 2e2e 2f2e 2e20 6973  solute, ../.. is
+0000b9e0: 206e 6f74 2061 6c6c 6f77 6564 9475 7575   not allowed.uuu
+0000b9f0: 8c17 4372 6561 7465 5065 726d 6973 7369  ..CreatePermissi
+0000ba00: 6f6e 5265 7175 6573 7494 7d94 288c 0872  onRequest.}.(..r
+0000ba10: 6571 7569 7265 6494 5d94 288c 0a70 6572  equired.].(..per
+0000ba20: 6d69 7373 696f 6e94 8c08 7573 6572 6e61  mission...userna
+0000ba30: 6d65 9465 8c04 7479 7065 948c 066f 626a  me.e..type...obj
+0000ba40: 6563 7494 8c0a 7072 6f70 6572 7469 6573  ect...properties
+0000ba50: 947d 9428 8c08 7573 6572 6e61 6d65 947d  .}.(..username.}
+0000ba60: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+0000ba70: 9473 8c0a 7065 726d 6973 7369 6f6e 947d  .s..permission.}
+0000ba80: 948c 0424 7265 6694 8c1d 232f 636f 6d70  ...$ref...#/comp
+0000ba90: 6f6e 656e 7473 2f73 6368 656d 6173 2f50  onents/schemas/P
+0000baa0: 6572 6d45 6e75 6d94 7375 758c 0e52 6571  ermEnum.suu..Req
+0000bab0: 5368 6172 6555 7064 6174 6594 7d94 288c  ShareUpdate.}.(.
+0000bac0: 0474 7970 6594 8c06 6f62 6a65 6374 948c  .type...object..
+0000bad0: 0872 6571 7569 7265 6494 5d94 8c05 7573  .required.]...us
+0000bae0: 6572 7394 618c 0a70 726f 7065 7274 6965  ers.a..propertie
+0000baf0: 7394 7d94 8c05 7573 6572 7394 7d94 288c  s.}...users.}.(.
+0000bb00: 0474 7970 6594 8c05 6172 7261 7994 8c08  .type...array...
+0000bb10: 6d69 6e49 7465 6d73 944b 018c 0569 7465  minItems.K...ite
+0000bb20: 6d73 947d 948c 0424 7265 6694 8c23 232f  ms.}...$ref..##/
+0000bb30: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+0000bb40: 6173 2f55 7365 724e 616d 6553 7472 696e  as/UserNameStrin
+0000bb50: 6794 7375 7375 8c0b 5265 7154 7261 6e73  g.susu..ReqTrans
+0000bb60: 6665 7294 7d94 288c 0872 6571 7569 7265  fer.}.(..require
+0000bb70: 6494 5d94 8c08 656c 656d 656e 7473 9461  d.]...elements.a
+0000bb80: 8c04 7479 7065 948c 066f 626a 6563 7494  ..type...object.
+0000bb90: 8c0a 7072 6f70 6572 7469 6573 947d 9428  ..properties.}.(
+0000bba0: 8c03 7461 6794 7d94 8c04 7479 7065 948c  ..tag.}...type..
+0000bbb0: 0673 7472 696e 6794 738c 0865 6c65 6d65  .string.s..eleme
+0000bbc0: 6e74 7394 7d94 288c 0474 7970 6594 8c05  nts.}.(..type...
+0000bbd0: 6172 7261 7994 8c05 6974 656d 7394 7d94  array...items.}.
+0000bbe0: 8c04 2472 6566 948c 2723 2f63 6f6d 706f  ..$ref..'#/compo
+0000bbf0: 6e65 6e74 732f 7363 6865 6d61 732f 5265  nents/schemas/Re
+0000bc00: 7154 7261 6e73 6665 7245 6c65 6d65 6e74  qTransferElement
+0000bc10: 9473 7575 758c 1252 6571 5472 616e 7366  .suuu..ReqTransf
+0000bc20: 6572 456c 656d 656e 7494 7d94 288c 0872  erElement.}.(..r
+0000bc30: 6571 7569 7265 6494 5d94 288c 0e64 6573  equired.].(..des
+0000bc40: 7469 6e61 7469 6f6e 5552 4994 8c09 736f  tinationURI...so
+0000bc50: 7572 6365 5552 4994 658c 0474 7970 6594  urceURI.e..type.
+0000bc60: 8c06 6f62 6a65 6374 948c 0a70 726f 7065  ..object...prope
+0000bc70: 7274 6965 7394 7d94 288c 0973 6f75 7263  rties.}.(..sourc
+0000bc80: 6555 5249 947d 948c 0474 7970 6594 8c06  eURI.}...type...
+0000bc90: 7374 7269 6e67 9473 8c0e 6465 7374 696e  string.s..destin
+0000bca0: 6174 696f 6e55 5249 947d 948c 0474 7970  ationURI.}...typ
+0000bcb0: 6594 8c06 7374 7269 6e67 9473 8c08 6f70  e...string.s..op
+0000bcc0: 7469 6f6e 616c 947d 9428 8c04 7479 7065  tional.}.(..type
+0000bcd0: 948c 0762 6f6f 6c65 616e 948c 0764 6566  ...boolean...def
+0000bce0: 6175 6c74 9489 8c0b 6465 7363 7269 7074  ault....descript
+0000bcf0: 696f 6e94 8c3e 416c 6c6f 7720 7468 6520  ion..>Allow the 
+0000bd00: 6675 6c6c 2074 7261 6e73 6665 7220 746f  full transfer to
+0000bd10: 2073 7563 6365 6564 2065 7665 6e20 6966   succeed even if
+0000bd20: 2074 6869 7320 656c 656d 656e 7420 6661   this element fa
+0000bd30: 696c 732e 9475 8c0c 7372 6353 6861 7265  ils..u..srcShare
+0000bd40: 6443 7478 947d 948c 0424 7265 6694 8c23  dCtx.}...$ref..#
+0000bd50: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+0000bd60: 656d 6173 2f55 7365 724e 616d 6553 7472  emas/UserNameStr
+0000bd70: 696e 6794 738c 0d64 6573 7453 6861 7265  ing.s..destShare
+0000bd80: 6443 7478 947d 948c 0424 7265 6694 8c23  dCtx.}...$ref..#
+0000bd90: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+0000bda0: 656d 6173 2f55 7365 724e 616d 6553 7472  emas/UserNameStr
+0000bdb0: 696e 6794 7375 758c 144e 6174 6976 654c  ing.suu..NativeL
+0000bdc0: 696e 7578 4f70 5265 7175 6573 7494 7d94  inuxOpRequest.}.
+0000bdd0: 288c 0872 6571 7569 7265 6494 5d94 288c  (..required.].(.
+0000bde0: 0861 7267 756d 656e 7494 8c09 6f70 6572  .argument...oper
+0000bdf0: 6174 696f 6e94 658c 0474 7970 6594 8c06  ation.e..type...
+0000be00: 6f62 6a65 6374 948c 0a70 726f 7065 7274  object...propert
+0000be10: 6965 7394 7d94 288c 096f 7065 7261 7469  ies.}.(..operati
+0000be20: 6f6e 947d 9428 8c04 7479 7065 948c 0673  on.}.(..type...s
+0000be30: 7472 696e 6794 8c04 656e 756d 945d 9428  tring...enum.].(
+0000be40: 8c05 4348 4d4f 4494 8c05 4348 4f57 4e94  ..CHMOD...CHOWN.
+0000be50: 8c05 4348 4752 5094 6575 8c08 6172 6775  ..CHGRP.eu..argu
+0000be60: 6d65 6e74 947d 9428 8c04 7479 7065 948c  ment.}.(..type..
+0000be70: 0673 7472 696e 6794 8c0b 6465 7363 7269  .string...descri
+0000be80: 7074 696f 6e94 8c23 4172 6775 6d65 6e74  ption..#Argument
+0000be90: 2066 6f72 206e 6174 6976 6520 6c69 6e75   for native linu
+0000bea0: 7820 6f70 6572 6174 696f 6e94 7575 758c  x operation.uuu.
+0000beb0: 194e 6174 6976 654c 696e 7578 5365 7446  .NativeLinuxSetF
+0000bec0: 6163 6c52 6571 7565 7374 947d 9428 8c08  aclRequest.}.(..
+0000bed0: 7265 7175 6972 6564 945d 9428 8c09 6f70  required.].(..op
+0000bee0: 6572 6174 696f 6e94 8c09 6163 6c53 7472  eration...aclStr
+0000bef0: 696e 6794 658c 0474 7970 6594 8c06 6f62  ing.e..type...ob
+0000bf00: 6a65 6374 948c 0a70 726f 7065 7274 6965  ject...propertie
+0000bf10: 7394 7d94 288c 096f 7065 7261 7469 6f6e  s.}.(..operation
+0000bf20: 947d 9428 8c04 7479 7065 948c 0673 7472  .}.(..type...str
+0000bf30: 696e 6794 8c04 656e 756d 945d 9428 8c03  ing...enum.].(..
+0000bf40: 4144 4494 8c06 5245 4d4f 5645 948c 0e52  ADD...REMOVE...R
+0000bf50: 454d 4f56 455f 4445 4641 554c 5494 8c0a  EMOVE_DEFAULT...
+0000bf60: 5245 4d4f 5645 5f41 4c4c 9465 758c 0f72  REMOVE_ALL.eu..r
+0000bf70: 6563 7572 7369 6f6e 4d65 7468 6f64 947d  ecursionMethod.}
+0000bf80: 9428 8c04 7479 7065 948c 0673 7472 696e  .(..type...strin
+0000bf90: 6794 8c04 656e 756d 945d 9428 8c04 4e4f  g...enum.].(..NO
+0000bfa0: 4e45 948c 0850 4859 5349 4341 4c94 8c07  NE...PHYSICAL...
+0000bfb0: 4c4f 4749 4341 4c94 658c 0764 6566 6175  LOGICAL.e..defau
+0000bfc0: 6c74 948c 044e 4f4e 4594 8c0b 6465 7363  lt...NONE...desc
+0000bfd0: 7269 7074 696f 6e94 8c70 5265 6375 7273  ription..pRecurs
+0000bfe0: 696f 6e20 6d61 7920 6265 2073 6574 2074  ion may be set t
+0000bff0: 6f20 7068 7973 6963 616c 2028 646f 6e27  o physical (don'
+0000c000: 7420 666f 6c6c 6f77 2073 796d 6c69 6e6b  t follow symlink
+0000c010: 7329 206f 720a 6c6f 6769 6361 6c20 2866  s) or.logical (f
+0000c020: 6f6c 6c6f 7720 7379 6d6c 696e 6b73 292c  ollow symlinks),
+0000c030: 206f 7220 6e6f 6e65 2028 646f 6e27 7420   or none (don't 
+0000c040: 7265 6375 7273 6529 2e0a 9475 8c09 6163  recurse)...u..ac
+0000c050: 6c53 7472 696e 6794 7d94 288c 0474 7970  lString.}.(..typ
+0000c060: 6594 8c06 7374 7269 6e67 948c 0b64 6573  e...string...des
+0000c070: 6372 6970 7469 6f6e 948c c673 7065 6369  cription...speci
+0000c080: 6669 6573 2074 6865 2061 6374 7561 6c20  fies the actual 
+0000c090: 6163 6c20 7374 7269 6e67 2074 6f20 7365  acl string to se
+0000c0a0: 742e 2020 4d75 6c74 6970 6c65 2061 636c  t.  Multiple acl
+0000c0b0: 7320 6d61 7920 6265 2073 6570 6172 6174  s may be separat
+0000c0c0: 6564 2062 7920 0a63 6f6d 6d61 732e 0a45  ed by .commas..E
+0000c0d0: 7861 6d70 6c65 7320 2d20 7573 6572 3a6d  xamples - user:m
+0000c0e0: 7975 7365 723a 7277 782c 6772 6f75 7020  yuser:rwx,group 
+0000c0f0: 0a20 2020 2020 2020 2020 2020 6772 6f75  .           grou
+0000c100: 703a 6d79 6772 6f75 703a 7277 200a 2020  p:mygroup:rw .  
+0000c110: 2020 2020 2020 2020 2075 7365 723a 6d79           user:my
+0000c120: 7573 6572 3a72 7778 2c67 726f 7570 2c67  user:rwx,group,g
+0000c130: 726f 7570 3a6d 7967 726f 7570 3a72 7720  roup:mygroup:rw 
+0000c140: 0a94 7575 758c 1343 7265 6174 6550 6f73  ..uuu..CreatePos
+0000c150: 7449 7452 6571 7565 7374 947d 9428 8c04  tItRequest.}.(..
+0000c160: 7479 7065 948c 066f 626a 6563 7494 8c0a  type...object...
+0000c170: 7072 6f70 6572 7469 6573 947d 9428 8c0b  properties.}.(..
+0000c180: 616c 6c6f 7765 6455 7365 7394 7d94 288c  allowedUses.}.(.
+0000c190: 0474 7970 6594 8c07 696e 7465 6765 7294  .type...integer.
+0000c1a0: 8c06 666f 726d 6174 948c 0569 6e74 3332  ..format...int32
+0000c1b0: 948c 0b64 6573 6372 6970 7469 6f6e 948c  ...description..
+0000c1c0: b84e 756d 6265 7220 6f66 2074 696d 6573  .Number of times
+0000c1d0: 2074 6861 7420 7468 6520 6e65 7720 506f   that the new Po
+0000c1e0: 7374 4974 2063 616e 2062 6520 7265 6465  stIt can be rede
+0000c1f0: 656d 6564 2e20 5468 650a 6465 6661 756c  emed. The.defaul
+0000c200: 7420 6973 206f 6e65 2075 7365 2e20 2053  t is one use.  S
+0000c210: 6574 7469 6e67 2074 6865 2076 616c 7565  etting the value
+0000c220: 2074 6f20 2d31 2028 6e65 6761 7469 7665   to -1 (negative
+0000c230: 206f 6e65 290a 7769 6c6c 2061 6c6c 6f77   one).will allow
+0000c240: 2074 6865 2050 6f73 7449 7420 746f 2062   the PostIt to b
+0000c250: 6520 7265 6465 656d 6564 2061 6e20 756e  e redeemed an un
+0000c260: 6c69 6d69 7465 6420 6e75 6d62 6572 206f  limited number o
+0000c270: 660a 7469 6d65 732e 0a94 8c07 6465 6661  f.times.....defa
+0000c280: 756c 7494 4b01 758c 0c76 616c 6964 5365  ult.K.u..validSe
+0000c290: 636f 6e64 7394 7d94 288c 0474 7970 6594  conds.}.(..type.
+0000c2a0: 8c06 7374 7269 6e67 948c 0666 6f72 6d61  ..string...forma
+0000c2b0: 7494 8c05 696e 7433 3294 8c0b 6465 7363  t...int32...desc
+0000c2c0: 7269 7074 696f 6e94 8c42 4e75 6d62 6572  ription..BNumber
+0000c2d0: 206f 6620 7365 636f 6e64 7320 756e 7469   of seconds unti
+0000c2e0: 6c20 7468 6520 506f 7374 4974 2065 7870  l the PostIt exp
+0000c2f0: 6972 6573 2e20 200a 4465 6661 756c 7420  ires.  .Default 
+0000c300: 6973 2033 3020 6461 7973 2e0a 948c 0764  is 30 days.....d
+0000c310: 6566 6175 6c74 944a 008d 2700 7575 758c  efault.J..'.uuu.
+0000c320: 1355 7064 6174 6550 6f73 7449 7452 6571  .UpdatePostItReq
+0000c330: 7565 7374 947d 9428 8c04 7479 7065 948c  uest.}.(..type..
+0000c340: 066f 626a 6563 7494 8c0a 7072 6f70 6572  .object...proper
+0000c350: 7469 6573 947d 9428 8c0b 616c 6c6f 7765  ties.}.(..allowe
+0000c360: 6455 7365 7394 7d94 288c 0474 7970 6594  dUses.}.(..type.
+0000c370: 8c07 696e 7465 6765 7294 8c06 666f 726d  ..integer...form
+0000c380: 6174 948c 0569 6e74 3332 948c 0b64 6573  at...int32...des
+0000c390: 6372 6970 7469 6f6e 948c 344e 756d 6265  cription..4Numbe
+0000c3a0: 7220 6f66 2074 696d 6573 2074 6861 7420  r of times that 
+0000c3b0: 7468 6520 6e65 7720 506f 7374 4974 2063  the new PostIt c
+0000c3c0: 616e 2062 6520 7265 6465 656d 6564 2e94  an be redeemed..
+0000c3d0: 758c 0a65 7870 6972 6174 696f 6e94 7d94  u..expiration.}.
+0000c3e0: 288c 0474 7970 6594 8c06 7374 7269 6e67  (..type...string
+0000c3f0: 948c 0666 6f72 6d61 7494 8c09 6461 7465  ...format...date
+0000c400: 2d74 696d 6594 8c0b 6465 7363 7269 7074  -time...descript
+0000c410: 696f 6e94 8c1e 4578 7069 7261 7469 6f6e  ion...Expiration
+0000c420: 2064 6174 6520 6f66 2074 6865 2050 6f73   date of the Pos
+0000c430: 7449 742e 9475 8c09 756e 6c69 6d69 7465  tIt..u..unlimite
+0000c440: 6494 7d94 288c 0474 7970 6594 8c07 626f  d.}.(..type...bo
+0000c450: 6f6c 6561 6e94 8c0b 6465 7363 7269 7074  olean...descript
+0000c460: 696f 6e94 8c44 4966 2073 6574 2074 6f20  ion..DIf set to 
+0000c470: 7472 7565 2c20 7468 6973 2050 6f73 7449  true, this PostI
+0000c480: 7420 7769 6c6c 2068 6176 6520 756e 6c69  t will have unli
+0000c490: 6d69 7465 6420 7573 6573 2061 6e64 206e  mited uses and n
+0000c4a0: 6f74 2065 7870 6972 652e 9475 7575 8c09  ot expire..uuu..
+0000c4b0: 5265 7370 4261 7369 6394 7d94 288c 0474  RespBasic.}.(..t
+0000c4c0: 7970 6594 8c06 6f62 6a65 6374 948c 0a70  ype...object...p
+0000c4d0: 726f 7065 7274 6965 7394 7d94 288c 0673  roperties.}.(..s
+0000c4e0: 7461 7475 7394 7d94 8c04 7479 7065 948c  tatus.}...type..
+0000c4f0: 0673 7472 696e 6794 738c 076d 6573 7361  .string.s..messa
+0000c500: 6765 947d 948c 0474 7970 6594 8c06 7374  ge.}...type...st
+0000c510: 7269 6e67 9473 8c07 7665 7273 696f 6e94  ring.s..version.
+0000c520: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+0000c530: 6794 738c 0672 6573 756c 7494 7d94 8c04  g.s..result.}...
+0000c540: 7479 7065 948c 066f 626a 6563 7494 738c  type...object.s.
+0000c550: 086d 6574 6164 6174 6194 7d94 8c04 7479  .metadata.}...ty
+0000c560: 7065 948c 066f 626a 6563 7494 7375 758c  pe...object.suu.
+0000c570: 1246 696c 6553 7472 696e 6752 6573 706f  .FileStringRespo
+0000c580: 6e73 6594 7d94 288c 0474 7970 6594 8c06  nse.}.(..type...
+0000c590: 6f62 6a65 6374 948c 0a70 726f 7065 7274  object...propert
+0000c5a0: 6965 7394 7d94 288c 0673 7461 7475 7394  ies.}.(..status.
+0000c5b0: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+0000c5c0: 6794 738c 076d 6573 7361 6765 947d 948c  g.s..message.}..
+0000c5d0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+0000c5e0: 8c06 7265 7375 6c74 947d 948c 0474 7970  ..result.}...typ
+0000c5f0: 6594 8c06 7374 7269 6e67 9473 8c07 7665  e...string.s..ve
+0000c600: 7273 696f 6e94 7d94 8c04 7479 7065 948c  rsion.}...type..
+0000c610: 0673 7472 696e 6794 738c 086d 6574 6164  .string.s..metad
+0000c620: 6174 6194 7d94 8c04 7479 7065 948c 066f  ata.}...type...o
+0000c630: 626a 6563 7494 7375 758c 0e53 7472 696e  bject.suu..Strin
+0000c640: 6752 6573 706f 6e73 6594 7d94 288c 0474  gResponse.}.(..t
+0000c650: 7970 6594 8c06 6f62 6a65 6374 948c 0a70  ype...object...p
+0000c660: 726f 7065 7274 6965 7394 7d94 288c 0673  roperties.}.(..s
+0000c670: 7461 7475 7394 7d94 8c04 7479 7065 948c  tatus.}...type..
+0000c680: 0673 7472 696e 6794 738c 076d 6573 7361  .string.s..messa
+0000c690: 6765 947d 948c 0474 7970 6594 8c06 7374  ge.}...type...st
+0000c6a0: 7269 6e67 9473 8c06 7265 7375 6c74 947d  ring.s..result.}
+0000c6b0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+0000c6c0: 9473 8c07 7665 7273 696f 6e94 7d94 8c04  .s..version.}...
+0000c6d0: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
+0000c6e0: 086d 6574 6164 6174 6194 7d94 8c04 7479  .metadata.}...ty
+0000c6f0: 7065 948c 066f 626a 6563 7494 7375 758c  pe...object.suu.
+0000c700: 0a52 6573 7053 7472 696e 6794 7d94 288c  .RespString.}.(.
+0000c710: 0474 7970 6594 8c06 6f62 6a65 6374 948c  .type...object..
+0000c720: 0a70 726f 7065 7274 6965 7394 7d94 288c  .properties.}.(.
+0000c730: 0673 7461 7475 7394 7d94 8c04 7479 7065  .status.}...type
+0000c740: 948c 0673 7472 696e 6794 738c 076d 6573  ...string.s..mes
+0000c750: 7361 6765 947d 948c 0474 7970 6594 8c06  sage.}...type...
+0000c760: 7374 7269 6e67 9473 8c06 7265 7375 6c74  string.s..result
+0000c770: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000c780: 6e67 9473 8c07 7665 7273 696f 6e94 7d94  ng.s..version.}.
+0000c790: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000c7a0: 738c 086d 6574 6164 6174 6194 7d94 8c04  s..metadata.}...
+0000c7b0: 7479 7065 948c 066f 626a 6563 7494 7375  type...object.su
+0000c7c0: 758c 0f52 6573 7043 6861 6e67 6543 6f75  u..RespChangeCou
+0000c7d0: 6e74 947d 9428 8c04 7479 7065 948c 066f  nt.}.(..type...o
+0000c7e0: 626a 6563 7494 8c0a 7072 6f70 6572 7469  bject...properti
+0000c7f0: 6573 947d 9428 8c06 7374 6174 7573 947d  es.}.(..status.}
+0000c800: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+0000c810: 9473 8c07 6d65 7373 6167 6594 7d94 8c04  .s..message.}...
+0000c820: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
+0000c830: 0776 6572 7369 6f6e 947d 948c 0474 7970  .version.}...typ
+0000c840: 6594 8c06 7374 7269 6e67 9473 8c06 7265  e...string.s..re
+0000c850: 7375 6c74 947d 948c 0424 7265 6694 8c26  sult.}...$ref..&
+0000c860: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+0000c870: 656d 6173 2f52 6573 756c 7443 6861 6e67  emas/ResultChang
+0000c880: 6543 6f75 6e74 9473 8c08 6d65 7461 6461  eCount.s..metada
+0000c890: 7461 947d 948c 0474 7970 6594 8c06 6f62  ta.}...type...ob
+0000c8a0: 6a65 6374 9473 7575 8c11 5265 7375 6c74  ject.suu..Result
+0000c8b0: 4368 616e 6765 436f 756e 7494 7d94 288c  ChangeCount.}.(.
+0000c8c0: 0474 7970 6594 8c06 6f62 6a65 6374 948c  .type...object..
+0000c8d0: 0a70 726f 7065 7274 6965 7394 7d94 8c07  .properties.}...
+0000c8e0: 6368 616e 6765 7394 7d94 288c 0474 7970  changes.}.(..typ
+0000c8f0: 6594 8c07 696e 7465 6765 7294 8c06 666f  e...integer...fo
+0000c900: 726d 6174 948c 0569 6e74 3332 948c 0765  rmat...int32...e
+0000c910: 7861 6d70 6c65 944b 0175 7375 8c0c 5265  xample.K.usu..Re
+0000c920: 7370 4669 6c65 4c69 7374 947d 9428 8c04  spFileList.}.(..
+0000c930: 7479 7065 948c 066f 626a 6563 7494 8c0a  type...object...
+0000c940: 7072 6f70 6572 7469 6573 947d 9428 8c06  properties.}.(..
+0000c950: 7374 6174 7573 947d 948c 0474 7970 6594  status.}...type.
+0000c960: 8c06 7374 7269 6e67 9473 8c07 6d65 7373  ..string.s..mess
+0000c970: 6167 6594 7d94 8c04 7479 7065 948c 0673  age.}...type...s
+0000c980: 7472 696e 6794 738c 0672 6573 756c 7494  tring.s..result.
+0000c990: 7d94 288c 0474 7970 6594 8c05 6172 7261  }.(..type...arra
+0000c9a0: 7994 8c05 6974 656d 7394 7d94 8c04 2472  y...items.}...$r
+0000c9b0: 6566 948c 1d23 2f63 6f6d 706f 6e65 6e74  ef...#/component
+0000c9c0: 732f 7363 6865 6d61 732f 4669 6c65 496e  s/schemas/FileIn
+0000c9d0: 666f 9473 758c 0776 6572 7369 6f6e 947d  fo.su..version.}
+0000c9e0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+0000c9f0: 9473 8c08 6d65 7461 6461 7461 947d 948c  .s..metadata.}..
+0000ca00: 0474 7970 6594 8c06 6f62 6a65 6374 9473  .type...object.s
+0000ca10: 7575 8c14 4669 6c65 5374 6174 496e 666f  uu..FileStatInfo
+0000ca20: 5265 7370 6f6e 7365 947d 9428 8c04 7479  Response.}.(..ty
+0000ca30: 7065 948c 066f 626a 6563 7494 8c0a 7072  pe...object...pr
+0000ca40: 6f70 6572 7469 6573 947d 9428 8c06 7374  operties.}.(..st
+0000ca50: 6174 7573 947d 948c 0474 7970 6594 8c06  atus.}...type...
+0000ca60: 7374 7269 6e67 9473 8c07 6d65 7373 6167  string.s..messag
+0000ca70: 6594 7d94 8c04 7479 7065 948c 0673 7472  e.}...type...str
+0000ca80: 696e 6794 738c 0672 6573 756c 7494 7d94  ing.s..result.}.
+0000ca90: 8c04 2472 6566 948c 2123 2f63 6f6d 706f  ..$ref..!#/compo
+0000caa0: 6e65 6e74 732f 7363 6865 6d61 732f 4669  nents/schemas/Fi
+0000cab0: 6c65 5374 6174 496e 666f 9473 8c07 7665  leStatInfo.s..ve
+0000cac0: 7273 696f 6e94 7d94 8c04 7479 7065 948c  rsion.}...type..
+0000cad0: 0673 7472 696e 6794 738c 086d 6574 6164  .string.s..metad
+0000cae0: 6174 6194 7d94 8c04 7479 7065 948c 066f  ata.}...type...o
+0000caf0: 626a 6563 7494 7375 758c 154e 6174 6976  bject.suu..Nativ
+0000cb00: 654c 696e 7578 4f70 5265 7370 6f6e 7365  eLinuxOpResponse
+0000cb10: 947d 9428 8c04 7479 7065 948c 066f 626a  .}.(..type...obj
+0000cb20: 6563 7494 8c0a 7072 6f70 6572 7469 6573  ect...properties
+0000cb30: 947d 9428 8c06 7374 6174 7573 947d 948c  .}.(..status.}..
+0000cb40: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+0000cb50: 8c07 6d65 7373 6167 6594 7d94 8c04 7479  ..message.}...ty
+0000cb60: 7065 948c 0673 7472 696e 6794 738c 0672  pe...string.s..r
+0000cb70: 6573 756c 7494 7d94 8c04 2472 6566 948c  esult.}...$ref..
+0000cb80: 3023 2f63 6f6d 706f 6e65 6e74 732f 7363  0#/components/sc
+0000cb90: 6865 6d61 732f 4e61 7469 7665 4c69 6e75  hemas/NativeLinu
+0000cba0: 784f 7052 6573 756c 7452 6573 706f 6e73  xOpResultRespons
+0000cbb0: 6594 738c 0776 6572 7369 6f6e 947d 948c  e.s..version.}..
+0000cbc0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+0000cbd0: 8c08 6d65 7461 6461 7461 947d 948c 0474  ..metadata.}...t
+0000cbe0: 7970 6594 8c06 6f62 6a65 6374 9473 7575  ype...object.suu
+0000cbf0: 8c1b 4e61 7469 7665 4c69 6e75 784f 7052  ..NativeLinuxOpR
+0000cc00: 6573 756c 7452 6573 706f 6e73 6594 7d94  esultResponse.}.
+0000cc10: 288c 0474 7970 6594 8c06 6f62 6a65 6374  (..type...object
+0000cc20: 948c 0a70 726f 7065 7274 6965 7394 7d94  ...properties.}.
+0000cc30: 288c 0763 6f6d 6d61 6e64 947d 948c 0474  (..command.}...t
+0000cc40: 7970 6594 8c06 7374 7269 6e67 9473 8c08  ype...string.s..
+0000cc50: 6578 6974 436f 6465 947d 9428 8c04 7479  exitCode.}.(..ty
+0000cc60: 7065 948c 0769 6e74 6567 6572 948c 0666  pe...integer...f
+0000cc70: 6f72 6d61 7494 8c05 696e 7433 3294 758c  ormat...int32.u.
+0000cc80: 0673 7464 4f75 7494 7d94 8c04 7479 7065  .stdOut.}...type
+0000cc90: 948c 0673 7472 696e 6794 738c 0673 7464  ...string.s..std
+0000cca0: 4572 7294 7d94 8c04 7479 7065 948c 0673  Err.}...type...s
+0000ccb0: 7472 696e 6794 7375 758c 1a4e 6174 6976  tring.suu..Nativ
+0000ccc0: 654c 696e 7578 5365 7446 6163 6c52 6573  eLinuxSetFaclRes
+0000ccd0: 706f 6e73 6594 7d94 288c 0474 7970 6594  ponse.}.(..type.
+0000cce0: 8c06 6f62 6a65 6374 948c 0a70 726f 7065  ..object...prope
+0000ccf0: 7274 6965 7394 7d94 288c 0673 7461 7475  rties.}.(..statu
+0000cd00: 7394 7d94 8c04 7479 7065 948c 0673 7472  s.}...type...str
+0000cd10: 696e 6794 738c 076d 6573 7361 6765 947d  ing.s..message.}
+0000cd20: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+0000cd30: 9473 8c06 7265 7375 6c74 947d 948c 0424  .s..result.}...$
+0000cd40: 7265 6694 8c2d 232f 636f 6d70 6f6e 656e  ref..-#/componen
+0000cd50: 7473 2f73 6368 656d 6173 2f4e 6174 6976  ts/schemas/Nativ
+0000cd60: 654c 696e 7578 5365 7446 6163 6c52 6573  eLinuxSetFaclRes
+0000cd70: 756c 7494 738c 0776 6572 7369 6f6e 947d  ult.s..version.}
+0000cd80: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+0000cd90: 9473 8c08 6d65 7461 6461 7461 947d 948c  .s..metadata.}..
+0000cda0: 0474 7970 6594 8c06 6f62 6a65 6374 9473  .type...object.s
+0000cdb0: 7575 8c18 4e61 7469 7665 4c69 6e75 7853  uu..NativeLinuxS
+0000cdc0: 6574 4661 636c 5265 7375 6c74 947d 9428  etFaclResult.}.(
+0000cdd0: 8c04 7479 7065 948c 066f 626a 6563 7494  ..type...object.
+0000cde0: 8c0a 7072 6f70 6572 7469 6573 947d 9428  ..properties.}.(
+0000cdf0: 8c07 636f 6d6d 616e 6494 7d94 8c04 7479  ..command.}...ty
+0000ce00: 7065 948c 0673 7472 696e 6794 738c 0865  pe...string.s..e
+0000ce10: 7869 7443 6f64 6594 7d94 288c 0474 7970  xitCode.}.(..typ
+0000ce20: 6594 8c07 696e 7465 6765 7294 8c06 666f  e...integer...fo
+0000ce30: 726d 6174 948c 0569 6e74 3332 9475 8c06  rmat...int32.u..
+0000ce40: 7374 644f 7574 947d 948c 0474 7970 6594  stdOut.}...type.
+0000ce50: 8c06 7374 7269 6e67 9473 8c06 7374 6445  ..string.s..stdE
+0000ce60: 7272 947d 948c 0474 7970 6594 8c06 7374  rr.}...type...st
+0000ce70: 7269 6e67 9473 7575 8c1a 4e61 7469 7665  ring.suu..Native
+0000ce80: 4c69 6e75 7847 6574 4661 636c 5265 7370  LinuxGetFaclResp
+0000ce90: 6f6e 7365 947d 9428 8c04 7479 7065 948c  onse.}.(..type..
+0000cea0: 066f 626a 6563 7494 8c0a 7072 6f70 6572  .object...proper
+0000ceb0: 7469 6573 947d 9428 8c06 7374 6174 7573  ties.}.(..status
+0000cec0: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000ced0: 6e67 9473 8c07 6d65 7373 6167 6594 7d94  ng.s..message.}.
+0000cee0: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000cef0: 738c 0672 6573 756c 7494 7d94 8c05 6974  s..result.}...it
+0000cf00: 656d 7394 7d94 8c04 2472 6566 948c 2123  ems.}...$ref..!#
+0000cf10: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+0000cf20: 6d61 732f 4163 6c45 6e74 7279 496e 666f  mas/AclEntryInfo
+0000cf30: 9473 738c 0776 6572 7369 6f6e 947d 948c  .ss..version.}..
+0000cf40: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+0000cf50: 8c08 6d65 7461 6461 7461 947d 948c 0474  ..metadata.}...t
+0000cf60: 7970 6594 8c06 6f62 6a65 6374 9473 7575  ype...object.suu
+0000cf70: 8c16 4669 6c65 5065 726d 6973 7369 6f6e  ..FilePermission
+0000cf80: 5265 7370 6f6e 7365 947d 9428 8c04 7479  Response.}.(..ty
+0000cf90: 7065 948c 066f 626a 6563 7494 8c0a 7072  pe...object...pr
+0000cfa0: 6f70 6572 7469 6573 947d 9428 8c06 7374  operties.}.(..st
+0000cfb0: 6174 7573 947d 948c 0474 7970 6594 8c06  atus.}...type...
+0000cfc0: 7374 7269 6e67 9473 8c07 6d65 7373 6167  string.s..messag
+0000cfd0: 6594 7d94 8c04 7479 7065 948c 0673 7472  e.}...type...str
+0000cfe0: 696e 6794 738c 0672 6573 756c 7494 7d94  ing.s..result.}.
+0000cff0: 8c04 2472 6566 948c 2323 2f63 6f6d 706f  ..$ref..##/compo
+0000d000: 6e65 6e74 732f 7363 6865 6d61 732f 4669  nents/schemas/Fi
+0000d010: 6c65 5065 726d 6973 7369 6f6e 9473 8c07  lePermission.s..
+0000d020: 7665 7273 696f 6e94 7d94 8c04 7479 7065  version.}...type
+0000d030: 948c 0673 7472 696e 6794 738c 086d 6574  ...string.s..met
+0000d040: 6164 6174 6194 7d94 8c04 7479 7065 948c  adata.}...type..
+0000d050: 066f 626a 6563 7494 7375 758c 0d52 6573  .object.suu..Res
+0000d060: 7053 6861 7265 496e 666f 947d 9428 8c04  pShareInfo.}.(..
+0000d070: 7479 7065 948c 066f 626a 6563 7494 8c0a  type...object...
+0000d080: 7072 6f70 6572 7469 6573 947d 9428 8c06  properties.}.(..
+0000d090: 7374 6174 7573 947d 948c 0474 7970 6594  status.}...type.
+0000d0a0: 8c06 7374 7269 6e67 9473 8c07 6d65 7373  ..string.s..mess
+0000d0b0: 6167 6594 7d94 8c04 7479 7065 948c 0673  age.}...type...s
+0000d0c0: 7472 696e 6794 738c 0776 6572 7369 6f6e  tring.s..version
+0000d0d0: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000d0e0: 6e67 9473 8c06 7265 7375 6c74 947d 948c  ng.s..result.}..
+0000d0f0: 0424 7265 6694 8c24 232f 636f 6d70 6f6e  .$ref..$#/compon
+0000d100: 656e 7473 2f73 6368 656d 6173 2f52 6573  ents/schemas/Res
+0000d110: 756c 7453 6861 7265 496e 666f 9473 8c08  ultShareInfo.s..
+0000d120: 6d65 7461 6461 7461 947d 948c 0474 7970  metadata.}...typ
+0000d130: 6594 8c06 6f62 6a65 6374 9473 7575 8c0f  e...object.suu..
+0000d140: 5265 7375 6c74 5368 6172 6549 6e66 6f94  ResultShareInfo.
+0000d150: 7d94 288c 0474 7970 6594 8c06 6f62 6a65  }.(..type...obje
+0000d160: 6374 948c 0a70 726f 7065 7274 6965 7394  ct...properties.
+0000d170: 7d94 288c 0869 7350 7562 6c69 6394 7d94  }.(..isPublic.}.
+0000d180: 288c 0474 7970 6594 8c07 626f 6f6c 6561  (..type...boolea
+0000d190: 6e94 8c0b 6465 7363 7269 7074 696f 6e94  n...description.
+0000d1a0: 8c27 496e 6469 6361 7465 7320 6769 7665  .'Indicates give
+0000d1b0: 6e20 7061 7468 2069 7320 7368 6172 6564  n path is shared
+0000d1c0: 2070 7562 6c69 636c 7994 758c 0c69 7350   publicly.u..isP
+0000d1d0: 7562 6c69 6350 6174 6894 7d94 288c 0474  ublicPath.}.(..t
+0000d1e0: 7970 6594 8c06 7374 7269 6e67 948c 0b64  ype...string...d
+0000d1f0: 6573 6372 6970 7469 6f6e 948c 3a50 6174  escription..:Pat
+0000d200: 6820 7468 6174 2072 6573 756c 7465 6420  h that resulted 
+0000d210: 696e 2073 7065 6369 6669 6564 2070 6174  in specified pat
+0000d220: 6820 6265 696e 6720 7368 6172 6564 2070  h being shared p
+0000d230: 7562 6c69 636c 7994 758c 0775 7365 7253  ublicly.u..userS
+0000d240: 6574 947d 9428 8c04 7479 7065 948c 0561  et.}.(..type...a
+0000d250: 7272 6179 948c 0b64 6573 6372 6970 7469  rray...descripti
+0000d260: 6f6e 948c 2a53 6574 206f 6620 7573 6572  on..*Set of user
+0000d270: 7320 7769 7468 2077 686f 6d20 7468 6520  s with whom the 
+0000d280: 7061 7468 2069 7320 7368 6172 6564 2e94  path is shared..
+0000d290: 8c05 6974 656d 7394 7d94 8c04 2472 6566  ..items.}...$ref
+0000d2a0: 948c 2323 2f63 6f6d 706f 6e65 6e74 732f  ..##/components/
+0000d2b0: 7363 6865 6d61 732f 5573 6572 4e61 6d65  schemas/UserName
+0000d2c0: 5374 7269 6e67 9473 758c 1075 7365 7253  String.su..userS
+0000d2d0: 6861 7265 496e 666f 5365 7494 7d94 288c  hareInfoSet.}.(.
+0000d2e0: 0474 7970 6594 8c05 6172 7261 7994 8c0b  .type...array...
+0000d2f0: 6465 7363 7269 7074 696f 6e94 8c33 4c69  description..3Li
+0000d300: 7374 206f 6620 6164 6469 7469 6f6e 616c  st of additional
+0000d310: 2073 6861 7265 2069 6e66 6f72 6d61 7469   share informati
+0000d320: 6f6e 2066 6f72 2065 6163 6820 7573 6572  on for each user
+0000d330: 2e94 8c05 6974 656d 7394 7d94 8c04 2472  ....items.}...$r
+0000d340: 6566 948c 2223 2f63 6f6d 706f 6e65 6e74  ef.."#/component
+0000d350: 732f 7363 6865 6d61 732f 5573 6572 5368  s/schemas/UserSh
+0000d360: 6172 6549 6e66 6f94 7375 7575 8c0d 5573  areInfo.suuu..Us
+0000d370: 6572 5368 6172 6549 6e66 6f94 7d94 288c  erShareInfo.}.(.
+0000d380: 0474 7970 6594 8c06 6f62 6a65 6374 948c  .type...object..
+0000d390: 0a70 726f 7065 7274 6965 7394 7d94 288c  .properties.}.(.
+0000d3a0: 0875 7365 726e 616d 6594 7d94 8c04 2472  .username.}...$r
+0000d3b0: 6566 948c 2323 2f63 6f6d 706f 6e65 6e74  ef..##/component
+0000d3c0: 732f 7363 6865 6d61 732f 5573 6572 4e61  s/schemas/UserNa
+0000d3d0: 6d65 5374 7269 6e67 9473 8c04 7061 7468  meString.s..path
+0000d3e0: 947d 9428 8c04 7479 7065 948c 0673 7472  .}.(..type...str
+0000d3f0: 696e 6794 8c0b 6465 7363 7269 7074 696f  ing...descriptio
+0000d400: 6e94 8c3f 5061 7468 2074 6861 7420 7265  n..?Path that re
+0000d410: 7375 6c74 6564 2069 6e20 7370 6563 6966  sulted in specif
+0000d420: 6965 6420 7061 7468 2062 6569 6e67 2073  ied path being s
+0000d430: 6861 7265 6420 7769 7468 2074 6865 2075  hared with the u
+0000d440: 7365 7294 7575 758c 1454 7261 6e73 6665  ser.uuu..Transfe
+0000d450: 7254 6173 6b52 6573 706f 6e73 6594 7d94  rTaskResponse.}.
+0000d460: 288c 0474 7970 6594 8c06 6f62 6a65 6374  (..type...object
+0000d470: 948c 0a70 726f 7065 7274 6965 7394 7d94  ...properties.}.
+0000d480: 288c 0673 7461 7475 7394 7d94 8c04 7479  (..status.}...ty
+0000d490: 7065 948c 0673 7472 696e 6794 738c 076d  pe...string.s..m
+0000d4a0: 6573 7361 6765 947d 948c 0474 7970 6594  essage.}...type.
+0000d4b0: 8c06 7374 7269 6e67 9473 8c06 7265 7375  ..string.s..resu
+0000d4c0: 6c74 947d 948c 0424 7265 6694 8c21 232f  lt.}...$ref..!#/
+0000d4d0: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+0000d4e0: 6173 2f54 7261 6e73 6665 7254 6173 6b94  as/TransferTask.
+0000d4f0: 738c 0776 6572 7369 6f6e 947d 948c 0474  s..version.}...t
+0000d500: 7970 6594 8c06 7374 7269 6e67 9473 8c08  ype...string.s..
+0000d510: 6d65 7461 6461 7461 947d 948c 0474 7970  metadata.}...typ
+0000d520: 6594 8c06 6f62 6a65 6374 9473 7575 8c18  e...object.suu..
+0000d530: 5472 616e 7366 6572 5461 736b 4c69 7374  TransferTaskList
+0000d540: 5265 7370 6f6e 7365 947d 9428 8c04 7479  Response.}.(..ty
+0000d550: 7065 948c 066f 626a 6563 7494 8c0a 7072  pe...object...pr
+0000d560: 6f70 6572 7469 6573 947d 9428 8c06 7374  operties.}.(..st
+0000d570: 6174 7573 947d 948c 0474 7970 6594 8c06  atus.}...type...
+0000d580: 7374 7269 6e67 9473 8c07 6d65 7373 6167  string.s..messag
+0000d590: 6594 7d94 8c04 7479 7065 948c 0673 7472  e.}...type...str
+0000d5a0: 696e 6794 738c 0672 6573 756c 7494 7d94  ing.s..result.}.
+0000d5b0: 288c 0474 7970 6594 8c05 6172 7261 7994  (..type...array.
+0000d5c0: 8c05 6974 656d 7394 7d94 8c04 2472 6566  ..items.}...$ref
+0000d5d0: 948c 2123 2f63 6f6d 706f 6e65 6e74 732f  ..!#/components/
+0000d5e0: 7363 6865 6d61 732f 5472 616e 7366 6572  schemas/Transfer
+0000d5f0: 5461 736b 9473 758c 0776 6572 7369 6f6e  Task.su..version
+0000d600: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000d610: 6e67 9473 8c08 6d65 7461 6461 7461 947d  ng.s..metadata.}
+0000d620: 948c 0474 7970 6594 8c06 6f62 6a65 6374  ...type...object
+0000d630: 9473 7575 8c0e 506f 7374 4974 5265 7370  .suu..PostItResp
+0000d640: 6f6e 7365 947d 9428 8c04 7479 7065 948c  onse.}.(..type..
+0000d650: 066f 626a 6563 7494 8c0a 7072 6f70 6572  .object...proper
+0000d660: 7469 6573 947d 9428 8c06 7374 6174 7573  ties.}.(..status
+0000d670: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000d680: 6e67 9473 8c07 6d65 7373 6167 6594 7d94  ng.s..message.}.
+0000d690: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000d6a0: 738c 0672 6573 756c 7494 7d94 8c04 2472  s..result.}...$r
+0000d6b0: 6566 948c 1b23 2f63 6f6d 706f 6e65 6e74  ef...#/component
+0000d6c0: 732f 7363 6865 6d61 732f 506f 7374 4974  s/schemas/PostIt
+0000d6d0: 9473 8c07 7665 7273 696f 6e94 7d94 8c04  .s..version.}...
+0000d6e0: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
+0000d6f0: 086d 6574 6164 6174 6194 7d94 8c04 7479  .metadata.}...ty
+0000d700: 7065 948c 066f 626a 6563 7494 7375 758c  pe...object.suu.
+0000d710: 1250 6f73 7449 744c 6973 7452 6573 706f  .PostItListRespo
+0000d720: 6e73 6594 7d94 288c 0474 7970 6594 8c06  nse.}.(..type...
+0000d730: 6f62 6a65 6374 948c 0a70 726f 7065 7274  object...propert
+0000d740: 6965 7394 7d94 288c 0673 7461 7475 7394  ies.}.(..status.
+0000d750: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+0000d760: 6794 738c 076d 6573 7361 6765 947d 948c  g.s..message.}..
+0000d770: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+0000d780: 8c06 7265 7375 6c74 947d 9428 8c04 7479  ..result.}.(..ty
+0000d790: 7065 948c 0561 7272 6179 948c 0569 7465  pe...array...ite
+0000d7a0: 6d73 947d 948c 0424 7265 6694 8c1b 232f  ms.}...$ref...#/
+0000d7b0: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+0000d7c0: 6173 2f50 6f73 7449 7494 7375 8c07 7665  as/PostIt.su..ve
+0000d7d0: 7273 696f 6e94 7d94 8c04 7479 7065 948c  rsion.}...type..
+0000d7e0: 0673 7472 696e 6794 738c 086d 6574 6164  .string.s..metad
+0000d7f0: 6174 6194 7d94 8c04 7479 7065 948c 066f  ata.}...type...o
+0000d800: 626a 6563 7494 7375 758c 1254 7261 6e73  bject.suu..Trans
+0000d810: 6665 7253 7461 7475 7345 6e75 6d94 7d94  ferStatusEnum.}.
+0000d820: 288c 0474 7970 6594 8c06 7374 7269 6e67  (..type...string
+0000d830: 948c 0b64 6573 6372 6970 7469 6f6e 948c  ...description..
+0000d840: 4b54 6865 2073 7461 7475 7320 6f66 2074  KThe status of t
+0000d850: 6865 2074 6173 6b2c 2073 7563 6820 6173  he task, such as
+0000d860: 2041 4343 4550 5445 442c 2049 4e5f 5052   ACCEPTED, IN_PR
+0000d870: 4f47 5245 5353 2c20 434f 4d50 4c45 5445  OGRESS, COMPLETE
+0000d880: 442c 2043 414e 4345 4c4c 4544 948c 0765  D, CANCELLED...e
+0000d890: 7861 6d70 6c65 948c 0750 454e 4449 4e47  xample...PENDING
+0000d8a0: 948c 0465 6e75 6d94 5d94 288c 0841 4343  ...enum.].(..ACC
+0000d8b0: 4550 5445 4494 8c06 5354 4147 4544 948c  EPTED...STAGED..
+0000d8c0: 0b49 4e5f 5052 4f47 5245 5353 948c 0943  .IN_PROGRESS...C
+0000d8d0: 4f4d 504c 4554 4544 948c 0943 414e 4345  OMPLETED...CANCE
+0000d8e0: 4c4c 4544 948c 0646 4149 4c45 4494 8c0a  LLED...FAILED...
+0000d8f0: 4641 494c 4544 5f4f 5054 948c 0650 4155  FAILED_OPT...PAU
+0000d900: 5345 4494 6575 8c08 5065 726d 456e 756d  SED.eu..PermEnum
+0000d910: 947d 9428 8c04 7479 7065 948c 0673 7472  .}.(..type...str
+0000d920: 696e 6794 8c04 656e 756d 945d 9428 8c04  ing...enum.].(..
+0000d930: 5245 4144 948c 064d 4f44 4946 5994 6575  READ...MODIFY.eu
+0000d940: 8c0c 4c69 7374 5479 7065 456e 756d 947d  ..ListTypeEnum.}
+0000d950: 9428 8c04 7479 7065 948c 0673 7472 696e  .(..type...strin
+0000d960: 6794 8c07 6465 6661 756c 7494 8c05 4f57  g...default...OW
+0000d970: 4e45 4494 8c04 656e 756d 945d 9428 8c05  NED...enum.].(..
+0000d980: 4f57 4e45 4494 8c03 414c 4c94 6575 7573  OWNED...ALL.euus
+0000d990: 752e                                     u.
```

### Comparing `tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-jobs.pickle` & `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-jobs.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-meta.pickle` & `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-meta.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-notifications.pickle` & `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-notifications.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-pgrest.pickle` & `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-pgrest.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-sk.pickle` & `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-sk.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-streams.pickle` & `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-streams.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-systems.pickle` & `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-systems.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tenants.pickle` & `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tenants.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tokens.pickle` & `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tokens.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-workflows.pickle` & `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-workflows.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/specs/tapis-project-tapis-client-java-dev-jobs-client-src-main-resources-jobsapi.pickle` & `tapipy-1.3.3/tapipy/specs/tapis-project-tapis-client-java-dev-jobs-client-src-main-resources-jobsapi.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/tapipy/tapis.py` & `tapipy-1.3.3/tapipy/tapis.py`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.2/setup.py` & `tapipy-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'requests>=2.20.0,<3.0.0',
  'setuptools>=21.0.0',
  'six>=1.10,<2.0',
  'urllib3>=1.26.5,<2.0.0']
 
 setup_kwargs = {
     'name': 'tapipy',
-    'version': '1.3.2',
+    'version': '1.3.3',
     'description': 'Python lib for interacting with an instance of the Tapis API Framework',
     'long_description': '# tapipy - Tapis V3 Python SDK\n\nPython library for interacting with an instance of the Tapis API Framework.\n\nThe library is automatically generated by referencing the OpenAPI spec files which  a `Tapis` object built from the OpenAPI spec files from TACC\'s Tapis services. With this functionality a user is able to authorize itself with the `Tapis` object and have a \'live\' library in order to interact with Tapis services.\n\n## Development\n\nThis project is under active development, exploring different approaches to SDK generation.\n\n## Installation\nTapipy is packaged on [pypi](https://pypi.org/project/tapipy/) and can be installed with pip.\n\n```\npip install tapipy\n```\n\n\n## Usage\nTapipy\'s Tapis object first must be initialized in order to be used.\nA basic example of logging in with a user account is below.\n\n```\n# Import the Tapis object\nfrom tapipy.tapis import Tapis\n\n# Log into you the Tapis service by providing user/pass and the base url of your tenant. For example, to interact with the tacc tenant --\nt = Tapis(base_url=\'https://tacc.tapis.io\',\n          username=\'myuser\',\n          password=\'mypass\')\n\t  \n# Get tokens that will be used for authentication function calls\nt.get_tokens()\n```\n\nNow you have a Tapis object that is authenticated and able to call Tapis service endpoints. It\'s useful to know that the Tapis object will automatically refresh it\'s token if it is deemed appropriate, so the object should stay in the good graces of Tapis indefinitely.\n\nNow in order to use the Tapis object you can reference the [Tapis Framework](https://tapis-project.github.io/live-docs/) to browse all functions. For example, if I wanted to use the SK service in order to check if a user has a specific role I would find the function on the site (which is just a better way to look at the json specs).\n\nWith the site I can see that I need to use my Tapis object, initialized as `t`, access `sk`, and then use the `hasRole` function with the required inputs as follows.\n```\nt.sk.hasRole(tenant=\'dev\', user=\'_testuser\', roleName=\'Do you have this role?\')\n```\n\n### Special Query Parameters and Headers\nFor the most part, arguments that can or should be passed to a Tapis endpoint are described in the OpenAPI \ndefinition files and recognized automatically by `tapipy`. However, due to limitations in what can be expressed\nin OpenAPI, there are some paramaters that are not defined in the definition files; for example, the search\nparameters for various endpoints.\n\nTo accommodate these cases, `tapipy` recognizes two special keyword arguments to all of its methods that\ncorrespond to Tapis API calls (i.e., all of its "operations"). They are:\n\n  * `_tapis_headers` -- dictionary-like object of header names (keys) and vales.\n  * `_tapis_query_parameters` -- dictionary-like object of query parameter names (keys) and values.\n\nUse the above two special arguments for passing headers (respectively, query parameters) that are not specified\nin the OpenAPI definition of an endpoint.\n\nFor example, I can issue a search using the following syntax:\n\n```\nt.jobs.getJobSearchList(limit=5, orderBy=\'lastUpdated(desc),name(asc)\', _tapis_query_parameters={\'key\': \'value\'})\n```\n\n# Development Docs\n## Running the tests\n\nTests resources are contained within the `test` directory. `Dockerfile-tests` is at root.\n1. Build the test docker image: `docker build -t tapis/tapipy-tests -f Dockerfile-tests .`\n2. Run these tests using the built docker image: `docker run -it --rm -e username=<dev_user> -e password=<dev_pass> tapis/tapipy-tests`\n\n\n## Important Parameters to Know\n\nThe `tapipy` package allows for spec file customization in Tapis object initialization:\n* resource_set: str \n\t* Determines which set of resource to use, master or dev, defaults to master.\n\t* Important to note that if a custom_spec_dictionary is used, it is appended to this resource_set.\n\t\t* For example, you would set master and then specify a custom specs that will be added on.\n* custom_spec_dict: {resource_name: str, resource_url: str}\n\t* Allows users to modify the base resource set urls.\n\t\t* e.g. I can specify actor as a resource name and change the url.\n\t* Also allows users to add new resources to the set.\n\t\t* e.g. I can add a new resource named "test" with a  custom url.\n\t\t* Important that know that any new specs will be downloaded and added to the cache\n\t\t\t* No need to specify download_latest_specs or update spec files.\n\t* ALLOWS LOCAL RESOURCES!\n\t\t* Specify an absolute path in the dict with `local:` prefixing it and tapipy will load in a local OpenAPI v3 yml spec file.\n\t\t* `custom_spec_dict={\'cactus\': \'local: /home/tapis/myfolder/cactusSpec.yml\'}`\n* download_latest_specs: bool\n\t* Allows users to re-download all specs regardless on if they already exist in the cache. Defaulted to False\n\t* This will happen every time the Tapis object is initialized, it\'s a tad slower, and can cause live updates to specs.\n\t\t* As such, be warned. There are functions to update spec files below.\n* spec_dir: str\n\t* Allows users to specify folder to save specs to. Defaults to none which uses Tapipy\'s package folder.\n\t* If you are updating specs it\'s wise to use a different folder in order to not modify the base specs.\n\nThe following is an example of some custom parameter setting. As you can see, the abaco resource will now use the spec at `URL#1`, overwriting the resource definition in the master resource set, it\'ll download it if it doesn\'t exist. The same for the longhorn resource. This means that the Tapis object will now have access to all specs in master like normal, but with a modified abaco and with a new longhorn resource. All of these are stored at the new spec_dir because I don\'t want to accidentally overwrite any base specs if I call `update_spec_cache()` later (talked about in the next section).\n```\nfrom tapipy.tapis import Tapis\n\nt = Tapis(base_url=\'https://admin.develop.tapis.io\',\n          tenant_id=\'admin\',\n          username=\'username\',\n          account_type=\'user\',\n          password=\'password\',\n          resource_set=\'admin\',\n          custom_spec_dict={\'abaco\': \'URL#1\',\n                            \'longhorn\': \'URL#2\'},\n                            \'cactus\': \'local: /home/tapis/myfolder/cactusSpec.yml\'},\n          spec_dir=\'/home/username/tapipy_specs\')\nt.get_tokens()\n```\n\n## Update Specs Files\n\nThe Tapipy package now uses a cache to organize spec dictionaries as pickled files and has the ability to accept custom spec files. By default Tapipy keeps a set of base spec files in the `%tapipy%/specs` folder. These specs are pre-pickled at package creation time.\n\nIn order to update all default spec files a user can use the `update_spec_cache()` function. Said function\'s definition is below. If no resources are provided the function will download all default spec urls in the RESOURCES object in `%tapipy%/tapipy/tapis.py` file.\n```\nResources = Dict[ResourceName, ResourceUrl]\nupdate_spec_cache(resources: Resources = None, spec_dir: str = None)\n```\nUsers are able to specify custom resources to download by providing their own resource dictionary. For example, providing `{\'actors\': \'URLToMyActorDictionary\'}` would update that spec.\n\nUsers can also specify here where to update the spec with the `spec_dir` variable.\n\nThe Tapis object itself also has a `update_spec_cache()` function that takes the Tapis parameters given at startup and updates the spec cache. Meaning that if the Tapis object was given a custom dictionary, the `update_spec_cache()` function would update it without the need for setting parameters.\n```\nt.update_spec_cache()\n```\n\n## Build instructions\n\nBuilding is done with poetry as follows:\n```\npip install poetry\npoetry install\n```\nThis installs `tapipy` to a virtual environment. Run a shell in this environment with:\n```\npoetry shell\n```\n\nTo install locally (not in a virtual environment):\n```\npip install poetry\npoetry build\ncd dists\npip install *.whl\n```\n\n## PyPi Push Instructions\n\n```\npoetry build\npoetry publish\n```\n\n## Archive Usage\nTODO - provide working examples, e.g., \n```\nimport tapipy\nt = tapipy.Tapis(base_url=\'http://localhost:5001\')\nreq = t.tokens.NewTokenRequest(token_type=\'service\', token_tenant_id=\'dev\', token_username=\'admin\')\nt.tokens.create_token(req)\n\nimport openapi_client\nconfiguration = openapi_client.Configuration()\nconfiguration.host = \'http://localhost:5001\'\napi_instance = openapi_client.TokensApi(openapi_client.ApiClient(configuration))\n\nnew_token = openapi_client.NewTokenRequest(token_type=\'service\', token_tenant_id=\'dev\', token_username=\'admin\')\n\nresp = api_instance.create_token(new_token)\njwt = resp.get(\'result\').get(\'access_token\').get(\'access_token\')\n```\n',
     'author': 'Joe Stubbs',
     'author_email': 'jstubbs@tacc.utexas.edu',
     'maintainer': 'Joe Stubbs',
     'maintainer_email': 'jstubbs@tacc.utexas.edu',
     'url': 'https://github.com/tapis-project/tapipy',
```

### Comparing `tapipy-1.3.2/PKG-INFO` & `tapipy-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapipy
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python lib for interacting with an instance of the Tapis API Framework
 Home-page: https://github.com/tapis-project/tapipy
 License: BSD-4-Clause
 Author: Joe Stubbs
 Author-email: jstubbs@tacc.utexas.edu
 Maintainer: Joe Stubbs
 Maintainer-email: jstubbs@tacc.utexas.edu
```

