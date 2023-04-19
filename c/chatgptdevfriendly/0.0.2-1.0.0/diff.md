# Comparing `tmp/chatgptdevfriendly-0.0.2.tar.gz` & `tmp/chatgptdevfriendly-1.0.0.tar.gz`

## Comparing `chatgptdevfriendly-0.0.2.tar` & `chatgptdevfriendly-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0    59016 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.2/printed_metrics.png
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.2/requirements.txt
--rw-r--r--   0        0        0    43746 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.2/response_times.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.2/src/chatgptdevfriendly/__init__.py
--rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.2/src/chatgptdevfriendly/v1.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.2/tests/test_main.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.2/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 chatgptdevfriendly-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    59016 2020-02-02 00:00:00.000000 chatgptdevfriendly-1.0.0/printed_metrics.png
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 chatgptdevfriendly-1.0.0/requirements.txt
+-rw-r--r--   0        0        0    43746 2020-02-02 00:00:00.000000 chatgptdevfriendly-1.0.0/response_time_grp.png
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 chatgptdevfriendly-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chatgptdevfriendly-1.0.0/src/chatgptdevfriendly/__init__.py
+-rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 chatgptdevfriendly-1.0.0/src/chatgptdevfriendly/v1.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 chatgptdevfriendly-1.0.0/tests/test_main.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 chatgptdevfriendly-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 chatgptdevfriendly-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 chatgptdevfriendly-1.0.0/README.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 chatgptdevfriendly-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 chatgptdevfriendly-1.0.0/PKG-INFO
```

### Comparing `chatgptdevfriendly-0.0.2/printed_metrics.png` & `chatgptdevfriendly-1.0.0/printed_metrics.png`

 * *Files identical despite different names*

### Comparing `chatgptdevfriendly-0.0.2/response_times.png` & `chatgptdevfriendly-1.0.0/response_time_grp.png`

 * *Files identical despite different names*

### Comparing `chatgptdevfriendly-0.0.2/src/chatgptdevfriendly/v1.py` & `chatgptdevfriendly-1.0.0/src/chatgptdevfriendly/v1.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,261 +1,315 @@
-import openai
-import time
-from functools import wraps
-import requests
-import logging
-import sys
-import json
-
-import matplotlib.pyplot as plt
-from datetime import datetime
-
-
-
-log_formatter = logging.Formatter('%(asctime)s | %(levelname)s | %(message)s', 
-                            '%m-%d-%Y %H:%M:%S')
-
-
-def retry(tries=5, delay=3, backoff=2):
-    """
-    Retries a function or method until it succeeds or the number of retries is exceeded.
-
-    :param tries: the maximum number of times to retry (default 4).
-    :param delay: the initial delay between retries in seconds (default 3).
-    :param backoff: the backoff multiplier (e.g. value of 2 will double the delay each retry) (default 2).
-    """
-
-    def deco_retry(func):
-        @wraps(func)
-        def f_retry(*args, **kwargs):
-            mtries, mdelay = tries, delay
-            while mtries >= 0:
-                try:
-                    #args[0].logger.info("Trying the the function.......")
-                    return func(*args, **kwargs)
-                except (
-                    openai.error.APIError,
-                    openai.error.APIConnectionError,
-                    requests.exceptions.RequestException,
-                ) as e:
-                    args[0].logger.info(f"Error occurred: {str(e)}")
-                    mtries -= 1
-                    if mtries >= 0:
-                        args[0].logger.info(f"Retrying after {mdelay} seconds...")
-                        time.sleep(mdelay)
-
-                    mdelay *= backoff
-            return func(*args, **kwargs)
-
-        return f_retry
-
-    return deco_retry
-
-
-def dot_product(list1, list2):
-    # Check if the lengths of the two lists are equal
-    if len(list1) != len(list2):
-        raise ValueError("Lists must have same length")
-
-    # Calculate the dot product using a loop
-    dot_product = 0
-    for i in range(len(list1)):
-        dot_product += list1[i] * list2[i]
-
-    return dot_product
-
-
-class ChatGptSmartClient(object):
-    """
-    This is a wrapper class for the chatgpt python api,
-    it is meant to provide developers a smooth expereince in
-    developing chatgpt applications of their own without the need
-    for worrying about things like retries, tracking message history
-    or storing messages. This runs on top of the Chat APIs provided by OpenAI
-    read more on that here: https://platform.openai.com/docs/guides/chat .
-    """
-
-    CONTEXT_TOKEN_LIMIT = 4000
-
-    def __init__(self, api_key: str, model: str, log_info: bool=False):
-        openai.api_key = api_key
-
-        self.instruction_msgs = {
-            "role": "system",
-            "content": "You are a  useful assistant",
-        }
-        self.prev_msgs = [self.instruction_msgs]
-        self.model = model
-        self.rsp_id = 1
-        self.query_id = 0
-
-        self.rsp_time_list = []
-        self.rsp_tstamp_list = []
-        self.total_token_cnt_list = []
-
-        self.rspid_vs_tottokens_dict = {}
-
-        self.total_token_cnt = 0 
-
-        self.log_info = log_info
-        self.logger = logging.getLogger(f"chatgptlogger{time.time()}")
-        self.logger.setLevel(logging.INFO)
-        stdout_handler = logging.StreamHandler(sys.stdout)
-        stdout_handler.setFormatter(log_formatter)
-        self.logger.addHandler(stdout_handler)
-
-
-    @retry()
-    def query(self, query: str, w_context=True, add_to_context=True):
-        # TODO: We coud get the embeddings, cache and further use them to speed up the results.
-        # self.get_embeddings(query=query)
-
-        query = {"role": "user", "content": query}
-        rsp_id = None
-
-        if sum(self.total_token_cnt_list) >= self.CONTEXT_TOKEN_LIMIT:
-            self.trim_conversation()
-
-        if w_context:
-            msgs = self.prev_msgs[:]
-            msgs.append(query)
-        else:
-            msgs = [self.instruction_msgs, query]
-        
-        start_time = time.time()
-        response = openai.ChatCompletion.create(model=self.model, messages=msgs)
-        end_time = time.time()
-
-        if self.log_info:
-            self.logger.info(f"The time taken for this response is : {end_time - start_time} seconds")
-        #print(f"The time taken for this response is : {end_time - start_time} seconds")
-
-        f_resp = response["choices"][0]["message"]
-        tot_token_cnt = response["usage"]["total_tokens"]
-
-        self.rsp_tstamp_list.append(end_time)
-        self.rsp_time_list.append(end_time - start_time)
-        self.total_token_cnt_list.append(tot_token_cnt)
-
-        self.total_token_cnt += tot_token_cnt
-
-
-        if self.log_info:
-            self.logger.info(f"The total token count currently is {self.total_token_cnt}")
-
-        if add_to_context:
-            self.prev_msgs.append(query)
-            self.prev_msgs.append(f_resp)
-            self.rsp_id += 1
-            rsp_id = self.rsp_id
-            self.rspid_vs_tottokens_dict[self.rsp_id] = tot_token_cnt
-
-        #print(self.prev_msgs)
-
-        return f_resp, rsp_id
-
-    def erase_history(self):
-        self.prev_msgs = [self.instruction_msgs]
-        self.rsp_id = len(self.prev_msgs)
-
-
-    # This function is used for getting embeddings and hence maybe
-    # used to speedup the system by caching.
-    def get_embeddings(self, query: str):
-        """_summary_
-
-        Args:
-            query (str): _description_
-        """
-        response = openai.Embedding.create(input=query, model="text-embedding-ada-002")
-        embeddings = response["data"][0]["embedding"]
-        return embeddings
-
-    def rollback_conversation(self, rsp_id):
-        """Rollback conversation to the point of a particular response. 
-
-        Args:
-            rsp_id (int): Id number of previous tracked response to roll back to. 
-        """
-        self.prev_msgs = self.prev_msgs[0:rsp_id]
-        self.rsp_id = len(self.prev_msgs)
-    
-    def print_metrics(self):
-        self.logger.info(f"The total tokens used up-till now is: {self.total_token_cnt}")
-        self.logger.info(f"The average response time is: {sum(self.rsp_time_list)/len(self.rsp_time_list)} sec")
-
-        self.plot_rsp_times()
-
-    def plot_rsp_times(self):
-
-        formatted_timestamps = [datetime.fromtimestamp(ts).strftime('%Y-%m-%d %H:%M:%S') for ts in self.rsp_tstamp_list]
-
-
-        # Plot the response times against the timestamps
-        fig, ax = plt.subplots()
-        ax.plot(formatted_timestamps, self.rsp_time_list)
-        ax.set_xlabel("Timestamp")
-        ax.set_ylabel("Response Time (s)")
-        ax.set_title("ChatGPT API Response Time")
-        ax.tick_params(axis='x', rotation=45)
-        ax.xaxis.labelpad = 85
-        ax.yaxis.labelpad = 35
-
-        # Increase the bottom and left margins of the plot
-        plt.subplots_adjust(bottom=0.2, left=0.15)
-
-        plt.xticks(rotation=45, fontsize=6)
-
-        # Save the figure as a PNG file
-        plt.savefig("response_times.png")
-
-        # Show the plot
-        plt.show()
-
-    def dump_context_to_a_file(self, filename="context"):
-        self.dicts_to_jsonl(data_list=self.prev_msgs, filename=filename)
-
-        
-    def dicts_to_jsonl(self, data_list: list, filename: str, compress: bool = True) -> None:
-        """
-        Method saves list of dicts into jsonl file.
-        :param data_list: (list) list of dicts to be stored,
-        :param filename: (str) path to the output file. If suffix .jsonl is not given then methods appends
-            .jsonl suffix into the file.
-        :param compress: (bool) should file be compressed into a gzip archive?
-        """
-        sjsonl = '.jsonl'
-
-        # Check filename
-        if not filename.endswith(sjsonl):
-            filename = filename + sjsonl
-
-        # Save data
-        with open(filename, 'w') as out:
-            for ddict in data_list:
-                jout = json.dumps(ddict) + '\n'
-                out.write(jout)
-    
-    def load_context_from_a_file(self, filename):
-
-        sjsonl = '.jsonl'
-
-        # Check filename
-        if not filename.endswith(sjsonl):
-            filename = filename + sjsonl
-        
-        self.prev_msgs = []
-        
-        with open(filename, encoding='utf-8') as json_file:
-            for line in json_file.readlines():
-                self.prev_msgs.append(line)
-
-        return self.prev_msgs
-
-    def trim_conversation(self):
-        while sum(self.total_token_cnt_list) >= self.CONTEXT_TOKEN_LIMIT:
-
-            del  self.total_token_cnt_list[0]
-            del self.prev_msgs[1]
-            del self.prev_msgs[2]
-        
-        self.logger.info(f"Trimmed the context list to length: {sum(self.total_token_cnt_list)}")
+import openai
+import time
+from functools import wraps
+import requests
+import logging
+import sys
+import json
+
+import matplotlib.pyplot as plt
+from datetime import datetime
+
+
+log_formatter = logging.Formatter(
+    "%(asctime)s | %(levelname)s | %(message)s", "%m-%d-%Y %H:%M:%S"
+)
+
+
+def retry(tries: int = 5, delay: int = 3, backoff: int = 2):
+    """Retry  wrapper, to retry functions on exceptions and errors.
+
+    Args:
+        tries (int, optional): Number of retries. Defaults to 5.
+        delay (int, optional): Time delay in seconds. Defaults to 3.
+        backoff (int, optional): Backoff between the retries. Defaults to 2.
+    """
+
+    def deco_retry(func):
+        @wraps(func)
+        def f_retry(*args, **kwargs):
+            mtries, mdelay = tries, delay
+            while mtries >= 0:
+                try:
+                    # args[0].logger.info("Trying the the function.......")
+                    return func(*args, **kwargs)
+                except (
+                    openai.error.APIError,
+                    openai.error.APIConnectionError,
+                    requests.exceptions.RequestException,
+                ) as e:
+                    args[0].logger.info(f"Error occurred: {str(e)}")
+                    mtries -= 1
+                    if mtries >= 0:
+                        args[0].logger.info(f"Retrying after {mdelay} seconds...")
+                        time.sleep(mdelay)
+
+                    mdelay *= backoff
+            return func(*args, **kwargs)
+
+        return f_retry
+
+    return deco_retry
+
+
+def dot_product(list1: list, list2: list):
+    """Computes the dot product of 2 vectors.
+
+    Args:
+        list1 (int): List 1 values
+        list2 (int): List 2 values
+
+    Raises:
+        ValueError: _description_
+
+    Returns:
+        int: Dot product value of the 2 lists.
+    """
+    # Check if the lengths of the two lists are equal
+    if len(list1) != len(list2):
+        raise ValueError("Lists must have same length")
+
+    # Calculate the dot product using a loop
+    dot_product = 0
+    for i in range(len(list1)):
+        dot_product += list1[i] * list2[i]
+
+    return dot_product
+
+
+class ChatGptSmartClient(object):
+    """
+    This is a wrapper class for the chatgpt python api,
+    it is meant to provide developers a smooth expereince in
+    developing chatgpt applications of their own without the need
+    for worrying about things like retries, tracking message history
+    or storing messages. This runs on top of the Chat APIs provided by OpenAI
+    read more on that here: https://platform.openai.com/docs/guides/chat .
+    """
+
+    CONTEXT_TOKEN_LIMIT = 4000
+
+    def __init__(self, api_key: str, model: str, log_info: bool = False):
+        """Init method to instantiate the client.
+
+        Args:
+            api_key (str): OpenAI api key.
+            model (str): The model to be used for chat completion, ex: "gpt-3.5-turbo"
+            log_info (bool, optional): Whether to log stats for each query. Defaults to False.
+        """
+        openai.api_key = api_key
+
+        self.instruction_msgs = {
+            "role": "system",
+            "content": "You are a  useful assistant",
+        }
+        self.prev_msgs = [self.instruction_msgs]
+        self.model = model
+        self.rsp_id = 1
+        self.query_id = 0
+
+        self.rsp_time_list = []
+        self.rsp_tstamp_list = []
+        self.total_token_cnt_list = []
+
+        self.rspid_vs_tottokens_dict = {}
+
+        self.total_token_cnt = 0
+
+        self.log_info = log_info
+        self.logger = logging.getLogger(f"chatgptlogger{time.time()}")
+        self.logger.setLevel(logging.INFO)
+        stdout_handler = logging.StreamHandler(sys.stdout)
+        stdout_handler.setFormatter(log_formatter)
+        self.logger.addHandler(stdout_handler)
+
+    @retry()
+    def query(self, query: str, w_context: bool = True, add_to_context: bool = True):
+        """Wrapper method to make conversation with ChatGPT apis.
+
+        Args:
+            query (str): Query to send to Chatgpt servers.
+            w_context (bool, optional): Whether to ask this query with previous conversation context. Defaults to True.
+            add_to_context (bool, optional): Whether to add this query and response to conversation context. Defaults to True.
+
+        Returns:
+            OpenAIJson, int: Response to query  and the response id for later rollbck if necessary
+        """
+
+        # TODO: We coud get the embeddings, cache and further use them to speed up the results.
+        # self.get_embeddings(query=query)
+
+        query = {"role": "user", "content": query}
+        rsp_id = None
+
+        if sum(self.total_token_cnt_list) >= self.CONTEXT_TOKEN_LIMIT:
+            self.trim_conversation()
+
+        if w_context:
+            msgs = self.prev_msgs[:]
+            msgs.append(query)
+        else:
+            msgs = [self.instruction_msgs, query]
+
+        start_time = time.time()
+        response = openai.ChatCompletion.create(model=self.model, messages=msgs)
+        end_time = time.time()
+
+        if self.log_info:
+            self.logger.info(
+                f"The time taken for this response is : {end_time - start_time} seconds"
+            )
+        # print(f"The time taken for this response is : {end_time - start_time} seconds")
+
+        f_resp = response["choices"][0]["message"]
+        tot_token_cnt = response["usage"]["total_tokens"]
+
+        self.rsp_tstamp_list.append(end_time)
+        self.rsp_time_list.append(end_time - start_time)
+        self.total_token_cnt_list.append(tot_token_cnt)
+
+        self.total_token_cnt += tot_token_cnt
+
+        if self.log_info:
+            self.logger.info(
+                f"The total token count currently is {self.total_token_cnt}"
+            )
+
+        if add_to_context:
+            self.prev_msgs.append(query)
+            self.prev_msgs.append(f_resp)
+            self.rsp_id += 1
+            rsp_id = self.rsp_id
+            self.rspid_vs_tottokens_dict[self.rsp_id] = tot_token_cnt
+
+        # print(self.prev_msgs)
+
+        return f_resp, rsp_id
+
+    def erase_history(self) -> None:
+        """Removing all previous context."""
+        self.prev_msgs = [self.instruction_msgs]
+        self.rsp_id = len(self.prev_msgs)
+
+    # This function is used for getting embeddings and hence maybe
+    # used to speedup the system by caching.
+    def get_embeddings(self, query: str) -> None:
+        """Calls the OpenAI embeddings API to get the generated embeddings for a query,
+            can be used later for caching and faster response time.
+
+        Args:
+            query (str): Query to be sent to OpenAI servers Chat Apis.
+        """
+        response = openai.Embedding.create(input=query, model="text-embedding-ada-002")
+        embeddings = response["data"][0]["embedding"]
+        return embeddings
+
+    def rollback_conversation(self, rsp_id: int) -> None:
+        """Rollback conversation to the point of a particular response.
+
+        Args:
+            rsp_id (int): Id number of previous tracked response to roll back to.
+        """
+        self.prev_msgs = self.prev_msgs[0:rsp_id]
+        self.rsp_id = len(self.prev_msgs)
+
+    def print_metrics(self) -> None:
+        """Method to log the token usage and response time information."""
+        self.logger.info(
+            f"The total tokens used up-till now is: {self.total_token_cnt}"
+        )
+        self.logger.info(
+            f"The average response time is: {sum(self.rsp_time_list)/len(self.rsp_time_list)} sec"
+        )
+
+        self.plot_rsp_times()
+
+    def plot_rsp_times(self) -> None:
+        """Method to plot the response times versus the timestamps."""
+        formatted_timestamps = [
+            datetime.fromtimestamp(ts).strftime("%Y-%m-%d %H:%M:%S")
+            for ts in self.rsp_tstamp_list
+        ]
+
+        # Plot the response times against the timestamps
+        fig, ax = plt.subplots()
+        ax.plot(formatted_timestamps, self.rsp_time_list)
+        ax.set_xlabel("Timestamp")
+        ax.set_ylabel("Response Time (s)")
+        ax.set_title("ChatGPT API Response Time")
+        ax.tick_params(axis="x", rotation=45)
+        ax.xaxis.labelpad = 85
+        ax.yaxis.labelpad = 35
+
+        # Increase the bottom and left margins of the plot
+        plt.subplots_adjust(bottom=0.2, left=0.15)
+
+        plt.xticks(rotation=45, fontsize=6)
+
+        # Save the figure as a PNG file
+        plt.savefig("response_times.png")
+
+        # Show the plot
+        plt.show()
+
+    def dump_context_to_a_file(self, filename: str = "context"):
+        """Wrapper method to call to dump context to a file.
+
+        Args:
+            filename (str, optional): Filename to dump to. Defaults to "context".
+        """
+        self.dicts_to_jsonl(data_list=self.prev_msgs, filename=filename)
+
+    def dicts_to_jsonl(self, data_list: list, filename: str) -> None:
+        """Method saves context list of dicts to .jsonl format.
+
+        Args:
+            data_list (list): List of dicts of previous conversations
+            filename (str): Filenam to save to
+        """
+        sjsonl = ".jsonl"
+
+        # Check filename
+        if not filename.endswith(sjsonl):
+            filename = filename + sjsonl
+
+        # Save data
+        with open(filename, "w") as out:
+            for ddict in data_list:
+                jout = json.dumps(ddict) + "\n"
+                out.write(jout)
+
+    def load_context_from_a_file(self, filename: str):
+        """Fills up the self.prev_msgs i.e context from a dumped file.
+
+        Args:
+            filename (str): Filename should be a .jsonl file.
+
+        Returns:
+            list: List containing the context information
+        """
+        sjsonl = ".jsonl"
+
+        # Check filename
+        if not filename.endswith(sjsonl):
+            filename = filename + sjsonl
+
+        self.prev_msgs = []
+
+        with open(filename, encoding="utf-8") as json_file:
+            for line in json_file.readlines():
+                self.prev_msgs.append(line)
+
+        return self.prev_msgs
+
+    def trim_conversation(self):
+        """Method to trim, context generatd till now to below the token limit.
+        The queries are removed in FIFO manner until the token count goes below the limit.
+        """
+        while sum(self.total_token_cnt_list) >= self.CONTEXT_TOKEN_LIMIT:
+            del self.total_token_cnt_list[0]
+            del self.prev_msgs[1]
+            del self.prev_msgs[2]
+
+        self.logger.info(
+            f"Trimmed the context list to length: {sum(self.total_token_cnt_list)}"
+        )
```

### Comparing `chatgptdevfriendly-0.0.2/tests/test_main.py` & `chatgptdevfriendly-1.0.0/tests/test_main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-api_key = "api_key"
-model_name = "gpt-3.5-turbo"
-
-from chatgptdevfriendly.v1 import ChatGptSmartClient
-
-
-chatgptsmtclient = ChatGptSmartClient(api_key=api_key, model=model_name, log_info=True)
-
-for _ in range(10):
-    chatgptsmtclient.query("List the top 10 upcoming startups in India?")
-    chatgptsmtclient.query("Ok thanks, can you giv me the valuation of these startups in tabuar format")
-
-chatgptsmtclient.dump_context_to_a_file("context")
-chatgptsmtclient.load_context_from_a_file("context")
-
-chatgptsmtclient.print_metrics()
+api_key = "api_key"
+model_name = "gpt-3.5-turbo"
+
+from chatgptdevfriendly.v1 import ChatGptSmartClient
+
+
+chatgptsmtclient = ChatGptSmartClient(api_key=api_key, model=model_name, log_info=True)
+
+for _ in range(10):
+    chatgptsmtclient.query("List the top 10 upcoming startups in India?")
+    chatgptsmtclient.query(
+        "Ok thanks, can you giv me the valuation of these startups in tabuar format"
+    )
+
+chatgptsmtclient.dump_context_to_a_file("context")
+chatgptsmtclient.load_context_from_a_file("context")
+
+chatgptsmtclient.print_metrics()
```

### Comparing `chatgptdevfriendly-0.0.2/LICENSE.txt` & `chatgptdevfriendly-1.0.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-MIT License
-
-Copyright (c) [year] [fullname]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+MIT License
+
+Copyright (c) [year] [fullname]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `chatgptdevfriendly-0.0.2/README.md` & `chatgptdevfriendly-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-# ChatGPTDevFriendly
-
-
-This package can be used by developers to quickly develop ChatGPT applications with the robustness 
-and boilerplate code being taken care of by this wrapper.
-
-## Requirements 
-`pip install chatgptdevfriendly`
-
-## Usage 
-
-All the source code is currently in `src` directory and also in `tests` with sample usage in `test_main.py`. You will need an [OpenAI key](https://platform.openai.com/account/api-keys
-) to use this. 
-
-```python
-
-from chatgptdevfriendly.v1 import ChatGptSmartClient
-
-chatgpt_client = ChatGptSmartClient(openai_api_key, model_name)
-# We can query with some previous context and also decide whether to add a prompts answer to the context
-prompt="List the top 10 upcoming startups in India?"
-response, response_id = chatgpt_client.query(prompt, w_context=True, add_to_context=True)
-print(f"The answer from ChatGPT is {response}")
-
-# We build on previous context but do not add the current prompts answer to context
-prompt="Ok thanks, can you give me the valuation of these startups in tabular format"
-response  = chatgpt_client.query(prompt, w_context=True, add_to_context=False)
-...
-
-```
-
-## Features
-
-
-- [x] Save Conversations to a file
-- [x] Resume conversations by loading context from a file. 
-- [x] Retry logic in case of API failures.
-- [x] Regular Trimming of context to 4000 tokens so that limit of 4097 is not breached. 
-- [x] Total token and token vs time metric. 
-
-
-- Retries: This is incase of failures like connection based request exceptions, API errors.
-```
-    (openai) C:\Users\Srinivas\OneDrive\Desktop\StartupSearchGPT\tests>python test_main.py
-    Error occurred: API error , please try later
-    Retrying after 3 seconds...
-    Error occurred: API error , please try later
-    Retrying after 6 seconds...
-    Error occurred: API error , please try later
-    Retrying after 12 seconds...
-    Error occurred: API error , please try later
-``` 
-- Context trimming: Context is trimmed as needed when the limit breaches 4000 tokens. 
-![Trimming and printing metrics](printed_metrics.png)
-
-- Tracking metrics such as average time per response and total token usage.
-```
-    04-10-2023 10:26:44 | INFO | The time taken for this response is : 7.85 seconds
-
-    04-10-2023 10:34:34 | INFO | The total tokens used up-till now is: 665
-    04-10-2023 10:34:34 | INFO | The average response time is: 10.28 sec
-```
-![Sample response times graph](response_times.png)
-
-```python
-    chatgpt_client.print_metrics()
-```
-- Erasing Context: We can erase all previous chat history to star from fresh.
-```python
-    chatgpt_client.erase_history()
-```
-- Rollback: we can rollback to a particular Chatresponse context to an restart from there.
-```python
-    chatgpt_client.rollback_conversation(response_id)
-```
-
-- Embeddings: We can get the query embeddings and cache them for further use. (In developement)
-```python
-    chatgpt_client.get_embeddings()
-```
-
-## Contributions
-
-This project is meant to make the chatgpt developer life easy, so please do add any featues you feel is needed! Also if you fnd it useful please leave a star!! 
+# ChatGPTDevFriendly
+
+
+This package can be used by developers to quickly develop ChatGPT applications with the robustness 
+and boilerplate code being taken care of by this wrapper.
+
+## Requirements 
+`pip install chatgptdevfriendly`
+
+## Usage 
+
+All the source code is currently in `src` directory and also in `tests` with sample usage in `test_main.py`. You will need an [OpenAI key](https://platform.openai.com/account/api-keys
+) to use this. 
+
+```python
+
+from chatgptdevfriendly.v1 import ChatGptSmartClient
+
+chatgpt_client = ChatGptSmartClient(openai_api_key, model_name)
+# We can query with some previous context and also decide whether to add a prompts answer to the context
+prompt="List the top 10 upcoming startups in India?"
+response, response_id = chatgpt_client.query(prompt, w_context=True, add_to_context=True)
+print(f"The answer from ChatGPT is {response}")
+
+# We build on previous context but do not add the current prompts answer to context
+prompt="Ok thanks, can you give me the valuation of these startups in tabular format"
+response  = chatgpt_client.query(prompt, w_context=True, add_to_context=False)
+...
+
+```
+
+## Features
+
+
+- [x] Save Conversations to a file
+- [x] Resume conversations by loading context from a file. 
+- [x] Retry logic in case of API failures.
+- [x] Regular Trimming of context to 4000 tokens so that limit of 4097 is not breached. 
+- [x] Total token and token vs time metric. 
+
+
+- Retries: This is incase of failures like connection based request exceptions, API errors.
+```
+    (openai) C:\Users\Srinivas\OneDrive\Desktop\StartupSearchGPT\tests>python test_main.py
+    Error occurred: API error , please try later
+    Retrying after 3 seconds...
+    Error occurred: API error , please try later
+    Retrying after 6 seconds...
+    Error occurred: API error , please try later
+    Retrying after 12 seconds...
+    Error occurred: API error , please try later
+``` 
+- Context trimming: Context is trimmed as needed when the limit breaches 4000 tokens. 
+![Trimming and printing metrics](printed_metrics.png)
+
+- Tracking metrics such as average time per response and total token usage.
+```
+    04-10-2023 10:26:44 | INFO | The time taken for this response is : 7.85 seconds
+
+    04-10-2023 10:34:34 | INFO | The total tokens used up-till now is: 665
+    04-10-2023 10:34:34 | INFO | The average response time is: 10.28 sec
+```
+![Sample response times graph](response_time_grp.png)
+
+```python
+    chatgpt_client.print_metrics()
+```
+- Erasing Context: We can erase all previous chat history to star from fresh.
+```python
+    chatgpt_client.erase_history()
+```
+- Rollback: we can rollback to a particular Chatresponse context to an restart from there.
+```python
+    chatgpt_client.rollback_conversation(response_id)
+```
+
+- Embeddings: We can get the query embeddings and cache them for further use. (In developement)
+```python
+    chatgpt_client.get_embeddings()
+```
+
+## Contributions
+
+This project is meant to make the chatgpt developer life easy, so please do add any featues you feel is needed! Also if you fnd it useful please leave a star!!
```

### Comparing `chatgptdevfriendly-0.0.2/PKG-INFO` & `chatgptdevfriendly-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgptdevfriendly
-Version: 0.0.2
+Version: 1.0.0
 Summary: A wrapper package which takes care of API call robustness to ensure developers quickly and easily develop CHatGPT based applications.
 Project-URL: Homepage, https://github.com/codeastra2/ChatGPTDevFriendly
 Author-email: Srinivas Kumar R <srinivas1996kumar@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -72,15 +72,15 @@
 - Tracking metrics such as average time per response and total token usage.
 ```
     04-10-2023 10:26:44 | INFO | The time taken for this response is : 7.85 seconds
 
     04-10-2023 10:34:34 | INFO | The total tokens used up-till now is: 665
     04-10-2023 10:34:34 | INFO | The average response time is: 10.28 sec
 ```
-![Sample response times graph](response_times.png)
+![Sample response times graph](response_time_grp.png)
 
 ```python
     chatgpt_client.print_metrics()
 ```
 - Erasing Context: We can erase all previous chat history to star from fresh.
 ```python
     chatgpt_client.erase_history()
```

