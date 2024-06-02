# Comparing `tmp/jobquery-1.0.1.tar.gz` & `tmp/jobquery-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobquery-1.0.1.tar", last modified: Sat Jun  1 11:25:09 2024, max compression
+gzip compressed data, was "jobquery-1.0.2.tar", last modified: Sat Jun  1 12:30:04 2024, max compression
```

## Comparing `jobquery-1.0.1.tar` & `jobquery-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 11:25:09.044171 jobquery-1.0.1/
--rw-rw-rw-   0        0        0      206 2024-06-01 11:25:09.043177 jobquery-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-01 11:25:09.021904 jobquery-1.0.1/jobQuery/
--rw-rw-rw-   0        0        0        0 2024-05-29 08:44:01.000000 jobquery-1.0.1/jobQuery/__init__.py
--rw-rw-rw-   0        0        0    33090 2024-06-01 11:18:58.000000 jobquery-1.0.1/jobQuery/jobAPI.py
-drwxrwxrwx   0        0        0        0 2024-06-01 11:25:09.042170 jobquery-1.0.1/jobQuery.egg-info/
--rw-rw-rw-   0        0        0      206 2024-06-01 11:25:08.000000 jobquery-1.0.1/jobQuery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2024-06-01 11:25:08.000000 jobquery-1.0.1/jobQuery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 11:25:08.000000 jobquery-1.0.1/jobQuery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-06-01 11:25:08.000000 jobquery-1.0.1/jobQuery.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 11:25:09.044171 jobquery-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      587 2024-06-01 11:24:44.000000 jobquery-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:30:04.257794 jobquery-1.0.2/
+-rw-rw-rw-   0        0        0      206 2024-06-01 12:30:04.255795 jobquery-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 12:30:04.239047 jobquery-1.0.2/jobQuery/
+-rw-rw-rw-   0        0        0        0 2024-05-29 08:44:01.000000 jobquery-1.0.2/jobQuery/__init__.py
+-rw-rw-rw-   0        0        0    33006 2024-06-01 12:28:47.000000 jobquery-1.0.2/jobQuery/jobAPI.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:30:04.254793 jobquery-1.0.2/jobQuery.egg-info/
+-rw-rw-rw-   0        0        0      206 2024-06-01 12:30:04.000000 jobquery-1.0.2/jobQuery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2024-06-01 12:30:04.000000 jobquery-1.0.2/jobQuery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 12:30:04.000000 jobquery-1.0.2/jobQuery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 12:30:04.000000 jobquery-1.0.2/jobQuery.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 12:30:04.257794 jobquery-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      587 2024-06-01 12:28:57.000000 jobquery-1.0.2/setup.py
```

### Comparing `jobquery-1.0.1/jobQuery/jobAPI.py` & `jobquery-1.0.2/jobQuery/jobAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -543,22 +543,17 @@
             print("Connection to MySQL not established.")
 
     def get_jobInfo(self, n):
         for i in range(n):
             yield self.get_jobInfo_by_id(i+1)
     
     def get_jobInfo_by_filter(self, category=None, skill=None, education=None, tool=None, experience=None, days=None, min_salary=0, max_salary=INF, limit=None):
-        if self.conn is not None:
-            try:
-                cursor = self.conn.cursor()
-                # 使用left join
-                # todo
-                
-            except mysql.connector.Error as e:
-                print("Error retrieving data from MySQL:", e)
+        job_ids = self.get_jobs_id_by_filter(category, skill, education, tool, experience, days, min_salary, max_salary, limit)
+        for job_id in job_ids:
+            yield self.get_jobInfo_by_id(job_id[0])
     
     def get_number_by_filter(self, category=None, skill=None, education=None, tool=None, experience=None, days=None, min_salary=0, max_salary=INF):
         if self.conn is not None:
             try:
                 cursor = self.conn.cursor()
                 query = '''
                     SELECT COUNT(*) FROM job
@@ -775,23 +770,24 @@
                                  education=None,
                                  tool=['python'],
                                  experience=None,
                                  days=None,
                                  min_salary=None,
                                  max_salary=None))
 
-    # jobs = db.get_jobInfo_by_filter(category=['後端工程師', '網路管理工程師'],
-    #                              skill=None,
-    #                              education=None,
-    #                              tool=None,
-    #                              experience=None,
-    #                              days=None,
-    #                              min_salary=None,
-    #                              max_salary=None
-    #                             )
+    jobs = db.get_jobInfo_by_filter(category=['後端工程師', '網路管理工程師'],
+                                 skill=None,
+                                 education=None,
+                                 tool=None,
+                                 experience=None,
+                                 days=None,
+                                 min_salary=None,
+                                 max_salary=None
+                                )
+    
     
     # for i in jobs:
     #     print(i)
     # name = 'jobs'
     # with open(fr'{name}.txt', 'w', encoding='utf-8') as f:
     #     data = [j for j in jobs]
     #     pprint.pprint(data, stream=f)
```

### Comparing `jobquery-1.0.1/setup.py` & `jobquery-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from setuptools import setup, find_packages
 setup(name='jobQuery',
-      version='1.0.1',
+      version='1.0.2',
       description='birds atttributes and functions',
       author='megnet',
       author_email='2290906844@qq.com',
       requires= ['numpy','matplotlib'], # 定义依赖哪些模块
       packages=find_packages(),  # 系统自动从当前目录开始找包
       # 如果有的文件不用打包，则只能指定需要打包的文件
       #packages=['代码1','代码2','__init__']  #指定目录中需要打包的py文件，注意不要.py后缀
```

