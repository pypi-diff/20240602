# Comparing `tmp/scikit_fingerprints-1.4.1.tar.gz` & `tmp/scikit_fingerprints-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit_fingerprints-1.4.1.tar", max compression
+gzip compressed data, was "scikit_fingerprints-1.5.0.tar", max compression
```

## Comparing `scikit_fingerprints-1.4.1.tar` & `scikit_fingerprints-1.5.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0     1116 2024-05-09 17:44:16.016286 scikit_fingerprints-1.4.1/LICENSE.md
--rw-r--r--   0        0        0     3243 2024-05-09 17:44:16.016286 scikit_fingerprints-1.4.1/README.md
--rwxr-xr-x   0        0        0     1445 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/__init__.py
--rw-r--r--   0        0        0      170 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/bases/__init__.py
--rw-r--r--   0        0        0     6701 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/bases/base_fp_transformer.py
--rw-r--r--   0        0        0     1704 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/bases/base_preprocessor.py
--rw-r--r--   0        0        0     4439 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/bases/base_substructure_fp.py
--rw-r--r--   0        0        0     1327 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/__init__.py
--rw-r--r--   0        0        0     9788 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/atom_pair.py
--rw-r--r--   0        0        0     1535 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/autocorr.py
--rw-r--r--   0        0        0     4499 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/avalon.py
--rw-r--r--   0        0        0     8677 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/e3fp_fp.py
--rw-r--r--   0        0        0     3121 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/ecfp.py
--rw-r--r--   0        0        0     8220 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/erg.py
--rw-r--r--   0        0        0     1517 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/estate.py
--rw-r--r--   0        0        0     7576 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/functional_groups.py
--rw-r--r--   0        0        0     1457 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/getaway.py
--rw-r--r--   0        0        0     7291 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/ghose_crippen.py
--rw-r--r--   0        0        0   235078 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/klekota_roth.py
--rw-r--r--   0        0        0    28063 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/laggner.py
--rw-r--r--   0        0        0     2434 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/layered.py
--rw-r--r--   0        0        0     6320 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/lingo.py
--rw-r--r--   0        0        0     1095 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/maccs.py
--rw-r--r--   0        0        0     6807 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/map.py
--rw-r--r--   0        0        0     3092 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/mhfp.py
--rw-r--r--   0        0        0     1425 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/mordred_fp.py
--rw-r--r--   0        0        0     1069 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/morse.py
--rw-r--r--   0        0        0     1653 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/pattern.py
--rw-r--r--   0        0        0     2683 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/pharmacophore.py
--rw-r--r--   0        0        0     1760 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/physiochemical_properties.py
--rw-r--r--   0        0        0    41704 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/fingerprints/pubchem.py
--rw-r--r--   0        0        0     1061 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/fingerprints/rdf.py
--rw-r--r--   0        0        0     3002 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/fingerprints/rdk.py
--rw-r--r--   0        0        0     2730 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/fingerprints/secfp.py
--rw-r--r--   0        0        0     2341 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/fingerprints/topological_torsion.py
--rw-r--r--   0        0        0     7561 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/fingerprints/usr.py
--rw-r--r--   0        0        0     8145 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/fingerprints/usrcat.py
--rw-r--r--   0        0        0     1445 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/fingerprints/whim.py
--rw-r--r--   0        0        0     3787 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/parallel.py
--rw-r--r--   0        0        0      133 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/preprocessing/__init__.py
--rw-r--r--   0        0        0    15027 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/preprocessing/conformer_generator.py
--rw-r--r--   0        0        0     2613 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/preprocessing/mol_to_from_smiles.py
--rw-r--r--   0        0        0      243 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/rdkit_logging.py
--rw-r--r--   0        0        0     1118 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/validators.py
--rw-r--r--   0        0        0     4246 1970-01-01 00:00:00.000000 scikit_fingerprints-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1116 2024-06-02 20:31:11.602161 scikit_fingerprints-1.5.0/LICENSE.md
+-rw-r--r--   0        0        0     4701 2024-06-02 20:31:11.602161 scikit_fingerprints-1.5.0/README.md
+-rwxr-xr-x   0        0        0     1510 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/__init__.py
+-rw-r--r--   0        0        0      170 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/bases/__init__.py
+-rw-r--r--   0        0        0     6701 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/bases/base_fp_transformer.py
+-rw-r--r--   0        0        0     1704 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/bases/base_preprocessor.py
+-rw-r--r--   0        0        0     4685 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/bases/base_substructure_fp.py
+-rw-r--r--   0        0        0     1361 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/__init__.py
+-rw-r--r--   0        0        0     9723 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/atom_pair.py
+-rw-r--r--   0        0        0     5288 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/autocorr.py
+-rw-r--r--   0        0        0     4500 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/avalon.py
+-rw-r--r--   0        0        0     8676 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/e3fp_fp.py
+-rw-r--r--   0        0        0     3121 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/ecfp.py
+-rw-r--r--   0        0        0     8220 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/erg.py
+-rw-r--r--   0        0        0     1517 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/estate.py
+-rw-r--r--   0        0        0     7576 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/functional_groups.py
+-rw-r--r--   0        0        0     1457 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/getaway.py
+-rw-r--r--   0        0        0     7537 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/ghose_crippen.py
+-rw-r--r--   0        0        0   235329 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/klekota_roth.py
+-rw-r--r--   0        0        0    28292 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/laggner.py
+-rw-r--r--   0        0        0     2434 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/layered.py
+-rw-r--r--   0        0        0     6320 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/lingo.py
+-rw-r--r--   0        0        0    12430 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/maccs.py
+-rw-r--r--   0        0        0     6807 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/map.py
+-rw-r--r--   0        0        0     3092 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/mhfp.py
+-rw-r--r--   0        0        0     1425 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/mordred_fp.py
+-rw-r--r--   0        0        0     1069 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/morse.py
+-rw-r--r--   0        0        0     4804 2024-06-02 20:31:11.606161 scikit_fingerprints-1.5.0/skfp/fingerprints/mqns.py
+-rw-r--r--   0        0        0     1653 2024-06-02 20:31:11.610161 scikit_fingerprints-1.5.0/skfp/fingerprints/pattern.py
+-rw-r--r--   0        0        0     2683 2024-06-02 20:31:11.610161 scikit_fingerprints-1.5.0/skfp/fingerprints/pharmacophore.py
+-rw-r--r--   0        0        0     1760 2024-06-02 20:31:11.610161 scikit_fingerprints-1.5.0/skfp/fingerprints/physiochemical_properties.py
+-rw-r--r--   0        0        0    44130 2024-06-02 20:31:11.610161 scikit_fingerprints-1.5.0/skfp/fingerprints/pubchem.py
+-rw-r--r--   0        0        0     1061 2024-06-02 20:31:11.610161 scikit_fingerprints-1.5.0/skfp/fingerprints/rdf.py
+-rw-r--r--   0        0        0     3002 2024-06-02 20:31:11.610161 scikit_fingerprints-1.5.0/skfp/fingerprints/rdk.py
+-rw-r--r--   0        0        0     2730 2024-06-02 20:31:11.610161 scikit_fingerprints-1.5.0/skfp/fingerprints/secfp.py
+-rw-r--r--   0        0        0     6248 2024-06-02 20:31:11.610161 scikit_fingerprints-1.5.0/skfp/fingerprints/topological_torsion.py
+-rw-r--r--   0        0        0     7595 2024-06-02 20:31:11.610161 scikit_fingerprints-1.5.0/skfp/fingerprints/usr.py
+-rw-r--r--   0        0        0     8175 2024-06-02 20:31:11.610161 scikit_fingerprints-1.5.0/skfp/fingerprints/usrcat.py
+-rw-r--r--   0        0        0     1445 2024-06-02 20:31:11.610161 scikit_fingerprints-1.5.0/skfp/fingerprints/whim.py
+-rw-r--r--   0        0        0     3787 2024-06-02 20:31:11.610161 scikit_fingerprints-1.5.0/skfp/parallel.py
+-rw-r--r--   0        0        0      133 2024-06-02 20:31:11.610161 scikit_fingerprints-1.5.0/skfp/preprocessing/__init__.py
+-rw-r--r--   0        0        0    15486 2024-06-02 20:31:11.610161 scikit_fingerprints-1.5.0/skfp/preprocessing/conformer_generator.py
+-rw-r--r--   0        0        0     2613 2024-06-02 20:31:11.610161 scikit_fingerprints-1.5.0/skfp/preprocessing/mol_to_from_smiles.py
+-rw-r--r--   0        0        0      243 2024-06-02 20:31:11.610161 scikit_fingerprints-1.5.0/skfp/rdkit_logging.py
+-rw-r--r--   0        0        0     1118 2024-06-02 20:31:11.610161 scikit_fingerprints-1.5.0/skfp/validators.py
+-rw-r--r--   0        0        0     5970 1970-01-01 00:00:00.000000 scikit_fingerprints-1.5.0/PKG-INFO
```

### Comparing `scikit_fingerprints-1.4.1/LICENSE.md` & `scikit_fingerprints-1.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/bases/base_fp_transformer.py` & `scikit_fingerprints-1.5.0/skfp/bases/base_fp_transformer.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/bases/base_preprocessor.py` & `scikit_fingerprints-1.5.0/skfp/bases/base_preprocessor.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/bases/base_substructure_fp.py` & `scikit_fingerprints-1.5.0/skfp/bases/base_substructure_fp.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,18 @@
 
     n_jobs : int, default=None
         The number of jobs to run in parallel. :meth:`transform` is parallelized
         over the input molecules. ``None`` means 1 unless in a
         :obj:`joblib.parallel_backend` context. ``-1`` means using all processors.
         See Scikit-learn documentation on ``n_jobs`` for more details.
 
+    batch_size : int, default=None
+        Number of inputs processed in each batch. ``None`` divides input data into
+        equal-sized parts, as many as ``n_jobs``.
+
     verbose : int, default=0
         Controls the verbosity when computing fingerprints.
 
     Attributes
     ----------
     n_features_out : int
         Number of output features, size of patterns. Equal to length of ``patterns``.
@@ -58,22 +62,24 @@
 
     def __init__(
         self,
         patterns: Sequence[str],
         count: bool = False,
         sparse: bool = False,
         n_jobs: Optional[int] = None,
+        batch_size: Optional[int] = None,
         verbose: int = 0,
         random_state: Optional[int] = 0,
     ):
         super().__init__(
             n_features_out=len(patterns),
             count=count,
             sparse=sparse,
             n_jobs=n_jobs,
+            batch_size=batch_size,
             verbose=verbose,
             random_state=random_state,
         )
         self.patterns = patterns
 
     def _validate_params(self) -> None:
         from rdkit.Chem import MolFromSmarts
```

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/__init__.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from .layered import LayeredFingerprint
 from .lingo import LingoFingerprint
 from .maccs import MACCSFingerprint
 from .map import MAPFingerprint
 from .mhfp import MHFPFingerprint
 from .mordred_fp import MordredFingerprint
 from .morse import MORSEFingerprint
+from .mqns import MQNsFingerprint
 from .pattern import PatternFingerprint
 from .pharmacophore import PharmacophoreFingerprint
 from .physiochemical_properties import PhysiochemicalPropertiesFingerprint
 from .pubchem import PubChemFingerprint
 from .rdf import RDFFingerprint
 from .rdk import RDKitFingerprint
 from .secfp import SECFPFingerprint
```

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/atom_pair.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/atom_pair.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,27 +56,26 @@
         Maximal distance between atoms. Must be positive and greater or equal to
         `min_distance`.
 
     include_chirality : bool, default=False
         Whether to include chirality information when computing atom types.
 
     count_simulation : bool, default=True
-        Whether to use count simulation for approximating feature counts.
-        See [3] for details.
+        Whether to use count simulation for approximating feature counts [3]_.
 
     use_3D : bool, default=False
         Whether to use 3D Euclidean distance matrix. If False, uses topological
         distances on molecular graph.
 
     count : bool, default=False
         Whether to return binary (bit) features, or their counts.
 
     scale_by_hac: bool or int, default=False
         Whether to scale count fingerprint by the heavy atom count (HAC) to
-        obtain a proportionality to molecule size [2]. If integer value is given,
+        obtain a proportionality to molecule size [2]_. If integer value is given,
         scaling uses given power of HAC, e.g. `scale_by_hac=2` divides counts by
         squared HAC. Values are expressed as percentages in range [0, 100].
 
     sparse : bool, default=False
         Whether to return dense NumPy array, or sparse SciPy CSR array.
 
     n_jobs : int, default=None
@@ -96,15 +95,15 @@
     ----------
     n_features_out : int
         Number of output features, size of fingerprints. Equal to `fp_size`.
 
     requires_conformers : bool
         Whether the fingerprint is 3D-based and requires molecules with conformers as
         inputs, with ``conf_id`` integer property set. This depends on the ``use_3D``
-        attribute, and has the same value as that parameter.
+        parameter, and has the same value.
 
     See Also
     --------
     :class:`TopologicalTorsionFingerprint` : Related fingerprint, but uses 4-atom paths.
 
     References
     ----------
@@ -118,15 +117,14 @@
         "Atom Pair 2D-Fingerprints Perceive 3D-Molecular Shape and Pharmacophores for
         Very Fast Virtual Screening of ZINC and GDB-17"
         J. Chem. Inf. Model. 2014, 54, 7, 1892–1907
         <https://pubs.acs.org/doi/10.1021/ci500232g>`_
 
     .. [3] `Greg Landrum
         "Simulating count fingerprints"
-        RDKit blog 2021
         <https://greglandrum.github.io/rdkit-blog/posts/2021-07-06-simulating-counts.html>`_
 
     Examples
     --------
     >>> from skfp.fingerprints import AtomPairFingerprint
     >>> smiles = ["O", "CC", "[C-]#N", "CC=O"]
     >>> fp = AtomPairFingerprint()
```

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/autocorr.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/physiochemical_properties.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,60 @@
 from collections.abc import Sequence
+from numbers import Integral
 from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
+from sklearn.utils._param_validation import Interval, StrOptions
 
 from skfp.bases import BaseFingerprintTransformer
-from skfp.validators import ensure_mols, require_mols_with_conf_ids
+from skfp.validators import ensure_mols
 
 
-class AutocorrFingerprint(BaseFingerprintTransformer):
-    """Autocorrelation fingerprint."""
+class PhysiochemicalPropertiesFingerprint(BaseFingerprintTransformer):
+    """Physiochemical properties fingerprint."""
 
     _parameter_constraints: dict = {
         **BaseFingerprintTransformer._parameter_constraints,
-        "use_3D": ["boolean"],
+        "fp_size": [Interval(Integral, 1, None, closed="left")],
+        "variant": [StrOptions({"BP", "BT"})],
     }
 
     def __init__(
         self,
-        use_3D: bool = False,
+        fp_size: int = 2048,
+        variant: str = "BP",
+        count: bool = False,
         sparse: bool = False,
         n_jobs: Optional[int] = None,
         batch_size: Optional[int] = None,
         verbose: int = 0,
     ):
-        n_features_out = 80 if use_3D else 192
         super().__init__(
-            n_features_out=n_features_out,
-            requires_conformers=use_3D,
+            n_features_out=fp_size,
+            count=count,
             sparse=sparse,
             n_jobs=n_jobs,
             batch_size=batch_size,
             verbose=verbose,
         )
-        self.use_3D = use_3D
+        self.fp_size = fp_size
+        self.variant = variant
 
     def _calculate_fingerprint(
         self, X: Sequence[Union[str, Mol]]
     ) -> Union[np.ndarray, csr_array]:
-        from rdkit.Chem.rdMolDescriptors import CalcAUTOCORR2D, CalcAUTOCORR3D
+        from rdkit.Chem.AtomPairs.Sheridan import GetBPFingerprint, GetBTFingerprint
 
-        if not self.use_3D:
-            X = ensure_mols(X)
-            X = [CalcAUTOCORR2D(mol) for mol in X]
-        else:
-            X = require_mols_with_conf_ids(X)
-            X = [CalcAUTOCORR3D(mol, confId=mol.GetIntProp("conf_id")) for mol in X]
+        X = ensure_mols(X)
 
-        return csr_array(X) if self.sparse else np.array(X)
+        if self.variant == "BP":
+            X = [GetBPFingerprint(mol) for mol in X]
+        else:  # "BT" variant
+            X = [GetBTFingerprint(mol) for mol in X]
+
+        X = self._hash_fingerprint_bits(
+            X, fp_size=self.fp_size, count=self.count, sparse=self.sparse
+        )
+
+        return X
```

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/avalon.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/avalon.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     requires_conformers : bool = False
         This fingerprint uses only 2D molecular graphs and does not require conformers.
 
     References
     ----------
     .. [1] Avalon toolkit
         https://sourceforge.net/projects/avalontoolkit/
+
     .. [2] `Gedeck, Peter, Bernhard Rohde, and Christian Bartels
         "QSAR − How Good Is It in Practice? Comparison of Descriptor Sets on an Unbiased
         Cross Section of Corporate Data Sets."
         J. Chem. Inf. Model. 2006, 46, 5, 1924–1936
         <https://pubs.acs.org/doi/abs/10.1021/ci050413p>`_
 
     Examples
```

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/e3fp_fp.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/e3fp_fp.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,14 @@
         X = require_mols_with_conf_ids(X)
         X = [self._calculate_single_mol_fingerprint(mol) for mol in X]
         return scipy.sparse.vstack(X) if self.sparse else np.array(X)
 
     def _calculate_single_mol_fingerprint(
         self, mol: Mol
     ) -> Union[np.ndarray, csr_array]:
-
         # e3fp requires "_Name" property to be set
         mol.SetProp("_Name", MolToSmiles(mol))
 
         # suppress flood of logs
         try:
             if not self.verbose:
                 logging.disable(logging.INFO)
```

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/ecfp.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/ecfp.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/erg.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/erg.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/estate.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/estate.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/functional_groups.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/functional_groups.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/getaway.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/getaway.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/ghose_crippen.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/ghose_crippen.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 
     n_jobs : int, default=None
         The number of jobs to run in parallel. :meth:`transform` is parallelized
         over the input molecules. ``None`` means 1 unless in a
         :obj:`joblib.parallel_backend` context. ``-1`` means using all processors.
         See Scikit-learn documentation on ``n_jobs`` for more details.
 
+    batch_size : int, default=None
+        Number of inputs processed in each batch. ``None`` divides input data into
+        equal-sized parts, as many as ``n_jobs``.
+
     verbose : int, default=0
         Controls the verbosity when computing fingerprints.
 
     Attributes
     ----------
     n_features_out : int = 110
         Number of output features, size of fingerprints.
@@ -73,14 +77,15 @@
     """
 
     def __init__(
         self,
         count: bool = False,
         sparse: bool = False,
         n_jobs: Optional[int] = None,
+        batch_size: Optional[int] = None,
         verbose: int = 0,
     ):
         # flake8: noqa: E501
         patterns = [
             "[CH4]",
             "[CH3]C",
             "[CH2](C)C",
@@ -194,14 +199,15 @@
         ]
         # flake8: noqa
         super().__init__(
             patterns=patterns,
             count=count,
             sparse=sparse,
             n_jobs=n_jobs,
+            batch_size=batch_size,
             verbose=verbose,
         )
 
     def transform(
         self, X: Sequence[Union[str, Mol]], copy: bool = False
     ) -> Union[np.ndarray, csr_array]:
         """
```

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/klekota_roth.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/klekota_roth.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
 
 from skfp.bases import BaseSubstructureFingerprint
 
 
 class KlekotaRothFingerprint(BaseSubstructureFingerprint):
-    """Klekota-Roth Fingerprint
+    """
+    Klekota-Roth Fingerprint
 
     A substructure fingerprint based on [1]_. Tests for presence of 4860 predefined
     substructures which are predisposed for bioactivity.
 
     Parameters
     ----------
     count : bool, default=False
@@ -24,14 +25,18 @@
 
     n_jobs : int, default=None
         The number of jobs to run in parallel. :meth:`transform` is parallelized
         over the input molecules. ``None`` means 1 unless in a
         :obj:`joblib.parallel_backend` context. ``-1`` means using all processors.
         See Scikit-learn documentation on ``n_jobs`` for more details.
 
+    batch_size : int, default=None
+        Number of inputs processed in each batch. ``None`` divides input data into
+        equal-sized parts, as many as ``n_jobs``.
+
     verbose : int, default=0
         Controls the verbosity when computing fingerprints.
 
     Attributes
     ----------
     n_features_out : int = 4860
         Number of output features, size of fingerprints.
@@ -62,14 +67,15 @@
     """
 
     def __init__(
         self,
         count: bool = False,
         sparse: bool = False,
         n_jobs: Optional[int] = None,
+        batch_size: Optional[int] = None,
         verbose: int = 0,
     ):
         # flake8: noqa: E501
         patterns = [
             "[!#1][CH]([!#1])[!#1]",
             "[!#1][CH]([!#1])[CH]([!#1])[!#1]",
             "[!#1][CH]([!#1])[CH]([!#1])C([CH3])([CH3])[CH3]",
@@ -4933,14 +4939,15 @@
         ]
         # flake8: noqa
         super().__init__(
             patterns=patterns,
             count=count,
             sparse=sparse,
             n_jobs=n_jobs,
+            batch_size=batch_size,
             verbose=verbose,
         )
 
     def transform(
         self, X: Sequence[Union[str, Mol]], copy: bool = False
     ) -> Union[np.ndarray, csr_array]:
         """
```

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/laggner.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/laggner.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class LaggnerFingerprint(BaseSubstructureFingerprint):
     """
     Substructure fingerprint with definitions by Christian Laggner.
 
     A substructure fingerprint based on SMARTS patterns for functional group
     classification, proposed by Christian Laggner [1]_. It is also known as
-    SubstructureFingerprint in Chemistry Development Toolkit (CDK) [2]_.
+    SubstructureFingerprint in Chemistry Development Kit (CDK) [2]_.
     It tests for presence of 307 predefined substructures, designed for functional
     groups of organic compounds, for use in similarity searching.
 
     Parameters
     ----------
     count : bool, default=False
         Whether to return binary (bit) features, or their counts.
@@ -29,14 +29,18 @@
 
     n_jobs : int, default=None
         The number of jobs to run in parallel. :meth:`transform` is parallelized
         over the input molecules. ``None`` means 1 unless in a
         :obj:`joblib.parallel_backend` context. ``-1`` means using all processors.
         See Scikit-learn documentation on ``n_jobs`` for more details.
 
+    batch_size : int, default=None
+        Number of inputs processed in each batch. ``None`` divides input data into
+        equal-sized parts, as many as ``n_jobs``.
+
     verbose : int, default=0
         Controls the verbosity when computing fingerprints.
 
     Attributes
     ----------
     n_features_out : int = 307
         Number of output features, size of fingerprints.
@@ -47,17 +51,17 @@
     References
     ----------
     .. [1] `Christian Laggner
         "SMARTS Patterns for Functional Group Classification"
         OpenBabel
         <https://raw.githubusercontent.com/openbabel/openbabel/master/data/SMARTS_InteLigand.txt>`_
 
-    .. [1] `egonw
+    .. [2] `egonw
         "SubstructureFingerprinter"
-        Chemistry Development Toolkit (CDK) API reference
+        Chemistry Development Kit (CDK) API reference
         <https://cdk.github.io/cdk/1.5/docs/api/org/openscience/cdk/fingerprint/SubstructureFingerprinter.html>`_
 
     Examples
     --------
     >>> from skfp.fingerprints import LaggnerFingerprint
     >>> smiles = ["O", "CC", "[C-]#N", "CC=O"]
     >>> fp = LaggnerFingerprint()
@@ -72,14 +76,15 @@
     """
 
     def __init__(
         self,
         count: bool = False,
         sparse: bool = False,
         n_jobs: Optional[int] = None,
+        batch_size: Optional[int] = None,
         verbose: int = 0,
     ):
         # RDKit does not support multi-component SMARTS (with a dot), so we can't match
         # the salts pattern "([-1,-2,-3,-4,-5,-6,-7]).([+1,+2,+3,+4,+5,+6,+7])"
         # (position 299); we compute it manually in .transform(), and here temporarily
         # replace it with a wildcard pattern "*"
 
@@ -395,22 +400,23 @@
         ]
         # flake8: noqa
         super().__init__(
             patterns=patterns,
             count=count,
             sparse=sparse,
             n_jobs=n_jobs,
+            batch_size=batch_size,
             verbose=verbose,
         )
 
     def transform(
         self, X: Sequence[Union[str, Mol]], copy: bool = False
     ) -> Union[np.ndarray, csr_array]:
         """
-        Compute CDK substructure fingerprints.
+        Compute Laggner fingerprints.
 
         Parameters
         ----------
         X : {sequence, array-like} of shape (n_samples,)
             Sequence containing SMILES strings or RDKit Mol objects.
 
         copy : bool, default=False
```

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/layered.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/layered.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/lingo.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/lingo.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/maccs.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/morse.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,40 +2,35 @@
 from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
 
 from skfp.bases import BaseFingerprintTransformer
-from skfp.validators import ensure_mols
+from skfp.validators import require_mols_with_conf_ids
 
 
-class MACCSFingerprint(BaseFingerprintTransformer):
-    """MACCS fingerprint."""
+class MORSEFingerprint(BaseFingerprintTransformer):
+    """MORSE fingerprint."""
 
     def __init__(
         self,
         sparse: bool = False,
         n_jobs: Optional[int] = None,
         batch_size: Optional[int] = None,
         verbose: int = 0,
     ):
         super().__init__(
-            n_features_out=167,
+            n_features_out=224,
+            requires_conformers=True,
             sparse=sparse,
             n_jobs=n_jobs,
             batch_size=batch_size,
             verbose=verbose,
         )
 
-    def _calculate_fingerprint(
-        self, X: Sequence[Union[str, Mol]]
-    ) -> Union[np.ndarray, csr_array]:
-        from rdkit.Chem.rdMolDescriptors import GetMACCSKeysFingerprint
-
-        X = ensure_mols(X)
-        X = [GetMACCSKeysFingerprint(mol) for mol in X]
-
-        if self.sparse:
-            return csr_array(X, dtype=np.uint8)
-        else:
-            return np.array(X, dtype=np.uint8)
+    def _calculate_fingerprint(self, X: Sequence[Mol]) -> Union[np.ndarray, csr_array]:
+        from rdkit.Chem.rdMolDescriptors import CalcMORSE
+
+        X = require_mols_with_conf_ids(X)
+        X = [CalcMORSE(mol, confId=mol.GetIntProp("conf_id")) for mol in X]
+        return csr_array(X) if self.sparse else np.array(X)
```

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/map.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/map.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/mhfp.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/mhfp.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/mordred_fp.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/mordred_fp.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/morse.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/rdf.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
 
 from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import require_mols_with_conf_ids
 
 
-class MORSEFingerprint(BaseFingerprintTransformer):
-    """MORSE fingerprint."""
+class RDFFingerprint(BaseFingerprintTransformer):
+    """RDF fingerprint."""
 
     def __init__(
         self,
         sparse: bool = False,
         n_jobs: Optional[int] = None,
         batch_size: Optional[int] = None,
         verbose: int = 0,
     ):
         super().__init__(
-            n_features_out=224,
+            n_features_out=210,
             requires_conformers=True,
             sparse=sparse,
             n_jobs=n_jobs,
             batch_size=batch_size,
             verbose=verbose,
         )
 
     def _calculate_fingerprint(self, X: Sequence[Mol]) -> Union[np.ndarray, csr_array]:
-        from rdkit.Chem.rdMolDescriptors import CalcMORSE
+        from rdkit.Chem.rdMolDescriptors import CalcRDF
 
         X = require_mols_with_conf_ids(X)
-        X = [CalcMORSE(mol, confId=mol.GetIntProp("conf_id")) for mol in X]
+        X = [CalcRDF(mol, confId=mol.GetIntProp("conf_id")) for mol in X]
         return csr_array(X) if self.sparse else np.array(X)
```

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/pattern.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/pattern.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/pharmacophore.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/pharmacophore.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/rdf.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/whim.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 from collections.abc import Sequence
+from numbers import Real
 from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
+from sklearn.utils._param_validation import Interval
 
 from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import require_mols_with_conf_ids
 
 
-class RDFFingerprint(BaseFingerprintTransformer):
-    """RDF fingerprint."""
+class WHIMFingerprint(BaseFingerprintTransformer):
+    """WHIM fingerprint."""
+
+    _parameter_constraints: dict = {
+        **BaseFingerprintTransformer._parameter_constraints,
+        "clip_val": [Interval(Real, 0, None, closed="left")],
+    }
 
     def __init__(
         self,
+        clip_val: int = np.iinfo(np.int32).max,
         sparse: bool = False,
         n_jobs: Optional[int] = None,
         batch_size: Optional[int] = None,
         verbose: int = 0,
     ):
         super().__init__(
-            n_features_out=210,
+            n_features_out=114,
             requires_conformers=True,
             sparse=sparse,
             n_jobs=n_jobs,
             batch_size=batch_size,
             verbose=verbose,
         )
+        self.clip_val = clip_val
 
     def _calculate_fingerprint(self, X: Sequence[Mol]) -> Union[np.ndarray, csr_array]:
-        from rdkit.Chem.rdMolDescriptors import CalcRDF
+        from rdkit.Chem.rdMolDescriptors import CalcWHIM
 
         X = require_mols_with_conf_ids(X)
-        X = [CalcRDF(mol, confId=mol.GetIntProp("conf_id")) for mol in X]
+        X = [CalcWHIM(mol, confId=mol.GetIntProp("conf_id")) for mol in X]
+        X = np.clip(X, -self.clip_val, self.clip_val)
         return csr_array(X) if self.sparse else np.array(X)
```

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/rdk.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/rdk.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/secfp.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/secfp.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/usr.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/usr.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 from skfp.validators import require_mols_with_conf_ids
 
 
 class USRFingerprint(BaseFingerprintTransformer):
     """
     USR (Ultrafast Shape Recognition) fingerprint.
 
-    The implementation uses RDKit. This fingerprint characterizes the shape of the
-    molecule by encoding the relative positions of its atoms [1]_ [2]_. Four points
-    are considered: molecular centroid (ctd), the closest atom to centroid (cst), the
-    farthest atom from centroid (fct), and atom the fartest from fct (ftf). Distances
-    from all atoms to each of those four points are computed, and each of those
-    distributions is summarized its first three moments: mean, variance, and skewness.
-    Concretely, standard deviation and cubic root of skewness are used to keep the same
-    unit. This results in 12 descriptors.
+    The implementation uses RDKit. This is a descriptor-based fingerprint, which
+    characterizes the shape of the molecule by encoding the relative positions of its
+    atoms [1]_ [2]_.
+
+    Four points are considered: molecular centroid (ctd), the closest atom to centroid (cst),
+    the farthest atom from centroid (fct), and atom the fartest from fct (ftf). Distances
+    from all atoms to each of those four points are computed, and each of those distributions
+    is summarized its first three moments: mean, variance, and skewness. Concretely, standard
+    deviation and cubic root of skewness are used to keep the same unit. This results in
+    12 descriptors.
 
     This is a 3D fingerprint, and requries molecules with ``conf_id`` integer property
     set. They can be generated with :class:`~skfp.preprocessing.ConformerGenerator`.
     Furthermore, only molecules with 3 or more atoms are allowed, to allow computation
     of all three moments.
 
     Parameters
```

### Comparing `scikit_fingerprints-1.4.1/skfp/fingerprints/usrcat.py` & `scikit_fingerprints-1.5.0/skfp/fingerprints/usrcat.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 from skfp.validators import require_mols_with_conf_ids
 
 
 class USRCATFingerprint(BaseFingerprintTransformer):
     """
     USRCAT (Ultrafast Shape Recognition with CREDO Atom Types) fingerprint.
 
-    The implementation uses RDKit. This fingerprint extends the USR fingerprint by
-    additionally considering pharmacophoric atom types [1]_. Firstly, the four
-    reference points are computed, and they are used in all five feature groups. Each
-    group is processed exactly the same, i.e. distance distributions to reference
-    points are calculated, and features from the first three moments (mean, standard
-    deviation, cubic root of skewness) are computed. This results in 12 features.
+    The implementation uses RDKit. This is a descriptor-based fingerprint, extending
+    the USR fingerprint by additionally considering pharmacophoric atom types [1]_.
+
+    Firstly, the four reference points are computed, and they are used in all five
+    feature groups. Each group is processed exactly the same, i.e. distance distributions
+    to reference points are calculated, and features from the first three moments
+    (mean, standard deviation, cubic root of skewness) are computed. This results in
+    12 features.
 
     USRCAT expands on USR by considering 4 additional subsets of atoms, based on their
     pharmacophoric types: hydrophobic, aromatic, hydrogen bond donor or acceptor atoms.
     For each atoms subset, distance distribution and moments are calculated like in
     the original USR. This results in 5 * 12 = 60 features.
 
     This is a 3D fingerprint, and requries molecules with ``conf_id`` integer property
```

### Comparing `scikit_fingerprints-1.4.1/skfp/parallel.py` & `scikit_fingerprints-1.5.0/skfp/parallel.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/preprocessing/conformer_generator.py` & `scikit_fingerprints-1.5.0/skfp/preprocessing/conformer_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 from rdkit.Chem.rdForceFieldHelpers import (
     MMFFGetMoleculeForceField,
     MMFFGetMoleculeProperties,
     MMFFSanitizeMolecule,
     UFFGetMoleculeForceField,
 )
 from rdkit.ForceField import ForceField
-from sklearn.utils import Interval
-from sklearn.utils._param_validation import InvalidParameterError, StrOptions
+from sklearn.utils._param_validation import Interval, InvalidParameterError, StrOptions
 
 from skfp.bases import BasePreprocessor
 from skfp.parallel import run_in_parallel
 from skfp.validators import ensure_mols
 
 
 class ConformerGenerator(BasePreprocessor):
@@ -62,26 +61,32 @@
         If larger than 1, one conformation will be selected, as specified with
         ``multiple_confs_select``.
 
     max_gen_attempts : int, default=10000
         Number of attempts to generate a conformer. Must be positive, and should be
         sufficiently large, typically at least a few thousands.
 
-    error_on_gen_fail : boolean, default=True
-        Whether to throw an error when no conformers can be generated for a molecule.
-
     optimize_force_field : {"UFF", "MMFF94", "MMFF94s", None}, default=None
         Force field optimization algorithm used on generated conformers. It is also
         used for calculation of conformer energy when selecting one of multiple
         conformations with ``multiple_confs_select="min_energy"``.
 
     multiple_confs_select : {"min_energy", "first"}, default="min_energy"
         How to select final conformer for each molecule when multiple conformers are
         generated. "first" selects first conformer generated by RDKit.
 
+    errors : {"raise", "ignore", "filter"}, default="raise"
+        How to handle errors during conformer generation, if after all attempts and
+        approaches a conformer could not be generated. ``"raise"`` immediately raises
+        any errors, with failure reason. ``"ignore"`` suppresses errors and returns
+        molecules without conformers and ``conf_id`` property set to `-1`. ``"filter"``
+        suppresses errors and removes such conformers, resulting in potentially less
+        output molecules than inputs. The latter two options can potentially cause
+        problems downstream, and should be used with caution.
+
     n_jobs : int, default=None
         The number of jobs to run in parallel. :meth:`transform_x_y` and
         :meth:`transform` are parallelized over the input molecules. ``None`` means 1
         unless in a :obj:`joblib.parallel_backend` context. ``-1`` means using all
         processors. See Scikit-learn documentation on ``n_jobs`` for more details.
 
     batch_size : int, default=None
@@ -132,37 +137,38 @@
 
     _parameter_constraints: dict = {
         "num_conformers": [Interval(Integral, 1, None, closed="left")],
         "max_gen_attempts": [Interval(Integral, 1, None, closed="left")],
         "error_on_conf_gen_fail": ["boolean"],
         "optimize_force_field": [StrOptions({"UFF", "MMFF94", "MMFF94s"}), None],
         "multiple_confs_select": [StrOptions({"min_energy", "first"})],
+        "errors": [StrOptions({"raise", "ignore", "filter"})],
         "n_jobs": [Integral, None],
         "batch_size": [Integral, None],
         "verbose": ["verbose"],
         "random_state": [Interval(Integral, left=-1, right=None, closed="left")],
     }
 
     def __init__(
         self,
         num_conformers: int = 1,
         max_gen_attempts: int = 1000,
-        error_on_gen_fail: bool = True,
         optimize_force_field: Optional[str] = None,
         multiple_confs_select: Optional[str] = "min_energy",
+        errors: str = "raise",
         n_jobs: Optional[int] = None,
         batch_size: Optional[int] = None,
         verbose: int = 0,
         random_state: Optional[int] = 0,
     ):
         self.num_conformers = num_conformers
         self.max_gen_attempts = max_gen_attempts
-        self.error_on_gen_fail = error_on_gen_fail
         self.optimize_force_field = optimize_force_field
         self.multiple_confs_select = multiple_confs_select
+        self.errors = errors
         self.n_jobs = n_jobs
         self.batch_size = batch_size
         self.verbose = verbose
         self.random_state = random_state
 
     def _validate_params(self) -> None:
         super()._validate_params()
@@ -180,14 +186,19 @@
 
     def transform_x_y(
         self, X: Sequence[Mol], y: np.ndarray, copy: bool = False
     ) -> tuple[list[PropertyMol], np.ndarray]:
         """
         Generate conformers for molecules.
 
+        If ``errors`` is set to ``"filter"``, then in case of errors less than
+        n_samples values may be returned. If ``errors`` is set to ``"ignore"``,
+        some molecules may be returned without conformers generated and with
+        ``conf_id`` property set to -1.
+
         Parameters
         ----------
         X : {sequence, array-like} of shape (n_samples,)
             Sequence containing RDKit Mol objects.
 
         y : np.ndarray of shape (n_samples,)
             Array with labels for molecules.
@@ -198,47 +209,42 @@
 
         Returns
         -------
         X : list of shape (n_samples_conf_gen,)
             List with RDKit PropertyMol objects, each one with conformers computed and
             ``conf_id`` integer property set.
 
-            Length of returned outputs ``n_samples_conf_gen`` will ideally be the same
-            as input ``n_samples``, but can be less if conformer generation failed and
-            ``error_on_gen_fail`` is False.
-
         y : np.ndarray of shape (n_samples_conf_gen,)
-            Array with labels for molecules, for which conformers were generated. Has
-            the same length as output ``X``, which can be less than input ``n_samples``
-            if conformer generation fails for some molecules.
+            Array with labels for molecules.
         """
         return self._transform(X, y, copy)
 
     def transform(self, X: Sequence[Mol], copy: bool = False) -> list[PropertyMol]:
         """
         Generate conformers for molecules.
 
+        If ``errors`` is set to ``"filter"``, then in case of errors less than
+        n_samples values may be returned. If ``errors`` is set to ``"ignore"``,
+        some molecules may be returned without conformers generated and with
+        ``conf_id`` property set to -1.
+
         Parameters
         ----------
         X : {sequence, array-like} of shape (n_samples,)
             Sequence containing RDKit Mol objects.
 
         copy : bool, default=True
             Copy the input X or not. In contrast to most classes, input molecules
             are copied by default, since RDKit modifies them with conformers in place.
 
         Returns
         -------
         X : list of shape (n_samples_conf_gen,)
             List with RDKit PropertyMol objects, each one with conformers computed and
             ``conf_id`` integer property set.
-
-            Length of returned outputs ``n_samples_conf_gen`` will ideally be the same
-            as input ``n_samples``, but can be less if conformer generation failed and
-            ``error_on_gen_fail`` is False.
         """
         y = np.empty(len(X))
         X, y = self._transform(X, y, copy)
         return X
 
     def _transform(
         self, X: Sequence[Mol], y: np.ndarray, copy: bool = True
@@ -264,15 +270,15 @@
                 verbose=self.verbose,
             )
 
         # keep only molecules and labels for which we generated conformers
         mols_with_conformers = []
         idxs_to_keep = []
         for idx, mol in enumerate(mols):
-            if mol.GetIntProp("conf_id") != -1:
+            if mol.GetIntProp("conf_id") != -1 or self.errors == "ignore":
                 mols_with_conformers.append(mol)
                 idxs_to_keep.append(idx)
 
         y = y[idxs_to_keep]
 
         return mols_with_conformers, y
 
@@ -328,15 +334,15 @@
             embed_params.ignoreSmoothingFailures = True
             conf_id = embedder(mol, params=embed_params)
 
         # we should not fail at this point
         if conf_id == -1:
             smiles = MolToSmiles(RemoveHs(mol))
             fail_reason = self._print_conf_gen_failure_reason(embed_params)
-            if self.error_on_gen_fail:
+            if self.errors == "raise":
                 raise ValueError(
                     f"Could not generate conformer for {smiles}:\n{fail_reason}"
                 )
             elif self.verbose:
                 print(f"Could not generate conformer for {smiles}:\n{fail_reason}")
                 return mol, -1
```

### Comparing `scikit_fingerprints-1.4.1/skfp/preprocessing/mol_to_from_smiles.py` & `scikit_fingerprints-1.5.0/skfp/preprocessing/mol_to_from_smiles.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.1/skfp/validators.py` & `scikit_fingerprints-1.5.0/skfp/validators.py`

 * *Files identical despite different names*

