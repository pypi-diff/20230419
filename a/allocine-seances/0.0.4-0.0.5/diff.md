# Comparing `tmp/allocine-seances-0.0.4.tar.gz` & `tmp/allocine-seances-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allocine-seances-0.0.4.tar", last modified: Sat Apr 15 18:36:10 2023, max compression
+gzip compressed data, was "allocine-seances-0.0.5.tar", last modified: Wed Apr 19 17:52:44 2023, max compression
```

## Comparing `allocine-seances-0.0.4.tar` & `allocine-seances-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 18:36:10.165266 allocine-seances-0.0.4/
--rw-rw-rw-   0        0        0     1088 2023-04-15 16:16:47.000000 allocine-seances-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     4607 2023-04-15 18:36:10.164264 allocine-seances-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2779 2023-04-15 18:32:35.000000 allocine-seances-0.0.4/README.md
--rw-rw-rw-   0        0        0      721 2023-04-15 18:35:45.000000 allocine-seances-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 18:36:10.165266 allocine-seances-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 18:36:10.136269 allocine-seances-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:36:10.143264 allocine-seances-0.0.4/src/allocineAPI/
--rw-rw-rw-   0        0        0        0 2023-04-15 16:02:27.000000 allocine-seances-0.0.4/src/allocineAPI/__init__.py
--rw-rw-rw-   0        0        0     6200 2023-04-15 18:28:42.000000 allocine-seances-0.0.4/src/allocineAPI/allocineAPI.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:36:10.163265 allocine-seances-0.0.4/src/allocine_seances.egg-info/
--rw-rw-rw-   0        0        0     4607 2023-04-15 18:36:10.000000 allocine-seances-0.0.4/src/allocine_seances.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-04-15 18:36:10.000000 allocine-seances-0.0.4/src/allocine_seances.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 18:36:10.000000 allocine-seances-0.0.4/src/allocine_seances.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-15 18:36:10.000000 allocine-seances-0.0.4/src/allocine_seances.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-15 18:36:10.000000 allocine-seances-0.0.4/src/allocine_seances.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 17:52:44.250181 allocine-seances-0.0.5/
+-rw-rw-rw-   0        0        0     1088 2023-04-15 16:16:47.000000 allocine-seances-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4607 2023-04-19 17:52:44.250181 allocine-seances-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2779 2023-04-15 18:32:35.000000 allocine-seances-0.0.5/README.md
+-rw-rw-rw-   0        0        0      721 2023-04-19 17:52:30.000000 allocine-seances-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 17:52:44.250181 allocine-seances-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 17:52:44.220332 allocine-seances-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 17:52:44.230599 allocine-seances-0.0.5/src/allocineAPI/
+-rw-rw-rw-   0        0        0        0 2023-04-15 16:02:27.000000 allocine-seances-0.0.5/src/allocineAPI/__init__.py
+-rw-rw-rw-   0        0        0     6515 2023-04-19 17:48:48.000000 allocine-seances-0.0.5/src/allocineAPI/allocineAPI.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:52:44.250181 allocine-seances-0.0.5/src/allocine_seances.egg-info/
+-rw-rw-rw-   0        0        0     4607 2023-04-19 17:52:44.000000 allocine-seances-0.0.5/src/allocine_seances.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-04-19 17:52:44.000000 allocine-seances-0.0.5/src/allocine_seances.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 17:52:44.000000 allocine-seances-0.0.5/src/allocine_seances.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-19 17:52:44.000000 allocine-seances-0.0.5/src/allocine_seances.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-19 17:52:44.000000 allocine-seances-0.0.5/src/allocine_seances.egg-info/top_level.txt
```

### Comparing `allocine-seances-0.0.4/LICENSE` & `allocine-seances-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `allocine-seances-0.0.4/PKG-INFO` & `allocine-seances-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allocine-seances
-Version: 0.0.4
+Version: 0.0.5
 Summary: Récupération des scéances de cinémas sur allociné
 Author-email: lefevre-dev <louislefevre.dev@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `allocine-seances-0.0.4/README.md` & `allocine-seances-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `allocine-seances-0.0.4/pyproject.toml` & `allocine-seances-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "allocine-seances"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="lefevre-dev", email="louislefevre.dev@gmail.com" },
 ]
 description = "Récupération des scéances de cinémas sur allociné"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
```

### Comparing `allocine-seances-0.0.4/src/allocineAPI/allocineAPI.py` & `allocine-seances-0.0.5/src/allocineAPI/allocineAPI.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,31 +114,36 @@
     def get_showtime(self, id_cinema, day_shift=0):
         """
         Récupération des horaires des seances pour un cinema, pour un jour donné
         :param id_cinema: id du cinema
         :param day_shift: décalage en jours par rapport à la date actuelle (positif)
         :return:
         """
-        json_data = self._get_json_request(URLs.showtime_url(id_cinema, day_shift))
         formated_data = list()
-        for movie in json_data["results"]:
-            title = movie["movie"]["title"]
-            duration = movie["movie"]["runtime"]
-            list_vf = list()
-            for showtime_original in movie["showtimes"]["original"]:
-                list_vf.append(showtime_original["startsAt"])
-            list_vo = list()
-            for showtime_multiple in movie["showtimes"]["multiple"]:
-                list_vo.append(showtime_multiple["startsAt"])
-            formated_data.append({
-                "title": title,
-                "duration": duration,
-                "VF": list_vf,
-                "VO": list_vo
-            })
+        page, totalPages = 0, 1
+        while page < totalPages:
+            json_data = self._get_json_request(URLs.showtime_url(id_cinema, day_shift, page+1))
+            page = int(json_data["pagination"]["page"])
+            totalPages = int(json_data["pagination"]["totalPages"])
+            for movie in json_data["results"]:
+                title = movie["movie"]["title"]
+                duration = movie["movie"]["runtime"]
+                list_vf = list()
+                for showtime_original in movie["showtimes"]["original"]:
+                    list_vf.append(showtime_original["startsAt"])
+                list_vo = list()
+                for showtime_multiple in movie["showtimes"]["multiple"]:
+                    list_vo.append(showtime_multiple["startsAt"])
+                formated_data.append({
+                    "title": title,
+                    "duration": duration,
+                    "VF": list_vf,
+                    "VO": list_vo
+                })
+
         return formated_data
 
 
 class URLs:
 
     BASE_URL = "https://www.allocine.fr/"
     SEANCES = "salle/"
@@ -153,16 +158,16 @@
     def cinemas_url(id_location):
         if "circuit" in id_location:
             return URLs.BASE_URL + URLs.SEANCES + id_location
         else:
             return URLs.BASE_URL + URLs.SEANCES + URLs.CINEMA + id_location
 
     @staticmethod
-    def showtime_url(id_cinema, day_shift):
-        return URLs.BASE_URL + URLs.SHOWTIMES + id_cinema + "/d-" + str(day_shift)
+    def showtime_url(id_cinema, day_shift, page):
+        return URLs.BASE_URL + URLs.SHOWTIMES + id_cinema + "/d-" + str(day_shift) + "/p-" + str(page)
 
 
 if __name__ == '__main__':
 
     api = allocineAPI()
 
     # ret = api.get_top_villes()
@@ -181,10 +186,11 @@
     # circuit
     PatheCinemas = "circuit-81002"
 
     # cinemas = api.get_cinema(PatheCinemas)
     # for cinema in cinemas:
     #     print(cinema)
 
-    data = api.get_showtime("W2920")
+    data = api.get_showtime("P0036")
     for showtime in data:
         print(showtime)
+    print(len(data))
```

### Comparing `allocine-seances-0.0.4/src/allocine_seances.egg-info/PKG-INFO` & `allocine-seances-0.0.5/src/allocine_seances.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allocine-seances
-Version: 0.0.4
+Version: 0.0.5
 Summary: Récupération des scéances de cinémas sur allociné
 Author-email: lefevre-dev <louislefevre.dev@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

