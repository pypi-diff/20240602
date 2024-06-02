# Comparing `tmp/Baseball-Info-0.0.0.1.tar.gz` & `tmp/Baseball-Info-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Baseball-Info-0.0.0.1.tar", last modified: Sun Jun  2 10:44:08 2024, max compression
+gzip compressed data, was "Baseball-Info-0.0.0.2.tar", last modified: Sun Jun  2 11:17:41 2024, max compression
```

## Comparing `Baseball-Info-0.0.0.1.tar` & `Baseball-Info-0.0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 10:44:08.323576 Baseball-Info-0.0.0.1/
-drwxrwxrwx   0        0        0        0 2024-06-02 10:44:08.316938 Baseball-Info-0.0.0.1/Baseball_Info.egg-info/
--rw-rw-rw-   0        0        0      229 2024-06-02 10:44:08.000000 Baseball-Info-0.0.0.1/Baseball_Info.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-06-02 10:44:08.000000 Baseball-Info-0.0.0.1/Baseball_Info.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 10:44:08.000000 Baseball-Info-0.0.0.1/Baseball_Info.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-06-02 10:44:08.000000 Baseball-Info-0.0.0.1/Baseball_Info.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-06-02 10:44:08.000000 Baseball-Info-0.0.0.1/Baseball_Info.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      229 2024-06-02 10:44:08.322446 Baseball-Info-0.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-23 11:02:11.000000 Baseball-Info-0.0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 10:44:08.321445 Baseball-Info-0.0.0.1/baseball_Info/
--rw-rw-rw-   0        0        0       41 2024-03-29 03:51:58.000000 Baseball-Info-0.0.0.1/baseball_Info/__init__.py
--rw-rw-rw-   0        0        0     5497 2024-06-02 10:32:19.000000 Baseball-Info-0.0.0.1/baseball_Info/player.py
--rw-rw-rw-   0        0        0     3520 2024-06-02 10:43:04.000000 Baseball-Info-0.0.0.1/baseball_Info/team.py
--rw-rw-rw-   0        0        0       42 2024-06-02 10:44:08.323576 Baseball-Info-0.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      787 2024-06-02 09:40:06.000000 Baseball-Info-0.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 11:17:41.573994 Baseball-Info-0.0.0.2/
+drwxrwxrwx   0        0        0        0 2024-06-02 11:17:41.567989 Baseball-Info-0.0.0.2/Baseball_Info.egg-info/
+-rw-rw-rw-   0        0        0      229 2024-06-02 11:17:41.000000 Baseball-Info-0.0.0.2/Baseball_Info.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-06-02 11:17:41.000000 Baseball-Info-0.0.0.2/Baseball_Info.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 11:17:41.000000 Baseball-Info-0.0.0.2/Baseball_Info.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-02 11:17:41.000000 Baseball-Info-0.0.0.2/Baseball_Info.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-06-02 11:17:41.000000 Baseball-Info-0.0.0.2/Baseball_Info.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      229 2024-06-02 11:17:41.573994 Baseball-Info-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-03-23 11:02:11.000000 Baseball-Info-0.0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 11:17:41.571992 Baseball-Info-0.0.0.2/baseball_Info/
+-rw-rw-rw-   0        0        0       41 2024-03-29 03:51:58.000000 Baseball-Info-0.0.0.2/baseball_Info/__init__.py
+-rw-rw-rw-   0        0        0     5747 2024-06-02 11:13:36.000000 Baseball-Info-0.0.0.2/baseball_Info/player.py
+-rw-rw-rw-   0        0        0     3782 2024-06-02 11:15:00.000000 Baseball-Info-0.0.0.2/baseball_Info/team.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 11:17:41.573994 Baseball-Info-0.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      787 2024-06-02 11:16:00.000000 Baseball-Info-0.0.0.2/setup.py
```

### Comparing `Baseball-Info-0.0.0.1/baseball_Info/player.py` & `Baseball-Info-0.0.0.2/baseball_Info/player.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import pymysql
 
 def player_info(year, position, player_name=None):
+    try:
+        year = int(year)
+    except ValueError:
+        return "Year must be an integer between 2001 and 2023"
+    
     if not (2001 <= year <= 2023):
         return "Year must be between 2001 and 2023"
 
     valid_position = ["hitter", "pitcher", "defender", "runner"]
     if position not in valid_position:
         return "Position must be one of the following: hitter, pitcher, defender, runner" 
     try:
@@ -126,14 +131,19 @@
 
     except pymysql.Error as err:
         print(f"MySQL 오류: {err}")
         return None
     
     
 def homerun_rank(year, limit=50):
+    try:
+        year = int(year)
+    except ValueError:
+        return "Year must be an integer between 2001 and 2023"
+    
     if not (2001 <= year <= 2023):
         return "Year must be between 2001 and 2023"
     if not (1 <= limit <= 50):
         return "Rank must be between 1 and 50"
     
     conn = pymysql.connect(
         host='222.111.68.160',
```

### Comparing `Baseball-Info-0.0.0.1/baseball_Info/team.py` & `Baseball-Info-0.0.0.2/baseball_Info/team.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 import pymysql
 from tabulate import tabulate
 
 def team_info(year, team_name=None):
+    try:
+        year = int(year)
+    except ValueError:
+        return "Year must be an integer between 2001 and 2023"
+    
     if not (2001 <= year <= 2023):
         return "Year must be between 2001 and 2023"
     
     try:
         # MySQL 연결 설정
         conn = pymysql.connect(
             host='222.111.68.160', 
@@ -61,14 +66,19 @@
     finally:
         if 'conn' in locals() and conn.open:
             cursor.close()
             conn.close()
 
             
     def team_wl(year, team1=None):
+        try:
+            year = int(year)
+        except ValueError:
+            return "Year must be an integer between 2001 and 2023"
+
         if not (2001 <= year <= 2023):
             return "Year must be between 2001 and 2023"
         
         try:
             # MySQL 연결 설정
             conn = pymysql.connect(
                 host='222.111.68.160',
```

### Comparing `Baseball-Info-0.0.0.1/setup.py` & `Baseball-Info-0.0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as f: # README.md 내용 읽어오기
     long_description = f.read()
 
 setup(
     name='Baseball-Info', # 패키지 이름
-    version='0.0.0.1', # 버전 등록
+    version='0.0.0.2', # 버전 등록
     long_description=long_description, # readme.md 등록
     long_description_content_type='text/markdown',  # readme.md 포맷
     description='baseball API', # 패키지 설명
     author='basekk', # 작성자 등록
     author_email='jino152637@gmail.com', # 이메일 등록
     url='', # url 등록
     license='MIT', # 라이센스 등록
```

