# Comparing `tmp/Baseball-Info-0.0.0.5.tar.gz` & `tmp/Baseball-Info-0.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Baseball-Info-0.0.0.5.tar", last modified: Sun Jun  2 11:49:07 2024, max compression
+gzip compressed data, was "Baseball-Info-0.0.0.6.tar", last modified: Sun Jun  2 11:51:47 2024, max compression
```

## Comparing `Baseball-Info-0.0.0.5.tar` & `Baseball-Info-0.0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 11:49:07.123724 Baseball-Info-0.0.0.5/
-drwxrwxrwx   0        0        0        0 2024-06-02 11:49:07.118207 Baseball-Info-0.0.0.5/Baseball_Info.egg-info/
--rw-rw-rw-   0        0        0      229 2024-06-02 11:49:07.000000 Baseball-Info-0.0.0.5/Baseball_Info.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-06-02 11:49:07.000000 Baseball-Info-0.0.0.5/Baseball_Info.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 11:49:07.000000 Baseball-Info-0.0.0.5/Baseball_Info.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-06-02 11:49:07.000000 Baseball-Info-0.0.0.5/Baseball_Info.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-06-02 11:49:07.000000 Baseball-Info-0.0.0.5/Baseball_Info.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      229 2024-06-02 11:49:07.123724 Baseball-Info-0.0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-23 11:02:11.000000 Baseball-Info-0.0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 11:49:07.121711 Baseball-Info-0.0.0.5/baseball_Info/
--rw-rw-rw-   0        0        0       41 2024-03-29 03:51:58.000000 Baseball-Info-0.0.0.5/baseball_Info/__init__.py
--rw-rw-rw-   0        0        0     5657 2024-06-02 11:41:22.000000 Baseball-Info-0.0.0.5/baseball_Info/player.py
--rw-rw-rw-   0        0        0     3416 2024-06-02 11:47:59.000000 Baseball-Info-0.0.0.5/baseball_Info/team.py
--rw-rw-rw-   0        0        0       42 2024-06-02 11:49:07.124725 Baseball-Info-0.0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      787 2024-06-02 11:48:51.000000 Baseball-Info-0.0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 11:51:47.151062 Baseball-Info-0.0.0.6/
+drwxrwxrwx   0        0        0        0 2024-06-02 11:51:47.145049 Baseball-Info-0.0.0.6/Baseball_Info.egg-info/
+-rw-rw-rw-   0        0        0      229 2024-06-02 11:51:47.000000 Baseball-Info-0.0.0.6/Baseball_Info.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-06-02 11:51:47.000000 Baseball-Info-0.0.0.6/Baseball_Info.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 11:51:47.000000 Baseball-Info-0.0.0.6/Baseball_Info.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-02 11:51:47.000000 Baseball-Info-0.0.0.6/Baseball_Info.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-06-02 11:51:47.000000 Baseball-Info-0.0.0.6/Baseball_Info.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      229 2024-06-02 11:51:47.150062 Baseball-Info-0.0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-03-23 11:02:11.000000 Baseball-Info-0.0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 11:51:47.149052 Baseball-Info-0.0.0.6/baseball_Info/
+-rw-rw-rw-   0        0        0       41 2024-03-29 03:51:58.000000 Baseball-Info-0.0.0.6/baseball_Info/__init__.py
+-rw-rw-rw-   0        0        0     5650 2024-06-02 11:50:35.000000 Baseball-Info-0.0.0.6/baseball_Info/player.py
+-rw-rw-rw-   0        0        0     3416 2024-06-02 11:47:59.000000 Baseball-Info-0.0.0.6/baseball_Info/team.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 11:51:47.151062 Baseball-Info-0.0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      787 2024-06-02 11:51:36.000000 Baseball-Info-0.0.0.6/setup.py
```

### Comparing `Baseball-Info-0.0.0.5/baseball_Info/player.py` & `Baseball-Info-0.0.0.6/baseball_Info/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,16 +119,16 @@
                     '주루사': info[7],
                     '견제사': info[8]
                 }
             players.append(player)
 
         # 연결 종료
         conn.close()
-        
-        if player == []:
+
+        if players == []:
             return "Player name must be provided"
 
         return players
 
     except pymysql.Error as err:
         print(f"MySQL 오류: {err}")
         return None
```

### Comparing `Baseball-Info-0.0.0.5/baseball_Info/team.py` & `Baseball-Info-0.0.0.6/baseball_Info/team.py`

 * *Files identical despite different names*

### Comparing `Baseball-Info-0.0.0.5/setup.py` & `Baseball-Info-0.0.0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as f: # README.md 내용 읽어오기
     long_description = f.read()
 
 setup(
     name='Baseball-Info', # 패키지 이름
-    version='0.0.0.5', # 버전 등록
+    version='0.0.0.6', # 버전 등록
     long_description=long_description, # readme.md 등록
     long_description_content_type='text/markdown',  # readme.md 포맷
     description='baseball API', # 패키지 설명
     author='basekk', # 작성자 등록
     author_email='jino152637@gmail.com', # 이메일 등록
     url='', # url 등록
     license='MIT', # 라이센스 등록
```

