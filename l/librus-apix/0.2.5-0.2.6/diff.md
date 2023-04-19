# Comparing `tmp/librus_apix-0.2.5.tar.gz` & `tmp/librus_apix-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-0.2.5.tar", last modified: Mon Apr 17 21:11:32 2023, max compression
+gzip compressed data, was "librus_apix-0.2.6.tar", last modified: Wed Apr 19 20:21:06 2023, max compression
```

## Comparing `librus_apix-0.2.5.tar` & `librus_apix-0.2.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-17 21:11:32.350315 librus_apix-0.2.5/
--rw-r--r--   0 poro      (1000) poro      (1000)     1722 2023-04-17 20:43:54.000000 librus_apix-0.2.5/LICENSE
--rw-r--r--   0 poro      (1000) poro      (1000)     1722 2023-04-17 20:43:54.000000 librus_apix-0.2.5/LICENSE.orig
--rw-r--r--   0 poro      (1000) poro      (1000)      470 2023-04-17 21:11:32.350315 librus_apix-0.2.5/PKG-INFO
--rw-r--r--   0 poro      (1000) poro      (1000)     2427 2023-04-17 21:01:31.000000 librus_apix-0.2.5/README.md
-drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-17 21:11:32.350315 librus_apix-0.2.5/librus_apix/
--rw-r--r--   0 poro      (1000) poro      (1000)      346 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/__init__.py
--rw-r--r--   0 poro      (1000) poro      (1000)     1156 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/announcements.py
--rw-r--r--   0 poro      (1000) poro      (1000)     3038 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/attendance.py
--rw-r--r--   0 poro      (1000) poro      (1000)      210 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/exceptions.py
--rw-r--r--   0 poro      (1000) poro      (1000)     2367 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/get_token.py
--rw-r--r--   0 poro      (1000) poro      (1000)     4680 2023-04-17 20:49:54.000000 librus_apix-0.2.5/librus_apix/grades.py
--rw-r--r--   0 poro      (1000) poro      (1000)      287 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/helpers.py
--rw-r--r--   0 poro      (1000) poro      (1000)     2175 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/homework.py
--rw-r--r--   0 poro      (1000) poro      (1000)     2108 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/messages.py
--rw-r--r--   0 poro      (1000) poro      (1000)     3053 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/schedule.py
--rw-r--r--   0 poro      (1000) poro      (1000)     3098 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/timetable.py
--rw-r--r--   0 poro      (1000) poro      (1000)      422 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/urls.py
-drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-17 21:11:32.350315 librus_apix-0.2.5/librus_apix.egg-info/
--rw-r--r--   0 poro      (1000) poro      (1000)      470 2023-04-17 21:11:32.000000 librus_apix-0.2.5/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 poro      (1000) poro      (1000)      530 2023-04-17 21:11:32.000000 librus_apix-0.2.5/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 poro      (1000) poro      (1000)        1 2023-04-17 21:11:32.000000 librus_apix-0.2.5/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 poro      (1000) poro      (1000)       18 2023-04-17 21:11:32.000000 librus_apix-0.2.5/librus_apix.egg-info/requires.txt
--rw-r--r--   0 poro      (1000) poro      (1000)       12 2023-04-17 21:11:32.000000 librus_apix-0.2.5/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 poro      (1000) poro      (1000)       89 2023-04-17 20:43:54.000000 librus_apix-0.2.5/pyproject.toml
--rw-r--r--   0 poro      (1000) poro      (1000)      589 2023-04-17 21:11:32.353649 librus_apix-0.2.5/setup.cfg
--rw-r--r--   0 poro      (1000) poro      (1000)       37 2023-04-17 20:43:54.000000 librus_apix-0.2.5/setup.py
+drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-19 20:21:06.407740 librus_apix-0.2.6/
+-rw-r--r--   0 poro      (1000) poro      (1000)     1722 2022-09-08 20:51:34.000000 librus_apix-0.2.6/LICENSE
+-rw-r--r--   0 poro      (1000) poro      (1000)     1722 2022-09-08 20:51:34.000000 librus_apix-0.2.6/LICENSE.orig
+-rw-r--r--   0 poro      (1000) poro      (1000)      470 2023-04-19 20:21:06.407740 librus_apix-0.2.6/PKG-INFO
+-rw-r--r--   0 poro      (1000) poro      (1000)     2430 2023-04-19 11:50:28.000000 librus_apix-0.2.6/README.md
+drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-19 20:21:06.404405 librus_apix-0.2.6/librus_apix/
+-rw-r--r--   0 poro      (1000) poro      (1000)      346 2022-09-08 20:51:34.000000 librus_apix-0.2.6/librus_apix/__init__.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     1156 2022-09-08 20:51:34.000000 librus_apix-0.2.6/librus_apix/announcements.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     2277 2023-04-19 19:19:28.000000 librus_apix-0.2.6/librus_apix/attendance.py
+-rw-r--r--   0 poro      (1000) poro      (1000)      210 2022-09-08 20:51:34.000000 librus_apix-0.2.6/librus_apix/exceptions.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     2367 2022-09-08 20:51:34.000000 librus_apix-0.2.6/librus_apix/get_token.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     4693 2023-04-19 14:24:01.000000 librus_apix-0.2.6/librus_apix/grades.py
+-rw-r--r--   0 poro      (1000) poro      (1000)      287 2022-12-30 11:55:28.000000 librus_apix-0.2.6/librus_apix/helpers.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     2175 2023-04-19 12:13:37.000000 librus_apix-0.2.6/librus_apix/homework.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     2108 2023-01-12 19:56:33.000000 librus_apix-0.2.6/librus_apix/messages.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     3053 2023-04-19 11:50:10.000000 librus_apix-0.2.6/librus_apix/schedule.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     3098 2022-12-14 21:45:32.000000 librus_apix-0.2.6/librus_apix/timetable.py
+-rw-r--r--   0 poro      (1000) poro      (1000)      422 2022-09-08 20:51:34.000000 librus_apix-0.2.6/librus_apix/urls.py
+drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-19 20:21:06.407740 librus_apix-0.2.6/librus_apix.egg-info/
+-rw-r--r--   0 poro      (1000) poro      (1000)      470 2023-04-19 20:21:06.000000 librus_apix-0.2.6/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 poro      (1000) poro      (1000)      530 2023-04-19 20:21:06.000000 librus_apix-0.2.6/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 poro      (1000) poro      (1000)        1 2023-04-19 20:21:06.000000 librus_apix-0.2.6/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 poro      (1000) poro      (1000)       18 2023-04-19 20:21:06.000000 librus_apix-0.2.6/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 poro      (1000) poro      (1000)       12 2023-04-19 20:21:06.000000 librus_apix-0.2.6/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 poro      (1000) poro      (1000)       89 2022-09-08 20:51:34.000000 librus_apix-0.2.6/pyproject.toml
+-rw-r--r--   0 poro      (1000) poro      (1000)      589 2023-04-19 20:21:06.407740 librus_apix-0.2.6/setup.cfg
+-rw-r--r--   0 poro      (1000) poro      (1000)       37 2022-09-08 20:51:34.000000 librus_apix-0.2.6/setup.py
```

### Comparing `librus_apix-0.2.5/LICENSE` & `librus_apix-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.5/LICENSE.orig` & `librus_apix-0.2.6/LICENSE.orig`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.5/README.md` & `librus_apix-0.2.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -98,16 +98,16 @@
 
 ```py
 from datetime import datetime
 from librus_apix.timetable import get_timetable
 
 monday_date = '2023-04-3'
 monday_datetime = datetime.strptime(monday_date, '%Y-%m-%d')
-t_table = get_timetable(token, monday_datetime)
-for weekday in timetable
+timetable = get_timetable(token, monday_datetime)
+for weekday in timetable:
   for period in timetable[weekday]:
     print(period.subject, period.teacher_and_classroom)
 
 ```
 
 ## Working on the Project
```

### Comparing `librus_apix-0.2.5/librus_apix/announcements.py` & `librus_apix-0.2.6/librus_apix/announcements.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.5/librus_apix/attendance.py` & `librus_apix-0.2.6/librus_apix/attendance.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,39 +8,16 @@
 from dataclasses import dataclass
 
 
 @dataclass
 class Attendance:
     symbol: str
     href: str
-    _type: str
-    date: str
-    lesson: str
-    subject: str
-    teacher: str
-    hour: str
-    excursion: str
-    by: str
     semester: int
-
-
-def get_detail(token: Token, detail_url: str) -> dict[str, str]:
-    details = {}
-    div = no_access_check(
-        BeautifulSoup(token.get(ATTENDANCE_URL + detail_url).text, "lxml")
-    ).find("div", attrs={"class": "container-background"})
-    line = div.find_all("tr", attrs={"class": ["line0", "line1"]})
-    if len(line) < 1:
-        raise ParseError("Error in parsing attendance.")
-    for l in line:
-        if not l.find("th"):
-            continue
-        details[l.find("th").text] = l.find("td").text
-    return details
-
+    attributes: dict
 
 def get_attendance(token: Token, sort_by: dict[str, str] = {'zmiany_logowanie_wszystkie': ''}) -> list[list[Attendance]]:
     soup = no_access_check(
             BeautifulSoup(token.post(BASE_URL + "/przegladaj_nb/uczen", data=sort_by).text, "lxml")
     )
     table = soup.find("table", attrs={"class": "center big decorated"})
     if table is None:
@@ -56,37 +33,31 @@
         date = day.find("td", attrs={"class": None})
         attendance = day.find_all("td", attrs={"class": "center"})
         for attend in attendance:
             at = attend.find_all("a")
             for single in at:
                 if not single:
                     continue
-                _type, date, lesson, subject, teacher, hour, excursion, by = (
+                attributes = { i.split(": ")[0].strip():
                     i.split(": ")[1].strip()
                     for i in single.attrs["title"]
                     .replace("</b>", "<br>")
                     .replace("<br/>", "")
                     .strip()
                     .split("<br>")
-                )
+                    }
+                #_type, date, lesson, subject, teacher, hour, excursion, by = attributes.values()
                 href = (
                     single.attrs["onclick"]
                     .replace("otworz_w_nowym_oknie(", "")
                     .split(",")[0]
                     .replace("'", "")
                     .split("/")[3]
                 )
                 a = Attendance(
                     single.text,
                     href,
-                    _type,
-                    date.split(" ")[0],
-                    lesson,
-                    subject,
-                    teacher,
-                    hour,
-                    excursion,
-                    by,
                     semester,
+                    attributes
                 )
                 att[semester-1].append(a)
     return att
```

### Comparing `librus_apix-0.2.5/librus_apix/get_token.py` & `librus_apix-0.2.6/librus_apix/get_token.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.5/librus_apix/grades.py` & `librus_apix-0.2.6/librus_apix/grades.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 self.grade[1].replace("+", ".5").replace("-", "-0.25")
             )
         else:
             grade_value = float(self.grade)
         return grade_value
 
 
-def get_grades(token: Token, sort_by: str = 'all') -> tuple[dict[int, list[Union[Grade, Gpa]]], dict[str, Gpa]]:
+def get_grades(token: Token, sort_by: str = 'all') -> tuple[dict[int, dict[str ,Grade]], dict[str, Gpa]]:
     def get_desc_and_counts(a, grade, subject) -> list[str, bool]:
         desc = f"Ocena: {_grade}\nPrzedmiot: {subject}\n"
         desc += re.sub(
             r"<br*>",
             "\n",
             a.attrs["title"].replace("<br/>", "").replace("<br />", "\n"),
         )
@@ -58,15 +58,15 @@
         return desc, counts
     SORT = {
         "all": 'zmiany_logowanie_wszystkie',
         "week": 'zmiany_logowanie_tydzien',
         "last_login": 'zmiany_logowanie'
             }
     if sort_by not in SORT.keys():
-        raise ArgumentError("Wrong value for sort_by it can be either all, week or last_login") 
+        raise ArgumentError("Wrong value for sort_by it can be either all, week or last_login")
     sem_grades: dict[int, dict[str, list[Grade]]] = {1: {}, 2: {}}
     avg_grades = defaultdict(list)
 
     tr = no_access_check(
             BeautifulSoup(token.post(BASE_URL + "/przegladaj_oceny/uczen", data={SORT[sort_by]: 1}).text, "lxml")
     ).find_all("tr", attrs={"class": ["line0", "line1"], "id": None})
     if len(tr) < 1:
@@ -76,21 +76,21 @@
             continue
         semester_grades = box.select(
             'td[class!="center micro screen-only"]'#[class!="right"]'
         )
         if len(semester_grades) < 9:
             continue
         average_grades = list(map(lambda x: x.text, box.select('td.right')))
-        semesters = [semester_grades[1:4], semester_grades[5:7]]
+        semesters = [semester_grades[1:4], semester_grades[4:7]]
         subject = semester_grades[0].text.replace("\n", "").strip()
         for sem, semester in enumerate(semesters):
             if subject not in sem_grades[sem + 1]:
                 sem_grades[sem + 1][subject] = []
             for sg in semester:
-                grade_a = sg.select("span.grade-box > a")
+                grade_a = sg.select("td[class!='center'] > span.grade-box > a")
                 for a in grade_a:
                     date = re.search("Data:.{11}", a.attrs["title"])
                     attr_dict = {}
                     for attr in a.attrs['title'].replace('<br/>', '<br>').split('<br>'):
                         if len(attr.strip()) > 2:
                             key, value = attr.split(': ')
                             attr_dict[key] = value
@@ -117,10 +117,10 @@
                         sem + 1,
                         category,
                         teacher,
                         weight
                     )
                     sem_grades[sem + 1][subject].append(g)
             gpa = Gpa(sem+1, average_grades[sem], subject)
-            avg_grades[subject].append(gpa) 
+            avg_grades[subject].append(gpa)
         avg_grades[subject].append(Gpa(0, average_grades[-1], subject))
     return sem_grades, avg_grades
```

### Comparing `librus_apix-0.2.5/librus_apix/homework.py` & `librus_apix-0.2.6/librus_apix/homework.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.5/librus_apix/messages.py` & `librus_apix-0.2.6/librus_apix/messages.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.5/librus_apix/schedule.py` & `librus_apix-0.2.6/librus_apix/schedule.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.5/librus_apix/timetable.py` & `librus_apix-0.2.6/librus_apix/timetable.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.5/librus_apix.egg-info/SOURCES.txt` & `librus_apix-0.2.6/librus_apix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.5/setup.cfg` & `librus_apix-0.2.6/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = 0.2.5
+version = 0.2.6
 license = MIT
 description = Web Scraper for Librus Synergia
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers = 
 	License :: OSI Approved :: MIT License
```

