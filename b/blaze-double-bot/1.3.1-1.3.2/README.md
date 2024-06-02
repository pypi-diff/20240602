# Comparing `tmp/blaze_double_bot-1.3.1.tar.gz` & `tmp/blaze_double_bot-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaze_double_bot-1.3.1.tar", last modified: Sun Jun  2 18:19:01 2024, max compression
+gzip compressed data, was "blaze_double_bot-1.3.2.tar", last modified: Sun Jun  2 19:20:52 2024, max compression
```

## Comparing `blaze_double_bot-1.3.1.tar` & `blaze_double_bot-1.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 18:19:01.660783 blaze_double_bot-1.3.1/
--rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-1.3.1/LICENSE
--rw-rw-rw-   0        0        0     3573 2024-06-02 18:19:01.657463 blaze_double_bot-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     3076 2024-05-27 01:18:02.000000 blaze_double_bot-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 18:19:01.525707 blaze_double_bot-1.3.1/blaze_double_bot/
--rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-1.3.1/blaze_double_bot/__init__.py
--rw-rw-rw-   0        0        0    12551 2024-06-02 18:16:40.000000 blaze_double_bot-1.3.1/blaze_double_bot/bot.py
-drwxrwxrwx   0        0        0        0 2024-06-02 18:19:01.652071 blaze_double_bot-1.3.1/blaze_double_bot.egg-info/
--rw-rw-rw-   0        0        0     3573 2024-06-02 18:18:59.000000 blaze_double_bot-1.3.1/blaze_double_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-06-02 18:18:59.000000 blaze_double_bot-1.3.1/blaze_double_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 18:18:59.000000 blaze_double_bot-1.3.1/blaze_double_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 18:18:59.000000 blaze_double_bot-1.3.1/blaze_double_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-06-02 18:18:59.000000 blaze_double_bot-1.3.1/blaze_double_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 18:19:01.660783 blaze_double_bot-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      600 2024-06-02 18:18:22.000000 blaze_double_bot-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:20:52.108680 blaze_double_bot-1.3.2/
+-rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0     3573 2024-06-02 19:20:52.092974 blaze_double_bot-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3076 2024-05-27 01:18:02.000000 blaze_double_bot-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 19:20:51.924411 blaze_double_bot-1.3.2/blaze_double_bot/
+-rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-1.3.2/blaze_double_bot/__init__.py
+-rw-rw-rw-   0        0        0    13388 2024-06-02 19:06:19.000000 blaze_double_bot-1.3.2/blaze_double_bot/bot.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:20:52.085833 blaze_double_bot-1.3.2/blaze_double_bot.egg-info/
+-rw-rw-rw-   0        0        0     3573 2024-06-02 19:20:50.000000 blaze_double_bot-1.3.2/blaze_double_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-06-02 19:20:50.000000 blaze_double_bot-1.3.2/blaze_double_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 19:20:50.000000 blaze_double_bot-1.3.2/blaze_double_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 19:20:50.000000 blaze_double_bot-1.3.2/blaze_double_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-06-02 19:20:50.000000 blaze_double_bot-1.3.2/blaze_double_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 19:20:52.110099 blaze_double_bot-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      600 2024-06-02 19:20:19.000000 blaze_double_bot-1.3.2/setup.py
```

### Comparing `blaze_double_bot-1.3.1/LICENSE` & `blaze_double_bot-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-1.3.1/PKG-INFO` & `blaze_double_bot-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 1.3.1
+Version: 1.3.2
 Summary: This Python library automates the betting process on the Blaze Double
 Author: ror74559
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `blaze_double_bot-1.3.1/README.md` & `blaze_double_bot-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-1.3.1/blaze_double_bot/bot.py` & `blaze_double_bot-1.3.2/blaze_double_bot/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,14 +200,29 @@
 
 ''')
 
     def wait_for_next_round(self):
         while True:
             try:
                 self.driver.find_element(By.CLASS_NAME, 'time-left').find_element(By.TAG_NAME, 'span').text
+                return True
+            except:
+                pass
+
+        while True:
+            try:
+                self.driver.find_element(By.CLASS_NAME, 'time-left').find_element(By.TAG_NAME, 'span').text
+                
+            except:
+                break
+    def wait_for_result(self):
+        while True:
+            try:
+                self.driver.find_element(By.CLASS_NAME, 'time-left').find_element(By.TAG_NAME, 'span').text
+                
             except:
                 break
 
         while True:
             try:
                 self.driver.find_element(By.CLASS_NAME, 'time-left').find_element(By.TAG_NAME, 'span').text
                 return True
@@ -225,24 +240,32 @@
                         size,color = self.strategy(history)
                         if color:
                             self.choose_color(color)
                             self.place_bet(self.bet_amount)
                             print(self.get_text('Betting strategy -> '),[self.get_color(c) for c in history[:size][::-1]])
                             print()
                             self.print_bet(color)
-                            self.wait_for_next_round()
+                            self.wait_for_result()
+                            #self.wait_for_next_round()
                             #sleep(1)
                             history = self.get_history_api()[:size][::-1]
                             self.current_balance = self.get_balance()
                             for m in range(self.martingale):
                                 
                                 if history[-1] != self.color_dict[color] and self.stop_loss <= self.current_balance <= self.stop_win and self.current_balance - self.bet_amount >= 0:
                                     self.place_bet((2**(m+1)) * self.bet_amount)
-                                    print(f'Gale {m + 1} -> ',[self.get_color(c) for c in history],f'$ {(2**(m+1)) * self.bet_amount}')
-                                    self.wait_for_next_round()
+                                    print(f'Gale {m + 1
+                                          
+                                          
+                                          
+                                          
+                                          
+                                          } -> ',[self.get_color(c) for c in history],f'$ {(2**(m+1)) * self.bet_amount}')
+                                    self.wait_for_result()
+                                    #self.wait_for_next_round()
                                     #sleep(1)
                                     history = self.get_history_api()[:size][::-1]
                                     self.current_balance = self.get_balance()
                                     
                             self.print_bet_result(history, color)
                             sleep(8)
                             self.current_balance = self.get_balance()
```

### Comparing `blaze_double_bot-1.3.1/blaze_double_bot.egg-info/PKG-INFO` & `blaze_double_bot-1.3.2/blaze_double_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 1.3.1
+Version: 1.3.2
 Summary: This Python library automates the betting process on the Blaze Double
 Author: ror74559
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `blaze_double_bot-1.3.1/setup.py` & `blaze_double_bot-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 with open('README.md', 'r') as f:
           readme =f.read()
 
 setup(
     name='blaze_double_bot',
     licence='MIT License',
-    version='1.3.1',
+    version='1.3.2',
     author='ror74559',
     long_description=readme,
     long_description_content_type='text/markdown',
     author_email='ror74559@gmail.com',
     keywords='blaze double bot',
     description='This Python library automates the betting process on the Blaze Double',
     packages=['blaze_double_bot'],
```

