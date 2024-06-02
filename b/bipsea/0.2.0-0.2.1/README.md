# Comparing `tmp/bipsea-0.2.0.tar.gz` & `tmp/bipsea-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bipsea-0.2.0.tar", last modified: Sat Jun  1 03:25:30 2024, max compression
+gzip compressed data, was "bipsea-0.2.1.tar", last modified: Sat Jun  1 14:56:12 2024, max compression
```

## Comparing `bipsea-0.2.0.tar` & `bipsea-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-01 03:25:30.089135 bipsea-0.2.0/
--rw-r--r--   0 akarve     (501) staff       (20)    11356 2024-05-26 11:53:50.000000 bipsea-0.2.0/LICENSE.md
--rw-r--r--   0 akarve     (501) staff       (20)      778 2024-06-01 03:25:30.088907 bipsea-0.2.0/PKG-INFO
--rw-r--r--   0 akarve     (501) staff       (20)     9770 2024-05-26 22:37:27.000000 bipsea-0.2.0/README.md
--rw-r--r--   0 akarve     (501) staff       (20)       38 2024-06-01 03:25:30.089174 bipsea-0.2.0/setup.cfg
--rw-r--r--   0 akarve     (501) staff       (20)     1285 2024-06-01 03:17:12.000000 bipsea-0.2.0/setup.py
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-01 03:25:30.085508 bipsea-0.2.0/src/
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-01 03:25:30.087234 bipsea-0.2.0/src/bipsea/
--rw-r--r--   0 akarve     (501) staff       (20)        0 2024-05-26 22:08:44.000000 bipsea-0.2.0/src/bipsea/__init__.py
--rw-r--r--   0 akarve     (501) staff       (20)     8116 2024-05-26 22:08:44.000000 bipsea-0.2.0/src/bipsea/bip32.py
--rw-r--r--   0 akarve     (501) staff       (20)     3669 2024-05-26 22:08:44.000000 bipsea-0.2.0/src/bipsea/bip32types.py
--rw-r--r--   0 akarve     (501) staff       (20)     4602 2024-06-01 01:30:56.000000 bipsea-0.2.0/src/bipsea/bip39.py
--rw-r--r--   0 akarve     (501) staff       (20)     6794 2024-06-01 03:17:12.000000 bipsea-0.2.0/src/bipsea/bip85.py
--rw-r--r--   0 akarve     (501) staff       (20)     7854 2024-06-01 03:17:12.000000 bipsea-0.2.0/src/bipsea/bipsea.py
--rw-r--r--   0 akarve     (501) staff       (20)    13116 2024-05-26 22:39:38.000000 bipsea-0.2.0/src/bipsea/english.txt
--rw-r--r--   0 akarve     (501) staff       (20)      760 2024-06-01 03:17:12.000000 bipsea-0.2.0/src/bipsea/util.py
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-01 03:25:30.088702 bipsea-0.2.0/src/bipsea.egg-info/
--rw-r--r--   0 akarve     (501) staff       (20)      778 2024-06-01 03:25:30.000000 bipsea-0.2.0/src/bipsea.egg-info/PKG-INFO
--rw-r--r--   0 akarve     (501) staff       (20)      484 2024-06-01 03:25:30.000000 bipsea-0.2.0/src/bipsea.egg-info/SOURCES.txt
--rw-r--r--   0 akarve     (501) staff       (20)        1 2024-06-01 03:25:30.000000 bipsea-0.2.0/src/bipsea.egg-info/dependency_links.txt
--rw-r--r--   0 akarve     (501) staff       (20)       45 2024-06-01 03:25:30.000000 bipsea-0.2.0/src/bipsea.egg-info/entry_points.txt
--rw-r--r--   0 akarve     (501) staff       (20)       26 2024-06-01 03:25:30.000000 bipsea-0.2.0/src/bipsea.egg-info/requires.txt
--rw-r--r--   0 akarve     (501) staff       (20)        7 2024-06-01 03:25:30.000000 bipsea-0.2.0/src/bipsea.egg-info/top_level.txt
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-01 03:25:30.088456 bipsea-0.2.0/tests/
--rw-r--r--   0 akarve     (501) staff       (20)     1319 2024-05-26 22:36:53.000000 bipsea-0.2.0/tests/test_bip32.py
--rw-r--r--   0 akarve     (501) staff       (20)     3138 2024-06-01 01:30:56.000000 bipsea-0.2.0/tests/test_bip39.py
--rw-r--r--   0 akarve     (501) staff       (20)     5010 2024-06-01 01:30:56.000000 bipsea-0.2.0/tests/test_bip85.py
--rw-r--r--   0 akarve     (501) staff       (20)     7088 2024-06-01 03:17:12.000000 bipsea-0.2.0/tests/test_cli.py
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-01 14:56:12.388344 bipsea-0.2.1/
+-rw-r--r--   0 akarve     (501) staff       (20)    11356 2024-05-26 11:53:50.000000 bipsea-0.2.1/LICENSE.md
+-rw-r--r--   0 akarve     (501) staff       (20)      778 2024-06-01 14:56:12.388123 bipsea-0.2.1/PKG-INFO
+-rw-r--r--   0 akarve     (501) staff       (20)     9770 2024-05-26 22:37:27.000000 bipsea-0.2.1/README.md
+-rw-r--r--   0 akarve     (501) staff       (20)       38 2024-06-01 14:56:12.388382 bipsea-0.2.1/setup.cfg
+-rw-r--r--   0 akarve     (501) staff       (20)     1285 2024-06-01 03:17:12.000000 bipsea-0.2.1/setup.py
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-01 14:56:12.385143 bipsea-0.2.1/src/
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-01 14:56:12.386570 bipsea-0.2.1/src/bipsea/
+-rw-r--r--   0 akarve     (501) staff       (20)        0 2024-05-26 22:08:44.000000 bipsea-0.2.1/src/bipsea/__init__.py
+-rw-r--r--   0 akarve     (501) staff       (20)     8024 2024-06-01 14:56:06.000000 bipsea-0.2.1/src/bipsea/bip32.py
+-rw-r--r--   0 akarve     (501) staff       (20)     3669 2024-05-26 22:08:44.000000 bipsea-0.2.1/src/bipsea/bip32types.py
+-rw-r--r--   0 akarve     (501) staff       (20)     4578 2024-06-01 14:56:06.000000 bipsea-0.2.1/src/bipsea/bip39.py
+-rw-r--r--   0 akarve     (501) staff       (20)     6794 2024-06-01 03:17:12.000000 bipsea-0.2.1/src/bipsea/bip85.py
+-rw-r--r--   0 akarve     (501) staff       (20)     7545 2024-06-01 14:56:06.000000 bipsea-0.2.1/src/bipsea/bipsea.py
+-rw-r--r--   0 akarve     (501) staff       (20)    13116 2024-05-26 22:39:38.000000 bipsea-0.2.1/src/bipsea/english.txt
+-rw-r--r--   0 akarve     (501) staff       (20)      760 2024-06-01 14:56:06.000000 bipsea-0.2.1/src/bipsea/util.py
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-01 14:56:12.387930 bipsea-0.2.1/src/bipsea.egg-info/
+-rw-r--r--   0 akarve     (501) staff       (20)      778 2024-06-01 14:56:12.000000 bipsea-0.2.1/src/bipsea.egg-info/PKG-INFO
+-rw-r--r--   0 akarve     (501) staff       (20)      484 2024-06-01 14:56:12.000000 bipsea-0.2.1/src/bipsea.egg-info/SOURCES.txt
+-rw-r--r--   0 akarve     (501) staff       (20)        1 2024-06-01 14:56:12.000000 bipsea-0.2.1/src/bipsea.egg-info/dependency_links.txt
+-rw-r--r--   0 akarve     (501) staff       (20)       45 2024-06-01 14:56:12.000000 bipsea-0.2.1/src/bipsea.egg-info/entry_points.txt
+-rw-r--r--   0 akarve     (501) staff       (20)       26 2024-06-01 14:56:12.000000 bipsea-0.2.1/src/bipsea.egg-info/requires.txt
+-rw-r--r--   0 akarve     (501) staff       (20)        7 2024-06-01 14:56:12.000000 bipsea-0.2.1/src/bipsea.egg-info/top_level.txt
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-01 14:56:12.387767 bipsea-0.2.1/tests/
+-rw-r--r--   0 akarve     (501) staff       (20)     1319 2024-05-26 22:36:53.000000 bipsea-0.2.1/tests/test_bip32.py
+-rw-r--r--   0 akarve     (501) staff       (20)     3138 2024-06-01 01:30:56.000000 bipsea-0.2.1/tests/test_bip39.py
+-rw-r--r--   0 akarve     (501) staff       (20)     5010 2024-06-01 01:30:56.000000 bipsea-0.2.1/tests/test_bip85.py
+-rw-r--r--   0 akarve     (501) staff       (20)     7088 2024-06-01 03:17:12.000000 bipsea-0.2.1/tests/test_cli.py
```

### Comparing `bipsea-0.2.0/LICENSE.md` & `bipsea-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bipsea-0.2.0/PKG-INFO` & `bipsea-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipsea
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python implementation of BIP 85 (and BIP 32)
 Author: Aneesh Karve
 Author-email: bonded_metals_0u@icloud.com
 Project-URL: Source, https://github.com/akarve/bipsea
 Keywords: Bitcoin BIP85 BIP32 cryptography
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `bipsea-0.2.0/README.md` & `bipsea-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bipsea-0.2.0/setup.py` & `bipsea-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.2.0/src/bipsea/bip32.py` & `bipsea-0.2.1/src/bipsea/bip32.py`

 * *Files 19% similar despite different names*

```diff
@@ -43,31 +43,31 @@
 def derive_key(master: ExtendedKey, path: List[str], private: bool):
     indexes = [segment_to_index(s) for s in path[1:]]
     key_chain = [
         (
             master
             if indexes or private
             else N(
-                master.data,
-                master.chain_code,
-                master.child_number,
+                private_key=master.data,
+                chain_code=master.chain_code,
+                child_number=master.child_number,
                 depth=bytes(1),
                 finger=master.finger,
                 version=VERSIONS[master.get_network()]["public"],
             )
         )
     ]
     for depth, (index, _) in enumerate(indexes, 1):
         parent = key_chain[-1]
         key_chain.append(
             CKDpriv(
-                parent.data,
-                parent.chain_code,
-                index,
-                depth.to_bytes(1, "big"),
+                private_key=parent.data,
+                chain_code=parent.chain_code,
+                child_number=index,
+                depth=depth.to_bytes(1, "big"),
                 version=parent.version,
             )
         )
     # only use N() or CKDpub() if public at the highest depth (final segment)
     # so as to avoid complex, hard-to-read flow control with look-ahead since once
     # we harden a child anywhere in the chain we can't recover the private key
     if private or not indexes:
@@ -85,65 +85,63 @@
                 finger=parent.finger,
                 version=VERSIONS[parent.get_network()]["public"],
             )
         else:
             # CKDpub() is a true derivation so go to grandparent as parent
             grand_parent = key_chain[-2]
             return CKDpub(
-                to_public_key(grand_parent.data),
-                grand_parent.chain_code,
-                parent.child_number,
-                parent.depth,
+                public_key=to_public_key(grand_parent.data),
+                chain_code=grand_parent.chain_code,
+                child_number=parent.child_number,
+                depth=parent.depth,
                 finger=parent.finger,
                 version=VERSIONS[parent.get_network()]["public"],
             )
 
 
 def CKDpriv(
-    secret_key: bytes,
+    private_key: bytes,
     chain_code: bytes,
     child_number: int,
     depth: bytes,
     version: bytes,
 ) -> ExtendedKey:
     hardened = child_number >= TYPED_CHILD_KEY_COUNT
-    secret_int = int.from_bytes(secret_key[1:], "big")
+    secret_int = int.from_bytes(private_key[1:], "big")
     data = (
-        secret_key
+        private_key
         if hardened
         else VerifyingKey.from_public_point(
             secret_int * SECP256k1.generator,
             curve=SECP256k1,
         ).to_string("compressed")
     )
-    while True:
-        derived = hmac_sha512(
-            key=chain_code, data=data + child_number.to_bytes(4, "big")
-        )
-        if validate_derived_key(derived):
-            break
-        else:
-            child_number += 1
-            if hardened:
-                assert child_number < 2**32
-            else:
-                assert child_number < TYPED_CHILD_KEY_COUNT
-
+    derived = hmac_sha512(
+        key=chain_code,
+        data=data + child_number.to_bytes(4, "big"),
+    )
+    # BIP-32: In case parse256(IL) ≥ n or ki = 0, the resulting key is invalid
+    # (Note: this has probability lower than 1 in 2**127.)
+    parse_256_IL = int.from_bytes(derived[:32], "big")
     child_key_int = (
-        int.from_bytes(derived[:32], "big") + int.from_bytes(secret_key, "big")
+        parse_256_IL + int.from_bytes(private_key, "big")
     ) % SECP256k1.order
+    if (parse_256_IL >= SECP256k1.order) or not child_key_int:
+        raise ValueError(
+            f"Rare invalid child key. Retry with the next child index: {child_number} + 1."
+        )
     child_key = bytes(1) + child_key_int.to_bytes(32, "big")
 
     return ExtendedKey(
-        version=version,
-        depth=depth,
-        finger=fingerprint(secret_key),
-        child_number=child_number.to_bytes(4, "big"),
-        chain_code=derived[32:],
         data=child_key,
+        chain_code=derived[32:],
+        child_number=child_number.to_bytes(4, "big"),
+        depth=depth,
+        finger=fingerprint(private_key),
+        version=version,
     )
 
 
 def N(
     private_key: bytes,
     chain_code: bytes,
     child_number: bytes,
@@ -151,20 +149,20 @@
     finger: bytes,
     version: bytes,
 ) -> ExtendedKey:
     """neuter a private key into the public one (no derivation per se)
     pass in the fingerprint since it is from the parent (which we don't have)
     """
     return ExtendedKey(
-        version=version,
+        data=to_public_key(private_key),
+        chain_code=chain_code,
+        child_number=child_number,
         depth=depth,
         finger=finger,
-        child_number=child_number,
-        chain_code=chain_code,
-        data=to_public_key(private_key),
+        version=version,
     )
 
 
 def CKDpub(
     public_key: bytes,
     chain_code: bytes,
     child_number: bytes,
@@ -173,44 +171,42 @@
     version: bytes,
 ) -> ExtendedKey:
     child_number_int = int.from_bytes(child_number, "big")
     if child_number_int >= TYPED_CHILD_KEY_COUNT:
         raise ValueError(f"Cannot call CKDpub() for hardened child: {child_number_int}")
 
     parent_key = VerifyingKey.from_string(public_key, curve=SECP256k1).pubkey.point
-    while True:
-        derived = hmac_sha512(key=chain_code, data=public_key + child_number)
-        derived_key = int.from_bytes(derived[:32], "big")
-        derived_chain_code = derived[32:]
-        if derived_key >= SECP256k1.order:
-            child_number += 1
-            assert child_number < TYPED_CHILD_KEY_COUNT, "exhausted available children"
-            continue
-        child_point = SECP256k1.generator * derived_key + parent_key
-        try:
-            child_key = VerifyingKey.from_public_point(
-                child_point,
-                curve=SECP256k1,
-            ).to_string("compressed")
-        except MalformedPointError as m:
-            # Is this in fact how we detect the point at infinity?
-            warnings.warning(
-                "Point at infinity? Retrying with higher child_number in CKDPub()", m
-            )
-            child_number += 1
-            continue
-        break
+
+    derived = hmac_sha512(
+        key=chain_code,
+        data=public_key + child_number,
+    )
+    parse_256_IL = int.from_bytes(derived[:32], "big")
+    # BIP-39: In case parse256(IL) ≥ n or Ki is the point at infinity, the resulting
+    # key is invalid, and one should proceed with the next value for i.
+    if parse_256_IL >= SECP256k1.order:
+        raise ValueError(f"Invalid key. Try next child index: {child_number} + 1.")
+    try:
+        child_key = VerifyingKey.from_public_point(
+            SECP256k1.generator * parse_256_IL + parent_key,
+            curve=SECP256k1,
+        ).to_string("compressed")
+    except MalformedPointError as mal:
+        # TODO: Is this in fact how to detect the point at infinity?
+        raise ValueError(
+            f"Invalid key (point at infinity?). Try next child index: {child_number} + 1."
+        ) from mal
 
     return ExtendedKey(
-        version=version,
+        data=child_key,
+        chain_code=derived[32:],
+        child_number=child_number_int.to_bytes(4, "big"),
         depth=depth,
+        version=version,
         finger=finger,
-        child_number=child_number_int.to_bytes(4, "big"),
-        chain_code=derived_chain_code,
-        data=child_key,
     )
 
 
 def to_public_key(secret_key: bytes, as_point=False):
     """returns compressed ecdsa public key"""
     # ecdsa from_/to_string are actually from_/to_bytes b/c of some kind of
     # Python 2 hangover
@@ -246,17 +242,7 @@
     fingerprint = ripemd.digest()[:4]
 
     return fingerprint
 
 
 def hmac_sha512(key: bytes, data: bytes) -> bytes:
     return hmac.new(key=key, msg=data, digestmod="sha512").digest()
-
-
-def validate_derived_key(key: bytes) -> bool:
-    assert len(key) == 64
-    secret_key = key[:32]
-    secret_int = int.from_bytes(secret_key, "big")
-    if (secret_int == 0) or (secret_int >= SECP256k1.order):
-        return False
-
-    return True
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bipsea-0.2.0/src/bipsea/bip32types.py` & `bipsea-0.2.1/src/bipsea/bip32types.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.2.0/src/bipsea/bip39.py` & `bipsea-0.2.1/src/bipsea/bip39.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,20 @@
         if user_entropy
         else secrets.randbits(n_entropy_bits)
     )
     difference = int_entropy.bit_length() - n_entropy_bits
     if difference > 0:
         int_entropy >>= difference
     elif difference <= -8:
-        warn_stretching(difference + n_entropy_bits, n_entropy_bits)
+        warnings.warn(
+            (
+                f"Warning: {difference + n_entropy_bits} bits in, {n_entropy_bits} bits out."
+                " Input more entropy?"
+            )
+        )
 
     entropy_hash = hashlib.sha256(int_entropy.to_bytes(n_entropy_bits // 8, "big"))
     int_checksum = int.from_bytes(entropy_hash.digest(), "big") >> (
         8 * entropy_hash.digest_size - n_checksum_bits  # cut hash down to CS-many bits
     )
     int_entropy_cs = (int_entropy << n_checksum_bits) + int_checksum  # shift CS bits in
 
@@ -124,12 +129,7 @@
 
     return pbkdf2_hmac(
         hash_name="sha512",
         password=mnemonic_nfkd,
         salt=salt_nfkd,
         iterations=iterations,
     )
-
-
-def warn_stretching(given: int, target: int):
-    msg = f"Warning: {given} bits in, {target} bits out. Input more entropy."
-    warnings.warn(msg)
```

### Comparing `bipsea-0.2.0/src/bipsea/bip85.py` & `bipsea-0.2.1/src/bipsea/bip85.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.2.0/src/bipsea/bipsea.py` & `bipsea-0.2.1/src/bipsea/bipsea.py`

 * *Files 5% similar despite different names*

```diff
@@ -247,20 +247,14 @@
         output = apply_85(derived, path)["application"]
     click.echo(output)
 
 
 cli.add_command(bip85_cmd)
 
 
-# TODO From BIP32: In case parse256(IL) is 0 or ≥ n, the resulting key is invalid,
-# and one should proceed with the next value for i. (Note: this has probability lower than 1 in 2127.)
-# they say hard fail but does 39? i say let's hard fail in these cases because otherwise
-# you are modifying the path?
-
-
 def check_range(number: int, application: str):
     (min, max) = RANGES[application]
     if not (min <= number <= max):
         raise click.BadOptionUsage(
             option_name="--number",
             message=f"out of range; try [{min}, {max}] for {application}",
         )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bipsea-0.2.0/src/bipsea/english.txt` & `bipsea-0.2.1/src/bipsea/english.txt`

 * *Files identical despite different names*

### Comparing `bipsea-0.2.0/src/bipsea/util.py` & `bipsea-0.2.1/src/bipsea/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """constants and utilities"""
 
 import binascii
 import logging
 from hashlib import pbkdf2_hmac
 from unicodedata import normalize as unicode_normalize
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __app_name__ = "bipsea"
 
 FORMAT = "utf-8"
 NFKD = "NFKD"
 LOGGER = __app_name__
```

### Comparing `bipsea-0.2.0/src/bipsea.egg-info/PKG-INFO` & `bipsea-0.2.1/src/bipsea.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipsea
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python implementation of BIP 85 (and BIP 32)
 Author: Aneesh Karve
 Author-email: bonded_metals_0u@icloud.com
 Project-URL: Source, https://github.com/akarve/bipsea
 Keywords: Bitcoin BIP85 BIP32 cryptography
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `bipsea-0.2.0/tests/test_bip32.py` & `bipsea-0.2.1/tests/test_bip32.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.2.0/tests/test_bip39.py` & `bipsea-0.2.1/tests/test_bip39.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.2.0/tests/test_bip85.py` & `bipsea-0.2.1/tests/test_bip85.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.2.0/tests/test_cli.py` & `bipsea-0.2.1/tests/test_cli.py`

 * *Files identical despite different names*

