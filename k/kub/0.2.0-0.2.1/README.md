# Comparing `tmp/kub-0.2.0.tar.gz` & `tmp/kub-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kub-0.2.0.tar", max compression
+gzip compressed data, was "kub-0.2.1.tar", max compression
```

## Comparing `kub-0.2.0.tar` & `kub-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-08-26 02:01:01.716187 kub-0.2.0/LICENSE
--rw-r--r--   0        0        0       46 2023-08-26 02:01:01.716427 kub-0.2.0/README.md
--rw-r--r--   0        0        0      327 2024-05-25 00:43:38.171638 kub-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-26 12:23:34.125444 kub-0.2.0/src/kub/__init__.py
--rw-r--r--   0        0        0     7904 2024-05-25 00:43:02.784088 kub-0.2.0/src/kub/kubUtilities.py
--rw-r--r--   0        0        0      440 1970-01-01 00:00:00.000000 kub-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-26 02:01:01.716187 kub-0.2.1/LICENSE
+-rw-r--r--   0        0        0       46 2023-08-26 02:01:01.716427 kub-0.2.1/README.md
+-rw-r--r--   0        0        0      327 2024-06-02 14:03:46.377767 kub-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-26 12:23:34.125444 kub-0.2.1/src/kub/__init__.py
+-rw-r--r--   0        0        0     8930 2024-06-02 14:01:28.973911 kub-0.2.1/src/kub/kubUtilities.py
+-rw-r--r--   0        0        0      440 1970-01-01 00:00:00.000000 kub-0.2.1/PKG-INFO
```

### Comparing `kub-0.2.0/LICENSE` & `kub-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kub-0.2.0/src/kub/kubUtilities.py` & `kub-0.2.1/src/kub/kubUtilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -198,14 +198,37 @@
     async def retrieve_monthly_usage(self):
         """Retrieve all usage for the current month"""
         async with Http() as self.http:
             await self.retrieve_usage(KUBUtilityTypes.ELECTRICITY)
             await self.retrieve_usage(KUBUtilityTypes.GAS)
             await self.retrieve_usage(KUBUtilityTypes.WATER)
         self.http = None
+        return self.usage
+
+    async def retrieve_usage_by_range(
+        self,
+        start_date: str = datetime.today().strftime("%Y-%m-%d"),
+        end_date: str = datetime.today().strftime("%Y-%m-%d"),
+    ):
+        """Retrieve all usage for the current month"""
+        async with Http() as self.http:
+            await self.retrieve_usage(KUBUtilityTypes.ELECTRICITY, start_date, end_date)
+            await self.retrieve_usage(KUBUtilityTypes.GAS, start_date, end_date)
+            await self.retrieve_usage(KUBUtilityTypes.WATER, start_date, end_date)
+        self.http = None
+        return self.usage
+
+    async def retrieve_monthly_summary(self):
+        """Retrieve summary of usage for the current month"""
+        if self.usage is None:
+            async with Http() as self.http:
+                await self.retrieve_usage(KUBUtilityTypes.ELECTRICITY)
+                await self.retrieve_usage(KUBUtilityTypes.GAS)
+                await self.retrieve_usage(KUBUtilityTypes.WATER)
+            self.http = None
         return self.monthly_total
 
     async def get_usage_by_datetime(self, usage_record: datetime = datetime.now()):
         """Retrieve usage by datetime"""
         await self.retrieve_monthly_usage()
         elec = (
             self.usage.get("electricity")
```

