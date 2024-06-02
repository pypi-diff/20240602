# Comparing `tmp/barotropic-3.0.1.tar.gz` & `tmp/barotropic-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barotropic-3.0.1.tar", last modified: Mon Mar 28 08:17:22 2022, max compression
+gzip compressed data, was "barotropic-3.1.0.tar", last modified: Sun Jun  2 17:40:37 2024, max compression
```

## Comparing `barotropic-3.0.1.tar` & `barotropic-3.1.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-03-28 08:17:22.343019 barotropic-3.0.1/
--rw-rw-r--   0 chris     (1000) chris     (1000)    10175 2022-03-28 08:15:08.000000 barotropic-3.0.1/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)      328 2022-03-28 08:17:22.343019 barotropic-3.0.1/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     2817 2022-03-28 08:15:08.000000 barotropic-3.0.1/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-03-28 08:17:22.343019 barotropic-3.0.1/barotropic/
--rw-rw-r--   0 chris     (1000) chris     (1000)      383 2022-03-28 08:15:08.000000 barotropic-3.0.1/barotropic/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      209 2022-03-28 08:15:08.000000 barotropic-3.0.1/barotropic/constants.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    16293 2022-03-28 08:15:08.000000 barotropic-3.0.1/barotropic/diagnostics.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2403 2022-03-28 08:15:08.000000 barotropic-3.0.1/barotropic/formatting.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    37062 2022-03-28 08:15:08.000000 barotropic-3.0.1/barotropic/grid.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3775 2022-03-28 08:15:08.000000 barotropic-3.0.1/barotropic/init.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4097 2022-03-28 08:15:08.000000 barotropic-3.0.1/barotropic/io.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6300 2022-03-28 08:15:08.000000 barotropic-3.0.1/barotropic/model.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    16335 2022-03-28 08:15:08.000000 barotropic-3.0.1/barotropic/plot.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9058 2022-03-28 08:15:08.000000 barotropic-3.0.1/barotropic/rhs.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    12721 2022-03-28 08:15:08.000000 barotropic-3.0.1/barotropic/state.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-03-28 08:17:22.343019 barotropic-3.0.1/barotropic/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2022-03-28 08:15:08.000000 barotropic-3.0.1/barotropic/tests/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      700 2022-03-28 08:15:08.000000 barotropic-3.0.1/barotropic/tests/test_examples.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8941 2022-03-28 08:15:08.000000 barotropic-3.0.1/barotropic/tests/test_grid.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3282 2022-03-28 08:15:08.000000 barotropic-3.0.1/barotropic/tests/test_state.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-03-28 08:17:22.343019 barotropic-3.0.1/barotropic.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      328 2022-03-28 08:17:22.000000 barotropic-3.0.1/barotropic.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      549 2022-03-28 08:17:22.000000 barotropic-3.0.1/barotropic.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2022-03-28 08:17:22.000000 barotropic-3.0.1/barotropic.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      100 2022-03-28 08:17:22.000000 barotropic-3.0.1/barotropic.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       11 2022-03-28 08:17:22.000000 barotropic-3.0.1/barotropic.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2022-03-28 08:17:22.343019 barotropic-3.0.1/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)      589 2022-03-28 08:15:08.000000 barotropic-3.0.1/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-06-02 17:40:37.383594 barotropic-3.1.0/
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10175 2024-06-02 17:35:40.000000 barotropic-3.1.0/LICENSE
+-rw-r--r--   0 chris     (1000) chris     (1000)    12780 2024-06-02 17:40:37.383594 barotropic-3.1.0/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2941 2024-06-02 17:35:40.000000 barotropic-3.1.0/README.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1296 2024-06-02 17:35:40.000000 barotropic-3.1.0/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-06-02 17:40:37.383594 barotropic-3.1.0/setup.cfg
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-06-02 17:40:37.379594 barotropic-3.1.0/src/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-06-02 17:40:37.379594 barotropic-3.1.0/src/barotropic/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      407 2024-06-02 17:35:40.000000 barotropic-3.1.0/src/barotropic/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      209 2024-06-02 17:35:40.000000 barotropic-3.1.0/src/barotropic/constants.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    16293 2024-06-02 17:35:40.000000 barotropic-3.1.0/src/barotropic/diagnostics.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2403 2024-06-02 17:35:40.000000 barotropic-3.1.0/src/barotropic/formatting.py
+-rwxrwxr-x   0 chris     (1000) chris     (1000)    42875 2024-06-02 17:35:40.000000 barotropic-3.1.0/src/barotropic/grid.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3775 2024-06-02 17:35:40.000000 barotropic-3.1.0/src/barotropic/init.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    13690 2024-06-02 17:35:40.000000 barotropic-3.1.0/src/barotropic/io.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7331 2024-06-02 17:35:40.000000 barotropic-3.1.0/src/barotropic/model.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    16335 2024-06-02 17:35:40.000000 barotropic-3.1.0/src/barotropic/plot.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9058 2024-06-02 17:35:40.000000 barotropic-3.1.0/src/barotropic/rhs.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    17441 2024-06-02 17:35:40.000000 barotropic-3.1.0/src/barotropic/state.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-06-02 17:40:37.383594 barotropic-3.1.0/src/barotropic.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)    12780 2024-06-02 17:40:37.000000 barotropic-3.1.0/src/barotropic.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      606 2024-06-02 17:40:37.000000 barotropic-3.1.0/src/barotropic.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-06-02 17:40:37.000000 barotropic-3.1.0/src/barotropic.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      176 2024-06-02 17:40:37.000000 barotropic-3.1.0/src/barotropic.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       11 2024-06-02 17:40:37.000000 barotropic-3.1.0/src/barotropic.egg-info/top_level.txt
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-06-02 17:40:37.383594 barotropic-3.1.0/tests/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      700 2024-06-02 17:35:40.000000 barotropic-3.1.0/tests/test_examples.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9036 2024-06-02 17:35:40.000000 barotropic-3.1.0/tests/test_grid.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6282 2024-06-02 17:35:40.000000 barotropic-3.1.0/tests/test_io.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4953 2024-06-02 17:35:40.000000 barotropic-3.1.0/tests/test_state.py
```

### Comparing `barotropic-3.0.1/LICENSE` & `barotropic-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `barotropic-3.0.1/README.md` & `barotropic-3.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # barotropic
 
 A framework for barotropic analysis and modelling of the atmosphere.
 
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7330469.svg)](https://doi.org/10.5281/zenodo.7330469)
+
 
 ## Features
 
 - Integration of the barotropic PV equation on the sphere. 
   Fields are represented on a regular latitude-longitude grid while spatial derivatives are evaluated in spectral space (spherical harmonics).
   The model uses a leapfrog time integration scheme with Robert-Asselin filter, initialized with an Euler-forward step.
 - A range of diagnostic functions to investigate properties of the flow and extract features, e.g. Rossby wave packets.
@@ -44,20 +46,20 @@
 Dependencies:
 
 - [numpy](https://github.com/numpy/numpy)
 - [scipy](https://github.com/scipy/scipy)
 - [pyspharm](https://github.com/jswhit/pyspharm)
 - [matplotlib](https://github.com/matplotlib/matplotlib) (optional)
 - [PyWavelets](https://github.com/PyWavelets/pywt) (optional, >= 1.1)
-- [hn2016_falwa](https://github.com/csyhuang/hn2016_falwa) (optional)
+- [falwa](https://github.com/csyhuang/hn2016_falwa) (optional, hn2016_falwa for 3.0.x)
 
 
 ## License
 
-Copyright 2019-2022 Christopher Polster
+Copyright 2019-2024 Christopher Polster
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
 http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `barotropic-3.0.1/barotropic/diagnostics.py` & `barotropic-3.1.0/src/barotropic/diagnostics.py`

 * *Files identical despite different names*

### Comparing `barotropic-3.0.1/barotropic/formatting.py` & `barotropic-3.1.0/src/barotropic/formatting.py`

 * *Files identical despite different names*

### Comparing `barotropic-3.0.1/barotropic/grid.py` & `barotropic-3.1.0/src/barotropic/grid.py`

 * *Files 23% similar despite different names*

```diff
@@ -47,16 +47,14 @@
         self.rsphere = rsphere
         self.omega = omega
         # Setup longitude and latitude grid. Make sure longitude 0° is not
         # repeated and that both latitudes 90° and -90° exist. Latitudes start
         # at the North pole, which is the convention used by pyspharm.
         self.nlon = int(360. / resolution)
         self.nlat = int(180. / resolution) + 1
-        if self.nlat % 2 == 0:
-            raise ValueError("Number of latitudes must be odd but is {}".format(self.nlat))
         self.lon = np.linspace( 0., 360., self.nlon, endpoint=False)
         self.lat = np.linspace(90., -90., self.nlat, endpoint=True)
         self.lon2, self.lat2 = np.meshgrid(self.lon, self.lat)
         # Grid spacing in degrees
         self.dlon = resolution
         self.dlat = -resolution
         # Spherical coordinate grid (for use with trigonometric functions)
@@ -123,18 +121,70 @@
         """
         return 2. * self.omega * np.sin(np.deg2rad(lat))
 
     # Region extraction
 
     @property
     def region(self):
-        """Region extractor with indexing syntax.
+        """Region extractor with indexing syntax based on coordinates::
+
+            grid.region[lon_slice,lat_slice]
+
+        with the slices' `start` and `stop` values in the range of 0° to 360°.
+        Slices must not have the `step` parameter specified but `start` and
+        `stop` can be left unspecified. If a single numeric value :code:`x` is
+        given instead of a slice, the value is treated like :code:`slice(x, x)`
+        but additionally verified for existence on the :py:class:`Grid`.
+
+        Returns:
+            Configured :py:class:`barotropic.grid.GridRegion` instance for
+            a valid selection.
 
         .. note::
-            Coordinate order is [lon,lat]. This is inverted compared to indexing into the arrays.
+            Coordinate order is [lon,lat] (plotting convention) and inclusive
+            on all sides (like xarray selections). This is different from
+            indexing into the arrays directly on purpose.
+
+        Selections can cross the grid boundary in the (periodic) longitude
+        dimension and the order of the selection ranges does not matter:
+
+        >>> grid = bt.Grid(10.)
+        >>> grid.region[300:50,-5:-50]
+        Region -50.00 to -10.00 °N (nlat = 5)
+               300.00 to  50.00 °E (nlon = 12)
+            ···································· 90°N
+            ····································
+            ····································
+            ····································
+            XXXXXX························XXXXXX EQ
+            XXXXXX························XXXXXX
+            XXXXXX························XXXXXX
+            ····································
+            ···································· 90°S
+            0°E              180°E
+        of <barotropic.Grid> ...
+
+        The latitude dimension accepts ``"N"`` and ``"S"`` as special keywords
+        for easy reference to the northern and southern hemisphere,
+        respectively, e.g.:
+
+        >>> grid.region[:,"N"]
+        Region   0.00 to  90.00 °N (nlat = 10)
+                 0.00 to 350.00 °E (nlon = 36)
+            XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX 90°N
+            XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
+            XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
+            XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
+            XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX EQ
+            ····································
+            ····································
+            ····································
+            ···································· 90°S
+            0°E              180°E
+        of <barotropic.Grid> ...
         """
         return GridRegionIndexer(self)
 
     # Spectral-grid transforms
 
     def to_spectral(self, field_grid):
         """Transform a gridded field into spectral space.
@@ -364,15 +414,15 @@
 
     @property
     def gridpoint_area(self):
         """Surface area of each gridpoint as a function of latitude.
 
         The area associated with a gridpoint (λ, φ) in a regular lon-lat grid::
 
-            r² * dλ * ( sin(φ + dφ) - sin(φ - dφ) )
+            r² * dλ * ( sin(φ + dφ/2) - sin(φ - dφ/2) )
         """
         # Calculate dual phi grid (latitude mid-points)
         mid_phi = 0.5 * (self.phi[1:] + self.phi[:-1])
         # Start with scaling factor
         gridpoint_area = np.full(self.nlat, self.rsphere * self.rsphere * self.dlam, dtype=float)
         # Calculate latitude term of area formula
         gridpoint_area[1:-1] *= np.sin(mid_phi[:-1]) - np.sin(mid_phi[1:])
@@ -384,15 +434,15 @@
     def mean(self, field, axis=None, region=None):
         """Area-weighted mean of the input field.
 
         Parameters:
             field (array): 2D input field.
             axis (None | int | "meridional" | "zonal"): Axis over which to
                 compute the mean.
-            region (None | :py:class:`GridRegion`): Region to which the mean is
+            region (None | :py:class:`grid.GridRegion`): Region to which the mean is
                 restricted. Construct regions with :py:attr:`region` or specify
                 any object that implements a compatible **extract** method.
 
         Returns:
             Area-weighted mean.
         """
         # 
@@ -741,14 +791,20 @@
         # dimension (only rectangular, axis-aligned regions possible)
         lon_indices = self._get_lon_indices(selection[0])
         lat_indices = self._get_lat_indices(selection[1])
         # Now in index world, axes order is flipped there (lat first)
         return GridRegion(self._grid, lat_indices, lon_indices)
 
     def _get_lat_indices(self, slc):
+        # Single-value selection still returns full array but value is checked
+        if isinstance(slc, Number):
+            idx = np.argwhere(np.isclose(self._grid.lat, slc)).flatten()
+            if idx.size != 1:
+                raise IndexError(f"latitude {slc} is not on the grid")
+            return idx
         # Allow special values N and S to select hemispheres
         if slc == "N":
             slc = slice(0, 90)
         if slc == "S":
             slc = slice(-90, 0)
         # Selection must be a numeric slice without a step parameter
         if not isinstance(slc, slice):
@@ -770,14 +826,20 @@
             return indices[self._grid.lat <= hi]
         elif hi is None:
             return indices[lo <= self._grid.lat]
         else:
             return indices[(min(lo, hi) <= self._grid.lat) & (self._grid.lat <= max(lo, hi))]
 
     def _get_lon_indices(self, slc):
+        # Single-value selection still returns full array but value is checked
+        if isinstance(slc, Number):
+            idx = np.argwhere(np.isclose(self._grid.lon, slc)).flatten()
+            if idx.size != 1:
+                raise IndexError(f"longitude {slc} is not on the grid")
+            return idx
         # Selection must be a numeric slice without a step parameter
         if not isinstance(slc, slice):
             raise IndexError("longitude selection must given as a slice")
         if not (isinstance(slc.start, Number) or slc.start is None):
             raise IndexError("start value of longitude selection must be numeric or None")
         if not (isinstance(slc.stop, Number) or slc.stop is None):
             raise IndexError("stop value of longitude selection must be numeric or None")
@@ -799,14 +861,27 @@
             return np.roll(indices[(self._grid.lon <= hi) | lo_mask], np.count_nonzero(lo_mask))
         else:
             return indices[(lo <= self._grid.lon) & (self._grid.lon <= hi)]
 
 
 
 class GridRegion:
+    """Region selection for convenient data extraction.
+
+    .. note::
+        Use :py:attr:`barotropic.Grid.region` to create instances of this
+        class.
+
+    Parameters: 
+        grid (Grid): Lon-lat grid instance that the selection is tied to.
+        lat_indices (sequence): Latitude dimension indices included in the
+            selection.
+        lon_indices (sequence): Longitude dimension indices included in the
+            selection.
+    """
 
     def __init__(self, grid, lat_indices, lon_indices):
         self._grid = grid
         self._lon_indices = np.require(lon_indices, dtype=int)
         self._lat_indices = np.require(lat_indices, dtype=int)
         assert self._lat_indices.ndim == 1 and self._lat_indices.size <= grid.nlat
         assert self._lon_indices.ndim == 1 and self._lon_indices.size <= grid.nlon
@@ -825,59 +900,114 @@
         elif field.shape == self._grid.shape:
             # https://stackoverflow.com/questions/42309460
             return field[np.ix_(self._lat_indices, self._lon_indices)]
         else:
             raise ValueError("unable to extract from field '{}'".format(field))
 
     def extract(self, *fields):
-        """Extract the region from the given fields."""
+        """Extract data from the selected region.
+
+        Parameters:
+            fields (array): Field or fields from which to extract the selected
+                region. The shape of each field must match that of the
+                :py:class:`Grid` associated with the :py:class:`GridRegion`
+                instance.
+
+        Returns:
+            A single array (one-argument call) or a tuple of arrays
+            (multi-argument call, order preserved) containing the data
+            selection.
+
+        >>> grid = bt.Grid(10.)
+        >>> sel = grid.region[45:90,-20:30]
+        >>> sel.extract(grid.lon2)
+        array([[50., 60., 70., 80., 90.],
+               [50., 60., 70., 80., 90.],
+               [50., 60., 70., 80., 90.],
+               [50., 60., 70., 80., 90.],
+               [50., 60., 70., 80., 90.],
+               [50., 60., 70., 80., 90.]])
+
+        If the region crosses the periodic boundary in the longitude
+        dimension, the two parts of the fields from the original array are
+        reassembled into a field connected across the boundary:
+
+        >>> grid.region[340:10,60:70].extract(grid.lon2)
+        array([[340., 350.,   0.,  10.],
+               [340., 350.,   0.,  10.]])
+
+        Use :py:attr:`GridRegion.lon_mono` to obtain continuous longitude
+        coordinates in such situations.
+
+        Always returns fields of full dimensionality, even for single-value
+        selections:
+
+        >>> grid.region[0,50].extract(grid.fcor2)
+        array([[0.00011172]])
+        """
         if len(fields) == 0:
             raise ValueError("no field(s) given for extraction")
         elif len(fields) == 1:
             return self._extract_one(fields[0])
         else:
             return tuple(map(self._extract_one, fields))
 
     @property
     def mask(self):
-        """Boolean array that is true in the region."""
+        """Boolean array that is *True* in the selected region."""
         mask = np.full(self._grid.shape, False)
         mask[np.ix_(self._lat_indices, self._lon_indices)] = True
         return mask
 
     @property
     def shape(self):
         """Shape of extracted 2D fields."""
         return self._lat_indices.size, self._lon_indices.size
 
     @property
     def lat(self):
-        """Latitudes of the region."""
+        """Latitude coordinate array for the region."""
         return self._grid.lat[self._lat_indices]
 
     @property
     def lon(self):
-        """Longitudes of the region.
+        """Longitude coordinate array for the region.
 
-        If the region crosses the 0° meridian, these will not be monotonic. If
-        you need a monotonic longitude coordinate, e.g. for plotting, use
-        `lon_mono`, where longitudes left of 0° are reduced by 360°.
+        .. note::
+            The array will not be monotonic if the region crosses the 0°
+            meridian.  In case a monotonic longitude coordinate is required,
+            e.g. for plotting, use :py:attr:`lon_mono`.
         """
         return self._grid.lon[self._lon_indices]
 
     @property
     def lon_mono(self):
-        """Longitudes of the region, monotonic even for regions crossing 0°"""
+        """Longitude coordinate array for the region, monotonic across 0°.
+
+        Longitudes west of 0° (the western edge of a :py:class:`Grid`) are
+        reduced by 360° to obtain monotonic values:
+
+        >>> sel = bt.Grid(10.).region[320:30,:]
+        >>> sel.lon
+        array([320., 330., 340., 350.,   0.,  10.,  20.,  30.])
+        >>> sel.lon_mono
+        array([-40., -30., -20., -10.,   0.,  10.,  20.,  30.])
+        """
         lon = self.lon
         jump = np.argwhere(np.diff(lon) < 0)
         assert 0 <= jump.size <= 1
         if jump.size == 1:
             lon[:jump[0,0]+1] -= 360.
         return lon
 
     @property
     def gridpoint_area(self):
+        """See :py:attr:`barotropic.Grid.gridpoint_area`."""
         return self.extract(self._grid.gridpoint_area)
 
     def mean(self, field):
+        """Area-weighted mean in the selected region.
+
+        Wraps :py:meth:`barotropic.Grid.mean`.
+        """
         return self._grid.mean(field, region=self)
```

### Comparing `barotropic-3.0.1/barotropic/init.py` & `barotropic-3.1.0/src/barotropic/init.py`

 * *Files identical despite different names*

### Comparing `barotropic-3.0.1/barotropic/model.py` & `barotropic-3.1.0/src/barotropic/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 from numbers import Number
+
 import numpy as np
+
 from . import formatting
-from .state import State
+from .state import State, StateList
 
 
 class BarotropicModel:
     """Integrate the barotropic PV equation on the sphere forward in time.
 
     Parameters:
         rhs (:py:class:`rhs.RHS`): Model forcing. Build from the components
             provided in :py:mod:`rhs`.
         diffusion_order (int): Order of diffusion term added for numerical
             stability to the PV equation. Hyperdiffusion by default.
         diffusion_coeff (number): Strength of diffusion.
+        diffusion_bg (array | None): A background vorticity field that is
+            removed before application of the diffusion steps.
 
     Barotropic PV equation with forcing::
 
         Dq/Dt = ∂q/∂t + ∇(u·q) = RHS,
 
     where ``q`` is the barotropic potential vorticity (i.e. absolute vorticity)
     and ``u`` is the divergence-free horizontal wind (which can be obtained
     from the PV by inversion).
 
     Does not carry state aside from the forcing and diffusion setup and can be
-    reused for multiple integrations with different :py:class`barotropic.State`
-    instances.
+    reused for multiple integrations with different :py:class:`State` instances
+    (though note that when used with the **diffusion_bg** parameter or some RHS
+    terms, the :py:class:`BarotropicModel` can be restricted to a specific grid
+    resolution).
+
+    .. versionadded:: 3.1
+        The *diffusion_bg* parameter.
     """
 
-    def __init__(self, rhs=None, diffusion_order=2, diffusion_coeff=1.e15):
+    def __init__(self, rhs=None, diffusion_order=2, diffusion_coeff=1.e15,
+            diffusion_bg=None):
         self.rhs = rhs
         self.diffusion_order = diffusion_order
         self.diffusion_coeff = diffusion_coeff
+        self._diffusion_bg = diffusion_bg
 
     def __repr__(self):
         return formatting.barotropic_model_repr(self)
 
     def run(self, state_init, dt, tend, save_every=0):
         """Run the model until a specified time is reached.
 
@@ -48,16 +59,16 @@
                 soon as it is exeeded.
             save_every (number): If larger than zero, an intermediate state is
                 saved and returned in the list of states every time this time
                 interval is exceeded. Does not work for datetime/timedelta
                 **dt** currently.
 
         Returns:
-            Tuple containing the final state and a list of all saved
-            intermediate states.
+            Tuple containing the final state (:py:class:`State`) and a list of
+            all saved intermediate states (:py:class:`StateList`).
 
         Initializes with a first-order Euler forward step, then continues with
         second-order Leapfrog steps.
 
         """
         if tend < state_init.time:
             return state_init, [state_init]
@@ -71,15 +82,15 @@
         # Integrate one step further than requested so Robert-Asselin filter is
         # applied to model state at the end
         while state.time < tend:
             state, state_new = self.leapfrog(state, state_new)
             if save_every > 0 and state.time >= t_save:
                 states.append(state)
                 t_save += save_every
-        return state, states
+        return state, StateList(states)
 
     def euler(self, state_now, dt):
         """Step forward in time with a first-order Euler-forward scheme
 
         Parameters:
             state_now (:py:class:`State`): Initial state.
             dt (number | timedelta): Time step size.
@@ -142,20 +153,30 @@
         """Evaluate ∂q/∂t = -∇(u·q) + RHS in spectral space"""
         tendency = -state.pv_flux_spectral 
         if self.rhs is not None:
             tendency += state.grid.to_spectral(self.rhs(state))
         return tendency 
 
     def _apply_diffusion(self, grid, dt, pv_spectral):
-        return grid.solve_diffusion_spectral(
+        # If a reference background field is specified, apply the diffusion
+        # only to the anomaly field
+        if self._diffusion_bg is not None:
+            background = grid.to_spectral(self._diffusion_bg) # keep for later
+            pv_spectral = pv_spectral - background
+        # Solve on step of the diffusion equation
+        pv_spectral = grid.solve_diffusion_spectral(
             pv_spectral,
             dt=dt,
             coeff=self.diffusion_coeff,
             order=self.diffusion_order
         )
+        # Reinstate the full field if a background was removed
+        if self._diffusion_bg is not None:
+            pv_spectral = pv_spectral + background
+        return pv_spectral
 
 
 def _to_seconds(dt):
     """Return time interval dt as number of seconds
 
     Provides compatibility with both timedelta objects and direct input of dt
     as a number of seconds.
```

### Comparing `barotropic-3.0.1/barotropic/plot.py` & `barotropic-3.1.0/src/barotropic/plot.py`

 * *Files identical despite different names*

### Comparing `barotropic-3.0.1/barotropic/rhs.py` & `barotropic-3.1.0/src/barotropic/rhs.py`

 * *Files identical despite different names*

### Comparing `barotropic-3.0.1/barotropic/state.py` & `barotropic-3.1.0/src/barotropic/state.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,14 @@
+import collections.abc
+import itertools
+import functools
+import numbers
+
 import numpy as np
+
 from . import diagnostics, formatting
 from .constants import ZONAL
 from .grid import Grid
 
 
 def _cached_property(f):
     cache = "_" + f.__name__
@@ -24,19 +30,23 @@
         pv (None | array): Gridded field of potential vorticity (PV, absolute
             vorticity in the barotropic framework).
         pv_spectral (None | array): Spectral representation of potential
             vorticity. Only specify if **pv** is ``None``.
 
     Note:
         There are alternative classmethod constructors of :py:class:`State` and
-        the :py:mod:`init` module also provides functions to create
+        the :py:mod:`.init` module also provides functions to create
         :py:class:`State` objects for model initialization.
 
     Provides convenient access to fields, diagnostics and plots. Should
     generally be treated as an immutable object.
+
+    Attributes:
+        time: Valid time.
+        grid: Associated :py:class:`.Grid` object.
     """
 
     def __init__(self, grid, time, pv=None, pv_spectral=None):
         self.grid = grid
         self.time = time
         # Always send PV field through spectral representation to ensure
         # consistency between spherical harmonics and gridded representation
@@ -131,14 +141,22 @@
     def pv(self):
         """Barotropic potential vorticity (i.e. absolute vorticity)."""
         if self._pv is None:
             self._pv = self.grid.to_grid(self._pv_spectral)
         return self._pv
 
     @property
+    def avo(self):
+        """Absolute vorticity (alias of :py:attr:`.pv`).
+
+        .. versionadded:: 3.1
+        """
+        return self.pv
+
+    @property
     def pv_spectral(self):
         """Barotropic potential vorticity in spectral space."""
         if self._pv_spectral is None:
             self._pv_spectral = self.grid.to_spectral(self._pv)
         return self._pv_spectral
 
     @property
@@ -176,14 +194,22 @@
 
     @property
     def vorticity(self):
         """Relative vorticity."""
         return self.pv - self.grid.fcor2
 
     @property
+    def vo(self):
+        """Relative vorticity (alias of :py:attr:`.vorticity`).
+
+        .. versionadded:: 3.1
+        """
+        return self.vorticity
+
+    @property
     def vorticity_spectral(self):
         return self.pv_spectral - self.grid.fcor2_spectral
 
     @property
     def enstrophy(self):
         """Enstropy = ``0.5 * q²`` where ``q`` is PV."""
         return 0.5 * self.pv**2
@@ -260,15 +286,15 @@
     def extract_ks_waveguides(self, *args, **kwargs):
         """Shortcut to :py:func:`diagnostics.extract_ks_waveguides`."""
         return diagnostics.extract_ks_waveguides(self, *args, **kwargs)
 
     # Shortcut to model integration
 
     def run(self, model, *args, **kwargs):
-        """Shortcut to :py:meth:`BarotropicModel.run`"""
+        """Shortcut to :py:meth:`BarotropicModel.run`."""
         return model.run(self, *args, **kwargs)
 
     # Shortcuts to plotting. Do not return figures here, so user does not have
     # to put semicolons in Jupyter notebooks to suppress double figure output.
 
     @property
     def plot(self):
@@ -288,49 +314,49 @@
         as the returned object of the cell).
         """
         return StatePlotter(self)
 
     # Connection to other packages
 
     def as_hn2016(self, **barofield_kwargs):
-        """Convert state to hn2016_falwa Barotropic state.
+        """Convert state to a :py:mod:`falwa` Barotropic state.
 
         Parameters:
             barofield_kwargs: Keyword arguments given to the constructor.
 
         Returns:
-            :py:class:`hn2016_falwa.barotropic_field.BarotropicField` instance.
+            :py:class:`falwa.barotropic_field.BarotropicField` instance.
 
         .. note::
-            In :py:mod:`hn2016_falwa` latitude starts at the South Pole, so
+            In :py:mod:`falwa` latitude starts at the South Pole, so
             array contents are meridionally flipped compared to :py:mod:`barotropic`.
 
         See :py:meth:`State.from_hn2016` for the inverse operation.
 
-        Requires :py:mod:`hn2016_falwa`.
+        Requires `falwa <https://github.com/csyhuang/hn2016_falwa>`_ package.
         """
-        from hn2016_falwa.barotropic_field import BarotropicField
+        from falwa.barotropic_field import BarotropicField
         pv = self.pv
-        # hn2016_falwa expects latitudes to start at the South Pole
+        # falwa expects latitudes to start at the South Pole
         xlon = self.grid.lon
         ylat = np.flip(self.grid.lat)
         pvud = np.flipud(self.pv)
         return BarotropicField(xlon, ylat, pv_field=pvud, **barofield_kwargs)
 
     @classmethod
     def from_hn2016(cls, grid, time, barofield):
-        """Take PV from :py:mod:`hn2016_falwa` barotropic state object.
+        """Take PV from :py:mod:`falwa` barotropic state object.
 
         Parameters:
             grid (:py:class:`Grid` | None): Grid used for instantiated
                 :py:class:`State`. If ``None``, a new :py:class:`Grid` matching
                 the input is created.
             time (number | datetime): Valid time as number in seconds or
                 a datetime-like object.
-            barofield (:py:class:`hn2016_falwa.barotropic_field.BarotropicField`):
+            barofield (:py:class:`falwa.barotropic_field.BarotropicField`):
                 Instance from which to take PV field for instantiation.
 
         Returns:
             New :py:class:`State` instance.
 
         See :py:meth:`State.as_hn2016` for the inverse operation.
         """
@@ -362,7 +388,131 @@
     def rwp_diagnostics(self, *args, **kwargs):
         from . import plot
         plot.rwp_diagnostics(self._state, *args, **kwargs)
 
     def waveguides(self, *args, **kwargs):
         from . import plot
         plot.waveguides(self._state, *args, **kwargs)
+
+
+
+def _convert_sequence(seq):
+    """Put a sequence into a more "appropriate" container.
+
+    The compatibility of the objects in the sequence is checked only
+    rudimentarily. Implemented:
+
+    - numpy arrays → numpy array (with an additional dimension)
+    - numbers → numpy array
+    - States → StateList
+
+    Other sequences are returned as a list.
+    """
+    seq = list(seq)
+    if all(isinstance(x, np.ndarray) for x in seq):
+        return np.asarray(seq)
+    if all(isinstance(x, numbers.Number) for x in seq):
+        return np.asarray(seq)
+    if all(isinstance(x, State) for x in seq):
+        return StateList(seq)
+    return seq
+
+
+class StateList(collections.abc.Sequence):
+    """Immutable sequence of :py:class:`State` instances.
+
+    Parameters:
+        states (iterable of :py:class:`State`): states to be included.
+
+    One-dimensional collection intended to represent the temporal evolution of
+    a simulation. Provides access to all :py:class:`State` properties and
+    methods and a :py:meth:`.map` method for customized function application.
+
+    .. versionadded:: 3.1
+    """
+
+    def __init__(self, states):
+        self._states = tuple(states)
+        for state in self._states:
+            if not isinstance(state, State):
+                raise TypeError(f"non-State object in StateList: {state}")
+            # Enforce that all states have the same grid
+            assert self.grid == state.grid, "states in StateList must live on same grid"
+
+    def __getitem__(self, index):
+        return self._states[index]
+
+    def __len__(self):
+        return len(self._states)
+
+    def __iter__(self):
+        return iter(self._states)
+
+    def __repr__(self):
+        return f"<StateList with {len(self)} states>"
+
+    def __add__(self, other):
+        return StateList(itertools.chain(self, other))
+
+    # Broadcasting
+
+    def __getattr__(self, name):
+        # Need to separate simple attributes/properties and State methods:
+        # Attribute access can be evaluated immediately. Method access is
+        # converted to a partially evaluated function that collects the result
+        # from the invocation on every State in the StateList. Separate
+        # attributes and methods by checking if the (unbound) method exists on
+        # the State class.
+        attr = getattr(State, name, None)
+        if callable(attr):
+            return functools.partial(self.map, attr)
+        return _convert_sequence(getattr(state, name) for state in self)
+
+    def map(self, func, *args, **kwargs):
+        """Apply a function to each State and collect the output.
+
+        Parameters:
+            func (callable): Function to apply.
+            args: additional positional arguments supplied to `func` with every
+                invocation.
+            kwargs: additional keyword argument supplied to `func` with every
+                invocation.
+
+        Returns:
+            Sequence container with results from function applications. For
+            special return types of `func` (e.g. numbers) a specialized
+            container (e.g. numpy array) is returned.
+        """
+        return _convert_sequence(func(state, *args, **kwargs) for state in self)
+
+    def run(self, model, *args, **kwargs):
+        """Shortcut to :py:meth:`BarotropicModel.run`.
+
+        Parameters:
+            model (:py:class:`BarotropicModel`): the temporal integrator.
+            args: forwarded positional arguments.
+            kwargs: forwarded keyword arguments.
+
+        Returns:
+            2-tuple of final states (:py:class:`StateList`) and full simulation
+            outputs (list of :py:class:`StateList`).
+        """
+        all_last = []
+        all_step = []
+        for state in self:
+            last, step = model.run(state, *args, **kwargs)
+            all_last.append(last)
+            all_step.append(step)
+        return StateList(all_last), all_step
+
+    # Shortcuts
+
+    @property
+    def grid(self):
+        """The underlying :py:class:`.Grid` of all states"""
+        return self[0].grid if self else None
+
+    def as_dataset(self, *args, **kwargs):
+        """Shortcut to :py:func:`.io.as_dataset`"""
+        from . import io
+        return io.as_dataset(self, *args, **kwargs)
+
```

### Comparing `barotropic-3.0.1/barotropic/tests/test_examples.py` & `barotropic-3.1.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `barotropic-3.0.1/barotropic/tests/test_grid.py` & `barotropic-3.1.0/tests/test_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,17 +177,18 @@
         assert region.shape == (5, 4)
         assert np.allclose(region.lat, [-50, -60, -70, -80, -90])
         assert np.allclose(region.lon, [20, 30, 40, 50])
         assert np.allclose(region.extract(grid.lat), [-50, -60, -70, -80, -90])
         assert np.allclose(region.extract(grid.lon), [20, 30, 40, 50])
         assert region.extract(grid.phi2).shape == (5, 4)
 
-    def test_single(self):
+    @pytest.mark.parametrize("selection", [(80, 40), (slice(80, 80), slice(40, 40))])
+    def test_single(self, selection):
         grid = Grid(resolution=10.)
-        region = grid.region[80:80,40:40]
+        region = grid.region[selection]
         assert region.shape == (1, 1)
         assert np.allclose(region.lat, [40])
         assert np.allclose(region.lon, [80])
         assert region.extract(grid.fcor2).shape == (1, 1)
 
     def test_empty(self):
         grid = Grid(resolution=10.)
```

### Comparing `barotropic-3.0.1/barotropic.egg-info/SOURCES.txt` & `barotropic-3.1.0/src/barotropic.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 LICENSE
 README.md
-setup.py
-barotropic/__init__.py
-barotropic/constants.py
-barotropic/diagnostics.py
-barotropic/formatting.py
-barotropic/grid.py
-barotropic/init.py
-barotropic/io.py
-barotropic/model.py
-barotropic/plot.py
-barotropic/rhs.py
-barotropic/state.py
-barotropic.egg-info/PKG-INFO
-barotropic.egg-info/SOURCES.txt
-barotropic.egg-info/dependency_links.txt
-barotropic.egg-info/requires.txt
-barotropic.egg-info/top_level.txt
-barotropic/tests/__init__.py
-barotropic/tests/test_examples.py
-barotropic/tests/test_grid.py
-barotropic/tests/test_state.py
+pyproject.toml
+./src/barotropic/__init__.py
+./src/barotropic/constants.py
+./src/barotropic/diagnostics.py
+./src/barotropic/formatting.py
+./src/barotropic/grid.py
+./src/barotropic/init.py
+./src/barotropic/io.py
+./src/barotropic/model.py
+./src/barotropic/plot.py
+./src/barotropic/rhs.py
+./src/barotropic/state.py
+./src/barotropic.egg-info/PKG-INFO
+./src/barotropic.egg-info/SOURCES.txt
+./src/barotropic.egg-info/dependency_links.txt
+./src/barotropic.egg-info/requires.txt
+./src/barotropic.egg-info/top_level.txt
+tests/test_examples.py
+tests/test_grid.py
+tests/test_io.py
+tests/test_state.py
```

