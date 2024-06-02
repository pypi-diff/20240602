# Comparing `tmp/dime_sampler-0.9.1.tar.gz` & `tmp/dime_sampler-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dime_sampler-0.9.1.tar", last modified: Mon May 13 12:32:27 2024, max compression
+gzip compressed data, was "dime_sampler-1.0.0.tar", last modified: Sun Jun  2 06:49:30 2024, max compression
```

## Comparing `dime_sampler-0.9.1.tar` & `dime_sampler-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-05-13 12:32:27.475895 dime_sampler-0.9.1/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-05-13 12:32:27.469229 dime_sampler-0.9.1/.github/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-05-13 12:32:27.472562 dime_sampler-0.9.1/.github/workflows/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1058 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/.github/workflows/continuous-integration.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      187 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/.gitignore
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      281 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      599 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/.readthedocs.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/LICENSE
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8374 2024-05-13 12:32:27.475895 dime_sampler-0.9.1/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7886 2024-05-13 12:22:37.000000 dime_sampler-0.9.1/README.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-05-13 12:32:27.472562 dime_sampler-0.9.1/dime_sampler/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       69 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/dime_sampler/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       47 2024-05-13 12:32:13.000000 dime_sampler-0.9.1/dime_sampler/__version__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7108 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/dime_sampler/moves.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2118 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/dime_sampler/test_all.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-05-13 12:32:27.472562 dime_sampler-0.9.1/dime_sampler/test_storage/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      136 2024-05-13 12:26:42.000000 dime_sampler-0.9.1/dime_sampler/test_storage/median.npy
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-05-13 12:32:27.475895 dime_sampler-0.9.1/dime_sampler.egg-info/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8374 2024-05-13 12:32:27.000000 dime_sampler-0.9.1/dime_sampler.egg-info/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      673 2024-05-13 12:32:27.000000 dime_sampler-0.9.1/dime_sampler.egg-info/SOURCES.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2024-05-13 12:32:27.000000 dime_sampler-0.9.1/dime_sampler.egg-info/dependency_links.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       18 2024-05-13 12:32:27.000000 dime_sampler-0.9.1/dime_sampler.egg-info/requires.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       13 2024-05-13 12:32:27.000000 dime_sampler-0.9.1/dime_sampler.egg-info/top_level.txt
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-05-13 12:32:27.475895 dime_sampler-0.9.1/docs/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-05-13 12:32:27.475895 dime_sampler-0.9.1/docs/.ipynb_checkpoints/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1520 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/docs/.ipynb_checkpoints/hank_estimation-checkpoint.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/docs/Makefile
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1606 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/docs/conf.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       68 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/docs/content.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    62581 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/docs/dist.png
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       27 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/docs/index.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    49094 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/docs/lprobs.png
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      800 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/docs/make.bat
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      129 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/docs/modules.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       83 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/docs/requirements.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   289010 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/docs/traces.png
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       18 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/requirements.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2024-05-13 12:32:27.475895 dime_sampler-0.9.1/setup.cfg
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1057 2024-05-13 11:53:10.000000 dime_sampler-0.9.1/setup.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-06-02 06:49:30.246698 dime_sampler-1.0.0/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-06-02 06:49:30.240031 dime_sampler-1.0.0/.github/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-06-02 06:49:30.243364 dime_sampler-1.0.0/.github/workflows/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1058 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/.github/workflows/continuous-integration.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      187 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/.gitignore
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      281 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      599 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/.readthedocs.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/LICENSE
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8377 2024-06-02 06:49:30.246698 dime_sampler-1.0.0/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7889 2024-05-19 19:31:27.000000 dime_sampler-1.0.0/README.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-06-02 06:49:30.243364 dime_sampler-1.0.0/dime_sampler/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       69 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/dime_sampler/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       47 2024-06-02 06:48:33.000000 dime_sampler-1.0.0/dime_sampler/__version__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7183 2024-06-02 05:52:34.000000 dime_sampler-1.0.0/dime_sampler/moves.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2118 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/dime_sampler/test_all.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-06-02 06:49:30.243364 dime_sampler-1.0.0/dime_sampler/test_storage/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      136 2024-06-02 06:47:25.000000 dime_sampler-1.0.0/dime_sampler/test_storage/median.npy
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-06-02 06:49:30.246698 dime_sampler-1.0.0/dime_sampler.egg-info/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8377 2024-06-02 06:49:30.000000 dime_sampler-1.0.0/dime_sampler.egg-info/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      673 2024-06-02 06:49:30.000000 dime_sampler-1.0.0/dime_sampler.egg-info/SOURCES.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2024-06-02 06:49:30.000000 dime_sampler-1.0.0/dime_sampler.egg-info/dependency_links.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       18 2024-06-02 06:49:30.000000 dime_sampler-1.0.0/dime_sampler.egg-info/requires.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       13 2024-06-02 06:49:30.000000 dime_sampler-1.0.0/dime_sampler.egg-info/top_level.txt
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-06-02 06:49:30.246698 dime_sampler-1.0.0/docs/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-06-02 06:49:30.246698 dime_sampler-1.0.0/docs/.ipynb_checkpoints/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1520 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/docs/.ipynb_checkpoints/hank_estimation-checkpoint.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/docs/Makefile
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1606 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/docs/conf.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       68 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/docs/content.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    62581 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/docs/dist.png
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       27 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/docs/index.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    49094 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/docs/lprobs.png
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      800 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/docs/make.bat
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      129 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/docs/modules.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       83 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/docs/requirements.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   289010 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/docs/traces.png
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       18 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/requirements.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2024-06-02 06:49:30.246698 dime_sampler-1.0.0/setup.cfg
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1057 2024-04-27 08:53:31.000000 dime_sampler-1.0.0/setup.py
```

### Comparing `dime_sampler-0.9.1/.github/workflows/continuous-integration.yml` & `dime_sampler-1.0.0/.github/workflows/continuous-integration.yml`

 * *Files identical despite different names*

### Comparing `dime_sampler-0.9.1/.readthedocs.yaml` & `dime_sampler-1.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dime_sampler-0.9.1/LICENSE` & `dime_sampler-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dime_sampler-0.9.1/PKG-INFO` & `dime_sampler-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dime_sampler
-Version: 0.9.1
+Version: 1.0.0
 Summary: DIME MCMC sampling for python
 Home-page: https://github.com/gboehl/dime_sampler
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,20 +17,21 @@
 
 dime_sampler
 ============
 
 .. |badge0| image:: https://img.shields.io/badge/GitHub-gboehl%2Fdime__sampler-blue.svg?style=flat
     :target: https://github.com/gboehl/dime_sampler
 .. |badge1| image:: https://github.com/gboehl/dime_sampler/actions/workflows/continuous-integration.yml/badge.svg
-    :target: https://github.com/gboehl/dime_sampler/actions/workflows/continuous-integration.yml
+    :target: https://github.com/gboehl/dime_sampler/actions/workflows
 .. |badge2| image:: https://readthedocs.org/projects/dime-sampler/badge/?version=latest
-    :target: https://dime-sampler.readthedocs.io/en/latest/?badge=latest
+    :target: https://dime-sampler.readthedocs.io
     :alt: Documentation Status
 .. |badge3| image:: https://img.shields.io/pypi/v/dime_sampler
-   :alt: PyPI - Version
+    :target: https://pypi.org/project/dime-sampler/ 
+    :alt: PyPI - Version
 
 |badge0| |badge1| |badge2| |badge3|
 
 **Differential-Independence Mixture Ensemble ("DIME") MCMC sampling for Python** 
 
 This is the Python implementation of the DIME sampler proposed in `Ensemble MCMC Sampling for Robust Bayesian Inference <https://gregorboehl.com/live/dime_mcmc_boehl.pdf>`_ *(Gregor Boehl, 2022, SSRN No. 4250395)*. It provides the ``DIMEMove`` as a drop-in replacement for the great `emcee <https://github.com/dfm/emcee>`_ MCMC package.
```

### Comparing `dime_sampler-0.9.1/README.rst` & `dime_sampler-1.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 dime_sampler
 ============
 
 .. |badge0| image:: https://img.shields.io/badge/GitHub-gboehl%2Fdime__sampler-blue.svg?style=flat
     :target: https://github.com/gboehl/dime_sampler
 .. |badge1| image:: https://github.com/gboehl/dime_sampler/actions/workflows/continuous-integration.yml/badge.svg
-    :target: https://github.com/gboehl/dime_sampler/actions/workflows/continuous-integration.yml
+    :target: https://github.com/gboehl/dime_sampler/actions/workflows
 .. |badge2| image:: https://readthedocs.org/projects/dime-sampler/badge/?version=latest
-    :target: https://dime-sampler.readthedocs.io/en/latest/?badge=latest
+    :target: https://dime-sampler.readthedocs.io
     :alt: Documentation Status
 .. |badge3| image:: https://img.shields.io/pypi/v/dime_sampler
-   :alt: PyPI - Version
+    :target: https://pypi.org/project/dime-sampler/ 
+    :alt: PyPI - Version
 
 |badge0| |badge1| |badge2| |badge3|
 
 **Differential-Independence Mixture Ensemble ("DIME") MCMC sampling for Python** 
 
 This is the Python implementation of the DIME sampler proposed in `Ensemble MCMC Sampling for Robust Bayesian Inference <https://gregorboehl.com/live/dime_mcmc_boehl.pdf>`_ *(Gregor Boehl, 2022, SSRN No. 4250395)*. It provides the ``DIMEMove`` as a drop-in replacement for the great `emcee <https://github.com/dfm/emcee>`_ MCMC package.
```

### Comparing `dime_sampler-0.9.1/dime_sampler/moves.py` & `dime_sampler-1.0.0/dime_sampler/moves.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,23 +37,25 @@
         standard deviation of the Gaussian used to stretch the proposal vector.
     gamma : float, optional
         mean stretch factor for the proposal vector. By default, it is :math:`2.38 / \sqrt{2\,\mathrm{ndim}}` as recommended by `ter Braak (2006) <http://www.stat.columbia.edu/~gelman/stuff_for_blog/cajo.pdf>`_.
     aimh_prob : float, optional
         probability to draw an adaptive independence Metropolis Hastings (AIMH) proposal. By default this is set to :math:`0.1`.
     df_proposal_dist : float, optional
         degrees of freedom of the multivariate t distribution used for AIMH proposals. Defaults to :math:`10`.
+    rho : float, optional
+        decay parameter for the aimh proposal mean and covariances. Defaults to :math:`0.999`.
     """
 
     def __init__(
-        self, sigma=1.0e-5, gamma=None, aimh_prob=0.1, df_proposal_dist=10, delta=.999, **kwargs
+        self, sigma=1.0e-5, gamma=None, aimh_prob=0.1, df_proposal_dist=10, rho=.999, **kwargs
     ):
 
         self.sigma = sigma
         self.g0 = gamma
-        self.decay = delta
+        self.decay = rho
         self.aimh_prob = aimh_prob
         self.dft = df_proposal_dist
 
         super(DIMEMove, self).__init__(**kwargs)
 
     def setup(self, coords):
         # set some sane defaults
@@ -106,16 +108,15 @@
             np.exp(self.cumlweight - newcumlweight) * self.prop_cov
             + np.exp(lweight - newcumlweight) * ncov
         )
         self.prop_mean = (
             np.exp(self.cumlweight - newcumlweight) * self.prop_mean
             + np.exp(lweight - newcumlweight) * nmean
         )
-        # self.cumlweight = newcumlweight + np.log(self.decay)
-        self.cumlweight = newcumlweight
+        self.cumlweight = newcumlweight + np.log(self.decay)
 
     def get_proposal(self, x, xref, random):
         """Actual proposal function
         """
 
         xref = xref[0]
         nchain, npar = x.shape
```

### Comparing `dime_sampler-0.9.1/dime_sampler/test_all.py` & `dime_sampler-1.0.0/dime_sampler/test_all.py`

 * *Files identical despite different names*

### Comparing `dime_sampler-0.9.1/dime_sampler.egg-info/PKG-INFO` & `dime_sampler-1.0.0/dime_sampler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dime_sampler
-Version: 0.9.1
+Version: 1.0.0
 Summary: DIME MCMC sampling for python
 Home-page: https://github.com/gboehl/dime_sampler
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,20 +17,21 @@
 
 dime_sampler
 ============
 
 .. |badge0| image:: https://img.shields.io/badge/GitHub-gboehl%2Fdime__sampler-blue.svg?style=flat
     :target: https://github.com/gboehl/dime_sampler
 .. |badge1| image:: https://github.com/gboehl/dime_sampler/actions/workflows/continuous-integration.yml/badge.svg
-    :target: https://github.com/gboehl/dime_sampler/actions/workflows/continuous-integration.yml
+    :target: https://github.com/gboehl/dime_sampler/actions/workflows
 .. |badge2| image:: https://readthedocs.org/projects/dime-sampler/badge/?version=latest
-    :target: https://dime-sampler.readthedocs.io/en/latest/?badge=latest
+    :target: https://dime-sampler.readthedocs.io
     :alt: Documentation Status
 .. |badge3| image:: https://img.shields.io/pypi/v/dime_sampler
-   :alt: PyPI - Version
+    :target: https://pypi.org/project/dime-sampler/ 
+    :alt: PyPI - Version
 
 |badge0| |badge1| |badge2| |badge3|
 
 **Differential-Independence Mixture Ensemble ("DIME") MCMC sampling for Python** 
 
 This is the Python implementation of the DIME sampler proposed in `Ensemble MCMC Sampling for Robust Bayesian Inference <https://gregorboehl.com/live/dime_mcmc_boehl.pdf>`_ *(Gregor Boehl, 2022, SSRN No. 4250395)*. It provides the ``DIMEMove`` as a drop-in replacement for the great `emcee <https://github.com/dfm/emcee>`_ MCMC package.
```

### Comparing `dime_sampler-0.9.1/dime_sampler.egg-info/SOURCES.txt` & `dime_sampler-1.0.0/dime_sampler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dime_sampler-0.9.1/docs/.ipynb_checkpoints/hank_estimation-checkpoint.ipynb` & `dime_sampler-1.0.0/docs/.ipynb_checkpoints/hank_estimation-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `dime_sampler-0.9.1/docs/Makefile` & `dime_sampler-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dime_sampler-0.9.1/docs/conf.py` & `dime_sampler-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dime_sampler-0.9.1/docs/dist.png` & `dime_sampler-1.0.0/docs/dist.png`

 * *Files identical despite different names*

### Comparing `dime_sampler-0.9.1/docs/lprobs.png` & `dime_sampler-1.0.0/docs/lprobs.png`

 * *Files identical despite different names*

### Comparing `dime_sampler-0.9.1/docs/make.bat` & `dime_sampler-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dime_sampler-0.9.1/docs/traces.png` & `dime_sampler-1.0.0/docs/traces.png`

 * *Files identical despite different names*

### Comparing `dime_sampler-0.9.1/setup.py` & `dime_sampler-1.0.0/setup.py`

 * *Files identical despite different names*

