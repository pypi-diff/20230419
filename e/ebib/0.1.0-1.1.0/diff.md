# Comparing `tmp/ebib-0.1.0.tar.gz` & `tmp/ebib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebib-0.1.0.tar", last modified: Thu Mar 30 01:35:55 2023, max compression
+gzip compressed data, was "ebib-1.1.0.tar", last modified: Wed Apr 19 16:50:44 2023, max compression
```

## Comparing `ebib-0.1.0.tar` & `ebib-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-03-30 01:35:55.748107 ebib-0.1.0/
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)    35149 2023-03-30 01:00:35.000000 ebib-0.1.0/LICENSE
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      635 2023-03-30 01:35:55.748107 ebib-0.1.0/PKG-INFO
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      241 2023-03-29 13:24:13.000000 ebib-0.1.0/README.md
-drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-03-30 01:35:55.748107 ebib-0.1.0/ebib/
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      796 2023-03-30 01:12:06.000000 ebib-0.1.0/ebib/__init__.py
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     6074 2023-03-30 01:11:48.000000 ebib-0.1.0/ebib/add.py
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     1063 2023-03-30 01:11:22.000000 ebib-0.1.0/ebib/cli.py
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)    32769 2023-03-30 01:11:34.000000 ebib-0.1.0/ebib/english_stemmer.py
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     1578 2023-03-30 01:11:53.000000 ebib-0.1.0/ebib/lexer.py
-drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-03-30 01:35:55.748107 ebib-0.1.0/ebib.egg-info/
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      635 2023-03-30 01:35:55.000000 ebib-0.1.0/ebib.egg-info/PKG-INFO
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      281 2023-03-30 01:35:55.000000 ebib-0.1.0/ebib.egg-info/SOURCES.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)        1 2023-03-30 01:35:55.000000 ebib-0.1.0/ebib.egg-info/dependency_links.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)       38 2023-03-30 01:35:55.000000 ebib-0.1.0/ebib.egg-info/entry_points.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)       23 2023-03-30 01:35:55.000000 ebib-0.1.0/ebib.egg-info/requires.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)        5 2023-03-30 01:35:55.000000 ebib-0.1.0/ebib.egg-info/top_level.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      558 2023-03-30 01:19:03.000000 ebib-0.1.0/pyproject.toml
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)       38 2023-03-30 01:35:55.751440 ebib-0.1.0/setup.cfg
+drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 16:50:44.718486 ebib-1.1.0/
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)    35149 2023-03-30 01:00:35.000000 ebib-1.1.0/LICENSE
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      635 2023-04-19 16:50:44.718486 ebib-1.1.0/PKG-INFO
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      241 2023-03-29 13:24:13.000000 ebib-1.1.0/README.md
+drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 16:50:44.718486 ebib-1.1.0/ebib/
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      775 2023-04-12 12:47:10.000000 ebib-1.1.0/ebib/__init__.py
+drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 16:50:44.718486 ebib-1.1.0/ebib/assets/
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)    38403 2023-04-19 12:43:51.000000 ebib-1.1.0/ebib/assets/english-stemmer.js
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     3798 2023-04-19 16:37:29.000000 ebib-1.1.0/ebib/assets/index.html
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     5967 2023-04-19 16:35:50.000000 ebib-1.1.0/ebib/assets/index.js
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     5815 2023-04-19 16:45:20.000000 ebib-1.1.0/ebib/cli.py
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)    32769 2023-03-30 01:11:34.000000 ebib-1.1.0/ebib/english_stemmer.py
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     5703 2023-04-19 13:23:21.000000 ebib-1.1.0/ebib/indexer.py
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     1576 2023-04-19 13:21:21.000000 ebib-1.1.0/ebib/lexer.py
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     1137 2023-04-12 12:47:10.000000 ebib-1.1.0/ebib/utils.py
+drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 16:50:44.718486 ebib-1.1.0/ebib.egg-info/
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      635 2023-04-19 16:50:44.000000 ebib-1.1.0/ebib.egg-info/PKG-INFO
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      374 2023-04-19 16:50:44.000000 ebib-1.1.0/ebib.egg-info/SOURCES.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)        1 2023-04-19 16:50:44.000000 ebib-1.1.0/ebib.egg-info/dependency_links.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)       38 2023-04-19 16:50:44.000000 ebib-1.1.0/ebib.egg-info/entry_points.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)       23 2023-04-19 16:50:44.000000 ebib-1.1.0/ebib.egg-info/requires.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)        5 2023-04-19 16:50:44.000000 ebib-1.1.0/ebib.egg-info/top_level.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      609 2023-04-19 16:47:40.000000 ebib-1.1.0/pyproject.toml
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)       38 2023-04-19 16:50:44.718486 ebib-1.1.0/setup.cfg
```

### Comparing `ebib-0.1.0/LICENSE` & `ebib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ebib-0.1.0/PKG-INFO` & `ebib-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebib
-Version: 0.1.0
+Version: 1.1.0
 Summary: ebib is a bibliography manager system aimed to work with Gitlab/Github pages
 Author-email: Ernesto Lanchares <elancha98@gmail.com>
 Project-URL: Homepage, https://gitlab.com/elancha/ebib
 Project-URL: Bug Tracker, https://gitlab.com/elancha/ebib/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ebib-0.1.0/ebib/__init__.py` & `ebib-1.1.0/ebib/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,8 +13,7 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public
 # License along with ebib. If not, see <https://www.gnu.org/licenses/>.
 
 from .english_stemmer import EnglishStemmer
 from .lexer import Lexer
-from .add import add
```

### Comparing `ebib-0.1.0/ebib/add.py` & `ebib-1.1.0/ebib/indexer.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,29 +16,22 @@
 # License along with ebib. If not, see <https://www.gnu.org/licenses/>.
 
 import click
 import requests
 import json
 import fitz
 import re
-import os
-import shutil
 import hashlib
 
 from ebib import Lexer
 
 from typing import Dict, List, Tuple
 
 month_transform = ['jan', 'feb', 'mar', 'apr', 'may', 'jun', 'jul', 'aug', 'sep', 'oct', 'nov', 'dec']
 
-def transform_author_list(data: List[Dict[str, str]]) -> str:
-	return ' and '.join([
-	'{a[family]}, {a[given]}'.format(a=a) for a in data
-	])
-
 type_converter = {
 	'book': 'book',
 	'book-chapter': 'inbook',
 	'book-part': 'inbook',
 	'book-section': 'inbook',
 	'book-series': 'incollection',
 	'book-set': 'incollection',
@@ -59,75 +52,109 @@
 	'reference-book': 'book',
 	'report': 'report',
 	'report-series': 'inproceedings',
 	'standard-series': 'incollection',
 	'standard': 'techreport',
 }  # type: Dict[str, str]
 
-transformations = {
-	'publisher': [('publisher', lambda x: x)],
-	'issue': [('number', lambda x: x)],
-	'container-title': [('journal', lambda x: x)],
-	'published-print': [
-		('year', lambda x: x['date-parts'][0][0]),
-		('month', lambda x: month_transform[x['date-parts'][0][1]-1]),
-	],
-	'published-online': [
-		('year', lambda x: x['date-parts'][0][0]),
-		('month', lambda x: month_transform[x['date-parts'][0][1]-1]),
-	],
-	'issued': [
-		('year', lambda x: x['date-parts'][0][0]),
-		('month', lambda x: month_transform[x['date-parts'][0][1]-1]),
-	],
-	'DOI': [
-		('doi', lambda x: x),
-		('url', lambda x: 'https://doi.org/' + x),
-	],
-	'URL': [('url', lambda x: x)],
-	'page': [('pages', lambda x: x)],
-	'title': [('title', lambda x: x)],
-	'volume': [('volume', lambda x: x)],
-	'author': [('author', transform_author_list)],
-	'ISSN': [('isnn', lambda x: x[0])],
-	'type': [('type', lambda x: type_converter[x])]
+#transformations = {
+#	'publisher': [('publisher', lambda x: x)],
+#	'issue': [('number', lambda x: x)],
+#	'container-title': [('journal', lambda x: x)],
+#	'published-print': [
+#		('year', lambda x: x['date-parts'][0][0]),
+#		('month', lambda x: month_transform[x['date-parts'][0][1]-1]),
+#	],
+#	'published-online': [
+#		('year', lambda x: x['date-parts'][0][0]),
+#		('month', lambda x: month_transform[x['date-parts'][0][1]-1]),
+#	],
+#	'issued': [
+#		('year', lambda x: x['date-parts'][0][0]),
+#		('month', lambda x: month_transform[x['date-parts'][0][1]-1]),
+#	],
+#	'DOI': [
+#		('doi', lambda x: x),
+#		('url', lambda x: 'https://doi.org/' + x),
+#	],
+#	'URL': [('url', lambda x: x)],
+#	'page': [('pages', lambda x: x)],
+#	'title': [('title', lambda x: x)],
+#	'volume': [('volume', lambda x: x)],
+#	'author': [('author', transform_author_list)],
+#	'ISSN': [('isnn', lambda x: x[0])],
+#	'type': [('type', lambda x: type_converter[x])]
+#}
+#
+#ignored_keys = [
+#	'indexed', 'reference-count', 'license', 'content-domain',
+#	'short-container-title', 'created', 'source',
+#	'is-referenced-by-count', 'prefix', 'member',
+#	'reference', 'original-title', 'language', 'link',
+#	'deposited', 'score', 'resource', 'subtitle', 'short-title',
+#	'references-count', 'journal-issue', 'alternative-id',
+#	'relation', 'subject', 'container-title-short', 'published',
+#
+#]
+
+empty_metadata = {
+	'publisher': '',
+	'number': '',
+	'journal': '',
+	'doi': '',
+	'url': '',
+	'pages': '',
+	'title': '',
+	'volume': '',
+	'authors': '',
+	'issn': '',
+	'type': 'article',
+	'year': '',
+	'month': '',
 }
 
-ignored_keys = [
-	'indexed', 'reference-count', 'license', 'content-domain',
-	'short-container-title', 'created', 'source',
-	'is-referenced-by-count', 'prefix', 'member',
-	'reference', 'original-title', 'language', 'link',
-	'deposited', 'score', 'resource', 'subtitle', 'short-title',
-	'references-count', 'journal-issue', 'alternative-id',
-	'relation', 'subject', 'container-title-short', 'published',
-
-]
-
 def import_metadata(doi: str) -> Dict[str, str]:
 	r = requests.get('https://doi.org/' + doi, headers = {'accept': 'application/json'})
 
 	if r.status_code == 404:
 		print('ERROR: Invalid or unsupported DOI')
 		exit(1)
 	if r.status_code != 200:
 		print('ERROR: DOI service unaviable')
 		exit(1)
 
 	d_metadata = json.loads(r.text)
 
-	metadata = {}
+	def value_or_none(a):
+		return d_metadata[a] if a in d_metadata else ''
 
-	for k, v in d_metadata.items():
-		if k in transformations:
-			for ind, fn in transformations[k]:
-				metadata[ind] = fn(v)
-		elif k not in ignored_keys:
-			print('ERROR: Unknown message key "{}" => {}.'.format(k, v))
-			exit(1)
+	metadata = {
+		'publisher': value_or_none('publisher'),
+		'number': value_or_none('issue'),
+		'journal': value_or_none('conatiner-title'),
+		'doi': value_or_none('DOI'),
+		'url': d_metadata['URL'] if 'URL' in d_metadata else 'https://doi.org/' + value_or_none('DOI'),
+		'pages': value_or_none('page'),
+		'title': value_or_none('title'),
+		'volume': value_or_none('volume'),
+		'authors': list(map(lambda x: '{x[family]}, {x[given]}'.format(x=x), d_metadata['author'])),
+		'issn': d_metadata['ISSN'][0] if 'ISSN' in d_metadata else '',
+		'type': type_converter[d_metadata['type']],
+		'year': d_metadata['issued']['date-parts'][0][0],
+		'month': month_transform[d_metadata['issued']['date-parts'][0][1]-1],
+	}
+	print(metadata)
+
+#	for k, v in d_metadata.items():
+#		if k in transformations:
+#			for ind, fn in transformations[k]:
+#				metadata[ind] = fn(v)
+#		elif k not in ignored_keys:
+#			print('ERROR: Unknown message key "{}" => {}.'.format(k, v))
+#			exit(1)
 	return metadata
 
 def read_pdf(filepath: str) -> str:
 	pdf = fitz.open(filepath)
 	return '\n'.join([page.get_text() for page in pdf])
 
 def clean_doi(text: str) -> str:
@@ -155,53 +182,19 @@
 	for regex in [var_doi]:
 		for m in regex.finditer(text):
 			doi = m.group('doi')
 			return clean_doi(doi)
 
 def index(text: str) -> Dict[str, int]:
 	idx = {}
+	len = 0
 	for token in Lexer(text):
 		if token in idx:
 			idx[token] += 1
 		else:
 			idx[token] = 1
-	return idx
+		len += 1
+	return idx, len
 
 def checksum(filepath: str) -> str:
 	with open(filepath, 'rb') as f:
 		return hashlib.md5(f.read()).hexdigest()
-
-@click.command()
-@click.argument('filepath')
-@click.option('--doi', '-d', help = 'DOI of the imported document')
-@click.option('--force', is_flag = True, help = 'Force when detecting checksum coincidence')
-def add(filepath, doi, force):
-	full_text = read_pdf(filepath)
-	if doi is None:
-		doi = text_to_doi(full_text)
-		if not doi:
-			print("ERROR: Could not extract DOI from PDF file")
-			exit(1)
-	file_index = index(full_text)
-	metadata = import_metadata(doi)
-
-	filename = metadata['author'].split(',')[0] + str(metadata['year'])
-	if os.path.exists(filename + '.pdf'):
-		if checksum(filepath) == checksum(filename + '.pdf'):
-			print('WARN: "{}" and "{}" have the same checksum.'.format(filepath, filename + '.pdf'))
-			if not force:
-				print('      Are you trying to add the same document two times?')
-				exit(1)
-		shutil.move(filename + '.pdf', filename + 'a.pdf')
-		shutil.move(filename + '.json', filename + 'a.json')
-	i = 97
-	while os.path.exists(filename + chr(i) + '.pdf'):
-		i += 1
-	filename += chr(i) if i > 97 else ''
-
-	shutil.copy2(filepath, filename + '.pdf')
-	with open(filename + '.json', 'w') as f:
-		json.dump({'metadata': metadata, 'index': file_index, 'tags': []}, f)
-
-	# git add filename.pdf filename.json
-	# git commit -m added filename
-	# git push
```

### Comparing `ebib-0.1.0/ebib/english_stemmer.py` & `ebib-1.1.0/ebib/english_stemmer.py`

 * *Files identical despite different names*

### Comparing `ebib-0.1.0/ebib/lexer.py` & `ebib-1.1.0/ebib/lexer.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 #
 # You should have received a copy of the GNU General Public
 # License along with ebib. If not, see <https://www.gnu.org/licenses/>.
 
 from typing import Callable
 from ebib import EnglishStemmer
 
+stemmer = EnglishStemmer()
+
 class Lexer:
 	def __init__(self, text: str):
 		self.text = text
 	def trim_left(self):
 		while self.text and self.text[0].isspace():
 			self.text = self.text[1:]
 
@@ -42,14 +44,13 @@
 		if not self.text:
 			raise StopIteration
 
 		if self.text[0].isnumeric():
 			return self.chop_while(lambda x: x.isnumeric())
 		if self.text[0].isalpha():
 			term = self.chop_while(lambda x: x.isalnum()).lower()
-			stemmer = EnglishStemmer()
 			return stemmer.stemWord(term)
 
 		return self.chop(1)
 
 	def __iter__(self):
 		return self
```

### Comparing `ebib-0.1.0/ebib.egg-info/PKG-INFO` & `ebib-1.1.0/ebib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebib
-Version: 0.1.0
+Version: 1.1.0
 Summary: ebib is a bibliography manager system aimed to work with Gitlab/Github pages
 Author-email: Ernesto Lanchares <elancha98@gmail.com>
 Project-URL: Homepage, https://gitlab.com/elancha/ebib
 Project-URL: Bug Tracker, https://gitlab.com/elancha/ebib/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ebib-0.1.0/pyproject.toml` & `ebib-1.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [project]
 name = "ebib"
-version = "0.1.0"
+version = "1.1.0"
 authors = [
 	{ name = "Ernesto Lanchares", email = "elancha98@gmail.com" },
 ]
 description = "ebib is a bibliography manager system aimed to work with Gitlab/Github pages"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["Click", "requests", "pymupdf"]
 
 [project.scripts]
 ebib = "ebib.cli:cli"
 
+[tool.setuptools.package-data]
+ebib = ["assets/*"]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/elancha/ebib"
 "Bug Tracker" = "https://gitlab.com/elancha/ebib/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
```

