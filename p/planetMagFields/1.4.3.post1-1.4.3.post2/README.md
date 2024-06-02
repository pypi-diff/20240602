# Comparing `tmp/planetmagfields-1.4.3.post1.tar.gz` & `tmp/planetmagfields-1.4.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmagfields-1.4.3.post1.tar", last modified: Fri May 10 02:44:27 2024, max compression
+gzip compressed data, was "planetmagfields-1.4.3.post2.tar", last modified: Sun Jun  2 04:03:26 2024, max compression
```

## Comparing `planetmagfields-1.4.3.post1.tar` & `planetmagfields-1.4.3.post2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-10 02:44:27.880518 planetmagfields-1.4.3.post1/
--rw-r--r--   0 ankit     (1000) ankit     (1000)    35149 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post1/LICENSE
--rw-r--r--   0 ankit     (1000) ankit     (1000)     8676 2024-05-10 02:44:27.880518 planetmagfields-1.4.3.post1/PKG-INFO
--rw-r--r--   0 ankit     (1000) ankit     (1000)     7156 2024-05-10 02:41:59.000000 planetmagfields-1.4.3.post1/README.md
-drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-10 02:44:27.880518 planetmagfields-1.4.3.post1/planetMagFields.egg-info/
--rw-r--r--   0 ankit     (1000) ankit     (1000)     8676 2024-05-10 02:44:27.000000 planetmagfields-1.4.3.post1/planetMagFields.egg-info/PKG-INFO
--rw-r--r--   0 ankit     (1000) ankit     (1000)     1094 2024-05-10 02:44:27.000000 planetmagfields-1.4.3.post1/planetMagFields.egg-info/SOURCES.txt
--rw-r--r--   0 ankit     (1000) ankit     (1000)        1 2024-05-10 02:44:27.000000 planetmagfields-1.4.3.post1/planetMagFields.egg-info/dependency_links.txt
--rw-r--r--   0 ankit     (1000) ankit     (1000)       56 2024-05-10 02:44:27.000000 planetmagfields-1.4.3.post1/planetMagFields.egg-info/requires.txt
--rw-r--r--   0 ankit     (1000) ankit     (1000)       16 2024-05-10 02:44:27.000000 planetmagfields-1.4.3.post1/planetMagFields.egg-info/top_level.txt
-drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-10 02:44:27.860518 planetmagfields-1.4.3.post1/planetmagfields/
--rw-r--r--   0 ankit     (1000) ankit     (1000)      159 2024-05-06 04:12:55.000000 planetmagfields-1.4.3.post1/planetmagfields/__init__.py
-drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-10 02:44:27.870518 planetmagfields-1.4.3.post1/planetmagfields/data/
--rw-r--r--   0 ankit     (1000) ankit     (1000)    39975 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post1/planetmagfields/data/earth_igrf13.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      109 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post1/planetmagfields/data/ganymede_kivelson2002.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)     3600 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post1/planetmagfields/data/jupiter_jrm09.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)    29760 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post1/planetmagfields/data/jupiter_jrm33.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      340 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post1/planetmagfields/data/jupiter_vip4.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)       46 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post1/planetmagfields/data/mercury_anderson2012.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      157 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post1/planetmagfields/data/mercury_thebault2018.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      161 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post1/planetmagfields/data/mercury_wardinski2019.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      167 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post1/planetmagfields/data/neptune_connerny1991.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      169 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post1/planetmagfields/data/saturn_cassini11+.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      153 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post1/planetmagfields/data/saturn_cassini11.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)       37 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post1/planetmagfields/data/saturn_cassinisoi.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      176 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post1/planetmagfields/data/uranus_connerny1987.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)     4701 2024-02-26 00:30:26.000000 planetmagfields-1.4.3.post1/planetmagfields/libbfield.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)     3863 2024-02-26 01:09:53.000000 planetmagfields-1.4.3.post1/planetmagfields/libdata.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)    14085 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post1/planetmagfields/libgauss.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)    11746 2024-04-30 14:44:50.000000 planetmagfields-1.4.3.post1/planetmagfields/planet.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)     6725 2024-04-30 14:45:13.000000 planetmagfields-1.4.3.post1/planetmagfields/plotlib.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)     7835 2024-04-30 19:32:35.000000 planetmagfields-1.4.3.post1/planetmagfields/potextra.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)     1030 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post1/planetmagfields/utils.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)     1564 2024-05-10 02:43:31.000000 planetmagfields-1.4.3.post1/pyproject.toml
--rw-r--r--   0 ankit     (1000) ankit     (1000)       38 2024-05-10 02:44:27.880518 planetmagfields-1.4.3.post1/setup.cfg
--rw-r--r--   0 ankit     (1000) ankit     (1000)     1229 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post1/setup.py
-drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-10 02:44:27.880518 planetmagfields-1.4.3.post1/tests/
--rw-r--r--   0 ankit     (1000) ankit     (1000)      446 2024-04-30 18:47:40.000000 planetmagfields-1.4.3.post1/tests/test_earthBr.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)      702 2024-04-30 19:43:11.000000 planetmagfields-1.4.3.post1/tests/test_potextra.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)     1558 2024-04-30 20:14:46.000000 planetmagfields-1.4.3.post1/tests/test_read.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)      420 2024-04-30 20:52:34.000000 planetmagfields-1.4.3.post1/tests/test_vtk.py
+drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-06-02 04:03:26.144463 planetmagfields-1.4.3.post2/
+-rw-r--r--   0 ankit     (1000) ankit     (1000)    35149 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post2/LICENSE
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     9478 2024-06-02 04:03:26.144463 planetmagfields-1.4.3.post2/PKG-INFO
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     7958 2024-06-02 03:49:57.000000 planetmagfields-1.4.3.post2/README.md
+drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-06-02 04:03:26.144463 planetmagfields-1.4.3.post2/planetMagFields.egg-info/
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     9478 2024-06-02 04:03:26.000000 planetmagfields-1.4.3.post2/planetMagFields.egg-info/PKG-INFO
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     1094 2024-06-02 04:03:26.000000 planetmagfields-1.4.3.post2/planetMagFields.egg-info/SOURCES.txt
+-rw-r--r--   0 ankit     (1000) ankit     (1000)        1 2024-06-02 04:03:26.000000 planetmagfields-1.4.3.post2/planetMagFields.egg-info/dependency_links.txt
+-rw-r--r--   0 ankit     (1000) ankit     (1000)       56 2024-06-02 04:03:26.000000 planetmagfields-1.4.3.post2/planetMagFields.egg-info/requires.txt
+-rw-r--r--   0 ankit     (1000) ankit     (1000)       16 2024-06-02 04:03:26.000000 planetmagfields-1.4.3.post2/planetMagFields.egg-info/top_level.txt
+drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-06-02 04:03:26.124463 planetmagfields-1.4.3.post2/planetmagfields/
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      159 2024-05-06 04:12:55.000000 planetmagfields-1.4.3.post2/planetmagfields/__init__.py
+drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-06-02 04:03:26.134463 planetmagfields-1.4.3.post2/planetmagfields/data/
+-rw-r--r--   0 ankit     (1000) ankit     (1000)    39975 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post2/planetmagfields/data/earth_igrf13.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      109 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post2/planetmagfields/data/ganymede_kivelson2002.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     3600 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post2/planetmagfields/data/jupiter_jrm09.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)    29760 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post2/planetmagfields/data/jupiter_jrm33.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      340 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post2/planetmagfields/data/jupiter_vip4.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)       46 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post2/planetmagfields/data/mercury_anderson2012.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      157 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post2/planetmagfields/data/mercury_thebault2018.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      161 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post2/planetmagfields/data/mercury_wardinski2019.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      167 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post2/planetmagfields/data/neptune_connerny1991.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      169 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post2/planetmagfields/data/saturn_cassini11+.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      153 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post2/planetmagfields/data/saturn_cassini11.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)       37 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post2/planetmagfields/data/saturn_cassinisoi.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      176 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post2/planetmagfields/data/uranus_connerny1987.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     4701 2024-02-26 00:30:26.000000 planetmagfields-1.4.3.post2/planetmagfields/libbfield.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     3863 2024-02-26 01:09:53.000000 planetmagfields-1.4.3.post2/planetmagfields/libdata.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)    14085 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post2/planetmagfields/libgauss.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)    11746 2024-04-30 14:44:50.000000 planetmagfields-1.4.3.post2/planetmagfields/planet.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     6725 2024-04-30 14:45:13.000000 planetmagfields-1.4.3.post2/planetmagfields/plotlib.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     7835 2024-04-30 19:32:35.000000 planetmagfields-1.4.3.post2/planetmagfields/potextra.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     1030 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post2/planetmagfields/utils.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     1564 2024-06-02 04:02:52.000000 planetmagfields-1.4.3.post2/pyproject.toml
+-rw-r--r--   0 ankit     (1000) ankit     (1000)       38 2024-06-02 04:03:26.144463 planetmagfields-1.4.3.post2/setup.cfg
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     1229 2024-02-22 17:26:25.000000 planetmagfields-1.4.3.post2/setup.py
+drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-06-02 04:03:26.144463 planetmagfields-1.4.3.post2/tests/
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      446 2024-04-30 18:47:40.000000 planetmagfields-1.4.3.post2/tests/test_earthBr.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      702 2024-04-30 19:43:11.000000 planetmagfields-1.4.3.post2/tests/test_potextra.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     1558 2024-04-30 20:14:46.000000 planetmagfields-1.4.3.post2/tests/test_read.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      420 2024-04-30 20:52:34.000000 planetmagfields-1.4.3.post2/tests/test_vtk.py
```

### Comparing `planetmagfields-1.4.3.post1/LICENSE` & `planetmagfields-1.4.3.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.3.post1/PKG-INFO` & `planetmagfields-1.4.3.post2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetMagFields
-Version: 1.4.3.post1
+Version: 1.4.3.post2
 Summary: Routines to easily access information about magnetic fields of planets in our solar system and visualize them in both 2D and 3D
 Author: Barik, Ankit
 Author-email: Ankit Barik <ankit.barik@gmail.com>
 Maintainer-email: Ankit Barik <ankit.barik@gmail.com>, Regupathi Angappan <rangapp1@jhu.edu>
 Project-URL: Homepage, https://ankitbarik.github.io/planetMagFields/
 Project-URL: Issues, https://github.com/AnkitBarik/planetMagFields/issues
 Keywords: Spherical Harmonics,Planetary Science,Spectra,Magnetic Field,Visualization,3D visualization
@@ -49,14 +49,16 @@
 
 [Jupyter notebook](#jupyter-notebook)
 
 [Documentation](#documentation)
 
 [Code contribution and reporting issues](#code-contribution-and-reporting-issues)
 
+[Citing `planetMagFields`](#citing-planetmagfields)
+
 [Acknowledgements](#acknowledgements)
 
 # Prerequisites
 
 `planetMagFields` requires [NumPy](https://numpy.org/), [Matplotlib](https://matplotlib.org/) and [SciPy](https://www.scipy.org/). Other than that, the following external libraries are used for a few different functions:
 
  - 2D plotting for map projections other than Hammer : [Cartopy](https://scitools.org.uk/cartopy/docs/latest/) library
@@ -199,10 +201,31 @@
  - Please make sure the tests pass before opening a pull request. 
  - Please follow Python [PEP-8](https://peps.python.org/pep-0008/) guidelines when it comes to code style.
  - If you wish to add new data file, please name it following the convention `<planet>_<model>.dat`, where `planet` and `model` denote the names of the planet and the magnetic field model being used. See the `data` directory for examples.
  - If you implement a new feature or data source, please update the documentation accordingly. 
 
 Please report any bugs or other issues through [GitHub Issues](https://github.com/AnkitBarik/planetMagFields/issues). 
 
+# Citing `planetMagFields`
+
+If you're using `planetMagFields` for your work, please cite the [JOSS paper](https://joss.theoj.org/papers/10.21105/joss.06677#):
+
+Barik et al., (2024). planetMagFields: A Python package for analyzing and plotting planetary magnetic field data. Journal of Open Source Software, 9(97), 6677, https://doi.org/10.21105/joss.06677
+
+```
+@article{Barik2024,
+doi = {10.21105/joss.06677},
+url = {https://doi.org/10.21105/joss.06677},
+year = {2024},
+publisher = {The Open Journal},
+volume = {9},
+number = {97},
+pages = {6677},
+author = {Barik, Ankit and Angappan, Regupathi},
+title = {planetMagFields: A Python package for analyzing and plotting planetary magnetic field data},
+journal = {Journal of Open Source Software}
+}
+```
+
 # Acknowledgements
 
 I would like to thank [Regupathi Angappan](https://github.com/reguang) for motivating me to create this package, testing it and for writing the Jupyter notebook. I thank [Jon Aurnou](https://epss.ucla.edu/people/faculty/543/) for testing it out and pointing out runtime errors. I would like to thank [Thomas Gastine](https://github.com/tgastine) for comparing the plots with real data and pointing out a normalization error which has been fixed. Thanks a lot to [Arthus](https://github.com/arthus701) for adding the `setup.py`.
```

### Comparing `planetmagfields-1.4.3.post1/README.md` & `planetmagfields-1.4.3.post2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 [Jupyter notebook](#jupyter-notebook)
 
 [Documentation](#documentation)
 
 [Code contribution and reporting issues](#code-contribution-and-reporting-issues)
 
+[Citing `planetMagFields`](#citing-planetmagfields)
+
 [Acknowledgements](#acknowledgements)
 
 # Prerequisites
 
 `planetMagFields` requires [NumPy](https://numpy.org/), [Matplotlib](https://matplotlib.org/) and [SciPy](https://www.scipy.org/). Other than that, the following external libraries are used for a few different functions:
 
  - 2D plotting for map projections other than Hammer : [Cartopy](https://scitools.org.uk/cartopy/docs/latest/) library
@@ -166,10 +168,31 @@
  - Please make sure the tests pass before opening a pull request. 
  - Please follow Python [PEP-8](https://peps.python.org/pep-0008/) guidelines when it comes to code style.
  - If you wish to add new data file, please name it following the convention `<planet>_<model>.dat`, where `planet` and `model` denote the names of the planet and the magnetic field model being used. See the `data` directory for examples.
  - If you implement a new feature or data source, please update the documentation accordingly. 
 
 Please report any bugs or other issues through [GitHub Issues](https://github.com/AnkitBarik/planetMagFields/issues). 
 
+# Citing `planetMagFields`
+
+If you're using `planetMagFields` for your work, please cite the [JOSS paper](https://joss.theoj.org/papers/10.21105/joss.06677#):
+
+Barik et al., (2024). planetMagFields: A Python package for analyzing and plotting planetary magnetic field data. Journal of Open Source Software, 9(97), 6677, https://doi.org/10.21105/joss.06677
+
+```
+@article{Barik2024,
+doi = {10.21105/joss.06677},
+url = {https://doi.org/10.21105/joss.06677},
+year = {2024},
+publisher = {The Open Journal},
+volume = {9},
+number = {97},
+pages = {6677},
+author = {Barik, Ankit and Angappan, Regupathi},
+title = {planetMagFields: A Python package for analyzing and plotting planetary magnetic field data},
+journal = {Journal of Open Source Software}
+}
+```
+
 # Acknowledgements
 
 I would like to thank [Regupathi Angappan](https://github.com/reguang) for motivating me to create this package, testing it and for writing the Jupyter notebook. I thank [Jon Aurnou](https://epss.ucla.edu/people/faculty/543/) for testing it out and pointing out runtime errors. I would like to thank [Thomas Gastine](https://github.com/tgastine) for comparing the plots with real data and pointing out a normalization error which has been fixed. Thanks a lot to [Arthus](https://github.com/arthus701) for adding the `setup.py`.
```

### Comparing `planetmagfields-1.4.3.post1/planetMagFields.egg-info/PKG-INFO` & `planetmagfields-1.4.3.post2/planetMagFields.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetMagFields
-Version: 1.4.3.post1
+Version: 1.4.3.post2
 Summary: Routines to easily access information about magnetic fields of planets in our solar system and visualize them in both 2D and 3D
 Author: Barik, Ankit
 Author-email: Ankit Barik <ankit.barik@gmail.com>
 Maintainer-email: Ankit Barik <ankit.barik@gmail.com>, Regupathi Angappan <rangapp1@jhu.edu>
 Project-URL: Homepage, https://ankitbarik.github.io/planetMagFields/
 Project-URL: Issues, https://github.com/AnkitBarik/planetMagFields/issues
 Keywords: Spherical Harmonics,Planetary Science,Spectra,Magnetic Field,Visualization,3D visualization
@@ -49,14 +49,16 @@
 
 [Jupyter notebook](#jupyter-notebook)
 
 [Documentation](#documentation)
 
 [Code contribution and reporting issues](#code-contribution-and-reporting-issues)
 
+[Citing `planetMagFields`](#citing-planetmagfields)
+
 [Acknowledgements](#acknowledgements)
 
 # Prerequisites
 
 `planetMagFields` requires [NumPy](https://numpy.org/), [Matplotlib](https://matplotlib.org/) and [SciPy](https://www.scipy.org/). Other than that, the following external libraries are used for a few different functions:
 
  - 2D plotting for map projections other than Hammer : [Cartopy](https://scitools.org.uk/cartopy/docs/latest/) library
@@ -199,10 +201,31 @@
  - Please make sure the tests pass before opening a pull request. 
  - Please follow Python [PEP-8](https://peps.python.org/pep-0008/) guidelines when it comes to code style.
  - If you wish to add new data file, please name it following the convention `<planet>_<model>.dat`, where `planet` and `model` denote the names of the planet and the magnetic field model being used. See the `data` directory for examples.
  - If you implement a new feature or data source, please update the documentation accordingly. 
 
 Please report any bugs or other issues through [GitHub Issues](https://github.com/AnkitBarik/planetMagFields/issues). 
 
+# Citing `planetMagFields`
+
+If you're using `planetMagFields` for your work, please cite the [JOSS paper](https://joss.theoj.org/papers/10.21105/joss.06677#):
+
+Barik et al., (2024). planetMagFields: A Python package for analyzing and plotting planetary magnetic field data. Journal of Open Source Software, 9(97), 6677, https://doi.org/10.21105/joss.06677
+
+```
+@article{Barik2024,
+doi = {10.21105/joss.06677},
+url = {https://doi.org/10.21105/joss.06677},
+year = {2024},
+publisher = {The Open Journal},
+volume = {9},
+number = {97},
+pages = {6677},
+author = {Barik, Ankit and Angappan, Regupathi},
+title = {planetMagFields: A Python package for analyzing and plotting planetary magnetic field data},
+journal = {Journal of Open Source Software}
+}
+```
+
 # Acknowledgements
 
 I would like to thank [Regupathi Angappan](https://github.com/reguang) for motivating me to create this package, testing it and for writing the Jupyter notebook. I thank [Jon Aurnou](https://epss.ucla.edu/people/faculty/543/) for testing it out and pointing out runtime errors. I would like to thank [Thomas Gastine](https://github.com/tgastine) for comparing the plots with real data and pointing out a normalization error which has been fixed. Thanks a lot to [Arthus](https://github.com/arthus701) for adding the `setup.py`.
```

### Comparing `planetmagfields-1.4.3.post1/planetMagFields.egg-info/SOURCES.txt` & `planetmagfields-1.4.3.post2/planetMagFields.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.3.post1/planetmagfields/data/earth_igrf13.dat` & `planetmagfields-1.4.3.post2/planetmagfields/data/earth_igrf13.dat`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.3.post1/planetmagfields/data/jupiter_jrm09.dat` & `planetmagfields-1.4.3.post2/planetmagfields/data/jupiter_jrm09.dat`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.3.post1/planetmagfields/data/jupiter_jrm33.dat` & `planetmagfields-1.4.3.post2/planetmagfields/data/jupiter_jrm33.dat`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.3.post1/planetmagfields/libbfield.py` & `planetmagfields-1.4.3.post2/planetmagfields/libbfield.py`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.3.post1/planetmagfields/libdata.py` & `planetmagfields-1.4.3.post2/planetmagfields/libdata.py`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.3.post1/planetmagfields/libgauss.py` & `planetmagfields-1.4.3.post2/planetmagfields/libgauss.py`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.3.post1/planetmagfields/planet.py` & `planetmagfields-1.4.3.post2/planetmagfields/planet.py`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.3.post1/planetmagfields/plotlib.py` & `planetmagfields-1.4.3.post2/planetmagfields/plotlib.py`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.3.post1/planetmagfields/potextra.py` & `planetmagfields-1.4.3.post2/planetmagfields/potextra.py`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.3.post1/planetmagfields/utils.py` & `planetmagfields-1.4.3.post2/planetmagfields/utils.py`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.3.post1/pyproject.toml` & `planetmagfields-1.4.3.post2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "planetMagFields"
-version = "1.4.3.post1"
+version = "1.4.3.post2"
 authors = [
   { name="Ankit Barik", email="ankit.barik@gmail.com" },
 ]
 maintainers = [
   { name="Ankit Barik", email="ankit.barik@gmail.com" },
   { name="Regupathi Angappan", email="rangapp1@jhu.edu" },
 ]
```

### Comparing `planetmagfields-1.4.3.post1/setup.py` & `planetmagfields-1.4.3.post2/setup.py`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.3.post1/tests/test_potextra.py` & `planetmagfields-1.4.3.post2/tests/test_potextra.py`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.3.post1/tests/test_read.py` & `planetmagfields-1.4.3.post2/tests/test_read.py`

 * *Files identical despite different names*

