# Comparing `tmp/pyasynctracker-0.1.0.tar.gz` & `tmp/pyasynctracker-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyasynctracker-0.1.0.tar", max compression
+gzip compressed data, was "pyasynctracker-0.2.0.tar", max compression
```

## Comparing `pyasynctracker-0.1.0.tar` & `pyasynctracker-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2024-06-02 16:30:46.765970 pyasynctracker-0.1.0/LICENSE
--rw-r--r--   0        0        0     3427 2024-06-02 16:30:46.765970 pyasynctracker-0.1.0/README.md
--rw-r--r--   0        0        0      610 2024-06-02 16:30:46.765970 pyasynctracker-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-06-02 16:30:46.765970 pyasynctracker-0.1.0/src/pyasynctracker/__init__.py
--rw-r--r--   0        0        0    10416 2024-06-02 16:30:46.765970 pyasynctracker-0.1.0/src/pyasynctracker/scraper.py
--rw-r--r--   0        0        0      851 2024-06-02 16:30:46.765970 pyasynctracker-0.1.0/src/pyasynctracker/utils.py
--rw-r--r--   0        0        0     4056 1970-01-01 00:00:00.000000 pyasynctracker-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-06-02 18:28:52.073845 pyasynctracker-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3508 2024-06-02 18:28:52.073845 pyasynctracker-0.2.0/README.md
+-rw-r--r--   0        0        0      610 2024-06-02 18:28:52.073845 pyasynctracker-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      102 2024-06-02 18:28:52.073845 pyasynctracker-0.2.0/src/pyasynctracker/__init__.py
+-rw-r--r--   0        0        0    10614 2024-06-02 18:28:52.073845 pyasynctracker-0.2.0/src/pyasynctracker/scraper.py
+-rw-r--r--   0        0        0      851 2024-06-02 18:28:52.073845 pyasynctracker-0.2.0/src/pyasynctracker/utils.py
+-rw-r--r--   0        0        0     4137 1970-01-01 00:00:00.000000 pyasynctracker-0.2.0/PKG-INFO
```

### Comparing `pyasynctracker-0.1.0/LICENSE` & `pyasynctracker-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyasynctracker-0.1.0/README.md` & `pyasynctracker-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ## Usage
 
 ### Scrape Info Hashes
 
 Scrape torrent data asynchronously from multiple trackers for given info hashes.
 
 ```python
-from pyasynctracker.scraper import scrape_info_hashes
+from pyasynctracker import scrape_info_hashes
 
 async def main():
     info_hashes = ["2b66980093bc11806fab50cb3cb41835b95a0362", "706440a3f8fdac91591d6007c4314f3274317f85"]
     trackers = [
         "http://bttracker.debian.org:6969/announce",
         "udp://tracker.openbittorrent.com:80/announce",
         "udp://tracker.opentrackr.org:1337/announce",
@@ -55,15 +55,15 @@
 ```
 
 ### Batch Scrape Info Hashes
 
 Batch scrape info hashes based on a structured input of info hashes and their respective trackers. This function groups info hashes by their associated trackers and performs scraping in batches.
 
 ```python
-from pyasynctracker.scraper import batch_scrape_info_hashes
+from pyasynctracker import batch_scrape_info_hashes
 
 async def main():
     data_list = [
         ("2b66980093bc11806fab50cb3cb41835b95a0362", ["http://bttracker.debian.org:6969/announce"]),
         ("706440a3f8fdac91591d6007c4314f3274317f85", ["udp://tracker.opentrackr.org:1337/announce"])
     ]
 
@@ -76,19 +76,21 @@
 ```
 
 ### Find Maximum Seeders
 
 Analyze the results from scraping functions to find the maximum number of seeders for each info hash.
 
 ```python
-from pyasynctracker.utils import find_max_seeders
+from pyasynctracker import find_max_seeders
 
 # Assuming 'results' is populated from the scrape_info_hashes or batch_scrape_info_hashes functions
 max_seeders = find_max_seeders(results)
 print(max_seeders)
+
+# {'2b66980093bc11806fab50cb3cb41835b95a0362': 1022, '706440a3f8fdac91591d6007c4314f3274317f85': 168}
 ```
 
 ## Contributing
 
 Contributions to PyAsyncTracker are welcome! Please fork the repository and submit pull requests with your proposed changes. Ensure to follow coding standards and write tests for new features.
 
 ## License
```

### Comparing `pyasynctracker-0.1.0/pyproject.toml` & `pyasynctracker-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyAsyncTracker"
-version = "0.1.0"
+version = "0.2.0"
 description = "Asynchronous scraping library for torrent trackers."
 authors = ["Mohamed Zumair <mhdzumair@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
```

### Comparing `pyasynctracker-0.1.0/src/pyasynctracker/scraper.py` & `pyasynctracker-0.2.0/src/pyasynctracker/scraper.py`

 * *Files 6% similar despite different names*

```diff
@@ -195,70 +195,67 @@
     transaction_id = random.randint(0, 0xFFFFFFFF)
     # Use 'II' for unsigned ints instead of 'ii' to handle the full range of possible transaction_ids
     buf = struct.pack("!qII", connection_id, action, transaction_id)
     return buf, transaction_id
 
 
 def udp_create_scrape_request(connection_id, info_hashes):
-    max_hashes_per_request = (
-        74  # This number might need to be adjusted based on other packet content.
-    )
-    if len(info_hashes) > max_hashes_per_request:
-        raise ValueError(
-            f"Too many info hashes for a single UDP packet: {len(info_hashes)} provided, maximum is {max_hashes_per_request}. Consider splitting the request."
-        )
-
-    action = 2  # action (2 = scrape)
+    base_size = 16  # Basic overhead for connection ID, action, and transaction ID in bytes
+    max_packet_size = 508  # Maximum safe UDP packet size in bytes
+    action = 2  # Action code for 'scrape'
     transaction_id = random.randint(0, 0xFFFFFFFF)
-    buf = struct.pack("!qII", connection_id, action, transaction_id)
+
+    # Start assembling the packet
+    packet = struct.pack("!qII", connection_id, action, transaction_id)
+    included_hashes = []
+
     for info_hash in info_hashes:
-        buf += binascii.a2b_hex(info_hash)
-        if len(buf) > 508:  # Keeping the packet size within a safe limit
-            raise ValueError("Packet size exceeds the safe UDP packet size limit.")
+        hash_bytes = binascii.a2b_hex(info_hash)
+        # Check if adding this hash would exceed the max packet size considering base_size
+        if len(packet) + len(hash_bytes) + base_size > max_packet_size:
+            break  # Stop adding hashes if the packet would become too large
+        packet += hash_bytes
+        included_hashes.append(info_hash)
 
-    return buf, transaction_id
+    if not included_hashes:
+        raise ValueError("No hashes could be included in the packet without exceeding the size limit.")
+
+    return packet, included_hashes, transaction_id
 
 
 async def scrape_udp(parsed_tracker: parse.ParseResult, info_hashes: list[str], timeout: int):
     con_req, con_trans_id = udp_create_connection_request()
     results = {}
-    max_hashes_per_request = 74
+    remaining_hashes = list(info_hashes)  # Start with all hashes
 
     async def on_con_response(data):
         connection_id = struct.unpack_from("!q", data, 8)[0]
-        # Split info_hashes into manageable chunks if necessary
-        for i in range(0, len(info_hashes), max_hashes_per_request):
-            current_hashes = info_hashes[i: i + max_hashes_per_request]
+        nonlocal remaining_hashes  # Reference the non-local variable defined in outer scope
+
+        while remaining_hashes:
             try:
-                scrape_req, scrape_trans_id = udp_create_scrape_request(
-                    connection_id, current_hashes
-                )
-                await send_udp_request(
-                    parsed_tracker, scrape_req, on_scrape_response, on_error, timeout
-                )
+                scrape_req, included_hashes, trans_id = udp_create_scrape_request(connection_id, remaining_hashes)
+                remaining_hashes = [h for h in remaining_hashes if h not in included_hashes]  # Update remaining_hashes safely
+                await send_udp_request(parsed_tracker, scrape_req, lambda response: on_scrape_response(response, included_hashes), on_error, timeout)
             except ValueError as e:
                 logging.error(f"Error creating UDP scrape request: {e}")
+                break
 
-    async def on_scrape_response(data):
-        offset = 8  # skip action and transaction id
+    async def on_scrape_response(data, included_hashes):
+        offset = 8  # Skip action and transaction ID
         expected_length_per_hash = 12  # 4 bytes each for seeds, completed, leeches
         local_results = {}
 
-        # Ensure each hash has enough data in the buffer to unpack
-        for info_hash in info_hashes:
+        for info_hash in included_hashes:
             if offset + expected_length_per_hash > len(data):
-                logging.error(
-                    f"Not enough data to unpack results for hash: {info_hash}. Data length: {len(data)}, required: {offset + expected_length_per_hash}"
-                )
-                break
+                logging.error(f"Not enough data to unpack results for hash: {info_hash}. Data length: {len(data)}, required: {offset + expected_length_per_hash}")
+                continue  # Use continue to process next hashes if possible
 
             seeds, completed, leeches = struct.unpack_from("!iii", data, offset)
-            readable_hash = binascii.b2a_hex(binascii.a2b_hex(info_hash)).decode(
-                "utf-8"
-            )
+            readable_hash = binascii.b2a_hex(binascii.a2b_hex(info_hash)).decode("utf-8")
             local_results[readable_hash] = {
                 "tracker_url": parsed_tracker.geturl(),
                 "seeders": seeds,
                 "peers": leeches,
                 "complete": completed,
             }
             offset += expected_length_per_hash
```

### Comparing `pyasynctracker-0.1.0/src/pyasynctracker/utils.py` & `pyasynctracker-0.2.0/src/pyasynctracker/utils.py`

 * *Files identical despite different names*

### Comparing `pyasynctracker-0.1.0/PKG-INFO` & `pyasynctracker-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAsyncTracker
-Version: 0.1.0
+Version: 0.2.0
 Summary: Asynchronous scraping library for torrent trackers.
 License: MIT
 Author: Mohamed Zumair
 Author-email: mhdzumair@gmail.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -38,15 +38,15 @@
 ## Usage
 
 ### Scrape Info Hashes
 
 Scrape torrent data asynchronously from multiple trackers for given info hashes.
 
 ```python
-from pyasynctracker.scraper import scrape_info_hashes
+from pyasynctracker import scrape_info_hashes
 
 async def main():
     info_hashes = ["2b66980093bc11806fab50cb3cb41835b95a0362", "706440a3f8fdac91591d6007c4314f3274317f85"]
     trackers = [
         "http://bttracker.debian.org:6969/announce",
         "udp://tracker.openbittorrent.com:80/announce",
         "udp://tracker.opentrackr.org:1337/announce",
@@ -73,15 +73,15 @@
 ```
 
 ### Batch Scrape Info Hashes
 
 Batch scrape info hashes based on a structured input of info hashes and their respective trackers. This function groups info hashes by their associated trackers and performs scraping in batches.
 
 ```python
-from pyasynctracker.scraper import batch_scrape_info_hashes
+from pyasynctracker import batch_scrape_info_hashes
 
 async def main():
     data_list = [
         ("2b66980093bc11806fab50cb3cb41835b95a0362", ["http://bttracker.debian.org:6969/announce"]),
         ("706440a3f8fdac91591d6007c4314f3274317f85", ["udp://tracker.opentrackr.org:1337/announce"])
     ]
 
@@ -94,19 +94,21 @@
 ```
 
 ### Find Maximum Seeders
 
 Analyze the results from scraping functions to find the maximum number of seeders for each info hash.
 
 ```python
-from pyasynctracker.utils import find_max_seeders
+from pyasynctracker import find_max_seeders
 
 # Assuming 'results' is populated from the scrape_info_hashes or batch_scrape_info_hashes functions
 max_seeders = find_max_seeders(results)
 print(max_seeders)
+
+# {'2b66980093bc11806fab50cb3cb41835b95a0362': 1022, '706440a3f8fdac91591d6007c4314f3274317f85': 168}
 ```
 
 ## Contributing
 
 Contributions to PyAsyncTracker are welcome! Please fork the repository and submit pull requests with your proposed changes. Ensure to follow coding standards and write tests for new features.
 
 ## License
```

