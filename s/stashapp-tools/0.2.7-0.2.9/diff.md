# Comparing `tmp/stashapp-tools-0.2.7.tar.gz` & `tmp/stashapp-tools-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stashapp-tools-0.2.7.tar", last modified: Mon Sep 19 05:51:31 2022, max compression
+gzip compressed data, was "stashapp-tools-0.2.9.tar", last modified: Thu Sep 22 17:21:15 2022, max compression
```

## Comparing `stashapp-tools-0.2.7.tar` & `stashapp-tools-0.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 05:51:31.950499 stashapp-tools-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-09-19 05:51:24.000000 stashapp-tools-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-09-19 05:51:31.950499 stashapp-tools-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-09-19 05:51:24.000000 stashapp-tools-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-19 05:51:31.950499 stashapp-tools-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-09-19 05:51:25.000000 stashapp-tools-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 05:51:31.946499 stashapp-tools-0.2.7/stashapi/
--rw-r--r--   0 runner    (1001) docker     (121)     3056 2022-09-19 05:51:24.000000 stashapp-tools-0.2.7/stashapi/classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-09-19 05:51:24.000000 stashapp-tools-0.2.7/stashapi/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     5478 2022-09-19 05:51:24.000000 stashapp-tools-0.2.7/stashapi/marker_parse.py
--rw-r--r--   0 runner    (1001) docker     (121)     9869 2022-09-19 05:51:24.000000 stashapp-tools-0.2.7/stashapi/scrape_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    40744 2022-09-19 05:51:24.000000 stashapp-tools-0.2.7/stashapi/stashapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     9038 2022-09-19 05:51:24.000000 stashapp-tools-0.2.7/stashapi/stashapp_gql_fragments.py
--rw-r--r--   0 runner    (1001) docker     (121)     7828 2022-09-19 05:51:24.000000 stashapp-tools-0.2.7/stashapi/stashbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     1775 2022-09-19 05:51:24.000000 stashapp-tools-0.2.7/stashapi/stashbox_gql_fragments.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-09-19 05:51:24.000000 stashapp-tools-0.2.7/stashapi/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-09-19 05:51:24.000000 stashapp-tools-0.2.7/stashapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 05:51:31.950499 stashapp-tools-0.2.7/stashapp_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-09-19 05:51:31.000000 stashapp-tools-0.2.7/stashapp_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-09-19 05:51:31.000000 stashapp-tools-0.2.7/stashapp_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-19 05:51:31.000000 stashapp-tools-0.2.7/stashapp_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-19 05:51:31.000000 stashapp-tools-0.2.7/stashapp_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-19 05:51:31.000000 stashapp-tools-0.2.7/stashapp_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 17:21:15.475598 stashapp-tools-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-09-22 17:21:03.000000 stashapp-tools-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-09-22 17:21:15.475598 stashapp-tools-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      508 2022-09-22 17:21:03.000000 stashapp-tools-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-22 17:21:15.475598 stashapp-tools-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      833 2022-09-22 17:21:04.000000 stashapp-tools-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 17:21:15.475598 stashapp-tools-0.2.9/stashapi/
+-rw-r--r--   0 runner    (1001) docker     (121)     3021 2022-09-22 17:21:04.000000 stashapp-tools-0.2.9/stashapi/classes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-09-22 17:21:04.000000 stashapp-tools-0.2.9/stashapi/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5478 2022-09-22 17:21:04.000000 stashapp-tools-0.2.9/stashapi/marker_parse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9869 2022-09-22 17:21:04.000000 stashapp-tools-0.2.9/stashapi/scrape_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40926 2022-09-22 17:21:04.000000 stashapp-tools-0.2.9/stashapi/stashapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9033 2022-09-22 17:21:04.000000 stashapp-tools-0.2.9/stashapi/stashapp_gql_fragments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7808 2022-09-22 17:21:04.000000 stashapp-tools-0.2.9/stashapi/stashbox.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1775 2022-09-22 17:21:04.000000 stashapp-tools-0.2.9/stashapi/stashbox_gql_fragments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1025 2022-09-22 17:21:04.000000 stashapp-tools-0.2.9/stashapi/tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)      536 2022-09-22 17:21:04.000000 stashapp-tools-0.2.9/stashapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 17:21:15.475598 stashapp-tools-0.2.9/stashapp_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-09-22 17:21:15.000000 stashapp-tools-0.2.9/stashapp_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2022-09-22 17:21:15.000000 stashapp-tools-0.2.9/stashapp_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 17:21:15.000000 stashapp-tools-0.2.9/stashapp_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-22 17:21:15.000000 stashapp-tools-0.2.9/stashapp_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-22 17:21:15.000000 stashapp-tools-0.2.9/stashapp_tools.egg-info/top_level.txt
```

### Comparing `stashapp-tools-0.2.7/LICENSE` & `stashapp-tools-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stashapp-tools-0.2.7/PKG-INFO` & `stashapp-tools-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashapp-tools
-Version: 0.2.7
+Version: 0.2.9
 Summary: A python library for interfacing with a stashapp's API
 Home-page: https://github.com/stg-annon/stashapp-tools
 Author: stg-annon
 Author-email: 14135675+stg-annon@users.noreply.github.com
 License: MIT
 Description: # stashapp-tools
         This library primarily serves as a API wrapper for [Stash](https://github.com/stashapp/stash) written in python
```

### Comparing `stashapp-tools-0.2.7/setup.py` & `stashapp-tools-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="stashapp-tools",
-    version = "v0.2.7",
+    version = "v0.2.9",
     description="A python library for interfacing with a stashapp's API",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/stg-annon/stashapp-tools",
     author="stg-annon",
     author_email="14135675+stg-annon@users.noreply.github.com",
     license="MIT",
```

### Comparing `stashapp-tools-0.2.7/stashapi/classes.py` & `stashapp-tools-0.2.9/stashapi/classes.py`

 * *Files 15% similar despite different names*

```diff
@@ -65,34 +65,31 @@
 		query = self.__resolveFragments(query)
 
 		json_request = {'query': query}
 		if variables is not None:
 			json_request['variables'] = variables
 
 		response = requests.post(self.url, json=json_request, headers=self.headers, cookies=self.cookies)
-		
-		if response.status_code == 200:
-			result = response.json()
+		result = response.json()
+
+		for error in result.get("errors", []):
+			message = error.get("message")
+			code = error.get("extensions", {}).get("code", "GRAPHQL_ERROR")
+			path = error.get("path", "")
+			fmt_error = f"{code}: {message} {path}".strip()
+			log.error(fmt_error)
 
-			if result.get("errors"):
-				for error in result["errors"]:
-					log.error(f"GraphQL error: {error}")
-			if result.get("error"):
-				for error in result["error"]["errors"]:
-					log.error(f"GraphQL error: {error}")
-			if result.get("data"):
-				result_data = defaultify(result)
-				return result_data['data']
+		if response.status_code == 200:
+			result_data = defaultify(result.get("data"))
+			return result_data['data']
 		elif response.status_code == 401:
-			sys.exit("HTTP Error 401, Unauthorized. Cookie authentication most likely failed")
+			log.error(f"401, Unauthorized. Could not access endpoiont {self.url}. Did you provide an API key?")
 		else:
-			raise ConnectionError(
-				"GraphQL query failed:{} - {}. Query: {}. Variables: {}".format(
-					response.status_code, response.content, query, variables)
-			)
+			log.error(f"{response.status_code} query failed. {query}. Variables: {variables}")
+		sys.exit()
 
 class SQLiteWrapper:
 	conn = None
 
 	def __init__(self, db_filepath) -> None:
 		# generate uri for read-only connection, all write operations should be done from the API
 		p = Path(db_filepath).resolve()
```

### Comparing `stashapp-tools-0.2.7/stashapi/log.py` & `stashapp-tools-0.2.9/stashapi/log.py`

 * *Files identical despite different names*

### Comparing `stashapp-tools-0.2.7/stashapi/marker_parse.py` & `stashapp-tools-0.2.9/stashapi/marker_parse.py`

 * *Files identical despite different names*

### Comparing `stashapp-tools-0.2.7/stashapi/scrape_parser.py` & `stashapp-tools-0.2.9/stashapi/scrape_parser.py`

 * *Files identical despite different names*

### Comparing `stashapp-tools-0.2.7/stashapi/stashapp.py` & `stashapp-tools-0.2.9/stashapi/stashapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 		"Content-Type": "application/json",
 		"Accept": "application/json",
 		"Connection": "keep-alive",
 		"DNT": "1"
 	}
 	cookies = {}
 
-	def __init__(self, conn:dict={}, fragments:list[str]=[stashapp_gql_fragments.DEVELOP]):
+	def __init__(self, conn:dict={}, fragments:list[str]=[]):
 		global log
 
 		conn = CaseInsensitiveDict(conn)
 
 		log = conn.get("Logger", stash_logger)
 
 		# Session cookie for authentication
@@ -39,21 +39,29 @@
 		self.port = conn.get('Port', 9999)
 
 		# Stash GraphQL endpoint
 		self.url = f'{scheme}://{domain}:{self.port}/graphql'
 
 		try:
 			# test query to ensure good connection
-			version = self.stash_version()
+			build = self.stash_version()
+			version = build["version"]
 		except Exception as e:
 			log.error(f"Could not connect to Stash at {self.url}")
 			log.error(e)
 			sys.exit()
 			
-		log.debug(f'Using stash ({version["version"]}) endpoint at {self.url}')
+		log.debug(f'Using stash ({version}) endpoint at {self.url}')
+
+
+		if fragments == []:
+			if version > "v0.16.1-34":
+				fragments.append(stashapp_gql_fragments.DEVELOP)
+			else:
+				fragments.append(stashapp_gql_fragments.RELEASE_0_16_1)
 
 		self.fragments = {}
 		for fragment in fragments:
 			self.parse_fragments(fragment)
 
 	def __genric_find(self, query, item, fragment:tuple[str, str]=(None, None)):
 		item_id = None
@@ -114,15 +122,15 @@
 		return result['version']		
 
 	def get_sql_interface(self):
 		if "localhost" in self.url or "127.0.0.1" in self.url:
 			sql_file = self.call_gql("query dbPath{configuration{general{databasePath}}}")
 			return SQLiteWrapper(sql_file["configuration"]["general"]["databasePath"])
 		else:
-			raise Exception("not local stash instance cannot create sql interface")
+			raise Exception(f"cannot create sql interface on a non local stash instance ({self.url})")
 
 	def graphql_configuration(self):
 		query = """
 			query Configuration {
 				configuration {
 					...ConfigData
 				}
```

### Comparing `stashapp-tools-0.2.7/stashapi/stashapp_gql_fragments.py` & `stashapp-tools-0.2.9/stashapi/stashapp_gql_fragments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-RELEASE_0_16_0="""
+RELEASE_0_16_1="""
 fragment scrapedScene on ScrapedScene {
 	title
 	details
 	url
 	date
 	image
 	studio{ ...scrapedStudio }
@@ -452,15 +452,15 @@
 	url
 	date
 	rating
 	organized
 	o_counter
 	files { id path }
 	tags { ...stashTag }
-	galleries { id name }
+	galleries { id }
 	performers { ...stashPerformer }
 	scene_markers { ...stashSceneMarker }
 	studio{ ...stashStudio }
 	stash_ids{ endpoint stash_id }
 }
 fragment stashSceneSlim on Scene {
 	id
```

### Comparing `stashapp-tools-0.2.7/stashapi/stashbox.py` & `stashapp-tools-0.2.9/stashapi/stashbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,60 +185,57 @@
 
 		comments = [comment]
 		details = self.fetch_scene_edit_details(stash_id)
 		
 		if edit.get("tags"):
 			passed_tag_ids = edit["tags"]["ids"]
 			mode = edit["tags"]["mode"]
-			match mode:
-				case "SET":
-					details["tag_ids"] = passed_tag_ids
-					comments.append("SET Tags")
-				case "ADD":
-					details["tag_ids"].extend(passed_tag_ids)
-					comments.append(f"ADD {len(passed_tag_ids)} Tag(s)")
-				case "REMOVE":
-					details["tag_ids"] = [tid for tid in details["tag_ids"] if tid not in passed_tag_ids]
-					comments.append(f"REMOVE {len(passed_tag_ids)} Tag(s)")
+			if mode == "SET":
+				details["tag_ids"] = passed_tag_ids
+				comments.append("SET Tags")
+			if mode == "ADD":
+				details["tag_ids"].extend(passed_tag_ids)
+				comments.append(f"ADD {len(passed_tag_ids)} Tag(s)")
+			if mode == "REMOVE":
+				details["tag_ids"] = [tid for tid in details["tag_ids"] if tid not in passed_tag_ids]
+				comments.append(f"REMOVE {len(passed_tag_ids)} Tag(s)")
 
 		if edit.get("performers"):
 			passed_performer_appearances = edit["performers"]["appearances"]
 			mode = edit["performers"]["mode"]
-			match mode:
-				case "SET":
-					details["performers"] = passed_performer_appearances
-					comments.append("SET Performers")
-				case "ADD":
-					details["performers"].extend(passed_performer_appearances)
-					comments.append(f"ADD {len(passed_performer_appearances)} Performer(s)")
-				case "REMOVE":
-					remove_lookup = [p["performer_id"] for p in passed_performer_appearances]
-					details["performers"] = [p for p in details["performers"] if p["performer_id"] not in remove_lookup ]
-					comments.append(f"REMOVE {len(passed_performer_appearances)} Performer(s)")
+			if mode == "SET":
+				details["performers"] = passed_performer_appearances
+				comments.append("SET Performers")
+			if mode == "ADD":
+				details["performers"].extend(passed_performer_appearances)
+				comments.append(f"ADD {len(passed_performer_appearances)} Performer(s)")
+			if mode == "REMOVE":
+				remove_lookup = [p["performer_id"] for p in passed_performer_appearances]
+				details["performers"] = [p for p in details["performers"] if p["performer_id"] not in remove_lookup ]
+				comments.append(f"REMOVE {len(passed_performer_appearances)} Performer(s)")
 		
 		if edit.get("urls"):
 			passed_url_edits = edit["urls"]["links"]
 			mode = edit["urls"]["mode"]
-			match mode:
-				case "SET":
-					details["urls"] = passed_url_edits
-					comments.append("SET Performers")
-				case "ADD":
-					details["urls"].extend(passed_url_edits)
-					comments.append(f"ADD {len(passed_url_edits)} URL(s)")
-				case "REMOVE":
-					remove_lookup = [url["url"] for url in passed_url_edits]
-					details["urls"] = [url for url in details["urls"] if url["url"] not in remove_lookup ]
-					comments.append(f"REMOVE {len(passed_url_edits)} Performer(s)")
-				case "REPLACE":
-					for url_edit in passed_url_edits:
-						for url in details["urls"]:
-							if url["url"] == url_edit["target_url"]:
-								url["url"] = url_edit["url"]
-								comments.append(f'REPLACE {url_edit["target_url"]} with {url_edit["url"]}')
+			if mode == "SET":
+				details["urls"] = passed_url_edits
+				comments.append("SET Performers")
+			if mode == "ADD":
+				details["urls"].extend(passed_url_edits)
+				comments.append(f"ADD {len(passed_url_edits)} URL(s)")
+			if mode == "REMOVE":
+				remove_lookup = [url["url"] for url in passed_url_edits]
+				details["urls"] = [url for url in details["urls"] if url["url"] not in remove_lookup ]
+				comments.append(f"REMOVE {len(passed_url_edits)} Performer(s)")
+			if mode == "REPLACE":
+				for url_edit in passed_url_edits:
+					for url in details["urls"]:
+						if url["url"] == url_edit["target_url"]:
+							url["url"] = url_edit["url"]
+							comments.append(f'REPLACE {url_edit["target_url"]} with {url_edit["url"]}')
 
 		for attr in ["code","date","details","director","duration","studio_id","title"]:
 			if edit.get(attr):
 				details[attr] = edit[attr]
 
 		comment = "; ".join(comments)
 		query = """mutation SceneEdit($sceneData: SceneEditInput!) { sceneEdit(input: $sceneData) { id } }"""
```

### Comparing `stashapp-tools-0.2.7/stashapi/stashbox_gql_fragments.py` & `stashapp-tools-0.2.9/stashapi/stashbox_gql_fragments.py`

 * *Files identical despite different names*

### Comparing `stashapp-tools-0.2.7/stashapi/types.py` & `stashapp-tools-0.2.9/stashapi/types.py`

 * *Files identical despite different names*

### Comparing `stashapp-tools-0.2.7/stashapp_tools.egg-info/PKG-INFO` & `stashapp-tools-0.2.9/stashapp_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashapp-tools
-Version: 0.2.7
+Version: 0.2.9
 Summary: A python library for interfacing with a stashapp's API
 Home-page: https://github.com/stg-annon/stashapp-tools
 Author: stg-annon
 Author-email: 14135675+stg-annon@users.noreply.github.com
 License: MIT
 Description: # stashapp-tools
         This library primarily serves as a API wrapper for [Stash](https://github.com/stashapp/stash) written in python
```

