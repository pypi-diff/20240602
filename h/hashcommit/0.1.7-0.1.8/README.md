# Comparing `tmp/hashcommit-0.1.7.tar.gz` & `tmp/hashcommit-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashcommit-0.1.7.tar", last modified: Fri May 31 16:31:27 2024, max compression
+gzip compressed data, was "hashcommit-0.1.8.tar", last modified: Sun Jun  2 10:06:56 2024, max compression
```

## Comparing `hashcommit-0.1.7.tar` & `hashcommit-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:31:27.697664 hashcommit-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-31 16:31:20.000000 hashcommit-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-31 16:31:27.697664 hashcommit-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-31 16:31:20.000000 hashcommit-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:31:27.693664 hashcommit-0.1.7/hashcommit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 16:31:20.000000 hashcommit-0.1.7/hashcommit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-31 16:31:20.000000 hashcommit-0.1.7/hashcommit/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-31 16:31:20.000000 hashcommit-0.1.7/hashcommit/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-31 16:31:20.000000 hashcommit-0.1.7/hashcommit/git.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 16:31:20.000000 hashcommit-0.1.7/hashcommit/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-31 16:31:20.000000 hashcommit-0.1.7/hashcommit/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-31 16:31:20.000000 hashcommit-0.1.7/hashcommit/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 16:31:20.000000 hashcommit-0.1.7/hashcommit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:31:27.697664 hashcommit-0.1.7/hashcommit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-31 16:31:27.000000 hashcommit-0.1.7/hashcommit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-31 16:31:27.000000 hashcommit-0.1.7/hashcommit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 16:31:27.000000 hashcommit-0.1.7/hashcommit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 16:31:27.000000 hashcommit-0.1.7/hashcommit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 16:31:27.000000 hashcommit-0.1.7/hashcommit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 16:31:27.697664 hashcommit-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-31 16:31:20.000000 hashcommit-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:31:27.697664 hashcommit-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-31 16:31:20.000000 hashcommit-0.1.7/tests/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-31 16:31:20.000000 hashcommit-0.1.7/tests/test_empty_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-31 16:31:20.000000 hashcommit-0.1.7/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-31 16:31:20.000000 hashcommit-0.1.7/tests/test_existing_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:06:56.055196 hashcommit-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-02 10:06:47.000000 hashcommit-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-06-02 10:06:56.055196 hashcommit-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-06-02 10:06:47.000000 hashcommit-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:06:56.055196 hashcommit-0.1.8/hashcommit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:06:47.000000 hashcommit-0.1.8/hashcommit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-06-02 10:06:47.000000 hashcommit-0.1.8/hashcommit/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-06-02 10:06:47.000000 hashcommit-0.1.8/hashcommit/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-06-02 10:06:47.000000 hashcommit-0.1.8/hashcommit/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-02 10:06:47.000000 hashcommit-0.1.8/hashcommit/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-06-02 10:06:47.000000 hashcommit-0.1.8/hashcommit/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-06-02 10:06:47.000000 hashcommit-0.1.8/hashcommit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-02 10:06:47.000000 hashcommit-0.1.8/hashcommit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:06:56.055196 hashcommit-0.1.8/hashcommit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-06-02 10:06:56.000000 hashcommit-0.1.8/hashcommit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-06-02 10:06:56.000000 hashcommit-0.1.8/hashcommit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 10:06:56.000000 hashcommit-0.1.8/hashcommit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-02 10:06:56.000000 hashcommit-0.1.8/hashcommit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-02 10:06:56.000000 hashcommit-0.1.8/hashcommit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 10:06:56.055196 hashcommit-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-06-02 10:06:47.000000 hashcommit-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:06:56.055196 hashcommit-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-06-02 10:06:47.000000 hashcommit-0.1.8/tests/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-06-02 10:06:47.000000 hashcommit-0.1.8/tests/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-06-02 10:06:47.000000 hashcommit-0.1.8/tests/test_empty_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-06-02 10:06:47.000000 hashcommit-0.1.8/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-06-02 10:06:47.000000 hashcommit-0.1.8/tests/test_existing_repo.py
```

### Comparing `hashcommit-0.1.7/LICENSE` & `hashcommit-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.7/PKG-INFO` & `hashcommit-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashcommit
-Version: 0.1.7
+Version: 0.1.8
 Summary: A tool to generate a Git commit with a specific hash part.
 Home-page: https://github.com/wozniakpl/hashcommit
 Author: Bartosz Woźniak
 Author-email: bwozniakdev@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hashcommit-0.1.7/README.md` & `hashcommit-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.7/hashcommit/args.py` & `hashcommit-0.1.8/hashcommit/args.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.7/hashcommit/commit.py` & `hashcommit-0.1.8/hashcommit/commit.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     result = run_subprocess(args)
     return result.stdout.decode("utf-8").strip()
 
 
 def amend_a_commit(
     timestamp: str,
     tree_hash: str,
-    parent_hash: str,
+    parent_hash: Optional[str],
     content: str,
     preserve_author: bool,
     related_commit_hash: str,
 ) -> None:
     """Amend the last commit with new content."""
     new_commit_hash = run_commit_tree(
         tree_hash=tree_hash,
@@ -208,15 +208,17 @@
         timestamp=timestamp,
         head_hash=parent_hash,
         preserve_author=preserve_author,
         related_commit_hash=commit_hash,
     )
 
     logging.debug(f"Replacing {commit_hash} with {new_commit_hash}")
-    subprocess.run(["git", "replace", commit_hash, new_commit_hash, "--force"], check=True)
+    subprocess.run(
+        ["git", "replace", commit_hash, new_commit_hash, "--force"], check=True
+    )
 
     logging.debug(f"Rebasing onto {new_commit_hash}")
     subprocess.run(
         ["git", "rebase", "--onto", new_commit_hash, commit_hash, "HEAD"], check=True
     )
 
     logging.debug(f"Deleting {commit_hash} replacement")
```

### Comparing `hashcommit-0.1.7/hashcommit/git.py` & `hashcommit-0.1.8/hashcommit/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,23 +74,24 @@
     try:
         result = run_subprocess(["git", "rev-parse", "HEAD"])
         return result.stdout.decode("utf-8").strip()
     except subprocess.CalledProcessError:
         return None
 
 
-def get_parent_head_hash() -> str:
+def get_parent_head_hash() -> Optional[str]:
     try:
         result = run_subprocess(["git", "rev-parse", "HEAD^"])
         value = result.stdout.decode("utf-8").strip()
         if not value:
             raise ValueError("Empty HEAD^ hash")
         return value
     except subprocess.CalledProcessError:
-        raise ValueError("Failed to get HEAD^ hash")
+        # raise ValueError("Failed to get HEAD^ hash")
+        return None
 
 
 def will_commits_be_signed() -> bool:
     result = run_subprocess(["git", "config", "commit.gpgSign"], check=False)
     return result.returncode == 0 and result.stdout.decode("utf-8").strip() == "true"
```

### Comparing `hashcommit-0.1.7/hashcommit/main.py` & `hashcommit-0.1.8/hashcommit/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .commit import (
     create_a_commit_with_hash,
     overwrite_a_commit_with_hash,
     overwrite_and_rebase,
 )
 from .git import does_repo_have_any_commits, is_in_git_repo
 from .logging import configure_logging
+from .utils import run_subprocess
 from .version import VERSION
 
 
 def main() -> int:
     args: HashCommitArgs = parse_args()
     configure_logging(args.verbose)
     logging.info(f"Args: {args}")
@@ -67,13 +68,16 @@
             )
     except KeyboardInterrupt:
         print("\nProcess interrupted by user")
         return 3
     except RuntimeError as e:
         print(f"Error: {e}", file=sys.stderr)
         return 2
+    finally:
+        logging.info("Running git garbage collection")
+        run_subprocess(["git", "gc", "--prune=now"])
 
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `hashcommit-0.1.7/hashcommit.egg-info/PKG-INFO` & `hashcommit-0.1.8/hashcommit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashcommit
-Version: 0.1.7
+Version: 0.1.8
 Summary: A tool to generate a Git commit with a specific hash part.
 Home-page: https://github.com/wozniakpl/hashcommit
 Author: Bartosz Woźniak
 Author-email: bwozniakdev@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hashcommit-0.1.7/setup.py` & `hashcommit-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.7/tests/test_args.py` & `hashcommit-0.1.8/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.7/tests/test_errors.py` & `hashcommit-0.1.8/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `hashcommit-0.1.7/tests/test_existing_repo.py` & `hashcommit-0.1.8/tests/test_existing_repo.py`

 * *Files identical despite different names*

