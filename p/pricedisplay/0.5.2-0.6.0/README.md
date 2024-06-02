# Comparing `tmp/pricedisplay-0.5.2.tar.gz` & `tmp/pricedisplay-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pricedisplay-0.5.2.tar", max compression
+gzip compressed data, was "pricedisplay-0.6.0.tar", max compression
```

## Comparing `pricedisplay-0.5.2.tar` & `pricedisplay-0.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35148 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/LICENSE.md
--rw-r--r--   0        0        0     1924 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/README.md
--rw-r--r--   0        0        0       29 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pricedisplay/__init__.py
--rw-r--r--   0        0        0       65 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pricedisplay/__main__.py
--rw-r--r--   0        0        0     8357 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pricedisplay/application.py
--rw-r--r--   0        0        0      175 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pricedisplay/config.migrate
--rw-r--r--   0        0        0     3292 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pricedisplay/config.template
--rw-r--r--   0        0        0    11531 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pricedisplay/configparser.py
--rw-r--r--   0        0        0     8075 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pricedisplay/datahandler.py
--rw-r--r--   0        0        0     1217 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pricedisplay/exceptions.py
--rw-r--r--   0        0        0    29483 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pricedisplay/graphics.py
--rw-r--r--   0        0        0      795 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2959 1970-01-01 00:00:00.000000 pricedisplay-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-06-02 13:39:36.402269 pricedisplay-0.6.0/LICENSE.md
+-rw-r--r--   0        0        0     1924 2024-06-02 13:39:36.402269 pricedisplay-0.6.0/README.md
+-rw-r--r--   0        0        0       29 2024-06-02 13:39:36.402269 pricedisplay-0.6.0/pricedisplay/__init__.py
+-rw-r--r--   0        0        0       65 2024-06-02 13:39:36.402269 pricedisplay-0.6.0/pricedisplay/__main__.py
+-rw-r--r--   0        0        0     8937 2024-06-02 13:39:36.402269 pricedisplay-0.6.0/pricedisplay/application.py
+-rw-r--r--   0        0        0      175 2024-06-02 13:39:36.402269 pricedisplay-0.6.0/pricedisplay/config.migrate
+-rw-r--r--   0        0        0     4092 2024-06-02 13:39:36.402269 pricedisplay-0.6.0/pricedisplay/config.template
+-rw-r--r--   0        0        0    11535 2024-06-02 13:39:36.402269 pricedisplay-0.6.0/pricedisplay/configparser.py
+-rw-r--r--   0        0        0     8157 2024-06-02 13:39:36.402269 pricedisplay-0.6.0/pricedisplay/datahandler.py
+-rw-r--r--   0        0        0     1217 2024-06-02 13:39:36.402269 pricedisplay-0.6.0/pricedisplay/exceptions.py
+-rw-r--r--   0        0        0    32123 2024-06-02 13:39:36.402269 pricedisplay-0.6.0/pricedisplay/graphics.py
+-rw-r--r--   0        0        0      795 2024-06-02 13:39:36.402269 pricedisplay-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2959 1970-01-01 00:00:00.000000 pricedisplay-0.6.0/PKG-INFO
```

### Comparing `pricedisplay-0.5.2/LICENSE.md` & `pricedisplay-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pricedisplay-0.5.2/README.md` & `pricedisplay-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pricedisplay-0.5.2/pricedisplay/application.py` & `pricedisplay-0.6.0/pricedisplay/application.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from .configparser import Config
 from .datahandler import PriceDataHandler
 from .graphics import PriceDisplay
 
 from .exceptions import *
 
-__version__ = '0.5.1'
+__version__ = '0.6.0'
 
 _debug = 0
 
 _noErrors = 0
 _unexpectedError = 1
 _configError = 2
 _displayError = 3
@@ -43,14 +43,22 @@
 			dataOptions['source'] = options['data.source']
 			
 			displayOptions['carets'] = (
 				options['caret.style.above'],
 				options['caret.style.below']
 			)
 			
+			displayOptions['extremesVisible'] = options['extremes.visible']
+			displayOptions['extremes'] = (
+				options['extremes.style.lowest'],
+				options['extremes.style.highest']
+			)
+			
+			displayOptions['missing'] = options['missing.style']
+			
 			displayOptions['limits'] = (
 				options['price.low'],
 				options['price.high']
 			)
 			
 			displayOptions['day'] = (
 				options['day.begins'],
@@ -129,35 +137,49 @@
 	
 	def _DailyDataUpdate( self, now ):
 		"""Checks the data source for new data. If there is price data for tomorrow, updates the display."""
 		
 		prices = self._data.GetPrices()
 		
 		if not prices.tomorrow:
-			self._data.Update()
-			prices = self._data.GetPrices()
-			self._lastDataUpdate = now
+			try:
+				self._data.Update()
+				prices = self._data.GetPrices()
+				self._lastDataUpdate = now
+			
+			# catch any request errors and try again later
+			except DataRequestError:
+				pass
 			
 			if prices.tomorrow:
 				self._display.Update( prices )
 				self._lastDisplayUpdate = now
 	
 	def _HourlyUpdate( self, now ):
 		"""Updates the display every hour."""
 		
+		# try updating prices, if any of the prices for today are missing
 		prices = self._data.GetPrices()
+		if None in prices.today:
+			try:
+				self._data.Update()
+				prices = self._data.GetPrices()
+			except DataRequestError:
+				pass
+		
 		self._display.Update( prices )
 		self._lastDisplayUpdate = now
 	
 	def _Mainloop( self ):
 		"""Mainloop of the application."""
 		
 		delta = datetime.timedelta( minutes=self._updateFrequency )
 		while self._running:
 			now = datetime.datetime.now()
+			self._HourlyUpdate( now )
 			
 			# is midnight
 			if now.day != self._lastDataUpdate.day:
 				self._MidnightUpdate( now )
 			
 			# new data will be available soon, check every five minutes
 			if now > self._dataAvailable:
```

### Comparing `pricedisplay-0.5.2/pricedisplay/config.template` & `pricedisplay-0.6.0/pricedisplay/config.template`

 * *Files 12% similar despite different names*

```diff
@@ -73,14 +73,43 @@
             value: ▼
         
         below:
             description: "The style of the caret below the current hour in the graph."
             type: char
             question: Carot below graph?
             value: ▲
+
+extremes:
+    visible:
+        description: "Display markers for todays highest and lowest price."
+        essential: true
+        type: bool
+        question: Display markers for extremes?
+        value: false
+        
+    style:
+        highest:
+            description: "The style of the marker for the highest price today in the graph."
+            type: char
+            question: Highest price marker?
+            value: ∧
+        
+        lowest:
+            description: "The style of the marker for the lowest price today in the graph."
+            type: char
+            question: Lowest price marker?
+            value: ∨
+
+missing:
+    style:
+        description: "The style of the missing price symbol."
+        type: char
+        question: Missing price symbol?
+        value: "-"
+
 day:
     begins:
         description: "Day begins at this hour."
         type: int
         question: Day begins?
         value: 6
```

### Comparing `pricedisplay-0.5.2/pricedisplay/configparser.py` & `pricedisplay-0.6.0/pricedisplay/configparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import usersettings
 import yaml
 
 from .exceptions import ConfigParsingError
 from .exceptions import CorruptedTemplateError, MissingTemplateError, TemplateParsingError
 
-__version__ = '0.5.1'
+__version__ = '0.6.0'
 
 class _Queries:
 	def _YesNo( self, question ):
 		"""A simple yes/no prompt."""
 		
 		answer = None
 		while answer == None:
@@ -52,15 +52,15 @@
 			if value in ( False, 'False', 'false', '0' ):
 				return False
 			
 			raise ValueError( 'Invalid value' )
 		
 		if type == 'char':
 			value = str( value )
-			if len(value) == 1:
+			if len( value ) == 1:
 				return value
 		
 		if type == 'float':
 			try:
 				return float( value )
 			except:
 				raise ValueError( 'Invalid value' )
@@ -74,15 +74,15 @@
 		if type == 'string':
 			return str( value )
 		
 		if type == 'time':
 			try:
 				parts = value.split(':')
 				for part in parts:
-					int(part)
+					int( part )
 			except:
 				raise ValueError( 'Invalid value' )
 			
 			return str( value )
 		
 		raise ValueError( 'Invalid type' )
```

### Comparing `pricedisplay-0.5.2/pricedisplay/datahandler.py` & `pricedisplay-0.6.0/pricedisplay/datahandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 import json
 import requests
 
 from requests.exceptions import *
 from .exceptions import MissingOptionError
 from .exceptions import NoDataError, DataParsingError, DataRequestError
 
-__version__ = '0.5.0'
+__version__ = '0.6.0'
 
 class PriceData:
 	"""Represents the price data and its statistics."""
 	
 	_hasData = False
 	low = None
 	high = None
 	average = None
 	
 	def __init__( self, prices ):
-		self._data = prices		
+		self._data = prices
 		
 		# filter out None for comparing prices
 		filtered = []
 		for price in prices:
 			if price != None:
 				filtered.append( price )
 		
@@ -49,14 +49,17 @@
 			return PriceData( data )
 	
 	def __len__( self ):
 		return len( self._data )
 	
 	def __str__( self ):
 		return str( self._data )
+	
+	def index( self, *args, **kwargs ):
+		return self._data.index( *args, **kwargs )
 
 class DailyData:
 	"""Represents the price data for yesterday, today, and tomorrow."""
 	
 	def __init__( self, yesterday, today, tomorrow ):
 		self._data = [ yesterday, today, tomorrow ]
```

### Comparing `pricedisplay-0.5.2/pricedisplay/exceptions.py` & `pricedisplay-0.6.0/pricedisplay/exceptions.py`

 * *Files identical despite different names*

### Comparing `pricedisplay-0.5.2/pricedisplay/graphics.py` & `pricedisplay-0.6.0/pricedisplay/graphics.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import math
 import sparklines
 import warnings
 
 from .exceptions import MissingOptionError
 from .exceptions import CollectionSizeError, WindowSizeError, WindowPositionError
 
-__version__ = '0.5.2'
+__version__ = '0.6.0'
 
 class Point:
 	"""Represents a point on the terminal screen."""
 	
 	y = 0
 	x = 0
 	pos = ( 0,0 )
@@ -200,23 +200,29 @@
 class Graph( _PriceDisplayWindow ):
 	"""Displays a simple sparkline graph of the power price, color coded based on the limits given in options. The size of the graph, carets used to mark the current hour, and the number of past hours to show can be given as options."""
 	
 	minSize = Size( ( 12, 36 ) )
 	_defaultOptions = {
 		'height': minSize.height,
 		'width': minSize.width,
-		'carets': [ '▼', '▲' ],
+		'carets': ( '▼', '▲' ),
+		'extremes': ( '∨', '∧' ),
+		'extremesVisible': False,
+		'missing': '-',
 		'pastHours': 8
 	}
 	
 	def __init__( self, pos, options, parent=None ):
 		opts = self._defaultOptions.copy()
 		opts.update( options )
 		
 		self._carets = opts['carets']
+		self._extremes = opts['extremes']
+		self._extremesVisible = opts['extremesVisible']
+		self._missing = opts['missing']
 		pastHours = opts['pastHours']
 		width = opts['width']
 		
 		# normalize the number of past hours to fit in the space allowed
 		if pastHours < 0:
 			pastHours = 0
 		
@@ -226,102 +232,195 @@
 		self._pastHours = pastHours
 		
 		h = opts['height']
 		w = opts['width']
 		size = Size( ( h, w ) )
 		_PriceDisplayWindow.__init__(self, size, pos, options, parent)
 	
+	def _AddPadding( self, lines ):
+		"""Adds carets to indicate the current hour in the sparklines."""
+		
+		pos, neg = lines
+		hours = len( ( pos + neg )[0] )
+		
+		# add an empty line to the beginning and end to always fit the carets
+		pos = [ ' '*hours ] + pos
+		neg = neg + [ ' '*hours ]
+		
+		return pos, neg
+	
 	def _AddCarets( self, lines ):
 		"""Adds carets to indicate the current hour in the sparklines."""
 		
 		pos, neg = lines
 		carets = self._carets
 		pastHours = self._pastHours
 		curHour = pastHours + 1
 		hours = len( ( pos + neg )[0] )
 		
-		# add an empty line to the beginning and end to always fit the carets
-		# if there are no lines, include the caret on the line
-		if pos:
-			pos = [ ' '*hours ] + pos
-			pos = self._AddUpperCaret( pos )
-		else:
-			pos = [ ' '*pastHours + carets[0] + ' '*(hours - curHour) ]
-		
-		if neg:
-			neg = neg + [ ' '*hours ]
-			neg = self._AddLowerCaret( neg )
-		else:
-			neg = [ ' '*pastHours + carets[1] + ' '*(hours - curHour) ]
+		pos = self._AddUpperCaret( pos )
+		neg = self._AddLowerCaret( neg )
 		
 		return pos, neg
 	
 	def _AddLowerCaret( self, lines ):
 		"""Add the lower caret to the given lines."""
 		
-		carets = self._carets
-		curHour = self._pastHours
+		symbol = self._carets[1]
+		hour = self._pastHours
+		lines = self._AddSymbolBelow( lines, hour, symbol )
+		
+		return lines
+	
+	def _AddUpperCaret( self, lines ):
+		"""Add the upper caret to the given lines."""
+		
+		symbol = self._carets[0]
+		hour = self._pastHours
+		lines = self._AddSymbolAbove( lines, hour, symbol )
+		
+		return lines
+	
+	def _AddSymbolAbove( self, lines, hour, symbol ):
+		"""Finds the highest possible position for the symbol in positive lines, searching from top down."""
+		
+		if not 0 <= hour < len( lines[0] ):
+			return lines
+		
+		if len( lines ) == 1:
+			lines[0] = lines[0][ : hour ] + symbol + lines[0][ hour+1 : ]
+			return lines
+		
+		i = 0
+		while i < len( lines ) - 1:
+			line = lines[i]
+			next = lines[i + 1]
+			
+			# last empty space for the symbol, if price is positive
+			if line[ hour ] == ' ' and next[ hour ] != ' ':
+				symbolLine = line[ : hour ] + symbol + line[ hour+1 : ]
+				lines[i] = symbolLine
+				break
+			
+			# last possible line for the symbol
+			if i == len( lines ) - 2:
+				symbolLine = next[ : hour ] + symbol + next[ hour+1 : ]
+				lines[-1] = symbolLine
+				break
+			
+			i += 1
+		
+		return lines
+	
+	def _AddSymbolBelow( self, lines, hour, symbol ):
+		"""Finds the lowest possible position for the symbol in negative lines, searching from bottom up."""
+		
+		if not 0 <= hour < len( lines[0] ):
+			return lines
+		
+		if len( lines ) == 1:
+			lines[0] = lines[0][ : hour ] + symbol + lines[0][ hour+1 : ]
+			return lines
+		
+		if len( lines ) == 2:
+			lines[1] = lines[1][ : hour ] + symbol + lines[1][ hour+1 : ]
+			return lines
 		
-		# find the lowest possible position for the upper caret, searching from bottom up
 		i = iMax = len( lines ) - 2
 		while i > 0:
 			prev = lines[i + 1]
 			cur = lines[i]
 			next = lines[i - 1]
 			
-			# first possible line for the lower caret, if negative price extends all the way down
-			if i == iMax and cur[ curHour ] != ' ' and next[ curHour ] == ' ':
-				lowerCaretLine = prev[ : curHour ] + carets[1] + prev[ curHour+1 : ]
-				lines[i + 1] = lowerCaretLine
+			# first possible line for the symbol, if negative price extends all the way down
+			if i == iMax and cur[ hour ] != ' ' and next[ hour ] == ' ':
+				symbolLine = prev[ : hour ] + symbol + prev[ hour+1 : ]
+				lines[i + 1] = symbolLine
 				break
 			
 			# first empty space under negative sparkline on current hour
-			if prev[ curHour ] != ' ' and cur[ curHour ] != ' ' and next[ curHour ] == ' ':
-				lowerCaretLine = prev[ : curHour ] + carets[1] + prev[ curHour+1 : ]
-				lines[i + 1] = lowerCaretLine
+			if prev[ hour ] != ' ' and cur[ hour ] != ' ' and next[ hour ] == ' ':
+				symbolLine = prev[ : hour ] + symbol + prev[ hour+1 : ]
+				lines[i + 1] = symbolLine
 				break
 			
-			# last possible line for the lower caret, if price is positive
-			# the character is empty, because the value for the price is None
-			if i == 1 and next[ curHour ] == ' ':
-				lowerCaretLine = next[ : curHour ] + carets[1] + next[ curHour+1 : ]
-				lines[0] = lowerCaretLine
+			# last possible line for the symbol
+			if i == 1:
+				symbolLine = next[ : hour ] + symbol + next[ hour+1 : ]
+				lines[0] = symbolLine
 				break
 			
 			i -= 1
 		
 		return lines
 	
-	def _AddUpperCaret( self, lines ):
-		"""Add the upper caret to the given lines."""
+	def _AddLowestMarker( self, lines, priceData ):
+		"""Adds a marker for the lowest price today."""
 		
-		carets = self._carets
-		curHour = self._pastHours
+		symbol = self._extremes[0]
+		pos, neg = lines
 		
-		# find the highest possible position for the upper caret, searching from top down
-		i = 0
-		while i < len( lines ) - 1:
-			line = lines[i]
-			next = lines[i + 1]
-			
-			# last empty space for the upper caret, if price is positive
-			if line[ curHour ] == ' ' and next[ curHour ] != ' ':
-				upperCaretLine = line[ : curHour ] + carets[0] + line[ curHour+1 : ]
-				lines[i] = upperCaretLine
-				break
-			
-			# last possible line for the upper caret, if price is negative
-			if i == len( lines ) - 2 and next[ curHour ] == ' ':
-				upperCaretLine = next[ : curHour ] + carets[0] + next[ curHour+1 : ]
-				lines[-1] = upperCaretLine
-				break
+		low = priceData.today.low
+		hour = priceData.today.index( low )
+		
+		hoursInDay = len( priceData.today )
+		curHour = self._CurrentHourIndex( hoursInDay )
+		index = hour - curHour + self._pastHours
+		
+		# don't add the marker for current hour
+		if hour != curHour:
+			if low > 0:
+				pos = self._AddSymbolAbove( pos, index, symbol )
+			else:
+				neg = self._AddSymbolBelow( neg, index, symbol )
+		
+		return pos, neg
+	
+	def _AddHighestMarker( self, lines, priceData ):
+		"""Adds a marker for the highest price today."""
+		
+		symbol = self._extremes[1]
+		pos, neg = lines
+		
+		high = priceData.today.high
+		hour = priceData.today.index( high )
+		
+		hoursInDay = len( priceData.today )
+		curHour = self._CurrentHourIndex( hoursInDay )
+		index = hour - curHour + self._pastHours
+		
+		# don't add the marker for current hour
+		if hour != curHour:
+			if high > 0:
+				pos = self._AddSymbolAbove( pos, index, symbol )
+			else:
+				neg = self._AddSymbolBelow( neg, index, symbol )
+		
+		return pos, neg
+	
+	def _AddMissingSymbol( self, lines, visiblePrices ):
+		"""Adds a symbol for missing prices."""
+		
+		pos, neg = lines
+		hour = 0
+		while hour < len( visiblePrices ):
+			if visiblePrices[hour] == None:
+				if len( pos ) > 1:
+					line = pos[-1]
+					line = line[ : hour ] + self._missing + line[ hour+1 : ]
+					pos[-1] = line
+				
+				else:
+					line = neg[0]
+					line = line[ : hour ] + self._missing + line[ hour+1 : ]
+					neg[0] = line
 			
-			i += 1
+			hour += 1
 		
-		return lines
+		return pos, neg
 	
 	def _AddLines( self, lines, colors, prices ):
 		"""Adds the sparklines and the lower caret line."""
 		
 		win = self._win
 		pos, neg = lines
 		
@@ -335,33 +434,35 @@
 		# add the lower caret line
 		win.addstr( neg[-1] )
 	
 	def _AddNegativeLines( self, lines, colors, prices ):
 		"""Adds negative lines to the graph."""
 		
 		win = self._win
+		symbols = self._carets + self._extremes + tuple( self._missing )
 		
 		for line in lines[:-1]:
 			for hour in range( len(line) ):
 				price = prices[hour]
-				if not line[hour] in self._carets and price != None and price < 0:
+				if line[hour] not in symbols and price != None and price < 0:
 					win.addstr( line[hour], colors[hour] | curses.A_REVERSE )
 				else:
 					win.addstr( line[hour] )
 			
 			win.addstr( '\n' )
 	
 	def _AddPositiveLines( self, lines, colors, prices ):
 		"""Adds positive lines to the graph."""
 		
 		win = self._win
+		symbols = self._carets + self._extremes + tuple( self._missing )
 		
 		for line in lines[1:]:
 			for hour in range( len(line) ):
-				if not line[hour] in self._carets:
+				if line[hour] not in symbols:
 					win.addstr( line[hour], colors[hour] )
 				else:
 					win.addstr( line[hour] )
 			
 			win.addstr( '\n' )
 	
 	def _GetColors( self, visiblePrices ):
@@ -533,37 +634,46 @@
 	
 	def Update( self, priceData ):
 		"""Updates the graph, taking into account the changes in dst."""
 		
 		win = self._win
 		visiblePrices = self._GetVisiblePrices( priceData )
 		lines = self._GetSparklines( visiblePrices )
+		lines = self._AddPadding( lines )
+		
+		if self._extremesVisible:
+			lines = self._AddHighestMarker( lines, priceData )
+			lines = self._AddLowestMarker( lines, priceData )
+		
+		lines = self._AddMissingSymbol( lines, visiblePrices )
 		lines = self._AddCarets( lines )
 		colors = self._GetColors( visiblePrices )
 		
 		win.clear()
 		self._AddLines( lines, colors, visiblePrices )
 		win.refresh()
 
 ###  text based display windows for price details  ###
 
 class _DetailWindow( _PriceDisplayWindow ):
 	"""Displays price details in text."""
 	
 	_day = [ 6, 22 ]
 	_night = [ 22, 6 ]
+	_missing = '-'
 	
 	def __init__( self, pos, size, options, parent=None ):
 		start, end = options['day']
 		
 		# normalize the start and end of the night
 		start = self._Normalize( start )
 		end = self._Normalize( end )
 		self._day = [ start, end ]
 		self._night = [ end, start ]
+		self._missing = options['missing']
 		
 		_PriceDisplayWindow.__init__(self, size, pos, options, parent)
 	
 	def _AddDetail( self, name, price, linebreak=True, textStyle=None ):
 		"""Adds a detail with a name and price, formatted for the display."""
 		
 		if price != None:
@@ -590,15 +700,15 @@
 			win.addstr( '\n' )
 	
 	def _AddMissingDetail( self, name, linebreak=True ):
 		"""Adds a detail when price is missing."""
 		
 		win = self._win
 		n = name.ljust( 10 )
-		p = '-'.rjust( 6 )
+		p = self._missing.rjust( 6 )
 		
 		win.addstr( n )
 		win.addstr( p, curses.A_BOLD )
 		
 		if linebreak:
 			win.addstr( '\n' )
```

### Comparing `pricedisplay-0.5.2/pyproject.toml` & `pricedisplay-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pricedisplay"
-version = "0.5.2"
+version = "0.6.0"
 authors = ["Lumi"]
 description = "Terminal display for the Finnish power price."
 readme = "README.md"
 license = "LICENSE.md"
 repository = "https://github.com/YukiNeko-hime/pricedisplay"
 classifiers = [
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `pricedisplay-0.5.2/PKG-INFO` & `pricedisplay-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pricedisplay
-Version: 0.5.2
+Version: 0.6.0
 Summary: Terminal display for the Finnish power price.
 Home-page: https://github.com/YukiNeko-hime/pricedisplay
 License: LICENSE.md
 Author: Lumi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: Other/Proprietary License
```

