# Comparing `tmp/Baseball-Info-0.0.0.3.tar.gz` & `tmp/Baseball-Info-0.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Baseball-Info-0.0.0.3.tar", last modified: Sun Jun  2 11:22:05 2024, max compression
+gzip compressed data, was "Baseball-Info-0.0.0.4.tar", last modified: Sun Jun  2 11:30:04 2024, max compression
```

## Comparing `Baseball-Info-0.0.0.3.tar` & `Baseball-Info-0.0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 11:22:05.731782 Baseball-Info-0.0.0.3/
-drwxrwxrwx   0        0        0        0 2024-06-02 11:22:05.726272 Baseball-Info-0.0.0.3/Baseball_Info.egg-info/
--rw-rw-rw-   0        0        0      229 2024-06-02 11:22:05.000000 Baseball-Info-0.0.0.3/Baseball_Info.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-06-02 11:22:05.000000 Baseball-Info-0.0.0.3/Baseball_Info.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 11:22:05.000000 Baseball-Info-0.0.0.3/Baseball_Info.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-06-02 11:22:05.000000 Baseball-Info-0.0.0.3/Baseball_Info.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-06-02 11:22:05.000000 Baseball-Info-0.0.0.3/Baseball_Info.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      229 2024-06-02 11:22:05.731782 Baseball-Info-0.0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-23 11:02:11.000000 Baseball-Info-0.0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 11:22:05.730277 Baseball-Info-0.0.0.3/baseball_Info/
--rw-rw-rw-   0        0        0       41 2024-03-29 03:51:58.000000 Baseball-Info-0.0.0.3/baseball_Info/__init__.py
--rw-rw-rw-   0        0        0     5746 2024-06-02 11:21:55.000000 Baseball-Info-0.0.0.3/baseball_Info/player.py
--rw-rw-rw-   0        0        0     3785 2024-06-02 11:21:31.000000 Baseball-Info-0.0.0.3/baseball_Info/team.py
--rw-rw-rw-   0        0        0       42 2024-06-02 11:22:05.731782 Baseball-Info-0.0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      787 2024-06-02 11:20:27.000000 Baseball-Info-0.0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 11:30:04.710792 Baseball-Info-0.0.0.4/
+drwxrwxrwx   0        0        0        0 2024-06-02 11:30:04.704786 Baseball-Info-0.0.0.4/Baseball_Info.egg-info/
+-rw-rw-rw-   0        0        0      229 2024-06-02 11:30:04.000000 Baseball-Info-0.0.0.4/Baseball_Info.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-06-02 11:30:04.000000 Baseball-Info-0.0.0.4/Baseball_Info.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 11:30:04.000000 Baseball-Info-0.0.0.4/Baseball_Info.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-02 11:30:04.000000 Baseball-Info-0.0.0.4/Baseball_Info.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-06-02 11:30:04.000000 Baseball-Info-0.0.0.4/Baseball_Info.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      229 2024-06-02 11:30:04.709791 Baseball-Info-0.0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-03-23 11:02:11.000000 Baseball-Info-0.0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 11:30:04.708789 Baseball-Info-0.0.0.4/baseball_Info/
+-rw-rw-rw-   0        0        0       41 2024-03-29 03:51:58.000000 Baseball-Info-0.0.0.4/baseball_Info/__init__.py
+-rw-rw-rw-   0        0        0     5573 2024-06-02 11:29:26.000000 Baseball-Info-0.0.0.4/baseball_Info/player.py
+-rw-rw-rw-   0        0        0     3580 2024-06-02 11:29:43.000000 Baseball-Info-0.0.0.4/baseball_Info/team.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 11:30:04.710792 Baseball-Info-0.0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      787 2024-06-02 11:29:54.000000 Baseball-Info-0.0.0.4/setup.py
```

### Comparing `Baseball-Info-0.0.0.3/baseball_Info/player.py` & `Baseball-Info-0.0.0.4/baseball_Info/player.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import pymysql
 
 def player_info(year, position, player_name=None):
-    if not year.isdigit():
-        return "Year must be a numeric string between '2001' and '2023'"
-
+    
     year = int(year)
     if not (2001 <= year <= 2023):
         return "Year must be between 2001 and 2023"
 
     valid_position = ["hitter", "pitcher", "defender", "runner"]
     if position not in valid_position:
         return "Position must be one of the following: hitter, pitcher, defender, runner" 
@@ -130,18 +128,17 @@
 
     except pymysql.Error as err:
         print(f"MySQL 오류: {err}")
         return None
     
     
 def homerun_rank(year, limit=50):
-    if not year.isdigit():
-        return "Year must be a numeric string between '2001' and '2023'"
 
     year = int(year)
+    limit = int(limit)
     
     if not (2001 <= year <= 2023):
         return "Year must be between 2001 and 2023"
     if not (1 <= limit <= 50):
         return "Rank must be between 1 and 50"
     
     conn = pymysql.connect(
```

### Comparing `Baseball-Info-0.0.0.3/baseball_Info/team.py` & `Baseball-Info-0.0.0.4/baseball_Info/team.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import pymysql
 from tabulate import tabulate
 
 def team_info(year, team_name=None):
-    if not year.isdigit():
-        return "Year must be a numeric string between '2001' and '2023'"
-
+    
     year = int(year)
     if not (2001 <= year <= 2023):
         return "Year must be between 2001 and 2023"
     
     try:
         # MySQL 연결 설정
         conn = pymysql.connect(
@@ -65,19 +63,17 @@
     finally:
         if 'conn' in locals() and conn.open:
             cursor.close()
             conn.close()
 
             
     def team_wl(year, team1=None):
-        if not year.isdigit():
-            return "Year must be a numeric string between '2001' and '2023'"
-
+       
         year = int(year)
-        
+
         if not (2001 <= year <= 2023):
             return "Year must be between 2001 and 2023"
         
         try:
             # MySQL 연결 설정
             conn = pymysql.connect(
                 host='222.111.68.160',
```

### Comparing `Baseball-Info-0.0.0.3/setup.py` & `Baseball-Info-0.0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as f: # README.md 내용 읽어오기
     long_description = f.read()
 
 setup(
     name='Baseball-Info', # 패키지 이름
-    version='0.0.0.3', # 버전 등록
+    version='0.0.0.4', # 버전 등록
     long_description=long_description, # readme.md 등록
     long_description_content_type='text/markdown',  # readme.md 포맷
     description='baseball API', # 패키지 설명
     author='basekk', # 작성자 등록
     author_email='jino152637@gmail.com', # 이메일 등록
     url='', # url 등록
     license='MIT', # 라이센스 등록
```

