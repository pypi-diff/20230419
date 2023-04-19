# Comparing `tmp/notion_api-0.4.0.tar.gz` & `tmp/notion_api-0.4.1.tar.gz`

## Comparing `notion_api-0.4.0.tar` & `notion_api-0.4.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    11253 2020-02-02 00:00:00.000000 notion_api-0.4.0/README.md
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/py.typed
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/__init__.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/_about.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/_pkgv.py
--rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/blockmixin.py
--rw-r--r--   0        0        0    20946 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/blocktypefactory.py
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/client.py
--rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/notionblock.py
--rw-r--r--   0        0        0    25778 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/notiondatabase.py
--rw-r--r--   0        0        0    20082 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/notionpage.py
--rw-r--r--   0        0        0    15457 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/notionworkspace.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/exceptions/__init__.py
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/exceptions/errors.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/exceptions/validate.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/properties/__init__.py
--rw-r--r--   0        0        0    13595 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/properties/blocktypes.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/properties/build.py
--rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/properties/common.py
--rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/properties/files.py
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/properties/options.py
--rw-r--r--   0        0        0    14699 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/properties/propertyobjects.py
--rw-r--r--   0        0        0    15442 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/properties/propertyvalues.py
--rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/properties/richtext.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/propertyitems/__init__.py
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/propertyitems/base.py
--rw-r--r--   0        0        0     8508 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/propertyitems/call.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/query/__init__.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/query/compound.py
--rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/query/conditions.py
--rw-r--r--   0        0        0     7600 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/query/propfilter.py
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/query/sort.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/query/timestamp.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 notion_api-0.4.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 notion_api-0.4.0/LICENSE
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 notion_api-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    12717 2020-02-02 00:00:00.000000 notion_api-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11253 2020-02-02 00:00:00.000000 notion_api-0.4.1/README.md
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/py.typed
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/__init__.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/_about.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/_pkgv.py
+-rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/blockmixin.py
+-rw-r--r--   0        0        0    20946 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/blocktypefactory.py
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/client.py
+-rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/notionblock.py
+-rw-r--r--   0        0        0    26159 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/notiondatabase.py
+-rw-r--r--   0        0        0    20435 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/notionpage.py
+-rw-r--r--   0        0        0    15457 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/notionworkspace.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/exceptions/__init__.py
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/exceptions/errors.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/exceptions/validate.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/properties/__init__.py
+-rw-r--r--   0        0        0    13595 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/properties/blocktypes.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/properties/build.py
+-rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/properties/common.py
+-rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/properties/files.py
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/properties/options.py
+-rw-r--r--   0        0        0    14699 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/properties/propertyobjects.py
+-rw-r--r--   0        0        0    15442 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/properties/propertyvalues.py
+-rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/properties/richtext.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/propertyitems/__init__.py
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/propertyitems/base.py
+-rw-r--r--   0        0        0     8508 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/propertyitems/call.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/query/__init__.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/query/compound.py
+-rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/query/conditions.py
+-rw-r--r--   0        0        0     7600 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/query/propfilter.py
+-rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/query/sort.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/query/timestamp.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 notion_api-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 notion_api-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 notion_api-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    12717 2020-02-02 00:00:00.000000 notion_api-0.4.1/PKG-INFO
```

### Comparing `notion_api-0.4.0/README.md` & `notion_api-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/__init__.py` & `notion_api-0.4.1/notion/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/api/__init__.py` & `notion_api-0.4.1/notion/api/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/api/_about.py` & `notion_api-0.4.1/notion/api/_about.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "__package_url__",
     "__package_json__",
 )
 
 __notion_version__: Final[str] = "2022-06-28"
 __content_type__: Final[str] = "application/json"
 __base_url__: Final[str] = "https://api.notion.com/v1/"
-__version__: Final[str] = "0.4.0"
+__version__: Final[str] = "0.4.1"
 __package_url__: Final[str] = "https://pypi.org/pypi/notion-api/"
 __package_json__: Final[str] = "https://pypi.org/pypi/notion-api/json"
 
 
 # Notion API Changlog
 # https://developers.notion.com/page/changelog
```

### Comparing `notion_api-0.4.0/notion/api/_pkgv.py` & `notion_api-0.4.1/notion/api/_pkgv.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/api/blockmixin.py` & `notion_api-0.4.1/notion/api/blockmixin.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/api/blocktypefactory.py` & `notion_api-0.4.1/notion/api/blocktypefactory.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/api/client.py` & `notion_api-0.4.1/notion/api/client.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/api/notionblock.py` & `notion_api-0.4.1/notion/api/notionblock.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/api/notiondatabase.py` & `notion_api-0.4.1/notion/api/notiondatabase.py`

 * *Files 5% similar despite different names*

```diff
@@ -229,49 +229,62 @@
         self._patch(
             self._database_endpoint(self.id),
             payload=default_json.dumps({"is_inline": __inline}),
         )
 
     @property
     def description(self) -> str:
-        """:return: (str) description of database"""
+        """
+        :return: (str) description of database. Empty string if no description is set.
+
+        description.setter:
+            >>> database.description = "This is a description of the database."
+        """
         try:
             description = self.retrieve["description"][0]["text"]["content"]
             return cast(str, description)
         except IndexError:
             return ""  # description is empty.
 
     @description.setter
     def description(self, description: str) -> None:
         self._update(DatabaseDescription([RichText(description)]))
 
     @property
-    def icon(self) -> str:
-        """:return: (str) url of icon"""
-        icon = self.retrieve["icon"]["external"]["url"]
-        return cast(str, icon)
+    def icon(self) -> Union[str, None]:
+        """
+        :return: (str) url of icon. None if no icon is set.
+
+        icon.setter:
+            >>> database.icon = "https://www.notion.so/icons/code_gray.svg"
+        """
+        icon = self.retrieve["icon"]
+        if icon:
+            return cast(str, icon["external"]["url"])
+        return None
 
     @icon.setter
     def icon(self, icon_url: str) -> None:
-        """
-        >>> database.icon = "https://www.notion.so/icons/code_gray.svg"
-        """
         self._update(Icon(icon_url))
 
     @property
-    def cover(self) -> str:
-        """:return: (str) url of cover"""
-        cover = self.retrieve["cover"]["external"]["url"]
-        return cast(str, cover)
+    def cover(self) -> Union[str, None]:
+        """
+        :return: (str) url of cover. None if no cover is set.
+
+        cover.setter:
+            >>> database.cover = "https://www.notion.so/images/page-cover/webb1.jpg"
+        """
+        cover = self.retrieve["cover"]
+        if cover:
+            return cast(str, cover["external"]["url"])
+        return None
 
     @cover.setter
     def cover(self, cover_url: str) -> None:
-        """
-        >>> database.cover = "https://www.notion.so/images/page-cover/webb1.jpg"
-        """
         self._update(Cover(cover_url))
 
     @property
     def url(self) -> str:
         """:return: (str) url of database"""
         return cast(str, (self.retrieve["url"]))
```

### Comparing `notion_api-0.4.0/notion/api/notionpage.py` & `notion_api-0.4.1/notion/api/notionpage.py`

 * *Files 6% similar despite different names*

```diff
@@ -174,66 +174,83 @@
     def __contains__(self, property_name: str) -> bool:
         return property_name in self.properties
 
     def __iter__(self) -> Iterator[str]:
         return iter(self.properties)
 
     def __getitem__(self, property_name: str) -> MutableMapping[str, Any]:
-        if property_name in self.properties:
+        if property_name in self:
             return cast(MutableMapping[str, Any], self.properties[property_name])
         raise KeyError(f"{property_name} not found in page property values.")
 
     @cached_property
     def properties(self) -> MutableMapping[str, Any]:
         return cast(MutableMapping[str, Any], self.retrieve()["properties"])
 
     @property
     def title(self) -> str:
-        """:return: (str) title of page"""
+        """
+        :return: (str) title of page. Empty string if no title is set.
+
+        title setter:
+            >>> page.title = "New Title"
+        """
         try:
             if ("workspace" or "page_id") in self.parent_type:
                 return cast(str, self.properties["title"]["title"][0]["plain_text"])
 
             database_title_property = self.properties[
                 [k for k, v in self.properties.items() if "title" in v][0]
             ]
             return cast(str, database_title_property["title"][0]["plain_text"])
         except IndexError:
             return ""  # title is empty
 
     @title.setter
-    def title(self, __new_title: str) -> None:
-        self._patch_properties(Properties(TitlePropertyValue([RichText(__new_title)])))
+    def title(self, new_title: str) -> None:
+        self._patch_properties(Properties(TitlePropertyValue([RichText(new_title)])))
 
     @property
-    def icon(self) -> str:
-        """:return: (str) url of icon"""
-        icon = self.properties["icon"]["external"]["url"]
-        return cast(str, icon)
+    def icon(self) -> Union[str, None]:
+        """
+        :return: (str) url of icon. None if no icon is set.
+
+        icon setter:
+            >>> page.icon = "https://www.notion.so/icons/code_gray.svg"
+        """
+        icon = self.retrieve()["icon"]
+        if icon:
+            return cast(str, icon["external"]["url"])
+        return None
 
     @icon.setter
     def icon(self, icon_url: str) -> None:
-        """>>> page.icon = "https://www.notion.so/icons/code_gray.svg" """
         self._patch_properties(Icon(icon_url))
 
     @property
-    def cover(self) -> str:
-        """:return: (str) url of cover"""
-        cover = self.properties["cover"]["external"]["url"]
-        return cast(str, cover)
+    def cover(self) -> Union[str, None]:
+        """
+        :return: (str) url of cover. None if no cover is set.
+
+        cover setter:
+            >>> page.cover = "https://www.notion.so/images/page-cover/webb1.jpg"
+        """
+        cover = self.retrieve()["cover"]
+        if cover:
+            return cast(str, cover["external"]["url"])
+        return None
 
     @cover.setter
     def cover(self, cover_url: str) -> None:
-        """>>> page.cover = "https://www.notion.so/images/page-cover/webb1.jpg" """
         self._patch_properties(Cover(cover_url))
 
     @property
     def url(self) -> str:
         """:return: (str) url of page"""
-        return cast(str, self.properties["url"])
+        return cast(str, self.retrieve()["url"])
 
     @property
     def delete_self(self) -> None:
         if self.is_archived:
             return
 
         self._delete(self._block_endpoint(self.id))
```

### Comparing `notion_api-0.4.0/notion/api/notionworkspace.py` & `notion_api-0.4.1/notion/api/notionworkspace.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/exceptions/__init__.py` & `notion_api-0.4.1/notion/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/exceptions/errors.py` & `notion_api-0.4.1/notion/exceptions/errors.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/exceptions/validate.py` & `notion_api-0.4.1/notion/exceptions/validate.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/properties/__init__.py` & `notion_api-0.4.1/notion/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/properties/blocktypes.py` & `notion_api-0.4.1/notion/properties/blocktypes.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/properties/build.py` & `notion_api-0.4.1/notion/properties/build.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/properties/common.py` & `notion_api-0.4.1/notion/properties/common.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/properties/files.py` & `notion_api-0.4.1/notion/properties/files.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/properties/options.py` & `notion_api-0.4.1/notion/properties/options.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/properties/propertyobjects.py` & `notion_api-0.4.1/notion/properties/propertyobjects.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/properties/propertyvalues.py` & `notion_api-0.4.1/notion/properties/propertyvalues.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/properties/richtext.py` & `notion_api-0.4.1/notion/properties/richtext.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/propertyitems/__init__.py` & `notion_api-0.4.1/notion/propertyitems/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/propertyitems/base.py` & `notion_api-0.4.1/notion/propertyitems/base.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/propertyitems/call.py` & `notion_api-0.4.1/notion/propertyitems/call.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/query/__init__.py` & `notion_api-0.4.1/notion/query/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/query/compound.py` & `notion_api-0.4.1/notion/query/compound.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/query/conditions.py` & `notion_api-0.4.1/notion/query/conditions.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/query/propfilter.py` & `notion_api-0.4.1/notion/query/propfilter.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/query/sort.py` & `notion_api-0.4.1/notion/query/sort.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/notion/query/timestamp.py` & `notion_api-0.4.1/notion/query/timestamp.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/.gitignore` & `notion_api-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/LICENSE` & `notion_api-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/pyproject.toml` & `notion_api-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.0/PKG-INFO` & `notion_api-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-api
-Version: 0.4.0
+Version: 0.4.1
 Summary: An unofficial wrapper for Notion's API, aiming to simplify the dynamic nature of interacting with Notion.
 Project-URL: Homepage, https://github.com/ayvi-0001/notion-api
 Project-URL: Source Code, https://github.com/ayvi-0001/notion-api
 Author-email: Alan Vickers <alan.k.vickers@gmail.com>
 License-File: LICENSE
 Keywords: notion-api,notion-version-2022-06-28,wrapper
 Classifier: Development Status :: 3 - Alpha
```

