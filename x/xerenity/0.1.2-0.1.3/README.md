# Comparing `tmp/xerenity-0.1.2.tar.gz` & `tmp/xerenity-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xerenity-0.1.2.tar", last modified: Sat Jun  1 02:08:42 2024, max compression
+gzip compressed data, was "xerenity-0.1.3.tar", last modified: Sun Jun  2 03:51:38 2024, max compression
```

## Comparing `xerenity-0.1.2.tar` & `xerenity-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:08:42.833163 xerenity-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 02:08:33.000000 xerenity-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-06-01 02:08:42.833163 xerenity-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-06-01 02:08:33.000000 xerenity-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 02:08:42.833163 xerenity-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-06-01 02:08:33.000000 xerenity-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:08:42.829163 xerenity-0.1.2/xerenity/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-06-01 02:08:33.000000 xerenity-0.1.2/xerenity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:08:42.833163 xerenity-0.1.2/xerenity/connection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 02:08:33.000000 xerenity-0.1.2/xerenity/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-06-01 02:08:33.000000 xerenity-0.1.2/xerenity/connection/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:08:42.833163 xerenity-0.1.2/xerenity/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 02:08:33.000000 xerenity-0.1.2/xerenity/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-06-01 02:08:33.000000 xerenity-0.1.2/xerenity/search/series.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:08:42.833163 xerenity-0.1.2/xerenity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-06-01 02:08:42.000000 xerenity-0.1.2/xerenity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-06-01 02:08:42.000000 xerenity-0.1.2/xerenity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 02:08:42.000000 xerenity-0.1.2/xerenity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 02:08:42.000000 xerenity-0.1.2/xerenity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 02:08:42.000000 xerenity-0.1.2/xerenity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 03:51:38.779296 xerenity-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 03:51:30.000000 xerenity-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-06-02 03:51:38.779296 xerenity-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-06-02 03:51:30.000000 xerenity-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 03:51:38.779296 xerenity-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-06-02 03:51:30.000000 xerenity-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 03:51:38.775296 xerenity-0.1.3/xerenity/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-06-02 03:51:30.000000 xerenity-0.1.3/xerenity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 03:51:38.779296 xerenity-0.1.3/xerenity/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 03:51:30.000000 xerenity-0.1.3/xerenity/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-06-02 03:51:30.000000 xerenity-0.1.3/xerenity/connection/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 03:51:38.779296 xerenity-0.1.3/xerenity/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 03:51:30.000000 xerenity-0.1.3/xerenity/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-06-02 03:51:30.000000 xerenity-0.1.3/xerenity/search/series.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 03:51:38.779296 xerenity-0.1.3/xerenity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-06-02 03:51:38.000000 xerenity-0.1.3/xerenity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-06-02 03:51:38.000000 xerenity-0.1.3/xerenity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 03:51:38.000000 xerenity-0.1.3/xerenity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 03:51:38.000000 xerenity-0.1.3/xerenity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 03:51:38.000000 xerenity-0.1.3/xerenity.egg-info/top_level.txt
```

### Comparing `xerenity-0.1.2/PKG-INFO` & `xerenity-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xerenity
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package for xerenity
 Home-page: https://xerenity.vercel.app/login
 Author: Andres Velez
 Author-email: svelez@xerenity.co
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -62,21 +62,22 @@
 password = os.environ.get('XERENITY_PASSWORD')
 
 # Crea la clase principal de xerenity, con esta tienes acceso a todas nuestras series
 data = Xerenity(username, password)
 
 # En la funcion search, da el nombre de la serie que necesitas los datos
 # En este caso vamos a lerr los datos del ibr de 3 anos
-ibr_3y = data.series.search('ibr_3y')
+ibr_3y = data.series.search(ticker='3d9f4cdbc81a0e04d61b6c9601f3a049')
 
 # Puedes utilizar librearias como pandas, para analizar tus datos
 ibr_3y_df = pd.DataFrame(ibr_3y)
 
 print(ibr_3y_df)
 
+
 ```
 
 La salida del anterio ejemplo seria algo como
 
 ```commandline
 
            time   value
```

### Comparing `xerenity-0.1.2/README.md` & `xerenity-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -45,21 +45,22 @@
 password = os.environ.get('XERENITY_PASSWORD')
 
 # Crea la clase principal de xerenity, con esta tienes acceso a todas nuestras series
 data = Xerenity(username, password)
 
 # En la funcion search, da el nombre de la serie que necesitas los datos
 # En este caso vamos a lerr los datos del ibr de 3 anos
-ibr_3y = data.series.search('ibr_3y')
+ibr_3y = data.series.search(ticker='3d9f4cdbc81a0e04d61b6c9601f3a049')
 
 # Puedes utilizar librearias como pandas, para analizar tus datos
 ibr_3y_df = pd.DataFrame(ibr_3y)
 
 print(ibr_3y_df)
 
+
 ```
 
 La salida del anterio ejemplo seria algo como
 
 ```commandline
 
            time   value
```

### Comparing `xerenity-0.1.2/setup.py` & `xerenity-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='xerenity',
-    version='0.1.2',
+    version='0.1.3',
     description='Python package for xerenity',
     url='https://xerenity.vercel.app/login',
     author='Andres Velez',
     author_email='svelez@xerenity.co',
     license='BSD 2-clause',
     install_requires=['supabase>=2.4.4'],
     packages=find_packages(),
```

### Comparing `xerenity-0.1.2/xerenity/connection/db.py` & `xerenity-0.1.3/xerenity/connection/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,23 +43,23 @@
         """
         try:
             data = self.supabase.from_('search_mv').select('source_name,grupo,description,display_name').execute().data
             return data
         except Exception as er:
             return str(er)
 
-    def read_serie(self, source_name: str):
+    def read_serie(self, ticker: str):
         """
 
         Funcion que retorna los valores de la serie deseada, si la serie no es encontrada
         se retorna un contenedor vacio
 
-        :param serie_id: Identificador unico de la serie a leer
+        :param ticker: Identificador unico de la serie a leer
         :return:
         """
         try:
-            data = self.supabase.rpc('search', {"name": source_name}).execute().data
+            data = self.supabase.rpc('search', {"ticket": ticker}).execute().data
             if 'data' in data:
                 return data['data']
             return data
         except Exception as er:
             return str(er)
```

### Comparing `xerenity-0.1.2/xerenity/search/series.py` & `xerenity-0.1.3/xerenity/search/series.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,16 +7,16 @@
         """
 
         Function para obtener el portafolio completo de series que ofrece Xerenity
         :return: [{{'source_name': str, 'grupo': str, 'description': str, 'display_name':str}]
         """
         return self.sup.get_all_series()
 
-    def search(self, source_name):
+    def search(self, ticker):
         """
 
         Dado el nombre de una serie, retorna los valores almacenados por Xerenity
         Para obtener el nombre de la serie, puede vistar la pagina web o utilizar la funcion portafolio
-        :param source_name:
+        :param ticker:
         :return: [{"time":"fecha","value":valor de la serie en la fecha}]
         """
-        return self.sup.read_serie(source_name=source_name)
+        return self.sup.read_serie(ticker=ticker)
```

### Comparing `xerenity-0.1.2/xerenity.egg-info/PKG-INFO` & `xerenity-0.1.3/xerenity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xerenity
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package for xerenity
 Home-page: https://xerenity.vercel.app/login
 Author: Andres Velez
 Author-email: svelez@xerenity.co
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -62,21 +62,22 @@
 password = os.environ.get('XERENITY_PASSWORD')
 
 # Crea la clase principal de xerenity, con esta tienes acceso a todas nuestras series
 data = Xerenity(username, password)
 
 # En la funcion search, da el nombre de la serie que necesitas los datos
 # En este caso vamos a lerr los datos del ibr de 3 anos
-ibr_3y = data.series.search('ibr_3y')
+ibr_3y = data.series.search(ticker='3d9f4cdbc81a0e04d61b6c9601f3a049')
 
 # Puedes utilizar librearias como pandas, para analizar tus datos
 ibr_3y_df = pd.DataFrame(ibr_3y)
 
 print(ibr_3y_df)
 
+
 ```
 
 La salida del anterio ejemplo seria algo como
 
 ```commandline
 
            time   value
```

