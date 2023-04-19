# Comparing `tmp/xiezuocat-2.1.1.tar.gz` & `tmp/xiezuocat-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiezuocat-2.1.1.tar", last modified: Thu Apr  6 10:23:14 2023, max compression
+gzip compressed data, was "xiezuocat-2.1.2.tar", last modified: Wed Apr 19 09:54:27 2023, max compression
```

## Comparing `xiezuocat-2.1.1.tar` & `xiezuocat-2.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 10:23:14.985916 xiezuocat-2.1.1/
--rw-rw-rw-   0        0        0      311 2023-04-06 10:23:14.984919 xiezuocat-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     7291 2023-04-06 10:18:29.000000 xiezuocat-2.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-06 10:23:14.986914 xiezuocat-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1568 2023-04-06 10:13:57.000000 xiezuocat-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 10:23:14.973946 xiezuocat-2.1.1/xiezuocat/
--rw-rw-rw-   0        0        0       32 2022-10-26 09:43:08.000000 xiezuocat-2.1.1/xiezuocat/__init__.py
--rw-rw-rw-   0        0        0     5855 2022-10-26 07:22:44.000000 xiezuocat-2.1.1/xiezuocat/sm3.py
--rw-rw-rw-   0        0        0      570 2023-04-04 08:03:09.000000 xiezuocat-2.1.1/xiezuocat/sm3_signature_util.py
--rw-rw-rw-   0        0        0     2397 2023-04-06 10:15:43.000000 xiezuocat-2.1.1/xiezuocat/xiezuocat.py
-drwxrwxrwx   0        0        0        0 2023-04-06 10:23:14.982924 xiezuocat-2.1.1/xiezuocat.egg-info/
--rw-rw-rw-   0        0        0      311 2023-04-06 10:23:14.000000 xiezuocat-2.1.1/xiezuocat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-04-06 10:23:14.000000 xiezuocat-2.1.1/xiezuocat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 10:23:14.000000 xiezuocat-2.1.1/xiezuocat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-06 10:23:14.000000 xiezuocat-2.1.1/xiezuocat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 09:54:27.535348 xiezuocat-2.1.2/
+-rw-rw-rw-   0        0        0      311 2023-04-19 09:54:27.535348 xiezuocat-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6786 2023-04-19 09:51:00.000000 xiezuocat-2.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 09:54:27.536347 xiezuocat-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1568 2023-04-19 09:51:08.000000 xiezuocat-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 09:54:27.517030 xiezuocat-2.1.2/xiezuocat/
+-rw-rw-rw-   0        0        0       32 2022-10-26 09:43:08.000000 xiezuocat-2.1.2/xiezuocat/__init__.py
+-rw-rw-rw-   0        0        0     5855 2022-10-26 07:22:44.000000 xiezuocat-2.1.2/xiezuocat/sm3.py
+-rw-rw-rw-   0        0        0      570 2023-04-04 08:03:09.000000 xiezuocat-2.1.2/xiezuocat/sm3_signature_util.py
+-rw-rw-rw-   0        0        0     2397 2023-04-06 10:15:43.000000 xiezuocat-2.1.2/xiezuocat/xiezuocat.py
+drwxrwxrwx   0        0        0        0 2023-04-19 09:54:27.532047 xiezuocat-2.1.2/xiezuocat.egg-info/
+-rw-rw-rw-   0        0        0      311 2023-04-19 09:54:27.000000 xiezuocat-2.1.2/xiezuocat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-04-19 09:54:27.000000 xiezuocat-2.1.2/xiezuocat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 09:54:27.000000 xiezuocat-2.1.2/xiezuocat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-19 09:54:27.000000 xiezuocat-2.1.2/xiezuocat.egg-info/top_level.txt
```

### Comparing `xiezuocat-2.1.1/README.md` & `xiezuocat-2.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,141 +1,133 @@
 # xiezuocat-python
-对智能纠错、智能改写、AI写作、单点登录签名算法进行封装
+对智能纠错、智能改写、AI写作、单点登录签名算法进行封装<br />
+关于具体接口的调用方法与参数说明，请访问[写作猫API文档中心](https://apidocs.xiezuocat.com/guide/)
 ## 一、pip引入
 ```python
 pip install xiezuocat
 ```
 
 ## 二、调用示例
 ### 1、智能纠错
 #### 调用示例
 ```python
 import xiezuocat
 import json
 my_xiezuocat = xiezuocat.Xiezuocat({your-secretKey})
 check_data = json.dumps({
             "texts": [
-                "哈哈哈。我天今吃了一顿饭",
-                "我想念十分赵忠祥。嘿嘿嘿。"
+                "河北省赵县的洨河上，有一座世界文明的石拱桥，叫安济桥，又叫赵州桥。",
+                "它是隋朝的石匠李春涉及和参加建造的，到现在已经有一千三百多年了。"
             ]
         })
 check_result = my_xiezuocat.check(check_data)
 print(check_result)
 ```
 #### 返回结果
 ```json
 {
   "errCode" : 0,
   "errMsg" : "",
   "data" : null,
   "alerts" : [ [ {
     "alertType" : 4,
-    "alertMessage" : "建议用“今天”替换“天今”。",
-    "sourceText" : "天今",
-    "replaceText" : "今天",
-    "start" : 5,
-    "end" : 6,
-    "errorType" : 3,
-    "advancedTip" : true
-  }, {
-    "alertType" : 2,
-    "alertMessage" : "根据段落，句子应已完结，句尾建议添加句号",
-    "sourceText" : "饭",
-    "replaceText" : "。",
-    "start" : 11,
-    "end" : 11,
-    "errorType" : 2,
+    "alertMessage" : "建议用“闻名”替换“文明”。",
+    "sourceText" : "文明",
+    "replaceText" : "闻名",
+    "start" : 15,
+    "end" : 16,
+    "errorType" : 1,
     "advancedTip" : false
   } ], [ {
     "alertType" : 4,
-    "alertMessage" : "建议用“十分想念”替换“想念十分”。",
-    "sourceText" : "想念十分",
-    "replaceText" : "十分想念",
-    "start" : 1,
-    "end" : 4,
-    "errorType" : 3,
+    "alertMessage" : "建议用“设计”替换“涉及”。“涉及”指关联到，牵涉到。“设计”指根据一定要求﹐对某项工作预先制定图样﹑方案。",
+    "sourceText" : "涉及",
+    "replaceText" : "设计",
+    "start" : 9,
+    "end" : 10,
+    "errorType" : 1,
     "advancedTip" : false
   } ] ],
   "checkLimitInfo" : {
-    "checkWordCountLeftToday" : "997268",
-    "totalCheckWordCountLeft" : "997268",
+    "checkWordCountLeftToday" : "996730",
+    "totalCheckWordCountLeft" : "996730",
     "expireDate" : "2024-02-02 00:00:00"
   }
 }
 ```
 ### 2、智能改写
 ##### 调用示例
 ```python
 import xiezuocat
 import json
 my_xiezuocat = xiezuocat.Xiezuocat({your-secretKey})
 rewrite_data = json.dumps({
   "items": [
-    "一般"
+    "河北省赵县的洨河上，有一座世界文明的石拱桥，叫安济桥，又叫赵州桥。它是隋朝的石匠李春涉及和参加建造的，到现在已经有一千三百多年了。"
   ],
   "level": "middle"
 })
 rewrite_result = my_xiezuocat.rewrite(rewrite_data)
 print(rewrite_result)
 ```
 ##### 返回结果
 ```json
 {
   "errcode" : 0,
   "errmsg" : null,
-  "items" : [ "普通" ],
-  "stat" : "997268"
+  "items" : [ "河北省赵县境内，有一座名为“安济桥”的“赵州桥”，是一座举世闻名的“世界文化遗产”。这座桥由李春参与修建，距今已有1300年之久。" ],
+  "stat" : "996730"
 }
 ```
 
 ### 3、AI写作
 #### 创建生成任务
 ##### 调用示例
 ```python
 import xiezuocat
 import json
 my_xiezuocat = xiezuocat.Xiezuocat({your-secretKey})
 generate_params = json.dumps({
     "type": "Step",
-    "title": "飞机",
+    "title": "仿生人会梦见电子羊吗",
     "length": "default"
 })
 result = my_xiezuocat.generate(generate_params)
 print(result)
 ```
 ##### 返回结果
 ```json
 {
   "errCode" : 0,
   "errMsg" : "success",
   "data" : {
-    "docId" : "ffa614ac-631f-4e7d-b0ea-b5ac43670e59"
+    "docId" : "36f72645-2bd3-43a3-85a3-0512e2d52cd3"
   }
 }
 ```
 
 #### 获取生成结果
 ##### 调用示例
 ```python
 import xiezuocat
 my_xiezuocat = xiezuocat.Xiezuocat({your-secretKey})
-doc_id = "ffa614ac-631f-4e7d-b0ea-b5ac43670e59" # 此处docId为第一步生成的结果
+doc_id = "36f72645-2bd3-43a3-85a3-0512e2d52cd3" # 此处docId为第一步生成的结果
 result = my_xiezuocat.get_generate_result(doc_id)
 print(result)
 ```
 ##### 返回结果
 ```json
 {
   "errCode" : 0,
   "errMsg" : "success",
   "data" : {
     "status" : "FINISHED",
-    "result" : "飞机\n飞机是一种用于军事、民用、工业及运输的飞行器。在20世纪，飞机被广泛应用于军事和民用领域，成为现代军事和民用工业中最主要的组成部分。它在现代社会有着非常重要的作用，是一个国家综合实力及经济实力的体现。它与航空、航天事业一起成为世界上具有最广泛影响力的三大航空产业之一。\n发展历史\n飞机的发展史，其实是人类不断探索和发展的历史。从最早的飞机，到二战期间以英国人发明的F-104 “闪电”战机为标志的喷气式战斗机，再到上世纪50年代以后，各国在飞机技术上取得的重大突破，几乎都是在二战期间才开始形成并发展起来的。从20世纪50年代末直到今天，世界航空科技研究在高速发展。以美国为例，20世纪50年代至60年代初仅进行了一系列重大试验就获得了大量专利。而70多年来世界航空科技研究才有了长足发展，但也正是这样的高速发展使一些发达国家逐渐在世界处于领先地位。而在目前世界上的几个主要航空大国中，美国已经拥有了多项技术专利和发明专利。\n飞机分类\n按用途分，有军用飞机、民用飞机和军用运输机。在民用飞机中，按动力系统的不同又可分为喷气客机、涡桨喷气客机及喷气式支线客机三大类，其中，喷气客机的主要特点是：机身短小、机动灵活、速度快而平稳；发动机耗油量低；在较短时间内能飞得较高。从用途分，可分为侦察型飞机、攻击型飞机和战略运输机。侦察型飞机是由侦察机改装而来的，一般用于攻击敌方地面或空中目标；攻击型战斗机是具有较强攻击力的战略战斗机，主要用于攻击敌方地面或空中目标；战略运输机是一种大型运输飞机，可以运送一定数量的人员和物资。\n飞机制造\n飞机制造是一项集科学、技术、艺术与工程于一体的高科技工业，它的研制必须有严格的质量管理体系来保证。飞机制造是指从产品设计、原材料采购、生产过程控制到成品装配检验等整个过程。其主要包括材料、工艺和结构三大类内容。材料是指各种飞机部件及其零件，如机身（结构）、机翼（机尾）、尾翼、起落架等；工艺是指制造零件及生产过程的工艺方法和手段；结构是指对飞机整体进行结构设计，根据其使用要求来布置各种设备和结构以及保证性能要求；结构必须能承受各种载荷，如机翼上重量（包括载荷所带来的机械应力）和其他载荷；它包括各种装配方法，装配质量也直接影响产品的可靠性和使用寿命。\n飞机发展现状\n飞机是由发动机的飞机，由于喷气发动机的推力大、效率高、噪音小；燃料多，燃料消耗少。飞机的外形和构造与汽车十分相似，可以在空中自由升降、滑行而不会受到地面阻力影响。因此是一个理想的交通工具。目前在全世界范围内，世界上主要用于军用的飞机有：F-16隐身战斗机（北约代号F35）、F-16猛禽战斗机（北约代号F35）、F-35联合攻击战斗机（KF-X）以及C-17 “大力神”运输机；民用领域的飞机有：客机（波音777/747等）、支线客机（空客A320等，波音737等）和特种飞机（如图2-1所示）。从各国的军用和民用航空史上看，世界上有相当一部分先进的军用装备，是在20世纪中期由军事大国发展起来的。\n",
-    "wordCount" : "1194",
-    "restCount" : "135608"
+    "result" : "仿生人会梦见电子羊吗\n仿生人，即为人工仿生系统，其本质上是利用计算机技术模拟人体生理机能，设计制造出一种与人类相似的人工生物，具有一定的智力、语言、动作等。其设计原理简单来讲就是通过模仿生物体自身的神经回路结构，模拟人工生物的大脑信号。在过去很长一段时间内，仿生人始终是科幻小说和影视作品中虚构出来的角色。随着科技进步不断发展，现实生活中也有了许多仿生人形象。比如：人类模仿机械动物造型、电子羊造型等等。今天我们就来聊聊这类仿生人形象的故事。\n一、人体仿生人\n随着科学技术的发展，仿生技术也在不断地创新，这其中最为典型的当属“人体仿生人”了。所谓的人体仿生人就是通过模仿人体形态特征、生理机能，设计制造出与真人一样的“机器人”。\n二、机械人\n机械人是利用计算机技术在人体上植入程序，进行人工模仿和设计。比如机器人手臂的关节都是有关节定位的，所以可以像人类手臂一样灵活地运动。这种仿生机器人最大的特点就是可以根据不同类型的动作进行相应的调节。目前机器人在军事领域应用最为广泛，比如：军事侦察、特种部队、无人机等等。\n三、电子羊\n电子羊，又名“仿生人”，是一种可以通过模拟生物行为而非机械结构来实现动作的计算机仿真机器人。电子羊具有很强的环境适应能力和自我保护能力，能够完成复杂任务，具备多种动作模式和智能控制机制。目前，国际上已有相关研究团队进行了研发，并应用于人类生活中。\n四、仿生人与智能机器人\n当前，我们可以通过人工仿生系统来实现机器人的多种功能，比如：帮助人类去完成某些任务、帮助机器人控制一些智能设备等。在这方面的应用已经取得了不少成果。比如：利用仿生人模型在机器人身上进行虚拟现实技术测试，为将来机器人开发提供新的思路，甚至还可以直接与仿生人对话。除此之外，还有一些应用在医疗方面，比如：利用仿生人模拟心脏功能来设计人工心脏，实现了人体自身对机械和物理机制的自我调节；利用仿生人设计出人造器官，可以帮助人类实现器官移植手术的顺利进行等等。未来随着科技进步和仿生人研究的深入，我们有望看到更多高智能、高水平的仿生人形象出现在我们眼中。\n",
+    "wordCount" : "852",
+    "restCount" : "90578"
   }
 }
 ```
 ### 4、单点登录签名算法
 ##### 调用示例
 ```python
 import xiezuocat
```

### Comparing `xiezuocat-2.1.1/setup.py` & `xiezuocat-2.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from setuptools import setup, find_packages
 setup(name='xiezuocat',
-version='2.1.1',
+version='2.1.2',
 description='写作猫API及签名算法封装',
 author='metasotadata',
 author_email='support@xiezuocat.com',
 py_modules=['xiezuocat.xiezuocat'],
 packages=find_packages(),
 requires=['requests', 'json', 'time', 'base64'],
 license="apache 3.0"
```

### Comparing `xiezuocat-2.1.1/xiezuocat/sm3.py` & `xiezuocat-2.1.2/xiezuocat/sm3.py`

 * *Files identical despite different names*

### Comparing `xiezuocat-2.1.1/xiezuocat/sm3_signature_util.py` & `xiezuocat-2.1.2/xiezuocat/sm3_signature_util.py`

 * *Files identical despite different names*

### Comparing `xiezuocat-2.1.1/xiezuocat/xiezuocat.py` & `xiezuocat-2.1.2/xiezuocat/xiezuocat.py`

 * *Files identical despite different names*

