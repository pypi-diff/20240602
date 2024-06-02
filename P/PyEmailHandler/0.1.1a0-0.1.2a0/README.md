# Comparing `tmp/PyEmailHandler-0.1.1a0.tar.gz` & `tmp/pyemailhandler-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEmailHandler-0.1.1a0.tar", last modified: Thu Mar 14 11:28:21 2024, max compression
+gzip compressed data, was "pyemailhandler-0.1.2a0.tar", last modified: Sun Jun  2 14:50:19 2024, max compression
```

## Comparing `PyEmailHandler-0.1.1a0.tar` & `pyemailhandler-0.1.2a0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 11:28:21.895538 PyEmailHandler-0.1.1a0/
--rw-rw-rw-   0        0        0     1763 2024-03-14 11:28:21.893536 PyEmailHandler-0.1.1a0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-14 11:28:21.885538 PyEmailHandler-0.1.1a0/PyEmailHandler/
--rw-rw-rw-   0        0        0       40 2024-03-06 11:52:36.000000 PyEmailHandler-0.1.1a0/PyEmailHandler/__init__.py
--rw-rw-rw-   0        0        0     7128 2024-03-14 11:26:26.000000 PyEmailHandler-0.1.1a0/PyEmailHandler/mailer.py
--rw-rw-rw-   0        0        0     1351 2024-03-06 17:20:43.000000 PyEmailHandler-0.1.1a0/PyEmailHandler/tools.py
--rw-rw-rw-   0        0        0     1175 2024-03-14 11:27:03.000000 PyEmailHandler-0.1.1a0/PyEmailHandler/version.py
-drwxrwxrwx   0        0        0        0 2024-03-14 11:28:21.892537 PyEmailHandler-0.1.1a0/PyEmailHandler.egg-info/
--rw-rw-rw-   0        0        0     1763 2024-03-14 11:28:21.000000 PyEmailHandler-0.1.1a0/PyEmailHandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-03-14 11:28:21.000000 PyEmailHandler-0.1.1a0/PyEmailHandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 11:28:21.000000 PyEmailHandler-0.1.1a0/PyEmailHandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-03-14 11:28:21.000000 PyEmailHandler-0.1.1a0/PyEmailHandler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1101 2024-03-07 07:11:25.000000 PyEmailHandler-0.1.1a0/README.md
--rw-rw-rw-   0        0        0     1049 2024-03-07 10:46:04.000000 PyEmailHandler-0.1.1a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-14 11:28:21.895538 PyEmailHandler-0.1.1a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 14:50:19.149360 pyemailhandler-0.1.2a0/
+-rw-rw-rw-   0        0        0     1763 2024-06-02 14:50:19.147360 pyemailhandler-0.1.2a0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-02 14:50:19.139360 pyemailhandler-0.1.2a0/PyEmailHandler/
+-rw-rw-rw-   0        0        0       40 2024-03-06 11:52:36.000000 pyemailhandler-0.1.2a0/PyEmailHandler/__init__.py
+-rw-rw-rw-   0        0        0     7300 2024-06-02 14:11:29.000000 pyemailhandler-0.1.2a0/PyEmailHandler/mailer.py
+-rw-rw-rw-   0        0        0     1351 2024-03-06 17:20:43.000000 pyemailhandler-0.1.2a0/PyEmailHandler/tools.py
+-rw-rw-rw-   0        0        0     1175 2024-06-02 14:03:58.000000 pyemailhandler-0.1.2a0/PyEmailHandler/version.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:50:19.146360 pyemailhandler-0.1.2a0/PyEmailHandler.egg-info/
+-rw-rw-rw-   0        0        0     1763 2024-06-02 14:50:19.000000 pyemailhandler-0.1.2a0/PyEmailHandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-06-02 14:50:19.000000 pyemailhandler-0.1.2a0/PyEmailHandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 14:50:19.000000 pyemailhandler-0.1.2a0/PyEmailHandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-06-02 14:50:19.000000 pyemailhandler-0.1.2a0/PyEmailHandler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1101 2024-03-07 07:11:25.000000 pyemailhandler-0.1.2a0/README.md
+-rw-rw-rw-   0        0        0     1049 2024-06-02 14:02:27.000000 pyemailhandler-0.1.2a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 14:50:19.149360 pyemailhandler-0.1.2a0/setup.cfg
```

### Comparing `PyEmailHandler-0.1.1a0/PKG-INFO` & `pyemailhandler-0.1.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyEmailHandler
-Version: 0.1.1a0
+Version: 0.1.2a0
 Summary: A simplified tool for mailing services
 Author-email: Kinuseka <support@kinuseka.us>
 Project-URL: homepage, https://gitlab.com/brewedcoffee/PyEmailHandler
 Keywords: python,sockets,networking,communication
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `PyEmailHandler-0.1.1a0/PyEmailHandler/mailer.py` & `pyemailhandler-0.1.2a0/PyEmailHandler/mailer.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     def start_connection(self):
         if self.protocol == 'ssl':
             self.imap = imaplib.IMAP4_SSL(self.imap_address, self.port, ssl_context=self.context, timeout=30)
             retcode, message_indices = self.imap.login(user=self.username, password=self.password)
         elif self.protocol == 'starttls':
             self.imap = imaplib.IMAP4(self.imap_address, self.port, timeout=30)
             self.imap.starttls(ssl_context=self.context)
-            retcode, message_indices = self.smtp.login(user=self.username, password=self.password)
+            retcode, message_indices = self.imap.login(user=self.username, password=self.password)
         if retcode != "OK":
             raise ValueError("IMAP login failed! Return code: '" + cast(retcode, str) + "'.")
     
     def get_folder(self, name):
         _retcode, msg_count = self.imap.select(name)
         try:
             self._recheck(_retcode)
@@ -141,29 +141,32 @@
         if not self._is_connected():
             self.start_connection()
 
     def _is_connected(self):
         try:
             # Send a NOOP command to keep the connection alive
             status, response = self.imap.noop()
-        except Exception as e:
-            print("Error occurred while keeping connection alive:", e)
+        except imaplib.IMAP4.error as e:
             status = None
         return True if status == "OK" else False
     
     def close(self):
-        self.smtp.close()
-
+        self.imap.close()
 
-    def delete_mail(self, mail, _trash_folder = 'Trash'):
+    def delete_mail(self, mail: Message, temporary = False, _trash_folder = 'Trash'):
         '''
         Deletes a mail
+        - @self
+        - mail:  Message mail
+        - temporary:  Move to trash folder instead of instantly deleting it
+        - _trash_folder:  Name of the trash folder
         '''
-        _retcode, message = self.imap.uid('COPY', mail['mailserver_email_uid'], _trash_folder)
-        self._recheck(_retcode, _reason=message)
+        if temporary:
+            _retcode, message = self.imap.uid('COPY', mail['mailserver_email_uid'], _trash_folder)
+            self._recheck(_retcode, _reason=message)
         self.imap.uid('STORE', mail['mailserver_email_uid'], '+FLAGS', '(\Deleted)')
         self.imap.expunge()
 
     def _recheck(self, _retcode, _reason = None):
         if _retcode != "OK":
             if _reason:
                 raise ValueError(f"An error occured due to: {_reason}")
```

### Comparing `PyEmailHandler-0.1.1a0/PyEmailHandler/tools.py` & `pyemailhandler-0.1.2a0/PyEmailHandler/tools.py`

 * *Files identical despite different names*

### Comparing `PyEmailHandler-0.1.1a0/PyEmailHandler/version.py` & `pyemailhandler-0.1.2a0/PyEmailHandler/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #     (1, 1, 2, 'dev', 0) => "1.1.2.dev0"
 #     (1, 1, 2, 'alpha', 1) => "1.1.2a1"
 #     (1, 2, 0, 'beta', 2) => "1.2b2"
 #     (1, 2, 0, 'rc', 4) => "1.2rc4"
 #     (1, 2, 0, 'final', 0) => "1.2.0"
 # Taken from CFSession
 
-__version_info__ = (0, 1, 1, 'alpha', 0)
+__version_info__ = (0, 1, 2, 'alpha', 0)
 
 def _get_version(version_info, explicit_versioning = True):
     " Returns a PEP 440-compliant version number from version_info. "
     assert len(version_info) == 5
     assert version_info[3] in ('dev', 'alpha', 'beta', 'rc', 'final')
 
     if explicit_versioning:
```

### Comparing `PyEmailHandler-0.1.1a0/PyEmailHandler.egg-info/PKG-INFO` & `pyemailhandler-0.1.2a0/PyEmailHandler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyEmailHandler
-Version: 0.1.1a0
+Version: 0.1.2a0
 Summary: A simplified tool for mailing services
 Author-email: Kinuseka <support@kinuseka.us>
 Project-URL: homepage, https://gitlab.com/brewedcoffee/PyEmailHandler
 Keywords: python,sockets,networking,communication
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `PyEmailHandler-0.1.1a0/README.md` & `pyemailhandler-0.1.2a0/README.md`

 * *Files identical despite different names*

### Comparing `PyEmailHandler-0.1.1a0/pyproject.toml` & `pyemailhandler-0.1.2a0/pyproject.toml`

 * *Files identical despite different names*

