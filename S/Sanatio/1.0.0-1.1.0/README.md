# Comparing `tmp/Sanatio-1.0.0.tar.gz` & `tmp/Sanatio-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sanatio-1.0.0.tar", last modified: Fri May 31 15:34:15 2024, max compression
+gzip compressed data, was "Sanatio-1.1.0.tar", last modified: Sun Jun  2 04:47:25 2024, max compression
```

## Comparing `Sanatio-1.0.0.tar` & `Sanatio-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 15:34:15.068648 Sanatio-1.0.0/
--rw-rw-rw-   0        0        0    11545 2024-05-30 04:29:04.000000 Sanatio-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2224 2024-05-31 15:34:15.068648 Sanatio-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1418 2024-05-30 04:29:04.000000 Sanatio-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 15:34:15.006453 Sanatio-1.0.0/Sanatio.egg-info/
--rw-rw-rw-   0        0        0     2224 2024-05-31 15:34:14.000000 Sanatio-1.0.0/Sanatio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      509 2024-05-31 15:34:14.000000 Sanatio-1.0.0/Sanatio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 15:34:14.000000 Sanatio-1.0.0/Sanatio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-31 15:34:14.000000 Sanatio-1.0.0/Sanatio.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-31 15:34:14.000000 Sanatio-1.0.0/Sanatio.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-31 15:34:15.012054 Sanatio-1.0.0/sanatio/
--rw-rw-rw-   0        0        0       61 2024-05-31 14:54:09.000000 Sanatio-1.0.0/sanatio/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 15:34:15.016050 Sanatio-1.0.0/sanatio/assets/
--rw-rw-rw-   0        0        0    25900 2024-05-30 04:29:04.000000 Sanatio-1.0.0/sanatio/assets/country.json
--rw-rw-rw-   0        0        0     1181 2024-05-30 04:29:04.000000 Sanatio-1.0.0/sanatio/assets/regex.json
--rw-rw-rw-   0        0        0    15058 2024-05-30 04:45:20.000000 Sanatio-1.0.0/sanatio/main.py
-drwxrwxrwx   0        0        0        0 2024-05-31 15:34:15.023600 Sanatio-1.0.0/sanatio/utils/
--rw-rw-rw-   0        0        0        0 2024-05-31 15:11:29.000000 Sanatio-1.0.0/sanatio/utils/__init__.py
--rw-rw-rw-   0        0        0      655 2024-05-30 04:29:04.000000 Sanatio-1.0.0/sanatio/utils/checksum.py
-drwxrwxrwx   0        0        0        0 2024-05-31 15:34:15.028883 Sanatio-1.0.0/sanatio/utils/checksum_algorithms/
--rw-rw-rw-   0        0        0        0 2024-05-31 15:11:29.000000 Sanatio-1.0.0/sanatio/utils/checksum_algorithms/__init__.py
--rw-rw-rw-   0        0        0     1318 2024-05-30 04:29:04.000000 Sanatio-1.0.0/sanatio/utils/checksum_algorithms/luhn_algorithm.py
--rw-rw-rw-   0        0        0     1741 2024-05-30 04:29:04.000000 Sanatio-1.0.0/sanatio/utils/checksum_algorithms/verhoeff_algorithm.py
--rw-rw-rw-   0        0        0      691 2024-05-30 04:29:04.000000 Sanatio-1.0.0/sanatio/utils/utils.py
--rw-rw-rw-   0        0        0       81 2024-05-31 15:34:15.073617 Sanatio-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1304 2024-05-31 14:46:18.000000 Sanatio-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 04:47:25.484885 Sanatio-1.1.0/
+-rw-rw-rw-   0        0        0    11545 2024-05-30 04:29:04.000000 Sanatio-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2282 2024-06-02 04:47:25.485883 Sanatio-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1418 2024-06-01 07:33:28.000000 Sanatio-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 04:47:25.235172 Sanatio-1.1.0/Sanatio.egg-info/
+-rw-rw-rw-   0        0        0     2282 2024-06-02 04:47:22.000000 Sanatio-1.1.0/Sanatio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      860 2024-06-02 04:47:24.000000 Sanatio-1.1.0/Sanatio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 04:47:22.000000 Sanatio-1.1.0/Sanatio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-06-02 04:47:22.000000 Sanatio-1.1.0/Sanatio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-02 04:47:22.000000 Sanatio-1.1.0/Sanatio.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 04:47:25.384557 Sanatio-1.1.0/sanatio/
+-rw-rw-rw-   0        0        0       61 2024-06-02 04:36:09.000000 Sanatio-1.1.0/sanatio/__init__.py
+-rw-rw-rw-   0        0        0      878 2024-06-02 03:26:51.000000 Sanatio-1.1.0/sanatio/array_validator.py
+drwxrwxrwx   0        0        0        0 2024-06-02 04:47:25.399326 Sanatio-1.1.0/sanatio/assets/
+-rw-rw-rw-   0        0        0    25900 2024-05-30 04:29:04.000000 Sanatio-1.1.0/sanatio/assets/country.json
+-rw-rw-rw-   0        0        0     1181 2024-06-01 05:05:22.000000 Sanatio-1.1.0/sanatio/assets/regex.json
+-rw-rw-rw-   0        0        0      819 2024-06-02 03:25:17.000000 Sanatio-1.1.0/sanatio/base_class.py
+-rw-rw-rw-   0        0        0     1984 2024-06-01 09:14:47.000000 Sanatio-1.1.0/sanatio/date_validator.py
+-rw-rw-rw-   0        0        0     2015 2024-06-01 09:14:57.000000 Sanatio-1.1.0/sanatio/document_validator.py
+-rw-rw-rw-   0        0        0      481 2024-06-01 09:15:01.000000 Sanatio-1.1.0/sanatio/email_validator.py
+-rw-rw-rw-   0        0        0     5568 2024-06-01 09:15:09.000000 Sanatio-1.1.0/sanatio/file_validator.py
+-rw-rw-rw-   0        0        0      990 2024-06-02 04:35:16.000000 Sanatio-1.1.0/sanatio/main.py
+-rw-rw-rw-   0        0        0     1071 2024-06-01 09:15:15.000000 Sanatio-1.1.0/sanatio/number_validator.py
+-rw-rw-rw-   0        0        0     4157 2024-06-01 09:03:00.000000 Sanatio-1.1.0/sanatio/other_validator.py
+-rw-rw-rw-   0        0        0     2498 2024-06-02 03:23:10.000000 Sanatio-1.1.0/sanatio/password_validator.py
+-rw-rw-rw-   0        0        0     4293 2024-06-02 04:31:57.000000 Sanatio-1.1.0/sanatio/string_validator.py
+-rw-rw-rw-   0        0        0      257 2024-06-01 08:37:57.000000 Sanatio-1.1.0/sanatio/username_validator.py
+drwxrwxrwx   0        0        0        0 2024-06-02 04:47:25.436682 Sanatio-1.1.0/sanatio/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-31 15:11:29.000000 Sanatio-1.1.0/sanatio/utils/__init__.py
+-rw-rw-rw-   0        0        0      719 2024-06-01 09:04:08.000000 Sanatio-1.1.0/sanatio/utils/checksum.py
+drwxrwxrwx   0        0        0        0 2024-06-02 04:47:25.479882 Sanatio-1.1.0/sanatio/utils/checksum_algorithms/
+-rw-rw-rw-   0        0        0        0 2024-05-31 15:11:29.000000 Sanatio-1.1.0/sanatio/utils/checksum_algorithms/__init__.py
+-rw-rw-rw-   0        0        0      852 2024-06-02 04:20:53.000000 Sanatio-1.1.0/sanatio/utils/checksum_algorithms/ean_checksum.py
+-rw-rw-rw-   0        0        0     1299 2024-06-01 09:12:45.000000 Sanatio-1.1.0/sanatio/utils/checksum_algorithms/luhn_algorithm.py
+-rw-rw-rw-   0        0        0     1743 2024-06-01 09:13:07.000000 Sanatio-1.1.0/sanatio/utils/checksum_algorithms/verhoeff_algorithm.py
+-rw-rw-rw-   0        0        0      691 2024-05-30 04:29:04.000000 Sanatio-1.1.0/sanatio/utils/utils.py
+-rw-rw-rw-   0        0        0       81 2024-06-02 04:47:25.516346 Sanatio-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1351 2024-06-01 05:29:19.000000 Sanatio-1.1.0/setup.py
```

### Comparing `Sanatio-1.0.0/LICENSE` & `Sanatio-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Sanatio-1.0.0/PKG-INFO` & `Sanatio-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: Sanatio
-Version: 1.0.0
-Home-page: https://github.com/Py-Contributors/validator.py
+Version: 1.1.0
+Summary: Simple and easy to validate data in Python
+Home-page: https://github.com/codeperfectplus/Sanatio
 Author: Deepak Raj
 Author-email: deepak008@live.com
 Project-URL: Documentation, https://pycontributors.readthedocs.io/projects/morse/en/latest/
-Project-URL: Source, https://github.com/Py-Contributors/validator.py
-Project-URL: Tracker, https://github.com/Py-Contributors/validator.py/issues
+Project-URL: Source, https://github.com/codeperfectplus/Sanatio
+Project-URL: Tracker, https://github.com/codeperfectplus/Sanatio/issues
 Keywords: audiobook
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_y2jqrwnq_/tmpb2zo_z2g_TarContainer/0/2", line 22, column 81: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_y2jqrwnq_/tmpb2zo_z2g_TarContainer/0/2", line 23, column 195: Levels of opening and closing headings don't match*

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: Sanatio Version: 1.0.0 Home-page: https://
-github.com/Py-Contributors/validator.py Author: Deepak Raj Author-email:
-deepak008@live.com Project-URL: Documentation, https://
-pycontributors.readthedocs.io/projects/morse/en/latest/ Project-URL: Source,
-https://github.com/Py-Contributors/validator.py Project-URL: Tracker, https://
-github.com/Py-Contributors/validator.py/issues Keywords: audiobook Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: Programming Language :: Python
-:: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Classifier: Intended Audience :: Developers Requires-
-Python: >=3.4 Description-Content-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: Sanatio Version: 1.1.0 Summary: Simple and easy to
+validate data in Python Home-page: https://github.com/codeperfectplus/Sanatio
+Author: Deepak Raj Author-email: deepak008@live.com Project-URL: Documentation,
+https://pycontributors.readthedocs.io/projects/morse/en/latest/ Project-URL:
+Source, https://github.com/codeperfectplus/Sanatio Project-URL: Tracker, https:
+//github.com/codeperfectplus/Sanatio/issues Keywords: audiobook Classifier:
+Development Status :: 5 - Production/Stable Classifier: Programming Language ::
+Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
+Developers Requires-Python: >=3.4 Description-Content-Type: text/markdown
+License-File: LICENSE
                              _[_w_e_b_s_i_t_e_ _t_i_t_l_e_ _i_m_a_g_e_]
        ******** ?ð??? SSaannaattiioo iiss aa llaattiinn wwoorrdd wwhhiicchh mmeeaann VVaalliiddaattiioonn ?ð??? ********
  ******** DDooccuummeenntt,, SSttrriinngg,, NNuummbbeerr,, DDaattee,, EEmmaaiill,, UUsseerrnnaammee,, PPaasssswwoorrdd VVaalliiddaattoorr ffoorr
                      PPyytthhoonn.. IInnssppiirreedd bbyy _VV_aa_ll_ii_dd_aa_tt_oo_rr_.._JJ_SS ********
 ## Installation ```bash pip install sanatio ``` ## Documentation Check out the
 [documentation](https://pycontributors.readthedocs.io/projects/sanatio/en/
 latest/) for more information. After the stable release, we will add more
```

### Comparing `Sanatio-1.0.0/README.md` & `Sanatio-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `Sanatio-1.0.0/Sanatio.egg-info/PKG-INFO` & `Sanatio-1.1.0/Sanatio.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: Sanatio
-Version: 1.0.0
-Home-page: https://github.com/Py-Contributors/validator.py
+Version: 1.1.0
+Summary: Simple and easy to validate data in Python
+Home-page: https://github.com/codeperfectplus/Sanatio
 Author: Deepak Raj
 Author-email: deepak008@live.com
 Project-URL: Documentation, https://pycontributors.readthedocs.io/projects/morse/en/latest/
-Project-URL: Source, https://github.com/Py-Contributors/validator.py
-Project-URL: Tracker, https://github.com/Py-Contributors/validator.py/issues
+Project-URL: Source, https://github.com/codeperfectplus/Sanatio
+Project-URL: Tracker, https://github.com/codeperfectplus/Sanatio/issues
 Keywords: audiobook
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_y2jqrwnq_/tmpb2zo_z2g_TarContainer/0/5", line 22, column 81: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_y2jqrwnq_/tmpb2zo_z2g_TarContainer/0/5", line 23, column 195: Levels of opening and closing headings don't match*

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: Sanatio Version: 1.0.0 Home-page: https://
-github.com/Py-Contributors/validator.py Author: Deepak Raj Author-email:
-deepak008@live.com Project-URL: Documentation, https://
-pycontributors.readthedocs.io/projects/morse/en/latest/ Project-URL: Source,
-https://github.com/Py-Contributors/validator.py Project-URL: Tracker, https://
-github.com/Py-Contributors/validator.py/issues Keywords: audiobook Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: Programming Language :: Python
-:: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Classifier: Intended Audience :: Developers Requires-
-Python: >=3.4 Description-Content-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: Sanatio Version: 1.1.0 Summary: Simple and easy to
+validate data in Python Home-page: https://github.com/codeperfectplus/Sanatio
+Author: Deepak Raj Author-email: deepak008@live.com Project-URL: Documentation,
+https://pycontributors.readthedocs.io/projects/morse/en/latest/ Project-URL:
+Source, https://github.com/codeperfectplus/Sanatio Project-URL: Tracker, https:
+//github.com/codeperfectplus/Sanatio/issues Keywords: audiobook Classifier:
+Development Status :: 5 - Production/Stable Classifier: Programming Language ::
+Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
+Developers Requires-Python: >=3.4 Description-Content-Type: text/markdown
+License-File: LICENSE
                              _[_w_e_b_s_i_t_e_ _t_i_t_l_e_ _i_m_a_g_e_]
        ******** ?ð??? SSaannaattiioo iiss aa llaattiinn wwoorrdd wwhhiicchh mmeeaann VVaalliiddaattiioonn ?ð??? ********
  ******** DDooccuummeenntt,, SSttrriinngg,, NNuummbbeerr,, DDaattee,, EEmmaaiill,, UUsseerrnnaammee,, PPaasssswwoorrdd VVaalliiddaattoorr ffoorr
                      PPyytthhoonn.. IInnssppiirreedd bbyy _VV_aa_ll_ii_dd_aa_tt_oo_rr_.._JJ_SS ********
 ## Installation ```bash pip install sanatio ``` ## Documentation Check out the
 [documentation](https://pycontributors.readthedocs.io/projects/sanatio/en/
 latest/) for more information. After the stable release, we will add more
```

### Comparing `Sanatio-1.0.0/sanatio/assets/country.json` & `Sanatio-1.1.0/sanatio/assets/country.json`

 * *Files identical despite different names*

### Comparing `Sanatio-1.0.0/sanatio/assets/regex.json` & `Sanatio-1.1.0/sanatio/assets/regex.json`

 * *Files identical despite different names*

### Comparing `Sanatio-1.0.0/sanatio/utils/checksum.py` & `Sanatio-1.1.0/sanatio/utils/checksum.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import sys
 sys.path.append('.')
 from sanatio.utils.checksum_algorithms.verhoeff_algorithm import VerhoeffAlgorithm
 from sanatio.utils.checksum_algorithms.luhn_algorithm import LuhnAlgorithm
-
-verhoeff = VerhoeffAlgorithm()
-luhn = LuhnAlgorithm()
+from sanatio.utils.checksum_algorithms.ean_checksum import EANCheckSum
 
 
 def checksum_aadhar(aadhar_number):
     """ validates aadhar number """
-    return verhoeff.verify(aadhar_number)
+    return VerhoeffAlgorithm().verify(aadhar_number)
 
 def checksum_pan(pan_number):
     """ pancard checksum """
     pass
 
 def checksum_credit_card(credit_card_number):
     """ credit card checksum """
-    return luhn.verify(credit_card_number)
-    
-    
+    return LuhnAlgorithm().verify(credit_card_number)
     
-# res = checksum_credit_card('4578423013769219')
-# print(res)
+def checksum_ean(ean_number):
+    """ ean checksum """
+    return EANCheckSum().is_valid(ean_number)
```

### Comparing `Sanatio-1.0.0/sanatio/utils/checksum_algorithms/luhn_algorithm.py` & `Sanatio-1.1.0/sanatio/utils/checksum_algorithms/luhn_algorithm.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,13 +31,11 @@
         if (total + last_digit) % 10 == 0:
             return True
         return False
     
     def verify(self, numbers: str) -> bool:
         """Verify a number using Luhn algorithm."""
         if isinstance(numbers, int):
-            number = str(numbers)
+            numbers = str(numbers)
             
         return self.__checksum(numbers)
-        
-
```

### Comparing `Sanatio-1.0.0/sanatio/utils/checksum_algorithms/verhoeff_algorithm.py` & `Sanatio-1.1.0/sanatio/utils/checksum_algorithms/verhoeff_algorithm.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,8 @@
 
     def verify(self, numbers):
         """ Verify a given number including its checksum digit """
         if isinstance(numbers, int):
             number = str(numbers)
 
         numbers = numbers.replace(' ', '')
-        return self.__checksum(numbers)
+        return self.__checksum(numbers)
```

### Comparing `Sanatio-1.0.0/sanatio/utils/utils.py` & `Sanatio-1.1.0/sanatio/utils/utils.py`

 * *Files identical despite different names*

### Comparing `Sanatio-1.0.0/setup.py` & `Sanatio-1.1.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,29 +5,29 @@
     long_description = fh.read().decode("utf-8")
 
 with open("requirements.txt", "r") as fh:
     requirements = fh.read().splitlines()
 
 setuptools.setup(
     name="Sanatio",
-    version="1.0.0",
+    version="1.1.0",
     author="Deepak Raj",
     author_email="deepak008@live.com",
-    description="",
+    description="Simple and easy to validate data in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/Py-Contributors/validator.py",
+    url="https://github.com/codeperfectplus/Sanatio",
     data_files=[('assets', glob('sanatio/assets/*'))],
     keywords="audiobook",
     install_requires=requirements,
     packages=setuptools.find_packages(),
     project_urls={"Documentation": "https://pycontributors.readthedocs.io/projects/morse/en/latest/",
-                  "Source": "https://github.com/Py-Contributors/validator.py",
-                  "Tracker": "https://github.com/Py-Contributors/validator.py/issues"},
-    classifiers=["Development Status :: 2 - Pre-Alpha",
+                  "Source": "https://github.com/codeperfectplus/Sanatio",
+                  "Tracker": "https://github.com/codeperfectplus/Sanatio/issues"},
+    classifiers=["Development Status :: 5 - Production/Stable",
                  "Programming Language :: Python :: 3",
-                 "License :: OSI Approved :: MIT License",
+                 "License :: OSI Approved :: Apache Software License",
                  "Operating System :: OS Independent",
                  "Intended Audience :: Developers"],
     python_requires=">=3.4",
     include_package_data=True,
 )
```

