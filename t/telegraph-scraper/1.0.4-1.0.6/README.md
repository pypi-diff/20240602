# Comparing `tmp/telegraph-scraper-1.0.4.tar.gz` & `tmp/telegraph_scraper-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegraph-scraper-1.0.4.tar", last modified: Thu Sep 14 11:16:08 2023, max compression
+gzip compressed data, was "telegraph_scraper-1.0.6.tar", last modified: Sun Jun  2 15:42:23 2024, max compression
```

## Comparing `telegraph-scraper-1.0.4.tar` & `telegraph_scraper-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 solodk    (1000) solodk    (1000)        0 2023-09-14 11:16:08.179643 telegraph-scraper-1.0.4/
--rw-r--r--   0 solodk    (1000) solodk    (1000)    35823 2023-08-06 14:11:29.000000 telegraph-scraper-1.0.4/LICENSE
--rw-r--r--   0 solodk    (1000) solodk    (1000)      578 2023-09-14 11:16:08.179643 telegraph-scraper-1.0.4/PKG-INFO
--rw-r--r--   0 solodk    (1000) solodk    (1000)     2464 2023-09-14 10:32:36.000000 telegraph-scraper-1.0.4/README.md
-drwxr-xr-x   0 solodk    (1000) solodk    (1000)        0 2023-09-14 11:16:08.179643 telegraph-scraper-1.0.4/scraper/
--rw-r--r--   0 solodk    (1000) solodk    (1000)       37 2023-09-14 10:53:05.000000 telegraph-scraper-1.0.4/scraper/__init__.py
--rw-r--r--   0 solodk    (1000) solodk    (1000)     2720 2023-09-09 17:05:19.000000 telegraph-scraper-1.0.4/scraper/extra.py
--rw-r--r--   0 solodk    (1000) solodk    (1000)    17032 2023-09-14 11:15:32.000000 telegraph-scraper-1.0.4/scraper/telegraphscrape.py
--rw-r--r--   0 solodk    (1000) solodk    (1000)       38 2023-09-14 11:16:08.179643 telegraph-scraper-1.0.4/setup.cfg
--rw-r--r--   0 solodk    (1000) solodk    (1000)      856 2023-09-14 11:15:43.000000 telegraph-scraper-1.0.4/setup.py
-drwxr-xr-x   0 solodk    (1000) solodk    (1000)        0 2023-09-14 11:16:08.179643 telegraph-scraper-1.0.4/telegraph_scraper.egg-info/
--rw-r--r--   0 solodk    (1000) solodk    (1000)      578 2023-09-14 11:16:08.000000 telegraph-scraper-1.0.4/telegraph_scraper.egg-info/PKG-INFO
--rw-r--r--   0 solodk    (1000) solodk    (1000)      338 2023-09-14 11:16:08.000000 telegraph-scraper-1.0.4/telegraph_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 solodk    (1000) solodk    (1000)        1 2023-09-14 11:16:08.000000 telegraph-scraper-1.0.4/telegraph_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 solodk    (1000) solodk    (1000)       51 2023-09-14 11:16:08.000000 telegraph-scraper-1.0.4/telegraph_scraper.egg-info/entry_points.txt
--rw-r--r--   0 solodk    (1000) solodk    (1000)       14 2023-09-14 11:16:08.000000 telegraph-scraper-1.0.4/telegraph_scraper.egg-info/requires.txt
--rw-r--r--   0 solodk    (1000) solodk    (1000)        8 2023-09-14 11:16:08.000000 telegraph-scraper-1.0.4/telegraph_scraper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 15:42:23.927747 telegraph_scraper-1.0.6/
+-rw-rw-rw-   0        0        0    35823 2024-06-02 11:27:55.000000 telegraph_scraper-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      639 2024-06-02 15:42:23.925784 telegraph_scraper-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2464 2024-06-02 11:27:55.000000 telegraph_scraper-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 15:42:23.911788 telegraph_scraper-1.0.6/scraper/
+-rw-rw-rw-   0        0        0       37 2024-06-02 11:27:55.000000 telegraph_scraper-1.0.6/scraper/__init__.py
+-rw-rw-rw-   0        0        0     2720 2024-06-02 11:27:55.000000 telegraph_scraper-1.0.6/scraper/extra.py
+-rw-rw-rw-   0        0        0    18071 2024-06-02 15:32:37.000000 telegraph_scraper-1.0.6/scraper/telegraphscrape.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 15:42:23.927747 telegraph_scraper-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      885 2024-06-02 15:38:53.000000 telegraph_scraper-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:42:23.923756 telegraph_scraper-1.0.6/telegraph_scraper.egg-info/
+-rw-rw-rw-   0        0        0      639 2024-06-02 15:42:23.000000 telegraph_scraper-1.0.6/telegraph_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-06-02 15:42:23.000000 telegraph_scraper-1.0.6/telegraph_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 15:42:23.000000 telegraph_scraper-1.0.6/telegraph_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-06-02 15:42:23.000000 telegraph_scraper-1.0.6/telegraph_scraper.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-06-02 15:42:23.000000 telegraph_scraper-1.0.6/telegraph_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-02 15:42:23.000000 telegraph_scraper-1.0.6/telegraph_scraper.egg-info/top_level.txt
```

### Comparing `telegraph-scraper-1.0.4/LICENSE` & `telegraph_scraper-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `telegraph-scraper-1.0.4/PKG-INFO` & `telegraph_scraper-1.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 2.1
-Name: telegraph-scraper
-Version: 1.0.4
-Summary: A Python scraper for Telegraph pages
-Home-page: https://github.com/solodk/telegraph-scraper
-Author: Mykola Solodky
-Author-email: solodk.m@gmail.com
-Keywords: telegraph scrape image images download
-Classifier: Development Status :: 3 - Alpha
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-License-File: LICENSE
+Metadata-Version: 2.1
+Name: telegraph-scraper
+Version: 1.0.6
+Summary: A Python scraper for Telegraph pages
+Home-page: https://github.com/solodk/telegraph-scraper
+Author: Mykola Solodky
+Author-email: solodk.m@gmail.com
+Keywords: telegraph scrape image images download
+Classifier: Development Status :: 3 - Alpha
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE
+Requires-Dist: tqdm
+Requires-Dist: requests
```

### Comparing `telegraph-scraper-1.0.4/README.md` & `telegraph_scraper-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `telegraph-scraper-1.0.4/scraper/extra.py` & `telegraph_scraper-1.0.6/scraper/extra.py`

 * *Files identical despite different names*

### Comparing `telegraph-scraper-1.0.4/scraper/telegraphscrape.py` & `telegraph_scraper-1.0.6/scraper/telegraphscrape.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import concurrent.futures
 import os
 import requests
 import json
 import logging
+import re
 
 from datetime import datetime, timedelta
 from tqdm import tqdm
 
 from . import extra
 
 logging.basicConfig(
@@ -15,41 +16,56 @@
     filename=os.path.join(os.path.dirname(__file__), 'scraper.log'),
     format='%(asctime)s [%(levelname)s] - %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S',
 )
 
 class Scraper(object):
     def __init__(self, query):
-        self.input_query = query
+        logging.info(f'Initialization...')
+        self.formated_query = self.formatQuery(query)
         self.session = requests.Session()
-        self.cache_file = query + '_cache_store'
+        self.cache_file = self.formated_query + '_cache_store'
         self.cache_path = os.path.join(os.path.dirname(__file__), 'cache', self.cache_file)
         self.currentdate = datetime.now()
         self.headers = extra.visitinfo
         root = os.getcwd()
-        self.query_path = os.path.join(root, query)
+        self.query_path = os.path.join(root, self.formated_query)
         if not os.path.exists(self.query_path):
             os.makedirs(self.query_path)
         os.chdir(self.query_path)
         logging.info(f'Initialized scraper for query: {query}')
     
+    def formatQuery(self, query):
+        '''
+        Replaces non-Latin characters with '-' and cleans up extra '-' symbols
+        :param query: The input query string.
+        :return: The cleaned query string.
+        '''
+        # Replace non-Latin characters with '-'
+        cleaned_query = re.sub(r'[^a-zA-Z0-9]', '-', query)
+        # Replace multiple '-' with a single '-'
+        cleaned_query = re.sub(r'[-]+', '-', cleaned_query)
+        # Remove '-' from the start and end of the query
+        cleaned_query = cleaned_query.strip('-')
+        return cleaned_query
+
     def getCache(self):
         '''
         Loads cached data from the cache file or initializes an empty cache if none is found
         :params: none
         :return: none
         '''
         try:
             with open(self.cache_path, 'r', encoding='utf-8') as f:
                 f.seek(0)
                 self.cache = json.load(f)
             logging.info(f'Loaded cached data from: {self.cache_path}')
-        except Exception:
+        except Exception as ex:
             self.cache = {}
-            logging.info(f'Loaded cached data from: {self.cache_path}')
+            logging.info(f'Loaded empty cache. Exception: {ex}')
         self.newQuery()
 
     def updateCache(self):
         '''
         Updates the cache with the current page list and date and writes it to the cache file
         :params: none
         :return: none
@@ -87,88 +103,89 @@
         '''
         Iterates through a range of dates to fetch pages using the search query, appending valid pages to the pagelist
         :params: none
         :return: none
         '''
         delta = self.end_date - self.start_date
 
-        logging.info(f'Indexing "{self.input_query}" pages...')
+        logging.info(f'Indexing "{self.formated_query}" pages...')
         self.outer_pbar = tqdm(
                 total=delta.days,
-                desc=f'Indexing "{self.input_query}" pages',
+                desc=f'Indexing "{self.formated_query}" pages',
                 unit=' page',
                 # position=0,
                 leave=False
         )
 
         def fetch_page(start_date):
             index = 1
             while True:
                 formatted_date = start_date.strftime('%m-%d')
-                search_query = [self.input_query, formatted_date]
+                search_query = [self.formated_query, formatted_date]
 
                 if index > 1:
                     search_query.append(str(index))
 
                 try:
                     data = self.getJSON('-'.join(search_query))
                     if data['ok']:
                         self.pagelist.append(data)
                         index += 1
-                        logging.info(f'Successfully fetched page data for {search_query}')
                     else:
                         self.outer_pbar.update()
                         break
                 except Exception as ex:
                     logging.error(f'Error at {search_query}: {ex}')
 
         with concurrent.futures.ThreadPoolExecutor(max_workers=workers) as executor:
             dates_range = [self.start_date + timedelta(days=i) for i in range(delta.days)]
             list(executor.map(fetch_page, dates_range))
 
+        logging.info(f'Successfully fetched pages list for "{self.formated_query}"')
         self.outer_pbar.close()
 
     def getJSON(self, search_query):
         '''
         Sends an HTTP request to the Telegraph API to fetch page data for a given search query
         :params: search_query (str) - The search query for a single page
         :return: JSON response from the API
         '''
         try:
             result = self.session.get(
                 f'https://api.telegra.ph/getPage/{search_query}?return_content=true',
                 headers=self.headers
             ).json()
-            logging.info(f'Successfully fetched JSON data for {search_query}')
         except Exception as ex:
             logging.error(f'Error while processing {search_query}: {ex}')
             result = None
         return result
 
     def getImages(self):
         '''
         Downloads images from indexed pages and stores them in corresponding directories
         :params: none
         :return: none
         '''
         self.outer_pbar = tqdm(
                 total=len(self.pagelist),
-                desc=f'Scrapping images from "{self.input_query}" pages',
+                desc=f'Scrapping images from "{self.formated_query}" pages',
                 unit=' page',
                 # position=0,
                 leave=True
             )
+        
+        logging.info(f'Scrapping images from "{self.formated_query}" pages...')
+
         for page in self.pagelist:
             page_name = page['result']['path']
             page_path = os.path.join(self.query_path, page_name)
             if not os.path.exists(page_path):
                 os.makedirs(page_path)
             os.chdir(page_path)
 
-            logging.info(f'Extracting image URLs from page "{page_name}"...')
             try:
                 self.getImageList(page)
             except Exception as ex:
                 logging.error(f'Error while processing page "{page_name}": {ex}')
 
             self.inner_pbar = tqdm(
                 total=len(self.imagelist),
@@ -183,24 +200,24 @@
                         image_url = f'https://telegra.ph/file/{file}'
                         image_response = requests.get(
                             image_url,
                             stream=True,
                             headers=self.headers
                         )
                         f.write(image_response.content)
-                    logging.info(f'Downloaded {index} of {len(self.imagelist)} images from page "{page_name}"')
                 except requests.RequestException as ex:
                     logging.error(f'Error downloading image {file}: {ex}')
                 except Exception as ex:
                     logging.error(f'Error while processing image {file}: {ex}')
                 self.inner_pbar.update()
             self.inner_pbar.close()
 
             self.outer_pbar.update()
         self.outer_pbar.close()
+        logging.info(f'Successfully scraped images for "{self.formated_query}"')
             
     
     def getImageList(self, page):
         '''
         Extracts image URLs from the content of a given page and populates the imagelist
         :params: page (dict) - JSON data for a telegraph page
         :return: None
@@ -216,40 +233,43 @@
         '''
         Gathers all text content from indexed pages and saves it into text files
         :params: none
         :return: none
         '''
         self.outer_pbar = tqdm(
                 total=len(self.pagelist),
-                desc=f'Scrapping text from "{self.input_query}" pages',
+                desc=f'Scrapping text from "{self.formated_query}" pages',
                 unit=' page',
                 # position=0,
                 leave=True
             )
+        
+        logging.info(f'Scrapping text from "{self.formated_query}" pages...')
+
         for page in self.pagelist:
             page_name = page['result']['path']
             page_path = os.path.join(self.query_path, page_name)
             if not os.path.exists(page_path):
                 os.makedirs(page_path)
             os.chdir(page_path)
             
-            logging.info(f'Collecting text from page "{page_name}"...')
             try:
                 self.getTextList(page)
             except Exception as ex:
                 logging.error(f'Error while processing page "{page_name}": {ex}')
 
             self.textlist = list(filter(None, self.textlist)) #filter empty values from textlist
             if self.textlist:
                 with open('text.txt', 'w', encoding='utf-8') as f:
                     for line in self.textlist:
                         f.write(f'{line}\n')
 
             self.outer_pbar.update()
         self.outer_pbar.close()
+        logging.info(f'Successfully scraped text for "{self.formated_query}"')
 
     def getTextList(self, page):
         '''
         Collects all text from a given page and stores it in the textlist
         :params: page (dict) - JSON data for a telegraph page.
         :return: None
         '''
@@ -264,39 +284,42 @@
         '''
         Gathers all links from indexed pages and saves them into a text file
         :params: page (dict) - JSON data for a telegraph page.
         :return: none
         '''
         self.outer_pbar = tqdm(
                 total=len(self.pagelist),
-                desc=f'Scrapping links from "{self.input_query}" pages',
+                desc=f'Scrapping links from "{self.formated_query}" pages',
                 unit=' page',
                 #position=0,
                 leave=True
             )
+        
+        logging.info(f'Scrapping links from "{self.formated_query}" pages..."')
+
         for page in self.pagelist:
             page_name = page['result']['path']
             page_path = os.path.join(self.query_path, page_name)
             if not os.path.exists(page_path):
                 os.makedirs(page_path)
             os.chdir(page_path)
             
-            logging.info(f'Collecting links from page "{page_name}"...')
             try:
                 self.getLinksList(page)
             except Exception as ex:
                 logging.error(f'Error while processing page "{page_name}": {ex}')
 
             if self.linklist:
                 with open('links.txt', 'w', encoding='utf-8') as f:
                     for line in self.linklist:
                         f.write(f'{line}\n')
 
             self.outer_pbar.update()
         self.outer_pbar.close()
+        logging.info(f'Successfully scraped links for "{self.formated_query}"')
 
     def getLinksList(self, page):
         '''
         Collects all links from a given page and stores them in the linklist
         :params: page (dict) - JSON data for a telegraph page.
         :return: none
         '''
@@ -313,59 +336,59 @@
         '''
         Collects and stores the URLs of all indexed pages in a text file
         :params: none
         :return: none
         '''
         links = [page['result']['url'] for page in self.pagelist]
         os.chdir(self.query_path)
-        with open(f'{self.input_query}.txt', 'w') as f:
+        with open(f'{self.formated_query}.txt', 'w') as f:
             for link in links:
                 f.write(f'{link}\n')
 
     def filterSpam(self):
         '''
         Filters out pages with authors in a predefined spam list from the pagelist
         :params: none
         :return: none
         '''
-        logging.info(f'Filtering out spam pages...')
         for page in self.pagelist[:]:
             author_name = page.get('result', {}).get('author_name')
             if author_name is not None and author_name in extra.spam:
-                self.pagelist.remove(page)     
+                self.pagelist.remove(page)
+        logging.info(f'Filtered out spam pages')
 
     def filterText(self, min_length, max_length):
         '''
         Filters pages based on text length criteria, removing pages falling outside the specified range
         :params: min_length (int, optional) - Minimum text length; max_length (int, optional) - Maximum text length.
         :return: none
         '''
-        logging.info(f'Filtering pages based on text length criteria...')
         for page in self.pagelist[:]:
             self.getTextList(page)
             length = sum(len(string) for string in self.textlist)
             if min_length is not None and length < min_length:
                 self.pagelist.remove(page)
             elif max_length is not None and length > max_length:
                 self.pagelist.remove(page)
+        logging.info(f'Filtered out pages based on text length criteria')
 
 def parser():
     '''
     Returns the parser arguments
     :params: none
     :return: parser.parse_args() object
     '''
     parser = argparse.ArgumentParser(
         description='Scrapes a telegraph pages from a specified search query'
     )
     main_grp = parser.add_argument_group('Main parameters')
     main_grp.add_argument('QUERY', help = 'Single query given as a positional argument', type=str, nargs = '?')
-    main_grp.add_argument('-i', '--input-file', help = '<INPUT_FILE> text file containing the target list. Ex: list.txt')
-    main_grp.add_argument('-o', '--output-directory', help = '<OUTPUT_DIRECTORY> (optional): query output directory (default "./Scraper/")',
-                          default=os.path.join(os.getcwd(), 'Scraper'))
+    main_grp.add_argument('-i', '--input-file', help = '<INPUT_FILE> text file (each query separated by new line) containing the target list. Ex: list.txt')
+    main_grp.add_argument('-o', '--output-directory', help = '<OUTPUT_DIRECTORY> (optional): query output directory (default "./Scraper results/")',
+                          default=os.path.join(os.getcwd(), 'Scraper results'))
     main_grp.add_argument('-w', '--workers', help = '<WORKERS> (optional): number of parallel execution workers (default 4)', type=int, default = 4)
 
     output_grp = parser.add_argument_group('Output parameters')
     output_grp.add_argument('-I', '--images', action='store_true', help = 'collect all images on indexed pages')
     output_grp.add_argument('-T', '--text', action='store_true', help='collect all text on indexed pages')
     output_grp.add_argument('-L', '--links', action='store_true', help = 'collect all links on indexed pages')
     output_grp.add_argument('-max', help='<MAX> (optional): Filter pages with text length greater than defined value.', type=int, nargs='?')
@@ -375,20 +398,21 @@
 
 def deleteEmptyFolders(directory):
     '''
     Recursively delete empty folders starting from the given directory.
     :params: The directory to start searching for empty folders.
     :return: none
     '''
+    logging.info(f'Deleting empty folders...')
+
     for root, dirs, files in os.walk(directory, topdown=False):
         for dir_name in dirs:
             folder_path = os.path.join(root, dir_name)
             if not os.listdir(folder_path):
                 os.rmdir(folder_path)
-                logging.info(f'Deleted empty folder: {folder_path}')
 
 def main():
     args = parser()
     
     if args.input_file != None:
         with open(args.input_file,'rb') as file:
             try:
@@ -411,24 +435,30 @@
         scraper.getCache()
         scraper.indexQuery(args.workers)
         scraper.updateCache()
         scraper.filterSpam()
 
         if args.min or args.max:
             scraper.filterText(args.min, args.max)
+            os.chdir(args.output_directory)
 
         if args.images:
             scraper.getImages()
+            os.chdir(args.output_directory)
         
         if args.text:
             scraper.getText()
+            os.chdir(args.output_directory)
         
         if args.links:
             scraper.getLinks()
+            os.chdir(args.output_directory)
                 
         if not (args.images or args.text or args.links):
             scraper.getPagesUrl()
     
     deleteEmptyFolders(args.output_directory)
-    
+
+    logging.info(f'Done')
+
 if __name__ == '__main__':
     main()
```

### Comparing `telegraph-scraper-1.0.4/telegraph_scraper.egg-info/PKG-INFO` & `telegraph_scraper-1.0.6/telegraph_scraper.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 2.1
-Name: telegraph-scraper
-Version: 1.0.4
-Summary: A Python scraper for Telegraph pages
-Home-page: https://github.com/solodk/telegraph-scraper
-Author: Mykola Solodky
-Author-email: solodk.m@gmail.com
-Keywords: telegraph scrape image images download
-Classifier: Development Status :: 3 - Alpha
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-License-File: LICENSE
+Metadata-Version: 2.1
+Name: telegraph-scraper
+Version: 1.0.6
+Summary: A Python scraper for Telegraph pages
+Home-page: https://github.com/solodk/telegraph-scraper
+Author: Mykola Solodky
+Author-email: solodk.m@gmail.com
+Keywords: telegraph scrape image images download
+Classifier: Development Status :: 3 - Alpha
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE
+Requires-Dist: tqdm
+Requires-Dist: requests
```

