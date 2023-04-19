# Comparing `tmp/sosin-1.0.0.tar.gz` & `tmp/sosin-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosin-1.0.0.tar", last modified: Mon Apr 17 12:09:32 2023, max compression
+gzip compressed data, was "sosin-1.0.1.tar", last modified: Wed Apr 19 14:56:48 2023, max compression
```

## Comparing `sosin-1.0.0.tar` & `sosin-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 12:09:32.822819 sosin-1.0.0/
--rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1268 2023-04-17 12:09:32.821819 sosin-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 12:09:32.822819 sosin-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      994 2023-04-17 12:09:21.000000 sosin-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:09:32.800917 sosin-1.0.0/sosin/
--rw-rw-rw-   0        0        0        0 2023-04-17 12:05:52.000000 sosin-1.0.0/sosin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:09:32.811468 sosin-1.0.0/sosin/databases/
--rw-rw-rw-   0        0        0     5081 2023-04-17 11:46:46.000000 sosin-1.0.0/sosin/databases/rdb.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:09:32.812471 sosin-1.0.0/sosin/rpa/
--rw-rw-rw-   0        0        0     8301 2023-04-17 11:46:46.000000 sosin-1.0.0/sosin/rpa/email_mgr.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:09:32.817499 sosin-1.0.0/sosin/utils/
--rw-rw-rw-   0        0        0     1687 2023-04-17 11:46:46.000000 sosin-1.0.0/sosin/utils/currency.py
--rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.0.0/sosin/utils/log.py
--rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.0.0/sosin/utils/progress.py
--rw-rw-rw-   0        0        0      385 2023-04-17 11:46:46.000000 sosin-1.0.0/sosin/utils/secret.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:09:32.820818 sosin-1.0.0/sosin/web/
--rw-rw-rw-   0        0        0     1055 2023-04-17 11:46:46.000000 sosin-1.0.0/sosin/web/content.py
--rw-rw-rw-   0        0        0     1018 2023-04-17 11:46:46.000000 sosin-1.0.0/sosin/web/translate.py
--rw-rw-rw-   0        0        0     4796 2023-04-17 11:46:46.000000 sosin-1.0.0/sosin/web/virtual.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:09:32.809452 sosin-1.0.0/sosin.egg-info/
--rw-rw-rw-   0        0        0     1268 2023-04-17 12:09:32.000000 sosin-1.0.0/sosin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2023-04-17 12:09:32.000000 sosin-1.0.0/sosin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 12:09:32.000000 sosin-1.0.0/sosin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-17 12:09:32.000000 sosin-1.0.0/sosin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-17 12:09:32.000000 sosin-1.0.0/sosin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 14:56:48.476827 sosin-1.0.1/
+-rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1268 2023-04-19 14:56:48.476827 sosin-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 14:56:48.476827 sosin-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      994 2023-04-19 14:56:38.000000 sosin-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:56:48.443100 sosin-1.0.1/sosin/
+-rw-rw-rw-   0        0        0        0 2023-04-17 12:05:52.000000 sosin-1.0.1/sosin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:56:48.465416 sosin-1.0.1/sosin/databases/
+-rw-rw-rw-   0        0        0     6203 2023-04-19 13:20:07.000000 sosin-1.0.1/sosin/databases/rdb.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:56:48.466416 sosin-1.0.1/sosin/rpa/
+-rw-rw-rw-   0        0        0     9951 2023-04-18 14:45:09.000000 sosin-1.0.1/sosin/rpa/email_mgr.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:56:48.471417 sosin-1.0.1/sosin/utils/
+-rw-rw-rw-   0        0        0     1687 2023-04-17 11:46:46.000000 sosin-1.0.1/sosin/utils/currency.py
+-rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.0.1/sosin/utils/log.py
+-rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.0.1/sosin/utils/progress.py
+-rw-rw-rw-   0        0        0      385 2023-04-17 11:46:46.000000 sosin-1.0.1/sosin/utils/secret.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:56:48.474463 sosin-1.0.1/sosin/web/
+-rw-rw-rw-   0        0        0     1055 2023-04-18 14:49:45.000000 sosin-1.0.1/sosin/web/content.py
+-rw-rw-rw-   0        0        0     1018 2023-04-17 11:46:46.000000 sosin-1.0.1/sosin/web/translate.py
+-rw-rw-rw-   0        0        0     4796 2023-04-17 11:46:46.000000 sosin-1.0.1/sosin/web/virtual.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:56:48.464414 sosin-1.0.1/sosin.egg-info/
+-rw-rw-rw-   0        0        0     1268 2023-04-19 14:56:48.000000 sosin-1.0.1/sosin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2023-04-19 14:56:48.000000 sosin-1.0.1/sosin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 14:56:48.000000 sosin-1.0.1/sosin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-19 14:56:48.000000 sosin-1.0.1/sosin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 14:56:48.000000 sosin-1.0.1/sosin.egg-info/top_level.txt
```

### Comparing `sosin-1.0.0/LICENSE` & `sosin-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sosin-1.0.0/PKG-INFO` & `sosin-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosin
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python utils for general works
 Home-page: https://github.com/devsosin/sosin
 Author: Jason Choi
 Author-email: svstar94@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sosin-1.0.0/README.md` & `sosin-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sosin-1.0.0/setup.py` & `sosin-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name                                = "sosin",
-    version                             = "1.0.0",
+    version                             = "1.0.1",
     license                             = 'MIT',
     author                              = "Jason Choi",
     author_email                        = "svstar94@gmail.com",
     description                         = "Python utils for general works",
     long_description                    = open('README.md').read(),
     url                                 = "https://github.com/devsosin/sosin",
     install_requires                    = ['requests', 'beautifulsoup4', 'PyMySQL',],
```

### Comparing `sosin-1.0.0/sosin/databases/rdb.py` & `sosin-1.0.1/sosin/databases/rdb.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,68 @@
 import pymysql
 import traceback
 
 class MariaDB:
 
     def __init__(self, db_config:dict, cursor_type="tuple") -> None:
-        '''
+        """
         생성자 메서드
         인스턴스 생성 시 db_config를 전달받아 DB에 연결합니다.
         
         **db_config**
             host=데이터베이스 서버 주소
             port=포트번호
             user=사용자 이름
             password=사용자 암호
             database=데이터베이스 이름
             charset=문자 인코딩
-        '''
+        """
 
         db_config['port'] = int(db_config.get('port', '3306'))
         self.DB = pymysql.connect(**db_config)
 
         if cursor_type == 'dict':
             self.cursor_type = pymysql.cursors.DictCursor
         else:
             self.cursor_type = None
             
         return
 
     def __del__(self):
-        '''
+        """
         인스턴스 소멸 시 DB 연결을 해제합니다.
-        '''
+        """
         self.DB.close()
         return
     
+    def get_tables(self) -> list:
+        """
+        get table names
+        """
+        with self.DB.cursor() as cursor:
+            sql_qr = """show tables;"""
+            cursor.execute(sql_qr)
+            result = cursor.fetchall()
+        return [t[0] for t in result]
+    
+    def get_table_columns(self, table:str) -> tuple:
+        """
+        get table column infos
+        """
+        with self.DB.cursor() as cursor:
+            sql_qr = """SELECT * FROM INFORMATION_SCHEMA.COLUMNS WHERE table_name=%s"""
+            cursor.execute(sql_qr, table)
+            return cursor.fetchall()
+    
     def custom_select(self, sql_qr:str, only_one=False) -> tuple:
         with self.DB.cursor() as cur:
             cur.execute(sql_qr)
             return cur.fetchone() if only_one else cur.fetchall()
 
-    def select(self, column_qry:str, table:str, limit=None, offset=None, order_by=None, where_condition=list[tuple]) -> tuple:
+    def select(self, column_qry:str, table:str, limit=None, offset=None, order_by=None, where_condition=[]) -> tuple:
         """
         Select
         예시) 
         column_qry = "*"
         column_qry = "id, name, email"
         table = "Students"
         """
@@ -106,16 +125,14 @@
                 cur.executemany(sql, values)
                 self.DB.commit()
             return True
         except:
             traceback.print_exc()
             return False
 
-
-
     def update(self, table:str, set_column:str, set_value, where_column:str, where_value) -> bool:
         """
         Update
         예시)
         table = "Students"
         set_column = "name"
         set_value = "jason"
@@ -145,14 +162,30 @@
         try:
             with self.DB.cursor() as cur:
                 cur.execute(sql)
                 self.DB.commit()
             return True
         except:
             return False
+    
+    def truncate(self, table:str, forcing=True) -> bool:
+        """
+        truncate table
+        """
+        try:
+            with self.DB.cursor() as cursor:
+                cursor.execute(f'SET FOREIGN_KEY_CHECKS = {int(forcing)};')
+                self.DB.commit()
+                
+            with self.DB.cursor() as cursor:
+                cursor.execute(f'TRUNCATE TABLE {table};')
+                self.DB.commit()
+                return True
+        except:
+            return False
 
     @staticmethod
     def make_columns(data: dict) -> str:
         """
         dictionary 객체에서 키를 칼럼 문자열로 변경
         """
         return ','.join(data.keys())
```

### Comparing `sosin-1.0.0/sosin/rpa/email_mgr.py` & `sosin-1.0.1/sosin/rpa/email_mgr.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,234 +11,263 @@
 
 from os.path import basename
 
 import time
 from datetime import datetime
 
 import traceback
+from typing import Union
 
-def is_ascii(s):
+def _is_ascii(s):
     '''
-    ASCII 체크 함수
+    ASCII 체크
     '''
     return all(ord(c) < 128 for c in s)
 
-def get_subject(subject):
+def _get_subject(subject):
     '''
-    메일의 제목 반환
+    메일 제목 반환
     '''
     s, encoding = decode_header(subject)[0]
     if encoding:
         return str(s, encoding, 'replace')
     else:
         return s
 
-def get_body(msg):
+def _get_body(msg):
     '''
     메일 내용 반환
     '''
     if msg.is_multipart():
-        return get_body(msg.get_payload(0))
+        return _get_body(msg.get_payload(0))
     else:
         return msg.get_payload(None, True)
+    
+class EmailManager:
+    """
+    Email Manager
+    """
+
+    def __init__(self, email_id, email_pw, mail_server:str='naver', mode='send') -> None:
+        """
+        mail_server: gmail, naver
+        mode: send, get
+        """
+        self.email_id = email_id
+        self.email_pw = email_pw
+        
+        if mode == 'send':
+            SMTP_SERVER = f'smtp.{mail_server.lower()}.com'
+            SMTP_PORT = 465
+            smtp = smtplib.SMTP_SSL(SMTP_SERVER, SMTP_PORT)
+            smtp.login(email_id, email_pw)
+            self.protocol = smtp
+        elif mode == 'get':
+            IMAP_SERVER = f"imap.{mail_server.lower().strip()}.com" 
+            IMAP_PORT = 993
+            imap = imaplib.IMAP4_SSL(IMAP_SERVER, IMAP_PORT)
+            imap.login(self.email_id, self.email_pw)
+            self.protocol = imap
+
+    def __del__(self) -> None:
+        self.protocol.close()
+        self.protocol.logout()
+
+    def get_email(self, header_subjects:list=[], header_since:str=None, header_from:str=None, 
+                  label:str=None, encode_type='utf-8', save_path:str=None, remove_email=True
+                    ) -> list[dict]:
+        """
+        메일 제목에 특정 문자열이 있거나 특정 발송인의 이메일 반환\n
+        **필수값**\n
+        header_str : 검색할 제목 (non-ascii) | header_from : 발송인\n
+        **선택값**\n
+        save_path : 첨부 파일 저장 경로 (지정하지 않을 시 첨부파일 저장되지 않음)\n
+        return list[dict]
+        [
+            {
+                'subject': subject,
+                'date': date
+                'content': mail_content,
+                'attaches': [path:str]
+            }
+        ]
+        """
 
-def get_email(email_id, email_pw, header_subjects:list=[], header_since:str=None,
-                header_from:str=None, label:str=None, mail_server:str='naver', 
-                encode_type='utf-8', save_path:str=None, remove_email=True
-                ) -> list[dict]:
-    '''
-    메일 제목에 특정 문자열이 있거나 특정 발송인의 이메일 반환
-    **필수값**
-    email_id, email_pw: 메일서버 계정정보
-    header_str : 검색할 제목 (non-ascii) | header_from : 발송인
-    **선택값**
-    mail_server : naver, gmail
-    save_path : 첨부 파일 저장 경로
-    return list[dict]
-    [
-        {
-            'subject': subject,
-            'date': date
-            'content': mail_content,
-            'attaches': [str]
-        }
-    ]
-    '''
-
-    # 메일 검색어 ASCII 체크
-    if header_subjects:
-        assert all([is_ascii(header_str) for header_str in header_subjects]), 'In ASCII 문자열만 입력해주세요 (영문, 기호)'
-    assert header_subjects or header_from or header_since or label, '메일 제목이나 발신인, 날짜, 라벨을 추가해주세요.'
-
-    IMAP_SERVER = f"imap.{mail_server.lower().strip()}.com" 
-    IMAP_PORT = 993
-
-    email_result = []
-
-    try:
-        imap = imaplib.IMAP4_SSL(IMAP_SERVER, IMAP_PORT)
-        imap.login(email_id, email_pw)
-        imap.select('inbox') if not label else imap.select(label)
-        search_list = []
+        # 메일 검색어 ASCII 체크
         if header_subjects:
-            if len(header_subjects) == 1:
-                search_list.append(f'(Header Subject "{header_subjects[0]}")')
-            else:
-                # 230315 업데이트
-                search_list.append('OR ' * (len(header_subjects)-1) + ' '.join([f'Subject "{hs}"' for hs in header_subjects]) if header_subjects else '')
-        
-        if header_from:
-            search_list.append(f'(from "{header_from}")' if header_from else '')
-            
-        if header_since:
-            search_list.append(f'(SINCE "{header_since}")')
+            assert all([_is_ascii(header_str) for header_str in header_subjects]), 'In ASCII 문자열만 입력해주세요 (영문, 기호)'
+        assert header_subjects or header_from or header_since or label, '메일 제목이나 발신인, 날짜, 라벨을 추가해주세요.'
 
-        if search_list:
-            _, data = imap.uid('search', None, *search_list)
-        else:
-            _, data = imap.uid('search', None, 'All')
-
-        for target_uid in data[0].split():
-            try:
-                _, data = imap.uid('fetch', target_uid, '(RFC822)')
-                try:
-                    email_message = email.message_from_string(data[0][1].decode(encode_type))
-                except:
-                    email_message = email.message_from_string(data[0][1].decode('cp949')) #euc-kr
+        email_result = []
 
-                # 메일 제목
-                subject = get_subject(email_message['subject'])
+        try:
+            self.protocol.select('inbox') if not label else self.protocol.select(label)
+            search_list = []
+            if header_subjects:
+                if len(header_subjects) == 1:
+                    search_list.append(f'(Header Subject "{header_subjects[0]}")')
+                else:
+                    # 230315 업데이트
+                    search_list.append('OR ' * (len(header_subjects)-1) + ' '.join([f'Subject "{hs}"' for hs in header_subjects]) if header_subjects else '')
+            
+            if header_from:
+                search_list.append(f'(from "{header_from}")' if header_from else '')
+                
+            if header_since:
+                search_list.append(f'(SINCE "{header_since}")')
+
+            if search_list:
+                _, data = self.protocol.uid('search', None, *search_list)
+            else:
+                _, data = self.protocol.uid('search', None, 'All')
 
-                # 메일 내용
+            for target_uid in data[0].split():
                 try:
-                    mail_content = get_body(email_message).decode(encode_type).strip()
-                except:
-                    # print(target_uid, subject)
-                    mail_content = get_body(email_message).decode('cp949').strip()
+                    _, data = self.protocol.uid('fetch', target_uid, '(RFC822)')
+                    try:
+                        email_message = email.message_from_string(data[0][1].decode(encode_type))
+                    except:
+                        email_message = email.message_from_string(data[0][1].decode('cp949')) #euc-kr
 
-                # 수신 일시
-                timestamp = (time.mktime(email.utils.parsedate(email_message['Date'])))
-                mail_time = datetime.fromtimestamp(timestamp)
-
-                # 첨부 파일
-                file_list = []
-                for part in email_message.walk():
-                    if part.get_content_maintype() == 'multipart':
-                        continue
-                    if part.get('Content-Disposition') is None:
-                        continue
+                    # 메일 제목
+                    subject = _get_subject(email_message['subject'])
 
+                    # 메일 내용
                     try:
-                        filename = part.get_filename()
-                        s, encoding = decode_header(filename)[0]
-                        if encoding:
-                            filename = str(s, encoding, 'replace')
-
-                        file_list.append({
-                            'name': filename,
-                            'file': part.get_payload(decode=True)
-                        })
+                        mail_content = _get_body(email_message).decode(encode_type).strip()
                     except:
-                        pass
+                        mail_content = _get_body(email_message).decode('cp949').strip()
+
+                    # 수신 일시
+                    timestamp = (time.mktime(email.utils.parsedate(email_message['Date'])))
+                    mail_time = datetime.fromtimestamp(timestamp)
+
+                    # 첨부 파일
+                    file_list = []
+                    for part in email_message.walk():
+                        if part.get_content_maintype() == 'multipart':
+                            continue
+                        if part.get('Content-Disposition') is None:
+                            continue
+
+                        try:
+                            filename = part.get_filename()
+                            s, encoding = decode_header(filename)[0]
+                            if encoding:
+                                filename = str(s, encoding, 'replace')
+
+                            file_list.append({
+                                'name': filename,
+                                'file': part.get_payload(decode=True)
+                            })
+                        except:
+                            pass
+
+                    saved_files = []
+
+                    # 첨부파일 저장여부
+                    if save_path:
+                        os.makedirs(save_path, exist_ok=True)
+                        for eval_file in file_list:
+                            att_path = os.path.join(save_path, eval_file['name'])
+                            saved_files.append(str(att_path))
+                            if not os.path.isfile(att_path):
+                                with open(att_path, 'wb') as fp:
+                                    fp.write(eval_file['file'])
+
+                    # 이메일 지우기(지울 메세지의 uid)
+                    if remove_email:
+                        self.protocol.uid('store', target_uid, '+FLAGS', '(\\Deleted)')
+                        # 메일함 정리하기
+                        self.protocol.expunge()
+
+                    email_result.append({
+                        'subject':subject,
+                        'date': mail_time,
+                        'content': mail_content,
+                        'attaches': saved_files,
+                    })
+                except:
+                    with open('./email_error', 'a') as f:
+                        f.write('에러 발생, ' + str(target_uid) + '\n')
+
+        except:
+            traceback.print_exc()
+            
+        return email_result
+    
+    
+    # 이메일 발송 함수
+    def send_email(self, from_user:str, to_users:list, 
+                   subject:str, contents:list[Union[tuple, str]],
+                   attachments:list=[], cc_targets=[]
+                   ) -> bool:
+        '''
+        메일을 발송하는 함수입니다.
+
+        **필수값**
+        from_user: 보내는 사람의 이메일 주소
+        to_users: 받는 사람의 이메일 주소들 (list)
+        subject: 메일 제목
+        content: 메일 내용
+
+        **선택**
+        attachments: 첨부 파일들 (파일경로 리스트)
+        cc_targets: 참조 이메일 주소들 (list)
+        '''
+
+        try:
+            msg = MIMEMultipart('alternative')
+
+            if attachments:
+                msg = MIMEMultipart('mixed')
+
+                for attachment in attachments:
+                    email_file = MIMEBase('application', 'octet-stream')
+
+                    with open(attachment, 'rb') as f:
+                        file_data = f.read()
+
+                    email_file.set_payload(file_data)
+                    encoders.encode_base64(email_file)
+
+                    file_name = basename(attachment)
+                    email_file.add_header('Content-Disposition', 'attachment',
+                        filename=file_name)
+
+                    msg.attach(email_file)
+
+            msg['From'] = from_user
+            msg['To'] = ','.join(set(to_users))
+            if cc_targets:
+                msg['CC'] = ','.join(cc_targets)
+            msg['Subject'] = subject
+
+            for content in contents:
+                # don't care content is str or tuple
+                msg.attach(MIMEText(content))
 
-                saved_files = []
+            self.protocol.sendmail(from_user, set(to_users+cc_targets), msg.as_string())
+            return True
 
-                # 첨부파일 저장여부
-                if save_path:
-                    os.makedirs(save_path, exist_ok=True)
-                    for eval_file in file_list:
-                        att_path = os.path.join(save_path, eval_file['name'])
-                        saved_files.append(str(att_path))
-                        if not os.path.isfile(att_path):
-                            with open(att_path, 'wb') as fp:
-                                fp.write(eval_file['file'])
-
-                # 이메일 지우기(지울 메세지의 uid)
-                if remove_email:
-                    imap.uid('store', target_uid, '+FLAGS', '(\\Deleted)')
-                    # 메일함 정리하기
-                    imap.expunge()
-
-                email_result.append({
-                    'subject':subject,
-                    'date': mail_time,
-                    'content': mail_content,
-                    'attaches': saved_files,
-                })
-            except:
-                with open('./email_error', 'a') as f:
-                    f.write('에러 발생, ' + str(target_uid) + '\n')
-
-    except Exception as e:
-        print(e)
-        traceback.print_exc()
-    finally:
-        imap.close()
-        imap.logout()
+        except Exception:
+            traceback.print_exc()
         
-    return email_result
+        return False
 
-# 이메일 발송 함수
-def send_email(email_id, email_pw, 
-                from_user:str, to_users:list, subject:str, content:str, # contents -> (content, 'html'), (content, 'plain')
-                mail_server:str='naver', attachments:list=[], cc_targets=[]
-                ) -> bool:
-    '''
-    메일을 발송하는 함수입니다.
-    **필수값**
-    email_id, email_pw: 메일서버 계정정보
-    from_user: 보내는 사람의 이메일 주소
-    to_users: 받는 사람의 이메일 주소들 (list)
-    subject: 메일 제목
-    content: 메일 내용
-    **선택**
-    mail_server: 메일 서버 (naver, gmail)
-    attachments: 첨부 파일들 (파일경로 리스트)
-    cc_targets: 참조 이메일 주소들 (list)
-    '''
-
-    SMTP_SERVER = f'smtp.{mail_server.lower()}.com'
-    SMTP_PORT = 465
-
-    try:
-        smtp = smtplib.SMTP_SSL(SMTP_SERVER, SMTP_PORT)
-        smtp.login(email_id, email_pw)
-
-        msg = MIMEMultipart('alternative')
-
-        if attachments:
-            msg = MIMEMultipart('mixed')
-
-            for attachment in attachments:
-                email_file = MIMEBase('application', 'octet-stream')
-
-                with open(attachment, 'rb') as f:
-                    file_data = f.read()
-
-                email_file.set_payload(file_data)
-                encoders.encode_base64(email_file)
-
-                file_name = basename(attachment)
-                email_file.add_header('Content-Disposition', 'attachment',
-                    filename=file_name)
-
-                msg.attach(email_file)
-
-        msg['From'] = from_user
-        msg['To'] = ','.join(set(to_users))
-        if cc_targets:
-            msg['CC'] = ','.join(cc_targets)
-        msg['Subject'] = subject
-
-        text = MIMEText(content)
-        msg.attach(text)
-
-        smtp.sendmail(from_user, set(to_users+cc_targets), msg.as_string())
-        print('이메일 발송 성공 !')
-        return True
-
-    except Exception as e:
-        print(e)
-    finally:
-        smtp.close()
+if __name__ == '__main__':
+    config = {
+        'EMAIL_ID': 'your-email-id',
+        'EMAIL_PW': 'your-email-pw',
+    }
+    emgr = EmailManager(config.get('EMAIL_ID'), config.get('EMAIL_PW'), mail_server='gmail')
+    emgr.send_email(config['EMAIL_ID'], ['target-user-email'], 'this is test email !', 
+                    [('this is test content', 'plain'), 'this is just text', ('<div style="color:red;">this is html</div>', 'html')])
     
-    return False
+    # date_now = datetime(2022, 3, 7).strftime("%d-%b-%Y")
+    result = emgr.get_email(
+        # header_subjects=['test', 'store'],
+        # header_from='svstar94@gmail.com',
+        # header_since=date_now,
+        label='report',
+        remove_email=False, 
+    )
```

### Comparing `sosin-1.0.0/sosin/utils/currency.py` & `sosin-1.0.1/sosin/utils/currency.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.0/sosin/utils/progress.py` & `sosin-1.0.1/sosin/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.0/sosin/web/content.py` & `sosin-1.0.1/sosin/web/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,12 +26,12 @@
     def get_content_type(self):
         return self.r.headers['content-type']
     
     def get_body(self):
         return self.r.content
 
 if __name__ == '__main__':
-    wfm = WebContentManager('https://media.classicmanager.com/album/aac/MM014-2/01.m4a')
+    wcm = WebContentManager('https://media.classicmanager.com/album/aac/MM014-2/01.m4a')
 
-    wfm.download('./music.m4a')
+    wcm.download('./music.m4a')
 
-    wfm.get_content_type()
+    wcm.get_content_type()
```

### Comparing `sosin-1.0.0/sosin/web/translate.py` & `sosin-1.0.1/sosin/web/translate.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.0/sosin/web/virtual.py` & `sosin-1.0.1/sosin/web/virtual.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.0/sosin.egg-info/PKG-INFO` & `sosin-1.0.1/sosin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosin
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python utils for general works
 Home-page: https://github.com/devsosin/sosin
 Author: Jason Choi
 Author-email: svstar94@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

