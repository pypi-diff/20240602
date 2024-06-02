# Comparing `tmp/Baseball-Info-0.0.0.4.tar.gz` & `tmp/Baseball-Info-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Baseball-Info-0.0.0.4.tar", last modified: Sun Jun  2 11:30:04 2024, max compression
+gzip compressed data, was "Baseball-Info-0.0.0.5.tar", last modified: Sun Jun  2 11:49:07 2024, max compression
```

## Comparing `Baseball-Info-0.0.0.4.tar` & `Baseball-Info-0.0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 11:30:04.710792 Baseball-Info-0.0.0.4/
-drwxrwxrwx   0        0        0        0 2024-06-02 11:30:04.704786 Baseball-Info-0.0.0.4/Baseball_Info.egg-info/
--rw-rw-rw-   0        0        0      229 2024-06-02 11:30:04.000000 Baseball-Info-0.0.0.4/Baseball_Info.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-06-02 11:30:04.000000 Baseball-Info-0.0.0.4/Baseball_Info.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 11:30:04.000000 Baseball-Info-0.0.0.4/Baseball_Info.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-06-02 11:30:04.000000 Baseball-Info-0.0.0.4/Baseball_Info.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-06-02 11:30:04.000000 Baseball-Info-0.0.0.4/Baseball_Info.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      229 2024-06-02 11:30:04.709791 Baseball-Info-0.0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-23 11:02:11.000000 Baseball-Info-0.0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 11:30:04.708789 Baseball-Info-0.0.0.4/baseball_Info/
--rw-rw-rw-   0        0        0       41 2024-03-29 03:51:58.000000 Baseball-Info-0.0.0.4/baseball_Info/__init__.py
--rw-rw-rw-   0        0        0     5573 2024-06-02 11:29:26.000000 Baseball-Info-0.0.0.4/baseball_Info/player.py
--rw-rw-rw-   0        0        0     3580 2024-06-02 11:29:43.000000 Baseball-Info-0.0.0.4/baseball_Info/team.py
--rw-rw-rw-   0        0        0       42 2024-06-02 11:30:04.710792 Baseball-Info-0.0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      787 2024-06-02 11:29:54.000000 Baseball-Info-0.0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 11:49:07.123724 Baseball-Info-0.0.0.5/
+drwxrwxrwx   0        0        0        0 2024-06-02 11:49:07.118207 Baseball-Info-0.0.0.5/Baseball_Info.egg-info/
+-rw-rw-rw-   0        0        0      229 2024-06-02 11:49:07.000000 Baseball-Info-0.0.0.5/Baseball_Info.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-06-02 11:49:07.000000 Baseball-Info-0.0.0.5/Baseball_Info.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 11:49:07.000000 Baseball-Info-0.0.0.5/Baseball_Info.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-02 11:49:07.000000 Baseball-Info-0.0.0.5/Baseball_Info.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-06-02 11:49:07.000000 Baseball-Info-0.0.0.5/Baseball_Info.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      229 2024-06-02 11:49:07.123724 Baseball-Info-0.0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-03-23 11:02:11.000000 Baseball-Info-0.0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 11:49:07.121711 Baseball-Info-0.0.0.5/baseball_Info/
+-rw-rw-rw-   0        0        0       41 2024-03-29 03:51:58.000000 Baseball-Info-0.0.0.5/baseball_Info/__init__.py
+-rw-rw-rw-   0        0        0     5657 2024-06-02 11:41:22.000000 Baseball-Info-0.0.0.5/baseball_Info/player.py
+-rw-rw-rw-   0        0        0     3416 2024-06-02 11:47:59.000000 Baseball-Info-0.0.0.5/baseball_Info/team.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 11:49:07.124725 Baseball-Info-0.0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      787 2024-06-02 11:48:51.000000 Baseball-Info-0.0.0.5/setup.py
```

### Comparing `Baseball-Info-0.0.0.4/baseball_Info/player.py` & `Baseball-Info-0.0.0.5/baseball_Info/player.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,14 +119,17 @@
                     '주루사': info[7],
                     '견제사': info[8]
                 }
             players.append(player)
 
         # 연결 종료
         conn.close()
+        
+        if player == []:
+            return "Player name must be provided"
 
         return players
 
     except pymysql.Error as err:
         print(f"MySQL 오류: {err}")
         return None
```

### Comparing `Baseball-Info-0.0.0.4/baseball_Info/team.py` & `Baseball-Info-0.0.0.5/baseball_Info/team.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,60 +62,60 @@
 
     finally:
         if 'conn' in locals() and conn.open:
             cursor.close()
             conn.close()
 
             
-    def team_wl(year, team1=None):
+def team_wl(year, team1=None):
        
-        year = int(year)
+    year = int(year)
 
-        if not (2001 <= year <= 2023):
-            return "Year must be between 2001 and 2023"
-        
-        try:
-            # MySQL 연결 설정
-            conn = pymysql.connect(
-                host='222.111.68.160', 
-                user='root',
-                password='1322', 
-                database='baseball_stat',
-                charset='utf8'
-            )
-
-            # 커서 생성
-            cursor = conn.cursor()
-
-            # 쿼리 생성
-            if team1:  # 특정 팀의 승패표를 가져오는 경우
-                query = f"SELECT * FROM regular_team_WL_{year} WHERE `team_name` = '{team1}'"
-            else:  # 전체 팀의 승패표를 가져오는 경우
-                query = f"SELECT * FROM regular_team_WL_{year}"
-
-            # 쿼리 실행
-            cursor.execute(query)
-
-            if team1 and not team_wl:
-                return f"Error: '{team1}' does not exist in the year {year}"
-
-            # 컬럼 이름 가져오기
-            columns = [col[0] for col in cursor.description]
-
-            # 결과 가져오기
-            team_wl = cursor.fetchall()
-
-            # 테이블 형태로 출력하기 위한 데이터 가공
-            data = [columns]  # 헤더 추가
-            for wl in team_wl:
-                data.append(list(wl))
-
-            # 테이블 형태로 출력
-            return tabulate(data, tablefmt="grid")
-
-        except pymysql.Error as err:
-            print("")
-
-        finally:
-            if 'conn' in locals() and conn.open:
-                cursor.close()
-                conn.close()
+    if not (2001 <= year <= 2023):
+        return "Year must be between 2001 and 2023"
+    
+    try:
+        # MySQL 연결 설정
+        conn = pymysql.connect(
+            host='222.111.68.160', 
+            user='root',
+            password='1322', 
+            database='baseball_stat',
+            charset='utf8'
+        )
+
+        # 커서 생성
+        cursor = conn.cursor()
+
+        # 쿼리 생성
+        if team1:  # 특정 팀의 승패표를 가져오는 경우
+            query = f"SELECT * FROM regular_team_WL_{year} WHERE `team_name` = '{team1}'"
+        else:  # 전체 팀의 승패표를 가져오는 경우
+            query = f"SELECT * FROM regular_team_WL_{year}"
+
+        # 쿼리 실행
+        cursor.execute(query)
+
+        if team1 and not team_wl:
+            return f"Error: '{team1}' does not exist in the year {year}"
+
+        # 컬럼 이름 가져오기
+        columns = [col[0] for col in cursor.description]
+
+        # 결과 가져오기
+        team_wl = cursor.fetchall()
+
+        # 테이블 형태로 출력하기 위한 데이터 가공
+        data = [columns]  # 헤더 추가
+        for wl in team_wl:
+            data.append(list(wl))
+
+        # 테이블 형태로 출력
+        return tabulate(data, tablefmt="grid")
+
+    except pymysql.Error as err:
+        print("")
+
+    finally:
+        if 'conn' in locals() and conn.open:
+            cursor.close()
+            conn.close()
```

### Comparing `Baseball-Info-0.0.0.4/setup.py` & `Baseball-Info-0.0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as f: # README.md 내용 읽어오기
     long_description = f.read()
 
 setup(
     name='Baseball-Info', # 패키지 이름
-    version='0.0.0.4', # 버전 등록
+    version='0.0.0.5', # 버전 등록
     long_description=long_description, # readme.md 등록
     long_description_content_type='text/markdown',  # readme.md 포맷
     description='baseball API', # 패키지 설명
     author='basekk', # 작성자 등록
     author_email='jino152637@gmail.com', # 이메일 등록
     url='', # url 등록
     license='MIT', # 라이센스 등록
```

