# Comparing `tmp/seo-keyword-research-tool-0.1.8.tar.gz` & `tmp/seo-keyword-research-tool-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seo-keyword-research-tool-0.1.8.tar", last modified: Wed Apr 19 10:59:41 2023, max compression
+gzip compressed data, was "seo-keyword-research-tool-0.1.9.tar", last modified: Wed Apr 19 11:16:14 2023, max compression
```

## Comparing `seo-keyword-research-tool-0.1.8.tar` & `seo-keyword-research-tool-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 chukhraiartur  (1000) chukhraiartur  (1000)        0 2023-04-19 10:59:41.886376 seo-keyword-research-tool-0.1.8/
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)     1092 2023-01-24 10:20:20.000000 seo-keyword-research-tool-0.1.8/LICENSE
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)    10506 2023-04-19 10:59:41.886376 seo-keyword-research-tool-0.1.8/PKG-INFO
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)     7648 2023-04-18 18:28:59.000000 seo-keyword-research-tool-0.1.8/README.md
-drwxr-xr-x   0 chukhraiartur  (1000) chukhraiartur  (1000)        0 2023-04-19 10:59:41.886376 seo-keyword-research-tool-0.1.8/SeoKeywordResearch/
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       52 2023-03-29 06:41:45.000000 seo-keyword-research-tool-0.1.8/SeoKeywordResearch/__init__.py
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)     3191 2023-04-19 10:52:57.000000 seo-keyword-research-tool-0.1.8/SeoKeywordResearch/cli.py
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)     5111 2023-04-18 18:45:52.000000 seo-keyword-research-tool-0.1.8/SeoKeywordResearch/seo_keyword_research.py
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       91 2023-02-16 14:17:19.000000 seo-keyword-research-tool-0.1.8/pyproject.toml
-drwxr-xr-x   0 chukhraiartur  (1000) chukhraiartur  (1000)        0 2023-04-19 10:59:41.886376 seo-keyword-research-tool-0.1.8/seo_keyword_research_tool.egg-info/
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)    10506 2023-04-19 10:59:41.000000 seo-keyword-research-tool-0.1.8/seo_keyword_research_tool.egg-info/PKG-INFO
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)      437 2023-04-19 10:59:41.000000 seo-keyword-research-tool-0.1.8/seo_keyword_research_tool.egg-info/SOURCES.txt
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)        1 2023-04-19 10:59:41.000000 seo-keyword-research-tool-0.1.8/seo_keyword_research_tool.egg-info/dependency_links.txt
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       53 2023-04-19 10:59:41.000000 seo-keyword-research-tool-0.1.8/seo_keyword_research_tool.egg-info/entry_points.txt
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       27 2023-04-19 10:59:41.000000 seo-keyword-research-tool-0.1.8/seo_keyword_research_tool.egg-info/requires.txt
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)        1 2023-04-19 10:59:41.000000 seo-keyword-research-tool-0.1.8/seo_keyword_research_tool.egg-info/top_level.txt
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       38 2023-04-19 10:59:41.886376 seo-keyword-research-tool-0.1.8/setup.cfg
--rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)     2052 2023-04-19 10:56:37.000000 seo-keyword-research-tool-0.1.8/setup.py
+drwxr-xr-x   0 chukhraiartur  (1000) chukhraiartur  (1000)        0 2023-04-19 11:16:14.706388 seo-keyword-research-tool-0.1.9/
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)     1092 2023-01-24 10:20:20.000000 seo-keyword-research-tool-0.1.9/LICENSE
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)    10399 2023-04-19 11:16:14.706388 seo-keyword-research-tool-0.1.9/PKG-INFO
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)     7562 2023-04-19 11:10:01.000000 seo-keyword-research-tool-0.1.9/README.md
+drwxr-xr-x   0 chukhraiartur  (1000) chukhraiartur  (1000)        0 2023-04-19 11:16:14.696388 seo-keyword-research-tool-0.1.9/SeoKeywordResearch/
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       52 2023-03-29 06:41:45.000000 seo-keyword-research-tool-0.1.9/SeoKeywordResearch/__init__.py
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)     3191 2023-04-19 10:52:57.000000 seo-keyword-research-tool-0.1.9/SeoKeywordResearch/cli.py
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)     5111 2023-04-18 18:45:52.000000 seo-keyword-research-tool-0.1.9/SeoKeywordResearch/seo_keyword_research.py
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       91 2023-02-16 14:17:19.000000 seo-keyword-research-tool-0.1.9/pyproject.toml
+drwxr-xr-x   0 chukhraiartur  (1000) chukhraiartur  (1000)        0 2023-04-19 11:16:14.706388 seo-keyword-research-tool-0.1.9/seo_keyword_research_tool.egg-info/
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)    10399 2023-04-19 11:16:14.000000 seo-keyword-research-tool-0.1.9/seo_keyword_research_tool.egg-info/PKG-INFO
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)      437 2023-04-19 11:16:14.000000 seo-keyword-research-tool-0.1.9/seo_keyword_research_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)        1 2023-04-19 11:16:14.000000 seo-keyword-research-tool-0.1.9/seo_keyword_research_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       53 2023-04-19 11:16:14.000000 seo-keyword-research-tool-0.1.9/seo_keyword_research_tool.egg-info/entry_points.txt
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       27 2023-04-19 11:16:14.000000 seo-keyword-research-tool-0.1.9/seo_keyword_research_tool.egg-info/requires.txt
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)        1 2023-04-19 11:16:14.000000 seo-keyword-research-tool-0.1.9/seo_keyword_research_tool.egg-info/top_level.txt
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)       38 2023-04-19 11:16:14.706388 seo-keyword-research-tool-0.1.9/setup.cfg
+-rw-r--r--   0 chukhraiartur  (1000) chukhraiartur  (1000)     2052 2023-04-19 11:07:30.000000 seo-keyword-research-tool-0.1.9/setup.py
```

### Comparing `seo-keyword-research-tool-0.1.8/LICENSE` & `seo-keyword-research-tool-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `seo-keyword-research-tool-0.1.8/PKG-INFO` & `seo-keyword-research-tool-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seo-keyword-research-tool
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python SEO keywords suggestion tool. Google Autocomplete, Related Questions and Related Searches.
 Home-page: https://github.com/chukhraiartur/seo-keyword-research-tool
 Author: Artur Chukhrai
 Author-email: chukhraiartur@gmail.com
 Maintainer: Artur Chukhrai, Dmitiry Zub
 Maintainer-email: chukhraiartur@gmail.com, dimitryzub@gmail.com
 License: MIT
@@ -45,25 +45,21 @@
         
         ## ⚙️Installation
         
         ```bash
         $ pip install seo-keyword-research-tool
         ```
         
-        ```bash
-        $ git clone https://github.com/chukhraiartur/seo-keyword-research-tool.git
-        ```
-        
         
         ## 🤹‍♂️Usage
         
         #### Available CLI arugments:
         
         ```bash
-        $ python main.py -h
+        $ seo -h
         ```
         
         ```lang-none
         SerpApi SEO Keyword Research Tool [-h] -q  [-e  [...]] [-dl] [-st] [-ak] [-gd] [-gl] [-hl]
         
         Extract keywrods from: Google Autocomplete, People Also Ask, and People Also Search and saves data to CSV/JSON/TXT.
         
@@ -93,15 +89,15 @@
         | 4 | 324 | 72*3 = 216 + 108 = 324 |
         
         📌Note: This is how the logic works for the `google.com` domain, on other domains the results may differ.
         
         #### Simple example:
         
         ```bash
-        $ python main.py -q "starbucks coffee"
+        $ seo -q "starbucks coffee"
         ```
         
         ```json
         {
           "auto_complete": [
             "starbucks coffee menu",
             "starbucks coffee cups",
@@ -131,15 +127,15 @@
         ```
         
         #### Advanced example:
         
         This example will use [related questions API](https://serpapi.com/related-questions) engine with a depth limit value of 2, and saves data to JSON:
         
         ```bash
-        $ python main.py --api-key <your_serpapi_api_key> \
+        $ seo --api-key "<your_serpapi_api_key>" \
         > -q "starbucks coffee" \
         > -e rq \
         > -dl 2 \
         > -gd google.co.uk \
         > -gl uk \
         > -hl en \
         > -st json \
@@ -207,14 +203,15 @@
         
         data = {
             'auto_complete': auto_complete_results,
             'related_searches': related_searches_results,
             'related_questions': related_questions_results
         }
         
+        keyword_research.save_to_json(data)
         keyword_research.print_data(data)
         ```
         
         ### ✍Contributing
         
         Feel free to open bug issue, something isn't working, what feature to add, or anything else related to Google autocomplete, related searches or people also ask.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seo-keyword-research-tool Version: 0.1.8 Summary:
+Metadata-Version: 2.1 Name: seo-keyword-research-tool Version: 0.1.9 Summary:
 Python SEO keywords suggestion tool. Google Autocomplete, Related Questions and
 Related Searches. Home-page: https://github.com/chukhraiartur/seo-keyword-
 research-tool Author: Artur Chukhrai Author-email: chukhraiartur@gmail.com
 Maintainer: Artur Chukhrai, Dmitiry Zub Maintainer-email:
 chukhraiartur@gmail.com, dimitryzub@gmail.com License: MIT Project-URL:
 Documentation, https://github.com/chukhraiartur/seo-keyword-research-tool
 Project-URL: Source, https://github.com/chukhraiartur/seo-keyword-research-tool
@@ -23,87 +23,86 @@
 78694043/221098691-5ad4d2b9-0ebd-4c65-ab1e-47a599955e9c.gif) This tool uses
 [SerpApi](https://serpapi.com/) as a tool to parse data from Google search
 results. You can use provided API key that will be available after
 installation, however, it's purely for testing purposes to see if the tool fits
 your needs. If you'll be using it for your own purpose (personal or
 commercial), you have to use [your own SerpApi key](https://serpapi.com/manage-
 api-key). ## âï¸Installation ```bash $ pip install seo-keyword-research-tool
-``` ```bash $ git clone https://github.com/chukhraiartur/seo-keyword-research-
-tool.git ``` ## ð¤¹ââï¸Usage #### Available CLI arugments: ```bash $
-python main.py -h ``` ```lang-none SerpApi SEO Keyword Research Tool [-h] -q [-
-e [...]] [-dl] [-st] [-ak] [-gd] [-gl] [-hl] Extract keywrods from: Google
-Autocomplete, People Also Ask, and People Also Search and saves data to CSV/
-JSON/TXT. optional arguments: -h, --help show this help message and exit -q , -
--query Search query (required). -e [ ...], --engines [ ...] Choices of engines
-to extract: Autocomplete (ac), Related Searches (rs), People Also Ask (rq). You
-can select multiple engines. All engines are selected by default. -dl , --
-depth-limit Depth limit for People Also Ask. Default is 0, first 2-4 results. -
-st , --save-to Saves the results in the current directory in the selected
-format (CSV, JSON, TXT). Default CSV. -ak , --api-key Your SerpApi API key:
-https://serpapi.com/manage-api-key. Default is a test API key to test CLI. -gd
-, --domain Google domain: https://serpapi.com/google-domains. Default
-google.com. -gl , --country Country of the search: https://serpapi.com/google-
-countries. Default us. -hl , --lang Language of the search: https://
-serpapi.com/google-languages. Default en. Found a bug? Open issue: https://
-github.com/chukhraiartur/seo-keyword-research-tool/issues ``` The `--depth-
-limit` argument for People Also Ask can be set from `0` to `4`. For each depth
-limit value, the number of results returned grows exponentially. Below is a
-table showing how the depth limit argument is affected: | Depth limit | Number
-of results | Explanation | |-------------|-------------------|-------------| |
-0 | 4 | Standard results | | 1 | 12 | 4*2 = 8 + 4 = 12 | | 2 | 36 | 8*3 = 24 +
-12 = 36 | | 3 | 108 | 24*3 = 72 + 36 = 108 | | 4 | 324 | 72*3 = 216 + 108 = 324
-| ðNote: This is how the logic works for the `google.com` domain, on other
-domains the results may differ. #### Simple example: ```bash $ python main.py -
+``` ## ð¤¹ââï¸Usage #### Available CLI arugments: ```bash $ seo -h ```
+```lang-none SerpApi SEO Keyword Research Tool [-h] -q [-e [...]] [-dl] [-st]
+[-ak] [-gd] [-gl] [-hl] Extract keywrods from: Google Autocomplete, People Also
+Ask, and People Also Search and saves data to CSV/JSON/TXT. optional arguments:
+-h, --help show this help message and exit -q , --query Search query
+(required). -e [ ...], --engines [ ...] Choices of engines to extract:
+Autocomplete (ac), Related Searches (rs), People Also Ask (rq). You can select
+multiple engines. All engines are selected by default. -dl , --depth-limit
+Depth limit for People Also Ask. Default is 0, first 2-4 results. -st , --save-
+to Saves the results in the current directory in the selected format (CSV,
+JSON, TXT). Default CSV. -ak , --api-key Your SerpApi API key: https://
+serpapi.com/manage-api-key. Default is a test API key to test CLI. -gd , --
+domain Google domain: https://serpapi.com/google-domains. Default google.com. -
+gl , --country Country of the search: https://serpapi.com/google-countries.
+Default us. -hl , --lang Language of the search: https://serpapi.com/google-
+languages. Default en. Found a bug? Open issue: https://github.com/
+chukhraiartur/seo-keyword-research-tool/issues ``` The `--depth-limit` argument
+for People Also Ask can be set from `0` to `4`. For each depth limit value, the
+number of results returned grows exponentially. Below is a table showing how
+the depth limit argument is affected: | Depth limit | Number of results |
+Explanation | |-------------|-------------------|-------------| | 0 | 4 |
+Standard results | | 1 | 12 | 4*2 = 8 + 4 = 12 | | 2 | 36 | 8*3 = 24 + 12 = 36
+| | 3 | 108 | 24*3 = 72 + 36 = 108 | | 4 | 324 | 72*3 = 216 + 108 = 324 |
+ðNote: This is how the logic works for the `google.com` domain, on other
+domains the results may differ. #### Simple example: ```bash $ seo -
 q "starbucks coffee" ``` ```json { "auto_complete": [ "starbucks coffee menu",
 "starbucks coffee cups", "starbucks coffee sizes", "starbucks coffee mugs",
 "starbucks coffee gear", "starbucks coffee beans", "starbucks coffee near me",
 "starbucks coffee traveler" ], "related_searches": [ "starbucks near me",
 "starbucks coffee price", "starbucks coffee beans", "starbucks company",
 "starbucks coffee menu", "starbucks merchandise", "starbucks coffee bags" ],
 "related_questions": [ "What is the most popular Starbucks coffee?", "What is
 the number 1 Starbucks drink?", "What is the Tiktok coffee from Starbucks?",
 "Why is Starbucks coffee so famous?" ] } ``` #### Advanced example: This
 example will use [related questions API](https://serpapi.com/related-questions)
-engine with a depth limit value of 2, and saves data to JSON: ```bash $ python
-main.py --api-key  \ > -q "starbucks coffee" \ > -e rq \ > -dl 2 \ > -gd
-google.co.uk \ > -gl uk \ > -hl en \ > -st json \ ``` ```json
-{ "related_questions": [ "What is the best coffee in Starbucks?", "What is a
-popular Starbucks coffee?", "What is the number 1 Starbucks drink?", "Is
-Starbucks expensive?", "What should I try at Starbucks for the first time?",
-"Which Starbucks coffee is best and sweet?", "What is famous in Starbucks in
-India?", "Which Starbucks drink is the best in India?", "Why is Starbucks
-famous?", "What should I order in Starbucks?", "What is the least bitter coffee
-at Starbucks?", "What's the creamiest coffee?", "Which Starbucks coffee is best
-in taste?", "Which Starbucks coffee is best and sweet?", "Which Starbucks
-coffee is best in India?", "Which Starbucks coffee is best for first time?",
-"Why is Starbucks famous?", "What should I order at Starbucks for the first
-time?", "What is the best Starbucks drink for a first time coffee drinker?",
-"What should I order in Starbucks?", "What should I try at Starbucks for the
-first time?", "What is the most famous Starbucks drink?", "Which Starbucks
-coffee is best in taste?", "What coffee orders for beginners?", "What is the
-best thing to get at Starbucks?", "Which Starbucks drink is best?", "Which
-coffee is best in Starbucks India?", "Which Starbucks coffee is best in
-taste?", "Is Dunkin or Starbucks better?", "What are the negatives of
-Starbucks?", "Who has stronger coffee Starbucks or Dunkin?", "Why do people
-prefer Starbucks?", "Why is Starbucks so much better than Dunkin?", "Is
-Starbucks coffee high quality?", "Why is Starbucks coffee so good?", "Do
-Starbucks employees get free food?" ] } ``` #### Example of manual data
-extraction (without CLI): ```python from SeoKeywordResearch import
-SeoKeywordResearch keyword_research = SeoKeywordResearch( query='starbucks
-coffee', api_key='', lang='en', country='us', domain='google.com' )
-auto_complete_results = keyword_research.get_auto_complete()
-related_searches_results = keyword_research.get_related_searches()
-related_questions_results = keyword_research.get_related_questions() data =
-{ 'auto_complete': auto_complete_results, 'related_searches':
-related_searches_results, 'related_questions': related_questions_results }
-keyword_research.print_data(data) ``` ### âContributing Feel free to open bug
-issue, something isn't working, what feature to add, or anything else related
-to Google autocomplete, related searches or people also ask. Keywords: google
-scholar,serpapi,scraper,python,python google scholar,python google scholar
-api,web scraping,python web scraping,research,google-search-results,cli
+engine with a depth limit value of 2, and saves data to JSON: ```bash $ seo --
+api-key "" \ > -q "starbucks coffee" \ > -e rq \ > -dl 2 \ > -gd google.co.uk \
+> -gl uk \ > -hl en \ > -st json \ ``` ```json { "related_questions": [ "What
+is the best coffee in Starbucks?", "What is a popular Starbucks coffee?", "What
+is the number 1 Starbucks drink?", "Is Starbucks expensive?", "What should I
+try at Starbucks for the first time?", "Which Starbucks coffee is best and
+sweet?", "What is famous in Starbucks in India?", "Which Starbucks drink is the
+best in India?", "Why is Starbucks famous?", "What should I order in
+Starbucks?", "What is the least bitter coffee at Starbucks?", "What's the
+creamiest coffee?", "Which Starbucks coffee is best in taste?", "Which
+Starbucks coffee is best and sweet?", "Which Starbucks coffee is best in
+India?", "Which Starbucks coffee is best for first time?", "Why is Starbucks
+famous?", "What should I order at Starbucks for the first time?", "What is the
+best Starbucks drink for a first time coffee drinker?", "What should I order in
+Starbucks?", "What should I try at Starbucks for the first time?", "What is the
+most famous Starbucks drink?", "Which Starbucks coffee is best in taste?",
+"What coffee orders for beginners?", "What is the best thing to get at
+Starbucks?", "Which Starbucks drink is best?", "Which coffee is best in
+Starbucks India?", "Which Starbucks coffee is best in taste?", "Is Dunkin or
+Starbucks better?", "What are the negatives of Starbucks?", "Who has stronger
+coffee Starbucks or Dunkin?", "Why do people prefer Starbucks?", "Why is
+Starbucks so much better than Dunkin?", "Is Starbucks coffee high quality?",
+"Why is Starbucks coffee so good?", "Do Starbucks employees get free food?" ] }
+``` #### Example of manual data extraction (without CLI): ```python from
+SeoKeywordResearch import SeoKeywordResearch keyword_research =
+SeoKeywordResearch( query='starbucks coffee', api_key='', lang='en',
+country='us', domain='google.com' ) auto_complete_results =
+keyword_research.get_auto_complete() related_searches_results =
+keyword_research.get_related_searches() related_questions_results =
+keyword_research.get_related_questions() data = { 'auto_complete':
+auto_complete_results, 'related_searches': related_searches_results,
+'related_questions': related_questions_results } keyword_research.save_to_json
+(data) keyword_research.print_data(data) ``` ### âContributing Feel free to
+open bug issue, something isn't working, what feature to add, or anything else
+related to Google autocomplete, related searches or people also ask. Keywords:
+google scholar,serpapi,scraper,python,python google scholar,python google
+scholar api,web scraping,python web scraping,research,google-search-results,cli
 Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Developers Classifier: Operating System :: Microsoft ::
 Windows Classifier: Operating System :: MacOS Classifier: Operating System ::
 POSIX :: Linux Classifier: Topic :: Internet Classifier: Natural Language ::
 English Classifier: Topic :: Utilities Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
```

### Comparing `seo-keyword-research-tool-0.1.8/README.md` & `seo-keyword-research-tool-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,25 +32,21 @@
 
 ## ⚙️Installation
 
 ```bash
 $ pip install seo-keyword-research-tool
 ```
 
-```bash
-$ git clone https://github.com/chukhraiartur/seo-keyword-research-tool.git
-```
-
 
 ## 🤹‍♂️Usage
 
 #### Available CLI arugments:
 
 ```bash
-$ python main.py -h
+$ seo -h
 ```
 
 ```lang-none
 SerpApi SEO Keyword Research Tool [-h] -q  [-e  [...]] [-dl] [-st] [-ak] [-gd] [-gl] [-hl]
 
 Extract keywrods from: Google Autocomplete, People Also Ask, and People Also Search and saves data to CSV/JSON/TXT.
 
@@ -80,15 +76,15 @@
 | 4 | 324 | 72*3 = 216 + 108 = 324 |
 
 📌Note: This is how the logic works for the `google.com` domain, on other domains the results may differ.
 
 #### Simple example:
 
 ```bash
-$ python main.py -q "starbucks coffee"
+$ seo -q "starbucks coffee"
 ```
 
 ```json
 {
   "auto_complete": [
     "starbucks coffee menu",
     "starbucks coffee cups",
@@ -118,15 +114,15 @@
 ```
 
 #### Advanced example:
 
 This example will use [related questions API](https://serpapi.com/related-questions) engine with a depth limit value of 2, and saves data to JSON:
 
 ```bash
-$ python main.py --api-key <your_serpapi_api_key> \
+$ seo --api-key "<your_serpapi_api_key>" \
 > -q "starbucks coffee" \
 > -e rq \
 > -dl 2 \
 > -gd google.co.uk \
 > -gl uk \
 > -hl en \
 > -st json \
@@ -194,13 +190,14 @@
 
 data = {
     'auto_complete': auto_complete_results,
     'related_searches': related_searches_results,
     'related_questions': related_questions_results
 }
 
+keyword_research.save_to_json(data)
 keyword_research.print_data(data)
 ```
 
 ### ✍Contributing
 
 Feel free to open bug issue, something isn't working, what feature to add, or anything else related to Google autocomplete, related searches or people also ask.
```

#### html2text {}

```diff
@@ -13,78 +13,77 @@
 78694043/221098691-5ad4d2b9-0ebd-4c65-ab1e-47a599955e9c.gif) This tool uses
 [SerpApi](https://serpapi.com/) as a tool to parse data from Google search
 results. You can use provided API key that will be available after
 installation, however, it's purely for testing purposes to see if the tool fits
 your needs. If you'll be using it for your own purpose (personal or
 commercial), you have to use [your own SerpApi key](https://serpapi.com/manage-
 api-key). ## âï¸Installation ```bash $ pip install seo-keyword-research-tool
-``` ```bash $ git clone https://github.com/chukhraiartur/seo-keyword-research-
-tool.git ``` ## ð¤¹ââï¸Usage #### Available CLI arugments: ```bash $
-python main.py -h ``` ```lang-none SerpApi SEO Keyword Research Tool [-h] -q [-
-e [...]] [-dl] [-st] [-ak] [-gd] [-gl] [-hl] Extract keywrods from: Google
-Autocomplete, People Also Ask, and People Also Search and saves data to CSV/
-JSON/TXT. optional arguments: -h, --help show this help message and exit -q , -
--query Search query (required). -e [ ...], --engines [ ...] Choices of engines
-to extract: Autocomplete (ac), Related Searches (rs), People Also Ask (rq). You
-can select multiple engines. All engines are selected by default. -dl , --
-depth-limit Depth limit for People Also Ask. Default is 0, first 2-4 results. -
-st , --save-to Saves the results in the current directory in the selected
-format (CSV, JSON, TXT). Default CSV. -ak , --api-key Your SerpApi API key:
-https://serpapi.com/manage-api-key. Default is a test API key to test CLI. -gd
-, --domain Google domain: https://serpapi.com/google-domains. Default
-google.com. -gl , --country Country of the search: https://serpapi.com/google-
-countries. Default us. -hl , --lang Language of the search: https://
-serpapi.com/google-languages. Default en. Found a bug? Open issue: https://
-github.com/chukhraiartur/seo-keyword-research-tool/issues ``` The `--depth-
-limit` argument for People Also Ask can be set from `0` to `4`. For each depth
-limit value, the number of results returned grows exponentially. Below is a
-table showing how the depth limit argument is affected: | Depth limit | Number
-of results | Explanation | |-------------|-------------------|-------------| |
-0 | 4 | Standard results | | 1 | 12 | 4*2 = 8 + 4 = 12 | | 2 | 36 | 8*3 = 24 +
-12 = 36 | | 3 | 108 | 24*3 = 72 + 36 = 108 | | 4 | 324 | 72*3 = 216 + 108 = 324
-| ðNote: This is how the logic works for the `google.com` domain, on other
-domains the results may differ. #### Simple example: ```bash $ python main.py -
+``` ## ð¤¹ââï¸Usage #### Available CLI arugments: ```bash $ seo -h ```
+```lang-none SerpApi SEO Keyword Research Tool [-h] -q [-e [...]] [-dl] [-st]
+[-ak] [-gd] [-gl] [-hl] Extract keywrods from: Google Autocomplete, People Also
+Ask, and People Also Search and saves data to CSV/JSON/TXT. optional arguments:
+-h, --help show this help message and exit -q , --query Search query
+(required). -e [ ...], --engines [ ...] Choices of engines to extract:
+Autocomplete (ac), Related Searches (rs), People Also Ask (rq). You can select
+multiple engines. All engines are selected by default. -dl , --depth-limit
+Depth limit for People Also Ask. Default is 0, first 2-4 results. -st , --save-
+to Saves the results in the current directory in the selected format (CSV,
+JSON, TXT). Default CSV. -ak , --api-key Your SerpApi API key: https://
+serpapi.com/manage-api-key. Default is a test API key to test CLI. -gd , --
+domain Google domain: https://serpapi.com/google-domains. Default google.com. -
+gl , --country Country of the search: https://serpapi.com/google-countries.
+Default us. -hl , --lang Language of the search: https://serpapi.com/google-
+languages. Default en. Found a bug? Open issue: https://github.com/
+chukhraiartur/seo-keyword-research-tool/issues ``` The `--depth-limit` argument
+for People Also Ask can be set from `0` to `4`. For each depth limit value, the
+number of results returned grows exponentially. Below is a table showing how
+the depth limit argument is affected: | Depth limit | Number of results |
+Explanation | |-------------|-------------------|-------------| | 0 | 4 |
+Standard results | | 1 | 12 | 4*2 = 8 + 4 = 12 | | 2 | 36 | 8*3 = 24 + 12 = 36
+| | 3 | 108 | 24*3 = 72 + 36 = 108 | | 4 | 324 | 72*3 = 216 + 108 = 324 |
+ðNote: This is how the logic works for the `google.com` domain, on other
+domains the results may differ. #### Simple example: ```bash $ seo -
 q "starbucks coffee" ``` ```json { "auto_complete": [ "starbucks coffee menu",
 "starbucks coffee cups", "starbucks coffee sizes", "starbucks coffee mugs",
 "starbucks coffee gear", "starbucks coffee beans", "starbucks coffee near me",
 "starbucks coffee traveler" ], "related_searches": [ "starbucks near me",
 "starbucks coffee price", "starbucks coffee beans", "starbucks company",
 "starbucks coffee menu", "starbucks merchandise", "starbucks coffee bags" ],
 "related_questions": [ "What is the most popular Starbucks coffee?", "What is
 the number 1 Starbucks drink?", "What is the Tiktok coffee from Starbucks?",
 "Why is Starbucks coffee so famous?" ] } ``` #### Advanced example: This
 example will use [related questions API](https://serpapi.com/related-questions)
-engine with a depth limit value of 2, and saves data to JSON: ```bash $ python
-main.py --api-key  \ > -q "starbucks coffee" \ > -e rq \ > -dl 2 \ > -gd
-google.co.uk \ > -gl uk \ > -hl en \ > -st json \ ``` ```json
-{ "related_questions": [ "What is the best coffee in Starbucks?", "What is a
-popular Starbucks coffee?", "What is the number 1 Starbucks drink?", "Is
-Starbucks expensive?", "What should I try at Starbucks for the first time?",
-"Which Starbucks coffee is best and sweet?", "What is famous in Starbucks in
-India?", "Which Starbucks drink is the best in India?", "Why is Starbucks
-famous?", "What should I order in Starbucks?", "What is the least bitter coffee
-at Starbucks?", "What's the creamiest coffee?", "Which Starbucks coffee is best
-in taste?", "Which Starbucks coffee is best and sweet?", "Which Starbucks
-coffee is best in India?", "Which Starbucks coffee is best for first time?",
-"Why is Starbucks famous?", "What should I order at Starbucks for the first
-time?", "What is the best Starbucks drink for a first time coffee drinker?",
-"What should I order in Starbucks?", "What should I try at Starbucks for the
-first time?", "What is the most famous Starbucks drink?", "Which Starbucks
-coffee is best in taste?", "What coffee orders for beginners?", "What is the
-best thing to get at Starbucks?", "Which Starbucks drink is best?", "Which
-coffee is best in Starbucks India?", "Which Starbucks coffee is best in
-taste?", "Is Dunkin or Starbucks better?", "What are the negatives of
-Starbucks?", "Who has stronger coffee Starbucks or Dunkin?", "Why do people
-prefer Starbucks?", "Why is Starbucks so much better than Dunkin?", "Is
-Starbucks coffee high quality?", "Why is Starbucks coffee so good?", "Do
-Starbucks employees get free food?" ] } ``` #### Example of manual data
-extraction (without CLI): ```python from SeoKeywordResearch import
-SeoKeywordResearch keyword_research = SeoKeywordResearch( query='starbucks
-coffee', api_key='', lang='en', country='us', domain='google.com' )
-auto_complete_results = keyword_research.get_auto_complete()
-related_searches_results = keyword_research.get_related_searches()
-related_questions_results = keyword_research.get_related_questions() data =
-{ 'auto_complete': auto_complete_results, 'related_searches':
-related_searches_results, 'related_questions': related_questions_results }
-keyword_research.print_data(data) ``` ### âContributing Feel free to open bug
-issue, something isn't working, what feature to add, or anything else related
-to Google autocomplete, related searches or people also ask.
+engine with a depth limit value of 2, and saves data to JSON: ```bash $ seo --
+api-key "" \ > -q "starbucks coffee" \ > -e rq \ > -dl 2 \ > -gd google.co.uk \
+> -gl uk \ > -hl en \ > -st json \ ``` ```json { "related_questions": [ "What
+is the best coffee in Starbucks?", "What is a popular Starbucks coffee?", "What
+is the number 1 Starbucks drink?", "Is Starbucks expensive?", "What should I
+try at Starbucks for the first time?", "Which Starbucks coffee is best and
+sweet?", "What is famous in Starbucks in India?", "Which Starbucks drink is the
+best in India?", "Why is Starbucks famous?", "What should I order in
+Starbucks?", "What is the least bitter coffee at Starbucks?", "What's the
+creamiest coffee?", "Which Starbucks coffee is best in taste?", "Which
+Starbucks coffee is best and sweet?", "Which Starbucks coffee is best in
+India?", "Which Starbucks coffee is best for first time?", "Why is Starbucks
+famous?", "What should I order at Starbucks for the first time?", "What is the
+best Starbucks drink for a first time coffee drinker?", "What should I order in
+Starbucks?", "What should I try at Starbucks for the first time?", "What is the
+most famous Starbucks drink?", "Which Starbucks coffee is best in taste?",
+"What coffee orders for beginners?", "What is the best thing to get at
+Starbucks?", "Which Starbucks drink is best?", "Which coffee is best in
+Starbucks India?", "Which Starbucks coffee is best in taste?", "Is Dunkin or
+Starbucks better?", "What are the negatives of Starbucks?", "Who has stronger
+coffee Starbucks or Dunkin?", "Why do people prefer Starbucks?", "Why is
+Starbucks so much better than Dunkin?", "Is Starbucks coffee high quality?",
+"Why is Starbucks coffee so good?", "Do Starbucks employees get free food?" ] }
+``` #### Example of manual data extraction (without CLI): ```python from
+SeoKeywordResearch import SeoKeywordResearch keyword_research =
+SeoKeywordResearch( query='starbucks coffee', api_key='', lang='en',
+country='us', domain='google.com' ) auto_complete_results =
+keyword_research.get_auto_complete() related_searches_results =
+keyword_research.get_related_searches() related_questions_results =
+keyword_research.get_related_questions() data = { 'auto_complete':
+auto_complete_results, 'related_searches': related_searches_results,
+'related_questions': related_questions_results } keyword_research.save_to_json
+(data) keyword_research.print_data(data) ``` ### âContributing Feel free to
+open bug issue, something isn't working, what feature to add, or anything else
+related to Google autocomplete, related searches or people also ask.
```

### Comparing `seo-keyword-research-tool-0.1.8/SeoKeywordResearch/cli.py` & `seo-keyword-research-tool-0.1.9/SeoKeywordResearch/cli.py`

 * *Files identical despite different names*

### Comparing `seo-keyword-research-tool-0.1.8/SeoKeywordResearch/seo_keyword_research.py` & `seo-keyword-research-tool-0.1.9/SeoKeywordResearch/seo_keyword_research.py`

 * *Files identical despite different names*

### Comparing `seo-keyword-research-tool-0.1.8/seo_keyword_research_tool.egg-info/PKG-INFO` & `seo-keyword-research-tool-0.1.9/seo_keyword_research_tool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seo-keyword-research-tool
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python SEO keywords suggestion tool. Google Autocomplete, Related Questions and Related Searches.
 Home-page: https://github.com/chukhraiartur/seo-keyword-research-tool
 Author: Artur Chukhrai
 Author-email: chukhraiartur@gmail.com
 Maintainer: Artur Chukhrai, Dmitiry Zub
 Maintainer-email: chukhraiartur@gmail.com, dimitryzub@gmail.com
 License: MIT
@@ -45,25 +45,21 @@
         
         ## ⚙️Installation
         
         ```bash
         $ pip install seo-keyword-research-tool
         ```
         
-        ```bash
-        $ git clone https://github.com/chukhraiartur/seo-keyword-research-tool.git
-        ```
-        
         
         ## 🤹‍♂️Usage
         
         #### Available CLI arugments:
         
         ```bash
-        $ python main.py -h
+        $ seo -h
         ```
         
         ```lang-none
         SerpApi SEO Keyword Research Tool [-h] -q  [-e  [...]] [-dl] [-st] [-ak] [-gd] [-gl] [-hl]
         
         Extract keywrods from: Google Autocomplete, People Also Ask, and People Also Search and saves data to CSV/JSON/TXT.
         
@@ -93,15 +89,15 @@
         | 4 | 324 | 72*3 = 216 + 108 = 324 |
         
         📌Note: This is how the logic works for the `google.com` domain, on other domains the results may differ.
         
         #### Simple example:
         
         ```bash
-        $ python main.py -q "starbucks coffee"
+        $ seo -q "starbucks coffee"
         ```
         
         ```json
         {
           "auto_complete": [
             "starbucks coffee menu",
             "starbucks coffee cups",
@@ -131,15 +127,15 @@
         ```
         
         #### Advanced example:
         
         This example will use [related questions API](https://serpapi.com/related-questions) engine with a depth limit value of 2, and saves data to JSON:
         
         ```bash
-        $ python main.py --api-key <your_serpapi_api_key> \
+        $ seo --api-key "<your_serpapi_api_key>" \
         > -q "starbucks coffee" \
         > -e rq \
         > -dl 2 \
         > -gd google.co.uk \
         > -gl uk \
         > -hl en \
         > -st json \
@@ -207,14 +203,15 @@
         
         data = {
             'auto_complete': auto_complete_results,
             'related_searches': related_searches_results,
             'related_questions': related_questions_results
         }
         
+        keyword_research.save_to_json(data)
         keyword_research.print_data(data)
         ```
         
         ### ✍Contributing
         
         Feel free to open bug issue, something isn't working, what feature to add, or anything else related to Google autocomplete, related searches or people also ask.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seo-keyword-research-tool Version: 0.1.8 Summary:
+Metadata-Version: 2.1 Name: seo-keyword-research-tool Version: 0.1.9 Summary:
 Python SEO keywords suggestion tool. Google Autocomplete, Related Questions and
 Related Searches. Home-page: https://github.com/chukhraiartur/seo-keyword-
 research-tool Author: Artur Chukhrai Author-email: chukhraiartur@gmail.com
 Maintainer: Artur Chukhrai, Dmitiry Zub Maintainer-email:
 chukhraiartur@gmail.com, dimitryzub@gmail.com License: MIT Project-URL:
 Documentation, https://github.com/chukhraiartur/seo-keyword-research-tool
 Project-URL: Source, https://github.com/chukhraiartur/seo-keyword-research-tool
@@ -23,87 +23,86 @@
 78694043/221098691-5ad4d2b9-0ebd-4c65-ab1e-47a599955e9c.gif) This tool uses
 [SerpApi](https://serpapi.com/) as a tool to parse data from Google search
 results. You can use provided API key that will be available after
 installation, however, it's purely for testing purposes to see if the tool fits
 your needs. If you'll be using it for your own purpose (personal or
 commercial), you have to use [your own SerpApi key](https://serpapi.com/manage-
 api-key). ## âï¸Installation ```bash $ pip install seo-keyword-research-tool
-``` ```bash $ git clone https://github.com/chukhraiartur/seo-keyword-research-
-tool.git ``` ## ð¤¹ââï¸Usage #### Available CLI arugments: ```bash $
-python main.py -h ``` ```lang-none SerpApi SEO Keyword Research Tool [-h] -q [-
-e [...]] [-dl] [-st] [-ak] [-gd] [-gl] [-hl] Extract keywrods from: Google
-Autocomplete, People Also Ask, and People Also Search and saves data to CSV/
-JSON/TXT. optional arguments: -h, --help show this help message and exit -q , -
--query Search query (required). -e [ ...], --engines [ ...] Choices of engines
-to extract: Autocomplete (ac), Related Searches (rs), People Also Ask (rq). You
-can select multiple engines. All engines are selected by default. -dl , --
-depth-limit Depth limit for People Also Ask. Default is 0, first 2-4 results. -
-st , --save-to Saves the results in the current directory in the selected
-format (CSV, JSON, TXT). Default CSV. -ak , --api-key Your SerpApi API key:
-https://serpapi.com/manage-api-key. Default is a test API key to test CLI. -gd
-, --domain Google domain: https://serpapi.com/google-domains. Default
-google.com. -gl , --country Country of the search: https://serpapi.com/google-
-countries. Default us. -hl , --lang Language of the search: https://
-serpapi.com/google-languages. Default en. Found a bug? Open issue: https://
-github.com/chukhraiartur/seo-keyword-research-tool/issues ``` The `--depth-
-limit` argument for People Also Ask can be set from `0` to `4`. For each depth
-limit value, the number of results returned grows exponentially. Below is a
-table showing how the depth limit argument is affected: | Depth limit | Number
-of results | Explanation | |-------------|-------------------|-------------| |
-0 | 4 | Standard results | | 1 | 12 | 4*2 = 8 + 4 = 12 | | 2 | 36 | 8*3 = 24 +
-12 = 36 | | 3 | 108 | 24*3 = 72 + 36 = 108 | | 4 | 324 | 72*3 = 216 + 108 = 324
-| ðNote: This is how the logic works for the `google.com` domain, on other
-domains the results may differ. #### Simple example: ```bash $ python main.py -
+``` ## ð¤¹ââï¸Usage #### Available CLI arugments: ```bash $ seo -h ```
+```lang-none SerpApi SEO Keyword Research Tool [-h] -q [-e [...]] [-dl] [-st]
+[-ak] [-gd] [-gl] [-hl] Extract keywrods from: Google Autocomplete, People Also
+Ask, and People Also Search and saves data to CSV/JSON/TXT. optional arguments:
+-h, --help show this help message and exit -q , --query Search query
+(required). -e [ ...], --engines [ ...] Choices of engines to extract:
+Autocomplete (ac), Related Searches (rs), People Also Ask (rq). You can select
+multiple engines. All engines are selected by default. -dl , --depth-limit
+Depth limit for People Also Ask. Default is 0, first 2-4 results. -st , --save-
+to Saves the results in the current directory in the selected format (CSV,
+JSON, TXT). Default CSV. -ak , --api-key Your SerpApi API key: https://
+serpapi.com/manage-api-key. Default is a test API key to test CLI. -gd , --
+domain Google domain: https://serpapi.com/google-domains. Default google.com. -
+gl , --country Country of the search: https://serpapi.com/google-countries.
+Default us. -hl , --lang Language of the search: https://serpapi.com/google-
+languages. Default en. Found a bug? Open issue: https://github.com/
+chukhraiartur/seo-keyword-research-tool/issues ``` The `--depth-limit` argument
+for People Also Ask can be set from `0` to `4`. For each depth limit value, the
+number of results returned grows exponentially. Below is a table showing how
+the depth limit argument is affected: | Depth limit | Number of results |
+Explanation | |-------------|-------------------|-------------| | 0 | 4 |
+Standard results | | 1 | 12 | 4*2 = 8 + 4 = 12 | | 2 | 36 | 8*3 = 24 + 12 = 36
+| | 3 | 108 | 24*3 = 72 + 36 = 108 | | 4 | 324 | 72*3 = 216 + 108 = 324 |
+ðNote: This is how the logic works for the `google.com` domain, on other
+domains the results may differ. #### Simple example: ```bash $ seo -
 q "starbucks coffee" ``` ```json { "auto_complete": [ "starbucks coffee menu",
 "starbucks coffee cups", "starbucks coffee sizes", "starbucks coffee mugs",
 "starbucks coffee gear", "starbucks coffee beans", "starbucks coffee near me",
 "starbucks coffee traveler" ], "related_searches": [ "starbucks near me",
 "starbucks coffee price", "starbucks coffee beans", "starbucks company",
 "starbucks coffee menu", "starbucks merchandise", "starbucks coffee bags" ],
 "related_questions": [ "What is the most popular Starbucks coffee?", "What is
 the number 1 Starbucks drink?", "What is the Tiktok coffee from Starbucks?",
 "Why is Starbucks coffee so famous?" ] } ``` #### Advanced example: This
 example will use [related questions API](https://serpapi.com/related-questions)
-engine with a depth limit value of 2, and saves data to JSON: ```bash $ python
-main.py --api-key  \ > -q "starbucks coffee" \ > -e rq \ > -dl 2 \ > -gd
-google.co.uk \ > -gl uk \ > -hl en \ > -st json \ ``` ```json
-{ "related_questions": [ "What is the best coffee in Starbucks?", "What is a
-popular Starbucks coffee?", "What is the number 1 Starbucks drink?", "Is
-Starbucks expensive?", "What should I try at Starbucks for the first time?",
-"Which Starbucks coffee is best and sweet?", "What is famous in Starbucks in
-India?", "Which Starbucks drink is the best in India?", "Why is Starbucks
-famous?", "What should I order in Starbucks?", "What is the least bitter coffee
-at Starbucks?", "What's the creamiest coffee?", "Which Starbucks coffee is best
-in taste?", "Which Starbucks coffee is best and sweet?", "Which Starbucks
-coffee is best in India?", "Which Starbucks coffee is best for first time?",
-"Why is Starbucks famous?", "What should I order at Starbucks for the first
-time?", "What is the best Starbucks drink for a first time coffee drinker?",
-"What should I order in Starbucks?", "What should I try at Starbucks for the
-first time?", "What is the most famous Starbucks drink?", "Which Starbucks
-coffee is best in taste?", "What coffee orders for beginners?", "What is the
-best thing to get at Starbucks?", "Which Starbucks drink is best?", "Which
-coffee is best in Starbucks India?", "Which Starbucks coffee is best in
-taste?", "Is Dunkin or Starbucks better?", "What are the negatives of
-Starbucks?", "Who has stronger coffee Starbucks or Dunkin?", "Why do people
-prefer Starbucks?", "Why is Starbucks so much better than Dunkin?", "Is
-Starbucks coffee high quality?", "Why is Starbucks coffee so good?", "Do
-Starbucks employees get free food?" ] } ``` #### Example of manual data
-extraction (without CLI): ```python from SeoKeywordResearch import
-SeoKeywordResearch keyword_research = SeoKeywordResearch( query='starbucks
-coffee', api_key='', lang='en', country='us', domain='google.com' )
-auto_complete_results = keyword_research.get_auto_complete()
-related_searches_results = keyword_research.get_related_searches()
-related_questions_results = keyword_research.get_related_questions() data =
-{ 'auto_complete': auto_complete_results, 'related_searches':
-related_searches_results, 'related_questions': related_questions_results }
-keyword_research.print_data(data) ``` ### âContributing Feel free to open bug
-issue, something isn't working, what feature to add, or anything else related
-to Google autocomplete, related searches or people also ask. Keywords: google
-scholar,serpapi,scraper,python,python google scholar,python google scholar
-api,web scraping,python web scraping,research,google-search-results,cli
+engine with a depth limit value of 2, and saves data to JSON: ```bash $ seo --
+api-key "" \ > -q "starbucks coffee" \ > -e rq \ > -dl 2 \ > -gd google.co.uk \
+> -gl uk \ > -hl en \ > -st json \ ``` ```json { "related_questions": [ "What
+is the best coffee in Starbucks?", "What is a popular Starbucks coffee?", "What
+is the number 1 Starbucks drink?", "Is Starbucks expensive?", "What should I
+try at Starbucks for the first time?", "Which Starbucks coffee is best and
+sweet?", "What is famous in Starbucks in India?", "Which Starbucks drink is the
+best in India?", "Why is Starbucks famous?", "What should I order in
+Starbucks?", "What is the least bitter coffee at Starbucks?", "What's the
+creamiest coffee?", "Which Starbucks coffee is best in taste?", "Which
+Starbucks coffee is best and sweet?", "Which Starbucks coffee is best in
+India?", "Which Starbucks coffee is best for first time?", "Why is Starbucks
+famous?", "What should I order at Starbucks for the first time?", "What is the
+best Starbucks drink for a first time coffee drinker?", "What should I order in
+Starbucks?", "What should I try at Starbucks for the first time?", "What is the
+most famous Starbucks drink?", "Which Starbucks coffee is best in taste?",
+"What coffee orders for beginners?", "What is the best thing to get at
+Starbucks?", "Which Starbucks drink is best?", "Which coffee is best in
+Starbucks India?", "Which Starbucks coffee is best in taste?", "Is Dunkin or
+Starbucks better?", "What are the negatives of Starbucks?", "Who has stronger
+coffee Starbucks or Dunkin?", "Why do people prefer Starbucks?", "Why is
+Starbucks so much better than Dunkin?", "Is Starbucks coffee high quality?",
+"Why is Starbucks coffee so good?", "Do Starbucks employees get free food?" ] }
+``` #### Example of manual data extraction (without CLI): ```python from
+SeoKeywordResearch import SeoKeywordResearch keyword_research =
+SeoKeywordResearch( query='starbucks coffee', api_key='', lang='en',
+country='us', domain='google.com' ) auto_complete_results =
+keyword_research.get_auto_complete() related_searches_results =
+keyword_research.get_related_searches() related_questions_results =
+keyword_research.get_related_questions() data = { 'auto_complete':
+auto_complete_results, 'related_searches': related_searches_results,
+'related_questions': related_questions_results } keyword_research.save_to_json
+(data) keyword_research.print_data(data) ``` ### âContributing Feel free to
+open bug issue, something isn't working, what feature to add, or anything else
+related to Google autocomplete, related searches or people also ask. Keywords:
+google scholar,serpapi,scraper,python,python google scholar,python google
+scholar api,web scraping,python web scraping,research,google-search-results,cli
 Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Developers Classifier: Operating System :: Microsoft ::
 Windows Classifier: Operating System :: MacOS Classifier: Operating System ::
 POSIX :: Linux Classifier: Topic :: Internet Classifier: Natural Language ::
 English Classifier: Topic :: Utilities Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
```

### Comparing `seo-keyword-research-tool-0.1.8/setup.py` & `seo-keyword-research-tool-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     README = readme_file.read()
 
 setup(
     name='seo-keyword-research-tool',
     description = 'Python SEO keywords suggestion tool. Google Autocomplete, Related Questions and Related Searches.',
     url='https://github.com/chukhraiartur/seo-keyword-research-tool',
-    version='0.1.8',
+    version='0.1.9',
     license='MIT',
     author='Artur Chukhrai',
     author_email='chukhraiartur@gmail.com',
     maintainer='Artur Chukhrai, Dmitiry Zub',
     maintainer_email='chukhraiartur@gmail.com, dimitryzub@gmail.com',
     long_description_content_type='text/markdown',
     long_description=README,
```

