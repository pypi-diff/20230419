# Comparing `tmp/sarufi-0.1.2-py3-none-any.whl.zip` & `tmp/sarufi-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 13596 bytes, number of entries: 6
--rw-rw-r--  2.0 unx    35250 b- defN 23-Apr-04 10:36 sarufi/__init__.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Apr-04 10:38 sarufi-0.1.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6322 b- defN 23-Apr-04 10:38 sarufi-0.1.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-04 10:38 sarufi-0.1.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-04 10:38 sarufi-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      457 b- defN 23-Apr-04 10:38 sarufi-0.1.2.dist-info/RECORD
-6 files, 53485 bytes uncompressed, 12774 bytes compressed:  76.1%
+Zip file size: 13612 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx    35461 b- defN 23-Apr-19 17:17 sarufi/__init__.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Apr-19 17:20 sarufi-0.1.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6322 b- defN 23-Apr-19 17:20 sarufi-0.1.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-19 17:20 sarufi-0.1.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-19 17:20 sarufi-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      457 b- defN 23-Apr-19 17:20 sarufi-0.1.3.dist-info/RECORD
+6 files, 53696 bytes uncompressed, 12790 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: sarufi/__init__.py
 Comment: 
 
-Filename: sarufi-0.1.2.dist-info/LICENSE
+Filename: sarufi-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: sarufi-0.1.2.dist-info/METADATA
+Filename: sarufi-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: sarufi-0.1.2.dist-info/WHEEL
+Filename: sarufi-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: sarufi-0.1.2.dist-info/top_level.txt
+Filename: sarufi-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: sarufi-0.1.2.dist-info/RECORD
+Filename: sarufi-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sarufi/__init__.py

```diff
@@ -29,15 +29,15 @@
 
     def __init__(
         self,
         client_id: Optional[str] = None,
         client_secret: Optional[str] = None,
         token: Optional[str] = None,
     ) -> None:
-        """Initialize the Sarufi class with username and password or token
+        """Initialize the Sarufi class with client_id and client_secret or token
 
 
         Args:
             client_id (Optional[str], optional): Sarufi API Client ID. Defaults to None.
             client_secret (Optional[str], optional): Sarufi API Client Secret. Defaults to None.
             token (Optional[str], optional): Sarufi API token. Defaults to None.
 
@@ -59,15 +59,15 @@
                     "update_bot",
                     "update_from_file",
                 ]
         """
         self.__client_id = client_id
         self.__client_secret = client_secret
         if token:
-            self.token = token
+            self.token = {"access_token":token}
         else:
             self.token = self.__get_token()
 
     def __get_token(self):
         logging.info("Getting token")
         url = self._BASE_URL + "api/access_token/"
         data = json.dumps(
@@ -299,15 +299,15 @@
 
         Returns:
             Union[Bot, Dict]: Chatbot object if bot created successfully otherwise dict with error message
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('myname@domain.com', 'password')
+        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
         2022-08-23 15:03:00,928 - root - INFO - Getting token
         >>> bot = sarufi.create_bot(name='Maria')
         2022-08-23 15:03:09,891 - root - INFO - Creating bot
         >>> bot
         Bot(id=5, name=Maria, description=PUT DESCRIPTION HERE)
         """
 
@@ -345,15 +345,15 @@
 
         Returns:
             Union[type[Bot], Dict[Any, Any]]: Chatbot object if bot created successfully otherwise dict with error message
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your_email', 'your_password')
+        >>> sarufi = Sarufi('client_id', 'client_secret')
         >>> bot = sarufi.create_from_file(
         ...     intents='data/intents.json',
         ...     flow='data/flow.json',
         ...     metadata='data/metadata.json'
             )"""
 
         if intents:
@@ -395,22 +395,23 @@
             id (int): The ID of the chatbot to update
             name (str, optional): new chatbot name. Defaults to None.
             description (str, optional):new chatbot description . Defaults to None.
             intents (Dict[str, List[str]], optional): updated intents . Defaults to None.
             flow (Dict[str, Any], optional): updated flow . Defaults to None.
             webhook_url(str): The URL to be triggred by the chatbot at the fulfillment of intent
             webhook_trigger_intents(List[str]): Intents to be triggered by the webhook
+            visible_on_community(bool): Should a bot be visible on a community page.
 
         Returns:
             Union[type[Bot], Dict[Any, Any]]: Chatbot object if bot updated successfully otherwise dict with error message
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your_email', 'your_password')
+        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
         >>> bot = sarufi.update_bot(
             ...     id=5,
             ...     name='Maria',
             ...     description='A chatbot that does this and that',
             ...     intents={...},
             ...     flow={...},
             ...     industry='healthcare',
@@ -453,15 +454,15 @@
 
         Returns:
             Union[type[Bot], Dict[Any, Any]]: Chatbot object if bot updated successfully otherwise dict with error message
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your_email', 'your_password')
+        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
         >>> bot = sarufi.update_from_file(
             ...     id=5,
             ...     intents='data/intents.json',
             ...     flow='data/flow.json',
             ...     metadata='data/metadata.json'
             ... )
         """
@@ -496,15 +497,15 @@
 
         Returns:
             Union[Bot, Dict[Any, Any]]: Chatbot object if bot found otherwise dict with error message
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your_email', 'your_password')
+        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
         >>> bot = sarufi.get_bot(id=5)
         >>> print(bot)
         Bot(name='iBank', id=23)
         """
         logging.info("Getting bot with id: {}".format(id))
         url = self._BASE_URL + "chatbot/" + str(id)
         response = self._get_req(url=url)
@@ -519,15 +520,15 @@
 
         Returns:
             Union[List[Bot], Dict]: List of chatbots if successful otherwise dict with error message
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('myname@domain.com', 'password')
+        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
         2022-08-23 15:03:00,928 - root - INFO - Getting token
         >>> sarufi.bots()
         2022-08-23 15:03:57,845 - root - INFO - Getting bots
         [Bot(id=4, name=iBank, description=PUT DESCRIPTION HERE), Bot(id=5, name=Maria, description=Swahili Cognitive Mental Health Chatbot)]
 
         """
         logging.info("Getting bots")
@@ -571,15 +572,15 @@
             message_type (_type_): message type (text, image, audio, video, file)
 
         Returns:
             response (json): bot response
 
         Examples:
             >>> from sarufi import Sarufi
-            >>> sarufi = Sarufi('myname@domain.com', 'password')
+            >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
             >>> sarufi.chat(bot_id=5, chat_id='123456789', message='Hello')
 
             # You can also send direct from bot instance
 
             >>> mybot = sarufi.get_bot(id=5)
             >>> mybot.respond(chat_id='123456789', message='Hello')
         """
@@ -611,15 +612,15 @@
 
         Returns:
             response (json): bot response
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('sarufi-username', 'sarufi-password')
+        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
         >>> sarufi.chat_status(bot_id=5, chat_id='chat_id')
         >>> {'current_state': 'greetings', 'next_state':'end'}
 
         """
         logging.info("Sending message to bot and returning response")
         url = self._BASE_URL + "conversation/allchannels/status"
         data = {
@@ -647,15 +648,15 @@
 
         Returns:
             response (json): bot response
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('sarufi-username', 'sarufi-password')
+        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
         >>> sarufi.update_conversation_state(bot_id=5, chat_id='chat_id', state='greetings')
         >>> {..new state machine..}
 
         """
         logging.info("Sending message to bot and returning response")
         url = self._BASE_URL + "conversation-state"
         data = {
@@ -681,15 +682,15 @@
 
         Returns:
             Dict[Any, Any]: Dict with error message if bot not found otherwise dict with success message
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your-email', 'your-password')
+        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
         >>> sarufi.delete_bot(5)
         {'message': 'Bot with ID 5 deleted successfully'}
         """
         logging.info("Deleting bot")
         url = self._BASE_URL + f"chatbot/{id}"
         response = self._delete_req(url=url)
         return response.json()
@@ -700,15 +701,15 @@
     BOT OBJECT
 
     has `Helper` functions to access bot data in easy way
 
     Examples:
 
     >>> from sarufi import Sarufi
-    >>> sarufi = Sarufi('your_email', 'your_password')
+    >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
     >>> bot = sarufi.get_bot(4)
 
     ### Get bot name
     >>> bot.name
     'iBank'
 
     ### Get bot description
@@ -992,15 +993,15 @@
 
         Returns:
             Dict | None: The response from the bot
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your_email', 'your_password')
+        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
         >>> chatbot = sarufi.get_bot(1)
         >>> chatbot.respond('hello')
         {'message': ['Hello, how can I help you?'], 'next_state': 'greeting'}
         """
         return self.chat(
             bot_id=self.id,
             chat_id=chat_id or self.chat_id,
@@ -1022,15 +1023,15 @@
 
         Returns:
             Dict[bool, str, float]: An object containing the intent, status and the confidence of prediction
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your_email', 'your_password')
+        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
         >>> bot = sarufi.get_bot(id=5)
         >>> print(bot.predict_intent("your message"))
         {
             intent: "an_intent",
             status: true
             confidence: 0.75,
         }
@@ -1051,29 +1052,29 @@
             chat_id (str): The chat id to get the state of
 
         Returns:
             Union[Dict, None]: The state of the chat
 
         Examples:
             >>> from sarufi import Sarufi
-            >>> sarufi = Sarufi('myname@domain.com', 'password')
+            >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
             >>> chatbot = sarufi.get_bot(1)
             >>> chatbot.chat_state('chat_id')
             >>> {'current_state': 'greeting', 'next_state': 'main_menu'}
         """
         return self.chat_status(bot_id=self.id, chat_id=chat_id)
 
     def delete(self):
         """
         delete the bot with the given id
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your-email', 'your-password')
+        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
         >>> chatbot = sarufi.get_bot(1)
         >>> chatbot.delete()
         """
         return self.delete_bot(self.id)
 
     def __str__(self) -> str:
         return f"Bot(id={self.id}, name={self.name})"
```

## Comparing `sarufi-0.1.2.dist-info/LICENSE` & `sarufi-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sarufi-0.1.2.dist-info/METADATA` & `sarufi-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarufi
-Version: 0.1.2
+Version: 0.1.3
 Summary: Opensource python wrapper to Sarufi Conversation API
 Home-page: https://github.com/Neurotech-HQ/sarufi-python-sdk
 Author: Jordan Kalebu
 Author-email: isaackeinstein@gmail.com
 License: MIT
 Download-URL: https://github.com/Neurotech-HQ/sarufi-python-sdk/archive/refs/tags/v0.0.2.tar.gz
 Keywords: sarufi,Sarufi Python SDK,Conversation API python,Swahili Conversational API,Conversational platform Python
```

