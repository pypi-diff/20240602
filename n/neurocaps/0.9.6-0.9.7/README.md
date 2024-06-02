# Comparing `tmp/neurocaps-0.9.6.tar.gz` & `tmp/neurocaps-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocaps-0.9.6.tar", last modified: Fri May 31 05:18:19 2024, max compression
+gzip compressed data, was "neurocaps-0.9.7.tar", last modified: Sun Jun  2 20:36:28 2024, max compression
```

## Comparing `neurocaps-0.9.6.tar` & `neurocaps-0.9.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 05:18:19.197078 neurocaps-0.9.6/
--rw-rw-rw-   0        0        0     1077 2024-05-29 20:07:23.000000 neurocaps-0.9.6/LICENSE.md
--rw-rw-rw-   0        0        0       11 2024-05-31 00:35:11.000000 neurocaps-0.9.6/MANIFEST.in
--rw-rw-rw-   0        0        0    19418 2024-05-31 05:18:19.196426 neurocaps-0.9.6/PKG-INFO
--rw-rw-rw-   0        0        0    17788 2024-05-31 05:12:00.000000 neurocaps-0.9.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 05:18:19.148489 neurocaps-0.9.6/neurocaps/
--rw-rw-rw-   0        0        0       72 2024-05-27 18:25:53.000000 neurocaps-0.9.6/neurocaps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 05:18:19.175933 neurocaps-0.9.6/neurocaps/_utils/
--rw-rw-rw-   0        0        0      404 2024-05-31 05:11:21.000000 neurocaps-0.9.6/neurocaps/_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 05:18:19.179454 neurocaps-0.9.6/neurocaps/_utils/_cap_internals/
--rw-rw-rw-   0        0        0      126 2024-05-31 05:11:21.000000 neurocaps-0.9.6/neurocaps/_utils/_cap_internals/__init__.py
--rw-rw-rw-   0        0        0     2667 2024-05-31 05:12:00.000000 neurocaps-0.9.6/neurocaps/_utils/_cap_internals/_capgetter.py
--rw-rw-rw-   0        0        0      184 2024-05-31 05:11:21.000000 neurocaps-0.9.6/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
--rw-rw-rw-   0        0        0      645 2024-05-31 05:12:00.000000 neurocaps-0.9.6/neurocaps/_utils/_cap_internals/_run_kmeans.py
-drwxrwxrwx   0        0        0        0 2024-05-31 05:18:19.185557 neurocaps-0.9.6/neurocaps/_utils/_timeseriesextractor_internals/
--rw-rw-rw-   0        0        0      238 2024-05-23 03:16:17.000000 neurocaps-0.9.6/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
--rw-rw-rw-   0        0        0     2187 2024-05-27 18:25:53.000000 neurocaps-0.9.6/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
--rw-rw-rw-   0        0        0     5777 2024-05-27 18:25:53.000000 neurocaps-0.9.6/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
--rw-rw-rw-   0        0        0     8190 2024-05-27 18:25:53.000000 neurocaps-0.9.6/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
--rw-rw-rw-   0        0        0     2680 2024-05-27 18:25:53.000000 neurocaps-0.9.6/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
-drwxrwxrwx   0        0        0        0 2024-05-31 05:18:19.190465 neurocaps-0.9.6/neurocaps/analysis/
--rw-rw-rw-   0        0        0      139 2024-05-27 18:25:53.000000 neurocaps-0.9.6/neurocaps/analysis/__init__.py
--rw-rw-rw-   0        0        0    77464 2024-05-31 05:15:08.000000 neurocaps-0.9.6/neurocaps/analysis/cap.py
--rw-rw-rw-   0        0        0     4791 2024-05-27 18:25:53.000000 neurocaps-0.9.6/neurocaps/analysis/merge.py
--rw-rw-rw-   0        0        0     1626 2024-05-27 18:25:53.000000 neurocaps-0.9.6/neurocaps/analysis/standardize.py
-drwxrwxrwx   0        0        0        0 2024-05-31 05:18:19.192800 neurocaps-0.9.6/neurocaps/extraction/
--rw-rw-rw-   0        0        0       87 2024-05-27 18:25:53.000000 neurocaps-0.9.6/neurocaps/extraction/__init__.py
--rw-rw-rw-   0        0        0    33071 2024-05-31 05:12:00.000000 neurocaps-0.9.6/neurocaps/extraction/timeseriesextractor.py
-drwxrwxrwx   0        0        0        0 2024-05-31 05:18:19.195242 neurocaps-0.9.6/neurocaps.egg-info/
--rw-rw-rw-   0        0        0    19418 2024-05-31 05:18:19.000000 neurocaps-0.9.6/neurocaps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1002 2024-05-31 05:18:19.000000 neurocaps-0.9.6/neurocaps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 05:18:19.000000 neurocaps-0.9.6/neurocaps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      209 2024-05-31 05:18:19.000000 neurocaps-0.9.6/neurocaps.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-31 05:18:19.000000 neurocaps-0.9.6/neurocaps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1804 2024-05-31 05:11:21.000000 neurocaps-0.9.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-31 05:18:19.197078 neurocaps-0.9.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 20:36:28.385952 neurocaps-0.9.7/
+-rw-rw-rw-   0        0        0     1077 2024-05-29 20:07:23.000000 neurocaps-0.9.7/LICENSE.md
+-rw-rw-rw-   0        0        0       11 2024-05-31 00:35:11.000000 neurocaps-0.9.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    19422 2024-06-02 20:36:28.384935 neurocaps-0.9.7/PKG-INFO
+-rw-rw-rw-   0        0        0    17792 2024-06-02 20:35:20.000000 neurocaps-0.9.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 20:36:28.340273 neurocaps-0.9.7/neurocaps/
+-rw-rw-rw-   0        0        0       72 2024-05-27 18:25:53.000000 neurocaps-0.9.7/neurocaps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:36:28.364409 neurocaps-0.9.7/neurocaps/_utils/
+-rw-rw-rw-   0        0        0      404 2024-05-31 05:11:21.000000 neurocaps-0.9.7/neurocaps/_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:36:28.368612 neurocaps-0.9.7/neurocaps/_utils/_cap_internals/
+-rw-rw-rw-   0        0        0      126 2024-05-31 05:11:21.000000 neurocaps-0.9.7/neurocaps/_utils/_cap_internals/__init__.py
+-rw-rw-rw-   0        0        0     2667 2024-05-31 05:12:00.000000 neurocaps-0.9.7/neurocaps/_utils/_cap_internals/_capgetter.py
+-rw-rw-rw-   0        0        0      184 2024-05-31 05:11:21.000000 neurocaps-0.9.7/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
+-rw-rw-rw-   0        0        0      645 2024-05-31 05:12:00.000000 neurocaps-0.9.7/neurocaps/_utils/_cap_internals/_run_kmeans.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:36:28.374172 neurocaps-0.9.7/neurocaps/_utils/_timeseriesextractor_internals/
+-rw-rw-rw-   0        0        0      238 2024-05-23 03:16:17.000000 neurocaps-0.9.7/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
+-rw-rw-rw-   0        0        0     2187 2024-05-27 18:25:53.000000 neurocaps-0.9.7/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
+-rw-rw-rw-   0        0        0     5777 2024-05-27 18:25:53.000000 neurocaps-0.9.7/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
+-rw-rw-rw-   0        0        0     8190 2024-05-27 18:25:53.000000 neurocaps-0.9.7/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
+-rw-rw-rw-   0        0        0     2680 2024-05-27 18:25:53.000000 neurocaps-0.9.7/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:36:28.380123 neurocaps-0.9.7/neurocaps/analysis/
+-rw-rw-rw-   0        0        0      139 2024-05-27 18:25:53.000000 neurocaps-0.9.7/neurocaps/analysis/__init__.py
+-rw-rw-rw-   0        0        0    89350 2024-06-02 20:35:20.000000 neurocaps-0.9.7/neurocaps/analysis/cap.py
+-rw-rw-rw-   0        0        0     4791 2024-05-27 18:25:53.000000 neurocaps-0.9.7/neurocaps/analysis/merge.py
+-rw-rw-rw-   0        0        0     1626 2024-05-27 18:25:53.000000 neurocaps-0.9.7/neurocaps/analysis/standardize.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:36:28.382128 neurocaps-0.9.7/neurocaps/extraction/
+-rw-rw-rw-   0        0        0       87 2024-05-27 18:25:53.000000 neurocaps-0.9.7/neurocaps/extraction/__init__.py
+-rw-rw-rw-   0        0        0    33077 2024-06-02 20:35:20.000000 neurocaps-0.9.7/neurocaps/extraction/timeseriesextractor.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:36:28.383126 neurocaps-0.9.7/neurocaps.egg-info/
+-rw-rw-rw-   0        0        0    19422 2024-06-02 20:36:28.000000 neurocaps-0.9.7/neurocaps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1002 2024-06-02 20:36:28.000000 neurocaps-0.9.7/neurocaps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 20:36:28.000000 neurocaps-0.9.7/neurocaps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      209 2024-06-02 20:36:28.000000 neurocaps-0.9.7/neurocaps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-02 20:36:28.000000 neurocaps-0.9.7/neurocaps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1804 2024-06-02 20:35:20.000000 neurocaps-0.9.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 20:36:28.385952 neurocaps-0.9.7/setup.cfg
```

### Comparing `neurocaps-0.9.6/LICENSE.md` & `neurocaps-0.9.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.6/PKG-INFO` & `neurocaps-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.6
+Version: 0.9.7
 Summary: Co-activation Patterns (CAPs) Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Project-URL: Issues, https://github.com/donishadsmith/neurocaps/issues
 Project-URL: Changelog, https://github.com/donishadsmith/neurocaps/blob/main/CHANGELOG.md
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
@@ -184,22 +184,22 @@
 
 # Visualize CAPs
 # You can use seaborn's premade palettes as strings or generate your own custom palettes
 # Using seaborn's diverging_palette function, matplotlib's LinearSegmentedColormap, 
 # or other Classes or functions compatable with seaborn
 
 cap_analysis.caps2plot(visual_scope="regions", plot_options="outer product", 
-                            task_title="- Positive Valence", ncol=3, sharey=True, 
+                            suffix_title="- Positive Valence", ncol=3, sharey=True, 
                             subplots=True, cmap="coolwarm")
 # Create the colormap
 import seaborn as sns
 palette = sns.diverging_palette(260, 10, s=80, l=55, n=256, as_cmap=True)
 
 cap_analysis.caps2plot(visual_scope="nodes", plot_options="outer product", 
-                            task_title="- Positive Valence", ncol=3,sharey=True, 
+                            suffix_title="- Positive Valence", ncol=3,sharey=True, 
                             subplots=True, xlabel_rotation=90, tight_layout=False, 
                             hspace = 0.4, cmap=palette)
 
 ```
 **Plot Outputs:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/e1ab0f55-0c4c-4701-8f3a-838c2470d44d)
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/43e46a0a-8721-4df9-88fa-04758a34142e)
```

### Comparing `neurocaps-0.9.6/README.md` & `neurocaps-0.9.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -146,22 +146,22 @@
 
 # Visualize CAPs
 # You can use seaborn's premade palettes as strings or generate your own custom palettes
 # Using seaborn's diverging_palette function, matplotlib's LinearSegmentedColormap, 
 # or other Classes or functions compatable with seaborn
 
 cap_analysis.caps2plot(visual_scope="regions", plot_options="outer product", 
-                            task_title="- Positive Valence", ncol=3, sharey=True, 
+                            suffix_title="- Positive Valence", ncol=3, sharey=True, 
                             subplots=True, cmap="coolwarm")
 # Create the colormap
 import seaborn as sns
 palette = sns.diverging_palette(260, 10, s=80, l=55, n=256, as_cmap=True)
 
 cap_analysis.caps2plot(visual_scope="nodes", plot_options="outer product", 
-                            task_title="- Positive Valence", ncol=3,sharey=True, 
+                            suffix_title="- Positive Valence", ncol=3,sharey=True, 
                             subplots=True, xlabel_rotation=90, tight_layout=False, 
                             hspace = 0.4, cmap=palette)
 
 ```
 **Plot Outputs:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/e1ab0f55-0c4c-4701-8f3a-838c2470d44d)
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/43e46a0a-8721-4df9-88fa-04758a34142e)
```

### Comparing `neurocaps-0.9.6/neurocaps/_utils/_cap_internals/_capgetter.py` & `neurocaps-0.9.7/neurocaps/_utils/_cap_internals/_capgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.6/neurocaps/_utils/_cap_internals/_run_kmeans.py` & `neurocaps-0.9.7/neurocaps/_utils/_cap_internals/_run_kmeans.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.6/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py` & `neurocaps-0.9.7/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.6/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py` & `neurocaps-0.9.7/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.6/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py` & `neurocaps-0.9.7/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.6/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py` & `neurocaps-0.9.7/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.6/neurocaps/analysis/cap.py` & `neurocaps-0.9.7/neurocaps/analysis/cap.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
         Custom Key Structure:
         - 'maps': Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
         - 'nodes':  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
           Each label should match the parcellation index it represents. For example, if the parcellation label "1" corresponds to the left hemisphere 
           visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended.
           For timeseries extraction, this key is not required.
-        - 'regions': Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
+        - 'regions': Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. 
         
         Example 
         The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
 
         parcel_approach = {"Custom": {"maps": "/location/to/parcellation.nii.gz",
                              "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
                              "regions": {"Vis" : {"lh": [0,1],
@@ -129,20 +129,20 @@
             The number of CPU cores to use for multiprocessing, with joblib, to run multiple kmeans models if `cluster_selection_method` is not None. 
         kwargs: dict
             Dictionary to adjust certain parameters related to `cluster_selection_method` when set to "elbow". Additional parameters include:
              - "S": Adjusts the sensitivity of finding the elbow. Larger values are more conservative and less sensitive to small fluctuations. This package uses KneeLocator from the kneed package to identify the elbow. Default is 1.
              - "dpi": Adjusts the dpi of the elbow plot. Default is 300.
              - "figsize": Adjusts the size of the elbow plots.
         """
-        if n_cores and self.cluster_selection_method is not None:
+        if n_cores and self._cluster_selection_method is not None:
             if n_cores > cpu_count(): raise ValueError(f"More cores specified than available - Number of cores specified: {n_cores}; Max cores available: {cpu_count()}.")
             if isinstance(n_cores, int): self._n_cores = n_cores
             else: raise ValueError("`n_cores` must be an integer.")
         else:
-            if n_cores and self.cluster_selection_method == None: warnings.warn("Multiprocessing will not run since `cluster_selection_method` is None.")
+            if n_cores and self._cluster_selection_method == None: warnings.warn("Multiprocessing will not run since `cluster_selection_method` is None.")
             self._n_cores = None
 
         if runs:
             if isinstance(runs,int): runs = list(runs)
     
         self._runs = runs if runs else "all"
         self._standardize = standardize
@@ -294,31 +294,31 @@
             for subj_id in self._groups[group]:
                 if subj_id in self._subject_table.keys():
                     warnings.warn(f"Subject: {subj_id} appears more than once, only including the first instance of this subject in the analysis.") 
                 else:
                     self._subject_table.update({subj_id : group})
 
     def caps2plot(self, output_dir: str=None, plot_options: Union[str, list[str]]="outer product", visual_scope: list[str]="regions", 
-                       task_title: str=None, show_figs: bool=True, subplots: bool=False, **kwargs):
+                       suffix_title: str=None, show_figs: bool=True, subplots: bool=False, **kwargs):
         """Generate heatmaps and outer product plots of CAPs
 
         This function produces seaborn heatmaps for each CAP. If groups were given when the CAP class was initialized, plotting will be done for all CAPs for all groups.
 
         Parameters
         ----------
         output_dir: str, default=None
             Directory to save plots to. The directory will be created if it does not exist. If None, plots will not be saved.
         plot_options: str or list[str], default="outer product"
             Type of plots to create. Options are "outer product" or "heatmap".
         visual_scope: str or list[str], default="regions"
             Determines whether plotting is done at the region level or node level. 
             For region level, the value of each nodes in the same regions are averaged together then plotted.
             Options are "regions" or "nodes".
-        task_title: str, default=None
-            Serves as the title of each plot as well as the name of the saved file if `output_dir` is provided.
+        suffix_title: str, default=None
+            Appended to the title of each plot as well as the name of the saved file if `output_dir` is provided.
         show_figs: bool, default=True
             Whether to display figures.
         subplots: bool, default=True
             Whether to produce subplots for outer product plots.
         **kwargs: dict
             Keyword arguments used when saving figures. Valid keywords include:
             - "dpi": int, default=300
@@ -350,39 +350,57 @@
             - "sharey": bool, default=True
                 Share y-axis labels for subplots.
             - "xlabel_rotation": int, default=0
                 Rotation angle for x-axis labels.
             - "ylabel_rotation": int, default=0
                 Rotation angle for y-axis labels.
             - "annot": bool, default=False
-                Add values to cells on the outer product heatmap at the region level only.
+                Add values to cells.
+            - "fmt": str, default=".2g"
+                Modify how the annotated vales are presented.
             - "linewidths": float, default=0
                 Padding between each cell in the plot.
+            - "borderwidths": float, default=0
+                Width of the border around the plot.
             - "linecolor": str, default="black"
                 Color of the line that seperates each cell.
+            - "edgecolors": str, default=None
+                Color of the edges.
+            - "alpha": float, default=None
+                Controls transparancy and ranges from 0 (transparant) to 1 (opaque).
+            - "hemisphere_labels": bool, default=False
+                This option is only available when visual_scope="nodes". Instead of listing all individual labels, this parameter 
+                simplifies the labels to indicate only the left and right hemispheres, with a division line separating the cells 
+                belonging to each hemisphere. If set to True, "edgecolors" will not be used, and both "linewidths" and "linecolor" 
+                will be applied only to the division line. This option is available exclusively for "Custom" and "Schaefer" parcellations. 
+                WARNING, for the "Custom" option, the parcellation should be organized such that the first half of the labels/nodes belong to the left 
+                hemisphere and the latter half to the right hemisphere.
             - "cmap": str, Class, or function, default="coolwarm"
                 Color map for the cells in the plot. For this parameter, you can use premade color palettes or create custom ones.
                 Below is a list of valid options:
                 - Strings to call seaborn's premade palettes. Refer to seaborn's documentation for valid options.
                 - Seaborn's diverging_palette function to generate custom palettes.
                 - Matplotlib's LinearSegmentedColormap to generate custom palettes.
                 - Other classes or functions compatible with seaborn.
     
-         Notes
+        Notes
         -----
+        This function assumes that each node has a left and right counterpart (bilateral nodes). It also assumes that all the nodes belonging to the left hemisphere are listed first in the 'nodes' key.
+        For instance ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"].
+
         If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. Also, this function assumes that the background label is "zero". Do not add a a background label, in the "nodes" or "networks" key,
         the zero index should correspond the first id that is not zero.
 
         Custom Key Structure:
         - 'maps': Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
         - 'nodes':  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
           Each label should match the parcellation index it represents. For example, if the parcellation label "1" corresponds to the left hemisphere 
           visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended.
           For timeseries extraction, this key is not required.
-        - 'regions': Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
+        - 'regions': Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. 
         
         Example 
         The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
 
         parcel_approach = {"Custom": {"maps": "/location/to/parcellation.nii.gz",
                              "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
                              "regions": {"Vis" : {"lh": [0,1],
@@ -392,15 +410,15 @@
         """
         import itertools, os
 
         if not hasattr(self,"_caps"):
             raise AttributeError("Cannot plot caps since `self._caps` attribute does not exist. Run `self.get_caps()` first.")
         
         # Check if parcellation_approach is custom
-        if "Custom" in self.parcel_approach.keys() and ("nodes" not in self.parcel_approach["Custom"].keys() or "regions" not in self.parcel_approach["Custom"].keys()):
+        if "Custom" in self._parcel_approach.keys() and ("nodes" not in self._parcel_approach["Custom"].keys() or "regions" not in self._parcel_approach["Custom"].keys()):
             _check_parcel_approach(parcel_approach=self._parcel_approach, call="caps2plot")
 
         # Check labels
         check_caps = self._caps[list(self._caps.keys())[0]]
         check_caps = check_caps[list(check_caps.keys())[0]]
         if check_caps.shape[0] != len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]): 
                 raise ValueError("Number of rois/nodes used for CAPs does not equal the number of rois/nodes specified in `parcel_approach`.")
@@ -435,24 +453,35 @@
                         suptitle_fontsize = kwargs["suptitle_fontsize"] if kwargs and "suptitle_fontsize" in kwargs.keys() else 20,
                         tight_layout = kwargs["tight_layout"] if kwargs and "tight_layout" in kwargs.keys() else True,
                         rect = kwargs["rect"] if kwargs and "rect" in kwargs.keys() else [0, 0.03, 1, 0.95],
                         sharey = kwargs["sharey"] if kwargs and "sharey" in kwargs.keys() else True,
                         xlabel_rotation = kwargs["xlabel_rotation"] if kwargs and "xlabel_rotation" in kwargs.keys() else 0,
                         ylabel_rotation = kwargs["ylabel_rotation"] if kwargs and "ylabel_rotation" in kwargs.keys() else 0,
                         annot = kwargs["annot"] if kwargs and "annot" in kwargs.keys() else False,
+                        fmt = kwargs["fmt"] if kwargs and "fmt" in kwargs.keys() else ".2g",
                         linewidths = kwargs["linewidths"] if kwargs and "linewidths" in kwargs.keys() else 0,
                         linecolor = kwargs["linecolor"] if kwargs and "linecolor" in kwargs.keys() else "black",
-                        cmap = kwargs["cmap"] if kwargs and "cmap" in kwargs.keys() else "coolwarm"
+                        cmap = kwargs["cmap"] if kwargs and "cmap" in kwargs.keys() else "coolwarm",
+                        edgecolors = kwargs["edgecolors"] if kwargs and "edgecolors" in kwargs.keys() else None,
+                        alpha = kwargs["alpha"] if kwargs and "alpha" in kwargs.keys() else None,
+                        hemisphere_labels = kwargs["hemisphere_labels"] if kwargs and "hemisphere_labels" in kwargs.keys() else False,
+                        borderwidths = kwargs["borderwidths"] if kwargs and "borderwidths" in kwargs.keys() else 0,
                         )
         
         if kwargs:
             invalid_kwargs = {key : value for key, value in kwargs.items() if key not in plot_dict.keys()}
             if len(invalid_kwargs.keys()) > 0:
                 print(f"Invalid kwargs arguments used and will be ignored {invalid_kwargs}.")
 
+        if plot_dict["hemisphere_labels"] == True:
+            if "nodes" not in visual_scope:
+                raise ValueError("`hemisphere_labels` is only available when `visual_scope == 'nodes'`.")
+            if "AAL" in self._parcel_approach.keys():
+                raise ValueError("`hemisphere_labels` is only available for 'Custom' and 'Schaefer'.")
+        
         # Ensure plot_options and visual_scope are lists
         plot_options = plot_options if type(plot_options) == list else list(plot_options)
         visual_scope = visual_scope if type(visual_scope) == list else list(visual_scope)
         # Initialize outer product attribute
         if "outer product" in plot_options: self._outer_product = {}
 
         distributed_list = list(itertools.product(plot_options,visual_scope,self._groups.keys()))
@@ -468,20 +497,20 @@
                     if list(self._parcel_approach.keys())[0] in ["Schaefer", "AAL"]:
                         cap_dict, columns = self._caps, self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]
                     else:
                         cap_dict, columns = self._caps , [x[0] + " " + x[1] for x in list(itertools.product(["LH", "RH"],self._parcel_approach["Custom"]["regions"].keys()))]
 
                 #  Generate plot for each group
                 if plot_option == "outer product": self._generate_outer_product_plots(group=group, plot_dict=plot_dict, cap_dict=cap_dict, columns=columns, subplots=subplots,
-                                                                                    output_dir=output_dir, task_title=task_title, show_figs=show_figs, scope=scope)
+                                                                                    output_dir=output_dir, suffix_title=suffix_title, show_figs=show_figs, scope=scope)
                 elif plot_option == "heatmap": self._generate_heatmap_plots(group=group, plot_dict=plot_dict, cap_dict=cap_dict, columns=columns,
-                                                                            output_dir=output_dir, task_title=task_title, show_figs=show_figs, scope=scope)
+                                                                            output_dir=output_dir, suffix_title=suffix_title, show_figs=show_figs, scope=scope)
             
     def _create_regions(self):
-        # Internal function to create an attribute called `region_caps`. Purpose is to average the vales of all nodes in a corresponding region to create region heatmaps or outer product plots
+        # Internal function to create an attribute called `region_caps`. Purpose is to average the values of all nodes in a corresponding region to create region heatmaps or outer product plots
         self._region_caps = {group: {} for group in self._groups.keys()}
         for group in self._groups.keys():
             for cap in self._caps[group].keys():
                 region_caps = {}
                 if list(self._parcel_approach.keys())[0] != "Custom":
                     for region in self._parcel_approach[list(self._parcel_approach.keys())[0]]["regions"]:
                         if len(region_caps) == 0:
@@ -489,55 +518,55 @@
                         else:
                             region_caps = np.hstack([region_caps, np.average(self._caps[group][cap][np.array([index for index, node in enumerate(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]) if region in node])])])
                 else:
                     region_dict = self._parcel_approach["Custom"]["regions"]
                     region_keys = region_dict.keys()
                     for region in region_keys:
                         roi_indxs = np.array(region_dict[region]["lh"] + region_dict[region]["rh"])
-
                         if len(region_caps) == 0:
                             region_caps= np.array([np.average(self._caps[group][cap][roi_indxs])])
                         else:
                             region_caps= np.hstack([region_caps, np.average(self._caps[group][cap][roi_indxs])])
 
                 self._region_caps[group].update({cap: region_caps})
     
-    def _generate_outer_product_plots(self, group, plot_dict, cap_dict, columns, subplots, output_dir, task_title, show_figs, scope):
+    def _generate_outer_product_plots(self, group, plot_dict, cap_dict, columns, subplots, output_dir, suffix_title, show_figs, scope):
         import matplotlib.pyplot as plt, os
         from seaborn import heatmap
 
         # Nested dictionary for group
         self._outer_product[group] = {}
 
         # Create base grid for subplots
         if subplots:
             # Max five subplots per row for default
             default_col = len(cap_dict[group].keys()) if len(cap_dict[group].keys()) <= 5 else 5
             ncol = plot_dict["ncol"] if plot_dict["ncol"] != None else default_col
+            if ncol > len(cap_dict[group].keys()): ncol = len(cap_dict[group].keys())
             # Pad nrow, since int will round down, padding is needed for cases where len(cap_dict[group].keys())/ncol is a float. This will add the extra row needed
             x_pad = 0 if len(cap_dict[group].keys())/ncol <= 1 else 1
             nrow = plot_dict["nrow"] if plot_dict["nrow"] != None else x_pad + int(len(cap_dict[group].keys())/ncol)
-
+            
             subplot_figsize = (8 * ncol, 6 * nrow) if plot_dict["figsize"] == (8,6) else plot_dict["figsize"] 
 
             fig, axes = plt.subplots(nrow, ncol, sharex=False, sharey=plot_dict["sharey"], figsize=subplot_figsize)
-            suptitle = f"{group} {task_title}" if task_title else f"{group}"
+            suptitle = f"{group} {suffix_title}" if suffix_title else f"{group}"
             fig.suptitle(suptitle, fontsize=plot_dict["suptitle_fontsize"])
             fig.subplots_adjust(hspace=plot_dict["hspace"], wspace=plot_dict["wspace"])  
             if plot_dict["tight_layout"]: fig.tight_layout(rect=plot_dict["rect"])  
 
             # Current subplot
             axes_x, axes_y = [0,0] 
 
         # Iterate over CAPs
         for cap in cap_dict[group].keys():
             # Calculate outer product
             self._outer_product[group].update({cap: np.outer(cap_dict[group][cap],cap_dict[group][cap])})
             # Create labels if nodes requested for scope
-            if scope == "nodes":
+            if scope == "nodes" and plot_dict["hemisphere_labels"] == False:
                 import collections
                 
                 # Get frequency of each major hemisphere and region in Schaefer, AAL, or Custom atlas
                 if list(self._parcel_approach.keys())[0] == "Schaefer":
                     frequency_dict = dict(collections.Counter([names[0] + " " + names[1] for names in [name.split("_")[0:2] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]]]))
                 elif list(self._parcel_approach.keys())[0] == "AAL":
                     frequency_dict = collections.Counter([name.split("_")[0] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]])
@@ -563,24 +592,57 @@
                         starting_value += frequency_dict[names_list[num-1]] 
                         labels[starting_value] = name
 
             if subplots: 
                 ax = axes[axes_y] if nrow == 1 else axes[axes_x,axes_y]
                 # Modify tick labels based on scope
                 if scope == "regions":
-                    display = heatmap(ax=ax, data=self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"], xticklabels=columns, yticklabels=columns, cbar_kws={"shrink": plot_dict["shrink"]}, annot=plot_dict["annot"])
+                    display = heatmap(ax=ax, data=self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"], 
+                                      xticklabels=columns, yticklabels=columns, cbar_kws={"shrink": plot_dict["shrink"]}, annot=plot_dict["annot"], fmt=plot_dict["fmt"],
+                                      edgecolors=plot_dict["edgecolors"], alpha=plot_dict["alpha"])
                 else:
-                    display = heatmap(ax=ax, data=self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"], cbar_kws={"shrink": plot_dict["shrink"]})
-
-                    ticks = [i for i, label in enumerate(labels) if label]  
+                    if plot_dict["hemisphere_labels"] == False:
+                        display = heatmap(ax=ax, data=self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], 
+                                        linecolor=plot_dict["linecolor"], cbar_kws={"shrink": plot_dict["shrink"]}, annot=plot_dict["annot"], fmt=plot_dict["fmt"],
+                                        edgecolors=plot_dict["edgecolors"], alpha=plot_dict["alpha"])
+                    else:
+                        display = heatmap(ax=ax, data=self._outer_product[group][cap], cmap=plot_dict["cmap"], cbar_kws={"shrink": plot_dict["shrink"]}, 
+                                          annot=plot_dict["annot"], fmt=plot_dict["fmt"], alpha=plot_dict["alpha"])
+                        
+                    if plot_dict["hemisphere_labels"] == False:
+                        ticks = [i for i, label in enumerate(labels) if label]  
+
+                        ax.set_xticks(ticks)  
+                        ax.set_xticklabels([label for label in labels if label]) 
+                        ax.set_yticks(ticks)  
+                        ax.set_yticklabels([label for label in labels if label]) 
+                    else:
+                        n_labels = len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"])
+                        division_line = n_labels//2
+                        left_hemisphere_tick = (0 + division_line)//2
+                        right_hemisphere_tick = (division_line + n_labels)//2
+
+                        ax.set_xticks([left_hemisphere_tick,right_hemisphere_tick])
+                        ax.set_xticklabels(["LH", "RH"])
+                        ax.set_yticks([left_hemisphere_tick,right_hemisphere_tick])
+                        ax.set_yticklabels(["LH", "RH"])
+                        
+                        plot_dict["linewidths"] = plot_dict["linewidths"] if plot_dict["linewidths"] != 0 else 1
 
-                    ax.set_xticks(ticks)  
-                    ax.set_xticklabels([label for label in labels if label]) 
-                    ax.set_yticks(ticks)  
-                    ax.set_yticklabels([label for label in labels if label]) 
+                        ax.axhline(division_line, color=plot_dict["linecolor"], linewidth=plot_dict["linewidths"])
+                        ax.axvline(division_line, color=plot_dict["linecolor"], linewidth=plot_dict["linewidths"])
+                
+                # Add border 
+                if plot_dict['borderwidths'] != 0:
+                    border_length = self._outer_product[group][cap].shape[0] if scope == "regions" else self._outer_product[group][cap].shape[0]
+
+                    display.axhline(y=0, color=plot_dict["linecolor"],linewidth=plot_dict["borderwidths"])
+                    display.axhline(y=border_length, color=plot_dict["linecolor"],linewidth=plot_dict["borderwidths"])
+                    display.axvline(x=0, color=plot_dict["linecolor"],linewidth=plot_dict["borderwidths"])
+                    display.axvline(x=border_length, color=plot_dict["linecolor"],linewidth=plot_dict["borderwidths"])
 
                 # Modify label sizes
                 display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
 
                 if plot_dict["sharey"] == True:
                     if axes_y == 0: display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
                 else:
@@ -596,97 +658,161 @@
                 else:
                     axes_y += 1
 
             else:
                 # Create new plot for each iteration when not subplot
                 plt.figure(figsize=plot_dict["figsize"])
 
-                plot_title = f"{group} {cap} {task_title}" if task_title else f"{group} {cap}"
-                if scope == "regions": display = heatmap(self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"], xticklabels=columns, yticklabels=columns, cbar_kws={'shrink': plot_dict["shrink"]})
+                plot_title = f"{group} {cap} {suffix_title}" if suffix_title else f"{group} {cap}"
+                if scope == "regions": display = heatmap(self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"], 
+                                                         xticklabels=columns, yticklabels=columns, cbar_kws={'shrink': plot_dict["shrink"]}, annot=plot_dict["annot"], fmt=plot_dict["fmt"],
+                                                         edgecolors=plot_dict["edgecolors"], alpha=plot_dict["alpha"])
                 else: 
-                    display = heatmap(self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"], xticklabels=[], yticklabels=[], cbar_kws={'shrink': plot_dict["shrink"]})
-                    ticks = [i for i, label in enumerate(labels) if label]  
+                    if plot_dict["hemisphere_labels"] == False:
+                        display = heatmap(self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"], 
+                                        xticklabels=[], yticklabels=[], cbar_kws={'shrink': plot_dict["shrink"]}, annot=plot_dict["annot"], fmt=plot_dict["fmt"],
+                                        edgecolors=plot_dict["edgecolors"], alpha=plot_dict["alpha"])
+                    else:
+                        display = heatmap(self._outer_product[group][cap], cmap=plot_dict["cmap"], xticklabels=[], yticklabels=[], cbar_kws={'shrink': plot_dict["shrink"]}, 
+                                          annot=plot_dict["annot"], fmt=plot_dict["fmt"], alpha=plot_dict["alpha"])
+                    
+                    if plot_dict["hemisphere_labels"] == False:
+                        ticks = [i for i, label in enumerate(labels) if label]  
+
+                        display.set_xticks(ticks)  
+                        display.set_xticklabels([label for label in labels if label]) 
+                        display.set_yticks(ticks)  
+                        display.set_yticklabels([label for label in labels if label]) 
 
-                    display.set_xticks(ticks)  
-                    display.set_xticklabels([label for label in labels if label]) 
-                    display.set_yticks(ticks)  
-                    display.set_yticklabels([label for label in labels if label]) 
+                    else:
+                        n_labels = len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"])
+                        division_line = n_labels//2
+                        left_hemisphere_tick = (0 + division_line)//2
+                        right_hemisphere_tick = (division_line + n_labels)//2
+
+                        display.set_xticks([left_hemisphere_tick,right_hemisphere_tick])
+                        display.set_xticklabels(["LH", "RH"])
+                        display.set_yticks([left_hemisphere_tick,right_hemisphere_tick])
+                        display.set_yticklabels(["LH", "RH"])
+                        
+                        plot_dict["linewidths"] = plot_dict["linewidths"] if plot_dict["linewidths"] != 0 else 1
+
+                        plt.axhline(division_line, color=plot_dict["linecolor"], linewidth=plot_dict["linewidths"])
+                        plt.axvline(division_line, color=plot_dict["linecolor"], linewidth=plot_dict["linewidths"])
                 
+                # Add border
+                if plot_dict['borderwidths'] != 0:
+                    border_length = self._outer_product[group][cap].shape[0] if scope == "regions" else self._outer_product[group][cap].shape[0]
+
+                    display.axhline(y=0, color=plot_dict["linecolor"],linewidth=plot_dict["borderwidths"])
+                    display.axhline(y=border_length, color=plot_dict["linecolor"],linewidth=plot_dict["borderwidths"])
+                    display.axvline(x=0, color=plot_dict["linecolor"],linewidth=plot_dict["borderwidths"])
+                    display.axvline(x=border_length, color=plot_dict["linecolor"],linewidth=plot_dict["borderwidths"])
+
                 display.set_title(plot_title, fontdict= {'fontsize': plot_dict["fontsize"]})
 
                 display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
                 display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
 
                 # Save individual plots
                 if output_dir:
-                    partial_filename = f"{group}_{cap}_{task_title}" if task_title else f"{group}_{cap}"
+                    partial_filename = f"{group}_{cap}_{suffix_title}" if suffix_title else f"{group}_{cap}"
                     full_filename = f"{partial_filename.replace(' ','_')}_outer_product_heatmap-regions.png" if scope == "regions" else f"{partial_filename.replace(' ','_')}_outer_product_heatmap-nodes.png"
                     display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')
         
         # Remove subplots with no data
         if subplots: [fig.delaxes(ax) for ax in axes.flatten() if not ax.has_data()]
 
         # Save subplot
         if subplots and output_dir: 
-            partial_filename = f"{group}_CAPs_{task_title}" if task_title else f"{group}_CAPs"
+            partial_filename = f"{group}_CAPs_{suffix_title}" if suffix_title else f"{group}_CAPs"
             full_filename = f"{partial_filename.replace(' ','_')}_outer_product_heatmap-regions.png" if scope == "regions" else f"{partial_filename.replace(' ','_')}_outer_product_heatmap-nodes.png"
             display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')    
         
         # Display figures
         if not show_figs: plt.close()
 
-    def _generate_heatmap_plots(self, group, plot_dict, cap_dict, columns, output_dir, task_title, show_figs, scope):
+    def _generate_heatmap_plots(self, group, plot_dict, cap_dict, columns, output_dir, suffix_title, show_figs, scope):
         import matplotlib.pyplot as plt, os, pandas as pd
         from seaborn import heatmap
         
         # Initialize new grid
         plt.figure(figsize=plot_dict["figsize"])
 
         if scope == "regions": 
-            display = heatmap(pd.DataFrame(cap_dict[group], index=columns), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"], cbar_kws={'shrink': plot_dict["shrink"]}) 
+            display = heatmap(pd.DataFrame(cap_dict[group], index=columns), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"],
+                               linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"], cbar_kws={'shrink': plot_dict["shrink"]}, fmt=plot_dict["fmt"],
+                               edgecolors=plot_dict["edgecolors"], alpha=plot_dict["alpha"], ) 
         else: 
             # Create Labels
-            import collections
-            if list(self._parcel_approach.keys())[0] == "Schaefer":
-                frequency_dict = dict(collections.Counter([names[0] + " " + names[1] for names in [name.split("_")[0:2] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]]]))
-            elif list(self._parcel_approach.keys())[0] == "AAL":
-                frequency_dict = collections.Counter([name.split("_")[0] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]])
-            else:
-                    frequency_dict = {}
-                    for id in columns:
-                        hemisphere_id = "LH" if id.startswith("LH ") else "RH"
-                        region_id = re.split("LH |RH ", id)[-1]
-                        frequency_dict.update({id: len(self._parcel_approach["Custom"]["regions"][region_id][hemisphere_id.lower()])})
-            names_list = list(frequency_dict.keys())
-            labels = ["" for _ in range(0,len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]))]
+            if plot_dict["hemisphere_labels"] == False:
+                import collections
+                if list(self._parcel_approach.keys())[0] == "Schaefer":
+                    frequency_dict = dict(collections.Counter([names[0] + " " + names[1] for names in [name.split("_")[0:2] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]]]))
+                elif list(self._parcel_approach.keys())[0] == "AAL":
+                    frequency_dict = collections.Counter([name.split("_")[0] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]])
+                else:
+                        frequency_dict = {}
+                        for id in columns:
+                            hemisphere_id = "LH" if id.startswith("LH ") else "RH"
+                            region_id = re.split("LH |RH ", id)[-1]
+                            frequency_dict.update({id: len(self._parcel_approach["Custom"]["regions"][region_id][hemisphere_id.lower()])})
+                names_list = list(frequency_dict.keys())
+                labels = ["" for _ in range(0,len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]))]
 
-            starting_value = 0
+                starting_value = 0
 
-            # Iterate through names_list and assign the starting indices corresponding to unique region and hemisphere key
-            for num, name in enumerate(names_list): 
-                if num == 0:
-                    labels[0] = name
-                else:
-                    # Shifting to previous frequency of the preceding netwerk to obtain the new starting value of the subsequent region and hemosphere pair
-                    starting_value += frequency_dict[names_list[num-1]] 
-                    labels[starting_value] = name
+                # Iterate through names_list and assign the starting indices corresponding to unique region and hemisphere key
+                for num, name in enumerate(names_list): 
+                    if num == 0:
+                        labels[0] = name
+                    else:
+                        # Shifting to previous frequency of the preceding netwerk to obtain the new starting value of the subsequent region and hemosphere pair
+                        starting_value += frequency_dict[names_list[num-1]] 
+                        labels[starting_value] = name
+
+                display = heatmap(pd.DataFrame(cap_dict[group], columns=cap_dict[group].keys()), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], 
+                                linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"], cbar_kws={'shrink': plot_dict["shrink"]}, annot=plot_dict["annot"], fmt=plot_dict["fmt"],
+                                edgecolors=plot_dict["edgecolors"], alpha=plot_dict["alpha"])
+
+                plt.yticks(ticks=[pos for pos, label in enumerate(labels) if label], labels=names_list) 
+
+            else:
+                display = heatmap(pd.DataFrame(cap_dict[group], columns=cap_dict[group].keys()), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], 
+                                  cbar_kws={'shrink': plot_dict["shrink"]}, annot=plot_dict["annot"], fmt=plot_dict["fmt"], alpha=plot_dict["alpha"])
+                
+                n_labels = len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"])
+                division_line = n_labels//2
+                left_hemisphere_tick = (0 + division_line)//2
+                right_hemisphere_tick = (division_line + n_labels)//2
 
-            display = heatmap(pd.DataFrame(cap_dict[group], columns=cap_dict[group].keys()), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"], cbar_kws={'shrink': plot_dict["shrink"]})
+                display.set_yticks([left_hemisphere_tick,right_hemisphere_tick])
+                display.set_yticklabels(["LH", "RH"])
+                
+                plot_dict["linewidths"] = plot_dict["linewidths"] if plot_dict["linewidths"] != 0 else 1
+
+                plt.axhline(division_line, color=plot_dict["linecolor"], linewidth=plot_dict["linewidths"])
 
-            plt.yticks(ticks=[pos for pos, label in enumerate(labels) if label], labels=names_list)  
+        if plot_dict['borderwidths'] != 0:
+                y_length = len(cap_dict[group][list(cap_dict[group].keys())[0]])
 
+                display.axhline(y=0, color=plot_dict["linecolor"],linewidth=plot_dict["borderwidths"])
+                display.axhline(y=y_length, color=plot_dict["linecolor"],linewidth=plot_dict["borderwidths"])
+                display.axvline(x=0, color=plot_dict["linecolor"],linewidth=plot_dict["borderwidths"])
+                display.axvline(x=len(self._caps[group]), color=plot_dict["linecolor"],linewidth=plot_dict["borderwidths"])
+                
         display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
         display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
 
-        plot_title = f"{group} CAPs {task_title}" if task_title else f"{group} CAPs" 
+        plot_title = f"{group} CAPs {suffix_title}" if suffix_title else f"{group} CAPs" 
         display.set_title(plot_title, fontdict= {'fontsize': plot_dict["fontsize"]})
 
         # Save plots
         if output_dir:
-            partial_filename = f"{group}_CAPs_{task_title}" if task_title else f"{group}_CAPs"
+            partial_filename = f"{group}_CAPs_{suffix_title}" if suffix_title else f"{group}_CAPs"
             full_filename = f"{partial_filename.replace(' ','_')}_heatmap-regions.png" if scope == "regions" else f"{partial_filename.replace(' ','_')}_heatmap-nodes.png"
             display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')    
    
         # Display figures
         if not show_figs: plt.close()
 
     def calculate_metrics(self, subject_timeseries: Union[dict[dict[np.ndarray]], str], tr: float=None, runs: Union[int]=None, continuous_runs: bool=False, 
@@ -698,15 +824,14 @@
         The metrics include:
 
         - 'temporal fraction': The proportion of total volumes spent in a single CAP over all volumes in a run.
         - 'persistence;: The average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time).
         - 'counts': The frequency of each CAP observed in a run.
         - 'transition frequency': The number of switches between different CAPs across the entire run.
 
-
         Parameters
         ----------
         subject_timeseries: dict[dict[np.ndarray]] or str
             Path of the pickle file containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or
             the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject ID as a string, 
             the second level must consist of the run numbers in the form of 'run-#' (where # is the corresponding number of the run), and the last level must consist of the timeseries 
             (as a numpy array) associated with that run.
@@ -871,23 +996,25 @@
             for metric in df_dict.keys():
                 filename = os.path.splitext(file_name.rstrip())[0].rstrip() + f"-{metric.replace(' ','_')}" if file_name else f"{metric.replace(' ','_')}"
                 df_dict[f"{metric}"].to_csv(path_or_buf=os.path.join(output_dir,filename + ".csv"), sep=",", index=False)
 
         if return_df:
             return df_dict
 
-    def caps2corr(self, output_dir: str=None, show_figs: bool=True, **kwargs):
+    def caps2corr(self, output_dir: str=None, suffix_title: str=None, show_figs: bool=True, **kwargs):
         """Generate Correlation Matrix
 
         Produces the correlation matrix of all CAPs. If groups were given when the CAP class was initialized, a correlation matrix will be generated for each group. 
 
         Parameters
         ----------
         output_dir: str, default=None
             Directory to save plots to. The directory will be created if it does not exist. If None, plots will not be saved.
+        suffix_title: str, default=None
+            Appended to the title of each plot as well as the name of the saved file if `output_dir` is provided.
         show_figs: bool, default=True
             Whether to display figures.
         **kwargs: dict
             Keyword arguments used when saving figures. Valid keywords include:
             - "dpi": int, default=300
                 Dots per inch for the figure. Default is 300 if `output_dir` is provided and `dpi` is not specified.
             - "figsize": tuple, default=(8, 6)
@@ -902,18 +1029,26 @@
                 Fraction by which to shrink the colorbar.
             - "xlabel_rotation": int, default=0
                 Rotation angle for x-axis labels.
             - "ylabel_rotation": int, default=0
                 Rotation angle for y-axis labels.
             - "annot": bool, default=False
                 Add values to each cell.
+            - "fmt": str, default=".2g",
+                Modify how the annotated vales are presented.
             - "linewidths": float, default=0
                 Padding between each cell in the plot.
+            - "borderwidths": float, default=0
+                Width of the border around the plot.
             - "linecolor": str, default="black"
                 Color of the line that seperates each cell.
+            - "edgecolors": str, default=None
+                Color of the edges.
+            - "alpha": float, default=None
+                Controls transparancy and ranges from 0 (transparant) to 1 (opaque).
             - "cmap": str, Class, or function, default="coolwarm"
                 Color map for the cells in the plot. For this parameter, you can use premade color palettes or create custom ones.
                 Below is a list of valid options:
                 - Strings to call seaborn's premade palettes. Refer to seaborn's documentation for valid options.
                 - Seaborn's diverging_palette function to generate custom palettes.
                 - Matplotlib's LinearSegmentedColormap to generate custom palettes.
                 - Other classes or functions compatible with seaborn.
@@ -932,55 +1067,68 @@
                         yticklabels_size = kwargs["yticklabels_size"] if kwargs and "yticklabels_size" in kwargs.keys() else 8,
                         shrink = kwargs["shrink"] if kwargs and "shrink" in kwargs.keys() else 0.8,
                         xlabel_rotation = kwargs["xlabel_rotation"] if kwargs and "xlabel_rotation" in kwargs.keys() else 0,
                         ylabel_rotation = kwargs["ylabel_rotation"] if kwargs and "ylabel_rotation" in kwargs.keys() else 0,
                         annot = kwargs["annot"] if kwargs and "annot" in kwargs.keys() else False,
                         linewidths = kwargs["linewidths"] if kwargs and "linewidths" in kwargs.keys() else 0,
                         linecolor = kwargs["linecolor"] if kwargs and "linecolor" in kwargs.keys() else "black",
-                        cmap = kwargs["cmap"] if kwargs and "cmap" in kwargs.keys() else "coolwarm"
+                        cmap = kwargs["cmap"] if kwargs and "cmap" in kwargs.keys() else "coolwarm",
+                        fmt = kwargs["fmt"] if kwargs and "fmt" in kwargs.keys() else ".2g",
+                        borderwidths = kwargs["borderwidths"] if kwargs and "borderwidths" in kwargs.keys() else 0,
+                        edgecolors = kwargs["edgecolors"] if kwargs and "edgecolors" in kwargs.keys() else None,
+                        alpha = kwargs["alpha"] if kwargs and "alpha" in kwargs.keys() else None
                         )
         
         if kwargs:
             invalid_kwargs = {key : value for key, value in kwargs.items() if key not in plot_dict.keys()}
             if len(invalid_kwargs.keys()) > 0:
                 print(f"Invalid kwargs arguments used and will be ignored {invalid_kwargs}.")
 
-        for group in self.caps.keys():
+        for group in self._caps.keys():
             # Refresh grid for each iteration
             plt.figure(figsize=plot_dict["figsize"])
 
-            df = pd.DataFrame(self.caps[group])
+            df = pd.DataFrame(self._caps[group])
             display = heatmap(df.corr(), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"],
-                              cbar_kws={'shrink': plot_dict["shrink"]}, annot=plot_dict["annot"]) 
+                              cbar_kws={'shrink': plot_dict["shrink"]}, annot=plot_dict["annot"], fmt=plot_dict["fmt"], edgecolors=plot_dict["edgecolors"], alpha=plot_dict["alpha"]) 
+            # Add Border
+            if plot_dict["borderwidths"] != 0:
+                display.axhline(y=0, color=plot_dict["linecolor"],linewidth=plot_dict["borderwidths"])
+                display.axhline(y=df.corr().shape[1], color=plot_dict["linecolor"],linewidth=plot_dict["borderwidths"])
+                display.axvline(x=0, color=plot_dict["linecolor"],linewidth=plot_dict["borderwidths"])
+                display.axvline(x=df.corr().shape[0], color=plot_dict["linecolor"],linewidth=plot_dict["borderwidths"])
+            
             # Modify label sizes
             display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
             display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
             # Set plot name
-            plot_title = f"{group} - CAPs Correlation Matrix" 
+            plot_title = f"{group} CAPs Correlation Matrix {suffix_title}" if suffix_title else f"{group} CAPs Correlation Matrix" 
             display.set_title(plot_title, fontdict= {'fontsize': plot_dict["fontsize"]})
 
             # Display figures
             if not show_figs: plt.close()
             # Save figure
             if output_dir:
                 if not os.path.exists(output_dir): os.makedirs(output_dir)
-                full_filename = f"{group.replace(' ', '_')}_correlation_matrix.png"
+                full_filename = f"{group.replace(' ', '_')}_correlation_matrix_{suffix_title}.png" if suffix_title else f"{group.replace(' ', '_')}_correlation_matrix.png"
                 display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')
 
-    def caps2surf(self, output_dir: str=None, show_figs: bool=True, fwhm: float=None, 
+    def caps2surf(self, output_dir: str=None, suffix_title: str=None, show_figs: bool=True, fwhm: float=None, 
                   fslr_density: str="32k", method: str="linear", save_stat_map: bool=False, **kwargs):
         """Project CAPs onto surface plots
         
         Converts atlas into a stat map by replacing labels with the corresponding from the cluster centroids then plots on a surface plot.
         This function uses surfplot for surface plotting.
 
         Parameters
         ----------
         output_dir: str, default=None
             Directory to save plots to. The directory will be created if it does not exist. If None, plots will not be saved. 
+        suffix_title: str, default=None
+            Appended to the title of each plot as well as the name of the saved file if `output_dir` is provided.
         show_figs: bool, default=True
             Whether to display figures.
         fwhm: float, defualt=None
             Strength of spatial smoothing to apply (in millimeters) to the statistical map prior to interpolating from MNI152 space to fslr surface space. 
             Note, this can assist with coverage issues in the plot.
         fslr_density: str, default="32k"
             Density of the fslr surface when converting from MNI152 space to fslr surface. Options are "32k" or "164k".
@@ -1134,20 +1282,20 @@
                             alpha=plot_dict["cbar_alpha"], color_range=(plot_min,plot_max))
 
                 # Color bar
                 kws = dict(location=plot_dict["cbar_location"], draw_border=plot_dict["cbar_draw_border"], aspect=plot_dict["cbar_aspect"], shrink=plot_dict["cbar_shrink"],
                         decimals=plot_dict["cbar_decimals"], pad=plot_dict["cbar_pad"], fraction=plot_dict["cbar_fraction"], n_ticks=plot_dict["cbar_n_ticks"], 
                         fontsize=plot_dict["cbar_fontsize"])
                 fig = p.build(cbar_kws=kws, figsize=plot_dict["figsize"], scale=plot_dict["scale"])
-                fig_name = f"{group} - {cap}"
+                fig_name = f"{group} {cap} {suffix_title}" if suffix_title else f"{group} {cap}"
                 fig.axes[0].set_title(fig_name, pad=plot_dict["title_pad"])      
                 
                 if show_figs:
                     fig.show()
                 
                 if output_dir:
-                    save_name = f"{group.replace(' ', '_')}_{cap.replace('-', '_')}.png"
+                    save_name = f"{group.replace(' ', '_')}_{cap.replace('-', '_')}_{suffix_title}.png" if suffix_title else f"{group.replace(' ', '_')}_{cap.replace('-', '_')}.png" 
                     fig.savefig(os.path.join(output_dir, save_name), dpi=plot_dict["dpi"])
                     # Save stat map
                     if save_stat_map: 
                         stat_map_name = save_name.replace(".png", ".nii.gz")
                         nib.save(stat_map, stat_map_name)
```

### Comparing `neurocaps-0.9.6/neurocaps/analysis/merge.py` & `neurocaps-0.9.7/neurocaps/analysis/merge.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.6/neurocaps/analysis/standardize.py` & `neurocaps-0.9.7/neurocaps/analysis/standardize.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.6/neurocaps/extraction/timeseriesextractor.py` & `neurocaps-0.9.7/neurocaps/extraction/timeseriesextractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,32 +415,32 @@
         # Obtain the column indices associated with the rois; add logic for roi_indx == 0 since it would be recognized as False
         if roi_indx or roi_indx == 0:
             if type(roi_indx) == int:
                 plot_indxs = roi_indx
             
             elif type(roi_indx) == str:
                 # Check if parcellation_approach is custom
-                if "Custom" in self.parcel_approach.keys() and "nodes" not in self.parcel_approach["Custom"].keys():
+                if "Custom" in self._parcel_approach.keys() and "nodes" not in self._parcel_approach["Custom"].keys():
                     _check_parcel_approach(parcel_approach=self._parcel_approach, call="visualize_bold")
                 plot_indxs = self._parcel_approach[self._parcel_approach.keys[0]]["nodes"].index(roi_indx)
             
             elif type(roi_indx) == list:
                 if all([isinstance(indx,int) for indx in roi_indx]):
                     plot_indxs = np.array(roi_indx)
                 elif all([isinstance(indx,str) for indx in roi_indx]):
                     # Check if parcellation_approach is custom
-                    if "Custom" in self.parcel_approach.keys() and "nodes" not in self.parcel_approach["Custom"].keys():
+                    if "Custom" in self._parcel_approach.keys() and "nodes" not in self._parcel_approach["Custom"].keys():
                         _check_parcel_approach(parcel_approach=self._parcel_approach, call="visualize_bold")
                     plot_indxs = np.array([self._parcel_approach[self._parcel_approach.keys[0]]["nodes"].index(index) for index in roi_indx])
                 else:
                     raise ValueError("All elements in `roi_indx` need to be all strings or all integers.")
                 
         elif region:
-            if "Custom" in self.parcel_approach.keys():
-                if "regions" not in self.parcel_approach["Custom"].keys():
+            if "Custom" in self._parcel_approach.keys():
+                if "regions" not in self._parcel_approach["Custom"].keys():
                     _check_parcel_approach(parcel_approach=self._parcel_approach, call="visualize_bold")
                 else:
                     plot_indxs =  np.array(self._parcel_approach["Custom"]["regions"][region]["lh"] + self._parcel_approach["Custom"]["regions"][region]["rh"])
             else:
                 plot_indxs = np.array([index for index, label in enumerate(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]) if region in label])
         
         plt.figure(figsize=plot_dict["figsize"])
```

### Comparing `neurocaps-0.9.6/neurocaps.egg-info/PKG-INFO` & `neurocaps-0.9.7/neurocaps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.6
+Version: 0.9.7
 Summary: Co-activation Patterns (CAPs) Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Project-URL: Issues, https://github.com/donishadsmith/neurocaps/issues
 Project-URL: Changelog, https://github.com/donishadsmith/neurocaps/blob/main/CHANGELOG.md
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
@@ -184,22 +184,22 @@
 
 # Visualize CAPs
 # You can use seaborn's premade palettes as strings or generate your own custom palettes
 # Using seaborn's diverging_palette function, matplotlib's LinearSegmentedColormap, 
 # or other Classes or functions compatable with seaborn
 
 cap_analysis.caps2plot(visual_scope="regions", plot_options="outer product", 
-                            task_title="- Positive Valence", ncol=3, sharey=True, 
+                            suffix_title="- Positive Valence", ncol=3, sharey=True, 
                             subplots=True, cmap="coolwarm")
 # Create the colormap
 import seaborn as sns
 palette = sns.diverging_palette(260, 10, s=80, l=55, n=256, as_cmap=True)
 
 cap_analysis.caps2plot(visual_scope="nodes", plot_options="outer product", 
-                            task_title="- Positive Valence", ncol=3,sharey=True, 
+                            suffix_title="- Positive Valence", ncol=3,sharey=True, 
                             subplots=True, xlabel_rotation=90, tight_layout=False, 
                             hspace = 0.4, cmap=palette)
 
 ```
 **Plot Outputs:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/e1ab0f55-0c4c-4701-8f3a-838c2470d44d)
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/43e46a0a-8721-4df9-88fa-04758a34142e)
```

### Comparing `neurocaps-0.9.6/neurocaps.egg-info/SOURCES.txt` & `neurocaps-0.9.7/neurocaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.6/pyproject.toml` & `neurocaps-0.9.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 7322 2c20 2277 6865 656c  uptools", "wheel
 00000030: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
 00000040: 6420 3d20 2273 6574 7570 746f 6f6c 732e  d = "setuptools.
 00000050: 6275 696c 645f 6d65 7461 220d 0a0d 0a5b  build_meta"....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 6e65 7572 6f63 6170 7322 0d0a 7665   "neurocaps"..ve
-00000080: 7273 696f 6e20 3d20 2230 2e39 2e36 220d  rsion = "0.9.6".
+00000080: 7273 696f 6e20 3d20 2230 2e39 2e37 220d  rsion = "0.9.7".
 00000090: 0a6c 6963 656e 7365 203d 207b 7465 7874  .license = {text
 000000a0: 203d 2022 4d49 5420 4c69 6365 6e73 6522   = "MIT License"
 000000b0: 7d0d 0a61 7574 686f 7273 203d 205b 7b6e  }..authors = [{n
 000000c0: 616d 6520 3d20 2244 6f6e 6973 6861 2053  ame = "Donisha S
 000000d0: 6d69 7468 222c 2065 6d61 696c 203d 2022  mith", email = "
 000000e0: 646f 6e69 7368 6173 6d69 7468 406f 7574  donishasmith@out
 000000f0: 6c6f 6f6b 2e63 6f6d 227d 5d0d 0a64 6573  look.com"}]..des
```

