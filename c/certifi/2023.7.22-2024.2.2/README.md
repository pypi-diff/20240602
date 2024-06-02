# Comparing `tmp/certifi-2023.7.22.tar.gz` & `tmp/certifi-2024.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certifi-2023.7.22.tar", last modified: Sat Jul 22 08:39:21 2023, max compression
+gzip compressed data, was "certifi-2024.2.2.tar", last modified: Fri Feb  2 01:21:27 2024, max compression
```

## Comparing `certifi-2023.7.22.tar` & `certifi-2024.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cory       (502) staff       (20)        0 2023-07-22 08:39:21.704566 certifi-2023.7.22/
--rw-r--r--   0 cory       (502) staff       (20)     1052 2022-07-20 11:27:58.000000 certifi-2023.7.22/LICENSE
--rw-r--r--   0 cory       (502) staff       (20)      119 2022-05-23 19:19:32.000000 certifi-2023.7.22/MANIFEST.in
--rw-r--r--   0 cory       (502) staff       (20)     2191 2023-07-22 08:39:21.704456 certifi-2023.7.22/PKG-INFO
--rw-r--r--   0 cory       (502) staff       (20)     1157 2023-01-14 18:45:41.000000 certifi-2023.7.22/README.rst
-drwxr-xr-x   0 cory       (502) staff       (20)        0 2023-07-22 08:39:21.703787 certifi-2023.7.22/certifi/
--rw-r--r--   0 cory       (502) staff       (20)       94 2023-07-22 08:38:57.000000 certifi-2023.7.22/certifi/__init__.py
--rw-r--r--   0 cory       (502) staff       (20)      243 2020-04-05 15:50:05.000000 certifi-2023.7.22/certifi/__main__.py
--rw-r--r--   0 cory       (502) staff       (20)   281617 2023-07-22 08:39:15.000000 certifi-2023.7.22/certifi/cacert.pem
--rw-r--r--   0 cory       (502) staff       (20)     4219 2022-09-13 20:15:32.000000 certifi-2023.7.22/certifi/core.py
--rw-r--r--   0 cory       (502) staff       (20)        0 2022-05-18 19:10:22.000000 certifi-2023.7.22/certifi/py.typed
-drwxr-xr-x   0 cory       (502) staff       (20)        0 2023-07-22 08:39:21.704306 certifi-2023.7.22/certifi.egg-info/
--rw-r--r--   0 cory       (502) staff       (20)     2191 2023-07-22 08:39:21.000000 certifi-2023.7.22/certifi.egg-info/PKG-INFO
--rw-r--r--   0 cory       (502) staff       (20)      285 2023-07-22 08:39:21.000000 certifi-2023.7.22/certifi.egg-info/SOURCES.txt
--rw-r--r--   0 cory       (502) staff       (20)        1 2023-07-22 08:39:21.000000 certifi-2023.7.22/certifi.egg-info/dependency_links.txt
--rw-r--r--   0 cory       (502) staff       (20)        1 2023-07-22 08:39:21.000000 certifi-2023.7.22/certifi.egg-info/not-zip-safe
--rw-r--r--   0 cory       (502) staff       (20)        8 2023-07-22 08:39:21.000000 certifi-2023.7.22/certifi.egg-info/top_level.txt
--rw-r--r--   0 cory       (502) staff       (20)       38 2023-07-22 08:39:21.704603 certifi-2023.7.22/setup.cfg
--rwxr-xr-x   0 cory       (502) staff       (20)     2302 2022-07-20 11:27:58.000000 certifi-2023.7.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 01:21:27.234199 certifi-2024.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-02-02 01:21:20.000000 certifi-2024.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-02 01:21:20.000000 certifi-2024.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-02-02 01:21:27.234199 certifi-2024.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-02-02 01:21:20.000000 certifi-2024.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 01:21:27.234199 certifi-2024.2.2/certifi/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-02 01:21:20.000000 certifi-2024.2.2/certifi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-02 01:21:20.000000 certifi-2024.2.2/certifi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   292541 2024-02-02 01:21:20.000000 certifi-2024.2.2/certifi/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-02-02 01:21:20.000000 certifi-2024.2.2/certifi/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 01:21:20.000000 certifi-2024.2.2/certifi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 01:21:27.234199 certifi-2024.2.2/certifi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-02-02 01:21:27.000000 certifi-2024.2.2/certifi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-02 01:21:27.000000 certifi-2024.2.2/certifi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 01:21:27.000000 certifi-2024.2.2/certifi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 01:21:27.000000 certifi-2024.2.2/certifi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-02 01:21:27.000000 certifi-2024.2.2/certifi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-02 01:21:27.234199 certifi-2024.2.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2176 2024-02-02 01:21:20.000000 certifi-2024.2.2/setup.py
```

### Comparing `certifi-2023.7.22/LICENSE` & `certifi-2024.2.2/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 This package contains a modified version of ca-bundle.crt:
 
 ca-bundle.crt -- Bundle of CA Root Certificates
 
-Certificate data from Mozilla as of: Thu Nov  3 19:04:19 2011#
 This is a bundle of X.509 certificates of public Certificate Authorities
 (CA). These were automatically extracted from Mozilla's root certificates
 file (certdata.txt).  This file can be found in the mozilla source tree:
 https://hg.mozilla.org/mozilla-central/file/tip/security/nss/lib/ckfw/builtins/certdata.txt
 It contains the certificates in PEM format and therefore
 can be directly used with curl / libcurl / php_curl, or with
 an Apache+mod_ssl webserver for SSL client authentication.
```

### Comparing `certifi-2023.7.22/PKG-INFO` & `certifi-2024.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: certifi
-Version: 2023.7.22
+Version: 2024.2.2
 Summary: Python package for providing Mozilla's CA Bundle.
 Home-page: https://github.com/certifi/python-certifi
 Author: Kenneth Reitz
 Author-email: me@kennethreitz.com
 License: MPL-2.0
 Project-URL: Source, https://github.com/certifi/python-certifi
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -61,9 +60,7 @@
 Addition/Removal of Certificates
 --------------------------------
 
 Certifi does not support any addition/removal or other modification of the
 CA trust store content. This project is intended to provide a reliable and
 highly portable root of trust to python deployments. Look to upstream projects
 for methods to use alternate trust.
-
-
```

### Comparing `certifi-2023.7.22/README.rst` & `certifi-2024.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `certifi-2023.7.22/certifi/cacert.pem` & `certifi-2024.2.2/certifi/cacert.pem`

 * *Files 1% similar despite different names*

```diff
@@ -241,42 +241,14 @@
 k8HkyWkaPcBrTiJt7qtYTcbQQcEr6k8Sh17rRdhs9ZgC06DYVYoGmRmioHfRMJ6s
 zHXug/WwYjnPbFfiTNKRCw51KBuav/0aQ/HKd/s7j2G4aSgWQgRecCocIdiP4b0j
 Wy10QJLZYxkNc91pvGJHvOB0K7Lrfb5BG7XARsWhIstfTsEokt4YutUqKLsRixeT
 mJlglFwjz1onl14LBQaTNx47aTbrqZ5hHY8y2o4M1nQ+ewkk2gF3R8Q7zTSMmfXK
 4SVhM7JZG+Ju1zdXtg2pEto=
 -----END CERTIFICATE-----
 
-# Issuer: O=SECOM Trust.net OU=Security Communication RootCA1
-# Subject: O=SECOM Trust.net OU=Security Communication RootCA1
-# Label: "Security Communication Root CA"
-# Serial: 0
-# MD5 Fingerprint: f1:bc:63:6a:54:e0:b5:27:f5:cd:e7:1a:e3:4d:6e:4a
-# SHA1 Fingerprint: 36:b1:2b:49:f9:81:9e:d7:4c:9e:bc:38:0f:c6:56:8f:5d:ac:b2:f7
-# SHA256 Fingerprint: e7:5e:72:ed:9f:56:0e:ec:6e:b4:80:00:73:a4:3f:c3:ad:19:19:5a:39:22:82:01:78:95:97:4a:99:02:6b:6c
------BEGIN CERTIFICATE-----
-MIIDWjCCAkKgAwIBAgIBADANBgkqhkiG9w0BAQUFADBQMQswCQYDVQQGEwJKUDEY
-MBYGA1UEChMPU0VDT00gVHJ1c3QubmV0MScwJQYDVQQLEx5TZWN1cml0eSBDb21t
-dW5pY2F0aW9uIFJvb3RDQTEwHhcNMDMwOTMwMDQyMDQ5WhcNMjMwOTMwMDQyMDQ5
-WjBQMQswCQYDVQQGEwJKUDEYMBYGA1UEChMPU0VDT00gVHJ1c3QubmV0MScwJQYD
-VQQLEx5TZWN1cml0eSBDb21tdW5pY2F0aW9uIFJvb3RDQTEwggEiMA0GCSqGSIb3
-DQEBAQUAA4IBDwAwggEKAoIBAQCzs/5/022x7xZ8V6UMbXaKL0u/ZPtM7orw8yl8
-9f/uKuDp6bpbZCKamm8sOiZpUQWZJtzVHGpxxpp9Hp3dfGzGjGdnSj74cbAZJ6kJ
-DKaVv0uMDPpVmDvY6CKhS3E4eayXkmmziX7qIWgGmBSWh9JhNrxtJ1aeV+7AwFb9
-Ms+k2Y7CI9eNqPPYJayX5HA49LY6tJ07lyZDo6G8SVlyTCMwhwFY9k6+HGhWZq/N
-QV3Is00qVUarH9oe4kA92819uZKAnDfdDJZkndwi92SL32HeFZRSFaB9UslLqCHJ
-xrHty8OVYNEP8Ktw+N/LTX7s1vqr2b1/VPKl6Xn62dZ2JChzAgMBAAGjPzA9MB0G
-A1UdDgQWBBSgc0mZaNyFW2XjmygvV5+9M7wHSDALBgNVHQ8EBAMCAQYwDwYDVR0T
-AQH/BAUwAwEB/zANBgkqhkiG9w0BAQUFAAOCAQEAaECpqLvkT115swW1F7NgE+vG
-kl3g0dNq/vu+m22/xwVtWSDEHPC32oRYAmP6SBbvT6UL90qY8j+eG61Ha2POCEfr
-Uj94nK9NrvjVT8+amCoQQTlSxN3Zmw7vkwGusi7KaEIkQmywszo+zenaSMQVy+n5
-Bw+SUEmK3TGXX8npN6o7WWWXlDLJs58+OmJYxUmtYg5xpTKqL8aJdkNAExNnPaJU
-JRDL8Try2frbSVa7pv6nQTXD4IhhyYjH3zYQIphZ6rBK+1YWc26sTfcioU+tHXot
-RSflMMFe8toTyyVCUZVHA4xsIcx0Qu1T/zOLjw9XARYvz6buyXAiFL39vmwLAw==
------END CERTIFICATE-----
-
 # Issuer: CN=XRamp Global Certification Authority O=XRamp Security Services Inc OU=www.xrampsecurity.com
 # Subject: CN=XRamp Global Certification Authority O=XRamp Security Services Inc OU=www.xrampsecurity.com
 # Label: "XRamp Global CA Root"
 # Serial: 107108908803651509692980124233745014957
 # MD5 Fingerprint: a1:0b:44:b3:ca:10:d8:00:6e:9d:0f:d8:0f:92:0a:d1
 # SHA1 Fingerprint: b8:01:86:d1:eb:9c:86:a5:41:04:cf:30:54:f3:4c:52:b7:e5:58:c6
 # SHA256 Fingerprint: ce:cd:dc:90:50:99:d8:da:df:c5:b1:d2:09:b7:37:cb:e2:c1:8c:fb:2c:10:c0:ff:0b:cf:0d:32:86:fc:1a:a2
@@ -877,57 +849,14 @@
 jjM5RcOO5LlXbKr8EpbsU8Yt5CRsuZRj+9xTaGdWPoO4zzUhw8lo/s7awlOqzJCK
 6fBdRoyV3XpYKBovHd7NADdBj+1EbddTKJd+82cEHhXXipa0095MJ6RMG3NzdvQX
 mcIfeg7jLQitChws/zyrVQ4PkX4268NXSb7hLi18YIvDQVETI53O9zJrlAGomecs
 Mx86OyXShkDOOyyGeMlhLxS67ttVb9+E7gUJTb0o2HLO02JQZR7rkpeDMdmztcpH
 WD9f
 -----END CERTIFICATE-----
 
-# Issuer: CN=Autoridad de Certificacion Firmaprofesional CIF A62634068
-# Subject: CN=Autoridad de Certificacion Firmaprofesional CIF A62634068
-# Label: "Autoridad de Certificacion Firmaprofesional CIF A62634068"
-# Serial: 6047274297262753887
-# MD5 Fingerprint: 73:3a:74:7a:ec:bb:a3:96:a6:c2:e4:e2:c8:9b:c0:c3
-# SHA1 Fingerprint: ae:c5:fb:3f:c8:e1:bf:c4:e5:4f:03:07:5a:9a:e8:00:b7:f7:b6:fa
-# SHA256 Fingerprint: 04:04:80:28:bf:1f:28:64:d4:8f:9a:d4:d8:32:94:36:6a:82:88:56:55:3f:3b:14:30:3f:90:14:7f:5d:40:ef
------BEGIN CERTIFICATE-----
-MIIGFDCCA/ygAwIBAgIIU+w77vuySF8wDQYJKoZIhvcNAQEFBQAwUTELMAkGA1UE
-BhMCRVMxQjBABgNVBAMMOUF1dG9yaWRhZCBkZSBDZXJ0aWZpY2FjaW9uIEZpcm1h
-cHJvZmVzaW9uYWwgQ0lGIEE2MjYzNDA2ODAeFw0wOTA1MjAwODM4MTVaFw0zMDEy
-MzEwODM4MTVaMFExCzAJBgNVBAYTAkVTMUIwQAYDVQQDDDlBdXRvcmlkYWQgZGUg
-Q2VydGlmaWNhY2lvbiBGaXJtYXByb2Zlc2lvbmFsIENJRiBBNjI2MzQwNjgwggIi
-MA0GCSqGSIb3DQEBAQUAA4ICDwAwggIKAoICAQDKlmuO6vj78aI14H9M2uDDUtd9
-thDIAl6zQyrET2qyyhxdKJp4ERppWVevtSBC5IsP5t9bpgOSL/UR5GLXMnE42QQM
-cas9UX4PB99jBVzpv5RvwSmCwLTaUbDBPLutN0pcyvFLNg4kq7/DhHf9qFD0sefG
-L9ItWY16Ck6WaVICqjaY7Pz6FIMMNx/Jkjd/14Et5cS54D40/mf0PmbR0/RAz15i
-NA9wBj4gGFrO93IbJWyTdBSTo3OxDqqHECNZXyAFGUftaI6SEspd/NYrspI8IM/h
-X68gvqB2f3bl7BqGYTM+53u0P6APjqK5am+5hyZvQWyIplD9amML9ZMWGxmPsu2b
-m8mQ9QEM3xk9Dz44I8kvjwzRAv4bVdZO0I08r0+k8/6vKtMFnXkIoctXMbScyJCy
-Z/QYFpM6/EfY0XiWMR+6KwxfXZmtY4laJCB22N/9q06mIqqdXuYnin1oKaPnirja
-EbsXLZmdEyRG98Xi2J+Of8ePdG1asuhy9azuJBCtLxTa/y2aRnFHvkLfuwHb9H/T
-KI8xWVvTyQKmtFLKbpf7Q8UIJm+K9Lv9nyiqDdVF8xM6HdjAeI9BZzwelGSuewvF
-6NkBiDkal4ZkQdU7hwxu+g/GvUgUvzlN1J5Bto+WHWOWk9mVBngxaJ43BjuAiUVh
-OSPHG0SjFeUc+JIwuwIDAQABo4HvMIHsMBIGA1UdEwEB/wQIMAYBAf8CAQEwDgYD
-VR0PAQH/BAQDAgEGMB0GA1UdDgQWBBRlzeurNR4APn7VdMActHNHDhpkLzCBpgYD
-VR0gBIGeMIGbMIGYBgRVHSAAMIGPMC8GCCsGAQUFBwIBFiNodHRwOi8vd3d3LmZp
-cm1hcHJvZmVzaW9uYWwuY29tL2NwczBcBggrBgEFBQcCAjBQHk4AUABhAHMAZQBv
-ACAAZABlACAAbABhACAAQgBvAG4AYQBuAG8AdgBhACAANAA3ACAAQgBhAHIAYwBl
-AGwAbwBuAGEAIAAwADgAMAAxADcwDQYJKoZIhvcNAQEFBQADggIBABd9oPm03cXF
-661LJLWhAqvdpYhKsg9VSytXjDvlMd3+xDLx51tkljYyGOylMnfX40S2wBEqgLk9
-am58m9Ot/MPWo+ZkKXzR4Tgegiv/J2Wv+xYVxC5xhOW1//qkR71kMrv2JYSiJ0L1
-ILDCExARzRAVukKQKtJE4ZYm6zFIEv0q2skGz3QeqUvVhyj5eTSSPi5E6PaPT481
-PyWzOdxjKpBrIF/EUhJOlywqrJ2X3kjyo2bbwtKDlaZmp54lD+kLM5FlClrD2VQS
-3a/DTg4fJl4N3LON7NWBcN7STyQF82xO9UxJZo3R/9ILJUFI/lGExkKvgATP0H5k
-SeTy36LssUzAKh3ntLFlosS88Zj0qnAHY7S42jtM+kAiMFsRpvAFDsYCA0irhpuF
-3dvd6qJ2gHN99ZwExEWN57kci57q13XRcrHedUTnQn3iV2t93Jm8PYMo6oCTjcVM
-ZcFwgbg4/EMxsvYDNEeyrPsiBsse3RdHHF9mudMaotoRsaS8I8nkvof/uZS2+F0g
-StRf571oe2XyFR7SOqkt6dhrJKyXWERHrVkY8SFlcN7ONGCoQPHzPKTDKCOM/icz
-Q0CgFzzr6juwcqajuUpLXhZI9LK8yIySxZ2frHI2vDSANGupi5LAuBft7HZT9SQB
-jLMi6Et8Vcad+qMUu2WFbm5PEn4KPJ2V
------END CERTIFICATE-----
-
 # Issuer: CN=Izenpe.com O=IZENPE S.A.
 # Subject: CN=Izenpe.com O=IZENPE S.A.
 # Label: "Izenpe.com"
 # Serial: 917563065490389241595536686991402621
 # MD5 Fingerprint: a6:b0:cd:85:80:da:5c:50:34:a3:39:90:2f:55:67:73
 # SHA1 Fingerprint: 2f:78:3d:25:52:18:a7:4a:65:39:71:b5:2c:a2:9c:45:15:6f:e9:19
 # SHA256 Fingerprint: 25:30:cc:8e:98:32:15:02:ba:d9:6f:9b:1f:ba:1b:09:9e:2d:29:9e:0f:45:48:bb:91:4f:36:3b:c0:d4:53:1f
@@ -4629,7 +4558,257 @@
 rr3e97sPWD2PAzHoPYJQyi9eDF20l74gNAf0xBLh7tew2VktafcxBPTy+av5EzH4
 AXcOPUIjJsyacmdRIXrMPIWo6iFqO9taPKU0nprALN+AnCng33eU0aKAQv9qTFsR
 0PXNor6uzFFcw9VUewyu1rkGd4Di7wcaaMxZUa1+XGdrudviB0JbuAEFWDlN5LuY
 o7Ey7Nmj1m+UI/87tyll5gfp77YZ6ufCOB0yiJA8EytuzO+rdwY0d4RPcuSBhPm5
 dDTedk+SKlOxJTnbPP/lPqYO5Wue/9vsL3SD3460s6neFE3/MaNFcyT6lSnMEpcE
 oji2jbDwN/zIIX8/syQbPYtuzE2wFg2WHYMfRsCbvUOZ58SWLs5fyQ==
 -----END CERTIFICATE-----
+
+# Issuer: CN=TrustAsia Global Root CA G3 O=TrustAsia Technologies, Inc.
+# Subject: CN=TrustAsia Global Root CA G3 O=TrustAsia Technologies, Inc.
+# Label: "TrustAsia Global Root CA G3"
+# Serial: 576386314500428537169965010905813481816650257167
+# MD5 Fingerprint: 30:42:1b:b7:bb:81:75:35:e4:16:4f:53:d2:94:de:04
+# SHA1 Fingerprint: 63:cf:b6:c1:27:2b:56:e4:88:8e:1c:23:9a:b6:2e:81:47:24:c3:c7
+# SHA256 Fingerprint: e0:d3:22:6a:eb:11:63:c2:e4:8f:f9:be:3b:50:b4:c6:43:1b:e7:bb:1e:ac:c5:c3:6b:5d:5e:c5:09:03:9a:08
+-----BEGIN CERTIFICATE-----
+MIIFpTCCA42gAwIBAgIUZPYOZXdhaqs7tOqFhLuxibhxkw8wDQYJKoZIhvcNAQEM
+BQAwWjELMAkGA1UEBhMCQ04xJTAjBgNVBAoMHFRydXN0QXNpYSBUZWNobm9sb2dp
+ZXMsIEluYy4xJDAiBgNVBAMMG1RydXN0QXNpYSBHbG9iYWwgUm9vdCBDQSBHMzAe
+Fw0yMTA1MjAwMjEwMTlaFw00NjA1MTkwMjEwMTlaMFoxCzAJBgNVBAYTAkNOMSUw
+IwYDVQQKDBxUcnVzdEFzaWEgVGVjaG5vbG9naWVzLCBJbmMuMSQwIgYDVQQDDBtU
+cnVzdEFzaWEgR2xvYmFsIFJvb3QgQ0EgRzMwggIiMA0GCSqGSIb3DQEBAQUAA4IC
+DwAwggIKAoICAQDAMYJhkuSUGwoqZdC+BqmHO1ES6nBBruL7dOoKjbmzTNyPtxNS
+T1QY4SxzlZHFZjtqz6xjbYdT8PfxObegQ2OwxANdV6nnRM7EoYNl9lA+sX4WuDqK
+AtCWHwDNBSHvBm3dIZwZQ0WhxeiAysKtQGIXBsaqvPPW5vxQfmZCHzyLpnl5hkA1
+nyDvP+uLRx+PjsXUjrYsyUQE49RDdT/VP68czH5GX6zfZBCK70bwkPAPLfSIC7Ep
+qq+FqklYqL9joDiR5rPmd2jE+SoZhLsO4fWvieylL1AgdB4SQXMeJNnKziyhWTXA
+yB1GJ2Faj/lN03J5Zh6fFZAhLf3ti1ZwA0pJPn9pMRJpxx5cynoTi+jm9WAPzJMs
+hH/x/Gr8m0ed262IPfN2dTPXS6TIi/n1Q1hPy8gDVI+lhXgEGvNz8teHHUGf59gX
+zhqcD0r83ERoVGjiQTz+LISGNzzNPy+i2+f3VANfWdP3kXjHi3dqFuVJhZBFcnAv
+kV34PmVACxmZySYgWmjBNb9Pp1Hx2BErW+Canig7CjoKH8GB5S7wprlppYiU5msT
+f9FkPz2ccEblooV7WIQn3MSAPmeamseaMQ4w7OYXQJXZRe0Blqq/DPNL0WP3E1jA
+uPP6Z92bfW1K/zJMtSU7/xxnD4UiWQWRkUF3gdCFTIcQcf+eQxuulXUtgQIDAQAB
+o2MwYTAPBgNVHRMBAf8EBTADAQH/MB8GA1UdIwQYMBaAFEDk5PIj7zjKsK5Xf/Ih
+MBY027ySMB0GA1UdDgQWBBRA5OTyI+84yrCuV3/yITAWNNu8kjAOBgNVHQ8BAf8E
+BAMCAQYwDQYJKoZIhvcNAQEMBQADggIBACY7UeFNOPMyGLS0XuFlXsSUT9SnYaP4
+wM8zAQLpw6o1D/GUE3d3NZ4tVlFEbuHGLige/9rsR82XRBf34EzC4Xx8MnpmyFq2
+XFNFV1pF1AWZLy4jVe5jaN/TG3inEpQGAHUNcoTpLrxaatXeL1nHo+zSh2bbt1S1
+JKv0Q3jbSwTEb93mPmY+KfJLaHEih6D4sTNjduMNhXJEIlU/HHzp/LgV6FL6qj6j
+ITk1dImmasI5+njPtqzn59ZW/yOSLlALqbUHM/Q4X6RJpstlcHboCoWASzY9M/eV
+VHUl2qzEc4Jl6VL1XP04lQJqaTDFHApXB64ipCz5xUG3uOyfT0gA+QEEVcys+TIx
+xHWVBqB/0Y0n3bOppHKH/lmLmnp0Ft0WpWIp6zqW3IunaFnT63eROfjXy9mPX1on
+AX1daBli2MjN9LdyR75bl87yraKZk62Uy5P2EgmVtqvXO9A/EcswFi55gORngS1d
+7XB4tmBZrOFdRWOPyN9yaFvqHbgB8X7754qz41SgOAngPN5C8sLtLpvzHzW2Ntjj
+gKGLzZlkD8Kqq7HK9W+eQ42EVJmzbsASZthwEPEGNTNDqJwuuhQxzhB/HIbjj9LV
++Hfsm6vxL2PZQl/gZ4FkkfGXL/xuJvYz+NO1+MRiqzFRJQJ6+N1rZdVtTTDIZbpo
+FGWsJwt0ivKH
+-----END CERTIFICATE-----
+
+# Issuer: CN=TrustAsia Global Root CA G4 O=TrustAsia Technologies, Inc.
+# Subject: CN=TrustAsia Global Root CA G4 O=TrustAsia Technologies, Inc.
+# Label: "TrustAsia Global Root CA G4"
+# Serial: 451799571007117016466790293371524403291602933463
+# MD5 Fingerprint: 54:dd:b2:d7:5f:d8:3e:ed:7c:e0:0b:2e:cc:ed:eb:eb
+# SHA1 Fingerprint: 57:73:a5:61:5d:80:b2:e6:ac:38:82:fc:68:07:31:ac:9f:b5:92:5a
+# SHA256 Fingerprint: be:4b:56:cb:50:56:c0:13:6a:52:6d:f4:44:50:8d:aa:36:a0:b5:4f:42:e4:ac:38:f7:2a:f4:70:e4:79:65:4c
+-----BEGIN CERTIFICATE-----
+MIICVTCCAdygAwIBAgIUTyNkuI6XY57GU4HBdk7LKnQV1tcwCgYIKoZIzj0EAwMw
+WjELMAkGA1UEBhMCQ04xJTAjBgNVBAoMHFRydXN0QXNpYSBUZWNobm9sb2dpZXMs
+IEluYy4xJDAiBgNVBAMMG1RydXN0QXNpYSBHbG9iYWwgUm9vdCBDQSBHNDAeFw0y
+MTA1MjAwMjEwMjJaFw00NjA1MTkwMjEwMjJaMFoxCzAJBgNVBAYTAkNOMSUwIwYD
+VQQKDBxUcnVzdEFzaWEgVGVjaG5vbG9naWVzLCBJbmMuMSQwIgYDVQQDDBtUcnVz
+dEFzaWEgR2xvYmFsIFJvb3QgQ0EgRzQwdjAQBgcqhkjOPQIBBgUrgQQAIgNiAATx
+s8045CVD5d4ZCbuBeaIVXxVjAd7Cq92zphtnS4CDr5nLrBfbK5bKfFJV4hrhPVbw
+LxYI+hW8m7tH5j/uqOFMjPXTNvk4XatwmkcN4oFBButJ+bAp3TPsUKV/eSm4IJij
+YzBhMA8GA1UdEwEB/wQFMAMBAf8wHwYDVR0jBBgwFoAUpbtKl86zK3+kMd6Xg1mD
+pm9xy94wHQYDVR0OBBYEFKW7SpfOsyt/pDHel4NZg6ZvccveMA4GA1UdDwEB/wQE
+AwIBBjAKBggqhkjOPQQDAwNnADBkAjBe8usGzEkxn0AAbbd+NvBNEU/zy4k6LHiR
+UKNbwMp1JvK/kF0LgoxgKJ/GcJpo5PECMFxYDlZ2z1jD1xCMuo6u47xkdUfFVZDj
+/bpV6wfEU6s3qe4hsiFbYI89MvHVI5TWWA==
+-----END CERTIFICATE-----
+
+# Issuer: CN=CommScope Public Trust ECC Root-01 O=CommScope
+# Subject: CN=CommScope Public Trust ECC Root-01 O=CommScope
+# Label: "CommScope Public Trust ECC Root-01"
+# Serial: 385011430473757362783587124273108818652468453534
+# MD5 Fingerprint: 3a:40:a7:fc:03:8c:9c:38:79:2f:3a:a2:6c:b6:0a:16
+# SHA1 Fingerprint: 07:86:c0:d8:dd:8e:c0:80:98:06:98:d0:58:7a:ef:de:a6:cc:a2:5d
+# SHA256 Fingerprint: 11:43:7c:da:7b:b4:5e:41:36:5f:45:b3:9a:38:98:6b:0d:e0:0d:ef:34:8e:0c:7b:b0:87:36:33:80:0b:c3:8b
+-----BEGIN CERTIFICATE-----
+MIICHTCCAaOgAwIBAgIUQ3CCd89NXTTxyq4yLzf39H91oJ4wCgYIKoZIzj0EAwMw
+TjELMAkGA1UEBhMCVVMxEjAQBgNVBAoMCUNvbW1TY29wZTErMCkGA1UEAwwiQ29t
+bVNjb3BlIFB1YmxpYyBUcnVzdCBFQ0MgUm9vdC0wMTAeFw0yMTA0MjgxNzM1NDNa
+Fw00NjA0MjgxNzM1NDJaME4xCzAJBgNVBAYTAlVTMRIwEAYDVQQKDAlDb21tU2Nv
+cGUxKzApBgNVBAMMIkNvbW1TY29wZSBQdWJsaWMgVHJ1c3QgRUNDIFJvb3QtMDEw
+djAQBgcqhkjOPQIBBgUrgQQAIgNiAARLNumuV16ocNfQj3Rid8NeeqrltqLxeP0C
+flfdkXmcbLlSiFS8LwS+uM32ENEp7LXQoMPwiXAZu1FlxUOcw5tjnSCDPgYLpkJE
+hRGnSjot6dZoL0hOUysHP029uax3OVejQjBAMA8GA1UdEwEB/wQFMAMBAf8wDgYD
+VR0PAQH/BAQDAgEGMB0GA1UdDgQWBBSOB2LAUN3GGQYARnQE9/OufXVNMDAKBggq
+hkjOPQQDAwNoADBlAjEAnDPfQeMjqEI2Jpc1XHvr20v4qotzVRVcrHgpD7oh2MSg
+2NED3W3ROT3Ek2DS43KyAjB8xX6I01D1HiXo+k515liWpDVfG2XqYZpwI7UNo5uS
+Um9poIyNStDuiw7LR47QjRE=
+-----END CERTIFICATE-----
+
+# Issuer: CN=CommScope Public Trust ECC Root-02 O=CommScope
+# Subject: CN=CommScope Public Trust ECC Root-02 O=CommScope
+# Label: "CommScope Public Trust ECC Root-02"
+# Serial: 234015080301808452132356021271193974922492992893
+# MD5 Fingerprint: 59:b0:44:d5:65:4d:b8:5c:55:19:92:02:b6:d1:94:b2
+# SHA1 Fingerprint: 3c:3f:ef:57:0f:fe:65:93:86:9e:a0:fe:b0:f6:ed:8e:d1:13:c7:e5
+# SHA256 Fingerprint: 2f:fb:7f:81:3b:bb:b3:c8:9a:b4:e8:16:2d:0f:16:d7:15:09:a8:30:cc:9d:73:c2:62:e5:14:08:75:d1:ad:4a
+-----BEGIN CERTIFICATE-----
+MIICHDCCAaOgAwIBAgIUKP2ZYEFHpgE6yhR7H+/5aAiDXX0wCgYIKoZIzj0EAwMw
+TjELMAkGA1UEBhMCVVMxEjAQBgNVBAoMCUNvbW1TY29wZTErMCkGA1UEAwwiQ29t
+bVNjb3BlIFB1YmxpYyBUcnVzdCBFQ0MgUm9vdC0wMjAeFw0yMTA0MjgxNzQ0NTRa
+Fw00NjA0MjgxNzQ0NTNaME4xCzAJBgNVBAYTAlVTMRIwEAYDVQQKDAlDb21tU2Nv
+cGUxKzApBgNVBAMMIkNvbW1TY29wZSBQdWJsaWMgVHJ1c3QgRUNDIFJvb3QtMDIw
+djAQBgcqhkjOPQIBBgUrgQQAIgNiAAR4MIHoYx7l63FRD/cHB8o5mXxO1Q/MMDAL
+j2aTPs+9xYa9+bG3tD60B8jzljHz7aRP+KNOjSkVWLjVb3/ubCK1sK9IRQq9qEmU
+v4RDsNuESgMjGWdqb8FuvAY5N9GIIvejQjBAMA8GA1UdEwEB/wQFMAMBAf8wDgYD
+VR0PAQH/BAQDAgEGMB0GA1UdDgQWBBTmGHX/72DehKT1RsfeSlXjMjZ59TAKBggq
+hkjOPQQDAwNnADBkAjAmc0l6tqvmSfR9Uj/UQQSugEODZXW5hYA4O9Zv5JOGq4/n
+ich/m35rChJVYaoR4HkCMHfoMXGsPHED1oQmHhS48zs73u1Z/GtMMH9ZzkXpc2AV
+mkzw5l4lIhVtwodZ0LKOag==
+-----END CERTIFICATE-----
+
+# Issuer: CN=CommScope Public Trust RSA Root-01 O=CommScope
+# Subject: CN=CommScope Public Trust RSA Root-01 O=CommScope
+# Label: "CommScope Public Trust RSA Root-01"
+# Serial: 354030733275608256394402989253558293562031411421
+# MD5 Fingerprint: 0e:b4:15:bc:87:63:5d:5d:02:73:d4:26:38:68:73:d8
+# SHA1 Fingerprint: 6d:0a:5f:f7:b4:23:06:b4:85:b3:b7:97:64:fc:ac:75:f5:33:f2:93
+# SHA256 Fingerprint: 02:bd:f9:6e:2a:45:dd:9b:f1:8f:c7:e1:db:df:21:a0:37:9b:a3:c9:c2:61:03:44:cf:d8:d6:06:fe:c1:ed:81
+-----BEGIN CERTIFICATE-----
+MIIFbDCCA1SgAwIBAgIUPgNJgXUWdDGOTKvVxZAplsU5EN0wDQYJKoZIhvcNAQEL
+BQAwTjELMAkGA1UEBhMCVVMxEjAQBgNVBAoMCUNvbW1TY29wZTErMCkGA1UEAwwi
+Q29tbVNjb3BlIFB1YmxpYyBUcnVzdCBSU0EgUm9vdC0wMTAeFw0yMTA0MjgxNjQ1
+NTRaFw00NjA0MjgxNjQ1NTNaME4xCzAJBgNVBAYTAlVTMRIwEAYDVQQKDAlDb21t
+U2NvcGUxKzApBgNVBAMMIkNvbW1TY29wZSBQdWJsaWMgVHJ1c3QgUlNBIFJvb3Qt
+MDEwggIiMA0GCSqGSIb3DQEBAQUAA4ICDwAwggIKAoICAQCwSGWjDR1C45FtnYSk
+YZYSwu3D2iM0GXb26v1VWvZVAVMP8syMl0+5UMuzAURWlv2bKOx7dAvnQmtVzslh
+suitQDy6uUEKBU8bJoWPQ7VAtYXR1HHcg0Hz9kXHgKKEUJdGzqAMxGBWBB0HW0al
+DrJLpA6lfO741GIDuZNqihS4cPgugkY4Iw50x2tBt9Apo52AsH53k2NC+zSDO3Oj
+WiE260f6GBfZumbCk6SP/F2krfxQapWsvCQz0b2If4b19bJzKo98rwjyGpg/qYFl
+P8GMicWWMJoKz/TUyDTtnS+8jTiGU+6Xn6myY5QXjQ/cZip8UlF1y5mO6D1cv547
+KI2DAg+pn3LiLCuz3GaXAEDQpFSOm117RTYm1nJD68/A6g3czhLmfTifBSeolz7p
+UcZsBSjBAg/pGG3svZwG1KdJ9FQFa2ww8esD1eo9anbCyxooSU1/ZOD6K9pzg4H/
+kQO9lLvkuI6cMmPNn7togbGEW682v3fuHX/3SZtS7NJ3Wn2RnU3COS3kuoL4b/JO
+Hg9O5j9ZpSPcPYeoKFgo0fEbNttPxP/hjFtyjMcmAyejOQoBqsCyMWCDIqFPEgkB
+Ea801M/XrmLTBQe0MXXgDW1XT2mH+VepuhX2yFJtocucH+X8eKg1mp9BFM6ltM6U
+CBwJrVbl2rZJmkrqYxhTnCwuwwIDAQABo0IwQDAPBgNVHRMBAf8EBTADAQH/MA4G
+A1UdDwEB/wQEAwIBBjAdBgNVHQ4EFgQUN12mmnQywsL5x6YVEFm45P3luG0wDQYJ
+KoZIhvcNAQELBQADggIBAK+nz97/4L1CjU3lIpbfaOp9TSp90K09FlxD533Ahuh6
+NWPxzIHIxgvoLlI1pKZJkGNRrDSsBTtXAOnTYtPZKdVUvhwQkZyybf5Z/Xn36lbQ
+nmhUQo8mUuJM3y+Xpi/SB5io82BdS5pYV4jvguX6r2yBS5KPQJqTRlnLX3gWsWc+
+QgvfKNmwrZggvkN80V4aCRckjXtdlemrwWCrWxhkgPut4AZ9HcpZuPN4KWfGVh2v
+trV0KnahP/t1MJ+UXjulYPPLXAziDslg+MkfFoom3ecnf+slpoq9uC02EJqxWE2a
+aE9gVOX2RhOOiKy8IUISrcZKiX2bwdgt6ZYD9KJ0DLwAHb/WNyVntHKLr4W96ioD
+j8z7PEQkguIBpQtZtjSNMgsSDesnwv1B10A8ckYpwIzqug/xBpMu95yo9GA+o/E4
+Xo4TwbM6l4c/ksp4qRyv0LAbJh6+cOx69TOY6lz/KwsETkPdY34Op054A5U+1C0w
+lREQKC6/oAI+/15Z0wUOlV9TRe9rh9VIzRamloPh37MG88EU26fsHItdkJANclHn
+YfkUyq+Dj7+vsQpZXdxc1+SWrVtgHdqul7I52Qb1dgAT+GhMIbA1xNxVssnBQVoc
+icCMb3SgazNNtQEo/a2tiRc7ppqEvOuM6sRxJKi6KfkIsidWNTJf6jn7MZrVGczw
+-----END CERTIFICATE-----
+
+# Issuer: CN=CommScope Public Trust RSA Root-02 O=CommScope
+# Subject: CN=CommScope Public Trust RSA Root-02 O=CommScope
+# Label: "CommScope Public Trust RSA Root-02"
+# Serial: 480062499834624527752716769107743131258796508494
+# MD5 Fingerprint: e1:29:f9:62:7b:76:e2:96:6d:f3:d4:d7:0f:ae:1f:aa
+# SHA1 Fingerprint: ea:b0:e2:52:1b:89:93:4c:11:68:f2:d8:9a:ac:22:4c:a3:8a:57:ae
+# SHA256 Fingerprint: ff:e9:43:d7:93:42:4b:4f:7c:44:0c:1c:3d:64:8d:53:63:f3:4b:82:dc:87:aa:7a:9f:11:8f:c5:de:e1:01:f1
+-----BEGIN CERTIFICATE-----
+MIIFbDCCA1SgAwIBAgIUVBa/O345lXGN0aoApYYNK496BU4wDQYJKoZIhvcNAQEL
+BQAwTjELMAkGA1UEBhMCVVMxEjAQBgNVBAoMCUNvbW1TY29wZTErMCkGA1UEAwwi
+Q29tbVNjb3BlIFB1YmxpYyBUcnVzdCBSU0EgUm9vdC0wMjAeFw0yMTA0MjgxNzE2
+NDNaFw00NjA0MjgxNzE2NDJaME4xCzAJBgNVBAYTAlVTMRIwEAYDVQQKDAlDb21t
+U2NvcGUxKzApBgNVBAMMIkNvbW1TY29wZSBQdWJsaWMgVHJ1c3QgUlNBIFJvb3Qt
+MDIwggIiMA0GCSqGSIb3DQEBAQUAA4ICDwAwggIKAoICAQDh+g77aAASyE3VrCLE
+NQE7xVTlWXZjpX/rwcRqmL0yjReA61260WI9JSMZNRTpf4mnG2I81lDnNJUDMrG0
+kyI9p+Kx7eZ7Ti6Hmw0zdQreqjXnfuU2mKKuJZ6VszKWpCtYHu8//mI0SFHRtI1C
+rWDaSWqVcN3SAOLMV2MCe5bdSZdbkk6V0/nLKR8YSvgBKtJjCW4k6YnS5cciTNxz
+hkcAqg2Ijq6FfUrpuzNPDlJwnZXjfG2WWy09X6GDRl224yW4fKcZgBzqZUPckXk2
+LHR88mcGyYnJ27/aaL8j7dxrrSiDeS/sOKUNNwFnJ5rpM9kzXzehxfCrPfp4sOcs
+n/Y+n2Dg70jpkEUeBVF4GiwSLFworA2iI540jwXmojPOEXcT1A6kHkIfhs1w/tku
+FT0du7jyU1fbzMZ0KZwYszZ1OC4PVKH4kh+Jlk+71O6d6Ts2QrUKOyrUZHk2EOH5
+kQMreyBUzQ0ZGshBMjTRsJnhkB4BQDa1t/qp5Xd1pCKBXbCL5CcSD1SIxtuFdOa3
+wNemKfrb3vOTlycEVS8KbzfFPROvCgCpLIscgSjX74Yxqa7ybrjKaixUR9gqiC6v
+wQcQeKwRoi9C8DfF8rhW3Q5iLc4tVn5V8qdE9isy9COoR+jUKgF4z2rDN6ieZdIs
+5fq6M8EGRPbmz6UNp2YINIos8wIDAQABo0IwQDAPBgNVHRMBAf8EBTADAQH/MA4G
+A1UdDwEB/wQEAwIBBjAdBgNVHQ4EFgQUR9DnsSL/nSz12Vdgs7GxcJXvYXowDQYJ
+KoZIhvcNAQELBQADggIBAIZpsU0v6Z9PIpNojuQhmaPORVMbc0RTAIFhzTHjCLqB
+KCh6krm2qMhDnscTJk3C2OVVnJJdUNjCK9v+5qiXz1I6JMNlZFxHMaNlNRPDk7n3
++VGXu6TwYofF1gbTl4MgqX67tiHCpQ2EAOHyJxCDut0DgdXdaMNmEMjRdrSzbyme
+APnCKfWxkxlSaRosTKCL4BWaMS/TiJVZbuXEs1DIFAhKm4sTg7GkcrI7djNB3Nyq
+pgdvHSQSn8h2vS/ZjvQs7rfSOBAkNlEv41xdgSGn2rtO/+YHqP65DSdsu3BaVXoT
+6fEqSWnHX4dXTEN5bTpl6TBcQe7rd6VzEojov32u5cSoHw2OHG1QAk8mGEPej1WF
+sQs3BWDJVTkSBKEqz3EWnzZRSb9wO55nnPt7eck5HHisd5FUmrh1CoFSl+NmYWvt
+PjgelmFV4ZFUjO2MJB+ByRCac5krFk5yAD9UG/iNuovnFNa2RU9g7Jauwy8CTl2d
+lklyALKrdVwPaFsdZcJfMw8eD/A7hvWwTruc9+olBdytoptLFwG+Qt81IR2tq670
+v64fG9PiO/yzcnMcmyiQiRM9HcEARwmWmjgb3bHPDcK0RPOWlc4yOo80nOAXx17O
+rg3bhzjlP1v9mxnhMUF6cKojawHhRUzNlM47ni3niAIi9G7oyOzWPPO5std3eqx7
+-----END CERTIFICATE-----
+
+# Issuer: CN=Telekom Security TLS ECC Root 2020 O=Deutsche Telekom Security GmbH
+# Subject: CN=Telekom Security TLS ECC Root 2020 O=Deutsche Telekom Security GmbH
+# Label: "Telekom Security TLS ECC Root 2020"
+# Serial: 72082518505882327255703894282316633856
+# MD5 Fingerprint: c1:ab:fe:6a:10:2c:03:8d:bc:1c:22:32:c0:85:a7:fd
+# SHA1 Fingerprint: c0:f8:96:c5:a9:3b:01:06:21:07:da:18:42:48:bc:e9:9d:88:d5:ec
+# SHA256 Fingerprint: 57:8a:f4:de:d0:85:3f:4e:59:98:db:4a:ea:f9:cb:ea:8d:94:5f:60:b6:20:a3:8d:1a:3c:13:b2:bc:7b:a8:e1
+-----BEGIN CERTIFICATE-----
+MIICQjCCAcmgAwIBAgIQNjqWjMlcsljN0AFdxeVXADAKBggqhkjOPQQDAzBjMQsw
+CQYDVQQGEwJERTEnMCUGA1UECgweRGV1dHNjaGUgVGVsZWtvbSBTZWN1cml0eSBH
+bWJIMSswKQYDVQQDDCJUZWxla29tIFNlY3VyaXR5IFRMUyBFQ0MgUm9vdCAyMDIw
+MB4XDTIwMDgyNTA3NDgyMFoXDTQ1MDgyNTIzNTk1OVowYzELMAkGA1UEBhMCREUx
+JzAlBgNVBAoMHkRldXRzY2hlIFRlbGVrb20gU2VjdXJpdHkgR21iSDErMCkGA1UE
+AwwiVGVsZWtvbSBTZWN1cml0eSBUTFMgRUNDIFJvb3QgMjAyMDB2MBAGByqGSM49
+AgEGBSuBBAAiA2IABM6//leov9Wq9xCazbzREaK9Z0LMkOsVGJDZos0MKiXrPk/O
+tdKPD/M12kOLAoC+b1EkHQ9rK8qfwm9QMuU3ILYg/4gND21Ju9sGpIeQkpT0CdDP
+f8iAC8GXs7s1J8nCG6NCMEAwHQYDVR0OBBYEFONyzG6VmUex5rNhTNHLq+O6zd6f
+MA8GA1UdEwEB/wQFMAMBAf8wDgYDVR0PAQH/BAQDAgEGMAoGCCqGSM49BAMDA2cA
+MGQCMHVSi7ekEE+uShCLsoRbQuHmKjYC2qBuGT8lv9pZMo7k+5Dck2TOrbRBR2Di
+z6fLHgIwN0GMZt9Ba9aDAEH9L1r3ULRn0SyocddDypwnJJGDSA3PzfdUga/sf+Rn
+27iQ7t0l
+-----END CERTIFICATE-----
+
+# Issuer: CN=Telekom Security TLS RSA Root 2023 O=Deutsche Telekom Security GmbH
+# Subject: CN=Telekom Security TLS RSA Root 2023 O=Deutsche Telekom Security GmbH
+# Label: "Telekom Security TLS RSA Root 2023"
+# Serial: 44676229530606711399881795178081572759
+# MD5 Fingerprint: bf:5b:eb:54:40:cd:48:71:c4:20:8d:7d:de:0a:42:f2
+# SHA1 Fingerprint: 54:d3:ac:b3:bd:57:56:f6:85:9d:ce:e5:c3:21:e2:d4:ad:83:d0:93
+# SHA256 Fingerprint: ef:c6:5c:ad:bb:59:ad:b6:ef:e8:4d:a2:23:11:b3:56:24:b7:1b:3b:1e:a0:da:8b:66:55:17:4e:c8:97:86:46
+-----BEGIN CERTIFICATE-----
+MIIFszCCA5ugAwIBAgIQIZxULej27HF3+k7ow3BXlzANBgkqhkiG9w0BAQwFADBj
+MQswCQYDVQQGEwJERTEnMCUGA1UECgweRGV1dHNjaGUgVGVsZWtvbSBTZWN1cml0
+eSBHbWJIMSswKQYDVQQDDCJUZWxla29tIFNlY3VyaXR5IFRMUyBSU0EgUm9vdCAy
+MDIzMB4XDTIzMDMyODEyMTY0NVoXDTQ4MDMyNzIzNTk1OVowYzELMAkGA1UEBhMC
+REUxJzAlBgNVBAoMHkRldXRzY2hlIFRlbGVrb20gU2VjdXJpdHkgR21iSDErMCkG
+A1UEAwwiVGVsZWtvbSBTZWN1cml0eSBUTFMgUlNBIFJvb3QgMjAyMzCCAiIwDQYJ
+KoZIhvcNAQEBBQADggIPADCCAgoCggIBAO01oYGA88tKaVvC+1GDrib94W7zgRJ9
+cUD/h3VCKSHtgVIs3xLBGYSJwb3FKNXVS2xE1kzbB5ZKVXrKNoIENqil/Cf2SfHV
+cp6R+SPWcHu79ZvB7JPPGeplfohwoHP89v+1VmLhc2o0mD6CuKyVU/QBoCcHcqMA
+U6DksquDOFczJZSfvkgdmOGjup5czQRxUX11eKvzWarE4GC+j4NSuHUaQTXtvPM6
+Y+mpFEXX5lLRbtLevOP1Czvm4MS9Q2QTps70mDdsipWol8hHD/BeEIvnHRz+sTug
+BTNoBUGCwQMrAcjnj02r6LX2zWtEtefdi+zqJbQAIldNsLGyMcEWzv/9FIS3R/qy
+8XDe24tsNlikfLMR0cN3f1+2JeANxdKz+bi4d9s3cXFH42AYTyS2dTd4uaNir73J
+co4vzLuu2+QVUhkHM/tqty1LkCiCc/4YizWN26cEar7qwU02OxY2kTLvtkCJkUPg
+8qKrBC7m8kwOFjQgrIfBLX7JZkcXFBGk8/ehJImr2BrIoVyxo/eMbcgByU/J7MT8
+rFEz0ciD0cmfHdRHNCk+y7AO+oMLKFjlKdw/fKifybYKu6boRhYPluV75Gp6SG12
+mAWl3G0eQh5C2hrgUve1g8Aae3g1LDj1H/1Joy7SWWO/gLCMk3PLNaaZlSJhZQNg
++y+TS/qanIA7AgMBAAGjYzBhMA4GA1UdDwEB/wQEAwIBBjAdBgNVHQ4EFgQUtqeX
+gj10hZv3PJ+TmpV5dVKMbUcwDwYDVR0TAQH/BAUwAwEB/zAfBgNVHSMEGDAWgBS2
+p5eCPXSFm/c8n5OalXl1UoxtRzANBgkqhkiG9w0BAQwFAAOCAgEAqMxhpr51nhVQ
+pGv7qHBFfLp+sVr8WyP6Cnf4mHGCDG3gXkaqk/QeoMPhk9tLrbKmXauw1GLLXrtm
+9S3ul0A8Yute1hTWjOKWi0FpkzXmuZlrYrShF2Y0pmtjxrlO8iLpWA1WQdH6DErw
+M807u20hOq6OcrXDSvvpfeWxm4bu4uB9tPcy/SKE8YXJN3nptT+/XOR0so8RYgDd
+GGah2XsjX/GO1WfoVNpbOms2b/mBsTNHM3dA+VKq3dSDz4V4mZqTuXNnQkYRIer+
+CqkbGmVps4+uFrb2S1ayLfmlyOw7YqPta9BO1UAJpB+Y1zqlklkg5LB9zVtzaL1t
+xKITDmcZuI1CfmwMmm6gJC3VRRvcxAIU/oVbZZfKTpBQCHpCNfnqwmbU+AGuHrS+
+w6jv/naaoqYfRvaE7fzbzsQCzndILIyy7MMAo+wsVRjBfhnu4S/yrYObnqsZ38aK
+L4x35bcF7DvB7L6Gs4a8wPfc5+pbrrLMtTWGS9DiP7bY+A4A7l3j941Y/8+LN+lj
+X273CXE2whJdV/LItM3z7gLfEdxquVeEHVlNjM7IDiPCtyaaEBRx/pOyiriA8A4Q
+ntOoUAw3gi/q4Iqd4Sw5/7W0cwDk90imc6y/st53BIe0o82bNSQ3+pCTE4FCxpgm
+dTdmQRCsu/WU48IxK63nI1bMNSWSs1A=
+-----END CERTIFICATE-----
```

### Comparing `certifi-2023.7.22/certifi/core.py` & `certifi-2024.2.2/certifi/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """
 certifi.py
 ~~~~~~~~~~
 
 This module returns the installation location of cacert.pem or its contents.
 """
 import sys
+import atexit
+
+def exit_cacert_ctx() -> None:
+    _CACERT_CTX.__exit__(None, None, None)  # type: ignore[union-attr]
 
 
 if sys.version_info >= (3, 11):
 
     from importlib.resources import as_file, files
 
     _CACERT_CTX = None
@@ -31,14 +35,15 @@
             # return the file system location and the __exit__() is a no-op.
             #
             # We also have to hold onto the actual context manager, because
             # it will do the cleanup whenever it gets garbage collected, so
             # we will also store that at the global level as well.
             _CACERT_CTX = as_file(files("certifi").joinpath("cacert.pem"))
             _CACERT_PATH = str(_CACERT_CTX.__enter__())
+            atexit.register(exit_cacert_ctx)
 
         return _CACERT_PATH
 
     def contents() -> str:
         return files("certifi").joinpath("cacert.pem").read_text(encoding="ascii")
 
 elif sys.version_info >= (3, 7):
@@ -66,14 +71,15 @@
             # __exit__() is a no-op.
             #
             # We also have to hold onto the actual context manager, because
             # it will do the cleanup whenever it gets garbage collected, so
             # we will also store that at the global level as well.
             _CACERT_CTX = get_path("certifi", "cacert.pem")
             _CACERT_PATH = str(_CACERT_CTX.__enter__())
+            atexit.register(exit_cacert_ctx)
 
         return _CACERT_PATH
 
     def contents() -> str:
         return read_text("certifi", "cacert.pem", encoding="ascii")
 
 else:
```

### Comparing `certifi-2023.7.22/certifi.egg-info/PKG-INFO` & `certifi-2024.2.2/certifi.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: certifi
-Version: 2023.7.22
+Version: 2024.2.2
 Summary: Python package for providing Mozilla's CA Bundle.
 Home-page: https://github.com/certifi/python-certifi
 Author: Kenneth Reitz
 Author-email: me@kennethreitz.com
 License: MPL-2.0
 Project-URL: Source, https://github.com/certifi/python-certifi
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -61,9 +60,7 @@
 Addition/Removal of Certificates
 --------------------------------
 
 Certifi does not support any addition/removal or other modification of the
 CA trust store content. This project is intended to provide a reliable and
 highly portable root of trust to python deployments. Look to upstream projects
 for methods to use alternate trust.
-
-
```

### Comparing `certifi-2023.7.22/setup.py` & `certifi-2024.2.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,62 @@
 #!/usr/bin/env python
 import re
-import os
-import sys
 
 # While I generally consider it an antipattern to try and support both
 # setuptools and distutils with a single setup.py, in this specific instance
 # where certifi is a dependency of setuptools, it can create a circular
 # dependency when projects attempt to unbundle stuff from setuptools and pip.
 # Though we don't really support that, it makes things easier if we do this and
 # should hopefully cause less issues for end users.
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 
 version_regex = r'__version__ = ["\']([^"\']*)["\']'
-with open('certifi/__init__.py') as f:
+with open("certifi/__init__.py") as f:
     text = f.read()
     match = re.search(version_regex, text)
 
     if match:
         VERSION = match.group(1)
     else:
         raise RuntimeError("No version number found!")
 
-if sys.argv[-1] == 'publish':
-    os.system('python setup.py sdist bdist_wheel upload')
-    sys.exit()
-
 setup(
-    name='certifi',
+    name="certifi",
     version=VERSION,
-    description='Python package for providing Mozilla\'s CA Bundle.',
-    long_description=open('README.rst').read(),
-    author='Kenneth Reitz',
-    author_email='me@kennethreitz.com',
-    url='https://github.com/certifi/python-certifi',
+    description="Python package for providing Mozilla's CA Bundle.",
+    long_description=open("README.rst").read(),
+    author="Kenneth Reitz",
+    author_email="me@kennethreitz.com",
+    url="https://github.com/certifi/python-certifi",
     packages=[
-        'certifi',
+        "certifi",
     ],
-    package_dir={'certifi': 'certifi'},
-    package_data={'certifi': ['*.pem', 'py.typed']},
+    package_dir={"certifi": "certifi"},
+    package_data={"certifi": ["*.pem", "py.typed"]},
     # data_files=[('certifi', ['certifi/cacert.pem'])],
     include_package_data=True,
     zip_safe=False,
-    license='MPL-2.0',
+    license="MPL-2.0",
     python_requires=">=3.6",
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)',
-        'Natural Language :: English',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
+        "Natural Language :: English",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     project_urls={
-        'Source': 'https://github.com/certifi/python-certifi',
+        "Source": "https://github.com/certifi/python-certifi",
     },
 )
```

