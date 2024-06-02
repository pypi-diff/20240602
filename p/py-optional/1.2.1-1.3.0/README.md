# Comparing `tmp/py_optional-1.2.1.tar.gz` & `tmp/py_optional-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_optional-1.2.1.tar", max compression
+gzip compressed data, was "py_optional-1.3.0.tar", max compression
```

## Comparing `py_optional-1.2.1.tar` & `py_optional-1.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1075 2023-11-06 11:13:53.156543 py_optional-1.2.1/LICENSE
--rw-r--r--   0        0        0     3384 2023-11-06 11:13:53.156543 py_optional-1.2.1/README.md
--rw-r--r--   0        0        0      293 2023-11-06 11:13:53.156543 py_optional-1.2.1/optional/__init__.py
--rw-r--r--   0        0        0      109 2023-11-06 11:13:53.156543 py_optional-1.2.1/optional/exceptions.py
--rw-r--r--   0        0        0     7340 2023-11-06 11:13:53.156543 py_optional-1.2.1/optional/optional.py
--rw-r--r--   0        0        0     3769 2023-11-06 11:13:53.156543 py_optional-1.2.1/optional/optional_property.py
--rw-r--r--   0        0        0        0 2023-11-06 11:13:53.156543 py_optional-1.2.1/optional/py.typed
--rw-r--r--   0        0        0      900 2023-11-06 11:14:10.856495 py_optional-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3953 1970-01-01 00:00:00.000000 py_optional-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-06-02 16:41:07.321659 py_optional-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2512 2024-06-02 16:41:07.321659 py_optional-1.3.0/README.md
+-rw-r--r--   0        0        0      327 2024-06-02 16:41:07.325659 py_optional-1.3.0/optional/__init__.py
+-rw-r--r--   0        0        0      109 2024-06-02 16:41:07.325659 py_optional-1.3.0/optional/exceptions.py
+-rw-r--r--   0        0        0     8606 2024-06-02 16:41:07.325659 py_optional-1.3.0/optional/optional.py
+-rw-r--r--   0        0        0     3762 2024-06-02 16:41:07.325659 py_optional-1.3.0/optional/optional_property.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:41:07.325659 py_optional-1.3.0/optional/py.typed
+-rw-r--r--   0        0        0      881 2024-06-02 16:41:22.401882 py_optional-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 py_optional-1.3.0/PKG-INFO
```

### Comparing `py_optional-1.2.1/LICENSE` & `py_optional-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_optional-1.2.1/README.md` & `py_optional-1.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,212 +1,193 @@
-00000000: 2320 7079 2d6f 7074 696f 6e61 6c0a 0a3c  # py-optional..<
-00000010: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
-00000020: 3e0a 2020 2020 3c65 6d3e 4f70 7469 6f6e  >.    <em>Option
-00000030: 616c 2076 616c 7565 2069 6d70 6c65 6d65  al value impleme
-00000040: 6e74 6174 696f 6e20 666f 7220 7079 7468  ntation for pyth
-00000050: 6f6e 2e3c 2f65 6d3e 0a3c 2f70 3e0a 0a3c  on.</em>.</p>..<
-00000060: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
-00000070: 3e0a 3c61 2068 7265 663d 2268 7474 7073  >.<a href="https
-00000080: 3a2f 2f67 6974 6875 622e 636f 6d2f 6672  ://github.com/fr
-00000090: 616e 6369 7076 622f 7079 2d6f 7074 696f  ancipvb/py-optio
-000000a0: 6e61 6c2f 6163 7469 6f6e 733f 7175 6572  nal/actions?quer
-000000b0: 793d 776f 726b 666c 6f77 2533 4154 6573  y=workflow%3ATes
-000000c0: 7422 2074 6172 6765 743d 225f 626c 616e  t" target="_blan
-000000d0: 6b22 3e0a 2020 2020 3c69 6d67 2073 7263  k">.    <img src
-000000e0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-000000f0: 2e63 6f6d 2f66 7261 6e63 6970 7662 2f70  .com/francipvb/p
-00000100: 792d 6f70 7469 6f6e 616c 2f77 6f72 6b66  y-optional/workf
-00000110: 6c6f 7773 2f54 6573 742f 6261 6467 652e  lows/Test/badge.
-00000120: 7376 6722 2061 6c74 3d22 5465 7374 223e  svg" alt="Test">
-00000130: 0a3c 2f61 3e0a 3c61 2068 7265 663d 2268  .</a>.<a href="h
-00000140: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000150: 6d2f 6672 616e 6369 7076 622f 7079 2d6f  m/francipvb/py-o
-00000160: 7074 696f 6e61 6c2f 6163 7469 6f6e 733f  ptional/actions?
-00000170: 7175 6572 793d 776f 726b 666c 6f77 2533  query=workflow%3
-00000180: 4150 7562 6c69 7368 2220 7461 7267 6574  APublish" target
-00000190: 3d22 5f62 6c61 6e6b 223e 0a20 2020 203c  ="_blank">.    <
-000001a0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-000001b0: 2f67 6974 6875 622e 636f 6d2f 6672 616e  /github.com/fran
-000001c0: 6369 7076 622f 7079 2d6f 7074 696f 6e61  cipvb/py-optiona
-000001d0: 6c2f 776f 726b 666c 6f77 732f 5075 626c  l/workflows/Publ
-000001e0: 6973 682f 6261 6467 652e 7376 6722 2061  ish/badge.svg" a
-000001f0: 6c74 3d22 5075 626c 6973 6822 3e0a 3c2f  lt="Publish">.</
-00000200: 613e 0a3c 6120 6872 6566 3d22 6874 7470  a>.<a href="http
-00000210: 733a 2f2f 6465 7065 6e64 6162 6f74 2e63  s://dependabot.c
-00000220: 6f6d 2f22 2074 6172 6765 743d 225f 626c  om/" target="_bl
-00000230: 616e 6b22 3e0a 2020 2020 3c69 6d67 2073  ank">.    <img s
-00000240: 7263 3d22 6874 7470 733a 2f2f 666c 6174  rc="https://flat
-00000250: 2e62 6164 6765 6e2e 6e65 742f 6465 7065  .badgen.net/depe
-00000260: 6e64 6162 6f74 2f66 7261 6e63 6970 7662  ndabot/francipvb
-00000270: 2f70 792d 6f70 7469 6f6e 616c 3f69 636f  /py-optional?ico
-00000280: 6e3d 6465 7065 6e64 6162 6f74 2220 616c  n=dependabot" al
-00000290: 743d 2244 6570 656e 6461 626f 7420 456e  t="Dependabot En
-000002a0: 6162 6c65 6422 3e0a 3c2f 613e 0a3c 6120  abled">.</a>.<a 
-000002b0: 6872 6566 3d22 6874 7470 733a 2f2f 636f  href="https://co
-000002c0: 6465 636f 762e 696f 2f67 682f 6672 616e  decov.io/gh/fran
-000002d0: 6369 7076 622f 7079 2d6f 7074 696f 6e61  cipvb/py-optiona
-000002e0: 6c22 2074 6172 6765 743d 225f 626c 616e  l" target="_blan
-000002f0: 6b22 3e0a 2020 2020 3c69 6d67 2073 7263  k">.    <img src
-00000300: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00000310: 6965 6c64 732e 696f 2f63 6f64 6563 6f76  ields.io/codecov
-00000320: 2f63 2f67 6974 6875 622f 6672 616e 6369  /c/github/franci
-00000330: 7076 622f 7079 2d6f 7074 696f 6e61 6c3f  pvb/py-optional?
-00000340: 636f 6c6f 723d 2532 3333 3444 3035 3822  color=%2334D058"
-00000350: 2061 6c74 3d22 436f 7665 7261 6765 223e   alt="Coverage">
-00000360: 0a3c 2f61 3e0a 3c61 2068 7265 663d 2268  .</a>.<a href="h
-00000370: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00000380: 7072 6f6a 6563 742f 7079 2d6f 7074 696f  project/py-optio
-00000390: 6e61 6c22 2074 6172 6765 743d 225f 626c  nal" target="_bl
-000003a0: 616e 6b22 3e0a 2020 2020 3c69 6d67 2073  ank">.    <img s
-000003b0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-000003c0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-000003d0: 762f 7079 2d6f 7074 696f 6e61 6c3f 636f  v/py-optional?co
-000003e0: 6c6f 723d 2532 3333 3444 3035 3826 6c61  lor=%2334D058&la
-000003f0: 6265 6c3d 7079 7069 2532 3070 6163 6b61  bel=pypi%20packa
-00000400: 6765 2220 616c 743d 2250 6163 6b61 6765  ge" alt="Package
-00000410: 2076 6572 7369 6f6e 223e 0a3c 2f61 3e0a   version">.</a>.
-00000420: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000430: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00000440: 742f 7079 2d6f 7074 696f 6e61 6c2f 2220  t/py-optional/" 
-00000450: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00000460: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
-00000470: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000480: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
-00000490: 7369 6f6e 732f 7079 2d6f 7074 696f 6e61  sions/py-optiona
-000004a0: 6c2e 7376 6722 2061 6c74 3d22 5079 7468  l.svg" alt="Pyth
-000004b0: 6f6e 2056 6572 7369 6f6e 7322 3e0a 3c2f  on Versions">.</
-000004c0: 613e 0a0a 2323 2047 6574 7469 6e67 2073  a>..## Getting s
-000004d0: 7461 7274 6564 0a0a 5365 6520 5b44 6f63  tarted..See [Doc
-000004e0: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
-000004f0: 733a 2f2f 6672 616e 6369 7076 622e 6769  s://francipvb.gi
-00000500: 7468 7562 2e69 6f2f 7079 2d6f 7074 696f  thub.io/py-optio
-00000510: 6e61 6c2f 2920 666f 7220 6465 7461 696c  nal/) for detail
-00000520: 732e 0a0a 2323 2046 6561 7475 7265 730a  s...## Features.
-00000530: 0a2d 2050 6f65 7472 7920 2876 6972 7475  .- Poetry (virtu
-00000540: 616c 2065 6e76 6972 6f6e 6d65 6e74 2061  al environment a
-00000550: 6e64 2070 7562 6c69 7368 2074 6f20 5079  nd publish to Py
-00000560: 5069 2c20 616c 6c20 7769 7468 206f 6e65  Pi, all with one
-00000570: 2074 6f6f 6c29 0a2d 2062 6c61 636b 2028   tool).- black (
-00000580: 6c69 6e74 696e 672f 666f 726d 6174 7465  linting/formatte
-00000590: 7229 0a2d 2061 7574 6f66 6c61 6b65 2028  r).- autoflake (
-000005a0: 7265 6d6f 7669 6e67 2075 6e75 7365 6420  removing unused 
-000005b0: 7061 636b 6167 6573 290a 2d20 6973 6f72  packages).- isor
-000005c0: 7420 2864 6570 656e 6465 6e63 7920 6f72  t (dependency or
-000005d0: 6761 6e69 7a61 7469 6f6e 290a 2d20 6d79  ganization).- my
-000005e0: 7079 2028 7374 6174 6963 2074 7970 6520  py (static type 
-000005f0: 6368 6563 6b69 6e67 290a 2d20 7079 7465  checking).- pyte
-00000600: 7374 2028 696e 636c 7564 696e 6720 7465  st (including te
-00000610: 7374 2063 6f76 6572 6167 6529 0a2d 205b  st coverage).- [
-00000620: 7072 652d 636f 6d6d 6974 5d28 6874 7470  pre-commit](http
-00000630: 733a 2f2f 7072 652d 636f 6d6d 6974 2e63  s://pre-commit.c
-00000640: 6f6d 2f29 2028 686f 6f6b 7320 6f6e 2063  om/) (hooks on c
-00000650: 6f6d 6d69 7429 0a2d 2047 6974 4875 6220  ommit).- GitHub 
-00000660: 4163 7469 6f6e 7320 666f 7220 4349 2f43  Actions for CI/C
-00000670: 440a 2d20 6d6b 646f 6373 2066 6f72 2064  D.- mkdocs for d
-00000680: 6f63 756d 656e 7461 7469 6f6e 2028 7769  ocumentation (wi
-00000690: 7468 206d 6174 6572 6961 6c20 7468 656d  th material them
-000006a0: 6529 0a0a 2323 2049 6e73 7461 6c6c 696e  e)..## Installin
-000006b0: 6720 7079 2d6f 7074 696f 6e61 6c0a 0a49  g py-optional..I
-000006c0: 6e73 7461 6c6c 2074 6865 206c 6174 6573  nstall the lates
-000006d0: 7420 7265 6c65 6173 653a 0a0a 6060 6062  t release:..```b
-000006e0: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
-000006f0: 7079 2d6f 7074 696f 6e61 6c0a 6060 600a  py-optional.```.
-00000700: 0a4f 7220 796f 7520 6361 6e20 636c 6f6e  .Or you can clon
-00000710: 6520 6070 792d 6f70 7469 6f6e 616c 6020  e `py-optional` 
-00000720: 616e 6420 6765 7420 7374 6172 7465 6420  and get started 
-00000730: 6c6f 6361 6c6c 790a 0a60 6060 6261 7368  locally..```bash
-00000740: 0a0a 2320 656e 7375 7265 2079 6f75 2068  ..# ensure you h
-00000750: 6176 6520 506f 6574 7279 2069 6e73 7461  ave Poetry insta
-00000760: 6c6c 6564 0a70 6970 2069 6e73 7461 6c6c  lled.pip install
-00000770: 202d 2d75 7365 7220 706f 6574 7279 0a0a   --user poetry..
-00000780: 2320 696e 7374 616c 6c20 616c 6c20 6465  # install all de
-00000790: 7065 6e64 656e 6369 6573 2028 696e 636c  pendencies (incl
-000007a0: 7564 696e 6720 6465 7629 0a70 6f65 7472  uding dev).poetr
-000007b0: 7920 696e 7374 616c 6c0a 0a23 2064 6576  y install..# dev
-000007c0: 656c 6f70 210a 0a60 6060 0a0a 2323 2045  elop!..```..## E
-000007d0: 7861 6d70 6c65 2055 7361 6765 0a0a 6060  xample Usage..``
-000007e0: 6070 7974 686f 6e0a 696d 706f 7274 2070  `python.import p
-000007f0: 792d 6f70 7469 6f6e 616c 0a0a 2320 646f  y-optional..# do
-00000800: 2073 7475 6666 0a60 6060 0a0a 4f6e 6c79   stuff.```..Only
-00000810: 202a 2a50 7974 686f 6e20 332e 382b 2a2a   **Python 3.8+**
-00000820: 2069 7320 7375 7070 6f72 7465 6420 6173   is supported as
-00000830: 2072 6571 7569 7265 6420 6279 2074 6865   required by the
-00000840: 2062 6c61 636b 2c20 7079 6461 6e74 6963   black, pydantic
-00000850: 2070 6163 6b61 6765 730a 0a23 2320 5075   packages..## Pu
-00000860: 626c 6973 6869 6e67 2074 6f20 5079 7069  blishing to Pypi
-00000870: 0a0a 2323 2320 506f 6574 7279 2773 2064  ..### Poetry's d
-00000880: 6f63 756d 656e 7461 7469 6f6e 0a0a 4e6f  ocumentation..No
-00000890: 7465 2074 6861 7420 6974 2069 7320 7265  te that it is re
-000008a0: 636f 6d6d 656e 6465 6420 746f 2075 7365  commended to use
-000008b0: 205b 4150 4920 746f 6b65 6e73 5d28 6874   [API tokens](ht
-000008c0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f68  tps://pypi.org/h
-000008d0: 656c 702f 2361 7069 746f 6b65 6e29 2077  elp/#apitoken) w
-000008e0: 6865 6e20 7570 6c6f 6164 696e 6720 7061  hen uploading pa
-000008f0: 636b 6167 6573 2074 6f20 5079 5049 2e0a  ckages to PyPI..
-00000900: 0a3e 204f 6e63 6520 796f 7520 6861 7665  .> Once you have
-00000910: 2063 7265 6174 6564 2061 206e 6577 2074   created a new t
-00000920: 6f6b 656e 2c20 796f 7520 6361 6e20 7465  oken, you can te
-00000930: 6c6c 2050 6f65 7472 7920 746f 2075 7365  ll Poetry to use
-00000940: 2069 743a 0a0a 3c68 7474 7073 3a2f 2f70   it:..<https://p
-00000950: 7974 686f 6e2d 706f 6574 7279 2e6f 7267  ython-poetry.org
-00000960: 2f64 6f63 732f 7265 706f 7369 746f 7269  /docs/repositori
-00000970: 6573 2f23 636f 6e66 6967 7572 696e 672d  es/#configuring-
-00000980: 6372 6564 656e 7469 616c 733e 0a0a 5765  credentials>..We
-00000990: 2064 6f20 7468 6973 2075 7369 6e67 2047   do this using G
-000009a0: 6974 4875 6220 4163 7469 6f6e 7327 2057  itHub Actions' W
-000009b0: 6f72 6b66 6c6f 7773 2061 6e64 2052 6570  orkflows and Rep
-000009c0: 6f73 6974 6f72 7920 5365 6372 6574 7321  ository Secrets!
-000009d0: 0a0a 2323 2320 5265 706f 2053 6563 7265  ..### Repo Secre
-000009e0: 7473 0a0a 476f 2074 6f20 796f 7572 2072  ts..Go to your r
-000009f0: 6570 6f20 7365 7474 696e 6773 2061 6e64  epo settings and
-00000a00: 2061 6464 2061 2060 5059 5049 5f54 4f4b   add a `PYPI_TOK
-00000a10: 454e 6020 656e 7669 726f 6e6d 656e 7420  EN` environment 
-00000a20: 7661 7269 6162 6c65 3a0a 0a21 5b47 6974  variable:..![Git
-00000a30: 6875 6220 4163 7469 6f6e 7320 7365 7475  hub Actions setu
-00000a40: 7020 6f66 2050 6f65 7472 7920 746f 6b65  p of Poetry toke
-00000a50: 6e20 656e 7669 726f 6e6d 656e 7420 7661  n environment va
-00000a60: 7269 6162 6c65 5d28 696d 6167 6573 2f47  riable](images/G
-00000a70: 6974 6875 622d 5365 6372 6574 732d 5059  ithub-Secrets-PY
-00000a80: 5049 5f54 4f4b 454e 2d53 6574 7570 2e70  PI_TOKEN-Setup.p
-00000a90: 6e67 290a 0a23 2323 2049 6e73 7065 6374  ng)..### Inspect
-00000aa0: 2074 6865 2047 6974 4875 6220 4163 7469   the GitHub Acti
-00000ab0: 6f6e 7320 5075 626c 6973 6820 576f 726b  ons Publish Work
-00000ac0: 666c 6f77 730a 0a60 6060 796d 6c0a 6e61  flows..```yml.na
-00000ad0: 6d65 3a20 5075 626c 6973 680a 0a6f 6e3a  me: Publish..on:
-00000ae0: 0a20 2072 656c 6561 7365 3a0a 2020 2020  .  release:.    
-00000af0: 7479 7065 733a 0a20 2020 2020 202d 2063  types:.      - c
-00000b00: 7265 6174 6564 0a0a 6a6f 6273 3a0a 2020  reated..jobs:.  
-00000b10: 7075 626c 6973 683a 0a20 2020 2072 756e  publish:.    run
-00000b20: 732d 6f6e 3a20 7562 756e 7475 2d6c 6174  s-on: ubuntu-lat
-00000b30: 6573 740a 2020 2020 7374 6570 733a 0a20  est.    steps:. 
-00000b40: 2020 2020 202d 2075 7365 733a 2061 6374       - uses: act
-00000b50: 696f 6e73 2f63 6865 636b 6f75 7440 7632  ions/checkout@v2
-00000b60: 0a20 2020 2020 202e 2e2e 0a20 2020 2020  .      ....     
-00000b70: 202e 2e2e 0a20 2020 2020 202e 2e2e 0a20   ....      .... 
-00000b80: 2020 2020 202d 206e 616d 653a 2050 7562       - name: Pub
-00000b90: 6c69 7368 0a20 2020 2020 2020 2065 6e76  lish.        env
-00000ba0: 3a0a 2020 2020 2020 2020 2020 5059 5049  :.          PYPI
-00000bb0: 5f54 4f4b 454e 3a20 247b 7b20 7365 6372  _TOKEN: ${{ secr
-00000bc0: 6574 732e 5059 5049 5f54 4f4b 454e 207d  ets.PYPI_TOKEN }
-00000bd0: 7d0a 2020 2020 2020 2020 7275 6e3a 207c  }.        run: |
-00000be0: 0a20 2020 2020 2020 2020 2070 6f65 7472  .          poetr
-00000bf0: 7920 636f 6e66 6967 2070 7970 692d 746f  y config pypi-to
-00000c00: 6b65 6e2e 7079 7069 2024 5059 5049 5f54  ken.pypi $PYPI_T
-00000c10: 4f4b 454e 0a20 2020 2020 2020 2020 2062  OKEN.          b
-00000c20: 6173 6820 7363 7269 7074 732f 7075 626c  ash scripts/publ
-00000c30: 6973 682e 7368 0a60 6060 0a0a 3e20 5468  ish.sh.```..> Th
-00000c40: 6174 2773 2069 7421 0a0a 5768 656e 2079  at's it!..When y
-00000c50: 6f75 206d 616b 6520 6120 7265 6c65 6173  ou make a releas
-00000c60: 6520 6f6e 2047 6974 4875 622c 2074 6865  e on GitHub, the
-00000c70: 2070 7562 6c69 7368 2077 6f72 6b66 6c6f   publish workflo
-00000c80: 7720 7769 6c6c 2072 756e 2061 6e64 2064  w will run and d
-00000c90: 6570 6c6f 7920 746f 2050 7950 6921 20f0  eploy to PyPi! .
-00000ca0: 9f9a 80f0 9f8e 89f0 9f98 8e0a 0a23 2320  .............## 
-00000cb0: 436f 6e74 7269 6275 7469 6e67 2047 7569  Contributing Gui
-00000cc0: 6465 0a0a 5765 6c63 6f6d 6521 20f0 9f98  de..Welcome! ...
-00000cd0: 8af0 9f91 8b0a 0a3e 2050 6c65 6173 6520  .......> Please 
-00000ce0: 7365 6520 7468 6520 5b43 6f6e 7472 6962  see the [Contrib
-00000cf0: 7574 696e 6720 4775 6964 655d 2868 7474  uting Guide](htt
-00000d00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000d10: 6672 616e 6369 7076 622f 7079 2d6f 7074  francipvb/py-opt
-00000d20: 696f 6e61 6c2f 434f 4e54 5249 4255 5449  ional/CONTRIBUTI
-00000d30: 4e47 2e6d 6429 2e0a                      NG.md)..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 2d6f  : 2.1.Name: py-o
+00000020: 7074 696f 6e61 6c0a 5665 7273 696f 6e3a  ptional.Version:
+00000030: 2031 2e33 2e30 0a53 756d 6d61 7279 3a20   1.3.0.Summary: 
+00000040: 546f 6f6c 7320 746f 2063 6f6e 7665 7274  Tools to convert
+00000050: 2053 514c 416c 6368 656d 7920 6d6f 6465   SQLAlchemy mode
+00000060: 6c73 2074 6f20 5079 6461 6e74 6963 206d  ls to Pydantic m
+00000070: 6f64 656c 730a 4c69 6365 6e73 653a 204d  odels.License: M
+00000080: 4954 0a41 7574 686f 723a 2046 7261 6e63  IT.Author: Franc
+00000090: 6973 636f 2044 656c 2052 6f69 6f0a 4175  isco Del Roio.Au
+000000a0: 7468 6f72 2d65 6d61 696c 3a20 6672 616e  thor-email: fran
+000000b0: 6369 7076 6240 686f 746d 6169 6c2e 636f  cipvb@hotmail.co
+000000c0: 6d0a 5265 7175 6972 6573 2d50 7974 686f  m.Requires-Pytho
+000000d0: 6e3a 203e 3d33 2e38 2e31 2c3c 342e 302e  n: >=3.8.1,<4.0.
+000000e0: 300a 436c 6173 7369 6669 6572 3a20 4c69  0.Classifier: Li
+000000f0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+00000100: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
+00000110: 656e 7365 0a43 6c61 7373 6966 6965 723a  ense.Classifier:
+00000120: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000130: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000140: 3a3a 2033 0a43 6c61 7373 6966 6965 723a  :: 3.Classifier:
+00000150: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000160: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000170: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
+00000180: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000190: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001a0: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
+000001b0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000001c0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000001d0: 7468 6f6e 203a 3a20 332e 3131 0a52 6571  thon :: 3.11.Req
+000001e0: 7569 7265 732d 4469 7374 3a20 7479 7069  uires-Dist: typi
+000001f0: 6e67 2d65 7874 656e 7369 6f6e 7320 283e  ng-extensions (>
+00000200: 3d34 2e35 2e30 2c3c 352e 302e 3029 0a44  =4.5.0,<5.0.0).D
+00000210: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
+00000220: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
+00000230: 726b 646f 776e 0a0a 2320 7079 2d6f 7074  rkdown..# py-opt
+00000240: 696f 6e61 6c0a 0a5b 215b 436f 7665 7261  ional..[![Covera
+00000250: 6765 2053 7461 7475 735d 2868 7474 7073  ge Status](https
+00000260: 3a2f 2f63 6f76 6572 616c 6c73 2e69 6f2f  ://coveralls.io/
+00000270: 7265 706f 732f 6769 7468 7562 2f66 7261  repos/github/fra
+00000280: 6e63 6970 7662 2f70 792d 6f70 7469 6f6e  ncipvb/py-option
+00000290: 616c 2f62 6164 6765 2e73 7667 3f62 7261  al/badge.svg?bra
+000002a0: 6e63 683d 6465 7665 6c6f 7029 5d28 6874  nch=develop)](ht
+000002b0: 7470 733a 2f2f 636f 7665 7261 6c6c 732e  tps://coveralls.
+000002c0: 696f 2f67 6974 6875 622f 6672 616e 6369  io/github/franci
+000002d0: 7076 622f 7079 2d6f 7074 696f 6e61 6c3f  pvb/py-optional?
+000002e0: 6272 616e 6368 3d64 6576 656c 6f70 290a  branch=develop).
+000002f0: 5b21 5b43 6f76 6572 6167 6520 5374 6174  [![Coverage Stat
+00000300: 7573 5d28 6874 7470 733a 2f2f 636f 7665  us](https://cove
+00000310: 7261 6c6c 732e 696f 2f72 6570 6f73 2f67  ralls.io/repos/g
+00000320: 6974 6875 622f 6672 616e 6369 7076 622f  ithub/francipvb/
+00000330: 7079 2d6f 7074 696f 6e61 6c2f 6261 6467  py-optional/badg
+00000340: 652e 7376 673f 6272 616e 6368 3d6d 6169  e.svg?branch=mai
+00000350: 6e29 5d28 6874 7470 733a 2f2f 636f 7665  n)](https://cove
+00000360: 7261 6c6c 732e 696f 2f67 6974 6875 622f  ralls.io/github/
+00000370: 6672 616e 6369 7076 622f 7079 2d6f 7074  francipvb/py-opt
+00000380: 696f 6e61 6c3f 6272 616e 6368 3d6d 6169  ional?branch=mai
+00000390: 6e29 0a0a 2323 2047 6574 7469 6e67 2073  n)..## Getting s
+000003a0: 7461 7274 6564 0a0a 5365 6520 5b44 6f63  tarted..See [Doc
+000003b0: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
+000003c0: 733a 2f2f 6672 616e 6369 7076 622e 6769  s://francipvb.gi
+000003d0: 7468 7562 2e69 6f2f 7079 2d6f 7074 696f  thub.io/py-optio
+000003e0: 6e61 6c2f 2920 666f 7220 6465 7461 696c  nal/) for detail
+000003f0: 732e 0a0a 2323 2046 6561 7475 7265 730a  s...## Features.
+00000400: 0a2d 2050 6f65 7472 7920 2876 6972 7475  .- Poetry (virtu
+00000410: 616c 2065 6e76 6972 6f6e 6d65 6e74 2061  al environment a
+00000420: 6e64 2070 7562 6c69 7368 2074 6f20 5079  nd publish to Py
+00000430: 5069 2c20 616c 6c20 7769 7468 206f 6e65  Pi, all with one
+00000440: 2074 6f6f 6c29 0a2d 2062 6c61 636b 2028   tool).- black (
+00000450: 6c69 6e74 696e 672f 666f 726d 6174 7465  linting/formatte
+00000460: 7229 0a2d 2061 7574 6f66 6c61 6b65 2028  r).- autoflake (
+00000470: 7265 6d6f 7669 6e67 2075 6e75 7365 6420  removing unused 
+00000480: 7061 636b 6167 6573 290a 2d20 6973 6f72  packages).- isor
+00000490: 7420 2864 6570 656e 6465 6e63 7920 6f72  t (dependency or
+000004a0: 6761 6e69 7a61 7469 6f6e 290a 2d20 6d79  ganization).- my
+000004b0: 7079 2028 7374 6174 6963 2074 7970 6520  py (static type 
+000004c0: 6368 6563 6b69 6e67 290a 2d20 7079 7465  checking).- pyte
+000004d0: 7374 2028 696e 636c 7564 696e 6720 7465  st (including te
+000004e0: 7374 2063 6f76 6572 6167 6529 0a2d 205b  st coverage).- [
+000004f0: 7072 652d 636f 6d6d 6974 5d28 6874 7470  pre-commit](http
+00000500: 733a 2f2f 7072 652d 636f 6d6d 6974 2e63  s://pre-commit.c
+00000510: 6f6d 2f29 2028 686f 6f6b 7320 6f6e 2063  om/) (hooks on c
+00000520: 6f6d 6d69 7429 0a2d 2047 6974 4875 6220  ommit).- GitHub 
+00000530: 4163 7469 6f6e 7320 666f 7220 4349 2f43  Actions for CI/C
+00000540: 440a 2d20 6d6b 646f 6373 2066 6f72 2064  D.- mkdocs for d
+00000550: 6f63 756d 656e 7461 7469 6f6e 2028 7769  ocumentation (wi
+00000560: 7468 206d 6174 6572 6961 6c20 7468 656d  th material them
+00000570: 6529 0a0a 2323 2049 6e73 7461 6c6c 696e  e)..## Installin
+00000580: 6720 7079 2d6f 7074 696f 6e61 6c0a 0a49  g py-optional..I
+00000590: 6e73 7461 6c6c 2074 6865 206c 6174 6573  nstall the lates
+000005a0: 7420 7265 6c65 6173 653a 0a0a 6060 6062  t release:..```b
+000005b0: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
+000005c0: 7079 2d6f 7074 696f 6e61 6c0a 6060 600a  py-optional.```.
+000005d0: 0a4f 7220 796f 7520 6361 6e20 636c 6f6e  .Or you can clon
+000005e0: 6520 6070 792d 6f70 7469 6f6e 616c 6020  e `py-optional` 
+000005f0: 616e 6420 6765 7420 7374 6172 7465 6420  and get started 
+00000600: 6c6f 6361 6c6c 790a 0a60 6060 6261 7368  locally..```bash
+00000610: 0a0a 2320 656e 7375 7265 2079 6f75 2068  ..# ensure you h
+00000620: 6176 6520 506f 6574 7279 2069 6e73 7461  ave Poetry insta
+00000630: 6c6c 6564 0a70 6970 2069 6e73 7461 6c6c  lled.pip install
+00000640: 202d 2d75 7365 7220 706f 6574 7279 0a0a   --user poetry..
+00000650: 2320 696e 7374 616c 6c20 616c 6c20 6465  # install all de
+00000660: 7065 6e64 656e 6369 6573 2028 696e 636c  pendencies (incl
+00000670: 7564 696e 6720 6465 7629 0a70 6f65 7472  uding dev).poetr
+00000680: 7920 696e 7374 616c 6c0a 0a23 2064 6576  y install..# dev
+00000690: 656c 6f70 210a 0a60 6060 0a0a 2323 2045  elop!..```..## E
+000006a0: 7861 6d70 6c65 2055 7361 6765 0a0a 6060  xample Usage..``
+000006b0: 6070 7974 686f 6e0a 696d 706f 7274 2070  `python.import p
+000006c0: 792d 6f70 7469 6f6e 616c 0a0a 2320 646f  y-optional..# do
+000006d0: 2073 7475 6666 0a60 6060 0a0a 4f6e 6c79   stuff.```..Only
+000006e0: 202a 2a50 7974 686f 6e20 332e 382b 2a2a   **Python 3.8+**
+000006f0: 2069 7320 7375 7070 6f72 7465 6420 6173   is supported as
+00000700: 2072 6571 7569 7265 6420 6279 2074 6865   required by the
+00000710: 2062 6c61 636b 2c20 7079 6461 6e74 6963   black, pydantic
+00000720: 2070 6163 6b61 6765 730a 0a23 2320 5075   packages..## Pu
+00000730: 626c 6973 6869 6e67 2074 6f20 5079 7069  blishing to Pypi
+00000740: 0a0a 2323 2320 506f 6574 7279 2773 2064  ..### Poetry's d
+00000750: 6f63 756d 656e 7461 7469 6f6e 0a0a 4e6f  ocumentation..No
+00000760: 7465 2074 6861 7420 6974 2069 7320 7265  te that it is re
+00000770: 636f 6d6d 656e 6465 6420 746f 2075 7365  commended to use
+00000780: 205b 4150 4920 746f 6b65 6e73 5d28 6874   [API tokens](ht
+00000790: 7470 733a 2f2f 7079 7069 2e6f 7267 2f68  tps://pypi.org/h
+000007a0: 656c 702f 2361 7069 746f 6b65 6e29 2077  elp/#apitoken) w
+000007b0: 6865 6e20 7570 6c6f 6164 696e 6720 7061  hen uploading pa
+000007c0: 636b 6167 6573 2074 6f20 5079 5049 2e0a  ckages to PyPI..
+000007d0: 0a3e 204f 6e63 6520 796f 7520 6861 7665  .> Once you have
+000007e0: 2063 7265 6174 6564 2061 206e 6577 2074   created a new t
+000007f0: 6f6b 656e 2c20 796f 7520 6361 6e20 7465  oken, you can te
+00000800: 6c6c 2050 6f65 7472 7920 746f 2075 7365  ll Poetry to use
+00000810: 2069 743a 0a0a 3c68 7474 7073 3a2f 2f70   it:..<https://p
+00000820: 7974 686f 6e2d 706f 6574 7279 2e6f 7267  ython-poetry.org
+00000830: 2f64 6f63 732f 7265 706f 7369 746f 7269  /docs/repositori
+00000840: 6573 2f23 636f 6e66 6967 7572 696e 672d  es/#configuring-
+00000850: 6372 6564 656e 7469 616c 733e 0a0a 5765  credentials>..We
+00000860: 2064 6f20 7468 6973 2075 7369 6e67 2047   do this using G
+00000870: 6974 4875 6220 4163 7469 6f6e 7327 2057  itHub Actions' W
+00000880: 6f72 6b66 6c6f 7773 2061 6e64 2052 6570  orkflows and Rep
+00000890: 6f73 6974 6f72 7920 5365 6372 6574 7321  ository Secrets!
+000008a0: 0a0a 2323 2320 5265 706f 2053 6563 7265  ..### Repo Secre
+000008b0: 7473 0a0a 476f 2074 6f20 796f 7572 2072  ts..Go to your r
+000008c0: 6570 6f20 7365 7474 696e 6773 2061 6e64  epo settings and
+000008d0: 2061 6464 2061 2060 5059 5049 5f54 4f4b   add a `PYPI_TOK
+000008e0: 454e 6020 656e 7669 726f 6e6d 656e 7420  EN` environment 
+000008f0: 7661 7269 6162 6c65 3a0a 0a21 5b47 6974  variable:..![Git
+00000900: 6875 6220 4163 7469 6f6e 7320 7365 7475  hub Actions setu
+00000910: 7020 6f66 2050 6f65 7472 7920 746f 6b65  p of Poetry toke
+00000920: 6e20 656e 7669 726f 6e6d 656e 7420 7661  n environment va
+00000930: 7269 6162 6c65 5d28 696d 6167 6573 2f47  riable](images/G
+00000940: 6974 6875 622d 5365 6372 6574 732d 5059  ithub-Secrets-PY
+00000950: 5049 5f54 4f4b 454e 2d53 6574 7570 2e70  PI_TOKEN-Setup.p
+00000960: 6e67 290a 0a23 2323 2049 6e73 7065 6374  ng)..### Inspect
+00000970: 2074 6865 2047 6974 4875 6220 4163 7469   the GitHub Acti
+00000980: 6f6e 7320 5075 626c 6973 6820 576f 726b  ons Publish Work
+00000990: 666c 6f77 730a 0a60 6060 796d 6c0a 6e61  flows..```yml.na
+000009a0: 6d65 3a20 5075 626c 6973 680a 0a6f 6e3a  me: Publish..on:
+000009b0: 0a20 2072 656c 6561 7365 3a0a 2020 2020  .  release:.    
+000009c0: 7479 7065 733a 0a20 2020 2020 202d 2063  types:.      - c
+000009d0: 7265 6174 6564 0a0a 6a6f 6273 3a0a 2020  reated..jobs:.  
+000009e0: 7075 626c 6973 683a 0a20 2020 2072 756e  publish:.    run
+000009f0: 732d 6f6e 3a20 7562 756e 7475 2d6c 6174  s-on: ubuntu-lat
+00000a00: 6573 740a 2020 2020 7374 6570 733a 0a20  est.    steps:. 
+00000a10: 2020 2020 202d 2075 7365 733a 2061 6374       - uses: act
+00000a20: 696f 6e73 2f63 6865 636b 6f75 7440 7632  ions/checkout@v2
+00000a30: 0a20 2020 2020 202e 2e2e 0a20 2020 2020  .      ....     
+00000a40: 202e 2e2e 0a20 2020 2020 202e 2e2e 0a20   ....      .... 
+00000a50: 2020 2020 202d 206e 616d 653a 2050 7562       - name: Pub
+00000a60: 6c69 7368 0a20 2020 2020 2020 2065 6e76  lish.        env
+00000a70: 3a0a 2020 2020 2020 2020 2020 5059 5049  :.          PYPI
+00000a80: 5f54 4f4b 454e 3a20 247b 7b20 7365 6372  _TOKEN: ${{ secr
+00000a90: 6574 732e 5059 5049 5f54 4f4b 454e 207d  ets.PYPI_TOKEN }
+00000aa0: 7d0a 2020 2020 2020 2020 7275 6e3a 207c  }.        run: |
+00000ab0: 0a20 2020 2020 2020 2020 2070 6f65 7472  .          poetr
+00000ac0: 7920 636f 6e66 6967 2070 7970 692d 746f  y config pypi-to
+00000ad0: 6b65 6e2e 7079 7069 2024 5059 5049 5f54  ken.pypi $PYPI_T
+00000ae0: 4f4b 454e 0a20 2020 2020 2020 2020 2062  OKEN.          b
+00000af0: 6173 6820 7363 7269 7074 732f 7075 626c  ash scripts/publ
+00000b00: 6973 682e 7368 0a60 6060 0a0a 3e20 5468  ish.sh.```..> Th
+00000b10: 6174 2773 2069 7421 0a0a 5768 656e 2079  at's it!..When y
+00000b20: 6f75 206d 616b 6520 6120 7265 6c65 6173  ou make a releas
+00000b30: 6520 6f6e 2047 6974 4875 622c 2074 6865  e on GitHub, the
+00000b40: 2070 7562 6c69 7368 2077 6f72 6b66 6c6f   publish workflo
+00000b50: 7720 7769 6c6c 2072 756e 2061 6e64 2064  w will run and d
+00000b60: 6570 6c6f 7920 746f 2050 7950 6921 20f0  eploy to PyPi! .
+00000b70: 9f9a 80f0 9f8e 89f0 9f98 8e0a 0a23 2320  .............## 
+00000b80: 436f 6e74 7269 6275 7469 6e67 2047 7569  Contributing Gui
+00000b90: 6465 0a0a 5765 6c63 6f6d 6521 20f0 9f98  de..Welcome! ...
+00000ba0: 8af0 9f91 8b0a 0a3e 2050 6c65 6173 6520  .......> Please 
+00000bb0: 7365 6520 7468 6520 5b43 6f6e 7472 6962  see the [Contrib
+00000bc0: 7574 696e 6720 4775 6964 655d 2868 7474  uting Guide](htt
+00000bd0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000be0: 6672 616e 6369 7076 622f 7079 2d6f 7074  francipvb/py-opt
+00000bf0: 696f 6e61 6c2f 434f 4e54 5249 4255 5449  ional/CONTRIBUTI
+00000c00: 4e47 2e6d 6429 2e0a 0a                   NG.md)...
```

### Comparing `py_optional-1.2.1/optional/optional.py` & `py_optional-1.3.0/optional/optional.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """The optional object implementation.
 
 This module has the implementations for the **Optional** object.
 """
+
 from __future__ import annotations
 
 import abc
 import typing
+
+import typing_extensions
+
 from .exceptions import ValueNotProvidedError
 
 _T = typing.TypeVar("_T")
 _TR = typing.TypeVar("_TR")
 
 
 class Optional(abc.ABC, typing.Generic[_T]):
-    """An optional value wrapper.
+    """Represents an optional value.
 
-    An **Optional** object is never constructed directly. Insthead, there are methods to
-    build them.
-
-    See the [of][optional.Optional.of] and
-    [empty][optional.Optional.empty] methods.
+    See the [of][optional.Of] and
+    [empty][optional.Empty] classes.
     """
 
     __slots__ = ()
 
     @property
     @abc.abstractmethod
     def value(self) -> _T:  # pragma: nocover
@@ -55,15 +56,15 @@
     def is_empty(self) -> bool:
         """Get wether this instance is empty
 
         This just returns the opposite of
         [has_value][optional.optional.Optional.has_value].
 
         Returns:
-            bool: `True` if the value is not present, `False` otherwise
+            `True` if the value is not present, `False` otherwise
         """
         return not self.has_value
 
     @typing.final
     def or_else(self, value: _T) -> Optional[_T]:
         """Return an optional value wrapping this.
 
@@ -142,84 +143,130 @@
         """
         if self.has_value:
             await func(self.value)
         elif if_empty is not None:
             await if_empty()
 
     @staticmethod
-    def of(value: _T) -> Optional[_T]:
+    @typing_extensions.deprecated("Use `optional.Of` class directly.")
+    def of(value: typing.Any) -> Optional[typing.Any]:  # pragma: nocover
         """Build an [Optional][optional.Optional] object.
 
+        This method is deprecated. Use [Of][optional.optional.Of] class directly.
+
         Args:
             value: The value to wrap
 
         Returns:
             The [Optional] wrapper.
         """
-        return _Value(value)
+        return Of(value)
 
     @staticmethod
-    def empty() -> Optional[typing.Any]:
+    @typing_extensions.deprecated("Please use `Optional.Empty` directly.")
+    def empty() -> Optional[typing.Any]:  # pragma: nocover
         """Build an empty [Optional][optional.optional.Optional] object.
 
+        This method is deprecated. Use [Empty][optional.optional.Empty] class directly.
+
         Returns:
             An empty optional instance
         """
-        return _Empty()
+        return Empty()
 
     def __eq__(self, __value: typing.Any) -> bool:
-        if type(__value) != type(self):
+        if not isinstance(__value, type(self)):
             return NotImplemented
 
         if self.has_value and __value.has_value:
             # Delegate comparison to value implementations itself.
             return self.value == __value.value
 
         # Compare the `has_value` property:
         return self.has_value == __value.has_value
 
     def __bool__(self) -> bool:
         return self.has_value
 
 
-class _Empty(Optional[_T], typing.Generic[_T]):
+class Empty(Optional[typing.Any]):
+    """Represents an optional empty value.
+
+    This is ideal to put in function argument default values as this object does not hold any data and therefore is not mutable.
+
+    Usage example:
+
+    ```python
+    from optional import Optional, Empty, Of
+
+
+    def multiply(optional_value: Optional[int]=Empty(), multiplier: Optional[int]=Empty()) -> int:
+        return optional_value.or_else(2).value * multiplier.or_else(2).value
+
+    ```
+    """
+
     @typing.final
     @property
-    def value(self) -> _T:
+    def value(self) -> typing.Any:
         raise ValueNotProvidedError("Value were not provided.")
 
     @typing.final
     @property
     def has_value(self) -> bool:
         return False
 
     def __repr__(self) -> str:
-        return "Optional.empty()"
+        return f"{self.__class__.__name__}()"
 
     def __str__(self) -> str:
         return "empty"
 
 
-class _Value(Optional[_T], typing.Generic[_T]):
+class Of(Optional[_T], typing.Generic[_T]):
+    """An optional value wrapper.
+
+    This is an optional value wrapping a concrete value.
+
+    Example usage:
+    ```python
+    from optional import Optional, Empty, Of
+
+    def update_something(entity_id: int, *, name: Optional[str]=Empty())->bool:
+        if name:
+            print(f"Setting name to {name.value}")
+            return True
+        return False
+
+    update_something(1, name=Of("Karl"))
+    ```
+
+    Note that this is not like the python `None` value. This can hold `None` values too
+
+    Args:
+        value: The value to wrap
+
+    """
+
     __slots__ = ("_value",)
 
-    def __init__(self, value: _T) -> None:
+    def __init__(self, value: _T, /) -> None:
         super().__init__()
         self._value = value
 
     @property
     def value(self) -> _T:
         return self._value
 
     @property
     def has_value(self) -> bool:
         return True
 
     def __repr__(self) -> str:
-        return f"Optional[{type(self.value).__qualname__}].of({self.value!r})"
+        return f"{type(self).__name__}({self.value!r})"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
 class _Mapped(Optional[_TR], typing.Generic[_T, _TR]):
     __slots__ = ("_mapped", "_mapper", "_value", "_value_set")
```

### Comparing `py_optional-1.2.1/optional/optional_property.py` & `py_optional-1.3.0/optional/optional_property.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import weakref
 from collections.abc import Callable
 from dataclasses import dataclass, field
 from typing import Any, Generic, TypeVar, overload
 
 from typing_extensions import Self
 
-from .optional import Optional
+from .optional import Empty, Of, Optional
 
 _V = TypeVar("_V")
 
 
 class OptionalProperty(Generic[_V]):
     """An optional property.
 
@@ -77,15 +77,15 @@
             entry = self._entry(instance)
             if entry.value.has_value:
                 return entry.value.value
             return self.__func__(instance)
         return self
 
     def __set__(self, __instance: Any, __value: _V) -> None:
-        self._entry(__instance).value = Optional.of(__value)
+        self._entry(__instance).value = Of(__value)
 
     def _entry(self, obj: object) -> _Entry[_V]:
         entry = self._values.get(id(obj))
         if entry is None:
 
             def _finalyze(x: int) -> None:
                 if x in self._values:
@@ -120,15 +120,15 @@
         """
         return self._entry(obj).value
 
 
 @dataclass()
 class _Entry(Generic[_V]):
     finalizer: weakref.finalize
-    value: Optional[_V] = field(default_factory=Optional.empty)
+    value: Optional[_V] = field(default_factory=Empty)
 
 
 def optionalproperty(func: Callable[[Any], _V]) -> OptionalProperty[_V]:
     """Alias for [OptionalProperty][optional.OptionalProperty].
 
     Args:
         func: The default value supplier.
```

### Comparing `py_optional-1.2.1/pyproject.toml` & `py_optional-1.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 [tool.poetry]
 name = "py-optional"
-version = "1.2.1"
+version = "1.3.0"
 description = "Tools to convert SQLAlchemy models to Pydantic models"
 authors = ["Francisco Del Roio <francipvb@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "optional" }]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 typing-extensions = "^4.5.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.1.1"
-black = "^23.1.0"
+black = "^24.4.2"
 isort = "^5.12.0"
 autoflake = "^2.0.2"
 flake8 = "^6.0.0"
-pre-commit = "^3.2.1"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 mkdocs = "^1.4.2"
-mkdocs-material = "9.1.6"
+mkdocs-material = "^9.1.6"
 markdown-include = "^0.8.1"
-mkdocstrings = { extras = ["python"], version = "^0.21.2" }
+mkdocstrings = { extras = ["python"], version = "^0.25.0" }
 anyio = "^3.6.2"
-uvloop = "^0.17.0"
 dunamai = "^1.16.0"
+pyright = "^1.1.365"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.isort]
 known_third_party = ["optional"]
```

