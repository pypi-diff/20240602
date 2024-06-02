# Comparing `tmp/DendroPy-5.0.0.tar.gz` & `tmp/DendroPy-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DendroPy-5.0.0.tar", last modified: Wed May 22 12:51:06 2024, max compression
+gzip compressed data, was "DendroPy-5.0.1.tar", last modified: Sun Jun  2 07:40:10 2024, max compression
```

## Comparing `DendroPy-5.0.0.tar` & `DendroPy-5.0.1.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:51:06.784423 DendroPy-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-22 12:50:52.000000 DendroPy-5.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-05-22 12:50:52.000000 DendroPy-5.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-22 12:50:52.000000 DendroPy-5.0.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-22 12:50:52.000000 DendroPy-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-22 12:51:06.784423 DendroPy-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-22 12:50:52.000000 DendroPy-5.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 12:51:06.784423 DendroPy-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-22 12:50:52.000000 DendroPy-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:51:06.760424 DendroPy-5.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:51:06.764423 DendroPy-5.0.0/src/DendroPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-22 12:51:06.000000 DendroPy-5.0.0/src/DendroPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-22 12:51:06.000000 DendroPy-5.0.0/src/DendroPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:51:06.000000 DendroPy-5.0.0/src/DendroPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-22 12:51:06.000000 DendroPy-5.0.0/src/DendroPy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 12:51:06.000000 DendroPy-5.0.0/src/DendroPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 12:51:06.000000 DendroPy-5.0.0/src/DendroPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:51:06.000000 DendroPy-5.0.0/src/DendroPy.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:51:06.764423 DendroPy-5.0.0/src/dendropy/
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:51:06.764423 DendroPy-5.0.0/src/dendropy/application/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/application/dendropy_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/application/sumlabels.py
--rw-r--r--   0 runner    (1001) docker     (127)   103568 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/application/sumtrees.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:51:06.768423 DendroPy-5.0.0/src/dendropy/calculate/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/calculate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/calculate/combinatorics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/calculate/mathfn.py
--rw-r--r--   0 runner    (1001) docker     (127)    67545 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/calculate/phylogeneticdistance.py
--rw-r--r--   0 runner    (1001) docker     (127)    17039 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/calculate/popgenstat.py
--rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/calculate/probability.py
--rw-r--r--   0 runner    (1001) docker     (127)    14503 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/calculate/profiledistance.py
--rw-r--r--   0 runner    (1001) docker     (127)    16198 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/calculate/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    36698 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/calculate/treecompare.py
--rw-r--r--   0 runner    (1001) docker     (127)     9032 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/calculate/treemeasure.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/calculate/treescore.py
--rw-r--r--   0 runner    (1001) docker     (127)    19112 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/calculate/treesum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:51:06.768423 DendroPy-5.0.0/src/dendropy/dataio/
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/fastareader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/fastawriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    23229 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/ioservice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/multiphylipreader.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/newick.py
--rw-r--r--   0 runner    (1001) docker     (127)    35733 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/newickreader.py
--rw-r--r--   0 runner    (1001) docker     (127)    20902 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/newickwriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/newickyielder.py
--rw-r--r--   0 runner    (1001) docker     (127)    42585 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/nexmlreader.py
--rw-r--r--   0 runner    (1001) docker     (127)    30083 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/nexmlwriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/nexmlyielder.py
--rw-r--r--   0 runner    (1001) docker     (127)    20764 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/nexusprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    73158 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/nexusreader.py
--rw-r--r--   0 runner    (1001) docker     (127)    27424 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/nexuswriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/nexusyielder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14997 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/phylipreader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/phylipwriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/dataio/xmlprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:51:06.772423 DendroPy-5.0.0/src/dendropy/datamodel/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61706 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/datamodel/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    83288 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/datamodel/charmatrixmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    56921 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/datamodel/charstatemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    27922 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/datamodel/datasetmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    85537 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/datamodel/taxonmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)   127778 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/datamodel/treecollectionmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:51:06.772423 DendroPy-5.0.0/src/dendropy/datamodel/treemodel/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/datamodel/treemodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27197 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/datamodel/treemodel/_bipartition.py
--rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/datamodel/treemodel/_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)    62067 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/datamodel/treemodel/_node.py
--rw-r--r--   0 runner    (1001) docker     (127)   185176 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/datamodel/treemodel/_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:51:06.776423 DendroPy-5.0.0/src/dendropy/interop/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/interop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/interop/ape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/interop/biopython.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/interop/entrez.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/interop/ete.py
--rw-r--r--   0 runner    (1001) docker     (127)    15710 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/interop/gbif.py
--rw-r--r--   0 runner    (1001) docker     (127)    37088 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/interop/genbank.py
--rw-r--r--   0 runner    (1001) docker     (127)    15298 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/interop/itol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/interop/muscle.py
--rw-r--r--   0 runner    (1001) docker     (127)    38779 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/interop/paup.py
--rw-r--r--   0 runner    (1001) docker     (127)    37258 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/interop/raxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/interop/rspr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/interop/rstats.py
--rw-r--r--   0 runner    (1001) docker     (127)    10213 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/interop/seqgen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:51:06.776423 DendroPy-5.0.0/src/dendropy/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/legacy/coalescent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/legacy/continuous.py
--rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/legacy/ncbi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/legacy/popgensim.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/legacy/popgenstat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/legacy/reconcile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/legacy/seqmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/legacy/seqsim.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/legacy/treecalc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/legacy/treemanip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/legacy/treesim.py
--rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/legacy/treesplit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/legacy/treesum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:51:06.776423 DendroPy-5.0.0/src/dendropy/mathlib/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/mathlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/mathlib/mathfn.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/mathlib/probability.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/mathlib/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:51:06.780423 DendroPy-5.0.0/src/dendropy/model/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    85501 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/model/birthdeath.py
--rw-r--r--   0 runner    (1001) docker     (127)    32132 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/model/coalescent.py
--rw-r--r--   0 runner    (1001) docker     (127)    22471 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/model/continuous.py
--rw-r--r--   0 runner    (1001) docker     (127)    22245 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/model/discrete.py
--rw-r--r--   0 runner    (1001) docker     (127)    15419 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/model/multispeciescoalescent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15843 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/model/parsimony.py
--rw-r--r--   0 runner    (1001) docker     (127)    48905 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/model/protractedspeciation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26379 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/model/reconcile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/model/treeshape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:51:06.780423 DendroPy-5.0.0/src/dendropy/simulate/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/simulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/simulate/charsim.py
--rw-r--r--   0 runner    (1001) docker     (127)    12076 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/simulate/popgensim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/simulate/treesim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:51:06.780423 DendroPy-5.0.0/src/dendropy/utility/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11376 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/bitprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    43628 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/filesys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:51:06.784423 DendroPy-5.0.0/src/dendropy/utility/libexec/
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/libexec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/messaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/metavar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/processio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/textprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/timeprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/urlio.py
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-05-22 12:50:52.000000 DendroPy-5.0.0/src/dendropy/utility/vcsinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:40:10.550091 DendroPy-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-06-02 07:39:59.000000 DendroPy-5.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-06-02 07:39:59.000000 DendroPy-5.0.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-06-02 07:39:59.000000 DendroPy-5.0.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-06-02 07:39:59.000000 DendroPy-5.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7180 2024-06-02 07:40:10.550091 DendroPy-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-06-02 07:39:59.000000 DendroPy-5.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-02 07:40:10.550091 DendroPy-5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-06-02 07:39:59.000000 DendroPy-5.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:40:10.530091 DendroPy-5.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:40:10.530091 DendroPy-5.0.1/src/DendroPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7180 2024-06-02 07:40:10.000000 DendroPy-5.0.1/src/DendroPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-06-02 07:40:10.000000 DendroPy-5.0.1/src/DendroPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 07:40:10.000000 DendroPy-5.0.1/src/DendroPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-06-02 07:40:10.000000 DendroPy-5.0.1/src/DendroPy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-02 07:40:10.000000 DendroPy-5.0.1/src/DendroPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 07:40:10.000000 DendroPy-5.0.1/src/DendroPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 07:40:10.000000 DendroPy-5.0.1/src/DendroPy.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:40:10.534091 DendroPy-5.0.1/src/dendropy/
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:40:10.534091 DendroPy-5.0.1/src/dendropy/application/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/application/dendropy_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/application/sumlabels.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103568 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/application/sumtrees.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:40:10.534091 DendroPy-5.0.1/src/dendropy/calculate/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/calculate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/calculate/combinatorics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/calculate/mathfn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67545 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/calculate/phylogeneticdistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17039 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/calculate/popgenstat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/calculate/probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14503 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/calculate/profiledistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16198 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/calculate/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36698 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/calculate/treecompare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9032 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/calculate/treemeasure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/calculate/treescore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19112 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/calculate/treesum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:40:10.538091 DendroPy-5.0.1/src/dendropy/dataio/
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/fastareader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/fastawriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23229 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/ioservice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/multiphylipreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/newick.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35733 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/newickreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20965 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/newickwriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/newickyielder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42585 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/nexmlreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30083 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/nexmlwriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/nexmlyielder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20908 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/nexusprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73158 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/nexusreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27424 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/nexuswriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/nexusyielder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14997 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/phylipreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/phylipwriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/dataio/xmlprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:40:10.538091 DendroPy-5.0.1/src/dendropy/datamodel/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61706 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/datamodel/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83288 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/datamodel/charmatrixmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56921 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/datamodel/charstatemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27922 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/datamodel/datasetmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85537 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/datamodel/taxonmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127778 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/datamodel/treecollectionmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:40:10.538091 DendroPy-5.0.1/src/dendropy/datamodel/treemodel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/datamodel/treemodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27197 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/datamodel/treemodel/_bipartition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/datamodel/treemodel/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62067 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/datamodel/treemodel/_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)   185176 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/datamodel/treemodel/_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:40:10.542091 DendroPy-5.0.1/src/dendropy/interop/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/interop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/interop/ape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/interop/biopython.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/interop/entrez.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/interop/ete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15710 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/interop/gbif.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37088 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/interop/genbank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15298 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/interop/itol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/interop/muscle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38779 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/interop/paup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37258 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/interop/raxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/interop/rspr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/interop/rstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10213 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/interop/seqgen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:40:10.546091 DendroPy-5.0.1/src/dendropy/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/legacy/coalescent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/legacy/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/legacy/ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/legacy/popgensim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/legacy/popgenstat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/legacy/reconcile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/legacy/seqmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/legacy/seqsim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/legacy/treecalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/legacy/treemanip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/legacy/treesim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/legacy/treesplit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/legacy/treesum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:40:10.546091 DendroPy-5.0.1/src/dendropy/mathlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/mathlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/mathlib/mathfn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/mathlib/probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/mathlib/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:40:10.546091 DendroPy-5.0.1/src/dendropy/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85501 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/model/birthdeath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32132 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/model/coalescent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22471 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/model/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22245 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/model/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15419 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/model/multispeciescoalescent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15843 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/model/parsimony.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48905 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/model/protractedspeciation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26379 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/model/reconcile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/model/treeshape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:40:10.546091 DendroPy-5.0.1/src/dendropy/simulate/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/simulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/simulate/charsim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12076 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/simulate/popgensim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/simulate/treesim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:40:10.550091 DendroPy-5.0.1/src/dendropy/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11376 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/bitprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43628 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/filesys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:40:10.550091 DendroPy-5.0.1/src/dendropy/utility/libexec/
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/libexec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/messaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/metavar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/processio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/textprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/timeprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/urlio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-06-02 07:39:59.000000 DendroPy-5.0.1/src/dendropy/utility/vcsinfo.py
```

### Comparing `DendroPy-5.0.0/CHANGES.rst` & `DendroPy-5.0.1/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/LICENSE.rst` & `DendroPy-5.0.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/PKG-INFO` & `DendroPy-5.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DendroPy
-Version: 5.0.0
+Version: 5.0.1
 Summary: A Python library for phylogenetics and phylogenetic computing: reading, writing, simulation, processing and manipulation of phylogenetic trees (phylogenies) and characters.
 Home-page: http://github.com/jeetsukumaran/DendroPy
 Author: Jeet Sukumaran, Mark T. Holder, and Matthew Andres Moreno
 Author-email: jeetsukumaran@gmail.com, mtholder@ku.edu, morenoma@umich.edu
 License: BSD
 Project-URL: Documentation, https://jeetsukumaran.github.io/DendroPy/
 Project-URL: Source, https://github.com/jeetsukumaran/DendroPy
@@ -86,17 +86,38 @@
             -   `Descriptions of data formats supported for reading/writing <https://jeetsukumaran.github.io/DendroPy/schemas/index.html>`_ .
         
         and more.
         
         Citing
         ======
         
-        If you use this library or any portion thereof in published work, please cite it as:
+        If you use any portion of DendroPy v5 in your research, please cite it as:
         
-              Sukumaran, J. and M. T. Holder. 2010. DendroPy: a Python library for phylogenetic computing. Bioinformatics 26: 1569-1571.
+              Moreno, M. A., Sukumaran, J., and M. T. Holder. 2024. DendroPy 5: a mature Python library for phylogenetic computing. arXiv preprint arXiv:2405.14120. https://doi.org/10.48550/arXiv.2405.14120
+        
+        For BibTex users:
+        
+        .. code-block:: bibtex
+        
+              @misc{dendropy5,
+                 title = {DendroPy 5: a mature Python library for phylogenetic computing},
+                 author = {Moreno,  Matthew Andres and Sukumaran,  Jeet and Holder,  Mark T.},
+                 year = {2024},
+                 keywords = {Populations and Evolution (q-bio.PE),  FOS: Biological sciences,  FOS: Biological sciences},
+                 publisher = {arXiv},
+                 doi = {10.48550/ARXIV.2405.14120},
+                 url = {https://arxiv.org/abs/2405.14120},
+                 copyright = {arXiv.org perpetual, non-exclusive license}
+              }
+        
+        Earlier DendroPy versions can be cited as:
+        
+              Sukumaran, J. and M. T. Holder. 2010. DendroPy: a Python library for phylogenetic computing. Bioinformatics 26: 1569-1571. https://doi.org/10.1093/bioinformatics/btq228
+        
+        Consider also leaving a `star on GitHub <https://github.com/jeetsukumaran/DendroPy/stargazers>`_!
         
         License and Warranty
         ====================
         
         Please see the file "LICENSE.rst" for details.
         
         Developers
```

### Comparing `DendroPy-5.0.0/README.rst` & `DendroPy-5.0.1/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -81,17 +81,38 @@
     -   `Descriptions of data formats supported for reading/writing <https://jeetsukumaran.github.io/DendroPy/schemas/index.html>`_ .
 
 and more.
 
 Citing
 ======
 
-If you use this library or any portion thereof in published work, please cite it as:
+If you use any portion of DendroPy v5 in your research, please cite it as:
 
-      Sukumaran, J. and M. T. Holder. 2010. DendroPy: a Python library for phylogenetic computing. Bioinformatics 26: 1569-1571.
+      Moreno, M. A., Sukumaran, J., and M. T. Holder. 2024. DendroPy 5: a mature Python library for phylogenetic computing. arXiv preprint arXiv:2405.14120. https://doi.org/10.48550/arXiv.2405.14120
+
+For BibTex users:
+
+.. code-block:: bibtex
+
+      @misc{dendropy5,
+         title = {DendroPy 5: a mature Python library for phylogenetic computing},
+         author = {Moreno,  Matthew Andres and Sukumaran,  Jeet and Holder,  Mark T.},
+         year = {2024},
+         keywords = {Populations and Evolution (q-bio.PE),  FOS: Biological sciences,  FOS: Biological sciences},
+         publisher = {arXiv},
+         doi = {10.48550/ARXIV.2405.14120},
+         url = {https://arxiv.org/abs/2405.14120},
+         copyright = {arXiv.org perpetual, non-exclusive license}
+      }
+
+Earlier DendroPy versions can be cited as:
+
+      Sukumaran, J. and M. T. Holder. 2010. DendroPy: a Python library for phylogenetic computing. Bioinformatics 26: 1569-1571. https://doi.org/10.1093/bioinformatics/btq228
+
+Consider also leaving a `star on GitHub <https://github.com/jeetsukumaran/DendroPy/stargazers>`_!
 
 License and Warranty
 ====================
 
 Please see the file "LICENSE.rst" for details.
 
 Developers
```

### Comparing `DendroPy-5.0.0/setup.py` & `DendroPy-5.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/DendroPy.egg-info/PKG-INFO` & `DendroPy-5.0.1/src/DendroPy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DendroPy
-Version: 5.0.0
+Version: 5.0.1
 Summary: A Python library for phylogenetics and phylogenetic computing: reading, writing, simulation, processing and manipulation of phylogenetic trees (phylogenies) and characters.
 Home-page: http://github.com/jeetsukumaran/DendroPy
 Author: Jeet Sukumaran, Mark T. Holder, and Matthew Andres Moreno
 Author-email: jeetsukumaran@gmail.com, mtholder@ku.edu, morenoma@umich.edu
 License: BSD
 Project-URL: Documentation, https://jeetsukumaran.github.io/DendroPy/
 Project-URL: Source, https://github.com/jeetsukumaran/DendroPy
@@ -86,17 +86,38 @@
             -   `Descriptions of data formats supported for reading/writing <https://jeetsukumaran.github.io/DendroPy/schemas/index.html>`_ .
         
         and more.
         
         Citing
         ======
         
-        If you use this library or any portion thereof in published work, please cite it as:
+        If you use any portion of DendroPy v5 in your research, please cite it as:
         
-              Sukumaran, J. and M. T. Holder. 2010. DendroPy: a Python library for phylogenetic computing. Bioinformatics 26: 1569-1571.
+              Moreno, M. A., Sukumaran, J., and M. T. Holder. 2024. DendroPy 5: a mature Python library for phylogenetic computing. arXiv preprint arXiv:2405.14120. https://doi.org/10.48550/arXiv.2405.14120
+        
+        For BibTex users:
+        
+        .. code-block:: bibtex
+        
+              @misc{dendropy5,
+                 title = {DendroPy 5: a mature Python library for phylogenetic computing},
+                 author = {Moreno,  Matthew Andres and Sukumaran,  Jeet and Holder,  Mark T.},
+                 year = {2024},
+                 keywords = {Populations and Evolution (q-bio.PE),  FOS: Biological sciences,  FOS: Biological sciences},
+                 publisher = {arXiv},
+                 doi = {10.48550/ARXIV.2405.14120},
+                 url = {https://arxiv.org/abs/2405.14120},
+                 copyright = {arXiv.org perpetual, non-exclusive license}
+              }
+        
+        Earlier DendroPy versions can be cited as:
+        
+              Sukumaran, J. and M. T. Holder. 2010. DendroPy: a Python library for phylogenetic computing. Bioinformatics 26: 1569-1571. https://doi.org/10.1093/bioinformatics/btq228
+        
+        Consider also leaving a `star on GitHub <https://github.com/jeetsukumaran/DendroPy/stargazers>`_!
         
         License and Warranty
         ====================
         
         Please see the file "LICENSE.rst" for details.
         
         Developers
```

### Comparing `DendroPy-5.0.0/src/DendroPy.egg-info/SOURCES.txt` & `DendroPy-5.0.1/src/DendroPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/__init__.py` & `DendroPy-5.0.1/src/dendropy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,18 +101,18 @@
 from dendropy.legacy import treesplit
 from dendropy.legacy import treesum
 
 ###############################################################################
 ## PACKAGE METADATA
 import collections
 __project__ = "DendroPy"
-__version__ = "5.0.0"
-__author__ = "Jeet Sukumaran and Mark T. Holder"
+__version__ = "5.0.1"
+__author__ = "Jeet Sukumaran and Mark T. Holder and Matthew Andres Moreno"
 __copyright__ = "Copyright 2010-2022 Jeet Sukumaran and Mark T. Holder."
-__citation__ = "Sukumaran, J and MT Holder. 2010. DendroPy: a Python library for phylogenetic computing. Bioinformatics 26: 1569-1571."
+__citation__ = "Moreno, M. A., Sukumaran, J., and M. T. Holder. 2024. DendroPy 5: a mature Python library for phylogenetic computing. arXiv preprint arXiv:2405.14120. https://doi.org/10.48550/arXiv.2405.14120"
 PACKAGE_VERSION = __version__ # for backwards compatibility (with sate)
 
 def _get_revision_object():
     from dendropy.utility import vcsinfo
     __revision__ = vcsinfo.Revision(repo_path=homedir())
     return __revision__
```

### Comparing `DendroPy-5.0.0/src/dendropy/__main__.py` & `DendroPy-5.0.1/src/dendropy/__main__.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/application/dendropy_format.py` & `DendroPy-5.0.1/src/dendropy/application/dendropy_format.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/application/sumlabels.py` & `DendroPy-5.0.1/src/dendropy/application/sumlabels.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/application/sumtrees.py` & `DendroPy-5.0.1/src/dendropy/application/sumtrees.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/calculate/__init__.py` & `DendroPy-5.0.1/src/dendropy/calculate/__init__.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/calculate/combinatorics.py` & `DendroPy-5.0.1/src/dendropy/calculate/combinatorics.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/calculate/mathfn.py` & `DendroPy-5.0.1/src/dendropy/calculate/mathfn.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/calculate/phylogeneticdistance.py` & `DendroPy-5.0.1/src/dendropy/calculate/phylogeneticdistance.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/calculate/popgenstat.py` & `DendroPy-5.0.1/src/dendropy/calculate/popgenstat.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/calculate/probability.py` & `DendroPy-5.0.1/src/dendropy/calculate/probability.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/calculate/profiledistance.py` & `DendroPy-5.0.1/src/dendropy/calculate/profiledistance.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/calculate/statistics.py` & `DendroPy-5.0.1/src/dendropy/calculate/statistics.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/calculate/treecompare.py` & `DendroPy-5.0.1/src/dendropy/calculate/treecompare.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/calculate/treemeasure.py` & `DendroPy-5.0.1/src/dendropy/calculate/treemeasure.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/calculate/treescore.py` & `DendroPy-5.0.1/src/dendropy/calculate/treescore.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/calculate/treesum.py` & `DendroPy-5.0.1/src/dendropy/calculate/treesum.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/__init__.py` & `DendroPy-5.0.1/src/dendropy/dataio/__init__.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/fastareader.py` & `DendroPy-5.0.1/src/dendropy/dataio/fastareader.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/fastawriter.py` & `DendroPy-5.0.1/src/dendropy/dataio/fastawriter.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/ioservice.py` & `DendroPy-5.0.1/src/dendropy/dataio/ioservice.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/multiphylipreader.py` & `DendroPy-5.0.1/src/dendropy/dataio/multiphylipreader.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/newick.py` & `DendroPy-5.0.1/src/dendropy/dataio/newick.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/newickreader.py` & `DendroPy-5.0.1/src/dendropy/dataio/newickreader.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/newickwriter.py` & `DendroPy-5.0.1/src/dendropy/dataio/newickwriter.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,15 +374,16 @@
                 if len(tag_parts) > 0:
                     tag = self.node_label_element_separator.join(tag_parts)
                 else:
                     return ""
         if tag:
             tag = nexusprocessing.escape_nexus_token(tag,
                     preserve_spaces=self.preserve_spaces,
-                    quote_underscores=not self.unquoted_underscores)
+                    quote_underscores=not self.unquoted_underscores,
+                    protect_regex=r'''[()[\]{},;:'"\0\t\n]''')
             return tag
         else:
             return ""
 
     # def _compose_node(self, node):
     #     """
     #     Given a DendroPy Node, this returns the Node as a Newick
```

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/newickyielder.py` & `DendroPy-5.0.1/src/dendropy/dataio/newickyielder.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/nexmlreader.py` & `DendroPy-5.0.1/src/dendropy/dataio/nexmlreader.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/nexmlwriter.py` & `DendroPy-5.0.1/src/dendropy/dataio/nexmlwriter.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/nexmlyielder.py` & `DendroPy-5.0.1/src/dendropy/dataio/nexmlyielder.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/nexusprocessing.py` & `DendroPy-5.0.1/src/dendropy/dataio/nexusprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -466,26 +466,35 @@
     else:
         prefix = "[&"
         separator = ","
         suffix = "]"
     body = separator.join(parts)
     return prefix + body + suffix
 
-def escape_nexus_token(label, preserve_spaces=False, quote_underscores=True):
+def escape_nexus_token(
+    label,
+    preserve_spaces=False,
+    quote_underscores=True,
+    protect_regex=r'''[()[\]{}\\\/,;:=*'"`+\-<>\0\t\n]''',
+):
     """
     Properly protects a NEXUS token.
+
+    Kwarg protect_regex allows less eager quoting when working with non-Nexus
+    Newick strings.
     """
     if label is None:
         return ""
     if not preserve_spaces \
             and "_" not in label \
-            and not re.search(r'''[()[\]{}\\\/,;:=*'"`+\-<>\\0\\t\\n]''', label):
+            and not re.search(protect_regex, label):
         label = label.replace(' ', '_').replace('\t', '_')
-    elif re.search(r'''[()[\]{}\\\/,;:=*'"`+-<>\0\t\n\r ]''', label) \
-        or quote_underscores and "_" in label:
+    elif re.search(protect_regex, label) \
+        or " " in label \
+        or (quote_underscores and "_" in label):
         s = label.split("'")
         if len(s) == 1:
             return "'" + label + "'"
         return "'{}'".format("''".join(s))
     return label
 
 def bitmask_as_newick_string(split, taxon_set, preserve_spaces=False, quote_underscores=True):
```

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/nexusreader.py` & `DendroPy-5.0.1/src/dendropy/dataio/nexusreader.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/nexuswriter.py` & `DendroPy-5.0.1/src/dendropy/dataio/nexuswriter.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/nexusyielder.py` & `DendroPy-5.0.1/src/dendropy/dataio/nexusyielder.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/phylipreader.py` & `DendroPy-5.0.1/src/dendropy/dataio/phylipreader.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/phylipwriter.py` & `DendroPy-5.0.1/src/dendropy/dataio/phylipwriter.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/tokenizer.py` & `DendroPy-5.0.1/src/dendropy/dataio/tokenizer.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/dataio/xmlprocessing.py` & `DendroPy-5.0.1/src/dendropy/dataio/xmlprocessing.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/datamodel/__init__.py` & `DendroPy-5.0.1/src/dendropy/datamodel/__init__.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/datamodel/basemodel.py` & `DendroPy-5.0.1/src/dendropy/datamodel/basemodel.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/datamodel/charmatrixmodel.py` & `DendroPy-5.0.1/src/dendropy/datamodel/charmatrixmodel.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/datamodel/charstatemodel.py` & `DendroPy-5.0.1/src/dendropy/datamodel/charstatemodel.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/datamodel/datasetmodel.py` & `DendroPy-5.0.1/src/dendropy/datamodel/datasetmodel.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/datamodel/taxonmodel.py` & `DendroPy-5.0.1/src/dendropy/datamodel/taxonmodel.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/datamodel/treecollectionmodel.py` & `DendroPy-5.0.1/src/dendropy/datamodel/treecollectionmodel.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/datamodel/treemodel/__init__.py` & `DendroPy-5.0.1/src/dendropy/datamodel/treemodel/__init__.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/datamodel/treemodel/_bipartition.py` & `DendroPy-5.0.1/src/dendropy/datamodel/treemodel/_bipartition.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/datamodel/treemodel/_edge.py` & `DendroPy-5.0.1/src/dendropy/datamodel/treemodel/_edge.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/datamodel/treemodel/_node.py` & `DendroPy-5.0.1/src/dendropy/datamodel/treemodel/_node.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/datamodel/treemodel/_tree.py` & `DendroPy-5.0.1/src/dendropy/datamodel/treemodel/_tree.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/interop/__init__.py` & `DendroPy-5.0.1/src/dendropy/interop/__init__.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/interop/ape.py` & `DendroPy-5.0.1/src/dendropy/interop/ape.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/interop/biopython.py` & `DendroPy-5.0.1/src/dendropy/interop/biopython.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/interop/entrez.py` & `DendroPy-5.0.1/src/dendropy/interop/entrez.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/interop/ete.py` & `DendroPy-5.0.1/src/dendropy/interop/ete.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/interop/gbif.py` & `DendroPy-5.0.1/src/dendropy/interop/gbif.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/interop/genbank.py` & `DendroPy-5.0.1/src/dendropy/interop/genbank.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/interop/itol.py` & `DendroPy-5.0.1/src/dendropy/interop/itol.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/interop/muscle.py` & `DendroPy-5.0.1/src/dendropy/interop/muscle.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/interop/paup.py` & `DendroPy-5.0.1/src/dendropy/interop/paup.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/interop/raxml.py` & `DendroPy-5.0.1/src/dendropy/interop/raxml.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/interop/rspr.py` & `DendroPy-5.0.1/src/dendropy/interop/rspr.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/interop/rstats.py` & `DendroPy-5.0.1/src/dendropy/interop/rstats.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/interop/seqgen.py` & `DendroPy-5.0.1/src/dendropy/interop/seqgen.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/legacy/__init__.py` & `DendroPy-5.0.1/src/dendropy/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/legacy/coalescent.py` & `DendroPy-5.0.1/src/dendropy/legacy/coalescent.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/legacy/continuous.py` & `DendroPy-5.0.1/src/dendropy/legacy/continuous.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/legacy/ncbi.py` & `DendroPy-5.0.1/src/dendropy/legacy/ncbi.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/legacy/popgensim.py` & `DendroPy-5.0.1/src/dendropy/legacy/popgensim.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/legacy/popgenstat.py` & `DendroPy-5.0.1/src/dendropy/legacy/popgenstat.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/legacy/reconcile.py` & `DendroPy-5.0.1/src/dendropy/legacy/reconcile.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/legacy/seqmodel.py` & `DendroPy-5.0.1/src/dendropy/legacy/seqmodel.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/legacy/seqsim.py` & `DendroPy-5.0.1/src/dendropy/legacy/seqsim.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/legacy/treecalc.py` & `DendroPy-5.0.1/src/dendropy/legacy/treecalc.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/legacy/treemanip.py` & `DendroPy-5.0.1/src/dendropy/legacy/treemanip.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/legacy/treesim.py` & `DendroPy-5.0.1/src/dendropy/legacy/treesim.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/legacy/treesplit.py` & `DendroPy-5.0.1/src/dendropy/legacy/treesplit.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/legacy/treesum.py` & `DendroPy-5.0.1/src/dendropy/legacy/treesum.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/mathlib/__init__.py` & `DendroPy-5.0.1/src/dendropy/mathlib/__init__.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/mathlib/mathfn.py` & `DendroPy-5.0.1/src/dendropy/mathlib/mathfn.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/mathlib/probability.py` & `DendroPy-5.0.1/src/dendropy/mathlib/probability.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/mathlib/statistics.py` & `DendroPy-5.0.1/src/dendropy/mathlib/statistics.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/model/__init__.py` & `DendroPy-5.0.1/src/dendropy/model/__init__.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/model/birthdeath.py` & `DendroPy-5.0.1/src/dendropy/model/birthdeath.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/model/coalescent.py` & `DendroPy-5.0.1/src/dendropy/model/coalescent.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/model/continuous.py` & `DendroPy-5.0.1/src/dendropy/model/continuous.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/model/discrete.py` & `DendroPy-5.0.1/src/dendropy/model/discrete.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/model/multispeciescoalescent.py` & `DendroPy-5.0.1/src/dendropy/model/multispeciescoalescent.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/model/parsimony.py` & `DendroPy-5.0.1/src/dendropy/model/parsimony.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/model/protractedspeciation.py` & `DendroPy-5.0.1/src/dendropy/model/protractedspeciation.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/model/reconcile.py` & `DendroPy-5.0.1/src/dendropy/model/reconcile.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/model/treeshape.py` & `DendroPy-5.0.1/src/dendropy/model/treeshape.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/simulate/__init__.py` & `DendroPy-5.0.1/src/dendropy/simulate/__init__.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/simulate/charsim.py` & `DendroPy-5.0.1/src/dendropy/simulate/charsim.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/simulate/popgensim.py` & `DendroPy-5.0.1/src/dendropy/simulate/popgensim.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/simulate/treesim.py` & `DendroPy-5.0.1/src/dendropy/simulate/treesim.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/__init__.py` & `DendroPy-5.0.1/src/dendropy/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/bibtex.py` & `DendroPy-5.0.1/src/dendropy/utility/bibtex.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/bitprocessing.py` & `DendroPy-5.0.1/src/dendropy/utility/bitprocessing.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/cli.py` & `DendroPy-5.0.1/src/dendropy/utility/cli.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/constants.py` & `DendroPy-5.0.1/src/dendropy/utility/constants.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/container.py` & `DendroPy-5.0.1/src/dendropy/utility/container.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/debug.py` & `DendroPy-5.0.1/src/dendropy/utility/debug.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/deprecate.py` & `DendroPy-5.0.1/src/dendropy/utility/deprecate.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/error.py` & `DendroPy-5.0.1/src/dendropy/utility/error.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/filesys.py` & `DendroPy-5.0.1/src/dendropy/utility/filesys.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/libexec/__init__.py` & `DendroPy-5.0.1/src/dendropy/utility/libexec/__init__.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/messaging.py` & `DendroPy-5.0.1/src/dendropy/utility/messaging.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/metavar.py` & `DendroPy-5.0.1/src/dendropy/utility/metavar.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/processio.py` & `DendroPy-5.0.1/src/dendropy/utility/processio.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/terminal.py` & `DendroPy-5.0.1/src/dendropy/utility/terminal.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/textprocessing.py` & `DendroPy-5.0.1/src/dendropy/utility/textprocessing.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/timeprocessing.py` & `DendroPy-5.0.1/src/dendropy/utility/timeprocessing.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/urlio.py` & `DendroPy-5.0.1/src/dendropy/utility/urlio.py`

 * *Files identical despite different names*

### Comparing `DendroPy-5.0.0/src/dendropy/utility/vcsinfo.py` & `DendroPy-5.0.1/src/dendropy/utility/vcsinfo.py`

 * *Files identical despite different names*

