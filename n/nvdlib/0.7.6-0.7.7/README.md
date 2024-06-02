# Comparing `tmp/nvdlib-0.7.6-py3-none-any.whl.zip` & `tmp/nvdlib-0.7.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 14059 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat       84 b- defN 23-Nov-09 16:48 nvdlib/__init__.py
--rw-rw-rw-  2.0 fat    12345 b- defN 23-Nov-09 16:48 nvdlib/classes.py
--rw-rw-rw-  2.0 fat     9270 b- defN 23-Nov-09 16:48 nvdlib/cpe.py
--rw-rw-rw-  2.0 fat    23699 b- defN 23-Nov-09 16:48 nvdlib/cve.py
--rw-rw-rw-  2.0 fat     5983 b- defN 23-Nov-09 16:48 nvdlib/get.py
--rw-rw-rw-  2.0 fat     1077 b- defN 23-Nov-09 17:01 nvdlib-0.7.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3029 b- defN 23-Nov-09 17:01 nvdlib-0.7.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Nov-09 17:01 nvdlib-0.7.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Nov-09 17:01 nvdlib-0.7.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      739 b- defN 23-Nov-09 17:01 nvdlib-0.7.6.dist-info/RECORD
-10 files, 56325 bytes uncompressed, 12821 bytes compressed:  77.2%
+Zip file size: 14511 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Jun-02 14:46 nvdlib/__init__.py
+-rw-rw-rw-  2.0 fat    13305 b- defN 24-Jun-02 15:05 nvdlib/classes.py
+-rw-rw-rw-  2.0 fat    14057 b- defN 24-Jun-02 15:56 nvdlib/cpe.py
+-rw-rw-rw-  2.0 fat    23699 b- defN 24-Jun-02 14:23 nvdlib/cve.py
+-rw-rw-rw-  2.0 fat     6187 b- defN 24-Jun-02 14:47 nvdlib/get.py
+-rw-rw-rw-  2.0 fat     1077 b- defN 24-Jun-02 16:07 nvdlib-0.7.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3029 b- defN 24-Jun-02 16:07 nvdlib-0.7.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Jun-02 16:07 nvdlib-0.7.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-Jun-02 16:07 nvdlib-0.7.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      741 b- defN 24-Jun-02 16:07 nvdlib-0.7.7.dist-info/RECORD
+10 files, 62294 bytes uncompressed, 13273 bytes compressed:  78.7%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: nvdlib/cve.py
 Comment: 
 
 Filename: nvdlib/get.py
 Comment: 
 
-Filename: nvdlib-0.7.6.dist-info/LICENSE
+Filename: nvdlib-0.7.7.dist-info/LICENSE
 Comment: 
 
-Filename: nvdlib-0.7.6.dist-info/METADATA
+Filename: nvdlib-0.7.7.dist-info/METADATA
 Comment: 
 
-Filename: nvdlib-0.7.6.dist-info/WHEEL
+Filename: nvdlib-0.7.7.dist-info/WHEEL
 Comment: 
 
-Filename: nvdlib-0.7.6.dist-info/top_level.txt
+Filename: nvdlib-0.7.7.dist-info/top_level.txt
 Comment: 
 
-Filename: nvdlib-0.7.6.dist-info/RECORD
+Filename: nvdlib-0.7.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nvdlib/__init__.py

```diff
@@ -1,2 +1,2 @@
 from .cve import searchCVE, searchCVE_V2
-from .cpe import searchCPE, searchCPE_V2
+from .cpe import searchCPE, searchCPE_V2, searchCPEmatch
```

## nvdlib/classes.py

```diff
@@ -38,14 +38,52 @@
         return len(vars(self))
 
     def __iter__(self):
         yield 5
         yield from list(self.__dict__.keys())
 
 
+class MatchString:
+    """JSON dump class for CPE match strings
+
+    :var matchCriteriaId: UUID match criteria
+    :vartype matchCriteriaId: str
+
+    :var criteria: CPE name
+    :vartype criteria: str
+
+    :var lastModifiedDate: Match string modification date
+    :vartype lastModifiedDate: str
+
+    :var cpeLastModified: CPE modification date
+    :vartype cpeLastModified: str 
+
+    :var created: CPE creation date
+    :vartype created: str
+
+    :var status: CPE active status
+    :vartype status: str
+    
+    :var matches: CPE Names and IDs within the CPE Dictionary that matches the CPE Match Criteria
+    :vartype matches: list
+    """
+
+    def __init__(self, response):
+        vars(self).update(response)
+
+    def __repr__(self):
+        return str(self.__dict__)
+
+    def __len__(self):
+        return len(vars(self))
+
+    def __iter__(self):
+        yield 5
+        yield from list(self.__dict__.keys())
+
 class CVE:
     """JSON dump class for CVEs
         For more information the values returned from a CVE, please visit https://nvd.nist.gov/developers/vulnerabilities
     
     :var id: CVE ID
     :vartype id: str
 
@@ -209,15 +247,15 @@
     def getvars(self):
         try:
             self.cpe = self.configurations[0].nodes[0].cpeMatch
         except AttributeError:
             pass
         
         try:
-            self.cwe = [x.description[0] for x in self.weaknesses]
+            self.cwe = [x for w in self.weaknesses for x in w.description]
         except AttributeError:
             pass
 
         try:
             self.url = 'https://nvd.nist.gov/vuln/detail/' + self.id
         except:
             pass
```

## nvdlib/cpe.py

```diff
@@ -226,7 +226,131 @@
     if delay and key:
         if delay < 0.6:
             raise SyntaxError('Delay parameter must be greater than 0.6 seconds with an API key. NVD API recommends several seconds.')
     elif delay and not key:
         raise SyntaxError('Key parameter must be present to define a delay. Requests are delayed 6 seconds without an API key by default.')
 
     return parameters, headers
+
+def __buildCPEMatchCall(
+    cveId,
+    lastModStartDate,
+    lastModEndDate,
+    matchCriteriaId,
+    matchStringSearch,
+    limit,
+    key,
+    delay):
+
+    parameters = {}
+
+    if cveId:
+        parameters['cveId'] = cveId
+    
+    if lastModStartDate:
+        if isinstance(lastModStartDate, datetime):
+            date = lastModStartDate.isoformat()
+        elif isinstance(lastModStartDate, str):
+            date = datetime.strptime(lastModStartDate, '%Y-%m-%d %H:%M').isoformat()
+        else:
+            raise SyntaxError('Invalid date syntax: ' + lastModStartDate)
+        parameters['lastModStartDate'] = date.replace('+', '%2B')
+
+    if lastModEndDate:
+        if isinstance(lastModEndDate, datetime):
+            date = lastModEndDate.isoformat()
+        elif isinstance(lastModEndDate, str):
+            date = datetime.strptime(lastModEndDate, '%Y-%m-%d %H:%M').isoformat()
+        else:
+            raise SyntaxError('Invalid date syntax: ' + lastModEndDate)
+        parameters['lastModEndDate'] = date.replace('+', '%2B')
+
+    if matchCriteriaId:
+        parameters['matchCriteriaId'] = matchCriteriaId
+
+    if matchStringSearch:
+        parameters['matchStringSearch'] = matchStringSearch
+
+    if limit:
+        if limit > 2000 or limit < 1:
+            raise SyntaxError('Limit parameter must be between 1 and 2000')
+        parameters['resultsPerPage'] = limit
+
+    if key:
+        headers = {'content-type': 'application/json', 'apiKey': key}
+    else:
+        headers = {'content-type': 'application/json'}
+
+    if delay and key:
+        if delay < 0.6:
+            raise SyntaxError('Delay parameter must be greater than 0.6 seconds with an API key. NVD API recommends several seconds.')
+    elif delay and not key:
+        raise SyntaxError('Key parameter must be present to define a delay. Requests are delayed 6 seconds without an API key by default.')
+
+    return parameters, headers
+
+def searchCPEmatch(
+        cveId: str = None,
+        lastModStartDate: Tuple[str, datetime] = None,
+        lastModEndDate: Tuple[str, datetime] = None,
+        matchCriteriaId: str = None,
+        matchStringSearch: str = None,
+        limit: int = None,
+        key: str = None,
+        delay: int = None,
+        verbose: bool = None) -> list:
+    """Build and send GET request then return list of objects containing a collection of CPEs.
+    
+    :param cveId: Returns all matching CPE match strings for a CVE.
+    :type cveId: str
+
+    :param lastModStartDate: Match string last modification start date or CPE last modified start date. Maximum 120 day range. A start and end date is required. All times are in UTC 00:00.
+
+        A datetime object or string can be passed as a date. NVDLib will automatically parse the datetime object into the correct format.
+
+        String Example: '2020-06-28 00:00'
+    :type lastModStartDate: str/datetime obj
+
+    :param lastModEndDate: CPE last modification end date. Maximum 120 day range. Must be included with lastModStartDate.
+        Example: '2020-06-28 00:00'
+    :type lastModEndDate: str/datetime obj
+
+    :param matchCriteriaId: Returns CPE records associated with a match string by its UUID. Requires a properly formatted UUID.
+    :type matchCriteriaId: str
+
+    :param matchStringSearch: Returns CPE records that match the provided CPE match string. See the NVD API documentation website for more details on how to use CPE match strings. https://nvd.nist.gov/developers/products
+    :type matchStringSearch: str
+
+    :param limit: Limits the number of results of the search.
+    :type limit: int
+
+    :param key: NVD API Key. Allows for a request every 0.6 seconds instead of 6 seconds.
+    :type key: str
+
+    :param delay: Can only be used if an API key is provided. The amount of time to sleep in between requests. Must be a value above 0.6 seconds if an API key is present. `delay` is set to 6 seconds if no API key is passed.
+    :type verbose: bool   
+
+    :param verbose: Prints the URL request for debugging purposes.
+    :type verbose: bool
+    """
+
+
+
+    # Build the URL for the request
+    parameters, headers = __buildCPEMatchCall(
+        cveId,
+        lastModStartDate,
+        lastModEndDate,
+        matchCriteriaId,
+        matchStringSearch,
+        limit,
+        key,
+        delay)
+
+    # Send the GET request for the JSON and convert to dictionary
+    raw = __get('cpeMatch', headers, parameters, limit, verbose, delay)
+    cpes = []
+    # Generates the CVEs into objects for easy referencing and appends them to self.cves
+    for eachCPE in raw['matchStrings']:
+        cpe = __convert('MatchString', eachCPE['matchString'])
+        cpes.append(cpe)
+    return cpes
```

## nvdlib/get.py

```diff
@@ -8,14 +8,16 @@
     """Calculate required pages for multiple requests, send the GET request with the search criteria, return list of CVEs or CPEs objects."""
 
     # Get the default 2000 items to see the totalResults and determine pages required.
     if product == 'cve':
         link = 'https://services.nvd.nist.gov/rest/json/cves/2.0?'
     elif product == 'cpe':
         link = 'https://services.nvd.nist.gov/rest/json/cpes/2.0?'
+    elif product == 'cpeMatch':
+        link = 'https://services.nvd.nist.gov/rest/json/cpematch/2.0?'
 
     # Requests doesn't really work with dictionary parameters that have no value like `isVulnerable`. The workaround is to just pass a string instead.
     # This joins the parameters into a string with '&' and if a key contains a value then it will join the values with '='
     stringParams = '&'.join(
         [k if v is None else f"{k}={v}" for k, v in parameters.items()])
     if verbose:
         print('Filter:\n' + link + stringParams)
@@ -82,15 +84,16 @@
 def __get_with_generator(product, headers, parameters, limit,
                          verbose, delay):
     # Get the default 2000 items to see the totalResults and determine pages required.
     if product == 'cve':
         link = 'https://services.nvd.nist.gov/rest/json/cves/2.0?'
     elif product == 'cpe':
         link = 'https://services.nvd.nist.gov/rest/json/cpes/2.0?'
-
+    elif product == 'cpeMatch':
+        link = 'https://services.nvd.nist.gov/rest/json/cpes/2.0?'
     startIndex = 0
     while True:
         stringParams = '&'.join(
             [k if v is None else f"{k}={v}" for k, v in parameters.items()])
         if verbose:
             print('Filter:\n' + link + stringParams)
         rate_delay = 1
```

## Comparing `nvdlib-0.7.6.dist-info/LICENSE` & `nvdlib-0.7.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nvdlib-0.7.6.dist-info/METADATA` & `nvdlib-0.7.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvdlib
-Version: 0.7.6
+Version: 0.7.7
 Summary: National Vulnerability Database CPE/CVE API Library for Python
 Home-page: https://github.com/Vehemont/nvdlib/
 Author: Vehemont
 Author-email: brad@nvdlib.com
 License: MIT
 Requires-Python: >3.7.9
 Description-Content-Type: text/markdown
```

