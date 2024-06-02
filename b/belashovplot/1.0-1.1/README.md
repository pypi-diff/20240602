# Comparing `tmp/belashovplot-1.0.tar.gz` & `tmp/belashovplot-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "belashovplot-1.0.tar", last modified: Fri Sep  8 20:17:28 2023, max compression
+gzip compressed data, was "belashovplot-1.1.tar", last modified: Sun Jun  2 10:26:40 2024, max compression
```

## Comparing `belashovplot-1.0.tar` & `belashovplot-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-09-08 20:17:28.104531 belashovplot-1.0/
--rw-rw-rw-   0        0        0      229 2023-09-08 20:17:28.104531 belashovplot-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-09-08 20:17:28.070566 belashovplot-1.0/belashovplot/
--rw-rw-rw-   0        0        0      118 2023-09-08 20:17:23.000000 belashovplot-1.0/belashovplot/__init__.py
--rw-rw-rw-   0        0        0    76009 2023-09-08 20:10:48.000000 belashovplot-1.0/belashovplot/belashovplot.py
-drwxrwxrwx   0        0        0        0 2023-09-08 20:17:28.102533 belashovplot-1.0/belashovplot.egg-info/
--rw-rw-rw-   0        0        0      229 2023-09-08 20:17:27.000000 belashovplot-1.0/belashovplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-09-08 20:17:28.000000 belashovplot-1.0/belashovplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-08 20:17:27.000000 belashovplot-1.0/belashovplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-09-08 20:17:27.000000 belashovplot-1.0/belashovplot.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-09-08 20:17:27.000000 belashovplot-1.0/belashovplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-09-08 20:17:28.106531 belashovplot-1.0/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-09-08 20:17:23.000000 belashovplot-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:26:40.126692 belashovplot-1.1/
+-rw-rw-rw-   0        0        0      159 2024-06-02 10:26:40.125693 belashovplot-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-02 10:26:40.109720 belashovplot-1.1/belashovplot/
+-rw-rw-rw-   0        0        0      118 2023-09-08 20:17:23.000000 belashovplot-1.1/belashovplot/__init__.py
+-rw-rw-rw-   0        0        0    76571 2024-05-11 01:03:42.000000 belashovplot-1.1/belashovplot/belashovplot.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:26:40.124711 belashovplot-1.1/belashovplot.egg-info/
+-rw-rw-rw-   0        0        0      159 2024-06-02 10:26:40.000000 belashovplot-1.1/belashovplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-06-02 10:26:40.000000 belashovplot-1.1/belashovplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 10:26:40.000000 belashovplot-1.1/belashovplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-09-08 20:17:27.000000 belashovplot-1.1/belashovplot.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2024-06-02 10:26:40.000000 belashovplot-1.1/belashovplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 10:26:40.127709 belashovplot-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      253 2024-06-02 10:15:44.000000 belashovplot-1.1/setup.py
```

### Comparing `belashovplot-1.0/belashovplot/belashovplot.py` & `belashovplot-1.1/belashovplot/belashovplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -557,30 +557,39 @@
             window = figure_manager.window
             MaxWidth  = 0.9 * window.winfo_screenwidth()  / DPI
             MaxHeight = 0.9 * window.winfo_screenheight() / DPI
             plt.close(figure)
         size = ((MaxWidth if MaxWidth is not None else MaxHeight) + (MaxHeight if MaxHeight is not None else MaxWidth)) / 2
         self._Figure = plt.figure(dpi=DPI, figsize=(size, size))
         self._FigureAxes = self._Figure.add_axes((0,0,1,1))
+        self._FigureAxes.spines['top'].set_visible(False)
+        self._FigureAxes.spines['right'].set_visible(False)
+        self._FigureAxes.spines['bottom'].set_visible(False)
+        self._FigureAxes.spines['left'].set_visible(False)
+        self._FigureAxes.get_xaxis().set_ticks([])
+        self._FigureAxes.get_yaxis().set_ticks([])
         self._MaxWidth = MaxWidth
         self._MaxHeight = MaxHeight
         self._Columns = 0
         self._Rows = 0
         self._AxesList = []
         self._AxesCordsList = []
         self._SelectedIndex = None
         self._AxesWidthToHeight = 1.0
         self._init_plot_texts()
         self._init_rows_and_columns_texts()
         self._init_graphs_texts()
         self._init_paddings()
         self._init_highlighters()
-    def show    (self, finalize:bool=True):
+    def show    (self, *args, finalize:bool=True, block:bool=True, **kwargs):
         if finalize: self.finalize()
-        plt.show()
+        plt.show(*args, block=block, **kwargs)
+    def save(self, filename:str, finalize:bool=True):
+        if finalize: self.finalize()
+        plt.savefig(filename)
     def finalize(self):
         self._find_best_construction()
     def examine_virtual_figure_construction(self):
         self._calculate_axes_paddings()
         padding = 0.1
         points = 300
 
@@ -956,15 +965,15 @@
 
         # if self._HighlightTitle:                self._highlight(x(0), y(PlotH-TitleH), width(TitleW), height(TitleH))
         # if self._HighlightTopDescription:       self._highlight(x(0), y(PlotH-TitleH-self._TitlePad), width(TopDescriptionW), height(TopDescriptionH))
         # if self._HighlightBottomDescription:    self._highlight(x(0), y(0), width(BottomDescriptionW), height(BottomDescriptionH))
         # if self._HighlightLeftDescription:      self._highlight(x(0), y(BottomDescriptionH + self._BottomDescriptionPad), width(LeftDescriptionW), height(LeftDescriptionH))
         # if self._HighlightRightDescription:     self._highlight(x(0), y(BottomDescriptionH + self._BottomDescriptionPad), width(RightDescriptionW), height(LeftDescriptionH))
 
-        col_to_axes_x = lambda col: x(LeftDescriptionW + self._LeftDescriptionPad + RowLeftDescriptionW + GraphYAxisW + self._AxesLeftPad + col*(GraphTileW + self._GraphHorizontalPad))
+        col_to_axes_x = lambda col: x(LeftDescriptionW + self._LeftDescriptionPad + RowLeftDescriptionW + self._RowLeftDescriptionPad + GraphYAxisW + self._AxesLeftPad + col*(GraphTileW + self._GraphHorizontalPad))
         row_to_axes_y = lambda row: y(BottomDescriptionH + self._BottomDescriptionPad + ColumnBottomDescriptionH + self._ColumnBottomDescriptionPad + GraphDescriptionH + self._GraphDescriptionPad + GraphXAxisH + self._AxesBottomPad + (self._Rows - row - 1)*(GraphTileH + self._GraphVerticalPad))
 
         left_description_x = x(LeftDescriptionW + self._LeftDescriptionPad + RowLeftDescriptionW)
         for (r0, r1), description in zip(self._RowLeftDescriptionCordsList, self._RowLeftDescriptionList):
             figure.text(left_description_x, (row_to_axes_y(r0) + row_to_axes_y(r1) + y(AxesH))/2, description.text(), **description.font())
             # if self._HighlightRowLeftDescription: self._highlight(left_description_x-x(RowLeftDescriptionW), row_to_axes_y(r0), width(RowLeftDescriptionW), row_to_axes_y(r1)+y(AxesH)-row_to_axes_y(r0))
```

