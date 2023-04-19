# Comparing `tmp/nriapp-1.0.9.tar.gz` & `tmp/nriapp-1.1.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nriapp-1.0.9.tar", last modified: Fri Feb 24 20:12:35 2023, max compression
+gzip compressed data, was "nriapp-1.1.10.tar", last modified: Wed Apr 19 14:05:54 2023, max compression
```

## Comparing `nriapp-1.0.9.tar` & `nriapp-1.1.10.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-02-24 20:12:35.315151 nriapp-1.0.9/
--rw-rw-rw-   0        0        0      276 2023-02-24 20:12:35.315151 nriapp-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-02-24 16:05:03.000000 nriapp-1.0.9/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-02-24 20:12:35.299551 nriapp-1.0.9/setup/
--rw-rw-rw-   0        0        0     3672 2023-02-02 00:29:38.000000 nriapp-1.0.9/setup/changelog.txt
-drwxrwxrwx   0        0        0        0 2023-02-24 20:12:35.299551 nriapp-1.0.9/setup/config/
--rw-rw-rw-   0        0        0        2 2022-11-03 09:38:26.000000 nriapp-1.0.9/setup/config/__init__.py
--rw-rw-rw-   0        0        0       55 2023-02-23 10:29:55.000000 nriapp-1.0.9/setup/config/config.py
-drwxrwxrwx   0        0        0        0 2023-02-24 20:12:35.299551 nriapp-1.0.9/setup/core/
--rw-rw-rw-   0        0        0        0 2023-02-01 15:18:59.000000 nriapp-1.0.9/setup/core/__init__.py
--rw-rw-rw-   0        0        0     1520 2023-02-06 03:06:19.000000 nriapp-1.0.9/setup/core/abuseipdbapi.py
--rw-rw-rw-   0        0        0    12245 2023-02-23 11:20:22.000000 nriapp-1.0.9/setup/core/msgraphapi.py
--rw-rw-rw-   0        0        0    92843 2023-02-23 16:05:37.000000 nriapp-1.0.9/setup/core/mssentinelapi.py
--rw-rw-rw-   0        0        0     3313 2023-02-09 06:15:42.000000 nriapp-1.0.9/setup/core/multifactor.py
--rw-rw-rw-   0        0        0      640 2023-02-06 14:27:02.000000 nriapp-1.0.9/setup/core/vtquery.py
-drwxrwxrwx   0        0        0        0 2023-02-24 20:12:35.315151 nriapp-1.0.9/setup/helper/
--rw-rw-rw-   0        0        0        2 2023-02-01 15:49:59.000000 nriapp-1.0.9/setup/helper/__init__.py
--rw-rw-rw-   0        0        0     5324 2023-02-24 19:09:03.000000 nriapp-1.0.9/setup/helper/doc.py
--rw-rw-rw-   0        0        0      246 2023-02-23 01:18:54.000000 nriapp-1.0.9/setup/helper/excel.py
--rw-rw-rw-   0        0        0     7620 2023-02-12 08:52:30.000000 nriapp-1.0.9/setup/helper/login.py
--rw-rw-rw-   0        0        0     2443 2023-01-26 11:08:57.000000 nriapp-1.0.9/setup/helper/pylog.py
--rw-rw-rw-   0        0        0     1247 2023-02-08 06:48:37.000000 nriapp-1.0.9/setup/helper/requestheader.py
-drwxrwxrwx   0        0        0        0 2023-02-24 20:12:35.315151 nriapp-1.0.9/setup/logs/
--rw-rw-rw-   0        0        0        2 2022-11-03 09:38:26.000000 nriapp-1.0.9/setup/logs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 20:12:35.315151 nriapp-1.0.9/setup/nriapp.egg-info/
--rw-rw-rw-   0        0        0      276 2023-02-24 20:12:35.000000 nriapp-1.0.9/setup/nriapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      726 2023-02-24 20:12:35.000000 nriapp-1.0.9/setup/nriapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-24 20:12:35.000000 nriapp-1.0.9/setup/nriapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-02-24 20:12:35.000000 nriapp-1.0.9/setup/nriapp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      223 2023-02-24 20:12:35.000000 nriapp-1.0.9/setup/nriapp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-02-24 20:12:35.000000 nriapp-1.0.9/setup/nriapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    26222 2023-02-24 20:11:33.000000 nriapp-1.0.9/setup/nriapp.py
-drwxrwxrwx   0        0        0        0 2023-02-24 20:12:35.315151 nriapp-1.0.9/setup/output/
--rw-rw-rw-   0        0        0        2 2022-11-03 09:38:26.000000 nriapp-1.0.9/setup/output/__init__.py
--rw-rw-rw-   0        0        0      210 2023-02-12 02:05:19.000000 nriapp-1.0.9/setup/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-02-24 20:12:35.315151 nriapp-1.0.9/setup/session/
--rw-rw-rw-   0        0        0        2 2022-11-03 09:38:26.000000 nriapp-1.0.9/setup/session/__init__.py
--rw-rw-rw-   0        0        0       86 2023-02-24 20:12:35.315151 nriapp-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1093 2023-02-24 20:12:04.000000 nriapp-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:54.530306 nriapp-1.1.10/
+-rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.1.10/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.1.10/MANIFEST.in
+-rw-rw-rw-   0        0        0      273 2023-04-19 14:05:54.530306 nriapp-1.1.10/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.1.10/README
+-rw-rw-rw-   0        0        0      287 2023-03-02 08:33:05.000000 nriapp-1.1.10/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-04-19 14:05:54.545906 nriapp-1.1.10/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2023-04-19 14:01:24.000000 nriapp-1.1.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:54.483506 nriapp-1.1.10/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:54.514706 nriapp-1.1.10/src/nriapp/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.10/src/nriapp/__init__.py
+-rw-rw-rw-   0        0        0     3672 2023-02-02 00:29:38.000000 nriapp-1.1.10/src/nriapp/changelog.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:54.514706 nriapp-1.1.10/src/nriapp/config/
+-rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.10/src/nriapp/config/__init__.py
+-rw-rw-rw-   0        0        0       55 2023-03-02 07:59:35.000000 nriapp-1.1.10/src/nriapp/config/config.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:54.530306 nriapp-1.1.10/src/nriapp/core/
+-rw-rw-rw-   0        0        0        0 2023-03-02 07:59:35.000000 nriapp-1.1.10/src/nriapp/core/__init__.py
+-rw-rw-rw-   0        0        0     1520 2023-03-02 07:59:35.000000 nriapp-1.1.10/src/nriapp/core/abuseipdbapi.py
+-rw-rw-rw-   0        0        0    13766 2023-04-19 13:47:32.000000 nriapp-1.1.10/src/nriapp/core/dataexplorer.py
+-rw-rw-rw-   0        0        0    25825 2023-04-19 13:47:32.000000 nriapp-1.1.10/src/nriapp/core/msgraphapi.py
+-rw-rw-rw-   0        0        0   101391 2023-04-19 13:47:32.000000 nriapp-1.1.10/src/nriapp/core/mssentinelapi.py
+-rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.1.10/src/nriapp/core/multifactor.py
+-rw-rw-rw-   0        0        0      640 2023-03-02 07:59:35.000000 nriapp-1.1.10/src/nriapp/core/vtquery.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:54.530306 nriapp-1.1.10/src/nriapp/helper/
+-rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.10/src/nriapp/helper/__init__.py
+-rw-rw-rw-   0        0        0     5696 2023-04-19 13:47:32.000000 nriapp-1.1.10/src/nriapp/helper/doc.py
+-rw-rw-rw-   0        0        0      246 2023-03-02 07:59:35.000000 nriapp-1.1.10/src/nriapp/helper/excel.py
+-rw-rw-rw-   0        0        0     8482 2023-04-19 13:47:32.000000 nriapp-1.1.10/src/nriapp/helper/login.py
+-rw-rw-rw-   0        0        0     2443 2023-03-02 07:59:35.000000 nriapp-1.1.10/src/nriapp/helper/pylog.py
+-rw-rw-rw-   0        0        0     1247 2023-03-02 07:59:35.000000 nriapp-1.1.10/src/nriapp/helper/requestheader.py
+-rw-rw-rw-   0        0        0       92 2023-04-19 13:47:32.000000 nriapp-1.1.10/src/nriapp/helper/visualization.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:54.514706 nriapp-1.1.10/src/nriapp/nriapp.egg-info/
+-rw-rw-rw-   0        0        0      273 2023-04-19 14:05:53.000000 nriapp-1.1.10/src/nriapp/nriapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1024 2023-04-19 14:05:54.000000 nriapp-1.1.10/src/nriapp/nriapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 14:05:53.000000 nriapp-1.1.10/src/nriapp/nriapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-19 14:05:53.000000 nriapp-1.1.10/src/nriapp/nriapp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-04-19 14:05:53.000000 nriapp-1.1.10/src/nriapp/nriapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35379 2023-04-19 13:47:32.000000 nriapp-1.1.10/src/nriapp/nriapp.py
```

### Comparing `nriapp-1.0.9/setup/changelog.txt` & `nriapp-1.1.10/src/nriapp/changelog.txt`

 * *Files identical despite different names*

### Comparing `nriapp-1.0.9/setup/core/abuseipdbapi.py` & `nriapp-1.1.10/src/nriapp/core/abuseipdbapi.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.0.9/setup/core/mssentinelapi.py` & `nriapp-1.1.10/src/nriapp/core/mssentinelapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,105 +102,90 @@
                         dbgPrint.error("Gateway Time-out")
                         sys.exit()  
                     break
                 else:
                     dbgPrint.info("Sending POST request")
                     response = self._session.post(arg, headers=headers, json=data, verify=False)
                     if response.status_code == 440:
-                        login.login().delete_session()
-                        login.login(self.email).login()
+                        login.Login().delete_session()
+                        login.Login(self.email).login()
                         self.load_session()
                     elif response.status_code == 200:
                         break
                     elif response.status_code == 500:
                         message = json.loads(response.text)
                         dbgPrint.error(message["Message"])
                         sys.exit()
                     elif response.status_code == 504:
                         dbgPrint.error("Gateway Time-out")
                         sys.exit()      
             except:
                 continue
         return response
 
-    def get_incidents(self, incidentId = 0, alertStatus=['New','InProgress', 'Resolved'], severity=[256, 128, 64, 32], pageIndex= 1, lookBackInDays = 60, pageSize = 50, sourceFilter=[], titleFilter=["eDiscovery"]):
+    def get_incidents(self, incidentId = [], alertStatus=['New','InProgress', 'Resolved'], severity=[256, 128, 64, 32], pageIndex= 1, lookBackInDays = 60, pageSize = 3000, sourceFilter=[], titleFilter=[], incident_list=[]):
 
         incident_alerts = 'https://security.microsoft.com/apiproxy/mtp/incidentQueue/incidents/alerts'
         json_data = {
             'pageSize': pageSize,
             'lookBackInDays': str(lookBackInDays),
             'isMultipleIncidents': True,
             'alertStatus': alertStatus,
             'severity': severity,
             'pageIndex': pageIndex,
             }
-        response = self._session.post(incident_alerts, json=json_data, verify=False)
+        response = self.tryrequest(incident_alerts, json=json_data)
+        incident_list.extend(json.loads(response.text))
 
-        for _ in range(5):
-            if response.status_code == 440:
-#                raise Exception("Reset")
-                login.Login().delete_session()
-                login.Login(self.email).login()
-                self.load_session()
-                response = self._session.post(incident_alerts, json=json_data, verify=False)                      #Need exception handling
-                if response.status_code == 200:
-                    break
-            elif response.status_code == 200:
-                break
-
-            elif response.status_code == 500:
-                message = json.loads(response.text)
-                dbgPrint.error(message["Message"])
-                sys.exit()
-            elif response.status_code == 504:
-                dbgPrint.error("Gateway Time-out")
-                sys.exit()
-
-        #Need exception here
-        if incidentId:
-            return [i for i in json.loads(response.text) if i["IncidentId"] == int(incidentId)]
+        if len(json.loads(response.text)) == pageSize:
+            items = self.get_incidents(incidentId,pageIndex=pageIndex+1,lookBackInDays = 180, pageSize = 3000)
+            return items
         else:
-            temp = []
-
-            for i in json.loads(response.text):
-                for b in i["DetectionSources"]:
-                    if b in sourceFilter:
-                        continue
-                    for a in titleFilter:
-                        if a not in i["Title"]:
-                            temp.append(i)
-            return temp
-#            return [i for i in json.loads(response.text) if i["DetectionSources"][0] not in sourceFilter and ]
+            if incidentId:
+                temp = []
+                for a in incidentId:
+                    incident = [i for i in incident_list if i["IncidentId"] == a]
+                    if incident:
+                        temp.append(incident[0])
+                return temp
+            else:                      
+                return incident_list
 
     def search_incident(self, query, pageSize=3):
         incident_search = 'https://security.microsoft.com/apiproxy/mtp/incidentSearch'
 
         params = {
             'term': query,
             'pageSize': pageSize
             }
 
         response = self.tryrequest(incident_search, params=params)
 #        response = self._session.get(incident_search, params=params, verify=False)
         return json.loads(response.text)
 
     def save_session(self):
-        if not os.path.exists("./session"):
-            os.makedirs("./session")
-        if not os.path.exists('./session/ms365.pkl'):
-            with open('./session/ms365.pkl', 'wb') as f:
+
+        session_path = os.path.abspath(os.path.dirname(__file__)) + "\..\session"
+        session_file = session_path + "\\ms365.pkl"
+        if not os.path.exists(session_path):
+            os.makedirs(session_path)
+        if not os.path.exists(session_file):
+            with open(session_file, 'wb') as f:
                 pickle.dump(self._cookies, f)   
 
     def load_session(self):
 
-        if os.path.exists('./session/ms365.pkl'):
-            dbgPrint.debug("[+] Loading ./session/ms365.pkl...")
-            with open('./session/ms365.pkl', 'rb') as f:
+        session_path = os.path.abspath(os.path.dirname(__file__)) + "\..\session"
+        session_file = session_path + "\\ms365.pkl"
+
+        if os.path.exists(session_file):
+            dbgPrint.debug("[+] Loading " + session_file)
+            with open(session_file, 'rb') as f:
                 cookies = pickle.load(f)
-            self.__init__(cookies=cookies)
+            self.__init__(email=self.email, cookies=cookies)
             return self
         else:
             login.Login().delete_session()
             login.Login(self.email).login()
             self.load_session()
             return self
 
@@ -288,14 +273,58 @@
             return {
             "attachments" : attachmentsFilters,
             "urls"        : urlFilters
             }
         else:
             {}
 
+    def get_mail_timeline(self, startUtc, endUtc, networkMessageId):
+        metadata_search = "https://security.microsoft.com/apiproxy/di/Find/MailMetaData"
+
+        start = parser.parse(startUtc)
+        start = start - timedelta(days=1)
+        startUtc = start.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
+
+        end = parser.parse(endUtc)
+        end = end + timedelta(days=1)
+        endUtc = end.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
+        params = {
+            'tenantId'  : TENANT_ID,
+            'startTime' : startUtc,
+            'endTime'   : endUtc,
+            'Filter'    : "NetworkMessageId eq '" + networkMessageId + "'"
+            }
+
+        response = self.tryrequest(metadata_search, params=params)
+        object = json.loads(response.text)
+        timeline = []
+        if object["ResultData"] != None:
+            resultData = json.loads(object["ResultData"][0])
+            mailEvents = resultData["MailEvents"]
+            
+            for count, i in enumerate(mailEvents):
+                temp = {}
+                if i["ExecutionTime"]:
+                    utc_time = parser.parse(i["ExecutionTime"])
+                    utc_time = utc_time.replace(tzinfo=pytz.UTC) #replace method      
+                    ph_time=utc_time.astimezone(tz)        #astimezone method
+                    temp["executionTime"] = ph_time.strftime('%Y-%m-%d %H:%M:%S GMT+8')
+#                temp["executionTime"] = i["ExecutionTime"]
+                temp["eventId"] = i["EventId"]
+                temp["action"] = i["Action"]
+                temp["eventType"] = i["EventType"]
+                if i.get("EventResult"):
+                    temp["eventResult"] = i["EventResult"]
+                temp["deliveryFolder"] = i["XmiInfo"].get("DeliveryFolder", "")
+                timeline.append({count: temp})
+            return timeline
+        else:
+            return timeline
+
+
     def get_alert_story(self, alertId):
         
         class Alert:
             def __init__(self, item, source=0, parent=None, parentClass=None):
                 self.alertId = alertId
                 self.source = source
                 if item["type"] == "AlertStory":
@@ -593,40 +622,45 @@
 
                         
                         related_entities  = []
                         data["relatedEntities"] = related_entities
                         for i in self.related_entities:
                             mailMessage = {}
                             if i["type"] == "mailMessage":
-                                mailMessage["recipient"] = i["recipient"]
-
+                                mailMessage["type"] = "email"
+                                mailMessage["recipient"] = i.get("recipient", "")
+                                if "http" in i.get("SourceEntityId", ""):
+                                    mailMessage["SourceEntityId"] = i.get("SourceEntityId")
 
                                 mailMessage["urls"] = [{"url": _, "verdict": None} for _ in i.get("urls", [])]
                                 file_list = i.get("files", [])
                                 
 
-                                networkMessageId = i.get("networkMessageId")
+#                                networkMessageId = i.get("networkMessageId")
                                 urls = self.parentClass.get_mail_metadata(i["receivedDate"], i["receivedDate"], i["networkMessageId"])
 
                                 if urls:
                                     urls = urls["urls"] if urls else {}
-                                for x in urls:
-                                    uri = x["Url"]
-#                                    if x["Verdict"] != None:
+                                    for x in urls:
+                                        uri = x["Url"]
+    #                                    if x["Verdict"] != None:
                                         
-                                    verdict  = x["Verdict"]  if x["Verdict"] != None else None
-                                    for a in mailMessage["urls"]:
+                                        verdict  = x["Verdict"]  if x["Verdict"] != None else None
+                                        if mailMessage["urls"]:
+                                            for a in mailMessage["urls"]:
                                         
-                                        dom = extract(x["Url"].lower())
-                                        old = "{}.{}".format(dom.domain, dom.suffix)
+                                                dom = extract(x["Url"].lower())
+                                                old = "{}.{}".format(dom.domain, dom.suffix)
 
-                                        dom2 = extract(a["url"].lower())
-                                        new = "{}.{}".format(dom2.domain, dom2.suffix)
-                                        if old in a["url"].lower():
-                                                a["verdict"] = verdict
+                                                dom2 = extract(a["url"].lower())
+                                                new = "{}.{}".format(dom2.domain, dom2.suffix)
+                                                if old in a["url"].lower():
+                                                        a["verdict"] = verdict
+                                        else:
+                                            mailMessage["urls"].append({"url" : x["Url"], "verdict": x["Verdict"]})
 
                                 for a in mailMessage["urls"]:
                                     a["url"] = a["url"].replace("https", "hxxps").replace("http", "hxxp").replace(".", "[.]").replace(":","[:]")
 
                                 files = []
                                 for a in file_list:
                                     file = {}
@@ -634,28 +668,30 @@
                                         file["name"] = a["name"]
                                         file["malwareFamily"] = a["MalwareFamily"]
                                         file["type"] = "file"
                                         file["hash"] = [i["value"] for i in a["fileHashes"] if i["algorithm"] == "SHA256"][0] if [i for i in a["fileHashes"] if i.get("$id")] else ""
                                        # file["hash"] = hash["value"]
                                         if file["hash"]:
                                             files.append(file)
+
+
                                 mailMessage["lastRemediationState"] = i.get("lastRemediationState", "")
                                 mailMessage["files"] = files        
                                 mailMessage["senderIP"] = [i.get("senderIP", "")]
-                                mailMessage["sender"] = [i.get("sender", "").replace(".", "[.]").replace("@", "[@]")]
-
+                                mailMessage["sender"] = [i.get("sender", "").replace(".", "[.]").replace("@", "[@]")] if i.get("sender") else [i.get("p1Sender", "").replace(".", "[.]").replace("@", "[@]")]
+#                                mailMessage["p1Sender"] = i.get("p1Sender", "").replace(".", "[.]").replace("@", "[@]")
                                 mailMessage["p2SenderDisplayName"] = [i.get("p2SenderDisplayName", "")]
                                 mailMessage["subject"] = [i.get("subject", "")]
                                 mailMessage["threats"] = i.get("threats", [])
-                                mailMessage["type"] = "email"
+                                timeline = self.parentClass.get_mail_timeline(i["receivedDate"], i["receivedDate"], i["networkMessageId"])
+                                mailMessage["timeline"] = timeline
+
                                 related_entities.append(mailMessage)
 
                         
-
-
             def parse_mcas_alert_story(self, queue=None):
                 if hasattr(self, "items"):
                     data = {}
                     data["type"] = "mcasAlert"
                     if self.description["type"] == "ITPAlertStoryDescription":
 
                         if queue is not None:
@@ -703,14 +739,15 @@
                             data["user"] = user
                             data["value"] = currentValue
 
                         elif "CABINET_DISCOVERY_ALERT_BUILDER_SINGLE_DESCRIPTION" in localizedKey:                                  #Unofficial Cloud Storage Check
                             dbgPrint.info("Unofficial Cloud Storage Check")
                             data["title"] = "Unofficial Cloud Storage Check"
                             pass
+
                         elif "ANUBIS_SUSPICIOUS_IP_DETECTION_DESCRIPTION" in localizedKey:                                           #Activity from a password-spray associated IP address involving one user  
                             info = desArguments["ANUBIS_SUSPICIOUS_IP_DETECTION_DESCRIPTION"]["value"]            
                             ip = info["ips"]
                             riskType = info["risk_type"]
                             user = info["username"]
 
                             data["title"] = "Activity from a password-spray associated IP address involving one user"
@@ -912,26 +949,27 @@
                         description = self.description["text"]
                         dbgPrint.info("Title: %s" % title)
                         dbgPrint.info("Description: %s" % description)
 
                         if queue is not None:
                             queue.put(data)
 
+                        data["alertID"] = "https://security.microsoft.com/alerts/" + self.alertId 
                         data["title"] = title
                         data["description"] = description
                         logonSession = self.items[0]["cloudLogonSession"]
-                        data["sessionId"] = logonSession["sessionId"]
-                        data["userAgent"] = logonSession["userAgent"]
+                        data["sessionId"] = logonSession.get("sessionId", '')
+                        data["userAgent"] = logonSession.get("userAgent", '')
                         data["startTimeUtc"] = logonSession["startTimeUtc"]
-                        account = logonSession["account"]
-                        data["name"] = account["name"]
-                        data["ntDomain"] = account["ntDomain"]
+                        account = logonSession.get("account", '')
+                        data["name"] = account.get("name", '')
+                        data["ntDomain"] = account.get("ntDomain", '')
                         ip = self.items[0]["ip"]
-                        data["address"] = ip["address"]
-                        data["location"] = ip["location"]
+                        data["address"] = ip.get("address", '')
+                        data["location"] = ip.get("location")
                         data["type"] = "cloudLogonSession"
                         data["time"] = self.items[0]["time"]
 
                     else:
                         raise Exception("Error: Unhandled error (MCAS).")
 
 
@@ -1012,14 +1050,24 @@
                                             remediationAction = [item["value"] for item in i.details if item["key"] == "Remediation action"][0] if [item["value"] for item in i.details if item["key"] == "Remediation action"] else "N/A"
                                             remediationStatus = [item["value"] for item in i.details if item["key"] == "Remediation status"][0] if [item["value"] for item in i.details if item["key"] == "Remediation status"] else "N/A"
                                             remediationTime = [item["value"] for item in i.details if item["key"] == "Remediation time"][0] if [item["value"] for item in i.details if item["key"] == "Remediation time"] else "N/A"
                                             detectionTime = [item["value"] for item in i.details if item["key"] == "Detection time"][0] if [item["value"] for item in i.details if item["key"] == "Detection time"] else "N/A"
                                             scanSource = [item["value"] for item in i.details if item["key"] == "Scan source"][0] if [item["value"] for item in i.details if item["key"] == "Scan source"] else "N/A"
 #                                            dbgPrint.info("Title: %s" % title)
 #                                            dbgPrint.info("Threat Name: %s" % threatName)
+                                            if remediationTime != "N/A":
+                                                        utc_time = parser.parse(remediationTime)
+                                                        utc_time = utc_time.replace(tzinfo=pytz.UTC) #replace method      
+                                                        ph_time=utc_time.astimezone(tz)        #astimezone method
+                                                        remediationTime = ph_time.strftime('%Y-%m-%d %H:%M:%S GMT+8')
+                                            if detectionTime != "N/A":
+                                                        utc_time = parser.parse(detectionTime)
+                                                        utc_time = utc_time.replace(tzinfo=pytz.UTC) #replace method      
+                                                        ph_time=utc_time.astimezone(tz)        #astimezone method
+                                                        detectionTime = ph_time.strftime('%Y-%m-%d %H:%M:%S GMT+8')
 
                                             singleFile = {
                                                 "title"             : [title], 
                                                 "threatName"        : [threatName], 
                                                 "sha1"              : sha1,
                                                 "remediationStatus" : remediationStatus,
                                                 "remediationAction" : remediationAction,
@@ -1190,17 +1238,17 @@
                                 title = self.title.get("main", "")
                                 ip = self.entity.get("id", "") if hasattr(self, "entity") else "unknown" 
 
                                 resolved = ""
                                 for i in self.nested_item:
                                     resolved = i.title["main"]
                                 
-                                data["title"] = title,
-                                data["ip"]    = ip,
-                                data["resolved"] = resolved,
+                                data["title"] = title
+                                data["ip"]    = ip
+                                data["resolvedDomain"] = resolved.replace('.', "[.]")
                                 data["alertIds"] = alertIds
                                 data["type"] = "ip_wdatp" 
 
 #                                dbgPrint.info("\n")
 #                                dbgPrint.info("Alert: %s" % title)
 #                                dbgPrint.info("IP: %s" % ip)
 #                                dbgPrint.info("Resolved name: %s" % resolved)
@@ -1217,15 +1265,60 @@
                                 for i in self.associated_alerts:
                                     providerAlertId = i["providerAlertId"]
                                     alertDisplayName = i["alertDisplayName"]
     #                                dbgPrint.info("Alert Id: %s" % providerAlertId)
     #                                dbgPrint.info("Title: %s" % alertDisplayName)
                                     alertIds.append({"AlertID": "https://security.microsoft.com/alerts/" + providerAlertId, "DisplayName": alertDisplayName})
                                 data["type"] = "others"
-                                data["title"] = self.title["main"]
+
+                                if self.title["main"] == "File modify":
+                                    object = [i for i in self.nested_item if i.type=="file" and i.title["intro"]=="Modified File"][0]
+                                    sha1 = [i["value"] for i in object.details if i["key"]=="SHA1"][0] if [i["value"] for i in object.details if i["key"]=="SHA1"] else ""
+                                    path = [i["value"] for i in object.details if i["key"]=="Path"][0] if [i["value"] for i in object.details if i["key"]=="Path"] else ""
+                                    creationTime = [i["value"] for i in object.details if i["key"]=="Creation time"][0] if [i["value"] for i in object.details if i["key"]=="Creation time"] else ""
+                                    lastModifiedTime = [i["value"] for i in object.details if i["key"]=="Last modified time"][0] if [i["value"] for i in object.details if i["key"]=="Last modified time"] else ""
+                                    data["sha1"] = sha1
+                                    data["path"] = path
+                                    data["creationTime"] = creationTime
+                                    data["lastModifiedTime"] = lastModifiedTime
+                                    pid = ""
+                                    sha1 = ""
+                                    commandline = ""
+                                    path = ""
+
+                                    data["parent"] = [{
+                                        "pid": pid,
+                                        "sha1": sha1,
+                                        "commandline" : commandline,
+                                        "path" : path
+                                        }]
+                                    if self.parent is not None:
+                                        parent = self.parent
+                                        pid = [i["value"] for i in parent.details if i["key"]== "Process id"][0] if [i for i in parent.details if i["key"]== "Process id"] else -1
+                                        sha1 = [i["value"] for i in parent.details if i["key"] == "Image file SHA1"][0] if [i for i in parent.details if i["key"] == "Image file SHA1"] else ""
+                                        commandline = [i["value"] for i in parent.details if i["key"] == "Command line"][0] if [i for i in parent.details if i["key"] == "Command line"] else ""
+                                        path = [i["value"] for i in parent.details if i["key"] == "Image file path"][0] if [i["value"] for i in parent.details if i["key"] == "Image file path"] else ""
+                                        parent_process = {
+                                        "pid"        : pid,
+                                        "commandline": commandline,
+                                        "sha1"       : sha1,
+                                        "path"       : path,
+                                        "title"      : self.title["main"],
+                                        }
+                                        data["parent"] = [parent_process]
+                                
+                                elif "SmartScreen" in self.title["main"]:
+                                    data["title"] = self.title["main"]
+                                elif "Http request" in self.title.get("prefix", ""):
+                                    data["title"] = self.title["main"] + " " + self.title["prefix"]
+                                elif "MDE" in self.title["main"]:
+                                    data["title"] = self.title["main"]
+                                else:
+                                   raise RuntimeError("Unsupported alert type {}".format(alertDisplayName))
+                                        
                                 data["alertIds"] = alertIds
 
 
                     elif self.children:
                         for i in self.children:
                             i.parse_wdatp_alert_story(queue)
 
@@ -1468,21 +1561,21 @@
                     else:
                         object = [i for i in accumulator if i["type"] == "others" and i["sha1"] == id][0]
                         if [i for i in object["parent"] if i["commandline"] == parent["commandline"]]:
                             old_object = [i for i in object["parent"] if i["commandline"] == parent["commandline"]][0]
                             if old_object["pid"] == parent["pid"]:
                                 if old_object["path"] != parent["path"]:
                                     old_object["path"].append(parent["path"])
-                                displayName = [i["DisplayName"] for i in parent["alertIds"]]
-
-                                for i in parent["alertIds"]:
-                                    if i["DisplayName"] not in [a["DisplayName"] for a in old_object["alertIds"]] :
-                                        old_object["alertIds"].append(i)
-                                if parent["threatName"] and parent["threatName"][0] not in old_object["threatName"]:
-                                    old_object["threatName"].append(parent["threatName"][0])
+                                if parent.get("alertIds"):
+                                    displayName = [i["DisplayName"] for i in parent["alertIds"]] 
+                                    for i in parent["alertIds"]:
+                                        if i["DisplayName"] not in [a["DisplayName"] for a in old_object["alertIds"]] :
+                                            old_object["alertIds"].append(i)
+                                    if parent["threatName"] and parent["threatName"][0] not in old_object["threatName"]:
+                                        old_object["threatName"].append(parent["threatName"][0])
                         else:
                             object["parent"].append(parent)
                 else:
                     accumulator.append(current)
 
             elif current["type"] == "mdeUrl":
                 id = current["netMsgId"]
@@ -1514,15 +1607,15 @@
                 if id not in id_list["cloudLogonSession"]:
                     id_list["cloudLogonSession"].append(id)
                     accumulator.append(current)
                 else:
                     dbgPrint.warning("Logon Session Duplicate")
 
 
-            elif current["type"] == "mailMessage":
+            elif current["type"] == "mailMessage":  
                 if current.get("relatedEntities"):
                     for id in current["relatedEntities"]:
                         if id["recipient"] not in id_list["email"]:
                             id_list["email"].append(id["recipient"])
                             id["alertId"] = current["alertId"]
                             id["displayName"] = current["displayName"]
                             id["description"] = current["description"]
@@ -1540,14 +1633,16 @@
                                             object["urls"].append(x)
     #                            if id["files"] != object["files"]:
     #                                object["files"] = list(set(id["files"]) | set(object["files"]))            #Unhashable dictionary
                                 if id["senderIP"] != object["senderIP"]:
                                     for y in id["senderIP"]:
                                         if y not in object["senderIP"]:
                                             object["senderIP"].append(y)
+                                if id["sender"] != object["sender"]:
+                                    object["sender"] = list(set(id["sender"]) | set(object["sender"]))
     #                                object["senderIP"] = list(set("senderIP") | set(object["senderIP"]))
                                 if id["p2SenderDisplayName"] != object["p2SenderDisplayName"]:
                                     object["p2SenderDisplayName"] = list(set(id["p2SenderDisplayName"]) | set(object["p2SenderDisplayName"]))
                                 if id["subject"] != object["subject"]:
                                     object["subject"] = list(set(id["subject"]) | set(object["subject"]))
                 else:
                     for id in current["impactedEntities"]:
@@ -1560,19 +1655,21 @@
                             "mailbox"   : id["mailboxAddress"] 
                             }
                         accumulator.append(temp)                
 #            dbgPrint.info(current)
         return accumulator
 
     def get_audit_history(self, incidentId):
+        
 
         classifications = {
             20 : "True Positive",
             10 : "False Positive",
-            30 : "Informational, Expected Activity"
+            30 : "Informational, Expected Activity",
+            0  : "Not set"
             }
 
         determinations = {
             140 : "Line of Business Application", 
             130 : "Confirmed Activity",
             120 : "Not Enough Data to Validata",
             110 : "Not Malicious",
@@ -1580,14 +1677,15 @@
             90  : "Phishing",
             80  : "Compromised Account",
             70  : "Multi Stage Attack",
             60  : "Other",
             50  : "Unwanted Software",
             40  : "Security Testing",
             20  : "Malware",
+            0   : "Not set"
             }
 
         audit_history = "https://security.microsoft.com/apiproxy/mtp/auditHistory/AuditHistory"
 
         params = {
             'entityType' : 'IncidentEntity',
             'id'         : incidentId,
@@ -1606,23 +1704,24 @@
         resolved_timestamp = ""
         assignee = ""
         feedback = ""
         classification = ""
         determination = ""
         for x in range(len(sorted_list)):
             out = {k:v for k,v in [i for i in sorted_list][x].items()}
-            if out["type"] == "Status" and out["newValue"] == '4':   #Changed Status to progress
+            if out["type"] == "AssignedTo":   #Changed Status to progress
                 assigned_timestamp = out["timestamp"]
                 assignee = out["createdBy"]
-            elif out["type"] == "Status" and out["newValue"] == '2':
-                resolved_timestamp = out["timestamp"]
+#            elif out["type"] == "Status" and out["newValue"] == '2':
+#                resolved_timestamp = out["timestamp"]
             elif out["type"] == "Feedback":
                 feedback = out["newValue"]
             elif out["type"] == "Classification":
                 classification = out["newValue"]
+                resolved_timestamp = out["timestamp"]
             elif out["type"] == "Determination":
                 determination = out["newValue"]
 
         if assigned_timestamp:
             utc_time = parser.parse(assigned_timestamp)
             utc_time = utc_time.replace(tzinfo=pytz.UTC) #replace method      
             ph_time=utc_time.astimezone(tz)        #astimezone method
@@ -1644,25 +1743,58 @@
         
         # Determination - 0 - 69 True Positive
         # Classification - 0 - 20 Others
         # Feedback 
 
         return audit
 
+    def get_all_audit_logs(self, incidents):
+
+        id = [i["IncidentId"] for i in incidents]
+
+        audit_history = []
+        
+        for i in id:
+            audit_logs = self.get_audit_history(i)
+            audit_logs["id"] = i
+            audit_history.append(audit_logs)
+            dbgPrint.info(len(audit_history))
+        return audit_history
 
     def get_file_info(self, hash):
 
         file_info = "https://security.microsoft.com/apiproxy/mtp/virusFileReport/VirusTotalFileReport/" 
+        if len(hash) != 40 and len(hash) != 64:
+            return {}
 
         params = {
             "fileIdentifier" : hash
             }
 
         response = self.tryrequest(file_info, params=params)
         info = json.loads(response.text)
 
         if len(hash) != 40:
             info.update({"sha256" : hash.lower()})
         else:
             info.update({"sha1" : hash.lower()})
         
-        return info
+        return info
+
+    def get_device_info(self, senseMachineId):
+
+        machine_info = "https://security.microsoft.com/apiproxy/mtp/getMachine/machines"
+
+        params = {
+            "machineId"         : senseMachineId,
+            "idType"            : "SenseMachineId",
+            "readFromCache"     : "true",
+            "lookingBackIndays" : 180
+            }
+
+        response = self.tryrequest(machine_info, params=params)
+
+        info = json.loads(response.text)
+
+        return info
+        
+
```

### Comparing `nriapp-1.0.9/setup/core/vtquery.py` & `nriapp-1.1.10/src/nriapp/core/vtquery.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.0.9/setup/helper/doc.py` & `nriapp-1.1.10/src/nriapp/helper/doc.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,55 +57,64 @@
 
     def traverse(self, indict):
         self.walk(indict, origin=self.doc, depth=0, indent=self.indent)
 
     def walk(self, indict, origin, depth=0, indent=0):
         new = indent
         if isinstance(indict, dict):
-            depth = depth+1
+#            depth = depth+1
             for k,v in indict.items():
     #            print("\t"*(indent*depth) + k)
                 header = origin.add_paragraph()
                 header.paragraph_format.left_indent = Cm(depth * indent)
                 header.paragraph_format.space_before = Cm(0)
                 header.paragraph_format.space_after = Cm(0)
-                keys = re.sub('([a-zA-Z])', lambda x: x.groups()[0].upper(), k, 1)
+                keys = re.sub('([a-zA-Z])', lambda x: x.groups()[0].upper(), str(k), 1)
                 keys = " ".join(map(str, self.split_on_uppercase(keys, True)))
                 header.add_run(keys + ": ").bold = True
                 if isinstance(v, dict):
+                    
     #                header = origin.add_paragraph()
                     font = header.add_run()
                     font.font.name = name
                     header.paragraph_format.left_indent = Cm(depth * indent)
                     header.paragraph_format.space_before = Cm(0)
                     header.paragraph_format.space_after = Cm(0)
                     self.walk(v, origin, depth=depth+1, indent=indent)
                 elif isinstance(v, list):
                     for i in v:
                         self.walk(i, origin,  depth+1, indent=indent)
                 else:
     #                print("\t"*(indent*depth+1),  v)
-                    header = origin.add_paragraph()
-
-                    header.paragraph_format.left_indent = Cm((depth+1) * indent)
+#                    header = origin.add_paragraph()
+#                    header = origin.add_run()
+#                    header.paragraph_format.left_indent = Cm((depth+1) * indent)
                     header.paragraph_format.space_before = Cm(0)
                     header.paragraph_format.space_after = Cm(0)
                     header.add_run(str(v))
                     #paragraphs[-1].add_run(str(val) + "  ")
         elif isinstance(indict, list):
             for i in indict:
-                self.walk(i, origin,  depth+1, indent=indent)
+                self.walk(i, origin,  depth, indent=indent)
         else:
     #        print ("\t"*(indent*depth) + indict)
             header = origin.add_paragraph()
             header.paragraph_format.left_indent = Cm(depth * indent)
             header.paragraph_format.space_before = Cm(0)
             header.paragraph_format.space_after = Cm(0)
             header.add_run(indict)
 
+    def walk2(self, indict, origin, depth=0, indent=0):
+        new = indent
+        if isinstance(indict, dict):
+            depth = depth+1
+            for k,v in indict.items():
+    #            print("\t"*(indent*depth) + k)
+                header = origin.add_paragraph()
+        pass
 
     def insertHR(self, paragraph):
         p = paragraph._p  # p is the <w:p> XML element
         pPr = p.get_or_add_pPr()
         pBdr = OxmlElement('w:pBdr')
         pPr.insert_element_before(pBdr,
             'w:shd', 'w:tabs', 'w:suppressAutoHyphens', 'w:kinsoku', 'w:wordWrap',
```

### Comparing `nriapp-1.0.9/setup/helper/login.py` & `nriapp-1.1.10/src/nriapp/helper/login.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from seleniumwire import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from webdriver_manager.chrome import ChromeDriverManager            #for ChromeDriver installation
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
-from selenium.common.exceptions import TimeoutException
+from selenium.common.exceptions import TimeoutException, NoSuchElementException
 
 
 import sys, json
 sys.path.append("..") # Adds higher directory to python modules path.
 
 from config.config import *
 
@@ -26,137 +26,172 @@
 #from PyLog import *
 import logging
 from loguru import logger
 
 import time, os, re, pickle
 from pathlib import Path
 
-security_page = 'https://security.microsoft.com/incidents?tid=' + TENANT_ID
+security_page = 'https://security.microsoft.com'
 azuread_page = 'https://portal.azure.com/api/DelegationToken?feature.cacheextensionapp=true&feature.internalgraphapiversion=true&feature.tokencaching=true'
 Endpoint_page = 'https://endpoint.microsoft.com/api/DelegationToken?feature.internalgraphapiversion=true&feature.tokencaching=true'
 
 #dbgPrint = PyLog(__name__, level=logging.INFO, store=False, consolePrint=True)
 
 logger.add(f"./logs/{__name__}.log",mode="w", backtrace=True, diagnose=True, level="DEBUG", filter="Login")
 #logger.add(sys.stdout, backtrace=True, diagnose=True)
 dbgPrint = logger
 class Login(object):
     """description of class"""
-    def __init__(self, email=None):
+    def __init__(self, email=None, organization="kwijp.onmicrosoft.com"):
+        self.organization = organization
         if email != None:
-            self.email = email
+            self.email = email   
 
     def delete_session(self):
-        for p in Path("./session").glob("*.pkl"):
+        session_path = os.path.abspath(os.path.dirname(__file__)) + "\..\session"
+        for p in Path(session_path).glob("*.pkl"):
             os.remove(p)
 
-
     def wait(self, driver, timeout, type, element):
         while True:
             try:
                 WebDriverWait(driver, 20).until(EC.visibility_of_element_located((type, element)))
                 break
             except TimeoutException:
                 dbgPrint.warning("[-] Loading took too much time!!!")
         dbgPrint.debug("[+] Your webpage is ready...")
 
-    def login(self):
+    def web_app(self, driver, web_app, email, organization):
 
-        dbgPrint.info("[+] Checking session...")
+        if driver.current_url == 'data:,':
+            driver.get(web_app)
+        else:
+            driver.execute_script("window.open('');")
+            driver.switch_to.window(driver.window_handles[len(driver.window_handles)-1])
+            driver.get(web_app)
+
+        self.wait(driver, 20, By.XPATH, "//div[contains(text(),'Sign-in options')]")
+        driver.find_element(By.XPATH, "//div[contains(text(),'Sign-in options')]").click()
+        self.wait(driver, 20, By.XPATH, "//div[@data-test-cred-id='organization']")
+        driver.find_element(By.XPATH, "//div[@data-test-cred-id='organization']").click()
+        self.wait(driver, 20, By.ID, "searchOrganizationInput")
+        driver.find_element(By.ID, "searchOrganizationInput").send_keys(organization)
+        driver.find_element(By.ID, "idSIButton9").click()
+        time.sleep(3)
+
+        if "login.microsoftonline.com" not in driver.current_url:
+            return
+
+        self.wait(driver, 20, By.NAME, 'loginfmt')
+        driver.find_element(By.NAME, 'loginfmt').send_keys(email)
+        driver.find_element(By.ID, 'idSIButton9').click()
 
-        if not os.path.exists('./session/ms365.pkl'):
-            dbgPrint.debug("[-] Session does not exists...")
-            options = webdriver.ChromeOptions()
-            options.add_argument('--disable-logging')
-            options.add_experimental_option('excludeSwitches', ['enable-logging'])          #Disable logging of webdriver
-            driver = webdriver.Chrome(ChromeDriverManager().install(), options=options)
-
-            dbgPrint.info("[-] ./session/MS365Dheaders.pkl and ./session/MS365Dcookies.pkl does not exist")
-            time.sleep(1)
-            dbgPrint.debug("[+] Starting new session...")
-            #options = webdriver.EdgeOptions()
-            #driver = webdriver.Edge(options=options)
-            dbgPrint.debug("[+] Logging in...")
-            driver.get(security_page)
-            
-            dbgPrint.debug("[+] Enter your One-Time Code...")
-            self.wait(driver, 20, By.NAME, 'loginfmt')
-            driver.find_element(By.NAME, 'loginfmt').send_keys(self.email)
-            driver.find_element(By.ID, 'idSIButton9').click()
-
-            override = False
-            current_URL = driver.current_url
-            while True:
+        override = False
+        one_time_code = ""
+
+        while len(one_time_code) <= 8:
+            try:
                 one_time_code = WebDriverWait(driver, 20).until(EC.visibility_of_element_located((By.XPATH, "//input[@id='idTxtBx_OTC_Password']"))).get_attribute("value")
-                while len(one_time_code) < 8:
-                    time.sleep(2)                      
-                    try:
-                        one_time_code = WebDriverWait(driver, 20).until(EC.visibility_of_element_located((By.XPATH, "//input[@id='idTxtBx_OTC_Password']"))).get_attribute("value")
-                    except:
-                        if "https://security.microsoft.com" in driver.current_url:
-                            dbgPrint.debug("[+] Button override")
-                            override = True
-                            break
-                if not override:
-                    driver.find_element(By.ID, "idSIButton9").click()
-                    time.sleep(3)                           
-                    dbgPrint.debug("[+] Your one time code is : %s" % one_time_code)
-                if "https://security.microsoft.com" in driver.current_url:
+            except:
+                if "login.microsoftonline.com" not in driver.current_url:
+                    dbgPrint.debug("[+] Button override")
+                    override = True
                     break
+            if len(one_time_code) == 8:
+                driver.find_element(By.ID, "idSIButton9").click()
+
+
+    def create_driver(self):
+        options = webdriver.ChromeOptions()
+        options.add_argument('--disable-logging')
+        options.add_experimental_option('excludeSwitches', ['enable-logging'])          #Disable logging of webdriver
+        driver = webdriver.Chrome(ChromeDriverManager().install(), options=options)
+        return driver
+
+    def login(self):
+        self.driver = self.create_driver()   
+        dbgPrint.info("[+] Checking session...")
+
+#        if not os.path.exists('./session/ms365.pkl'):
+        dbgPrint.debug("[-] Session does not exists...")
+
+        dbgPrint.info("[-] ./session/MS365Dheaders.pkl and ./session/MS365Dcookies.pkl does not exist")
+        time.sleep(1)
+        dbgPrint.debug("[+] Starting new session...")
+        #options = webdriver.EdgeOptions()
+        #driver = webdriver.Edge(options=options)
+        dbgPrint.debug("[+] Logging in...")
+        
+        self.web_app(self.driver , security_page, self.email, self.organization)
+#        self.web_app(driver , security_page, "kwijp.onmicrosoft.com", self.email)
 
-            self.wait(driver, 20, By.XPATH, "//div[@class='ms-List-page']")
+        self.wait(self.driver, 20, By.XPATH, "//div[@class='ms-List-page']")
 
-            time.sleep(10)             
-            alerts = helper.RequestHeader(driver, "incidents/alerts")
-            cookie = alerts.get_param("cookie")
+        time.sleep(10)             
+        auth_header = helper.RequestHeader(self.driver, "api/v2/auth")
+        cookie = auth_header.get_param("cookie")
 
-            dbgPrint.debug("[+] Retrieving current cookie...\n")
+        dbgPrint.debug("[+] Retrieving current cookie...\n")
 
-            mde.MSSentinelApi(cookies=cookie).save_session()
+        mde.MSSentinelApi(cookies=cookie).save_session()
 
-            driver.execute_script('''window.open("https://endpoint.microsoft.com", "_blank")''')
-            driver.switch_to.window(driver.window_handles[1])
-            self.wait(driver, 20, By.XPATH, "//div[contains(text(),'Sign-in options')]")
-            driver.find_element(By.XPATH, "//div[contains(text(),'Sign-in options')]").click()
-            self.wait(driver, 20, By.XPATH, "//div[@data-test-cred-id='organization']")
-            driver.find_element(By.XPATH, "//div[@data-test-cred-id='organization']").click()
-            self.wait(driver, 20, By.ID, "searchOrganizationInput")
-            driver.find_element(By.ID, "searchOrganizationInput").send_keys("kwijp.onmicrosoft.com")
-            driver.find_element(By.ID, "idSIButton9").click()
-            self.wait(driver, 20, By.XPATH, "//div[@class='ext-FlexColumn']//div//div[@data-bind='pcControl: card']")
+        self.web_app(self.driver , "https://endpoint.microsoft.com", self.email, self.organization)
 
+        self.wait(self.driver, 20, By.XPATH, "//div[@class='ext-FlexColumn']//div//div[@data-bind='pcControl: card']")
 
-            time.sleep(10)
+        time.sleep(10)
 
-            http_rqst = helper.RequestHeader(driver, "api/DelegationToken")         #1/27/2023 5:00:48 PM 
-            cookie = http_rqst.get_param("cookie")
+        http_rqst = helper.RequestHeader(self.driver, "api/DelegationToken")         #1/27/2023 5:00:48 PM 
+        cookie = http_rqst.get_param("cookie")
 
-            json_data = json.loads(http_rqst.body)
+        json_data = json.loads(http_rqst.body)
 
-            msgraph.MSGraphApi(cookies=cookie, json=json_data, verify=False).save_session()
+        msgraph.MSGraphApi(cookies=cookie, json=json_data, verify=False).save_session()
 
-            driver.execute_script('''window.open("https://account.activedirectory.windowsazure.com/usermanagement/multifactorverification.aspx?", "_blank")''')
-            driver.switch_to.window(driver.window_handles[2])
+        self.web_app(self.driver , "https://account.activedirectory.windowsazure.com/usermanagement/multifactorverification.aspx?", self.email, self.organization)
 
-            self.wait(driver, 20, By.XPATH, "//div[contains(text(),'Sign-in options')]")
-            driver.find_element(By.XPATH, "//div[contains(text(),'Sign-in options')]").click()
-            self.wait(driver, 20, By.XPATH, "//div[@data-test-cred-id='organization']")
-            driver.find_element(By.XPATH, "//div[@data-test-cred-id='organization']").click()
-            self.wait(driver, 20, By.ID, "searchOrganizationInput")
-            driver.find_element(By.ID, "searchOrganizationInput").send_keys("kwijp.onmicrosoft.com")
-            driver.find_element(By.ID, "idSIButton9").click()
-            self.wait(driver, 20, By.ID, "UserListGrid_ActionBarContainer")
+        self.wait(self.driver, 20, By.ID, "UserListGrid_ActionBarContainer")
 #            self.wait(driver, 20, By.XPATH, "//img[@boxtype='Image' and @title='Search']")
 
-            time.sleep(2)
-            http_rqst = helper.RequestHeader(driver, "/GenericGetAvailableFilters.ajax")         #1/27/2023 5:00:48 PM 
-            cookies = http_rqst.get_param("Cookie")
-            headers = dict(http_rqst.headers._headers)
+        time.sleep(2)
+        http_rqst = helper.RequestHeader(self.driver, "/GenericGetAvailableFilters.ajax")         #1/27/2023 5:00:48 PM 
+        cookies = http_rqst.get_param("Cookie")
+        headers = dict(http_rqst.headers._headers)
+        page = mfa.MultiFactor(cookies=cookies, headers=headers)            
+
+        page.save_session()
+
+        self.driver.quit()
 
-            page = mfa.MultiFactor(cookies=cookies, headers=headers)            
+    def mfa_login(self, email):
+        self.driver = self.create_driver()  
+        self.web_app(self.driver , "https://account.activedirectory.windowsazure.com/usermanagement/multifactorverification.aspx?", email, self.organization)
 
-            page.save_session()
+        self.wait(self.driver, 20, By.ID, "UserListGrid_ActionBarContainer")
+#            self.wait(driver, 20, By.XPATH, "//img[@boxtype='Image' and @title='Search']")
+
+        time.sleep(2)
+        http_rqst = helper.RequestHeader(self.driver, "/GenericGetAvailableFilters.ajax")         #1/27/2023 5:00:48 PM 
+        cookies = http_rqst.get_param("Cookie")
+        headers = dict(http_rqst.headers._headers)
+        page = mfa.MultiFactor(cookies=cookies, headers=headers)            
+
+        page.save_session()
+
+    def msgraph_login(self, email):
+        self.driver = self.create_driver()  
+        self.web_app(self.driver , "https://endpoint.microsoft.com", email, self.organization)
+
+        self.wait(self.driver, 20, By.XPATH, "//div[@class='ext-FlexColumn']//div//div[@data-bind='pcControl: card']")
+#            self.wait(driver, 20, By.XPATH, "//img[@boxtype='Image' and @title='Search']")
 
-            driver.quit()
+        time.sleep(5)       
+        http_rqst = helper.RequestHeader(self.driver, "api/DelegationToken")         #1/27/2023 5:00:48 PM 
+        cookie = http_rqst.get_param("cookie")
+
+        json_data = json.loads(http_rqst.body)         
+        page = msgraph.MSGraphApi(cookies=cookie, json=json_data, verify=False)
+        page.save_session()
 
+        pass
```

### Comparing `nriapp-1.0.9/setup/helper/pylog.py` & `nriapp-1.1.10/src/nriapp/helper/pylog.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.0.9/setup/helper/requestheader.py` & `nriapp-1.1.10/src/nriapp/helper/requestheader.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.0.9/setup/nriapp.py` & `nriapp-1.1.10/src/nriapp/nriapp.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,122 +1,172 @@
 #!/usr/bin/python
+#this is a test
 import os, sys
 import time
 import requests, json, pickle, ast
 import queue
 import re
+
+sys.path.append("..")
+
 from core import msgraphapi as graphapi 
 from core import mssentinelapi as defender
 from core import multifactor as mfaauth
+from core import dataexplorer as dex
 from core.abuseipdbapi import ipquery
 from helper import requestheader as helper
 from helper import login
 from helper.doc import *
 from helper.doc import WordDoc
 from helper.excel import WorkBook
+
+from config.config import *
 from loguru import logger
 from docx import Document
 import argparse
 from datetime import datetime
 from dateutil import parser
 import pytz    
 import json
-from config.config import *
 import configparser
 import pandas as pd
+from urllib.parse import urlparse
 
 requests.packages.urllib3.disable_warnings()        #Disable requests warning logs
 
 logger.add(f"./logs/{__name__}.log", mode="w", backtrace=True, diagnose=True, level="INFO", filter="ChromeDriver")
 #logger.disable(__name__)
 dbgPrint = logger
 #dbgPrint.disable(__name__)
 dbgPrint.disable("core.mssentinelapi")
 dbgPrint.disable("core.msgraphapi")
 dbgPrint.disable("helper.login")
+dbgPrint.disable("core.dataexplorer")
 
 tz = pytz.timezone('Asia/Hong_Kong')
 
 class NriApp:
+    classifications = {
+        20 : "True Positive",
+        10 : "False Positive",
+        30 : "Informational, Expected Activity",
+        0   : "Not set"
+        }
+
+    determinations = {
+        140 : "Line of Business Application", 
+        130 : "Confirmed Activity",
+        120 : "Not Enough Data to Validata",
+        110 : "Not Malicious",
+        100 : "Malicious User Activity",
+        90  : "Phishing",
+        80  : "Compromised Account",
+        70  : "Multi Stage Attack",
+        60  : "Other",
+        50  : "Unwanted Software",
+        40  : "Security Testing",
+        20  : "Malware",
+        0   : "Not set"
+        }
+
+    source_list = {
+        1       : "Endpoint Detection and Response (EDR)",
+        2       : "Antivirus", 
+        4       : "SmartScreen", 
+        32      : "Custom TI",
+        512     : "Microsoft Defender for Office 365 (MDO)",
+        16384   : "Microsoft Defender for Cloud Apps (MCAS)",
+        32768   : "Microsoft 365 Defender",
+        65536   : "Identity Protection",
+        1048576 : "App Governance Policy"
+        }
+
+
+
     def __init__(self, args):
         self.args = args
-        self.__company_name = ""
-        self.__country = ""
+        self.__organization = []
         tracker = {}
 #        self.email = self.args.get("email", "")
 #        self.output = self.args.get("output",  os.path.abspath(os.path.dirname(__file__)) + "\\output")
-        
-
        
         self.write_config()
         self.read_config()
 
         if self.email and not hasattr(self, "msgraph"):
             self.msgraph = graphapi.MSGraphApi(self.email).load_session()
             self.mfa = mfaauth.MultiFactor(self.email).load_session()
             self.sentinel = defender.MSSentinelApi(self.email).load_session()
 
             
     def write_config(self):
-        self.config = configparser.ConfigParser()
-        self.config.read("config.ini")
+        self.config = configparser.RawConfigParser()
+        self.config.read(os.path.abspath(os.path.dirname(__file__)) + '\config.ini')
         flag = False
         if self.args.get("email"):
             if self.config.has_section("email"):
                 flag = True
-                self.config.set("email", "address", self.args["email"])
-#                self.config['email']['address'] = self.args["email"]
+#                self.config.set("email", "address", self.args["email"])
+                self.config['email'] = {"address" : self.args["email"]}
 #                self.email = self.args["email"]
             else:
                 flag = True
                 self.config.add_section("email")
-                self.config["email"]["address"] = self.args["email"]
+                self.config['email'] = {"address" : self.args["email"]}
+#                self.config.set("email", "address", self.args["email"])
+#                self.config["email"]["address"] = self.args["email"]
 #                self.email = self.args["email"]
             
 
         if self.args.get("output"):
             if self.config.has_section("folder"):
                 if not os.path.exists(self.args["output"]):
                     os.makedirs(self.output)     
-                self.config.set("folder", "output", self.args["output"])
+#                self.config.set("folder", "output", self.args["output"])
+                self.config["folder"] = {"output" : self.args["output"]}    
                 flag = True
             else:
                 self.config.add_section('folder')
-                self.config['folder']['output'] = self.args["output"]
+#                self.config['folder']['output'] = self.args["output"]
+                self.config.set("folder", "output", self.args["output"])
                 self.output = self.args["output"]
                 if not os.path.exists(self.output):
                     os.makedirs(self.output)
                 flag = True
 
 #        else:
 #            self.config.add_section('folder')
 #            self.config['folder']['output'] = os.path.abspath(os.path.dirname(__file__))
 #            self.output = os.path.abspath(os.path.dirname(__file__)) + "\\output"
 
         if self.args.get("companytags"):
             if self.config.has_section("companyTags"): 
                 if os.path.exists(self.args["companytags"]):
-                    self.config.set("companyTags", "path", self.args["companytags"])
- #                   self.config["companyTags"]["path"] = self.args["companytags"]
+  #                  self.config.set("companyTags", "path", self.args["companytags"])
+                    self.config["companyTags"]["path"] = self.args["companytags"]
                     flag = True
                 else:
                     dbgPrint.error("No such file {sample}", sample=self.args["companytags"])
                     sys.exit()
             else:
                 self.config.add_section("companyTags")
-                self.config["companyTags"]["path"] = self.args["companytags"]
+#                self.config["companyTags"]["path"] = self.args["companytags"]
                 if os.path.exists(self.args["companytags"]):
-                    self.config["companyTags"]["path"] = self.args["companytags"]
+                    self.config["companyTags"] = {"path": self.args["companytags"]}
+#                    self.config.set("companyTags", "path", self.args["companytags"])
+#                    self.config["companyTags"]["path"] = self.args["companytags"]
                     flag = True
                 
 #        else:
 #            self.config.add_section('companyTags')
 #            self.config["companyTags"]["Path"] = os.path.abspath(os.path.dirname(__file__) + "\\companyTags.csv") 
         if flag:
-            with open(os.path.abspath(os.path.dirname(__file__)) + '\config.ini', 'w+') as configfile:
+
+            with open(os.path.abspath(os.path.dirname(__file__)) + '\config.ini', 'w') as configfile:
+#            with open('.\config.ini', 'w+') as configfile:
                 self.config.write(configfile)
                 dbgPrint.info("Config has been setup.")
                 exit(0)
            
 
     def read_config(self):
 
@@ -136,22 +186,22 @@
             if self.config.has_section('companyTags'):
                 if os.path.exists(self.config["companyTags"]["path"]):
                     df = pd.read_csv(self.config["companyTags"]["path"])
                     df = df.reset_index() 
                     self.tags = [{"Tag": row["Tag"], "Country": row["Country"] , "Company": row["Company"]}  for index, row in df.iterrows()]
                 else:
                     dbgPrint.error("{a} does not exist", a=self.config["companyTags"]["path"])
-                    sys.exit()
+                    sys.exit(1)
             else:
                 dbgPrint.error("No company tags csv yet")
-                sys.exit()
+                sys.exit(1)
 
         else:
             dbgPrint.error("Setup configuration first. Use -h --help for help.")
-            sys.exit()
+            sys.exit(1)
 
 
     def user_summary(self, query):
 
         user_object = self.msgraph.search_user(query)[0] if self.msgraph.search_user(query) else {}
         temp = {}
         if user_object:
@@ -221,19 +271,22 @@
         hash_list = walk_dict(param, hash_list)
         return hash_list
 
     def format_userinfo(self, user_object):
         temp = {}
 
         if user_object["companyName"] != None:
+
             temp["companyName"] = user_object["companyName"]
             for i in self.tags:
-                if i["Tag"].lower() == user_object["companyName"].lower():
-                    self.__company_name = user_object["companyName"]
-                    self.__country = i["Country"]
+                if i["Tag"].lower() in user_object["companyName"].lower():
+                    if user_object["companyName"].lower() not in [z["company"].lower() for z in self.__organization]:
+                        self.__organization.append({"company" :user_object["companyName"], "country": i["Country"]})
+#                    self.__company_name = user_object["companyName"]
+#                    self.__country = i["Country"]
         if user_object["country"] != None:
             temp["country"] = user_object["country"]
         if user_object["usageLocation"] != None:
             temp["usageLocation"] = user_object["usageLocation"]
         if user_object["displayName"] != None:
             temp["name"] = user_object["displayName"] + " (" + user_object["userPrincipalName"] + ")"
         if user_object["userPrincipalName"] != None:
@@ -260,33 +313,19 @@
         machines = param["ImpactedEntities"]["Machines"]
         users = param["ImpactedEntities"]["Users"]
         mailboxes = param["ImpactedEntities"]["Mailboxes"]
         dSource = param["DetectionSources"]
 
         source = []
         for i in dSource:
-            if i == 512:
-                source.append("Microsoft Defender for Office 365 (MDO)")
-            elif i == 2:
-                source.append("Antivirus")
-            elif i == 1:
-                source.append("Endpoint Detection and Response (EDR)")
-            elif i == 4:
-                source.append("SmartScreen")
-            elif i == 65536:
-                source.append("Identity Protection")
-            elif i == 16384:
-                source.append("Microsoft Defender for Cloud Apps (MCAS)")
-            elif i == 32768:
-                source.append("Microsoft 365 Defender")
-            elif i == 32:
-                source.append("Custom TI")
-            else:
-                dbgPrint.error("Unknown source {i}", i)
-                pass
+            try:
+                source.append(self.source_list[i])
+            except:
+                dbgPrint.error("Unknown source : {value}", value=i)
+                continue
 
 #        computerName = param["ComputerDnsName"]
         users_list = []
         for i in users:
             temp = {}
             displayName = i["DisplayName"]
             userName = i["UserName"]
@@ -306,37 +345,70 @@
                 users_list.append(temp)
 
         device_list = []
         for i in machines:
             temp = {}
             computerName = i["ComputerDnsName"]
             exposureScore = i["ExposureScore"]
-            device_object = self.msgraph.search_device_by_name_beta(computerName.split(".")[0])
+            senseMachineId = i["SenseMachineId"]
+#            device_object = self.msgraph.search_device_by_name_beta(computerName.split(".")[0])
             device_object = self.msgraph.search_device_by_name(computerName.split(".")[0])[0] if self.msgraph.search_device_by_name(computerName.split(".")[0]) else {}
             if device_object:
                 if device_object["deviceName"] != 'none':
                     temp["deviceName"] = device_object["deviceName"]
                     for i in self.tags:
-                        if i["Tag"].lower() == device_object["deviceName"].split("-")[0].lower():
-                            self.__company_name = i["Tag"]
-                            self.__country = i["Country"]
+                        if i["Tag"].lower() == device_object["deviceName"].split("-")[0].lower().rstrip('0123456789'):
+                            if i["Tag"].upper() not in [z["company"].upper() for z in self.__organization]:
+                                self.__organization.append({"company" :i["Tag"].upper(), "country": i["Country"]})
+#                            self.__company_name = i["Tag"]
+#                            self.__country = i["Country"]
                 if device_object["complianceState"] != 'none':
                     temp["complianceState"] = device_object["complianceState"]
+                if device_object["azureADDeviceId"] != 'none':
+                    temp["azureADDeviceId"] = device_object["azureADDeviceId"]
                 if device_object["osVersion"] != 'none':
                     temp["osVersion"] = device_object["osVersion"]
-                if device_object["userPrincipalName"] != 'none':
+                if device_object["userPrincipalName"] != 'none' and device_object["userPrincipalName"] != '':
                     user_object = self.msgraph.search_user(device_object["userPrincipalName"])[0] if self.msgraph.search_user(device_object["userPrincipalName"]) else {}
                     user = {}
 #                    temp["userPrincipalName"] = user
                     if user_object:
                         user = self.format_userinfo(user_object)
     #                temp["userPrincipalName"] = device_object["userPrincipalName"]
                     user["groups"] = self.msgraph.get_user_groups(device_object["userPrincipalName"])
                     temp["Owner"] = user
                 device_list.append(temp)
+            else:
+                device_info = self.sentinel.get_device_info(senseMachineId)
+                if device_info:
+                    device_object = self.msgraph.search_device_by_azure_id(device_info["AadDeviceId"])[0] if self.msgraph.search_device_by_azure_id(device_info["AadDeviceId"] ) else {}
+                    if device_object:
+                        if device_object["deviceName"] != 'none':
+                            temp["deviceName"] = device_object["deviceName"]
+                            for i in self.tags:
+                                if i["Tag"].lower() == device_object["deviceName"].split("-")[0].lower().rstrip('0123456789'):
+                                    if i["Tag"].upper() not in [z["company"].upper() for z in self.__organization]:
+                                        self.__organization.append({"company" :i["Tag"], "country": i["Country"]})
+                        if device_object["complianceState"] != 'none':
+                            temp["complianceState"] = device_object["complianceState"]
+                        if device_object["azureADDeviceId"] != 'none':
+                            temp["azureADDeviceId"] = device_object["azureADDeviceId"]
+                        if device_object["osVersion"] != 'none':
+                            temp["osVersion"] = device_object["osVersion"]
+                        if device_object["userPrincipalName"] != 'none':
+                            user_object = self.msgraph.search_user(device_object["userPrincipalName"])[0] if self.msgraph.search_user(device_object["userPrincipalName"]) else {}
+                            user = {}
+        #                    temp["userPrincipalName"] = user
+                            if user_object:
+                                user = self.format_userinfo(user_object)
+            #                temp["userPrincipalName"] = device_object["userPrincipalName"]
+                            user["groups"] = self.msgraph.get_user_groups(device_object["userPrincipalName"])
+                            temp["Owner"] = user
+                        device_list.append(temp)                    
+                pass
 
         mailbox_list = []
         for i in mailboxes:
             temp = {}
             userPrincipalName = i["Upn"]
             user_object = self.msgraph.search_user(userPrincipalName)[0] if self.msgraph.search_user(userPrincipalName) else {}
             if user_object:
@@ -346,47 +418,52 @@
         
         impactedAssets = {"users"       : users_list, 
                          "machines"     : device_list,
                          "mailboxes"    : mailbox_list
                          }
 
 
+        if deviceTags:
+            for i in self.tags:
+                if i["Tag"].lower() == deviceTags[0].split("_")[0].lower():
+                    if i["Tag"].upper() not in [z["company"].upper() for z in self.__organization]:
+                        self.__organization.append({"company" :i["Tag"].upper(), "country": i["Country"]})
+                    break
+
         data["incidentID"]      = incidentId
-        data["incidentTitle"]   = title
-        data["categories"]      = categories
+        data["incidentName"]   = title
         data["severity"]        = severity
-        data["CSIRT Severity"]  = " "
+        data["CSIRTSeverity"]  = " "
+        data["verdict"] = self.classifications[param["Classification"]]
+        data["categories"]      = categories
+        if self.__organization:
+            temp = []
+            for z in self.__organization:
+                temp.append(z["company"] + " - " +  z["country"])
+            data["companyName /Country"] = temp
+        else:
+            data["companyName /Country"] = "N/A"
+#        data["determination"] = self.determinations[param["Determination"]]
         if source:
             data["detectionSource"] = source
         utc_time = parser.parse(firstActivity)
         utc_time = utc_time.replace(tzinfo=pytz.UTC) #replace method      
         ph_time=utc_time.astimezone(tz)        #astimezone method
         data["firstActivity"]   = ph_time.strftime('%Y-%m-%d %H:%M:%S GMT+8')
         utc_time = parser.parse(lastActivity)
         utc_time =utc_time.replace(tzinfo=pytz.UTC) #replace method      
         ph_time=utc_time.astimezone(tz)        #astimezone method
         data["lastActivity"]    = ph_time.strftime('%Y-%m-%d %H:%M:%S GMT+8')
-        if self.__company_name and self.__country:
-            data["companyName/Country"] = self.__company_name + " - " + self.__country
-        elif self.__company_name:
-            data["companyName/Country"] = self.__company_name
-        else:
-            data["companyName/Country"] = "N/A"
-#        if computerName:
-#            data["computerName"]    = computerName
         data["deviceTags"]      = deviceTags
         data["impactedAssets"]  = impactedAssets
-
-        self.__company_name = ""
-        self.__country = ""
-
+        self.__organization = []        
         return data
     
     def ip_summary(self, param, ip_list):
-        ip = param.get("senderIP", "")
+        ip = param.get("senderIP")
         if ip:
             return list(set(ip + ip_list))
         else:
             return ip_list
 
 
     def excel_tracker(self, out):
@@ -412,179 +489,269 @@
             elif impacted["mailboxes"]:
                 for a in impacted["mailboxes"]:
                     for x,y in a.items():
                         if x == "userPrincipalName":
                             if y["companyName"] not in company:
                                 company.append(y["companyName"])
 
+         
+    def get_timely_report(self, lookBackInDays, duration=5):
             
 
-    def get_full_report(self, args=None, lookBackInDays=180):
-        incidents = self.sentinel.get_incidents(incidentId=args, alertStatus=['New','InProgress', 'Resolved'] , severity=[256,128,64,32], pageIndex=1, lookBackInDays=lookBackInDays, pageSize=3000, sourceFilter=[16384, 1048576], titleFilter=["eDiscovery"])       #16384 == MCAS incidents 512 = eDiscovery
-        if args != None:
-            all_data = {}
-#            incidents = self.sentinel.get_incidents(incidentId=args, alertStatus=['New','InProgress', 'Resolved'] , severity=[256,128,64,32], pageIndex=1, lookBackInDays=180, pageSize=3000, sourceFilter=[16384, 65536, 1048576])       
-
-# Identity Protection   65536
-# MS 365 Defender       32768
-# MCAS                  16384
-# MDO                   512
-# Custom TI             32
-# SmartScreen           4
-# Antivirus             2
-# EDR                   1
-
-            doc = WordDoc()
-#            xls = WorkBook(self.output + "\\" + args + "xlsx")
-            ip_list = []
-            hash_list = []
-            recipient = []
-            for i in range(1):
-                q = queue.Queue()    
-                self.sentinel.get_associated_evidences(args, queue=q, lookBackInDays = lookBackInDays)
-                out = self.summary(incidents[0])
-                doc.title(out["incidentTitle"])
-                doc.author(self.email)
-                doc.traverse(out)
-#                self.excel_tracker(out)
-                all_data = self.sentinel.accumulate(q)
-                for a in all_data:
-                    doc.insertHR(doc.insert_paragraph())
-
-                    doc.traverse(a)
-
-                    ip_list = self.ip_summary(a, ip_list)
-                    hash_list = self.file_summary(a, hash_list)
-                    recipient = self.recipient_summary(a, recipient)
 
+        t_end = time.time() + 60 * duration
+        dataexplorer = dex.DataIngestion()
+        while time.time() < t_end:
+
+            dbgPrint.debug("Fetching incidents data")
+            incidents = self.sentinel.get_incidents(incidentId=0, 
+                                                    alertStatus=['New','InProgress', 'Resolved'] , 
+                                                    severity=[256,128,64,32], 
+                                                    pageIndex=1, 
+                                                    lookBackInDays=lookBackInDays, 
+                                                    pageSize=3000, 
+                                                    ) #sourceFilter=[16384, 1048576], titleFilter=["eDiscovery"]      #16384 == MCAS incidents 512 = eDiscovery
+
+    #        incidents_cpy = incidents[:]
+
+            if not dataexplorer.check_ingest_managed_devices_tag():
+                dbgPrint.debug("Fetching all Intune devices")
+                devices = self.msgraph.get_all_devices_beta()
+                dbgPrint.debug("Ingesting data")
+                dataexplorer.ingest_managed_devices(data=devices)
+                del devices[:]
+            
+            if not dataexplorer.check_ingest_devices_tags():
+                dbgPrint.debug("Fetching managed devices list")
+                devices = self.msgraph.get_all_devices()
+                dbgPrint.debug("Ingesting data")
+                dataexplorer.ingest_devices(data=devices)
+                del devices[:]
+
+            if not dataexplorer.check_ingest_users_tag():
+                dbgPrint.debug("Fetching all users info")      
+                all_users = self.msgraph.get_all_users()
+                dbgPrint.debug("Ingesting data")  
+                dataexplorer.ingest_users(data=all_users)
+                del all_users[:]
+
+            defender_agents = self.msgraph.get_defender_agents()
+            dataexplorer.ingest_defender_agents(path=defender_agents)
+
+            dbgPrint.debug("Ingesting data")
+            audit = dataexplorer.ingest_events(data=incidents)
+            dbgPrint.debug("Fetching audit logs of incidents")
+            audit_logs = self.sentinel.get_all_audit_logs(audit)
+            dbgPrint.debug("Ingesting data")
+            dataexplorer.ingest_audit_logs(data=audit_logs)
+            del audit_logs[:]
+            del incidents[:]
+            dbgPrint.debug("Sleeping for 3 mins")
+            time.sleep(3 * 60)
+
+
+
+
+
+
+#        user_list = []
+#        mfa_users_list = self.mfa.query_all_users(mfa_list=user_list, page=1)
+#        dataexplorer.ingest_mfastats(data=mfa_users_list)
+        
+
+
+
+        pass
+   
+    
+    def get_full_report_backend(self, incident, lookBackInDays=30, open_doc=False):
+        doc = WordDoc()
+        ip_list = []
+        hash_list = []
+        recipient = []
+        q = queue.Queue()
+        out = self.summary(incident)
+        doc.title(out["incidentName"])
+        doc.author(self.email)
+        doc.traverse(out)
+#       dbgPrint.info(incident["IncidentId"])
+        self.sentinel.get_associated_evidences(incident["IncidentId"], queue=q, lookBackInDays=lookBackInDays)   
+        all_data = self.sentinel.accumulate(q)
+        for a in all_data:
             doc.insertHR(doc.insert_paragraph())
-            doc.add_run("Additional Details")
-            doc.traverse([ipquery.check_endpoint(i) for i in ip_list])
-            doc.insertHR(doc.insert_paragraph())
-            doc.traverse([self.sentinel.get_file_info(i) for i in hash_list])
-            doc.insertHR(doc.insert_paragraph())
-            doc.traverse([self.user_summary(i) for i in recipient])
-            doc.insertHR(doc.insert_paragraph())
-            doc.traverse(self.sentinel.get_audit_history(args))
-            doc.save(self.output + "\\" + args + ".docx")
-            os.startfile(self.output + "\\" + args + ".docx")
+            ip_list = self.ip_summary(a, ip_list)
+            hash_list = self.file_summary(a, hash_list)
+            recipient = self.recipient_summary(a, recipient)
+
+            doc.traverse(a)
+
+        doc.insertHR(doc.insert_paragraph())
+        doc.add_run("Additional Details")
+        doc.traverse([{count: ipquery.check_endpoint(i)} for count, i in enumerate(ip_list) if i != ""])
+        doc.insertHR(doc.insert_paragraph())
+        doc.traverse([{count: self.sentinel.get_file_info(i)} for count, i in enumerate(hash_list) if i != ""])
+        doc.insertHR(doc.insert_paragraph())
+        doc.traverse([{count:self.user_summary(i)} for count, i in enumerate(recipient) if i != ""])
+        doc.insertHR(doc.insert_paragraph())
+        doc.traverse(self.sentinel.get_audit_history(incident["IncidentId"]))
+        doc.save(self.output + "\\" + str(incident["IncidentId"]) + ".docx")
+        if open_doc:
+            os.startfile(self.output + "\\" + str(incident["IncidentId"]) + ".docx")
+
+    def get_full_report(self, id=None, lookBackInDays=30, start_index=0, end_index=0):
+
+        all_data = {}
+        incidents = self.sentinel.get_incidents(incidentId=id, 
+                                                alertStatus=['New','InProgress', 'Resolved'] , 
+                                                severity=[256,128,64,32], 
+                                                pageIndex=1, 
+                                                lookBackInDays=lookBackInDays, 
+                                                pageSize=3000, 
+                                                sourceFilter=[16384, 1048576], titleFilter=["eDiscovery"])       #16384 == MCAS incidents 512 = eDiscovery
+
+        sorted_incidents = sorted(incidents, key=lambda x: x["IncidentId"], reverse=True)
+        if sorted_incidents:
+            start = sorted_incidents[0]["IncidentId"]
+            end = sorted_incidents[len(sorted_incidents)-1]["IncidentId"]
+        else:
+            dbgPrint.error("Out of range. You may change the lockBackInDays or the incident might be aggragated to other incidents.")
+            sys.exit(1)
+
+        if start_index: 
+            for count, i in enumerate(sorted_incidents, start=1):
+                if start_index >= int(i["IncidentId"]) >= end_index:
+                    dbgPrint.info(i["IncidentId"])
+                    self.get_full_report_backend(i, lookBackInDays)
+                elif int(i["IncidentId"]) < end_index:
+                    break
+        elif id != None:
+            for i in sorted_incidents:
+                dbgPrint.info(i["IncidentId"])
+                self.get_full_report_backend(i, lookBackInDays, open_doc=True)
 
         else:
-            all_data = {}
-            for count, i in enumerate(incidents, start=1):
-                doc = WordDoc()
-                ip_list = []
-                hash_list = []
-                recipient = []
-                q = queue.Queue()
-                out = self.summary(i)
-                doc.title(out["incidentTitle"])
-                doc.author(self.email)
-                doc.traverse(out)
-                self.sentinel.get_associated_evidences(i["IncidentId"], queue=q, lookBackInDays=lookBackInDays)   
+            for count, i in enumerate(sorted_incidents, start=1):
                 dbgPrint.info(i["IncidentId"])
-                all_data = self.sentinel.accumulate(q)
-                for a in all_data:
-                    doc.insertHR(doc.insert_paragraph())
-                    ip_list = self.ip_summary(a, ip_list)
-                    hash_list = self.file_summary(a, hash_list)
-                    recipient = self.recipient_summary(a, recipient)
-
-                    doc.traverse(a)
-
-                doc.insertHR(doc.insert_paragraph())
-                doc.add_run("Additional Details")
-                doc.traverse([ipquery.check_endpoint(i) for i in ip_list])
-                doc.insertHR(doc.insert_paragraph())
-                doc.traverse([self.sentinel.get_file_info(i) for i in hash_list])
-                doc.insertHR(doc.insert_paragraph())
-                doc.traverse([self.user_summary(i) for i in recipient])
-                doc.insertHR(doc.insert_paragraph())
-                doc.traverse(self.sentinel.get_audit_history(i["IncidentId"]))
-                doc.save(self.output + "\\" + str(i["IncidentId"]) + ".docx")
-            
-#                os.startfile(self.output + "\\output\\" + str(i["IncidentId"]) + ".docx")    
+                self.get_full_report_backend(i, lookBackInDays)
+
+
 
     def dispatcher(self):
         args = self.args
         path = os.path.dirname(os.path.realpath(__file__))
         if args.get("verbose"):
             val = int(args.get("verbose"))
 #            if  val == 1:
 #                dbgPrint.enable(__name__)
             if val == 2:
                 dbgPrint.enable("core.mssentinelapi")
             elif val == 3:
                 dbgPrint.enable("core.msgraphapi")
             elif val == 4:
-                dbgPrint.enable("helper.login")
+                dbgPrint.enable("core.multifactor")
             elif val == 5:
+                dbgPrint.enable("helper.login")
+            elif val == 6:
+                dbgPrint.enable("core.dataexplorer")
+            elif val == 7:
                 dbgPrint.enable(__name__)
                 dbgPrint.enable("core.mssentinelapi")
                 dbgPrint.enable("core.msgraphapi")
                 dbgPrint.enable("helper.login")
             else:
                 dbgPrint.error("Unknown value")
                 sys.exit()
         if args.get("clear"):
             pass
+        if args.get("resetmfa"):
+            self.mfa.reset_session(self.email)
         if args.get("user"):
             self.__init__(args)
             user_info = self.msgraph.check_mfa_status(args.get("user"))
 #            if user_info:
 #                printTable(user_info)
 #            user_info = self.msgraph.search_user(args.get("user"))
         elif args.get("incidentId"):
             self.__init__(args)
             start = time.time()
-            dbgPrint.info("Processing {value}", value=args.get("incidentId"))
-            self.get_full_report(args.get("incidentId"), lookBackInDays=args.get("daysgo", 30))
+#            dbgPrint.info("Processing {value}", value=args.get("incidentId"))
+            self.get_full_report(args.get("incidentId"), lookBackInDays=args.get("daysago") if args.get("daysago") else 30)
             end = time.time()
             dbgPrint.success("Job done (Elapsed time {value}).", value=end-start)
-        elif args.get("all"):
+#        elif args.get("all"):
+#            start = time.time()
+#            dbgPrint.info("Processing all incidents")
+#            self.get_full_report(lookBackInDays=args.get("daysago") if args.get("daysago") else 30)
+#            end = time.time()
+#            dbgPrint.success("Job done (Elapsed time {value}).", value=end-start)
+        elif args.get("range"):
             start = time.time()
-            dbgPrint.info("Processing all incidents")
-            self.get_full_report(lookBackInDays=args.get("daysago", 30))
+            dbgPrint.info("Processing Incidents with range")
+            start_index = args["range"][0]
+            end_index = 0
+            if len(args["range"]) > 1 and len(args["range"]) < 3:
+                end_index = args["range"][1]
+            if (start_index == end_index) or (start_index < end_index):
+                dbgPrint.error("The starting index must be higher than ending index")
+                sys.exit(1)
+            self.get_full_report(lookBackInDays=args.get("daysago") if args.get("daysago") else 30, start_index=start_index, end_index=end_index)
             end = time.time()
             dbgPrint.success("Job done (Elapsed time {value}).", value=end-start)
-            return
+        elif args.get("timely"):
+            if int(args["timely"]) >= 5:
+                self.get_timely_report(lookBackInDays=args.get("daysago") if args.get("daysago") else 30, duration= int(args["timely"]))
+        return
 
     #------------------------------------------------------
 
 def parse_argument():
 
     parser = argparse.ArgumentParser(
         prog = 'ChromeDriver',
         description  = 'This tool is used to retrieve all the necessary informaation of the incident',
         epilog = '',
         formatter_class=argparse.RawTextHelpFormatter
         )
 #    group = parser.add_mutually_exclusive_group(required=True)
 
-    parser.add_argument('-id', '--incidentId',help= "Select incident ID \n")
-    parser.add_argument('-a', '--all', help= "Process all incidents \n" , action='store_true')
+    parser.add_argument('-id', '--incidentId', nargs='+', type=int, help= "Select single or multiple IDs\n"
+                                                                          "Example: \n"
+                                                                          "-id 13572\n"
+                                                                          "-id 13572 13806\n")
+#    parser.add_argument('-a', '--all', help= "Process all incidents \n" , action='store_true')
     parser.add_argument('-v', '--verbose', help="Enable logging with specific level \n"
                                                 "1 : main \n"
                                                 "2 : sentinel \n"
                                                 "3 : msgraph \n"
-                                                "4 : login \n"
-                                                "5 : enable all")
+                                                "4 : multifactor \n"
+                                                "5 : login \n"
+                                                "6 : enable all")
 #    parser.add_argument('-r', '--reset', help="Reset the session and restart", action="store_true")
     parser.add_argument('-e', '--email', help="Set email address.")
 #    parser.add_argument('-u', '--user', help = "Fetch user info")
     parser.add_argument('-o', '--output', help = "Set output folder.")
 #    parser.add_argument('-c','--clear', help = "Clear cache", action="store_true")
     parser.add_argument('-d', '--daysago', help="Look back in days. Default=30")
+
+    parser.add_argument('-rm', '--resetmfa', help="Reset MFA Session", action='store_true')
  
     parser.add_argument('-c', '--companytags',help="CSV of company tags <Tag> <Company> <Country> to identify which country does a user belong.")
 
+    parser.add_argument('-r', '--range', nargs='+', type=int, help="Specify the range in a reverse order, \n"
+                                                                   "wherein the start is the higher limit and end is lower limit.\n"
+                                                                   "Lower limit is optional. If not provided, the default value will be zero.\n"
+                                                                   "Example: \n"
+                                                                   "-r 13700 13000")
+
+    parser.add_argument('-t', '--timely', nargs='?', default=5, help="Fetching and ingesting data to Azure Data Explorer and can be use to run with specific time duration, minimum of 5 mins")
+
     args = parser.parse_args()
 
-    if args.incidentId and args.all:
-        parser.error("Required only one between -id/--incidentId and -a/--all.")
+#    if args.incidentId and args.all:
+#        parser.error("Required only one between -id/--incidentId and -a/--all.")
 
     if len(sys.argv)==1:
         # display help message when no args are passed.
         parser.print_help()
         sys.exit(1)
 
     return args
```

### Comparing `nriapp-1.0.9/setup.py` & `nriapp-1.1.10/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 
 from setuptools import setup, find_packages
 from glob import glob
 
-with open('requirements.txt') as f:
-    requirements = f.read().splitlines()
+#with open('requirements.txt') as f:
+#    requirements = f.read().splitlines()
 
 
 setup(
    name='nriapp',
-   version='1.0.9',
+   version='1.1.10',
    description='This is an internal tool for crawling MS 365 Defender web with NRI',
+    license='MIT',
    author='Llallum Victoria',
    author_email='llallumvictoria@gmail.com',
-#   packages=find_packages('chrome'),
-   package_dir = {'':'setup'},
+#   packages=find_packages('src'),
+   package_dir = {'':'src/nriapp'},
     
-   packages=['.', 'config', 'core', 'helper'],  #same as name
+   packages=['.','config', 'core', 'helper'],  #same as name
 #   packages=find_packages(exclude=['ez_setup', 'tests', 'tests.*']),
-   data_files=[('', ['./setup/requirements.txt', './setup/changelog.txt']),
-               ('./session', glob('./setup/session/*.*')),
-               ('./logs', glob('./setup/logs/*.*')),
-               ('./output', glob('./setup/output/*.*'))
-
-               ],
+   data_files=[('.', ['src/nriapp/changelog.txt']),
+               ('./session', glob('./src/session/*.*')),
+               ('./logs', glob('./src/logs/*.*')),
+               ('./output', glob('./src/output/*.*'))
+              ],
    #setup_requires=['session', 'logs', 'output'],
-   include_package_data=True,  
-   install_requires=requirements, #external packages as dependencies,
+   include_package_data=True,
+   install_requires=[],
+#   install_requires=requirements, #external packages as dependencies,
    entry_points = '''
         [console_scripts]
         nriapp=nriapp:main
     '''
 
 )
```

