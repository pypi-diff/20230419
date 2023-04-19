# Comparing `tmp/musicli-0.0.1.tar.gz` & `tmp/musicli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicli-0.0.1.tar", max compression
+gzip compressed data, was "musicli-0.0.2.tar", max compression
```

## Comparing `musicli-0.0.1.tar` & `musicli-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2283 2023-04-17 14:51:42.670597 musicli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3788 2023-04-18 11:39:08.644573 musicli-0.0.1/README.md
--rw-r--r--   0        0        0     9900 2023-04-18 12:06:15.720479 musicli-0.0.1/src/musicli/musicli.py
--rw-r--r--   0        0        0     4469 1970-01-01 00:00:00.000000 musicli-0.0.1/setup.py
--rw-r--r--   0        0        0     4945 1970-01-01 00:00:00.000000 musicli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2379 2023-04-19 14:39:24.912681 musicli-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3788 2023-04-18 11:39:08.644573 musicli-0.0.2/README.md
+-rw-r--r--   0        0        0     9809 2023-04-19 14:24:04.050243 musicli-0.0.2/src/musicli/musicli.py
+-rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 musicli-0.0.2/setup.py
+-rw-r--r--   0        0        0     5021 1970-01-01 00:00:00.000000 musicli-0.0.2/PKG-INFO
```

### Comparing `musicli-0.0.1/pyproject.toml` & `musicli-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "musicli"
-version = "0.0.1"
+version = "0.0.2"
 description = "Rate, review, and catalogue all your artists and albums from the command line"
 authors = [
     "Atharva Shah <highnessatharva@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
 
@@ -27,14 +27,16 @@
 
 packages = [
     { include = "musicli", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.1, <4.0"
+pylast = "^5.1.0"
+pick = "^2.2.0"
 
 [tool.poetry.dev-dependencies]
 autoflake = "*"
 black = "*"
 flake8 = "*"
 flake8-bugbear = "*"
 flake8-builtins = "*"
@@ -52,14 +54,17 @@
 pytest = "*"
 pytest-github-actions-annotate-failures = "*"
 pytest-cov = "*"
 python-kacl = "*"
 pyupgrade = "*"
 tryceratops = "*"
 
+[tool.poetry.scripts]
+musicli = "musicli.musicli:start"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 src_paths = ["src", "tests"]
```

### Comparing `musicli-0.0.1/README.md` & `musicli-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `musicli-0.0.1/src/musicli/musicli.py` & `musicli-0.0.2/src/musicli/musicli.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     else:
         # create a new json file with empty dict
         with open("albums.json", "w") as f:
             ratings = {"album_ratings": [], "song_ratings": []}
             json.dump(ratings, f)
 
 
-def get_album_list(artist: str) -> List[str]:
+def get_album_list(artist: str, network: pylast.LastFMNetwork) -> List[str]:
     # GET THE TOP ALBUMS OF THE ARTIST AND STORE THEM IN A LIST
     artist = network.get_artist(artist)
     top_albums = artist.get_top_albums()
     album_list = [str(album.item) for album in top_albums]
 
     # CLEANUP THE LIST
     for album in album_list:
@@ -33,23 +33,23 @@
     album_list.sort()
 
     # ADD EXIT OPTION
     album_list.insert(0, "EXIT")
     return album_list
 
 
-def rate_by_album():
+def rate_by_album(network: pylast.LastFMNetwork) -> None:
     load_or_create_json()
     with open("albums.json") as f:
         album_file = json.load(f)
     print("RATE BY ARTIST")
     artist_search = input("Search for an artist: ")
 
     try:
-        album_list = get_album_list(artist_search)
+        album_list = get_album_list(artist_search, network)
 
         # PICK THE ALBUMS
         print("Select albums to rate")
         while True:
             selected_album, index = pick(album_list, "Albums", indicator="→")
             if selected_album == "EXIT":
                 break
@@ -120,15 +120,15 @@
         with open("albums.json", "w") as f:
             json.dump(album_file, f)
 
     except pylast.PyLastError:
         print("Artist not found")
 
 
-def rate_album_songs():
+def rate_album_songs(network: pylast.LastFMNetwork):
     load_or_create_json()
     with open("albums.json") as f:
         album_file = json.load(f)
 
     # show all albums from the file
     albums_in_file = []
     for collection in album_file["album_ratings"]:
@@ -202,15 +202,15 @@
                         f"You gave {artist}'s {selected_track} {rating} stars | {index+1}/10"
                     )
                     break
         with open("albums.json", "w") as f:
             json.dump(album_file, f)
 
 
-def rate_single_song():
+def rate_single_song(network: pylast.LastFMNetwork):
     load_or_create_json()
     with open("albums.json") as f:
         album_file = json.load(f)
 
     song_input = input("What's the name of the song?\t")
     artist_input = input("What's the name of the artist?\t")
 
@@ -267,22 +267,21 @@
     selected_option, index = pick(options, question, indicator="→")
     if index == 0:
         rate_album_songs()
     elif index == 1:
         rate_single_song()
 
 
-if __name__ == "__main__":
+
+def start():
     LASTFM_API_KEY = os.environ.get("LASTFM_API_KEY")
     LASTFM_API_SECRET = os.environ.get("LASTFM_API_SECRET")
     startup_question = "What do you want to do?"
     options = ["Rate by Album", "Rate Songs"]
     selected_option, index = pick(options, startup_question, indicator="→")
     network = pylast.LastFMNetwork(api_key=LASTFM_API_KEY, api_secret=LASTFM_API_SECRET)
-
     if index == 0:
-        rate_by_album()
+        rate_by_album(network)
     elif index == 1:
-        rate_by_song()
-
-
-# - Rate by Artist -> Search Artist -> Show Artist Albums and allow selection -> once selected ask for a rating on a 10 point scale -> save the date, rating, album -> Show the tracks and optionally prompt to rate each track [Y/N] ->
+        rate_by_song(network)
+    
+
```

### Comparing `musicli-0.0.1/setup.py` & `musicli-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,33 @@
 
 packages = \
 ['musicli']
 
 package_data = \
 {'': ['*']}
 
+install_requires = \
+['pick>=2.2.0,<3.0.0', 'pylast>=5.1.0,<6.0.0']
+
+entry_points = \
+{'console_scripts': ['musicli = musicli.musicli:start']}
+
 setup_kwargs = {
     'name': 'musicli',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Rate, review, and catalogue all your artists and albums from the command line',
     'long_description': "# musicli\n\n[![PyPI](https://img.shields.io/pypi/v/musicli?style=flat-square)](https://pypi.python.org/pypi/musicli/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/musicli?style=flat-square)](https://pypi.python.org/pypi/musicli/)\n[![PyPI - License](https://img.shields.io/pypi/l/musicli?style=flat-square)](https://pypi.python.org/pypi/musicli/)\n[![Coookiecutter - Wolt](https://img.shields.io/badge/cookiecutter-Wolt-00c2e8?style=flat-square&logo=cookiecutter&logoColor=D4AA00&link=https://github.com/woltapp/wolt-python-package-cookiecutter)](https://github.com/woltapp/wolt-python-package-cookiecutter)\n\n---\nmusicli is a powerful and user-friendly Python package that allows users to easily rate, review, and catalogue their favorite artists and albums from the command line. With intuitive search and selection features, users can quickly navigate their music library and rate each album on a 10-point scale. The package also offers the option to rate individual tracks and includes a variety of customization options to personalize the cataloguing experience. Whether you're a music aficionado or simply looking to organize your music library, musicli is the perfect tool for music lovers everywhere.\n\n**Documentation**: [https://HighnessAtharva.github.io/musicli](https://HighnessAtharva.github.io/musicli)\n\n**Source Code**: [https://github.com/HighnessAtharva/musicli](https://github.com/HighnessAtharva/musicli)\n\n**PyPI**: [https://pypi.org/project/musicli/](https://pypi.org/project/musicli/)\n\n---\n\nRate, review, and catalogue all your artists and albums from the command line\n\n## Installation\n\n```sh\npip install musicli\n```\n\nGet a Last.fm API key from [here](https://www.last.fm/api/account/create) and set it as an environment variable:\n\n```sh\nset LASTFM_API_KEY=<your_api_key>\nset LASTFM_API_SECRET=<your_api_secret>\n```\n\n## Development\n\n* Clone this repository\n* Requirements:\n  * [Poetry](https://python-poetry.org/)\n  * Python 3.7+\n* Create a virtual environment and install the dependencies\n\n```sh\npoetry install\n```\n\n* Activate the virtual environment\n\n```sh\npoetry shell\n```\n\n### Testing\n\n```sh\npytest\n```\n\n### Documentation\n\nThe documentation is automatically generated from the content of the [docs directory](./docs) and from the docstrings of the public signatures of the source code. The documentation is updated and published as a [Github project page](https://pages.github.com/) automatically as part each release.\n\n### Releasing\n\nTrigger the [Draft release workflow](https://github.com/HighnessAtharva/musicli/actions/workflows/draft_release.yml)\n(press _Run workflow_). This will update the changelog & version and create a GitHub release which is in _Draft_ state.\n\nFind the draft release from the\n[GitHub releases](https://github.com/HighnessAtharva/musicli/releases) and publish it. When a release is published, it'll trigger [release](https://github.com/HighnessAtharva/musicli/blob/master/.github/workflows/release.yml) workflow which creates PyPI release and deploys updated documentation.\n\n### Pre-commit\n\nPre-commit hooks run all the auto-formatters (e.g. `black`, `isort`), linters (e.g. `mypy`, `flake8`), and other quality\n checks to make sure the changeset is in good shape before a commit/push happens.\n\nYou can install the hooks with (runs for each commit):\n\n```sh\npre-commit install\n```\n\nOr if you want them to run only for each push:\n\n```sh\npre-commit install -t pre-push\n```\n\nOr if you want e.g. want to run all checks manually for all files:\n\n```sh\npre-commit run --all-files\n```\n\n---\n\nThis project was generated using the [wolt-python-package-cookiecutter](https://github.com/woltapp/wolt-python-package-cookiecutter) template.\n",
     'author': 'Atharva Shah',
     'author_email': 'highnessatharva@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://HighnessAtharva.github.io/musicli',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
+    'entry_points': entry_points,
     'python_requires': '>=3.7.1,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `musicli-0.0.1/PKG-INFO` & `musicli-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicli
-Version: 0.0.1
+Version: 0.0.2
 Summary: Rate, review, and catalogue all your artists and albums from the command line
 Home-page: https://HighnessAtharva.github.io/musicli
 License: MIT
 Author: Atharva Shah
 Author-email: highnessatharva@gmail.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -19,14 +19,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
+Requires-Dist: pick (>=2.2.0,<3.0.0)
+Requires-Dist: pylast (>=5.1.0,<6.0.0)
 Project-URL: Documentation, https://HighnessAtharva.github.io/musicli
 Project-URL: Repository, https://github.com/HighnessAtharva/musicli
 Description-Content-Type: text/markdown
 
 # musicli
 
 [![PyPI](https://img.shields.io/pypi/v/musicli?style=flat-square)](https://pypi.python.org/pypi/musicli/)
```

