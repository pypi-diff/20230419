# Comparing `tmp/fasdr-0.0.2.tar.gz` & `tmp/fasdr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasdr-0.0.2.tar", last modified: Wed Apr 19 17:44:11 2023, max compression
+gzip compressed data, was "fasdr-0.0.4.tar", last modified: Wed Apr 19 20:36:02 2023, max compression
```

## Comparing `fasdr-0.0.2.tar` & `fasdr-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:44:11.165659 fasdr-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-19 17:44:11.165659 fasdr-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-19 17:43:59.000000 fasdr-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:44:11.161659 fasdr-0.0.2/fasdr/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-19 17:43:59.000000 fasdr-0.0.2/fasdr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-04-19 17:43:59.000000 fasdr-0.0.2/fasdr/fasdr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:44:11.165659 fasdr-0.0.2/fasdr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-19 17:44:11.000000 fasdr-0.0.2/fasdr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 17:44:11.000000 fasdr-0.0.2/fasdr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 17:44:11.000000 fasdr-0.0.2/fasdr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-19 17:44:11.000000 fasdr-0.0.2/fasdr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 17:44:11.000000 fasdr-0.0.2/fasdr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 17:44:11.165659 fasdr-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-19 17:43:59.000000 fasdr-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:44:11.165659 fasdr-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-19 17:43:59.000000 fasdr-0.0.2/tests/test_fasdr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:36:02.066323 fasdr-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-19 20:36:02.066323 fasdr-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-19 20:35:48.000000 fasdr-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:36:02.066323 fasdr-0.0.4/fasdr/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-19 20:35:48.000000 fasdr-0.0.4/fasdr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-19 20:35:48.000000 fasdr-0.0.4/fasdr/fasdr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:36:02.066323 fasdr-0.0.4/fasdr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-19 20:36:02.000000 fasdr-0.0.4/fasdr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 20:36:02.000000 fasdr-0.0.4/fasdr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:36:02.000000 fasdr-0.0.4/fasdr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-19 20:36:02.000000 fasdr-0.0.4/fasdr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 20:36:02.000000 fasdr-0.0.4/fasdr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:36:02.066323 fasdr-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-19 20:35:48.000000 fasdr-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:36:02.066323 fasdr-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-19 20:35:48.000000 fasdr-0.0.4/tests/test_fasdr.py
```

### Comparing `fasdr-0.0.2/PKG-INFO` & `fasdr-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasdr
-Version: 0.0.2
+Version: 0.0.4
 Summary: Simple dense retrieval using SciPy, spaCy, and Sentence-Transformers
 Home-page: https://github.com/dmarx/fast-and-simple-dense-retrieval/
 Author: David Marx
 Author-email: david.marx84@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -59,16 +59,16 @@
 
 Once you have created the DocumentIndex object, you can search for documents or sentences using the search_documents and search_sentences methods:
 
 ```python
 # Find the top five documents relevant to the query "climate change"
 results = index.search_documents("climate change", k=5)
 
-# Find the top five sentences relevant to the query "climate change"
-results = index.search_sentences("climate change", k=5)
+# Find the top 10 sentences after filtering on the top 5 documents
+results = index.search_sentences_targeted("climate change", n_docs=5, n_sents=10)
 ```
 
 You can customize the behavior of the DocumentIndex object by specifying options such as the model name and the file extensions to include in the index:
 
 ```python
 index = DocumentIndex(
     "/path/to/documents",
```

### Comparing `fasdr-0.0.2/README.md` & `fasdr-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 
 Once you have created the DocumentIndex object, you can search for documents or sentences using the search_documents and search_sentences methods:
 
 ```python
 # Find the top five documents relevant to the query "climate change"
 results = index.search_documents("climate change", k=5)
 
-# Find the top five sentences relevant to the query "climate change"
-results = index.search_sentences("climate change", k=5)
+# Find the top 10 sentences after filtering on the top 5 documents
+results = index.search_sentences_targeted("climate change", n_docs=5, n_sents=10)
 ```
 
 You can customize the behavior of the DocumentIndex object by specifying options such as the model name and the file extensions to include in the index:
 
 ```python
 index = DocumentIndex(
     "/path/to/documents",
```

### Comparing `fasdr-0.0.2/fasdr/fasdr.py` & `fasdr-0.0.4/fasdr/fasdr.py`

 * *Files 21% similar despite different names*

```diff
@@ -106,32 +106,37 @@
         self.sentences = []
         self.sentence_embeddings = None
         self.summary_embedding = None
         self.sentence_index = None
 
         self.embeddings_loaded = False
         self._construct()
-            
-    def _save_summary_embedding(self, save_path: Path):
-        with save_path.open("wb") as file:
-            pickle.dump(self.summary_embedding, file)
 
     def save_embeddings(self):
+        """
+        Save the sentence embeddings and sentences of the document to a file.
+        """
         base_name = self.file_path.stem
         save_path = self.file_path.with_name(f"{base_name}_embeddings.pkl")
 
         data = {
             "sentences": self.sentences,
             "sentence_embeddings": self.sentence_embeddings,
         }
 
         with save_path.open("wb") as file:
             pickle.dump(data, file)
 
     def load_embeddings(self, save_path: Path):
+        """
+        Load the sentence embeddings and sentences of the document from the given file.
+
+        Args:
+            save_path (Path): The file path to load the embeddings and sentences from.
+        """
         with save_path.open("rb") as file:
             data = pickle.load(file)
             self.sentences = data["sentences"]
             self.sentence_embeddings = data["sentence_embeddings"]
             self.sentence_index = create_kdtree(np.array(self.sentence_embeddings))
 
     def _construct(self):
@@ -143,22 +148,22 @@
 
         doc = self.nlp(text)
         self.sentences = [str(sent) for sent in doc.sents]
         if not self.sentences:
             raise EmptyDocument
         self.sentence_embeddings = [sent.vector for sent in doc.sents]
         self.summary_embedding = doc.vector #np.mean(self.sentence_embeddings, axis=0)
+        # to do: don't need to build document index here. make a lazy property
         self.sentence_index = create_kdtree(np.array(self.sentence_embeddings))
 
     def search_sentences(self, query_embedding: np.ndarray, k: int = 1) -> List[Tuple[float, str]]:
         # ensure query is a 2d array
         query_embedding = query_embedding.reshape(1, -1)
 
         if not self.embeddings_loaded:
-            #self._load_all_embeddings()
             self._construct()
             self.embeddings_loaded = True
 
         distances, indices = search_index(self.sentence_index, query_embedding, k)
 
         results = []
         for dist, idx in zip(distances, indices):
@@ -256,30 +261,23 @@
                     subdir_index = DocumentIndex(
                         root_directory=subdir,
                         nlp=self.nlp,
                         extensions=self.extensions,
                         ignored_patterns=self.ignored_patterns,
                         force_reindex=force_reindex,
                     )
-                    #self.documents.extend(subdir_index.documents)
                     self.documents.update(subdir_index.documents)
                 except EmptyDocument:
                     continue
 
-        # Build summary index with new embeddings
-        #dummy_doc = self.nlp("a")
-        #embedding_dim = dummy_doc.vector.shape[0]
-        #self.summary_index = create_kdtree(np.empty((0, embedding_dim)))
-
         if len(self.documents) > 0:
             summary_embeddings = np.array([doc.summary_embedding for doc in self.documents.values()])
             self.summary_index = create_kdtree(summary_embeddings)
         else:
             raise EmptyDocument
-        #self.summary_index = update_kdtree(self.summary_index, summary_embeddings)
 
     def save(self):
         data = {
             "model_name": self.model_name,
             "documents": self.documents,
             "summary_index": self.summary_index,
         }
@@ -290,32 +288,145 @@
     def load(self):
         with self.index_save_path.open("rb") as file:
             data = pickle.load(file)
             self.model_name = data["model_name"]
             self.documents = data["documents"]
             self.summary_index = data["summary_index"]
 
-    def search_documents(self, query: str, k: int = 1) -> List[Tuple[float, Path]]:
-        query_embedding = self.nlp(query).vector
+    def search_documents(
+        self,
+        query: Optional[str]=None,
+        k: int = 1,
+        query_embedding: np.ndarray = None
+    ) -> List[Tuple[float, Path]]:
+        """
+        Search for the documents containing the most similar summary embeddings to the given query.
+
+        Args:
+            query (Optional[str]): The query to search for. If a query embedding is provided, this argument will be ignored.
+            k (int): The number of most similar documents to return.
+            query_embedding (np.ndarray): An optional query embedding to use instead of a query string.
+
+        Returns:
+            List[Tuple[float, Path]]: A list of tuples containing the distances and file paths of the most similar documents.
+        """
+        if query_embedding is None:
+            query_embedding = self.nlp(query).vector
         distances, indices = search_index(self.summary_index, np.array([query_embedding]), k)
-        print("Distances shape:", distances.shape)
-        print("Indices shape:", indices.shape)
 
         results = []
         for dist, idx in zip(distances, indices):
             document_key = list(self.documents.keys())[idx]
             results.append((dist, document_key))
 
         return results
 
-    def search_sentences(self, query: str, k: int = 1) -> List[Tuple[float, Path, List[Tuple[float, str]]]]:
-        doc_results = self.search_documents(query, k)
+    def search_sentences(self, query: str, k: int = 1, query_embedding: np.ndarray = None):
+        """
+        Search for the most similar sentences across all documents to the given query.
+
+        Args:
+            query (str): The query to search for.
+            k (int): The number of most similar sentences to return.
+            query_embedding (np.ndarray): An optional query embedding to use instead of a query string.
+
+        Returns:
+            List[Tuple[float, Path, List[Tuple[float, str]]]]: A list of tuples containing the distances, file paths, and
+            the most similar sentences for each file.
+        """
+        if query_embedding is None:
+            query_embedding = self.nlp(query).vector
+        doc_subset = list(self.documents.values())
+        return self.search_in_documents(query_embedding=query_embedding, docs=doc_subset, k=k)
+
+    def search_sentences_targeted(
+        self, 
+        query: str, 
+        n_docs: int = 1,
+        n_sents: int = 1,
+        query_embedding: np.ndarray = None,
+    ) -> List[Tuple[float, Path, List[Tuple[float, str]]]]:
+        """
+        Search for sentences in the documents that match a query string.
+
+        Args:
+        - query (str): The query string to search for.
+        - n_docs (int): The number of top documents to consider.
+        - n_sents (int): The number of top sentences to return.
+        - query_embedding (np.ndarray): The precomputed query embedding, if any.
+
+        Returns:
+        - List[Tuple[float, Path, List[Tuple[float, str]]]]: A list of tuples containing:
+        - float: The relevance score of the sentence to the query.
+        - Path: The path to the file where the sentence was found.
+        - List[Tuple[float, str]]: A list of tuples containing:
+            - float: The relevance score of the sentence to the query.
+            - str: The sentence text.
+        """
+        if query_embedding is None:
+            query_embedding = self.nlp(query).vector
+
+        if n_docs < len(self.documents):
+            doc_results = self.search_documents(query_embedding=query_embedding, k=n_docs)
+            doc_subset = [self.documents[file_path] for _, file_path in doc_results]
+        else:
+            doc_subset = list(self.documents.values())
+        return self.search_in_documents(query_embedding=query_embedding, docs=doc_subset, k=n_sents)
 
-        query_embedding = self.nlp(query).vector
+    def search_in_documents(self, docs: List[Document], query_embedding: Optional[np.ndarray] = None, k: int = 1):
+        """
+        Search for sentences in a set of documents that match a query embedding.
+
+        Args:
+        - docs (List[Document]): A list of documents to search in.
+        - query_embedding (Optional[np.ndarray]): The precomputed query embedding, if any.
+        - k (int): The number of top sentences to return.
+
+        Returns:
+        - List[Dict[str, Union[float, str]]]: A list of dictionaries containing:
+        - str: The path to the file where the sentence was found.
+        - str: The text of the sentence.
+        - float: The relevance score of the sentence to the query.
+        """
+        filtered = build_targeted_index(docs)
+        distances, indices = search_index(filtered['index'], np.array([query_embedding]), k)
 
         results = []
-        for dist, file_path in doc_results:
-            document = self.documents[file_path]
-            sentence_results = document.search_sentences(np.array([query_embedding]), k)
-            results.append((dist, file_path, sentence_results))
+        for dist, idx in zip(distances, indices):
+            idx = int(idx)
+            fpath = filtered['file_paths'][idx]
+            sent = filtered['sentences'][idx]
+            rec = {'fpath':fpath, 'text':sent, 'score':dist}
+            results.append(rec)
 
         return results
+
+
+def build_targeted_index(docs: List[Document]):
+    """
+    Build a KD-Tree index over the sentence embeddings in a set of documents.
+
+    Args:
+    - docs (List[Document]): A list of documents to build the index from.
+
+    Returns:
+    - Dict[str, Union[List[str], KDTree]]: A dictionary containing:
+      - List[str]: The text of all sentences in the documents.
+      - List[str]: The file paths of all documents in the set, repeated for each of their sentences.
+      - KDTree: The KD-Tree index built from the sentence embeddings.
+    """
+    assert len(docs) >0
+    sentences = []
+    sentence_embeddings = []
+    file_paths = []
+    for doc in docs:
+        assert len(doc.sentences) == len(doc.sentence_embeddings)
+        n = len(doc.sentences)
+        sentences.extend(doc.sentences)
+        sentence_embeddings.extend(doc.sentence_embeddings)
+        file_paths.extend([str(doc.file_path.absolute()) for _ in range(n)])
+    return dict(
+        sentences=sentences,
+        file_paths=file_paths,
+        index=KDTree(np.array(sentence_embeddings)),
+    )
+
```

### Comparing `fasdr-0.0.2/fasdr.egg-info/PKG-INFO` & `fasdr-0.0.4/fasdr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasdr
-Version: 0.0.2
+Version: 0.0.4
 Summary: Simple dense retrieval using SciPy, spaCy, and Sentence-Transformers
 Home-page: https://github.com/dmarx/fast-and-simple-dense-retrieval/
 Author: David Marx
 Author-email: david.marx84@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -59,16 +59,16 @@
 
 Once you have created the DocumentIndex object, you can search for documents or sentences using the search_documents and search_sentences methods:
 
 ```python
 # Find the top five documents relevant to the query "climate change"
 results = index.search_documents("climate change", k=5)
 
-# Find the top five sentences relevant to the query "climate change"
-results = index.search_sentences("climate change", k=5)
+# Find the top 10 sentences after filtering on the top 5 documents
+results = index.search_sentences_targeted("climate change", n_docs=5, n_sents=10)
 ```
 
 You can customize the behavior of the DocumentIndex object by specifying options such as the model name and the file extensions to include in the index:
 
 ```python
 index = DocumentIndex(
     "/path/to/documents",
```

### Comparing `fasdr-0.0.2/setup.py` & `fasdr-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='fasdr',
-    version='0.0.2',
+    version='0.0.4',
     author='David Marx',
     author_email='david.marx84@gmail.com',
     description='Simple dense retrieval using SciPy, spaCy, and Sentence-Transformers',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/dmarx/fast-and-simple-dense-retrieval/',
     packages=['fasdr'],
```

