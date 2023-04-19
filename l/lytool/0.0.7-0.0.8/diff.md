# Comparing `tmp/lytool-0.0.7.tar.gz` & `tmp/lytool-0.0.8.tar.gz`

## Comparing `lytool-0.0.7.tar` & `lytool-0.0.8.tar`

### file list

```diff
@@ -1,87 +1,97 @@
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/QRcode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/__init__.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/analysis_html_by_xpath_re.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/chaojiying.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/createFile.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/df_to_list_dict.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/down_img_url.txt
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/fileOperation.py
--rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/get_selenium_cookies_dict.py
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/headers.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/imageToWord.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/imageTool.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/init_self_headers.py
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/json_nested.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/mobilePhon.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myClient.py
--rw-r--r--   0        0        0    29679 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myEcharts.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myExecjs.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myJieBa.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myLog.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myMD5.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myMakDir.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myPickle.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myPlot.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myRandomUserAgent.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myRequests.py
--rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myServer.py
--rw-r--r--   0        0        0    15031 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/mySpider.py
--rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/mySql.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myTTS.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myTime.py
--rw-r--r--   0        0        0    18252 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myTkinter.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myToken.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/my_qr_code.py
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/operating_mongodb.py
--rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/operating_mysql.py
--rw-r--r--   0        0        0    14248 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/operating_redis.py
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/regularExpression.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/rgb_ras_stack.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/runJs.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/runNum.py
--rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/rwfile.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/sendEmail.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/speechRecognition.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/timer.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/xiciCrawler.py
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/yundama.py
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/快速将chrom复制的headers转变成字典.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/重命名.py
--rw-r--r--   0        0        0     9501 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/.idea/workspace.xml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/AdslProxy-master/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/AdslProxy-master/LICENSE
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/AdslProxy-master/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/AdslProxy-master/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/AdslProxy-master/api.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/AdslProxy-master/run.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/AdslProxy-master/setup.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/AdslProxy-master/adslproxy/__init__.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/AdslProxy-master/adslproxy/api.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/AdslProxy-master/adslproxy/config.py
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/AdslProxy-master/adslproxy/db.py
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/AdslProxy-master/adslproxy/sender.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/AdslProxy-master/test/__init__.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/AdslProxy-master/test/proxy.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myBaZhuaYu/main.py
--rw-r--r--   0        0        0    13778 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myBaZhuaYu/samples.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myBaZhuaYu/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myProcess/__init__.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/myProcess/myProcesse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/mySelenium/__init__.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/mySelenium/cookies.txt
--rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/mySelenium/jd_selenium.py
--rw-r--r--   0        0        0    19800 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/mySelenium/other_selenium.py
--rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/mySelenium/stealth.min.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/proxyADSL/__init__.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/proxyADSL/proxyADSL.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/proxyADSL/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/proxyZset/__init__.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/proxyZset/apiProxy.py
--rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/proxyZset/getProxy.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/proxyZset/save_Get_UA_Proxy.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/proxyZset/scheduler_UA_PROXY.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 lytool-0.0.7/src/lytool/proxyZset/testProxy.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lytool-0.0.7/LICENSE
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 lytool-0.0.7/README.md
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 lytool-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 lytool-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 lytool-0.0.8/src/chat.png
+-rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 lytool-0.0.8/src/chats.png
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 lytool-0.0.8/src/concept.png
+-rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 lytool-0.0.8/src/concepts.png
+-rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 lytool-0.0.8/src/findObject.png
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 lytool-0.0.8/src/findObjects.png
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 lytool-0.0.8/src/my.png
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 lytool-0.0.8/src/mys.png
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/QRcode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/__init__.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/analysis_html_by_xpath_re.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/chaojiying.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/createFile.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/df_to_list_dict.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/down_img_url.txt
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/fileOperation.py
+-rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/get_selenium_cookies_dict.py
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/headers.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/imageToWord.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/imageTool.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/init_self_headers.py
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/json_nested.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/mobilePhon.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myClient.py
+-rw-r--r--   0        0        0    29679 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myEcharts.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myExecjs.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myJieBa.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myLog.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myMD5.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myMakDir.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myPickle.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myPlot.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myRandomUserAgent.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myRequests.py
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myServer.py
+-rw-r--r--   0        0        0    15031 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/mySpider.py
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/mySql.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myTTS.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myTime.py
+-rw-r--r--   0        0        0    18252 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myTkinter.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myToken.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/my_qr_code.py
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/operating_mongodb.py
+-rw-r--r--   0        0        0    10731 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/operating_mysql.py
+-rw-r--r--   0        0        0    14248 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/operating_redis.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/regularExpression.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/rgb_ras_stack.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/runJs.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/runNum.py
+-rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/rwfile.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/sendEmail.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/speechRecognition.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/timer.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/xiciCrawler.py
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/yundama.py
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/快速将chrom复制的headers转变成字典.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/重命名.py
+-rw-r--r--   0        0        0     9731 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/.idea/workspace.xml
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/AdslProxy-master/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/AdslProxy-master/LICENSE
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/AdslProxy-master/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/AdslProxy-master/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/AdslProxy-master/api.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/AdslProxy-master/run.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/AdslProxy-master/setup.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/AdslProxy-master/adslproxy/__init__.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/AdslProxy-master/adslproxy/api.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/AdslProxy-master/adslproxy/config.py
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/AdslProxy-master/adslproxy/db.py
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/AdslProxy-master/adslproxy/sender.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/AdslProxy-master/test/__init__.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/AdslProxy-master/test/proxy.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myBaZhuaYu/main.py
+-rw-r--r--   0        0        0    13778 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myBaZhuaYu/samples.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myBaZhuaYu/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myProcess/__init__.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/myProcess/myProcesse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/mySelenium/__init__.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/mySelenium/cookies.txt
+-rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/mySelenium/jd_selenium.py
+-rw-r--r--   0        0        0    19800 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/mySelenium/other_selenium.py
+-rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/mySelenium/stealth.min.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/proxyADSL/__init__.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/proxyADSL/proxyADSL.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/proxyADSL/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/proxyZset/__init__.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/proxyZset/apiProxy.py
+-rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/proxyZset/getProxy.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/proxyZset/save_Get_UA_Proxy.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/proxyZset/scheduler_UA_PROXY.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 lytool-0.0.8/src/lytool/proxyZset/testProxy.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lytool-0.0.8/LICENSE
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 lytool-0.0.8/README.md
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 lytool-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 lytool-0.0.8/PKG-INFO
```

### Comparing `lytool-0.0.7/src/lytool/QRcode.py` & `lytool-0.0.8/src/lytool/QRcode.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/analysis_html_by_xpath_re.py` & `lytool-0.0.8/src/lytool/analysis_html_by_xpath_re.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/chaojiying.py` & `lytool-0.0.8/src/lytool/chaojiying.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/fileOperation.py` & `lytool-0.0.8/src/lytool/fileOperation.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/get_selenium_cookies_dict.py` & `lytool-0.0.8/src/lytool/get_selenium_cookies_dict.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/headers.py` & `lytool-0.0.8/src/lytool/headers.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/imageToWord.py` & `lytool-0.0.8/src/lytool/imageToWord.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/imageTool.py` & `lytool-0.0.8/src/lytool/imageTool.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/json_nested.py` & `lytool-0.0.8/src/lytool/json_nested.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/mobilePhon.py` & `lytool-0.0.8/src/lytool/mobilePhon.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/myClient.py` & `lytool-0.0.8/src/lytool/myClient.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/myEcharts.py` & `lytool-0.0.8/src/lytool/myEcharts.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/myRandomUserAgent.py` & `lytool-0.0.8/src/lytool/myRandomUserAgent.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/myRequests.py` & `lytool-0.0.8/src/lytool/myRequests.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/myServer.py` & `lytool-0.0.8/src/lytool/myServer.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/mySpider.py` & `lytool-0.0.8/src/lytool/mySpider.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/mySql.py` & `lytool-0.0.8/src/lytool/mySql.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/myTime.py` & `lytool-0.0.8/src/lytool/myTime.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/myTkinter.py` & `lytool-0.0.8/src/lytool/myTkinter.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/myToken.py` & `lytool-0.0.8/src/lytool/myToken.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/my_qr_code.py` & `lytool-0.0.8/src/lytool/my_qr_code.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/operating_mongodb.py` & `lytool-0.0.8/src/lytool/operating_mongodb.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/operating_mysql.py` & `lytool-0.0.8/src/lytool/operating_mysql.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,14 +76,24 @@
         :param fieldName: 要查询的字段名
         :param tableName: 要在哪个表里查
         :return: ['1','2']  # [value1, value2]
         '''
         df = self.getDf(f'''select {fieldName} from {tableName} where {where}''')
         return [i[fieldName] for i in list(json.loads(df.to_json(orient='index')).values())]
 
+    def getTextWhere(self, fieldName, tableName, where):
+        '''
+        获取1行数据，并转为列表
+        :param fieldName: 要查询的字段名
+        :param tableName: 要在哪个表里查
+        :return: '1'
+        '''
+        df = self.getDf(f'''select {fieldName} from {tableName} where {where}''')
+        return [i[fieldName] for i in list(json.loads(df.to_json(orient='index')).values())][0]
+
     def getSum(self, fieldName, tableName, where):
         '''
         获取多行数据，并转为列表
         :param fieldName: str,要查询的字段名
         :param tableName: str,要在哪个表里查
         :param where: str,条件
         :return: float or in  # 1.0+1.0
```

### Comparing `lytool-0.0.7/src/lytool/operating_redis.py` & `lytool-0.0.8/src/lytool/operating_redis.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/regularExpression.py` & `lytool-0.0.8/src/lytool/regularExpression.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/rgb_ras_stack.py` & `lytool-0.0.8/src/lytool/rgb_ras_stack.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/runJs.py` & `lytool-0.0.8/src/lytool/runJs.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/runNum.py` & `lytool-0.0.8/src/lytool/runNum.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/rwfile.py` & `lytool-0.0.8/src/lytool/rwfile.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/sendEmail.py` & `lytool-0.0.8/src/lytool/sendEmail.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/xiciCrawler.py` & `lytool-0.0.8/src/lytool/xiciCrawler.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/yundama.py` & `lytool-0.0.8/src/lytool/yundama.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/快速将chrom复制的headers转变成字典.py` & `lytool-0.0.8/src/lytool/快速将chrom复制的headers转变成字典.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/.idea/workspace.xml` & `lytool-0.0.8/src/lytool/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `lytool-0.0.7/src/lytool/.idea/workspace.xml` & `lytool-0.0.8/src/lytool/.idea/workspace.xml`

```diff
@@ -152,14 +152,18 @@
       <workItem from="1670806578849" duration="73000"/>
       <workItem from="1670855096201" duration="729000"/>
       <workItem from="1671602791733" duration="600000"/>
       <workItem from="1671618351871" duration="587000"/>
       <workItem from="1671664872579" duration="596000"/>
       <workItem from="1671787148235" duration="1250000"/>
       <workItem from="1673860936613" duration="602000"/>
+      <workItem from="1674177921280" duration="103000"/>
+      <workItem from="1674178031880" duration="34000"/>
+      <workItem from="1675906235460" duration="166000"/>
+      <workItem from="1676714122228" duration="10000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
```

### Comparing `lytool-0.0.7/src/lytool/AdslProxy-master/LICENSE` & `lytool-0.0.8/src/lytool/AdslProxy-master/LICENSE`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/AdslProxy-master/README.md` & `lytool-0.0.8/src/lytool/AdslProxy-master/README.md`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/AdslProxy-master/setup.py` & `lytool-0.0.8/src/lytool/AdslProxy-master/setup.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/AdslProxy-master/adslproxy/api.py` & `lytool-0.0.8/src/lytool/AdslProxy-master/adslproxy/api.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/AdslProxy-master/adslproxy/config.py` & `lytool-0.0.8/src/lytool/AdslProxy-master/adslproxy/config.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/AdslProxy-master/adslproxy/db.py` & `lytool-0.0.8/src/lytool/AdslProxy-master/adslproxy/db.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/AdslProxy-master/adslproxy/sender.py` & `lytool-0.0.8/src/lytool/AdslProxy-master/adslproxy/sender.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/myBaZhuaYu/main.py` & `lytool-0.0.8/src/lytool/myBaZhuaYu/main.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/myBaZhuaYu/samples.py` & `lytool-0.0.8/src/lytool/myBaZhuaYu/samples.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/myBaZhuaYu/util.py` & `lytool-0.0.8/src/lytool/myBaZhuaYu/util.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/myProcess/myProcesse.py` & `lytool-0.0.8/src/lytool/myProcess/myProcesse.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/mySelenium/jd_selenium.py` & `lytool-0.0.8/src/lytool/mySelenium/jd_selenium.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/mySelenium/other_selenium.py` & `lytool-0.0.8/src/lytool/mySelenium/other_selenium.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/mySelenium/stealth.min.js` & `lytool-0.0.8/src/lytool/mySelenium/stealth.min.js`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/proxyADSL/proxyADSL.py` & `lytool-0.0.8/src/lytool/proxyADSL/proxyADSL.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/proxyZset/apiProxy.py` & `lytool-0.0.8/src/lytool/proxyZset/apiProxy.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/proxyZset/getProxy.py` & `lytool-0.0.8/src/lytool/proxyZset/getProxy.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/proxyZset/save_Get_UA_Proxy.py` & `lytool-0.0.8/src/lytool/proxyZset/save_Get_UA_Proxy.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/proxyZset/scheduler_UA_PROXY.py` & `lytool-0.0.8/src/lytool/proxyZset/scheduler_UA_PROXY.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/src/lytool/proxyZset/testProxy.py` & `lytool-0.0.8/src/lytool/proxyZset/testProxy.py`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/LICENSE` & `lytool-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lytool-0.0.7/pyproject.toml` & `lytool-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lytool"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="longliangyu112233", email="2476673550@qq.com" },
 ]
 description = "CommonTools"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `lytool-0.0.7/PKG-INFO` & `lytool-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytool
-Version: 0.0.7
+Version: 0.0.8
 Summary: CommonTools
 Project-URL: Homepage, https://github.com/18086829907/lytool
 Author-email: longliangyu112233 <2476673550@qq.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

