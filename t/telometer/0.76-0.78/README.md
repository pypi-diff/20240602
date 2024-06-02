# Comparing `tmp/telometer-0.76.tar.gz` & `tmp/telometer-0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telometer-0.76.tar", last modified: Fri May 24 05:24:10 2024, max compression
+gzip compressed data, was "telometer-0.78.tar", last modified: Sun Jun  2 07:26:52 2024, max compression
```

## Comparing `telometer-0.76.tar` & `telometer-0.78.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2024-05-24 05:24:10.780628 telometer-0.76/
--rw-r--r--   0 santiago   (501) staff       (20)     1074 2024-05-22 15:01:09.000000 telometer-0.76/LICENSE.txt
--rw-r--r--   0 santiago   (501) staff       (20)      613 2024-05-24 05:24:10.775558 telometer-0.76/PKG-INFO
--rw-r--r--   0 santiago   (501) staff       (20)      148 2024-05-22 15:03:15.000000 telometer-0.76/README.md
--rw-r--r--   0 santiago   (501) staff       (20)       38 2024-05-24 05:24:10.780696 telometer-0.76/setup.cfg
--rw-r--r--   0 santiago   (501) staff       (20)      826 2024-05-24 05:23:49.000000 telometer-0.76/setup.py
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2024-05-24 05:24:10.756821 telometer-0.76/telometer/
--rw-r--r--   0 santiago   (501) staff       (20)       91 2023-12-02 23:50:44.000000 telometer-0.76/telometer/__init__.py
--rw-r--r--   0 santiago   (501) staff       (20)     6969 2024-05-24 05:23:57.000000 telometer-0.76/telometer/telometer.py
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2024-05-24 05:24:10.771441 telometer-0.76/telometer.egg-info/
--rw-r--r--   0 santiago   (501) staff       (20)      613 2024-05-24 05:24:10.000000 telometer-0.76/telometer.egg-info/PKG-INFO
--rw-r--r--   0 santiago   (501) staff       (20)      243 2024-05-24 05:24:10.000000 telometer-0.76/telometer.egg-info/SOURCES.txt
--rw-r--r--   0 santiago   (501) staff       (20)        1 2024-05-24 05:24:10.000000 telometer-0.76/telometer.egg-info/dependency_links.txt
--rw-r--r--   0 santiago   (501) staff       (20)       66 2024-05-24 05:24:10.000000 telometer-0.76/telometer.egg-info/entry_points.txt
--rw-r--r--   0 santiago   (501) staff       (20)       10 2024-05-24 05:24:10.000000 telometer-0.76/telometer.egg-info/top_level.txt
+drwxr-xr-x   0 santiago   (501) staff       (20)        0 2024-06-02 07:26:52.224284 telometer-0.78/
+-rw-r--r--   0 santiago   (501) staff       (20)     1074 2024-05-22 15:01:09.000000 telometer-0.78/LICENSE.txt
+-rw-r--r--   0 santiago   (501) staff       (20)      613 2024-06-02 07:26:52.223738 telometer-0.78/PKG-INFO
+-rw-r--r--   0 santiago   (501) staff       (20)      148 2024-05-22 15:03:15.000000 telometer-0.78/README.md
+-rw-r--r--   0 santiago   (501) staff       (20)       38 2024-06-02 07:26:52.224352 telometer-0.78/setup.cfg
+-rw-r--r--   0 santiago   (501) staff       (20)      826 2024-06-02 07:26:40.000000 telometer-0.78/setup.py
+drwxr-xr-x   0 santiago   (501) staff       (20)        0 2024-06-02 07:26:52.211165 telometer-0.78/telometer/
+-rw-r--r--   0 santiago   (501) staff       (20)       91 2023-12-02 23:50:44.000000 telometer-0.78/telometer/__init__.py
+-rw-r--r--   0 santiago   (501) staff       (20)     7890 2024-06-02 07:26:14.000000 telometer-0.78/telometer/telometer.py
+drwxr-xr-x   0 santiago   (501) staff       (20)        0 2024-06-02 07:26:52.223299 telometer-0.78/telometer.egg-info/
+-rw-r--r--   0 santiago   (501) staff       (20)      613 2024-06-02 07:26:52.000000 telometer-0.78/telometer.egg-info/PKG-INFO
+-rw-r--r--   0 santiago   (501) staff       (20)      243 2024-06-02 07:26:52.000000 telometer-0.78/telometer.egg-info/SOURCES.txt
+-rw-r--r--   0 santiago   (501) staff       (20)        1 2024-06-02 07:26:52.000000 telometer-0.78/telometer.egg-info/dependency_links.txt
+-rw-r--r--   0 santiago   (501) staff       (20)       66 2024-06-02 07:26:52.000000 telometer-0.78/telometer.egg-info/entry_points.txt
+-rw-r--r--   0 santiago   (501) staff       (20)       10 2024-06-02 07:26:52.000000 telometer-0.78/telometer.egg-info/top_level.txt
```

### Comparing `telometer-0.76/LICENSE.txt` & `telometer-0.78/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `telometer-0.76/PKG-INFO` & `telometer-0.78/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telometer
-Version: 0.76
+Version: 0.78
 Summary: a simple regular expression based method for measuring individual, chromosome-specific telomere lengths from long-read sequencing data
 Author: Santiago E Sanchez
 Author-email: ses94@stanford.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `telometer-0.76/setup.py` & `telometer-0.78/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="telometer",
-    version="0.76",
+    version="0.78",
     author="Santiago E Sanchez",
     author_email="ses94@stanford.edu",
     description="a simple regular expression based method for measuring individual, chromosome-specific telomere lengths from long-read sequencing data",
     packages=setuptools.find_packages(),
     license='MIT',
     long_description=open('README.md').read(),
     classifiers=[
```

### Comparing `telometer-0.76/telometer/telometer.py` & `telometer-0.78/telometer/telometer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python3
-# Telometer v0.76
-# Created by: Santiago E Sanchez
-# Artandi Lab, Stanford University, 2023
+# Telometer v0.78
+# Created by: Santiago E Sanche8
+# Artandi Lab, Stanford University, 2024
 # Measures telomeres from ONT or PacBio long reads aligned to a T2T genome assembly
-# Simple Usage: telometer -b sorted_t2t.bam -o output.tsv
-
+# Simple Usage: telometer -b sorted_t2t.bam -o output.ts8
 import pysam
 import re
-import regex
+import regex as re
 import csv
 import argparse
 from multiprocessing import Pool, cpu_count
 
 def reverse_complement(seq):
     """Returns the reverse complement of a DNA sequence."""
     complement = {'A': 'T', 'C': 'G', 'G': 'C', 'T': 'A', 'N': 'N'}
@@ -23,115 +22,127 @@
         adapters = ['TTTTTTTTCCTGTACTTCGTTCAGTTACGTATTGCT', 'GCAATACGTAACTGAACGAAGTACAGG']
     else:
         adapters = ['TTTTTTTTTTTAATGTACTTCGTTCAGTTACGTATTGCT', 'GCAATACGTAACTGAACGAAGT']
 
     adapters_rc = [reverse_complement(adapter) for adapter in adapters]
     return adapters + adapters_rc
 
-def get_telomere_repeats():
-    """Returns the telomere repeat sequences."""
-    telomere_repeats = ['GGCCA', 'CCCTAA', 'TTAGGG', 'CCCTGG', 'CTTCTT', 'TTAAAA', 'CCTGG']
-    telomere_repeats_rc = [reverse_complement(repeat) for repeat in telomere_repeats]
-    return telomere_repeats + telomere_repeats_rc
+def get_flexible_telomere_patterns():
+    """Returns flexible telomere repeat patterns for both G-rich and C-rich strands."""
+    g_rich_telomere_pattern = r'(T{1,2}T{1,2}A{1,2}G{1,2}G{1,2}G{1,2}){2,}'
+    c_rich_telomere_pattern = r'(C{1,2}C{1,2}C{1,2}T{1,2}A{1,2}A{1,2}){2,}'
+    return g_rich_telomere_pattern, c_rich_telomere_pattern
 
 def find_initial_boundary_region(sequence, patterns, max_mismatches):
     """Finds the initial boundary region with allowed mismatches."""
     boundary_length = 0
     combined_pattern = '|'.join(f'({pattern})' for pattern in patterns)
     regex_pattern = f'({combined_pattern}){{2,}}'
 
-    for match in regex.finditer(f'({regex_pattern}){{e<={max_mismatches}}}', sequence, regex.BESTMATCH):
+    for match in re.finditer(f'({regex_pattern}){{e<={max_mismatches}}}', sequence, re.BESTMATCH):
         boundary_length = max(boundary_length, len(match.group(0)))
     return boundary_length
 
+def determine_arm(reference_name, alignment_start, reference_length):
+    """Determine the chromosome arm based on the alignment start position and reference name."""
+    if alignment_start < 15000 and "q" not in reference_name:
+        return "p"
+    return "q"
+
 def process_read(args):
-    read_data, telomere_repeats_re, adapters, minreadlen = args
+    read_data, g_rich_telomere_pattern, c_rich_telomere_pattern, adapters, minreadlen = args
 
     if read_data['is_unmapped'] or read_data['query_sequence'] is None or len(read_data['query_sequence']) < minreadlen:
+        print(f"Skipping read {read_data['read_id']}: unmapped or too short")
         return None
 
     alignment_start = read_data['reference_start']
     alignment_end = read_data['reference_end']
-    seq = read_data['query_sequence']
+    seq_to_check = read_data['query_sequence']
 
     if read_data['is_reverse']:
         direction = "rev"
-        seq = reverse_complement(seq)
+        seq_to_check = reverse_complement(seq_to_check)
     else:
         direction = "fwd"
 
     reference_genome_length = read_data['reference_length']
-
     if alignment_start >= 15000 and alignment_start <= reference_genome_length - 30000:
+        print(f"Skipping read {read_data['read_id']}: alignment start {alignment_start} within filtered range")
         return None
 
-    if alignment_start < 15000 and "q" not in read_data['reference_name']:
-        arm = "p"
-    else:
-        arm = "q"
+    arm = determine_arm(read_data['reference_name'], alignment_start, reference_genome_length)
 
-    telomere_start = [m.start() for m in re.finditer(telomere_repeats_re, seq)]
-    if telomere_start:
-        telomere_start = telomere_start[0]
-        if telomere_start > 100 and (len(seq) - telomere_start > 200):
-            return None
-
-        telomere_end = min((seq.find(adapter) for adapter in adapters), default=-1)
-        if telomere_end == -1:
-            telomere_end = len(seq)
+    telomere_starts = [m.start() for m in re.finditer(g_rich_telomere_pattern, seq_to_check)]
+    if not telomere_starts:
+        telomere_starts = [m.start() for m in re.finditer(c_rich_telomere_pattern, seq_to_check)]
+
+    if telomere_starts:
+        telomere_start = telomere_starts[0]
+
+        # Find the end of the telomere region
+        telomere_end = min((pos for pos in (seq_to_check.find(adapter) for adapter in adapters) if pos != -1), default=len(seq_to_check))
+
+        telomere_region = seq_to_check[telomere_start:telomere_end]
+        telomere_repeat = [m.group() for m in re.finditer(g_rich_telomere_pattern, telomere_region)]
+        if not telomere_repeat:
+            telomere_repeat = [m.group() for m in re.finditer(c_rich_telomere_pattern, telomere_region)]
 
-        telomere_region = seq[telomere_start:telomere_end]
-        telomere_repeat = [m.group() for m in re.finditer('|'.join(telomere_repeats_re.split('|')), telomere_region)]
         telomere_length = len(''.join(telomere_repeat))
 
-        boundary_mm1_length = find_initial_boundary_region(telomere_region, telomere_repeats_re.split('|'), max_mismatches=1)
-
-        return {
-            'chromosome': read_data['reference_name'],
-            'reference_start': alignment_start,
-            'reference_end': alignment_end,
-            'telomere_length': telomere_length,
-            'subtel_boundary_length': boundary_mm1_length,
-            'read_id': read_data['query_name'],
-            'mapping_quality': read_data['mapping_quality'],
-            'read_length': len(seq),
-            'arm': arm,
-            'direction': direction
-        }
-    return None
+        # Find the region immediately adjacent to the telomere region
+        boundary_mm1_region = seq_to_check[telomere_end:]
+        boundary_mm1_length = find_initial_boundary_region(boundary_mm1_region, g_rich_telomere_pattern.split('|') + c_rich_telomere_pattern.split('|'), max_mismatches=2)
+    else:
+        telomere_start = None
+        telomere_end = None
+        telomere_length = 0
+        boundary_mm1_length = 0
+
+    result = {
+        'read_id': read_data['read_id'],
+        'telomere_start': telomere_start,
+        'telomere_end': telomere_end,
+        'telomere_length': telomere_length,
+        'boundary_mm1_length': boundary_mm1_length,
+        'chromosome': read_data['reference_name'],
+        'mapping_quality': read_data['mapping_quality'],
+        'direction': direction,
+        'arm': arm
+    }
+    return result
 
 def calculate_telomere_length():
     parser = argparse.ArgumentParser(description='Calculate telomere length from a BAM file.')
     parser.add_argument('-b', '--bam', help='The path to the sorted BAM file.', required=True)
     parser.add_argument('-o', '--output', help='The path to the output file.', required=True)
     parser.add_argument('-c', '--chemistry', default="r10", help="Sequencing chemistry (r9 or r10, default=r10). Optional", required=False)
     parser.add_argument('-m', '--minreadlen', default=1000, type=int, help='Minimum read length to consider (Default: 1000 for telomere capture, use 4000 for WGS). Optional', required=False)
     args = parser.parse_args()
-    bam_file = pysam.AlignmentFile(args.bam, "rb")
 
     adapters = get_adapters(args.chemistry)
-    telomere_repeats = get_telomere_repeats()
-    telomere_repeats_re = "|".join(f'({repeat}){{2,}}' for repeat in telomere_repeats)
+    g_rich_telomere_pattern, c_rich_telomere_pattern = get_flexible_telomere_patterns()
 
+    bam_file = pysam.AlignmentFile(args.bam, "rb")
     read_data_list = [{
-        'query_name': read.query_name,
+        'read_id': read.query_name,
         'is_unmapped': read.is_unmapped,
-        'is_reverse': read.is_reverse,
         'reference_start': read.reference_start,
         'reference_end': read.reference_end,
         'reference_name': read.reference_name,
         'mapping_quality': read.mapping_quality,
         'query_sequence': read.query_sequence,
-        'reference_length': bam_file.get_reference_length(read.reference_name) if read.reference_name is not None else None
+        'reference_length': bam_file.get_reference_length(read.reference_name) if read.reference_name is not None else None,
+        'is_reverse': read.is_reverse
     } for read in bam_file if read.reference_name is not None and read.reference_name != 'chrM']
 
     with Pool(processes=cpu_count()) as pool:
         results = pool.map(
             process_read,
-            [(read_data, telomere_repeats_re, adapters, args.minreadlen) for read_data in read_data_list]
+            [(read_data, g_rich_telomere_pattern, c_rich_telomere_pattern, adapters, args.minreadlen) for read_data in read_data_list]
         )
 
     results = [result for result in results if result]
 
     # Ensure only the best result per read_id is saved
     best_results = {}
     for result in results:
```

### Comparing `telometer-0.76/telometer.egg-info/PKG-INFO` & `telometer-0.78/telometer.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telometer
-Version: 0.76
+Version: 0.78
 Summary: a simple regular expression based method for measuring individual, chromosome-specific telomere lengths from long-read sequencing data
 Author: Santiago E Sanchez
 Author-email: ses94@stanford.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

