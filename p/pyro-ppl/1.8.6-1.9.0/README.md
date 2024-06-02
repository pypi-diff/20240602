# Comparing `tmp/pyro-ppl-1.8.6.tar.gz` & `tmp/pyro-ppl-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyro-ppl-1.8.6.tar", last modified: Sat Jul 29 21:08:19 2023, max compression
+gzip compressed data, was "pyro-ppl-1.9.0.tar", last modified: Mon Feb 19 18:03:18 2024, max compression
```

## Comparing `pyro-ppl-1.8.6.tar` & `pyro-ppl-1.9.0.tar`

### file list

```diff
@@ -1,374 +1,378 @@
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.253261 pyro-ppl-1.8.6/
--rw-r--r--   0 fritzo     (501) staff       (20)    11358 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/LICENSE.md
--rw-r--r--   0 fritzo     (501) staff       (20)       60 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/MANIFEST.in
--rw-r--r--   0 fritzo     (501) staff       (20)     4788 2023-07-29 21:08:19.253360 pyro-ppl-1.8.6/PKG-INFO
--rw-r--r--   0 fritzo     (501) staff       (20)     4538 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/README.md
--rw-r--r--   0 fritzo     (501) staff       (20)       81 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyproject.toml
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.191542 pyro-ppl-1.8.6/pyro/
--rw-r--r--   0 fritzo     (501) staff       (20)     1324 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)      113 2023-07-29 21:08:19.000000 pyro-ppl-1.8.6/pyro/_version.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.192378 pyro-ppl-1.8.6/pyro/contrib/
--rw-r--r--   0 fritzo     (501) staff       (20)      693 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)      317 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/autoguide.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.193067 pyro-ppl-1.8.6/pyro/contrib/autoname/
--rw-r--r--   0 fritzo     (501) staff       (20)      486 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/autoname/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5143 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/autoname/autoname.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8618 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/autoname/named.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6482 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/autoname/scoping.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.193425 pyro-ppl-1.8.6/pyro/contrib/bnn/
--rw-r--r--   0 fritzo     (501) staff       (20)      177 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/bnn/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5383 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/bnn/hidden_layer.py
--rw-r--r--   0 fritzo     (501) staff       (20)      490 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/bnn/utils.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.193539 pyro-ppl-1.8.6/pyro/contrib/cevae/
--rw-r--r--   0 fritzo     (501) staff       (20)    22960 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/cevae/__init__.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.193782 pyro-ppl-1.8.6/pyro/contrib/conjugate/
--rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/conjugate/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9073 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/conjugate/infer.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.194029 pyro-ppl-1.8.6/pyro/contrib/easyguide/
--rw-r--r--   0 fritzo     (501) staff       (20)      206 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/easyguide/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    12912 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/easyguide/easyguide.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.195178 pyro-ppl-1.8.6/pyro/contrib/epidemiology/
--rw-r--r--   0 fritzo     (501) staff       (20)      406 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/epidemiology/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    49835 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/epidemiology/compartmental.py
--rw-r--r--   0 fritzo     (501) staff       (20)    13549 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/epidemiology/distributions.py
--rw-r--r--   0 fritzo     (501) staff       (20)    51169 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/epidemiology/models.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10990 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/epidemiology/util.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.196474 pyro-ppl-1.8.6/pyro/contrib/examples/
--rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/examples/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6760 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/examples/bart.py
--rw-r--r--   0 fritzo     (501) staff       (20)      694 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/examples/finance.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2920 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/examples/multi_mnist.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1547 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/examples/nextstrain.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6875 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/examples/polyphonic_data_loader.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7442 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/examples/scanvi_data.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1556 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/examples/util.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.197159 pyro-ppl-1.8.6/pyro/contrib/forecast/
--rw-r--r--   0 fritzo     (501) staff       (20)      360 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/forecast/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8823 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/forecast/evaluate.py
--rw-r--r--   0 fritzo     (501) staff       (20)    23353 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/contrib/forecast/forecaster.py
--rw-r--r--   0 fritzo     (501) staff       (20)    16054 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/forecast/util.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.197285 pyro-ppl-1.8.6/pyro/contrib/funsor/
--rw-r--r--   0 fritzo     (501) staff       (20)     1223 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/__init__.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.198662 pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/
--rw-r--r--   0 fritzo     (501) staff       (20)      912 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9727 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/enum_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7623 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/named_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)    15224 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/plate_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1076 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/primitives.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1804 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/replay_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8558 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/runtime.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3632 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/trace_messenger.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.199389 pyro-ppl-1.8.6/pyro/contrib/funsor/infer/
--rw-r--r--   0 fritzo     (501) staff       (20)      514 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/infer/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2921 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/infer/discrete.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1652 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/infer/elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1698 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/infer/trace_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)    12663 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/infer/traceenum_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1882 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/infer/tracetmc_elbo.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.199851 pyro-ppl-1.8.6/pyro/contrib/gp/
--rw-r--r--   0 fritzo     (501) staff       (20)      340 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/__init__.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.201189 pyro-ppl-1.8.6/pyro/contrib/gp/kernels/
--rw-r--r--   0 fritzo     (501) staff       (20)     1533 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/kernels/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1577 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/kernels/brownian.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3699 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/kernels/coregionalize.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2646 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/kernels/dot_product.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5740 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/kernels/isotropic.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8446 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/kernels/kernel.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2424 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/kernels/periodic.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1536 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/kernels/static.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.202035 pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/
--rw-r--r--   0 fritzo     (501) staff       (20)      897 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1988 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/binary.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1677 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/gaussian.py
--rw-r--r--   0 fritzo     (501) staff       (20)      875 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/likelihood.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2859 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/multi_class.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1884 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/poisson.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.204359 pyro-ppl-1.8.6/pyro/contrib/gp/models/
--rw-r--r--   0 fritzo     (501) staff       (20)      546 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/models/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3897 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/models/gplvm.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8932 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/models/gpr.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9145 2022-05-12 17:23:25.000000 pyro-ppl-1.8.6/pyro/contrib/gp/models/model.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11001 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/gp/models/sgpr.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6859 2022-05-12 17:23:25.000000 pyro-ppl-1.8.6/pyro/contrib/gp/models/vgp.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8417 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/models/vsgp.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8058 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/parameterized.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7152 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/util.py
--rw-r--r--   0 fritzo     (501) staff       (20)    15591 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/minipyro.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.205290 pyro-ppl-1.8.6/pyro/contrib/mue/
--rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/mue/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6063 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/mue/dataloaders.py
--rw-r--r--   0 fritzo     (501) staff       (20)    13358 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/mue/missingdatahmm.py
--rw-r--r--   0 fritzo     (501) staff       (20)    34329 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/mue/models.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9017 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/mue/statearrangers.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.207638 pyro-ppl-1.8.6/pyro/contrib/oed/
--rw-r--r--   0 fritzo     (501) staff       (20)     3789 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/oed/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    44795 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/oed/eig.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.208062 pyro-ppl-1.8.6/pyro/contrib/oed/glmm/
--rw-r--r--   0 fritzo     (501) staff       (20)     1551 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/oed/glmm/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    16376 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/oed/glmm/glmm.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11368 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/oed/glmm/guides.py
--rw-r--r--   0 fritzo     (501) staff       (20)      867 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/oed/search.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1230 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/oed/util.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.208419 pyro-ppl-1.8.6/pyro/contrib/randomvariable/
--rw-r--r--   0 fritzo     (501) staff       (20)      193 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/randomvariable/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5424 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/randomvariable/random_variable.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.209095 pyro-ppl-1.8.6/pyro/contrib/timeseries/
--rw-r--r--   0 fritzo     (501) staff       (20)      711 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/timeseries/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2211 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/timeseries/base.py
--rw-r--r--   0 fritzo     (501) staff       (20)    23486 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/timeseries/gp.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6439 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/timeseries/lgssm.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11250 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/timeseries/lgssmgp.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.210262 pyro-ppl-1.8.6/pyro/contrib/tracking/
--rw-r--r--   0 fritzo     (501) staff       (20)      167 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/tracking/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    19243 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/tracking/assignment.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3576 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/tracking/distributions.py
--rw-r--r--   0 fritzo     (501) staff       (20)    16560 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/tracking/dynamic_models.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7796 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/tracking/extended_kalman_filter.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7266 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/tracking/hashing.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4544 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/tracking/measurements.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2800 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/util.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.218750 pyro-ppl-1.8.6/pyro/distributions/
--rw-r--r--   0 fritzo     (501) staff       (20)     5548 2023-01-03 22:31:38.000000 pyro-ppl-1.8.6/pyro/distributions/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3985 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/affine_beta.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7393 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/asymmetriclaplace.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4062 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/avf_mvn.py
--rw-r--r--   0 fritzo     (501) staff       (20)    20914 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/coalescent.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4815 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/distributions/conditional.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10824 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/conjugate.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4352 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/distributions/constraints.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3066 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/delta.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10356 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/distributions/diag_normal_mixture.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9012 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/distributions/diag_normal_mixture_shared_cov.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8443 2022-04-10 23:10:00.000000 pyro-ppl-1.8.6/pyro/distributions/distribution.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6765 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/empirical.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1885 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/extended.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1290 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/folded.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7983 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/gaussian_scale_mixture.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6571 2023-01-03 22:31:38.000000 pyro-ppl-1.8.6/pyro/distributions/grouped_normal_normal.py
--rw-r--r--   0 fritzo     (501) staff       (20)    54250 2023-01-13 02:07:01.000000 pyro-ppl-1.8.6/pyro/distributions/hmm.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2448 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/improper_uniform.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1429 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/inverse_gamma.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1661 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/kl.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2533 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/lkj.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5719 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/log_normal_negative_binomial.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5474 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/logistic.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6150 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/mixture.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5193 2022-06-12 12:50:39.000000 pyro-ppl-1.8.6/pyro/distributions/multivariate_studentt.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3381 2022-07-16 22:52:12.000000 pyro-ppl-1.8.6/pyro/distributions/nanmasked.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3176 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/omt_mvn.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6881 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/one_one_matching.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8360 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/one_two_matching.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2874 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/ordered_logistic.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3090 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/polya_gamma.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7441 2022-05-12 17:23:25.000000 pyro-ppl-1.8.6/pyro/distributions/projected_normal.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2933 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/rejector.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3637 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/relaxed_straight_through.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1125 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/score_parts.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11563 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/distributions/sine_bivariate_von_mises.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7318 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/sine_skewed.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2471 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/softlaplace.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7746 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/spanning_tree.cpp
--rw-r--r--   0 fritzo     (501) staff       (20)    22257 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/spanning_tree.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8208 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/stable.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.220022 pyro-ppl-1.8.6/pyro/distributions/testing/
--rw-r--r--   0 fritzo     (501) staff       (20)      215 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/testing/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)      421 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/testing/fakes.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10761 2022-07-10 14:38:43.000000 pyro-ppl-1.8.6/pyro/distributions/testing/gof.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1598 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/testing/naive_dirichlet.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1167 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/testing/rejection_exponential.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8842 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/testing/rejection_gamma.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3610 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/testing/special.py
--rw-r--r--   0 fritzo     (501) staff       (20)    14028 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/distributions/torch.py
--rw-r--r--   0 fritzo     (501) staff       (20)    20332 2022-10-02 18:17:50.000000 pyro-ppl-1.8.6/pyro/distributions/torch_distribution.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3044 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/distributions/torch_patch.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1452 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/distributions/torch_transform.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.224482 pyro-ppl-1.8.6/pyro/distributions/transforms/
--rw-r--r--   0 fritzo     (501) staff       (20)     6835 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    16342 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/affine_autoregressive.py
--rw-r--r--   0 fritzo     (501) staff       (20)    15805 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/affine_coupling.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2075 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/basic.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6147 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/batchnorm.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11702 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/block_autoregressive.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2115 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/cholesky.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3383 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/discrete_cosine.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11680 2022-11-22 19:06:49.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/generalized_channel_permute.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2883 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/haar.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10536 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/householder.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2479 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/lower_cholesky_affine.py
--rw-r--r--   0 fritzo     (501) staff       (20)    13725 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/matrix_exponential.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9794 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/neural_autoregressive.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1072 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/normalize.py
--rw-r--r--   0 fritzo     (501) staff       (20)      921 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/ordered.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5299 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/permute.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8881 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/planar.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7076 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/polynomial.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2138 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/power.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8711 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/radial.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1664 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/softplus.py
--rw-r--r--   0 fritzo     (501) staff       (20)    24458 2022-10-30 02:11:10.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/spline.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11370 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/spline_autoregressive.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6917 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/spline_coupling.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6318 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/sylvester.py
--rw-r--r--   0 fritzo     (501) staff       (20)      809 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/unit_cholesky.py
--rw-r--r--   0 fritzo     (501) staff       (20)      282 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/utils.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1886 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/unit.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11913 2022-11-06 16:58:27.000000 pyro-ppl-1.8.6/pyro/distributions/util.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2694 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/von_mises_3d.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6861 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/zero_inflated.py
--rw-r--r--   0 fritzo     (501) staff       (20)      266 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/generic.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.228735 pyro-ppl-1.8.6/pyro/infer/
--rw-r--r--   0 fritzo     (501) staff       (20)     2041 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    15986 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/abstract_infer.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.230463 pyro-ppl-1.8.6/pyro/infer/autoguide/
--rw-r--r--   0 fritzo     (501) staff       (20)     1618 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/autoguide/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    19662 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/autoguide/effect.py
--rw-r--r--   0 fritzo     (501) staff       (20)    26014 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/autoguide/gaussian.py
--rw-r--r--   0 fritzo     (501) staff       (20)    49205 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/infer/autoguide/guides.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8270 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/autoguide/initialization.py
--rw-r--r--   0 fritzo     (501) staff       (20)    16327 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/autoguide/structured.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3089 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/autoguide/utils.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7251 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/csis.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11547 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/discrete.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9535 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/infer/elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10044 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/energy_distance.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8063 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/enum.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9701 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/importance.py
--rw-r--r--   0 fritzo     (501) staff       (20)    21777 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/infer/inspect.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.231907 pyro-ppl-1.8.6/pyro/infer/mcmc/
--rw-r--r--   0 fritzo     (501) staff       (20)      412 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/mcmc/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    23000 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/mcmc/adaptation.py
--rw-r--r--   0 fritzo     (501) staff       (20)    29191 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/mcmc/api.py
--rw-r--r--   0 fritzo     (501) staff       (20)    18829 2023-01-03 22:31:38.000000 pyro-ppl-1.8.6/pyro/infer/mcmc/hmc.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9270 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/mcmc/logger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2347 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/mcmc/mcmc_kernel.py
--rw-r--r--   0 fritzo     (501) staff       (20)    21893 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/mcmc/nuts.py
--rw-r--r--   0 fritzo     (501) staff       (20)    33005 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/infer/mcmc/util.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11083 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/predictive.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9418 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/renyi_elbo.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.234291 pyro-ppl-1.8.6/pyro/infer/reparam/
--rw-r--r--   0 fritzo     (501) staff       (20)     1239 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4315 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/conjugate.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2076 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/discrete_cosine.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1594 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/haar.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6406 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/hmm.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3812 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/loc_scale.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5549 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/neutra.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1697 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/projected_normal.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2627 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/reparam.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1869 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/softmax.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2642 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/split.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10231 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/stable.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7481 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/strategies.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4312 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/structured.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1477 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/studentt.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1789 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/transform.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3913 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/unit_jacobian.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5720 2022-10-02 18:17:50.000000 pyro-ppl-1.8.6/pyro/infer/resampler.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11084 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/rws.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8713 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/smcfilter.py
--rw-r--r--   0 fritzo     (501) staff       (20)    12959 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/svgd.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5947 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/svi.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10334 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/trace_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8302 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/infer/trace_mean_field_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10876 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/trace_mmd.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3367 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/trace_tail_adaptive_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)    23531 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/traceenum_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)    16980 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/infer/tracegraph_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8714 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/tracetmc_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)    12502 2022-11-06 16:58:27.000000 pyro-ppl-1.8.6/pyro/infer/util.py
--rw-r--r--   0 fritzo     (501) staff       (20)      463 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/logger.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.235081 pyro-ppl-1.8.6/pyro/nn/
--rw-r--r--   0 fritzo     (501) staff       (20)      602 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/nn/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    13697 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/nn/auto_reg_nn.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5124 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/nn/dense_nn.py
--rw-r--r--   0 fritzo     (501) staff       (20)    31542 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/nn/module.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.243248 pyro-ppl-1.8.6/pyro/ops/
--rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4306 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/arrowhead.py
--rw-r--r--   0 fritzo     (501) staff       (20)    22550 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/ops/contract.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3402 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/dual_averaging.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.245648 pyro-ppl-1.8.6/pyro/ops/einsum/
--rw-r--r--   0 fritzo     (501) staff       (20)     1486 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/einsum/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4971 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/einsum/adjoint.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2010 2022-10-02 18:17:50.000000 pyro-ppl-1.8.6/pyro/ops/einsum/torch_log.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1952 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/einsum/torch_map.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2234 2022-07-05 20:35:43.000000 pyro-ppl-1.8.6/pyro/ops/einsum/torch_marginal.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2736 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/einsum/torch_sample.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1901 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/einsum/util.py
--rw-r--r--   0 fritzo     (501) staff       (20)    17941 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/gamma_gaussian.py
--rw-r--r--   0 fritzo     (501) staff       (20)    28046 2022-10-30 17:11:32.000000 pyro-ppl-1.8.6/pyro/ops/gaussian.py
--rw-r--r--   0 fritzo     (501) staff       (20)      673 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/hessian.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7458 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/indexing.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5119 2023-01-03 22:31:38.000000 pyro-ppl-1.8.6/pyro/ops/integrator.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5970 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/jit.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3577 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/linalg.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9520 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/newton.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6350 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/packed.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5967 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/ops/provenance.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11388 2022-07-05 20:10:55.000000 pyro-ppl-1.8.6/pyro/ops/rings.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7050 2022-05-12 17:23:25.000000 pyro-ppl-1.8.6/pyro/ops/special.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6648 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/ssm_gp.py
--rw-r--r--   0 fritzo     (501) staff       (20)    17109 2022-07-10 14:38:43.000000 pyro-ppl-1.8.6/pyro/ops/stats.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8903 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/streaming.py
--rw-r--r--   0 fritzo     (501) staff       (20)    15783 2022-11-06 16:58:27.000000 pyro-ppl-1.8.6/pyro/ops/tensor_utils.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3405 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/welford.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.246942 pyro-ppl-1.8.6/pyro/optim/
--rw-r--r--   0 fritzo     (501) staff       (20)      594 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/optim/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3060 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/optim/adagrad_rmsprop.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3462 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/optim/clipped_adam.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7634 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/optim/dct_adam.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1906 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/optim/horovod.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2351 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/optim/lr_scheduler.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6391 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/optim/multi.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10610 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/optim/optim.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2064 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/optim/pytorch_optimizers.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.247218 pyro-ppl-1.8.6/pyro/params/
--rw-r--r--   0 fritzo     (501) staff       (20)      317 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/params/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    13144 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/params/param_store.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.251620 pyro-ppl-1.8.6/pyro/poutine/
--rw-r--r--   0 fritzo     (501) staff       (20)      922 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/poutine/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4794 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/poutine/block_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3528 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/broadcast_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6129 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/collapse_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2128 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/condition_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3152 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/poutine/do_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9671 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/poutine/enum_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1228 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/escape_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5427 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/poutine/guide.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8605 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/poutine/handlers.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3849 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/indep_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1744 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/infer_config_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4830 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/lift_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3139 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/markov_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1239 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/mask_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8689 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/poutine/messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2794 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/plate_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)      664 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/reentrant_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5393 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/reparam_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2982 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/replay_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10402 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/poutine/runtime.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1824 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/scale_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1047 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/seed_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7725 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/poutine/subsample_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2935 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/poutine/substitute_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6891 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/poutine/trace_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)    20794 2023-07-24 22:31:37.000000 pyro-ppl-1.8.6/pyro/poutine/trace_struct.py
--rw-r--r--   0 fritzo     (501) staff       (20)      821 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/uncondition_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4073 2022-11-06 16:58:27.000000 pyro-ppl-1.8.6/pyro/poutine/util.py
--rw-r--r--   0 fritzo     (501) staff       (20)    23173 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/primitives.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5019 2022-11-06 16:58:27.000000 pyro-ppl-1.8.6/pyro/settings.py
--rw-r--r--   0 fritzo     (501) staff       (20)    22051 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/util.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.252156 pyro-ppl-1.8.6/pyro_ppl.egg-info/
--rw-r--r--   0 fritzo     (501) staff       (20)     4788 2023-07-29 21:08:19.000000 pyro-ppl-1.8.6/pyro_ppl.egg-info/PKG-INFO
--rw-r--r--   0 fritzo     (501) staff       (20)    10720 2023-07-29 21:08:19.000000 pyro-ppl-1.8.6/pyro_ppl.egg-info/SOURCES.txt
--rw-r--r--   0 fritzo     (501) staff       (20)        1 2023-07-29 21:08:19.000000 pyro-ppl-1.8.6/pyro_ppl.egg-info/dependency_links.txt
--rw-r--r--   0 fritzo     (501) staff       (20)      900 2023-07-29 21:08:19.000000 pyro-ppl-1.8.6/pyro_ppl.egg-info/requires.txt
--rw-r--r--   0 fritzo     (501) staff       (20)        5 2023-07-29 21:08:19.000000 pyro-ppl-1.8.6/pyro_ppl.egg-info/top_level.txt
--rw-r--r--   0 fritzo     (501) staff       (20)     1986 2023-07-29 21:08:19.253974 pyro-ppl-1.8.6/setup.cfg
--rw-r--r--   0 fritzo     (501) staff       (20)     5096 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/setup.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.253150 pyro-ppl-1.8.6/tests/
--rw-r--r--   0 fritzo     (501) staff       (20)    21987 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/tests/test_examples.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3354 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/tests/test_generic.py
--rw-r--r--   0 fritzo     (501) staff       (20)      740 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/tests/test_primitives.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1420 2022-11-06 16:58:27.000000 pyro-ppl-1.8.6/tests/test_settings.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3150 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.620567 pyro-ppl-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-02-19 18:03:18.620567 pyro-ppl-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.560567 pyro-ppl-1.9.0/pyro/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-19 18:03:18.000000 pyro-ppl-1.9.0/pyro/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.560567 pyro-ppl-1.9.0/pyro/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/autoguide.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.560567 pyro-ppl-1.9.0/pyro/contrib/autoname/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/autoname/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/autoname/autoname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/autoname/named.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/autoname/scoping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.560567 pyro-ppl-1.9.0/pyro/contrib/bnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/bnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/bnn/hidden_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/bnn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.560567 pyro-ppl-1.9.0/pyro/contrib/cevae/
+-rw-r--r--   0 runner    (1001) docker     (127)    23079 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/cevae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.560567 pyro-ppl-1.9.0/pyro/contrib/conjugate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/conjugate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/conjugate/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.564568 pyro-ppl-1.9.0/pyro/contrib/easyguide/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/easyguide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/easyguide/easyguide.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.564568 pyro-ppl-1.9.0/pyro/contrib/epidemiology/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/epidemiology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49835 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/epidemiology/compartmental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13549 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/epidemiology/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51217 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/epidemiology/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/epidemiology/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.564568 pyro-ppl-1.9.0/pyro/contrib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/examples/bart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/examples/finance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/examples/multi_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/examples/nextstrain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/examples/polyphonic_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/examples/scanvi_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/examples/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.564568 pyro-ppl-1.9.0/pyro/contrib/forecast/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/forecast/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23353 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/forecast/forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16054 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/forecast/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.564568 pyro-ppl-1.9.0/pyro/contrib/funsor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/funsor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.568568 pyro-ppl-1.9.0/pyro/contrib/funsor/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/funsor/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/funsor/handlers/enum_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/funsor/handlers/named_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15224 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/funsor/handlers/plate_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/funsor/handlers/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/funsor/handlers/replay_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8558 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/funsor/handlers/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/funsor/handlers/trace_messenger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.568568 pyro-ppl-1.9.0/pyro/contrib/funsor/infer/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/funsor/infer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/funsor/infer/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/funsor/infer/elbo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/funsor/infer/trace_elbo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12731 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/funsor/infer/traceenum_elbo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/funsor/infer/tracetmc_elbo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.568568 pyro-ppl-1.9.0/pyro/contrib/gp/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.568568 pyro-ppl-1.9.0/pyro/contrib/gp/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/kernels/brownian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/kernels/coregionalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/kernels/dot_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/kernels/isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/kernels/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/kernels/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/kernels/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.572568 pyro-ppl-1.9.0/pyro/contrib/gp/likelihoods/
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/likelihoods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/likelihoods/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/likelihoods/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/likelihoods/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/likelihoods/multi_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/likelihoods/poisson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.572568 pyro-ppl-1.9.0/pyro/contrib/gp/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/models/gplvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/models/gpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/models/sgpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/models/vgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/models/vsgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/parameterized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/gp/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15591 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/minipyro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.572568 pyro-ppl-1.9.0/pyro/contrib/mue/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/mue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/mue/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/mue/missingdatahmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34329 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/mue/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/mue/statearrangers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.572568 pyro-ppl-1.9.0/pyro/contrib/oed/
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/oed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44795 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/oed/eig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.576568 pyro-ppl-1.9.0/pyro/contrib/oed/glmm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/oed/glmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/oed/glmm/glmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/oed/glmm/guides.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/oed/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/oed/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.576568 pyro-ppl-1.9.0/pyro/contrib/randomvariable/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/randomvariable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/randomvariable/random_variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.576568 pyro-ppl-1.9.0/pyro/contrib/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/timeseries/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23486 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/timeseries/gp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/timeseries/lgssm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11260 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/timeseries/lgssmgp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.576568 pyro-ppl-1.9.0/pyro/contrib/tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/tracking/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/tracking/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16560 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/tracking/dynamic_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/tracking/extended_kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/tracking/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/tracking/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/contrib/zuko.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.584567 pyro-ppl-1.9.0/pyro/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/affine_beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/asymmetriclaplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/avf_mvn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20914 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/coalescent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/conjugate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10433 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/diag_normal_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/diag_normal_mixture_shared_cov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/empirical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/folded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/gaussian_scale_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/grouped_normal_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54251 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/hmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/improper_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/inverse_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/kl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/lkj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/log_normal_negative_binomial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/logistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/multivariate_studentt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/nanmasked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/omt_mvn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/one_one_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/one_two_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/ordered_logistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/polya_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/projected_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/rejector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/relaxed_straight_through.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/score_parts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/sine_bivariate_von_mises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/sine_skewed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/softlaplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/spanning_tree.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    22257 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/spanning_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/stable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.588567 pyro-ppl-1.9.0/pyro/distributions/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/testing/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/testing/gof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/testing/naive_dirichlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/testing/rejection_exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/testing/rejection_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/testing/special.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14222 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20865 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/torch_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/torch_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/torch_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.592567 pyro-ppl-1.9.0/pyro/distributions/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16342 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/affine_autoregressive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15805 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/affine_coupling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11703 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/block_autoregressive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/discrete_cosine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11680 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/generalized_channel_permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/haar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/householder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/lower_cholesky_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13725 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/matrix_exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/neural_autoregressive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/ordered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/planar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/power.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8711 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/radial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/simplex_to_ordered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/softplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24458 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/spline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/spline_autoregressive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/spline_coupling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/sylvester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/unit_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11913 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/von_mises_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/distributions/zero_inflated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.596567 pyro-ppl-1.9.0/pyro/infer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15986 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/abstract_infer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.596567 pyro-ppl-1.9.0/pyro/infer/autoguide/
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/autoguide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19652 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/autoguide/effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26016 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/autoguide/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49204 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/autoguide/guides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/autoguide/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16327 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/autoguide/structured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/autoguide/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/csis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11547 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/elbo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/energy_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/importance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23990 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.596567 pyro-ppl-1.9.0/pyro/infer/mcmc/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/mcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23000 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/mcmc/adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29278 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/mcmc/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18829 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/mcmc/hmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9270 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/mcmc/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/mcmc/mcmc_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21893 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/mcmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/mcmc/rwkernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33005 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/mcmc/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11083 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/predictive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/renyi_elbo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.600567 pyro-ppl-1.9.0/pyro/infer/reparam/
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/reparam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/reparam/conjugate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/reparam/discrete_cosine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/reparam/haar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/reparam/hmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/reparam/loc_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/reparam/neutra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/reparam/projected_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/reparam/reparam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/reparam/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/reparam/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/reparam/stable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/reparam/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/reparam/structured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/reparam/studentt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/reparam/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/reparam/unit_jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/resampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11140 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/rws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/smcfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12959 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/svgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/svi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/trace_elbo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/trace_mean_field_elbo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/trace_mmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/trace_tail_adaptive_elbo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23531 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/traceenum_elbo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16980 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/tracegraph_elbo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8714 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/tracetmc_elbo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12502 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/infer/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.600567 pyro-ppl-1.9.0/pyro/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13697 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/nn/auto_reg_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/nn/dense_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35110 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/nn/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.604567 pyro-ppl-1.9.0/pyro/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/arrowhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22550 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/dual_averaging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.604567 pyro-ppl-1.9.0/pyro/ops/einsum/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/einsum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/einsum/adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/einsum/torch_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/einsum/torch_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/einsum/torch_marginal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/einsum/torch_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/einsum/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17941 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/gamma_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28119 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/hessian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/newton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/packed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/rings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/special.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/ssm_gp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17109 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8903 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15783 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/ops/welford.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.608567 pyro-ppl-1.9.0/pyro/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/optim/adagrad_rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/optim/clipped_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/optim/dct_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/optim/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/optim/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/optim/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10610 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/optim/optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/optim/pytorch_optimizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.608567 pyro-ppl-1.9.0/pyro/params/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/params/param_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.612567 pyro-ppl-1.9.0/pyro/poutine/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/block_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/broadcast_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/collapse_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/condition_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/do_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/enum_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/escape_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/guide.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/indep_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/infer_config_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/lift_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/markov_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/mask_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9474 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/plate_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/reentrant_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/reparam_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/replay_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16602 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/scale_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/seed_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/subsample_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/substitute_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7695 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/trace_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22785 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/trace_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/uncondition_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/poutine/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24368 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22051 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/pyro/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.612567 pyro-ppl-1.9.0/pyro_ppl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-02-19 18:03:18.000000 pyro-ppl-1.9.0/pyro_ppl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-02-19 18:03:18.000000 pyro-ppl-1.9.0/pyro_ppl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 18:03:18.000000 pyro-ppl-1.9.0/pyro_ppl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-19 18:03:18.000000 pyro-ppl-1.9.0/pyro_ppl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-19 18:03:18.000000 pyro-ppl-1.9.0/pyro_ppl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-02-19 18:03:18.620567 pyro-ppl-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:03:18.612567 pyro-ppl-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    22086 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/tests/test_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-02-19 18:03:09.000000 pyro-ppl-1.9.0/tests/test_util.py
```

### Comparing `pyro-ppl-1.8.6/LICENSE.md` & `pyro-ppl-1.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/PKG-INFO` & `pyro-ppl-1.9.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,300 +1,284 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 726f  : 2.1.Name: pyro
-00000020: 2d70 706c 0a56 6572 7369 6f6e 3a20 312e  -ppl.Version: 1.
-00000030: 382e 360a 5375 6d6d 6172 793a 2041 2050  8.6.Summary: A P
-00000040: 7974 686f 6e20 6c69 6272 6172 7920 666f  ython library fo
-00000050: 7220 7072 6f62 6162 696c 6973 7469 6320  r probabilistic 
-00000060: 6d6f 6465 6c69 6e67 2061 6e64 2069 6e66  modeling and inf
-00000070: 6572 656e 6365 0a48 6f6d 652d 7061 6765  erence.Home-page
-00000080: 3a20 6874 7470 3a2f 2f70 7972 6f2e 6169  : http://pyro.ai
-00000090: 0a41 7574 686f 723a 2055 6265 7220 4149  .Author: Uber AI
-000000a0: 204c 6162 730a 4c69 6365 6e73 653a 2041   Labs.License: A
-000000b0: 7061 6368 6520 322e 300a 5072 6f6a 6563  pache 2.0.Projec
-000000c0: 742d 5552 4c3a 2044 6f63 756d 656e 7461  t-URL: Documenta
-000000d0: 7469 6f6e 2c20 6874 7470 733a 2f2f 646f  tion, https://do
-000000e0: 6373 2e70 7972 6f2e 6169 0a50 726f 6a65  cs.pyro.ai.Proje
-000000f0: 6374 2d55 524c 3a20 536f 7572 6365 2c20  ct-URL: Source, 
-00000100: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000110: 6f6d 2f70 7972 6f2d 7070 6c2f 7079 726f  om/pyro-ppl/pyro
-00000120: 0a4b 6579 776f 7264 733a 206d 6163 6869  .Keywords: machi
-00000130: 6e65 206c 6561 726e 696e 6720 7374 6174  ne learning stat
-00000140: 6973 7469 6373 2070 726f 6261 6269 6c69  istics probabili
-00000150: 7374 6963 2070 726f 6772 616d 6d69 6e67  stic programming
-00000160: 2062 6179 6573 6961 6e20 6d6f 6465 6c69   bayesian modeli
-00000170: 6e67 2070 7974 6f72 6368 0a50 6c61 7466  ng pytorch.Platf
-00000180: 6f72 6d3a 2055 4e4b 4e4f 574e 0a43 6c61  orm: UNKNOWN.Cla
-00000190: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
-000001a0: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
-000001b0: 7665 6c6f 7065 7273 0a43 6c61 7373 6966  velopers.Classif
-000001c0: 6965 723a 2049 6e74 656e 6465 6420 4175  ier: Intended Au
-000001d0: 6469 656e 6365 203a 3a20 4564 7563 6174  dience :: Educat
-000001e0: 696f 6e0a 436c 6173 7369 6669 6572 3a20  ion.Classifier: 
-000001f0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
-00000200: 6520 3a3a 2053 6369 656e 6365 2f52 6573  e :: Science/Res
-00000210: 6561 7263 680a 436c 6173 7369 6669 6572  earch.Classifier
-00000220: 3a20 4c69 6365 6e73 6520 3a3a 204f 5349  : License :: OSI
-00000230: 2041 7070 726f 7665 6420 3a3a 2041 7061   Approved :: Apa
-00000240: 6368 6520 536f 6674 7761 7265 204c 6963  che Software Lic
-00000250: 656e 7365 0a43 6c61 7373 6966 6965 723a  ense.Classifier:
-00000260: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
-00000270: 6d20 3a3a 2050 4f53 4958 203a 3a20 4c69  m :: POSIX :: Li
-00000280: 6e75 780a 436c 6173 7369 6669 6572 3a20  nux.Classifier: 
-00000290: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-000002a0: 203a 3a20 4d61 634f 5320 3a3a 204d 6163   :: MacOS :: Mac
-000002b0: 4f53 2058 0a43 6c61 7373 6966 6965 723a  OS X.Classifier:
-000002c0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000002d0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000002e0: 3a3a 2033 2e37 0a43 6c61 7373 6966 6965  :: 3.7.Classifie
-000002f0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000300: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000310: 6e20 3a3a 2033 2e38 0a43 6c61 7373 6966  n :: 3.8.Classif
-00000320: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000330: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000340: 686f 6e20 3a3a 2033 2e39 0a52 6571 7569  hon :: 3.9.Requi
-00000350: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
-00000360: 370a 4465 7363 7269 7074 696f 6e2d 436f  7.Description-Co
-00000370: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
-00000380: 2f6d 6172 6b64 6f77 6e0a 5072 6f76 6964  /markdown.Provid
-00000390: 6573 2d45 7874 7261 3a20 6578 7472 6173  es-Extra: extras
-000003a0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-000003b0: 2074 6573 740a 5072 6f76 6964 6573 2d45   test.Provides-E
-000003c0: 7874 7261 3a20 7072 6f66 696c 650a 5072  xtra: profile.Pr
-000003d0: 6f76 6964 6573 2d45 7874 7261 3a20 6465  ovides-Extra: de
-000003e0: 760a 5072 6f76 6964 6573 2d45 7874 7261  v.Provides-Extra
-000003f0: 3a20 686f 726f 766f 640a 5072 6f76 6964  : horovod.Provid
-00000400: 6573 2d45 7874 7261 3a20 6c69 6768 746e  es-Extra: lightn
-00000410: 696e 670a 5072 6f76 6964 6573 2d45 7874  ing.Provides-Ext
-00000420: 7261 3a20 6675 6e73 6f72 0a4c 6963 656e  ra: funsor.Licen
-00000430: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-00000440: 2e6d 640a 0a5b 4765 7474 696e 6720 5374  .md..[Getting St
-00000450: 6172 7465 645d 2868 7474 703a 2f2f 7079  arted](http://py
-00000460: 726f 2e61 692f 6578 616d 706c 6573 2920  ro.ai/examples) 
-00000470: 7c0a 5b44 6f63 756d 656e 7461 7469 6f6e  |.[Documentation
-00000480: 5d28 6874 7470 3a2f 2f64 6f63 732e 7079  ](http://docs.py
-00000490: 726f 2e61 692f 2920 7c0a 5b43 6f6d 6d75  ro.ai/) |.[Commu
-000004a0: 6e69 7479 5d28 6874 7470 3a2f 2f66 6f72  nity](http://for
-000004b0: 756d 2e70 7972 6f2e 6169 2f29 207c 0a5b  um.pyro.ai/) |.[
-000004c0: 436f 6e74 7269 6275 7469 6e67 5d28 6874  Contributing](ht
-000004d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000004e0: 2f70 7972 6f2d 7070 6c2f 7079 726f 2f62  /pyro-ppl/pyro/b
-000004f0: 6c6f 622f 6d61 7374 6572 2f43 4f4e 5452  lob/master/CONTR
-00000500: 4942 5554 494e 472e 6d64 290a 0a50 7972  IBUTING.md)..Pyr
-00000510: 6f20 6973 2061 2066 6c65 7869 626c 652c  o is a flexible,
-00000520: 2073 6361 6c61 626c 6520 6465 6570 2070   scalable deep p
-00000530: 726f 6261 6269 6c69 7374 6963 2070 726f  robabilistic pro
-00000540: 6772 616d 6d69 6e67 206c 6962 7261 7279  gramming library
-00000550: 2062 7569 6c74 206f 6e20 5079 546f 7263   built on PyTorc
-00000560: 682e 2020 4e6f 7461 626c 792c 2069 7420  h.  Notably, it 
-00000570: 7761 7320 6465 7369 676e 6564 2077 6974  was designed wit
-00000580: 6820 7468 6573 6520 7072 696e 6369 706c  h these principl
-00000590: 6573 2069 6e20 6d69 6e64 3a0a 0a2d 202a  es in mind:..- *
-000005a0: 2a55 6e69 7665 7273 616c 2a2a 3a20 5079  *Universal**: Py
-000005b0: 726f 2069 7320 6120 756e 6976 6572 7361  ro is a universa
-000005c0: 6c20 5050 4c20 2d20 6974 2063 616e 2072  l PPL - it can r
-000005d0: 6570 7265 7365 6e74 2061 6e79 2063 6f6d  epresent any com
-000005e0: 7075 7461 626c 6520 7072 6f62 6162 696c  putable probabil
-000005f0: 6974 7920 6469 7374 7269 6275 7469 6f6e  ity distribution
-00000600: 2e0a 2d20 2a2a 5363 616c 6162 6c65 2a2a  ..- **Scalable**
-00000610: 3a20 5079 726f 2073 6361 6c65 7320 746f  : Pyro scales to
-00000620: 206c 6172 6765 2064 6174 6120 7365 7473   large data sets
-00000630: 2077 6974 6820 6c69 7474 6c65 206f 7665   with little ove
-00000640: 7268 6561 6420 636f 6d70 6172 6564 2074  rhead compared t
-00000650: 6f20 6861 6e64 2d77 7269 7474 656e 2063  o hand-written c
-00000660: 6f64 652e 0a2d 202a 2a4d 696e 696d 616c  ode..- **Minimal
-00000670: 2a2a 3a20 5079 726f 2069 7320 6167 696c  **: Pyro is agil
-00000680: 6520 616e 6420 6d61 696e 7461 696e 6162  e and maintainab
-00000690: 6c65 2e20 4974 2069 7320 696d 706c 656d  le. It is implem
-000006a0: 656e 7465 6420 7769 7468 2061 2073 6d61  ented with a sma
-000006b0: 6c6c 2063 6f72 6520 6f66 2070 6f77 6572  ll core of power
-000006c0: 6675 6c2c 2063 6f6d 706f 7361 626c 6520  ful, composable 
-000006d0: 6162 7374 7261 6374 696f 6e73 2e0a 2d20  abstractions..- 
-000006e0: 2a2a 466c 6578 6962 6c65 2a2a 3a20 5079  **Flexible**: Py
-000006f0: 726f 2061 696d 7320 666f 7220 6175 746f  ro aims for auto
-00000700: 6d61 7469 6f6e 2077 6865 6e20 796f 7520  mation when you 
-00000710: 7761 6e74 2069 742c 2063 6f6e 7472 6f6c  want it, control
-00000720: 2077 6865 6e20 796f 7520 6e65 6564 2069   when you need i
-00000730: 742e 2054 6869 7320 6973 2061 6363 6f6d  t. This is accom
-00000740: 706c 6973 6865 6420 7468 726f 7567 6820  plished through 
-00000750: 6869 6768 2d6c 6576 656c 2061 6273 7472  high-level abstr
-00000760: 6163 7469 6f6e 7320 746f 2065 7870 7265  actions to expre
-00000770: 7373 2067 656e 6572 6174 6976 6520 616e  ss generative an
-00000780: 6420 696e 6665 7265 6e63 6520 6d6f 6465  d inference mode
-00000790: 6c73 2c20 7768 696c 6520 616c 6c6f 7769  ls, while allowi
-000007a0: 6e67 2065 7870 6572 7473 2065 6173 792d  ng experts easy-
-000007b0: 6163 6365 7373 2074 6f20 6375 7374 6f6d  access to custom
-000007c0: 697a 6520 696e 6665 7265 6e63 652e 0a0a  ize inference...
-000007d0: 5079 726f 2077 6173 206f 7269 6769 6e61  Pyro was origina
-000007e0: 6c6c 7920 6465 7665 6c6f 7065 6420 6174  lly developed at
-000007f0: 2055 6265 7220 4149 2061 6e64 2069 7320   Uber AI and is 
-00000800: 6e6f 7720 6163 7469 7665 6c79 206d 6169  now actively mai
-00000810: 6e74 6169 6e65 6420 6279 2063 6f6d 6d75  ntained by commu
-00000820: 6e69 7479 2063 6f6e 7472 6962 7574 6f72  nity contributor
-00000830: 732c 2069 6e63 6c75 6469 6e67 2061 2064  s, including a d
-00000840: 6564 6963 6174 6564 2074 6561 6d20 6174  edicated team at
-00000850: 2074 6865 205b 4272 6f61 6420 496e 7374   the [Broad Inst
-00000860: 6974 7574 655d 2868 7474 7073 3a2f 2f77  itute](https://w
-00000870: 7777 2e62 726f 6164 696e 7374 6974 7574  ww.broadinstitut
-00000880: 652e 6f72 672f 292e 0a49 6e20 3230 3139  e.org/)..In 2019
-00000890: 2c20 5079 726f 205b 6265 6361 6d65 5d28  , Pyro [became](
-000008a0: 6874 7470 733a 2f2f 7777 772e 6c69 6e75  https://www.linu
-000008b0: 7866 6f75 6e64 6174 696f 6e2e 6f72 672f  xfoundation.org/
-000008c0: 7072 6573 732d 7265 6c65 6173 652f 3230  press-release/20
-000008d0: 3139 2f30 322f 7079 726f 2d70 726f 6261  19/02/pyro-proba
-000008e0: 6269 6c69 7374 6963 2d70 726f 6772 616d  bilistic-program
-000008f0: 6d69 6e67 2d6c 616e 6775 6167 652d 6265  ming-language-be
-00000900: 636f 6d65 732d 6e65 7765 7374 2d6c 662d  comes-newest-lf-
-00000910: 6465 6570 2d6c 6561 726e 696e 672d 7072  deep-learning-pr
-00000920: 6f6a 6563 742f 2920 6120 7072 6f6a 6563  oject/) a projec
-00000930: 7420 6f66 2074 6865 204c 696e 7578 2046  t of the Linux F
-00000940: 6f75 6e64 6174 696f 6e2c 2061 206e 6575  oundation, a neu
-00000950: 7472 616c 2073 7061 6365 2066 6f72 2063  tral space for c
-00000960: 6f6c 6c61 626f 7261 7469 6f6e 206f 6e20  ollaboration on 
-00000970: 6f70 656e 2073 6f75 7263 6520 736f 6674  open source soft
-00000980: 7761 7265 2c20 6f70 656e 2073 7461 6e64  ware, open stand
-00000990: 6172 6473 2c20 6f70 656e 2064 6174 612c  ards, open data,
-000009a0: 2061 6e64 206f 7065 6e20 6861 7264 7761   and open hardwa
-000009b0: 7265 2e0a 0a46 6f72 206d 6f72 6520 696e  re...For more in
-000009c0: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
-000009d0: 7468 6520 6869 6768 206c 6576 656c 206d  the high level m
-000009e0: 6f74 6976 6174 696f 6e20 666f 7220 5079  otivation for Py
-000009f0: 726f 2c20 6368 6563 6b20 6f75 7420 6f75  ro, check out ou
-00000a00: 7220 5b6c 6175 6e63 6820 626c 6f67 2070  r [launch blog p
-00000a10: 6f73 745d 2868 7474 703a 2f2f 656e 672e  ost](http://eng.
-00000a20: 7562 6572 2e63 6f6d 2f70 7972 6f29 2e0a  uber.com/pyro)..
-00000a30: 466f 7220 6164 6469 7469 6f6e 616c 2062  For additional b
-00000a40: 6c6f 6720 706f 7374 732c 2063 6865 636b  log posts, check
-00000a50: 206f 7574 2077 6f72 6b20 6f6e 205b 6578   out work on [ex
-00000a60: 7065 7269 6d65 6e74 616c 2064 6573 6967  perimental desig
-00000a70: 6e5d 2868 7474 7073 3a2f 2f65 6e67 2e75  n](https://eng.u
-00000a80: 6265 722e 636f 6d2f 6f65 642d 7079 726f  ber.com/oed-pyro
-00000a90: 2d72 656c 6561 7365 2f29 2061 6e64 0a5b  -release/) and.[
-00000aa0: 7469 6d65 2d74 6f2d 6576 656e 7420 6d6f  time-to-event mo
-00000ab0: 6465 6c69 6e67 5d28 6874 7470 733a 2f2f  deling](https://
-00000ac0: 656e 672e 7562 6572 2e63 6f6d 2f6d 6f64  eng.uber.com/mod
-00000ad0: 656c 696e 672d 6365 6e73 6f72 6564 2d74  eling-censored-t
-00000ae0: 696d 652d 746f 2d65 7665 6e74 2d64 6174  ime-to-event-dat
-00000af0: 612d 7573 696e 672d 7079 726f 2f29 2069  a-using-pyro/) i
-00000b00: 6e20 5079 726f 2e0a 0a23 2320 496e 7374  n Pyro...## Inst
-00000b10: 616c 6c69 6e67 0a0a 2323 2320 496e 7374  alling..### Inst
-00000b20: 616c 6c69 6e67 2061 2073 7461 626c 6520  alling a stable 
-00000b30: 5079 726f 2072 656c 6561 7365 0a0a 2a2a  Pyro release..**
-00000b40: 496e 7374 616c 6c20 7573 696e 6720 7069  Install using pi
-00000b50: 703a 2a2a 0a60 6060 7368 0a70 6970 2069  p:**.```sh.pip i
-00000b60: 6e73 7461 6c6c 2070 7972 6f2d 7070 6c0a  nstall pyro-ppl.
-00000b70: 6060 600a 0a2a 2a49 6e73 7461 6c6c 2066  ```..**Install f
-00000b80: 726f 6d20 736f 7572 6365 3a2a 2a0a 6060  rom source:**.``
-00000b90: 6073 680a 6769 7420 636c 6f6e 6520 6769  `sh.git clone gi
-00000ba0: 7440 6769 7468 7562 2e63 6f6d 3a70 7972  t@github.com:pyr
-00000bb0: 6f2d 7070 6c2f 7079 726f 2e67 6974 0a63  o-ppl/pyro.git.c
-00000bc0: 6420 7079 726f 0a67 6974 2063 6865 636b  d pyro.git check
-00000bd0: 6f75 7420 6d61 7374 6572 2020 2320 6d61  out master  # ma
-00000be0: 7374 6572 2069 7320 7069 6e6e 6564 2074  ster is pinned t
-00000bf0: 6f20 7468 6520 6c61 7465 7374 2072 656c  o the latest rel
-00000c00: 6561 7365 0a70 6970 2069 6e73 7461 6c6c  ease.pip install
-00000c10: 202e 0a60 6060 0a0a 2a2a 496e 7374 616c   ..```..**Instal
-00000c20: 6c20 7769 7468 2065 7874 7261 2070 6163  l with extra pac
-00000c30: 6b61 6765 733a 2a2a 0a0a 546f 2069 6e73  kages:**..To ins
-00000c40: 7461 6c6c 2074 6865 2064 6570 656e 6465  tall the depende
-00000c50: 6e63 6965 7320 7265 7175 6972 6564 2074  ncies required t
-00000c60: 6f20 7275 6e20 7468 6520 7072 6f62 6162  o run the probab
-00000c70: 696c 6973 7469 6320 6d6f 6465 6c73 2069  ilistic models i
-00000c80: 6e63 6c75 6465 6420 696e 2074 6865 2060  ncluded in the `
-00000c90: 6578 616d 706c 6573 602f 6074 7574 6f72  examples`/`tutor
-00000ca0: 6961 6c73 6020 6469 7265 6374 6f72 6965  ials` directorie
-00000cb0: 732c 2070 6c65 6173 6520 7573 6520 7468  s, please use th
-00000cc0: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
-00000cd0: 616e 643a 0a60 6060 7368 0a70 6970 2069  and:.```sh.pip i
-00000ce0: 6e73 7461 6c6c 2070 7972 6f2d 7070 6c5b  nstall pyro-ppl[
-00000cf0: 6578 7472 6173 5d20 0a60 6060 0a4d 616b  extras] .```.Mak
-00000d00: 6520 7375 7265 2074 6861 7420 7468 6520  e sure that the 
-00000d10: 6d6f 6465 6c73 2063 6f6d 6520 6672 6f6d  models come from
-00000d20: 2074 6865 2073 616d 6520 7265 6c65 6173   the same releas
-00000d30: 6520 7665 7273 696f 6e20 6f66 2074 6865  e version of the
-00000d40: 205b 5079 726f 2073 6f75 7263 6520 636f   [Pyro source co
-00000d50: 6465 5d28 6874 7470 733a 2f2f 6769 7468  de](https://gith
-00000d60: 7562 2e63 6f6d 2f70 7972 6f2d 7070 6c2f  ub.com/pyro-ppl/
-00000d70: 7079 726f 2f72 656c 6561 7365 7329 2061  pyro/releases) a
-00000d80: 7320 796f 7520 6861 7665 2069 6e73 7461  s you have insta
-00000d90: 6c6c 6564 2e0a 0a23 2323 2049 6e73 7461  lled...### Insta
-00000da0: 6c6c 696e 6720 5079 726f 2064 6576 2062  lling Pyro dev b
-00000db0: 7261 6e63 680a 0a46 6f72 2072 6563 656e  ranch..For recen
-00000dc0: 7420 6665 6174 7572 6573 2079 6f75 2063  t features you c
-00000dd0: 616e 2069 6e73 7461 6c6c 2050 7972 6f20  an install Pyro 
-00000de0: 6672 6f6d 2073 6f75 7263 652e 0a0a 2a2a  from source...**
-00000df0: 496e 7374 616c 6c20 5079 726f 2075 7369  Install Pyro usi
-00000e00: 6e67 2070 6970 3a2a 2a0a 0a60 6060 7368  ng pip:**..```sh
-00000e10: 0a70 6970 2069 6e73 7461 6c6c 2067 6974  .pip install git
-00000e20: 2b68 7474 7073 3a2f 2f67 6974 6875 622e  +https://github.
-00000e30: 636f 6d2f 7079 726f 2d70 706c 2f70 7972  com/pyro-ppl/pyr
-00000e40: 6f2e 6769 740a 6060 600a 6f72 2c20 7769  o.git.```.or, wi
-00000e50: 7468 2074 6865 2060 6578 7472 6173 6020  th the `extras` 
-00000e60: 6465 7065 6e64 656e 6379 2074 6f20 7275  dependency to ru
-00000e70: 6e20 7468 6520 7072 6f62 6162 696c 6973  n the probabilis
-00000e80: 7469 6320 6d6f 6465 6c73 2069 6e63 6c75  tic models inclu
-00000e90: 6465 6420 696e 2074 6865 2060 6578 616d  ded in the `exam
-00000ea0: 706c 6573 602f 6074 7574 6f72 6961 6c73  ples`/`tutorials
-00000eb0: 6020 6469 7265 6374 6f72 6965 733a 0a60  ` directories:.`
-00000ec0: 6060 7368 0a70 6970 2069 6e73 7461 6c6c  ``sh.pip install
-00000ed0: 2067 6974 2b68 7474 7073 3a2f 2f67 6974   git+https://git
-00000ee0: 6875 622e 636f 6d2f 7079 726f 2d70 706c  hub.com/pyro-ppl
-00000ef0: 2f70 7972 6f2e 6769 7423 6567 673d 7072  /pyro.git#egg=pr
-00000f00: 6f6a 6563 745b 6578 7472 6173 5d0a 6060  oject[extras].``
-00000f10: 600a 0a2a 2a49 6e73 7461 6c6c 2050 7972  `..**Install Pyr
-00000f20: 6f20 6672 6f6d 2073 6f75 7263 653a 2a2a  o from source:**
-00000f30: 0a0a 6060 6073 680a 6769 7420 636c 6f6e  ..```sh.git clon
-00000f40: 6520 6874 7470 733a 2f2f 6769 7468 7562  e https://github
-00000f50: 2e63 6f6d 2f70 7972 6f2d 7070 6c2f 7079  .com/pyro-ppl/py
-00000f60: 726f 0a63 6420 7079 726f 0a70 6970 2069  ro.cd pyro.pip i
-00000f70: 6e73 7461 6c6c 202e 2020 2320 7069 7020  nstall .  # pip 
-00000f80: 696e 7374 616c 6c20 2e5b 6578 7472 6173  install .[extras
-00000f90: 5d20 666f 7220 7275 6e6e 696e 6720 6d6f  ] for running mo
-00000fa0: 6465 6c73 2069 6e20 6578 616d 706c 6573  dels in examples
-00000fb0: 2f74 7574 6f72 6961 6c73 0a60 6060 0a0a  /tutorials.```..
-00000fc0: 2323 2052 756e 6e69 6e67 2050 7972 6f20  ## Running Pyro 
-00000fd0: 6672 6f6d 2061 2044 6f63 6b65 7220 436f  from a Docker Co
-00000fe0: 6e74 6169 6e65 720a 0a52 6566 6572 2074  ntainer..Refer t
-00000ff0: 6f20 7468 6520 696e 7374 7275 6374 696f  o the instructio
-00001000: 6e73 205b 6865 7265 5d28 646f 636b 6572  ns [here](docker
-00001010: 2f52 4541 444d 452e 6d64 292e 0a0a 2323  /README.md)...##
-00001020: 2043 6974 6174 696f 6e0a 4966 2079 6f75   Citation.If you
-00001030: 2075 7365 2050 7972 6f2c 2070 6c65 6173   use Pyro, pleas
-00001040: 6520 636f 6e73 6964 6572 2063 6974 696e  e consider citin
-00001050: 673a 0a60 6060 0a40 6172 7469 636c 657b  g:.```.@article{
-00001060: 6269 6e67 6861 6d32 3031 3970 7972 6f2c  bingham2019pyro,
-00001070: 0a20 2061 7574 686f 7220 2020 203d 207b  .  author    = {
-00001080: 456c 6920 4269 6e67 6861 6d20 616e 640a  Eli Bingham and.
-00001090: 2020 2020 2020 2020 2020 2020 2020 204a                 J
-000010a0: 6f6e 6174 6861 6e20 502e 2043 6865 6e20  onathan P. Chen 
-000010b0: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-000010c0: 2020 204d 6172 7469 6e20 4a61 6e6b 6f77     Martin Jankow
-000010d0: 6961 6b20 616e 640a 2020 2020 2020 2020  iak and.        
-000010e0: 2020 2020 2020 2046 7269 747a 204f 6265         Fritz Obe
-000010f0: 726d 6579 6572 2061 6e64 0a20 2020 2020  rmeyer and.     
-00001100: 2020 2020 2020 2020 2020 4e65 6572 616a            Neeraj
-00001110: 2050 7261 6468 616e 2061 6e64 0a20 2020   Pradhan and.   
-00001120: 2020 2020 2020 2020 2020 2020 5468 656f              Theo
-00001130: 6661 6e69 7320 4b61 7261 6c65 7473 6f73  fanis Karaletsos
-00001140: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-00001150: 2020 2020 526f 6869 7420 5369 6e67 6820      Rohit Singh 
-00001160: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-00001170: 2020 2050 6175 6c20 412e 2053 7a65 726c     Paul A. Szerl
-00001180: 6970 2061 6e64 0a20 2020 2020 2020 2020  ip and.         
-00001190: 2020 2020 2020 5061 756c 2048 6f72 7366        Paul Horsf
-000011a0: 616c 6c20 616e 640a 2020 2020 2020 2020  all and.        
-000011b0: 2020 2020 2020 204e 6f61 6820 442e 2047         Noah D. G
-000011c0: 6f6f 646d 616e 7d2c 0a20 2074 6974 6c65  oodman},.  title
-000011d0: 2020 2020 203d 207b 5079 726f 3a20 4465       = {Pyro: De
-000011e0: 6570 2055 6e69 7665 7273 616c 2050 726f  ep Universal Pro
-000011f0: 6261 6269 6c69 7374 6963 2050 726f 6772  babilistic Progr
-00001200: 616d 6d69 6e67 7d2c 0a20 206a 6f75 726e  amming},.  journ
-00001210: 616c 2020 203d 207b 4a2e 204d 6163 682e  al   = {J. Mach.
-00001220: 204c 6561 726e 2e20 5265 732e 7d2c 0a20   Learn. Res.},. 
-00001230: 2076 6f6c 756d 6520 2020 203d 207b 3230   volume    = {20
-00001240: 7d2c 0a20 2070 6167 6573 2020 2020 203d  },.  pages     =
-00001250: 207b 3238 3a31 2d2d 3238 3a36 7d2c 0a20   {28:1--28:6},. 
-00001260: 2079 6561 7220 2020 2020 203d 207b 3230   year      = {20
-00001270: 3139 7d2c 0a20 2075 726c 2020 2020 2020  19},.  url      
-00001280: 203d 207b 6874 7470 3a2f 2f6a 6d6c 722e   = {http://jmlr.
-00001290: 6f72 672f 7061 7065 7273 2f76 3230 2f31  org/papers/v20/1
-000012a0: 382d 3430 332e 6874 6d6c 7d0a 7d0a 6060  8-403.html}.}.``
-000012b0: 600a 0a0a                                `...
+00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000010: 6572 223e 0a20 203c 6120 6872 6566 3d22  er">.  <a href="
+00000020: 6874 7470 3a2f 2f70 7972 6f2e 6169 223e  http://pyro.ai">
+00000030: 203c 696d 6720 7769 6474 683d 2232 3230   <img width="220
+00000040: 7078 2220 6865 6967 6874 3d22 3232 3070  px" height="220p
+00000050: 7822 2073 7263 3d22 646f 6373 2f73 6f75  x" src="docs/sou
+00000060: 7263 652f 5f73 7461 7469 632f 696d 672f  rce/_static/img/
+00000070: 7079 726f 5f6c 6f67 6f5f 7769 7468 5f74  pyro_logo_with_t
+00000080: 6578 742e 706e 6722 3e3c 2f61 3e0a 3c2f  ext.png"></a>.</
+00000090: 6469 763e 0a0a 2d2d 2d2d 2d2d 2d2d 2d2d  div>..----------
+000000a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000000b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+000000c0: 0a5b 215b 4275 696c 6420 5374 6174 7573  .[![Build Status
+000000d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000000e0: 2e63 6f6d 2f70 7972 6f2d 7070 6c2f 7079  .com/pyro-ppl/py
+000000f0: 726f 2f77 6f72 6b66 6c6f 7773 2f43 492f  ro/workflows/CI/
+00000100: 6261 6467 652e 7376 6729 5d28 6874 7470  badge.svg)](http
+00000110: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+00000120: 7972 6f2d 7070 6c2f 7079 726f 2f61 6374  yro-ppl/pyro/act
+00000130: 696f 6e73 290a 5b21 5b43 6f76 6572 6167  ions).[![Coverag
+00000140: 6520 5374 6174 7573 5d28 6874 7470 733a  e Status](https:
+00000150: 2f2f 636f 7665 7261 6c6c 732e 696f 2f72  //coveralls.io/r
+00000160: 6570 6f73 2f67 6974 6875 622f 7079 726f  epos/github/pyro
+00000170: 2d70 706c 2f70 7972 6f2f 6261 6467 652e  -ppl/pyro/badge.
+00000180: 7376 673f 6272 616e 6368 3d64 6576 295d  svg?branch=dev)]
+00000190: 2868 7474 7073 3a2f 2f63 6f76 6572 616c  (https://coveral
+000001a0: 6c73 2e69 6f2f 6769 7468 7562 2f70 7972  ls.io/github/pyr
+000001b0: 6f2d 7070 6c2f 7079 726f 3f62 7261 6e63  o-ppl/pyro?branc
+000001c0: 683d 6465 7629 0a5b 215b 4c61 7465 7374  h=dev).[![Latest
+000001d0: 2056 6572 7369 6f6e 5d28 6874 7470 733a   Version](https:
+000001e0: 2f2f 6261 6467 652e 6675 7279 2e69 6f2f  //badge.fury.io/
+000001f0: 7079 2f70 7972 6f2d 7070 6c2e 7376 6729  py/pyro-ppl.svg)
+00000200: 5d28 6874 7470 733a 2f2f 7079 7069 2e70  ](https://pypi.p
+00000210: 7974 686f 6e2e 6f72 672f 7079 7069 2f70  ython.org/pypi/p
+00000220: 7972 6f2d 7070 6c29 0a5b 215b 446f 6375  yro-ppl).[![Docu
+00000230: 6d65 6e74 6174 696f 6e20 5374 6174 7573  mentation Status
+00000240: 5d28 6874 7470 733a 2f2f 7265 6164 7468  ](https://readth
+00000250: 6564 6f63 732e 6f72 672f 7072 6f6a 6563  edocs.org/projec
+00000260: 7473 2f70 7972 6f2d 7070 6c2f 6261 6467  ts/pyro-ppl/badg
+00000270: 652f 3f76 6572 7369 6f6e 3d64 6576 295d  e/?version=dev)]
+00000280: 2868 7474 703a 2f2f 7079 726f 2d70 706c  (http://pyro-ppl
+00000290: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+000002a0: 656e 2f73 7461 626c 652f 3f62 6164 6765  en/stable/?badge
+000002b0: 3d64 6576 290a 5b21 5b43 4949 2042 6573  =dev).[![CII Bes
+000002c0: 7420 5072 6163 7469 6365 735d 2868 7474  t Practices](htt
+000002d0: 7073 3a2f 2f62 6573 7470 7261 6374 6963  ps://bestpractic
+000002e0: 6573 2e63 6f72 6569 6e66 7261 7374 7275  es.coreinfrastru
+000002f0: 6374 7572 652e 6f72 672f 7072 6f6a 6563  cture.org/projec
+00000300: 7473 2f33 3035 362f 6261 6467 6529 5d28  ts/3056/badge)](
+00000310: 6874 7470 733a 2f2f 6265 7374 7072 6163  https://bestprac
+00000320: 7469 6365 732e 636f 7265 696e 6672 6173  tices.coreinfras
+00000330: 7472 7563 7475 7265 2e6f 7267 2f70 726f  tructure.org/pro
+00000340: 6a65 6374 732f 3330 3536 290a 0a5b 4765  jects/3056)..[Ge
+00000350: 7474 696e 6720 5374 6172 7465 645d 2868  tting Started](h
+00000360: 7474 703a 2f2f 7079 726f 2e61 692f 6578  ttp://pyro.ai/ex
+00000370: 616d 706c 6573 2920 7c0a 5b44 6f63 756d  amples) |.[Docum
+00000380: 656e 7461 7469 6f6e 5d28 6874 7470 3a2f  entation](http:/
+00000390: 2f64 6f63 732e 7079 726f 2e61 692f 2920  /docs.pyro.ai/) 
+000003a0: 7c0a 5b43 6f6d 6d75 6e69 7479 5d28 6874  |.[Community](ht
+000003b0: 7470 3a2f 2f66 6f72 756d 2e70 7972 6f2e  tp://forum.pyro.
+000003c0: 6169 2f29 207c 0a5b 436f 6e74 7269 6275  ai/) |.[Contribu
+000003d0: 7469 6e67 5d28 6874 7470 733a 2f2f 6769  ting](https://gi
+000003e0: 7468 7562 2e63 6f6d 2f70 7972 6f2d 7070  thub.com/pyro-pp
+000003f0: 6c2f 7079 726f 2f62 6c6f 622f 6d61 7374  l/pyro/blob/mast
+00000400: 6572 2f43 4f4e 5452 4942 5554 494e 472e  er/CONTRIBUTING.
+00000410: 6d64 290a 0a50 7972 6f20 6973 2061 2066  md)..Pyro is a f
+00000420: 6c65 7869 626c 652c 2073 6361 6c61 626c  lexible, scalabl
+00000430: 6520 6465 6570 2070 726f 6261 6269 6c69  e deep probabili
+00000440: 7374 6963 2070 726f 6772 616d 6d69 6e67  stic programming
+00000450: 206c 6962 7261 7279 2062 7569 6c74 206f   library built o
+00000460: 6e20 5079 546f 7263 682e 2020 4e6f 7461  n PyTorch.  Nota
+00000470: 626c 792c 2069 7420 7761 7320 6465 7369  bly, it was desi
+00000480: 676e 6564 2077 6974 6820 7468 6573 6520  gned with these 
+00000490: 7072 696e 6369 706c 6573 2069 6e20 6d69  principles in mi
+000004a0: 6e64 3a0a 0a2d 202a 2a55 6e69 7665 7273  nd:..- **Univers
+000004b0: 616c 2a2a 3a20 5079 726f 2069 7320 6120  al**: Pyro is a 
+000004c0: 756e 6976 6572 7361 6c20 5050 4c20 2d20  universal PPL - 
+000004d0: 6974 2063 616e 2072 6570 7265 7365 6e74  it can represent
+000004e0: 2061 6e79 2063 6f6d 7075 7461 626c 6520   any computable 
+000004f0: 7072 6f62 6162 696c 6974 7920 6469 7374  probability dist
+00000500: 7269 6275 7469 6f6e 2e0a 2d20 2a2a 5363  ribution..- **Sc
+00000510: 616c 6162 6c65 2a2a 3a20 5079 726f 2073  alable**: Pyro s
+00000520: 6361 6c65 7320 746f 206c 6172 6765 2064  cales to large d
+00000530: 6174 6120 7365 7473 2077 6974 6820 6c69  ata sets with li
+00000540: 7474 6c65 206f 7665 7268 6561 6420 636f  ttle overhead co
+00000550: 6d70 6172 6564 2074 6f20 6861 6e64 2d77  mpared to hand-w
+00000560: 7269 7474 656e 2063 6f64 652e 0a2d 202a  ritten code..- *
+00000570: 2a4d 696e 696d 616c 2a2a 3a20 5079 726f  *Minimal**: Pyro
+00000580: 2069 7320 6167 696c 6520 616e 6420 6d61   is agile and ma
+00000590: 696e 7461 696e 6162 6c65 2e20 4974 2069  intainable. It i
+000005a0: 7320 696d 706c 656d 656e 7465 6420 7769  s implemented wi
+000005b0: 7468 2061 2073 6d61 6c6c 2063 6f72 6520  th a small core 
+000005c0: 6f66 2070 6f77 6572 6675 6c2c 2063 6f6d  of powerful, com
+000005d0: 706f 7361 626c 6520 6162 7374 7261 6374  posable abstract
+000005e0: 696f 6e73 2e0a 2d20 2a2a 466c 6578 6962  ions..- **Flexib
+000005f0: 6c65 2a2a 3a20 5079 726f 2061 696d 7320  le**: Pyro aims 
+00000600: 666f 7220 6175 746f 6d61 7469 6f6e 2077  for automation w
+00000610: 6865 6e20 796f 7520 7761 6e74 2069 742c  hen you want it,
+00000620: 2063 6f6e 7472 6f6c 2077 6865 6e20 796f   control when yo
+00000630: 7520 6e65 6564 2069 742e 2054 6869 7320  u need it. This 
+00000640: 6973 2061 6363 6f6d 706c 6973 6865 6420  is accomplished 
+00000650: 7468 726f 7567 6820 6869 6768 2d6c 6576  through high-lev
+00000660: 656c 2061 6273 7472 6163 7469 6f6e 7320  el abstractions 
+00000670: 746f 2065 7870 7265 7373 2067 656e 6572  to express gener
+00000680: 6174 6976 6520 616e 6420 696e 6665 7265  ative and infere
+00000690: 6e63 6520 6d6f 6465 6c73 2c20 7768 696c  nce models, whil
+000006a0: 6520 616c 6c6f 7769 6e67 2065 7870 6572  e allowing exper
+000006b0: 7473 2065 6173 792d 6163 6365 7373 2074  ts easy-access t
+000006c0: 6f20 6375 7374 6f6d 697a 6520 696e 6665  o customize infe
+000006d0: 7265 6e63 652e 0a0a 5079 726f 2077 6173  rence...Pyro was
+000006e0: 206f 7269 6769 6e61 6c6c 7920 6465 7665   originally deve
+000006f0: 6c6f 7065 6420 6174 2055 6265 7220 4149  loped at Uber AI
+00000700: 2061 6e64 2069 7320 6e6f 7720 6163 7469   and is now acti
+00000710: 7665 6c79 206d 6169 6e74 6169 6e65 6420  vely maintained 
+00000720: 6279 2063 6f6d 6d75 6e69 7479 2063 6f6e  by community con
+00000730: 7472 6962 7574 6f72 732c 2069 6e63 6c75  tributors, inclu
+00000740: 6469 6e67 2061 2064 6564 6963 6174 6564  ding a dedicated
+00000750: 2074 6561 6d20 6174 2074 6865 205b 4272   team at the [Br
+00000760: 6f61 6420 496e 7374 6974 7574 655d 2868  oad Institute](h
+00000770: 7474 7073 3a2f 2f77 7777 2e62 726f 6164  ttps://www.broad
+00000780: 696e 7374 6974 7574 652e 6f72 672f 292e  institute.org/).
+00000790: 0a49 6e20 3230 3139 2c20 5079 726f 205b  .In 2019, Pyro [
+000007a0: 6265 6361 6d65 5d28 6874 7470 733a 2f2f  became](https://
+000007b0: 7777 772e 6c69 6e75 7866 6f75 6e64 6174  www.linuxfoundat
+000007c0: 696f 6e2e 6f72 672f 7072 6573 732d 7265  ion.org/press-re
+000007d0: 6c65 6173 652f 3230 3139 2f30 322f 7079  lease/2019/02/py
+000007e0: 726f 2d70 726f 6261 6269 6c69 7374 6963  ro-probabilistic
+000007f0: 2d70 726f 6772 616d 6d69 6e67 2d6c 616e  -programming-lan
+00000800: 6775 6167 652d 6265 636f 6d65 732d 6e65  guage-becomes-ne
+00000810: 7765 7374 2d6c 662d 6465 6570 2d6c 6561  west-lf-deep-lea
+00000820: 726e 696e 672d 7072 6f6a 6563 742f 2920  rning-project/) 
+00000830: 6120 7072 6f6a 6563 7420 6f66 2074 6865  a project of the
+00000840: 204c 696e 7578 2046 6f75 6e64 6174 696f   Linux Foundatio
+00000850: 6e2c 2061 206e 6575 7472 616c 2073 7061  n, a neutral spa
+00000860: 6365 2066 6f72 2063 6f6c 6c61 626f 7261  ce for collabora
+00000870: 7469 6f6e 206f 6e20 6f70 656e 2073 6f75  tion on open sou
+00000880: 7263 6520 736f 6674 7761 7265 2c20 6f70  rce software, op
+00000890: 656e 2073 7461 6e64 6172 6473 2c20 6f70  en standards, op
+000008a0: 656e 2064 6174 612c 2061 6e64 206f 7065  en data, and ope
+000008b0: 6e20 6861 7264 7761 7265 2e0a 0a46 6f72  n hardware...For
+000008c0: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
+000008d0: 6e20 6162 6f75 7420 7468 6520 6869 6768  n about the high
+000008e0: 206c 6576 656c 206d 6f74 6976 6174 696f   level motivatio
+000008f0: 6e20 666f 7220 5079 726f 2c20 6368 6563  n for Pyro, chec
+00000900: 6b20 6f75 7420 6f75 7220 5b6c 6175 6e63  k out our [launc
+00000910: 6820 626c 6f67 2070 6f73 745d 2868 7474  h blog post](htt
+00000920: 703a 2f2f 656e 672e 7562 6572 2e63 6f6d  p://eng.uber.com
+00000930: 2f70 7972 6f29 2e0a 466f 7220 6164 6469  /pyro)..For addi
+00000940: 7469 6f6e 616c 2062 6c6f 6720 706f 7374  tional blog post
+00000950: 732c 2063 6865 636b 206f 7574 2077 6f72  s, check out wor
+00000960: 6b20 6f6e 205b 6578 7065 7269 6d65 6e74  k on [experiment
+00000970: 616c 2064 6573 6967 6e5d 2868 7474 7073  al design](https
+00000980: 3a2f 2f65 6e67 2e75 6265 722e 636f 6d2f  ://eng.uber.com/
+00000990: 6f65 642d 7079 726f 2d72 656c 6561 7365  oed-pyro-release
+000009a0: 2f29 2061 6e64 0a5b 7469 6d65 2d74 6f2d  /) and.[time-to-
+000009b0: 6576 656e 7420 6d6f 6465 6c69 6e67 5d28  event modeling](
+000009c0: 6874 7470 733a 2f2f 656e 672e 7562 6572  https://eng.uber
+000009d0: 2e63 6f6d 2f6d 6f64 656c 696e 672d 6365  .com/modeling-ce
+000009e0: 6e73 6f72 6564 2d74 696d 652d 746f 2d65  nsored-time-to-e
+000009f0: 7665 6e74 2d64 6174 612d 7573 696e 672d  vent-data-using-
+00000a00: 7079 726f 2f29 2069 6e20 5079 726f 2e0a  pyro/) in Pyro..
+00000a10: 0a23 2320 496e 7374 616c 6c69 6e67 0a0a  .## Installing..
+00000a20: 2323 2320 496e 7374 616c 6c69 6e67 2061  ### Installing a
+00000a30: 2073 7461 626c 6520 5079 726f 2072 656c   stable Pyro rel
+00000a40: 6561 7365 0a0a 2a2a 496e 7374 616c 6c20  ease..**Install 
+00000a50: 7573 696e 6720 7069 703a 2a2a 0a60 6060  using pip:**.```
+00000a60: 7368 0a70 6970 2069 6e73 7461 6c6c 2070  sh.pip install p
+00000a70: 7972 6f2d 7070 6c0a 6060 600a 0a2a 2a49  yro-ppl.```..**I
+00000a80: 6e73 7461 6c6c 2066 726f 6d20 736f 7572  nstall from sour
+00000a90: 6365 3a2a 2a0a 6060 6073 680a 6769 7420  ce:**.```sh.git 
+00000aa0: 636c 6f6e 6520 6769 7440 6769 7468 7562  clone git@github
+00000ab0: 2e63 6f6d 3a70 7972 6f2d 7070 6c2f 7079  .com:pyro-ppl/py
+00000ac0: 726f 2e67 6974 0a63 6420 7079 726f 0a67  ro.git.cd pyro.g
+00000ad0: 6974 2063 6865 636b 6f75 7420 6d61 7374  it checkout mast
+00000ae0: 6572 2020 2320 6d61 7374 6572 2069 7320  er  # master is 
+00000af0: 7069 6e6e 6564 2074 6f20 7468 6520 6c61  pinned to the la
+00000b00: 7465 7374 2072 656c 6561 7365 0a70 6970  test release.pip
+00000b10: 2069 6e73 7461 6c6c 202e 0a60 6060 0a0a   install ..```..
+00000b20: 2a2a 496e 7374 616c 6c20 7769 7468 2065  **Install with e
+00000b30: 7874 7261 2070 6163 6b61 6765 733a 2a2a  xtra packages:**
+00000b40: 0a0a 546f 2069 6e73 7461 6c6c 2074 6865  ..To install the
+00000b50: 2064 6570 656e 6465 6e63 6965 7320 7265   dependencies re
+00000b60: 7175 6972 6564 2074 6f20 7275 6e20 7468  quired to run th
+00000b70: 6520 7072 6f62 6162 696c 6973 7469 6320  e probabilistic 
+00000b80: 6d6f 6465 6c73 2069 6e63 6c75 6465 6420  models included 
+00000b90: 696e 2074 6865 2060 6578 616d 706c 6573  in the `examples
+00000ba0: 602f 6074 7574 6f72 6961 6c73 6020 6469  `/`tutorials` di
+00000bb0: 7265 6374 6f72 6965 732c 2070 6c65 6173  rectories, pleas
+00000bc0: 6520 7573 6520 7468 6520 666f 6c6c 6f77  e use the follow
+00000bd0: 696e 6720 636f 6d6d 616e 643a 0a60 6060  ing command:.```
+00000be0: 7368 0a70 6970 2069 6e73 7461 6c6c 2070  sh.pip install p
+00000bf0: 7972 6f2d 7070 6c5b 6578 7472 6173 5d20  yro-ppl[extras] 
+00000c00: 0a60 6060 0a4d 616b 6520 7375 7265 2074  .```.Make sure t
+00000c10: 6861 7420 7468 6520 6d6f 6465 6c73 2063  hat the models c
+00000c20: 6f6d 6520 6672 6f6d 2074 6865 2073 616d  ome from the sam
+00000c30: 6520 7265 6c65 6173 6520 7665 7273 696f  e release versio
+00000c40: 6e20 6f66 2074 6865 205b 5079 726f 2073  n of the [Pyro s
+00000c50: 6f75 7263 6520 636f 6465 5d28 6874 7470  ource code](http
+00000c60: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+00000c70: 7972 6f2d 7070 6c2f 7079 726f 2f72 656c  yro-ppl/pyro/rel
+00000c80: 6561 7365 7329 2061 7320 796f 7520 6861  eases) as you ha
+00000c90: 7665 2069 6e73 7461 6c6c 6564 2e0a 0a23  ve installed...#
+00000ca0: 2323 2049 6e73 7461 6c6c 696e 6720 5079  ## Installing Py
+00000cb0: 726f 2064 6576 2062 7261 6e63 680a 0a46  ro dev branch..F
+00000cc0: 6f72 2072 6563 656e 7420 6665 6174 7572  or recent featur
+00000cd0: 6573 2079 6f75 2063 616e 2069 6e73 7461  es you can insta
+00000ce0: 6c6c 2050 7972 6f20 6672 6f6d 2073 6f75  ll Pyro from sou
+00000cf0: 7263 652e 0a0a 2a2a 496e 7374 616c 6c20  rce...**Install 
+00000d00: 5079 726f 2075 7369 6e67 2070 6970 3a2a  Pyro using pip:*
+00000d10: 2a0a 0a60 6060 7368 0a70 6970 2069 6e73  *..```sh.pip ins
+00000d20: 7461 6c6c 2067 6974 2b68 7474 7073 3a2f  tall git+https:/
+00000d30: 2f67 6974 6875 622e 636f 6d2f 7079 726f  /github.com/pyro
+00000d40: 2d70 706c 2f70 7972 6f2e 6769 740a 6060  -ppl/pyro.git.``
+00000d50: 600a 6f72 2c20 7769 7468 2074 6865 2060  `.or, with the `
+00000d60: 6578 7472 6173 6020 6465 7065 6e64 656e  extras` dependen
+00000d70: 6379 2074 6f20 7275 6e20 7468 6520 7072  cy to run the pr
+00000d80: 6f62 6162 696c 6973 7469 6320 6d6f 6465  obabilistic mode
+00000d90: 6c73 2069 6e63 6c75 6465 6420 696e 2074  ls included in t
+00000da0: 6865 2060 6578 616d 706c 6573 602f 6074  he `examples`/`t
+00000db0: 7574 6f72 6961 6c73 6020 6469 7265 6374  utorials` direct
+00000dc0: 6f72 6965 733a 0a60 6060 7368 0a70 6970  ories:.```sh.pip
+00000dd0: 2069 6e73 7461 6c6c 2067 6974 2b68 7474   install git+htt
+00000de0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000df0: 7079 726f 2d70 706c 2f70 7972 6f2e 6769  pyro-ppl/pyro.gi
+00000e00: 7423 6567 673d 7072 6f6a 6563 745b 6578  t#egg=project[ex
+00000e10: 7472 6173 5d0a 6060 600a 0a2a 2a49 6e73  tras].```..**Ins
+00000e20: 7461 6c6c 2050 7972 6f20 6672 6f6d 2073  tall Pyro from s
+00000e30: 6f75 7263 653a 2a2a 0a0a 6060 6073 680a  ource:**..```sh.
+00000e40: 6769 7420 636c 6f6e 6520 6874 7470 733a  git clone https:
+00000e50: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7972  //github.com/pyr
+00000e60: 6f2d 7070 6c2f 7079 726f 0a63 6420 7079  o-ppl/pyro.cd py
+00000e70: 726f 0a70 6970 2069 6e73 7461 6c6c 202e  ro.pip install .
+00000e80: 2020 2320 7069 7020 696e 7374 616c 6c20    # pip install 
+00000e90: 2e5b 6578 7472 6173 5d20 666f 7220 7275  .[extras] for ru
+00000ea0: 6e6e 696e 6720 6d6f 6465 6c73 2069 6e20  nning models in 
+00000eb0: 6578 616d 706c 6573 2f74 7574 6f72 6961  examples/tutoria
+00000ec0: 6c73 0a60 6060 0a0a 2323 2052 756e 6e69  ls.```..## Runni
+00000ed0: 6e67 2050 7972 6f20 6672 6f6d 2061 2044  ng Pyro from a D
+00000ee0: 6f63 6b65 7220 436f 6e74 6169 6e65 720a  ocker Container.
+00000ef0: 0a52 6566 6572 2074 6f20 7468 6520 696e  .Refer to the in
+00000f00: 7374 7275 6374 696f 6e73 205b 6865 7265  structions [here
+00000f10: 5d28 646f 636b 6572 2f52 4541 444d 452e  ](docker/README.
+00000f20: 6d64 292e 0a0a 2323 2043 6974 6174 696f  md)...## Citatio
+00000f30: 6e0a 4966 2079 6f75 2075 7365 2050 7972  n.If you use Pyr
+00000f40: 6f2c 2070 6c65 6173 6520 636f 6e73 6964  o, please consid
+00000f50: 6572 2063 6974 696e 673a 0a60 6060 0a40  er citing:.```.@
+00000f60: 6172 7469 636c 657b 6269 6e67 6861 6d32  article{bingham2
+00000f70: 3031 3970 7972 6f2c 0a20 2061 7574 686f  019pyro,.  autho
+00000f80: 7220 2020 203d 207b 456c 6920 4269 6e67  r    = {Eli Bing
+00000f90: 6861 6d20 616e 640a 2020 2020 2020 2020  ham and.        
+00000fa0: 2020 2020 2020 204a 6f6e 6174 6861 6e20         Jonathan 
+00000fb0: 502e 2043 6865 6e20 616e 640a 2020 2020  P. Chen and.    
+00000fc0: 2020 2020 2020 2020 2020 204d 6172 7469             Marti
+00000fd0: 6e20 4a61 6e6b 6f77 6961 6b20 616e 640a  n Jankowiak and.
+00000fe0: 2020 2020 2020 2020 2020 2020 2020 2046                 F
+00000ff0: 7269 747a 204f 6265 726d 6579 6572 2061  ritz Obermeyer a
+00001000: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
+00001010: 2020 4e65 6572 616a 2050 7261 6468 616e    Neeraj Pradhan
+00001020: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
+00001030: 2020 2020 5468 656f 6661 6e69 7320 4b61      Theofanis Ka
+00001040: 7261 6c65 7473 6f73 2061 6e64 0a20 2020  raletsos and.   
+00001050: 2020 2020 2020 2020 2020 2020 526f 6869              Rohi
+00001060: 7420 5369 6e67 6820 616e 640a 2020 2020  t Singh and.    
+00001070: 2020 2020 2020 2020 2020 2050 6175 6c20             Paul 
+00001080: 412e 2053 7a65 726c 6970 2061 6e64 0a20  A. Szerlip and. 
+00001090: 2020 2020 2020 2020 2020 2020 2020 5061                Pa
+000010a0: 756c 2048 6f72 7366 616c 6c20 616e 640a  ul Horsfall and.
+000010b0: 2020 2020 2020 2020 2020 2020 2020 204e                 N
+000010c0: 6f61 6820 442e 2047 6f6f 646d 616e 7d2c  oah D. Goodman},
+000010d0: 0a20 2074 6974 6c65 2020 2020 203d 207b  .  title     = {
+000010e0: 5079 726f 3a20 4465 6570 2055 6e69 7665  Pyro: Deep Unive
+000010f0: 7273 616c 2050 726f 6261 6269 6c69 7374  rsal Probabilist
+00001100: 6963 2050 726f 6772 616d 6d69 6e67 7d2c  ic Programming},
+00001110: 0a20 206a 6f75 726e 616c 2020 203d 207b  .  journal   = {
+00001120: 4a2e 204d 6163 682e 204c 6561 726e 2e20  J. Mach. Learn. 
+00001130: 5265 732e 7d2c 0a20 2076 6f6c 756d 6520  Res.},.  volume 
+00001140: 2020 203d 207b 3230 7d2c 0a20 2070 6167     = {20},.  pag
+00001150: 6573 2020 2020 203d 207b 3238 3a31 2d2d  es     = {28:1--
+00001160: 3238 3a36 7d2c 0a20 2079 6561 7220 2020  28:6},.  year   
+00001170: 2020 203d 207b 3230 3139 7d2c 0a20 2075     = {2019},.  u
+00001180: 726c 2020 2020 2020 203d 207b 6874 7470  rl       = {http
+00001190: 3a2f 2f6a 6d6c 722e 6f72 672f 7061 7065  ://jmlr.org/pape
+000011a0: 7273 2f76 3230 2f31 382d 3430 332e 6874  rs/v20/18-403.ht
+000011b0: 6d6c 7d0a 7d0a 6060 600a                 ml}.}.```.
```

### Comparing `pyro-ppl-1.8.6/pyro/__init__.py` & `pyro-ppl-1.9.0/pyro/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     validation_enabled,
 )
 from pyro.util import set_rng_seed
 
 from . import settings
 
 # After changing this, run scripts/update_version.py
-version_prefix = "1.8.6"
+version_prefix = "1.9.0"
 
 # Get the __version__ string from the auto-generated _version.py file, if exists.
 try:
     from pyro._version import __version__  # type: ignore
 except ImportError:
     __version__ = version_prefix
```

### Comparing `pyro-ppl-1.8.6/pyro/contrib/__init__.py` & `pyro-ppl-1.9.0/pyro/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/autoname/autoname.py` & `pyro-ppl-1.9.0/pyro/contrib/autoname/autoname.py`

 * *Files 6% similar despite different names*

```diff
@@ -149,17 +149,16 @@
         raw_name = msg["fn"](*msg["args"])
         fresh_name = _SCOPE_STACK.fresh_name(raw_name)
 
         msg["value"] = str(_SCOPE_STACK) + "/" + fresh_name
         msg["stop"] = True
 
 
-_handler_name, _handler = _make_handler(AutonameMessenger)
-_handler.__module__ = __name__
-locals()[_handler_name] = _handler
+@_make_handler(AutonameMessenger, __name__)
+def autoname(fn=None, name=None): ...
 
 
 @singledispatch
 def sample(*args):
     raise NotImplementedError
```

### Comparing `pyro-ppl-1.8.6/pyro/contrib/autoname/named.py` & `pyro-ppl-1.9.0/pyro/contrib/autoname/named.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/autoname/scoping.py` & `pyro-ppl-1.9.0/pyro/contrib/autoname/scoping.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/bnn/hidden_layer.py` & `pyro-ppl-1.9.0/pyro/contrib/bnn/hidden_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
     Reference:
 
     Kingma, Diederik P., Tim Salimans, and Max Welling.
     "Variational dropout and the local reparameterization trick."
     Advances in Neural Information Processing Systems. 2015.
     """
+
     has_rsample = True
 
     def __init__(
         self,
         X=None,
         A_mean=None,
         A_scale=None,
```

### Comparing `pyro-ppl-1.8.6/pyro/contrib/cevae/__init__.py` & `pyro-ppl-1.9.0/pyro/contrib/cevae/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,15 @@
     Data pre-whitener.
     """
 
     def __init__(self, data):
         super().__init__()
         with torch.no_grad():
             loc = data.mean(0)
-            scale = data.std(0)
+            scale = data.std(0, unbiased=False)
             scale[~(scale > 0)] = 1.0
             self.register_buffer("loc", loc)
             self.register_buffer("inv_scale", scale.reciprocal())
 
     def forward(self, data):
         return (data - self.loc) * self.inv_scale
 
@@ -570,15 +570,20 @@
         """
         assert x.dim() == 2 and x.size(-1) == self.feature_dim
         assert t.shape == x.shape[:1]
         assert y.shape == y.shape[:1]
         self.whiten = PreWhitener(x)
 
         dataset = TensorDataset(x, t, y)
-        dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=True)
+        dataloader = DataLoader(
+            dataset,
+            batch_size=batch_size,
+            shuffle=True,
+            generator=torch.Generator(device=x.device),
+        )
         logger.info("Training with {} minibatches per epoch".format(len(dataloader)))
         num_steps = num_epochs * len(dataloader)
         optim = ClippedAdam(
             {
                 "lr": learning_rate,
                 "weight_decay": weight_decay,
                 "lrd": learning_rate_decay ** (1 / num_steps),
```

### Comparing `pyro-ppl-1.8.6/pyro/contrib/conjugate/infer.py` & `pyro-ppl-1.9.0/pyro/contrib/conjugate/infer.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/easyguide/easyguide.py` & `pyro-ppl-1.9.0/pyro/contrib/easyguide/easyguide.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/epidemiology/compartmental.py` & `pyro-ppl-1.9.0/pyro/contrib/epidemiology/compartmental.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/epidemiology/distributions.py` & `pyro-ppl-1.9.0/pyro/contrib/epidemiology/distributions.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/epidemiology/models.py` & `pyro-ppl-1.9.0/pyro/contrib/epidemiology/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -676,17 +676,19 @@
             obs=self.data[t] if t_is_observed else None,
         )
         if self.coal_likelihood is not None:
             R = R0 * state["S"] / self.population
             coal_rate = R * (1.0 + 1.0 / k) / (tau_i * state["I"] + 1e-8)
             pyro.factor(
                 "coalescent_{}".format(t),
-                self.coal_likelihood(coal_rate, t)
-                if t_is_observed
-                else torch.tensor(0.0),
+                (
+                    self.coal_likelihood(coal_rate, t)
+                    if t_is_observed
+                    else torch.tensor(0.0)
+                ),
             )
 
         # Update compartements with flows.
         state["S"] = state["S"] - S2E
         state["E"] = state["E"] + S2E - E2I
         state["I"] = state["I"] + E2I - I2R
```

### Comparing `pyro-ppl-1.8.6/pyro/contrib/epidemiology/util.py` & `pyro-ppl-1.9.0/pyro/contrib/epidemiology/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Contributors to the Pyro project.
 # SPDX-License-Identifier: Apache-2.0
 
-import numpy
+import numpy as np
 import torch
 
 import pyro
 import pyro.distributions as dist
 import pyro.poutine as poutine
 from pyro.distributions.util import broadcast_shape
 from pyro.ops.special import safe_log
@@ -164,15 +164,15 @@
         -3.561253561253564e-05,
         0.0,
         3.4687534687534714e-07,
         0.0,
     ],
 ]
 
-W16 = numpy.array(W16)
+W16 = np.array(W16)
 
 
 def compute_bin_probs(s, num_quant_bins):
     """
     Compute categorical probabilities for a quantization scheme with num_quant_bins many
     bins. `s` is a real-valued tensor with values in [0, 1]. Returns probabilities
     of shape `s.shape` + `(num_quant_bins,)`
```

### Comparing `pyro-ppl-1.8.6/pyro/contrib/examples/bart.py` & `pyro-ppl-1.9.0/pyro/contrib/examples/bart.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/examples/finance.py` & `pyro-ppl-1.9.0/pyro/contrib/examples/finance.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/examples/multi_mnist.py` & `pyro-ppl-1.9.0/pyro/contrib/examples/multi_mnist.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/examples/nextstrain.py` & `pyro-ppl-1.9.0/pyro/contrib/examples/nextstrain.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/examples/polyphonic_data_loader.py` & `pyro-ppl-1.9.0/pyro/contrib/examples/polyphonic_data_loader.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/examples/scanvi_data.py` & `pyro-ppl-1.9.0/pyro/contrib/examples/scanvi_data.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/examples/util.py` & `pyro-ppl-1.9.0/pyro/contrib/examples/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/forecast/evaluate.py` & `pyro-ppl-1.9.0/pyro/contrib/forecast/evaluate.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/forecast/forecaster.py` & `pyro-ppl-1.9.0/pyro/contrib/forecast/forecaster.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/forecast/util.py` & `pyro-ppl-1.9.0/pyro/contrib/forecast/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/funsor/__init__.py` & `pyro-ppl-1.9.0/pyro/contrib/funsor/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/enum_messenger.py` & `pyro-ppl-1.9.0/pyro/contrib/funsor/handlers/enum_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/named_messenger.py` & `pyro-ppl-1.9.0/pyro/contrib/funsor/handlers/named_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/plate_messenger.py` & `pyro-ppl-1.9.0/pyro/contrib/funsor/handlers/plate_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/primitives.py` & `pyro-ppl-1.9.0/pyro/contrib/funsor/handlers/primitives.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/replay_messenger.py` & `pyro-ppl-1.9.0/pyro/contrib/funsor/handlers/replay_messenger.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     This version of :class:`~ReplayMessenger` is almost identical to the original version,
     except that it calls :func:`~pyro.contrib.funsor.to_data` on the replayed funsor values.
     This may result in different unpacked shapes, but should produce correct allocations.
     """
 
     def _pyro_sample(self, msg):
         name = msg["name"]
-        msg[
-            "replay_active"
-        ] = True  # indicate replaying so importance weights can be scaled
+        msg["replay_active"] = (
+            True  # indicate replaying so importance weights can be scaled
+        )
         if self.trace is None:
             return
 
         if name in self.trace:
             guide_msg = self.trace.nodes[name]
             msg["funsor"] = {} if "funsor" not in msg else msg["funsor"]
             if guide_msg["type"] != "sample":
```

### Comparing `pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/runtime.py` & `pyro-ppl-1.9.0/pyro/contrib/funsor/handlers/runtime.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/trace_messenger.py` & `pyro-ppl-1.9.0/pyro/contrib/funsor/handlers/trace_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/funsor/infer/__init__.py` & `pyro-ppl-1.9.0/pyro/contrib/funsor/infer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/funsor/infer/discrete.py` & `pyro-ppl-1.9.0/pyro/contrib/funsor/infer/discrete.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/funsor/infer/elbo.py` & `pyro-ppl-1.9.0/pyro/contrib/funsor/infer/elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/funsor/infer/trace_elbo.py` & `pyro-ppl-1.9.0/pyro/contrib/funsor/infer/trace_elbo.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 from .elbo import ELBO, Jit_ELBO
 from .traceenum_elbo import terms_from_trace
 
 
 @copy_docs_from(_OrigTrace_ELBO)
 class Trace_ELBO(ELBO):
     def differentiable_loss(self, model, guide, *args, **kwargs):
-        with enum(), plate(
-            size=self.num_particles
-        ) if self.num_particles > 1 else contextlib.ExitStack():
+        with enum(), (
+            plate(size=self.num_particles)
+            if self.num_particles > 1
+            else contextlib.ExitStack()
+        ):
             guide_tr = trace(config_enumerate(default="flat")(guide)).get_trace(
                 *args, **kwargs
             )
             model_tr = trace(replay(model, trace=guide_tr)).get_trace(*args, **kwargs)
 
         model_terms = terms_from_trace(model_tr)
         guide_terms = terms_from_trace(guide_tr)
```

### Comparing `pyro-ppl-1.8.6/pyro/contrib/funsor/infer/traceenum_elbo.py` & `pyro-ppl-1.9.0/pyro/contrib/funsor/infer/traceenum_elbo.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,20 +89,22 @@
     return terms
 
 
 @copy_docs_from(_OrigTraceEnum_ELBO)
 class TraceMarkovEnum_ELBO(ELBO):
     def differentiable_loss(self, model, guide, *args, **kwargs):
         # get batched, enumerated, to_funsor-ed traces from the guide and model
-        with plate(
-            size=self.num_particles
-        ) if self.num_particles > 1 else contextlib.ExitStack(), enum(
-            first_available_dim=(-self.max_plate_nesting - 1)
-            if self.max_plate_nesting
-            else None
+        with (
+            plate(size=self.num_particles)
+            if self.num_particles > 1
+            else contextlib.ExitStack()
+        ), enum(
+            first_available_dim=(
+                (-self.max_plate_nesting - 1) if self.max_plate_nesting else None
+            )
         ):
             guide_tr = trace(guide).get_trace(*args, **kwargs)
             model_tr = trace(replay(model, trace=guide_tr)).get_trace(*args, **kwargs)
 
         # extract from traces all metadata that we will need to compute the elbo
         guide_terms = terms_from_trace(guide_tr)
         model_terms = terms_from_trace(model_tr)
@@ -166,20 +168,22 @@
             return -to_data(apply_optimizer(elbo))
 
 
 @copy_docs_from(_OrigTraceEnum_ELBO)
 class TraceEnum_ELBO(ELBO):
     def differentiable_loss(self, model, guide, *args, **kwargs):
         # get batched, enumerated, to_funsor-ed traces from the guide and model
-        with plate(
-            size=self.num_particles
-        ) if self.num_particles > 1 else contextlib.ExitStack(), enum(
-            first_available_dim=(-self.max_plate_nesting - 1)
-            if self.max_plate_nesting
-            else None
+        with (
+            plate(size=self.num_particles)
+            if self.num_particles > 1
+            else contextlib.ExitStack()
+        ), enum(
+            first_available_dim=(
+                (-self.max_plate_nesting - 1) if self.max_plate_nesting else None
+            )
         ):
             guide_tr = trace(guide).get_trace(*args, **kwargs)
             model_tr = trace(replay(model, trace=guide_tr)).get_trace(*args, **kwargs)
 
         # extract from traces all metadata that we will need to compute the elbo
         guide_terms = terms_from_trace(guide_tr)
         model_terms = terms_from_trace(model_tr)
```

### Comparing `pyro-ppl-1.8.6/pyro/contrib/funsor/infer/tracetmc_elbo.py` & `pyro-ppl-1.9.0/pyro/contrib/funsor/infer/tracetmc_elbo.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 from pyro.distributions.util import copy_docs_from
 from pyro.infer import TraceTMC_ELBO as _OrigTraceTMC_ELBO
 
 
 @copy_docs_from(_OrigTraceTMC_ELBO)
 class TraceTMC_ELBO(ELBO):
     def differentiable_loss(self, model, guide, *args, **kwargs):
-        with plate(
-            size=self.num_particles
-        ) if self.num_particles > 1 else contextlib.ExitStack(), enum(
-            first_available_dim=(-self.max_plate_nesting - 1)
-            if self.max_plate_nesting
-            else None
+        with (
+            plate(size=self.num_particles)
+            if self.num_particles > 1
+            else contextlib.ExitStack()
+        ), enum(
+            first_available_dim=(
+                (-self.max_plate_nesting - 1) if self.max_plate_nesting else None
+            )
         ):
             guide_tr = trace(guide).get_trace(*args, **kwargs)
             model_tr = trace(replay(model, trace=guide_tr)).get_trace(*args, **kwargs)
 
         model_terms = terms_from_trace(model_tr)
         guide_terms = terms_from_trace(guide_tr)
```

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/kernels/__init__.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/kernels/brownian.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/kernels/brownian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/kernels/coregionalize.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/kernels/coregionalize.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/kernels/dot_product.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/kernels/dot_product.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/kernels/isotropic.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/kernels/isotropic.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/kernels/kernel.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/kernels/kernel.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/kernels/periodic.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/kernels/periodic.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/kernels/static.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/kernels/static.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/__init__.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/likelihoods/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/binary.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/likelihoods/binary.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/gaussian.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/likelihoods/gaussian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/likelihood.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/likelihoods/likelihood.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/multi_class.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/likelihoods/multi_class.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/poisson.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/likelihoods/poisson.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/models/__init__.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/models/gplvm.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/models/gplvm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/models/gpr.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/models/gpr.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/models/model.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/models/model.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/models/sgpr.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/models/sgpr.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/models/vgp.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/models/vgp.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/models/vsgp.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/models/vsgp.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/parameterized.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/parameterized.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         >>> linear.b = PyroSample(dist.Normal(0, 1))
         >>> linear.autoguide("b", dist.Normal)
         >>> assert "a_unconstrained" in dict(linear.named_parameters())
         >>> assert "b_loc" in dict(linear.named_parameters())
         >>> assert "b_scale_unconstrained" in dict(linear.named_parameters())
 
     Note that by default, data of a parameter is a float :class:`torch.Tensor`
-    (unless we use :func:`torch.set_default_tensor_type` to change default
+    (unless we use :func:`torch.set_default_dtype` to change default
     tensor type). To cast these parameters to a correct data type or GPU device,
     we can call methods such as :meth:`~torch.nn.Module.double` or
     :meth:`~torch.nn.Module.cuda`. See :class:`torch.nn.Module` for more
     information.
     """
 
     def __init__(self):
```

### Comparing `pyro-ppl-1.8.6/pyro/contrib/gp/util.py` & `pyro-ppl-1.9.0/pyro/contrib/gp/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/minipyro.py` & `pyro-ppl-1.9.0/pyro/contrib/minipyro.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/mue/dataloaders.py` & `pyro-ppl-1.9.0/pyro/contrib/mue/dataloaders.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/mue/missingdatahmm.py` & `pyro-ppl-1.9.0/pyro/contrib/mue/missingdatahmm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/mue/models.py` & `pyro-ppl-1.9.0/pyro/contrib/mue/models.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/mue/statearrangers.py` & `pyro-ppl-1.9.0/pyro/contrib/mue/statearrangers.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/oed/__init__.py` & `pyro-ppl-1.9.0/pyro/contrib/oed/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/oed/eig.py` & `pyro-ppl-1.9.0/pyro/contrib/oed/eig.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/oed/glmm/__init__.py` & `pyro-ppl-1.9.0/pyro/contrib/oed/glmm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/oed/glmm/glmm.py` & `pyro-ppl-1.9.0/pyro/contrib/oed/glmm/glmm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/oed/glmm/guides.py` & `pyro-ppl-1.9.0/pyro/contrib/oed/glmm/guides.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/oed/search.py` & `pyro-ppl-1.9.0/pyro/contrib/oed/search.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/oed/util.py` & `pyro-ppl-1.9.0/pyro/contrib/oed/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/randomvariable/random_variable.py` & `pyro-ppl-1.9.0/pyro/contrib/randomvariable/random_variable.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/timeseries/__init__.py` & `pyro-ppl-1.9.0/pyro/contrib/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/timeseries/base.py` & `pyro-ppl-1.9.0/pyro/contrib/timeseries/base.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/timeseries/gp.py` & `pyro-ppl-1.9.0/pyro/contrib/timeseries/gp.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/timeseries/lgssm.py` & `pyro-ppl-1.9.0/pyro/contrib/timeseries/lgssm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/timeseries/lgssmgp.py` & `pyro-ppl-1.9.0/pyro/contrib/timeseries/lgssmgp.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,17 +105,17 @@
 
     def _get_init_dist(self):
         loc = self.z_trans_matrix.new_zeros(self.full_state_dim)
         covar = self.z_trans_matrix.new_zeros(self.full_state_dim, self.full_state_dim)
         covar[: self.full_gp_state_dim, : self.full_gp_state_dim] = block_diag_embed(
             self.kernel.stationary_covariance()
         )
-        covar[
-            self.full_gp_state_dim :, self.full_gp_state_dim :
-        ] = self.init_noise_scale_sq.diag_embed()
+        covar[self.full_gp_state_dim :, self.full_gp_state_dim :] = (
+            self.init_noise_scale_sq.diag_embed()
+        )
         return MultivariateNormal(loc, covar)
 
     def _get_obs_dist(self):
         return dist.Normal(self.obs_loc, self.obs_noise_scale).to_event(1)
 
     def get_dist(self, duration=None):
         """
@@ -130,31 +130,31 @@
             gp_trans_matrix,
             gp_process_covar,
         ) = self.kernel.transition_matrix_and_covariance(dt=self.dt)
 
         trans_covar = self.z_trans_matrix.new_zeros(
             self.full_state_dim, self.full_state_dim
         )
-        trans_covar[
-            : self.full_gp_state_dim, : self.full_gp_state_dim
-        ] = block_diag_embed(gp_process_covar)
-        trans_covar[
-            self.full_gp_state_dim :, self.full_gp_state_dim :
-        ] = self.trans_noise_scale_sq.diag_embed()
+        trans_covar[: self.full_gp_state_dim, : self.full_gp_state_dim] = (
+            block_diag_embed(gp_process_covar)
+        )
+        trans_covar[self.full_gp_state_dim :, self.full_gp_state_dim :] = (
+            self.trans_noise_scale_sq.diag_embed()
+        )
         trans_dist = MultivariateNormal(
             trans_covar.new_zeros(self.full_state_dim), trans_covar
         )
 
         full_trans_mat = trans_covar.new_zeros(self.full_state_dim, self.full_state_dim)
-        full_trans_mat[
-            : self.full_gp_state_dim, : self.full_gp_state_dim
-        ] = block_diag_embed(gp_trans_matrix)
-        full_trans_mat[
-            self.full_gp_state_dim :, self.full_gp_state_dim :
-        ] = self.z_trans_matrix
+        full_trans_mat[: self.full_gp_state_dim, : self.full_gp_state_dim] = (
+            block_diag_embed(gp_trans_matrix)
+        )
+        full_trans_mat[self.full_gp_state_dim :, self.full_gp_state_dim :] = (
+            self.z_trans_matrix
+        )
 
         return dist.GaussianHMM(
             self._get_init_dist(),
             full_trans_mat,
             trans_dist,
             self._get_obs_matrix(),
             self._get_obs_dist(),
```

### Comparing `pyro-ppl-1.8.6/pyro/contrib/tracking/assignment.py` & `pyro-ppl-1.9.0/pyro/contrib/tracking/assignment.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/tracking/distributions.py` & `pyro-ppl-1.9.0/pyro/contrib/tracking/distributions.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     :param measurement_cov: measurement covariance
     :type measurement_cov: torch.Tensor
     :param time_steps: number time step
     :type time_steps: int
     :param dt: time step
     :type dt: torch.Tensor
     """
+
     arg_constraints = {
         "measurement_cov": constraints.positive_definite,
         "P0": constraints.positive_definite,
         "x0": constraints.real_vector,
     }
     has_rsample = True
```

### Comparing `pyro-ppl-1.8.6/pyro/contrib/tracking/dynamic_models.py` & `pyro-ppl-1.9.0/pyro/contrib/tracking/dynamic_models.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/tracking/extended_kalman_filter.py` & `pyro-ppl-1.9.0/pyro/contrib/tracking/extended_kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/tracking/hashing.py` & `pyro-ppl-1.9.0/pyro/contrib/tracking/hashing.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/tracking/measurements.py` & `pyro-ppl-1.9.0/pyro/contrib/tracking/measurements.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/contrib/util.py` & `pyro-ppl-1.9.0/pyro/contrib/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/__init__.py` & `pyro-ppl-1.9.0/pyro/distributions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,17 @@
     GammaGaussianHMM,
     GaussianHMM,
     GaussianMRF,
     IndependentHMM,
     LinearHMM,
 )
 from pyro.distributions.improper_uniform import ImproperUniform
-from pyro.distributions.inverse_gamma import InverseGamma
+
+if "InverseGamma" not in locals():  # Use PyTorch version if available.
+    from pyro.distributions.inverse_gamma import InverseGamma
 from pyro.distributions.lkj import LKJ, LKJCorrCholesky
 from pyro.distributions.log_normal_negative_binomial import LogNormalNegativeBinomial
 from pyro.distributions.logistic import Logistic, SkewLogistic
 from pyro.distributions.mixture import MaskedMixture
 from pyro.distributions.multivariate_studentt import MultivariateStudentT
 from pyro.distributions.nanmasked import NanMaskedMultivariateNormal, NanMaskedNormal
 from pyro.distributions.omt_mvn import OMTMultivariateNormal
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/affine_beta.py` & `pyro-ppl-1.9.0/pyro/distributions/affine_beta.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/asymmetriclaplace.py` & `pyro-ppl-1.9.0/pyro/distributions/asymmetriclaplace.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,17 +195,15 @@
     @property
     def variance(self):
         left = self.left_scale
         right = self.right_scale
         total = left + right
         p = left / total
         q = right / total
-        return (
-            p * left**2 + q * right**2 + p * q * total**2 + self.soft_scale**2
-        )
+        return p * left**2 + q * right**2 + p * q * total**2 + self.soft_scale**2
 
 
 def _logerfc(x):
     try:
         # Requires https://github.com/pytorch/pytorch/issues/31945
         return torch.logerfc(x)
     except AttributeError:
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/avf_mvn.py` & `pyro-ppl-1.9.0/pyro/distributions/avf_mvn.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/coalescent.py` & `pyro-ppl-1.9.0/pyro/distributions/coalescent.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/conditional.py` & `pyro-ppl-1.9.0/pyro/distributions/conditional.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,17 +78,19 @@
         >>> context = torch.rand(10, 2)
         >>> data = torch.rand(10, 3)
         >>> nll = -cond_dist.condition(context).log_prob(data)
     """
 
     def __init__(self, transforms, cache_size: int = 0):
         self.transforms = [
-            ConstantConditionalTransform(t)
-            if not isinstance(t, ConditionalTransform)
-            else t
+            (
+                ConstantConditionalTransform(t)
+                if not isinstance(t, ConditionalTransform)
+                else t
+            )
             for t in transforms
         ]
         super().__init__()
         if cache_size not in {0, 1}:
             raise ValueError("cache_size must be 0 or 1")
         self._cache_size = cache_size
         # for parameter storage
@@ -127,17 +129,19 @@
     def __init__(self, base_dist, transforms):
         self.base_dist = (
             base_dist
             if isinstance(base_dist, ConditionalDistribution)
             else ConstantConditionalDistribution(base_dist)
         )
         self.transforms = [
-            t
-            if isinstance(t, ConditionalTransform)
-            else ConstantConditionalTransform(t)
+            (
+                t
+                if isinstance(t, ConditionalTransform)
+                else ConstantConditionalTransform(t)
+            )
             for t in transforms
         ]
 
     def condition(self, context):
         base_dist = self.base_dist.condition(context)
         transforms = [t.condition(context) for t in self.transforms]
         return TransformedDistribution(base_dist, transforms)
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/conjugate.py` & `pyro-ppl-1.9.0/pyro/distributions/conjugate.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     :type concentration1: float or torch.Tensor
     :param concentration0: 2nd concentration parameter (beta) for the
         Beta distribution.
     :type concentration0: float or torch.Tensor
     :param total_count: Number of Bernoulli trials.
     :type total_count: float or torch.Tensor
     """
+
     arg_constraints = {
         "concentration1": constraints.positive,
         "concentration0": constraints.positive,
         "total_count": constraints.nonnegative_integer,
     }
     has_enumerate_support = True
     support = Binomial.support
@@ -146,14 +147,15 @@
 
     :param float or torch.Tensor concentration: concentration parameter (alpha) for the
         Dirichlet distribution.
     :param int or torch.Tensor total_count: number of Categorical trials.
     :param bool is_sparse: Whether to assume value is mostly zero when computing
         :meth:`log_prob`, which can speed up computation when data is sparse.
     """
+
     arg_constraints = {
         "concentration": constraints.independent(constraints.positive, 1),
         "total_count": constraints.nonnegative_integer,
     }
     support = Multinomial.support
 
     def __init__(
@@ -245,15 +247,16 @@
         "concentration": constraints.positive,
         "rate": constraints.positive,
     }
     support = Poisson.support
 
     def __init__(self, concentration, rate, validate_args=None):
         concentration, rate = broadcast_all(concentration, rate)
-        self._gamma = Gamma(concentration, rate)
+        self._gamma = Gamma(concentration, rate, validate_args=False)
+        self._gamma._validate_args = validate_args
         super().__init__(self._gamma._batch_shape, validate_args=validate_args)
 
     @property
     def concentration(self):
         return self._gamma.concentration
 
     @property
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/constraints.py` & `pyro-ppl-1.9.0/pyro/distributions/constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,18 +154,20 @@
     [
         """
     {}
     ----------------------------------------------------------------
     {}
     """.format(
             _name,
-            "alias of :class:`torch.distributions.constraints.{}`".format(_name)
-            if globals()[_name].__module__.startswith("torch")
-            else ".. autoclass:: {}".format(
-                _name
-                if type(globals()[_name]) is type
-                else type(globals()[_name]).__name__
+            (
+                "alias of :class:`torch.distributions.constraints.{}`".format(_name)
+                if globals()[_name].__module__.startswith("torch")
+                else ".. autoclass:: {}".format(
+                    _name
+                    if type(globals()[_name]) is type
+                    else type(globals()[_name]).__name__
+                )
             ),
         )
         for _name in sorted(__all__)
     ]
 )
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/delta.py` & `pyro-ppl-1.9.0/pyro/distributions/delta.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/diag_normal_mixture.py` & `pyro-ppl-1.9.0/pyro/distributions/diag_normal_mixture.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,37 +42,39 @@
 
     has_rsample = True
     arg_constraints = {
         "locs": constraints.real,
         "coord_scale": constraints.positive,
         "component_logits": constraints.real,
     }
+    support = constraints.real_vector
 
     def __init__(self, locs, coord_scale, component_logits):
         self.batch_mode = locs.dim() > 2
         assert coord_scale.shape == locs.shape
-        assert (
-            self.batch_mode or locs.dim() == 2
-        ), "The locs parameter in MixtureOfDiagNormals should be K x D dimensional (or B x K x D if doing batches)"
+        assert self.batch_mode or locs.dim() == 2, (
+            "The locs parameter in MixtureOfDiagNormals should be K x D dimensional "
+            "(or ... x B x K x D if doing batches)"
+        )
         if not self.batch_mode:
             assert (
                 coord_scale.dim() == 2
             ), "The coord_scale parameter in MixtureOfDiagNormals should be K x D dimensional"
             assert (
                 component_logits.dim() == 1
             ), "The component_logits parameter in MixtureOfDiagNormals should be K dimensional"
             assert component_logits.size(-1) == locs.size(-2)
             batch_shape = ()
         else:
             assert (
                 coord_scale.dim() > 2
-            ), "The coord_scale parameter in MixtureOfDiagNormals should be B x K x D dimensional"
+            ), "The coord_scale parameter in MixtureOfDiagNormals should be ... x B x K x D dimensional"
             assert (
                 component_logits.dim() > 1
-            ), "The component_logits parameter in MixtureOfDiagNormals should be B x K dimensional"
+            ), "The component_logits parameter in MixtureOfDiagNormals should be ... x B x K dimensional"
             assert component_logits.size(-1) == locs.size(-2)
             batch_shape = tuple(locs.shape[:-2])
 
         self.locs = locs
         self.coord_scale = coord_scale
         self.component_logits = component_logits
         self.dim = locs.size(-1)
@@ -129,15 +131,15 @@
         )
 
 
 class _MixDiagNormalSample(Function):
     @staticmethod
     def forward(ctx, locs, scales, component_logits, pis, which, noise_shape):
         dim = scales.size(-1)
-        white = locs.new(noise_shape).normal_()
+        white = locs.new_empty(noise_shape).normal_()
         n_unsqueezes = locs.dim() - which.dim()
         for _ in range(n_unsqueezes):
             which = which.unsqueeze(-1)
         which_expand = which.expand(tuple(which.shape[:-1] + (dim,)))
         loc = torch.gather(locs, -2, which_expand).squeeze(-2)
         sigma = torch.gather(scales, -2, which_expand).squeeze(-2)
         z = loc + sigma * white
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/diag_normal_mixture_shared_cov.py` & `pyro-ppl-1.9.0/pyro/distributions/diag_normal_mixture_shared_cov.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,36 +41,39 @@
 
     has_rsample = True
     arg_constraints = {
         "locs": constraints.real,
         "coord_scale": constraints.positive,
         "component_logits": constraints.real,
     }
+    support = constraints.real_vector
 
     def __init__(self, locs, coord_scale, component_logits):
         self.batch_mode = locs.dim() > 2
-        assert (
-            self.batch_mode or locs.dim() == 2
-        ), "The locs parameter in MixtureOfDiagNormals should be K x D dimensional (or ... x B x K x D in batch mode)"
+        assert self.batch_mode or locs.dim() == 2, (
+            "The locs parameter in MixtureOfDiagNormalsSharedCovariance should be K x D dimensional "
+            "(or ... x B x K x D in batch mode)"
+        )
         if not self.batch_mode:
             assert (
                 coord_scale.dim() == 1
-            ), "The coord_scale parameter in MixtureOfDiagNormals should be D dimensional"
+            ), "The coord_scale parameter in MixtureOfDiagNormalsSharedCovariance should be D dimensional"
             assert (
                 component_logits.dim() == 1
-            ), "The component_logits parameter in MixtureOfDiagNormals should be K dimensional"
+            ), "The component_logits parameter in MixtureOfDiagNormalsSharedCovariance should be K dimensional"
             assert component_logits.size(0) == locs.size(0)
             batch_shape = ()
         else:
             assert (
                 coord_scale.dim() > 1
-            ), "The coord_scale parameter in MixtureOfDiagNormals should be ... x B x D dimensional"
-            assert (
-                component_logits.dim() > 1
-            ), "The component_logits parameter in MixtureOfDiagNormals should be ... x B x K dimensional"
+            ), "The coord_scale parameter in MixtureOfDiagNormalsSharedCovariance should be ... x B x D dimensional"
+            assert component_logits.dim() > 1, (
+                "The component_logits parameter in MixtureOfDiagNormalsSharedCovariance should be "
+                "... x B x K dimensional"
+            )
             assert component_logits.size(-1) == locs.size(-2)
             batch_shape = tuple(locs.shape[:-2])
         self.locs = locs
         self.coord_scale = coord_scale
         self.component_logits = component_logits
         self.dim = locs.size(-1)
         if self.dim < 2:
@@ -130,15 +133,15 @@
         )
 
 
 class _MixDiagNormalSharedCovarianceSample(Function):
     @staticmethod
     def forward(ctx, locs, coord_scale, component_logits, pis, which, noise_shape):
         dim = coord_scale.size(-1)
-        white = torch.randn(noise_shape, dtype=locs.dtype, device=locs.device)
+        white = locs.new_empty(noise_shape).normal_()
         n_unsqueezes = locs.dim() - which.dim()
         for _ in range(n_unsqueezes):
             which = which.unsqueeze(-1)
         expand_tuple = tuple(which.shape[:-1] + (dim,))
         loc = torch.gather(locs, -2, which.expand(expand_tuple)).squeeze(-2)
         z = loc + coord_scale * white
         ctx.save_for_backward(z, coord_scale, locs, component_logits, pis)
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/distribution.py` & `pyro-ppl-1.9.0/pyro/distributions/distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 import functools
 import inspect
 from abc import ABCMeta, abstractmethod
 
+import torch
+
 from pyro.distributions.score_parts import ScoreParts
 
 COERCIONS = []
 
 
 class DistributionMeta(ABCMeta):
     def __init__(cls, *args, **kwargs):
@@ -118,15 +120,15 @@
         else:
             # XXX should the user be able to control inclusion of the entropy term?
             # See Roeder, Wu, Duvenaud (2017) "Sticking the Landing" https://arxiv.org/abs/1703.09194
             return ScoreParts(
                 log_prob=log_prob, score_function=log_prob, entropy_term=0
             )
 
-    def enumerate_support(self, expand=True):
+    def enumerate_support(self, expand: bool = True) -> torch.Tensor:
         """
         Returns a representation of the parametrized distribution's support,
         along the first dimension. This is implemented only by discrete
         distributions.
 
         Note that this returns support values of all the batched RVs in
         lock-step, rather than the full cartesian product.
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/empirical.py` & `pyro-ppl-1.9.0/pyro/distributions/empirical.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/extended.py` & `pyro-ppl-1.9.0/pyro/distributions/extended.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/folded.py` & `pyro-ppl-1.9.0/pyro/distributions/folded.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/gaussian_scale_mixture.py` & `pyro-ppl-1.9.0/pyro/distributions/gaussian_scale_mixture.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/grouped_normal_normal.py` & `pyro-ppl-1.9.0/pyro/distributions/grouped_normal_normal.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     :param torch.Tensor prior_scale: Tensor of shape `(num_groups,)` specifying the prior scale of the latent
         of each group.
     :param torch.Tensor obs_scale: Tensor of shape `(num_data,)` specifying the scale of the observation noise
         of each observation.
     :param torch.LongTensor group_idx: Tensor of indices of shape `(num_data,)` linking each observation to one
         of the `num_groups` groups that are specified in `prior_loc` and `prior_scale`.
     """
+
     arg_constraints = {
         "prior_loc": constraints.real,
         "prior_scale": constraints.positive,
         "obs_scale": constraints.positive,
     }
     support = constraints.real
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/hmm.py` & `pyro-ppl-1.9.0/pyro/distributions/hmm.py`

 * *Files 0% similar despite different names*

```diff
@@ -999,14 +999,15 @@
     :param observation_dist: A observation noise distribution. This should have
         batch_shape broadcastable to ``self.batch_shape + (num_steps,)``.  This
         should have event_shape ``(obs_dim,)``.
     :param int duration: Optional size of the time axis ``event_shape[0]``.
         This is required when sampling from homogeneous HMMs whose parameters
         are not expanded along the time axis.
     """
+
     arg_constraints = {}
     support = constraints.independent(constraints.real, 2)
     has_rsample = True
 
     def __init__(
         self,
         initial_dist,
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/improper_uniform.py` & `pyro-ppl-1.9.0/pyro/distributions/improper_uniform.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/inverse_gamma.py` & `pyro-ppl-1.9.0/pyro/distributions/inverse_gamma.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 
 from torch.distributions import constraints
 from torch.distributions.transforms import PowerTransform
 
 from pyro.distributions.torch import Gamma, TransformedDistribution
 
 
+# DEPRECATED in favor of torch.distributions.InverseGamma.
 class InverseGamma(TransformedDistribution):
     r"""
     Creates an inverse-gamma distribution parameterized by
     `concentration` and `rate`.
 
         X ~ Gamma(concentration, rate)
         Y = 1/X ~ InverseGamma(concentration, rate)
 
     :param torch.Tensor concentration: the concentration parameter (i.e. alpha).
     :param torch.Tensor rate: the rate parameter (i.e. beta).
     """
+
     arg_constraints = {
         "concentration": constraints.positive,
         "rate": constraints.positive,
     }
     support = constraints.positive
     has_rsample = True
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/kl.py` & `pyro-ppl-1.9.0/pyro/distributions/kl.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/lkj.py` & `pyro-ppl-1.9.0/pyro/distributions/lkj.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         distribution (often referred to as eta)
 
     **References**
 
     [1] `Generating random correlation matrices based on vines and extended onion method`,
     Daniel Lewandowski, Dorota Kurowicka, Harry Joe
     """
+
     arg_constraints = {"concentration": constraints.positive}
     support = constraints.corr_matrix
 
     def __init__(self, dim, concentration=1.0, validate_args=None):
         base_dist = LKJCholesky(dim, concentration)
         self.dim, self.concentration = base_dist.dim, base_dist.concentration
         super(LKJ, self).__init__(
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/log_normal_negative_binomial.py` & `pyro-ppl-1.9.0/pyro/distributions/log_normal_negative_binomial.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     :type total_count: float or torch.Tensor
     :param torch.Tensor logits: Event log-odds for probabilities of success for underlying
         Negative Binomial distribution.
     :param torch.Tensor multiplicative_noise_scale: Controls the level of the injected Normal logit noise.
     :param int num_quad_points: Number of quadrature points used to compute the (approximate) `log_prob`.
         Defaults to 8.
     """
+
     arg_constraints = {
         "total_count": constraints.greater_than_eq(0),
         "logits": constraints.real,
         "multiplicative_noise_scale": constraints.positive,
     }
     support = constraints.nonnegative_integer
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/logistic.py` & `pyro-ppl-1.9.0/pyro/distributions/logistic.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/mixture.py` & `pyro-ppl-1.9.0/pyro/distributions/mixture.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/multivariate_studentt.py` & `pyro-ppl-1.9.0/pyro/distributions/multivariate_studentt.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/nanmasked.py` & `pyro-ppl-1.9.0/pyro/distributions/nanmasked.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/omt_mvn.py` & `pyro-ppl-1.9.0/pyro/distributions/omt_mvn.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/one_one_matching.py` & `pyro-ppl-1.9.0/pyro/distributions/one_one_matching.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,14 +73,15 @@
         "Approximating the permanent with fractional belief propagation"
         http://www.jmlr.org/papers/volume14/chertkov13a/chertkov13a.pdf
 
     :param Tensor logits: An ``(N, N)``-shaped tensor of edge logits.
     :param int bp_iters: Optional number of belief propagation iterations. If
         unspecified or ``None`` expensive exact algorithms will be used.
     """
+
     arg_constraints = {"logits": constraints.real}
     has_enumerate_support = True
 
     def __init__(self, logits, *, bp_iters=None, validate_args=None):
         if logits.dim() != 2:
             raise NotImplementedError("OneOneMatching does not support batching")
         assert bp_iters is None or isinstance(bp_iters, int) and bp_iters > 0
@@ -156,23 +157,19 @@
         # https://www.cc.gatech.edu/~vigoda/Permanent.pdf
         # https://papers.nips.cc/paper/2012/file/4c27cea8526af8cfee3be5e183ac9605-Paper.pdf
         raise NotImplementedError
 
     def mode(self):
         """
         Computes a maximum probability matching.
-
-        .. note:: This requires the `lap <https://pypi.org/project/lap/>`_
-            package and runs on CPU.
         """
         return maximum_weight_matching(self.logits)
 
 
 @torch.no_grad()
 def maximum_weight_matching(logits):
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", category=ImportWarning)
-        import lap
+    from scipy.optimize import linear_sum_assignment
+
     cost = -logits.cpu()
-    value = lap.lapjv(cost.numpy())[1]
+    value = linear_sum_assignment(cost.numpy())[1]
     value = torch.tensor(value, dtype=torch.long, device=logits.device)
     return value
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/one_two_matching.py` & `pyro-ppl-1.9.0/pyro/distributions/one_two_matching.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         "Approximating the permanent with fractional belief propagation"
         http://www.jmlr.org/papers/volume14/chertkov13a/chertkov13a.pdf
 
     :param Tensor logits: An ``(2 * N, N)``-shaped tensor of edge logits.
     :param int bp_iters: Optional number of belief propagation iterations. If
         unspecified or ``None`` expensive exact algorithms will be used.
     """
+
     arg_constraints = {"logits": constraints.real}
     has_enumerate_support = True
 
     def __init__(self, logits, *, bp_iters=None, validate_args=None):
         if logits.dim() != 2:
             raise NotImplementedError("OneTwoMatching does not support batching")
         assert bp_iters is None or isinstance(bp_iters, int) and bp_iters > 0
@@ -165,17 +166,14 @@
         # https://www.cc.gatech.edu/~vigoda/Permanent.pdf
         # https://papers.nips.cc/paper/2012/file/4c27cea8526af8cfee3be5e183ac9605-Paper.pdf
         raise NotImplementedError
 
     def mode(self):
         """
         Computes a maximum probability matching.
-
-        .. note:: This requires the `lap <https://pypi.org/project/lap/>`_
-            package and runs on CPU.
         """
         return maximum_weight_matching(self.logits)
 
 
 def enumerate_one_two_matchings(num_destins):
     if num_destins == 1:
         return torch.tensor([[0, 0]])
@@ -200,16 +198,15 @@
             block[:, s1 + 1 :] = subproblem[:, s1 - 1 :]
             pos += subsize
     return result
 
 
 @torch.no_grad()
 def maximum_weight_matching(logits):
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", category=ImportWarning)
-        import lap
+    from scipy.optimize import linear_sum_assignment
+
     cost = -logits.cpu()
     cost = torch.cat([cost, cost], dim=-1)  # Duplicate destinations.
-    value = lap.lapjv(cost.numpy())[1]
+    value = linear_sum_assignment(cost.numpy())[1]
     value = torch.tensor(value, dtype=torch.long, device=logits.device)
     value %= logits.size(1)
     return value
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/ordered_logistic.py` & `pyro-ppl-1.9.0/pyro/distributions/ordered_logistic.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/polya_gamma.py` & `pyro-ppl-1.9.0/pyro/distributions/polya_gamma.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/projected_normal.py` & `pyro-ppl-1.9.0/pyro/distributions/projected_normal.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/rejector.py` & `pyro-ppl-1.9.0/pyro/distributions/rejector.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/relaxed_straight_through.py` & `pyro-ppl-1.9.0/pyro/distributions/relaxed_straight_through.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/score_parts.py` & `pyro-ppl-1.9.0/pyro/distributions/score_parts.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
-from collections import namedtuple
+from typing import NamedTuple, Optional, Union
+
+import torch
 
 from pyro.distributions.util import scale_and_mask
 
 
-class ScoreParts(
-    namedtuple("ScoreParts", ["log_prob", "score_function", "entropy_term"])
-):
+class ScoreParts(NamedTuple):
     """
     This data structure stores terms used in stochastic gradient estimators that
     combine the pathwise estimator and the score function estimator.
     """
 
-    def scale_and_mask(self, scale=1.0, mask=None):
+    log_prob: torch.Tensor
+    score_function: torch.Tensor
+    entropy_term: torch.Tensor
+
+    def scale_and_mask(
+        self,
+        scale: Union[float, torch.Tensor] = 1.0,
+        mask: Optional[torch.BoolTensor] = None,
+    ) -> "ScoreParts":
         """
         Scale and mask appropriate terms of a gradient estimator by a data multiplicity factor.
         Note that the `score_function` term should not be scaled or masked.
 
         :param scale: a positive scale
         :type scale: torch.Tensor or number
         :param mask: an optional masking tensor
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/sine_bivariate_von_mises.py` & `pyro-ppl-1.9.0/pyro/distributions/sine_bivariate_von_mises.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         while torch.any(missing > 0) and max_iter:
             curr_conc = conc[:, missing > 0, :]
             curr_corr = corr[missing > 0]
             curr_eig = eig[:, missing > 0]
             curr_b0 = b0[missing > 0]
 
             x = (
-                torch.distributions.Normal(0.0, torch.sqrt(1 + 2 * curr_eig / curr_b0))
+                torch.distributions.Normal(0.0, torch.rsqrt(1 + 2 * curr_eig / curr_b0))
                 .sample((missing[missing > 0].min(),))
                 .view(2, -1, missing[missing > 0].min())
             )
             x /= x.norm(dim=0)[None, ...]  # Angular Central Gaussian distribution
 
             lf = (
                 curr_conc[0] * (x[0] - 1)
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/sine_skewed.py` & `pyro-ppl-1.9.0/pyro/distributions/sine_skewed.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,17 +110,19 @@
             )
 
     def __repr__(self):
         args_string = ", ".join(
             [
                 "{}: {}".format(
                     p,
-                    getattr(self, p)
-                    if getattr(self, p).numel() == 1
-                    else getattr(self, p).size(),
+                    (
+                        getattr(self, p)
+                        if getattr(self, p).numel() == 1
+                        else getattr(self, p).size()
+                    ),
                 )
                 for p in self.arg_constraints.keys()
             ]
         )
         return (
             self.__class__.__name__
             + "("
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/softlaplace.py` & `pyro-ppl-1.9.0/pyro/distributions/softlaplace.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/spanning_tree.cpp` & `pyro-ppl-1.9.0/pyro/distributions/spanning_tree.cpp`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/spanning_tree.py` & `pyro-ppl-1.9.0/pyro/distributions/spanning_tree.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/stable.py` & `pyro-ppl-1.9.0/pyro/distributions/stable.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,25 +129,26 @@
     [2] J.P. Nolan (1997).
         Numerical calculation of stable densities and distribution functions.
     [3] Rafal Weron (1996).
         On the Chambers-Mallows-Stuck Method for
         Simulating Skewed Stable Random Variables.
     [4] J.P. Nolan (2017).
         Stable Distributions: Models for Heavy Tailed Data.
-        http://fs2.american.edu/jpnolan/www/stable/chap1.pdf
+        https://edspace.american.edu/jpnolan/wp-content/uploads/sites/1720/2020/09/Chap1.pdf
 
     :param Tensor stability: Levy stability parameter :math:`\alpha\in(0,2]` .
     :param Tensor skew: Skewness :math:`\beta\in[-1,1]` .
     :param Tensor scale: Scale :math:`\sigma > 0` . Defaults to 1.
     :param Tensor loc: Location :math:`\mu_0` when using Nolan's S0
         parametrization [2], or :math:`\mu` when using the S parameterization.
         Defaults to 0.
     :param str coords: Either "S0" (default) to use Nolan's continuous S0
         parametrization, or "S" to use the discontinuous parameterization.
     """
+
     has_rsample = True
     arg_constraints = {
         "stability": constraints.interval(0, 2),  # half-open (0, 2]
         "skew": constraints.interval(-1, 1),  # closed [-1, 1]
         "scale": constraints.positive,
         "loc": constraints.real,
     }
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/testing/gof.py` & `pyro-ppl-1.9.0/pyro/distributions/testing/gof.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/testing/naive_dirichlet.py` & `pyro-ppl-1.9.0/pyro/distributions/testing/naive_dirichlet.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/testing/rejection_exponential.py` & `pyro-ppl-1.9.0/pyro/distributions/testing/rejection_exponential.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/testing/rejection_gamma.py` & `pyro-ppl-1.9.0/pyro/distributions/testing/rejection_gamma.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/testing/special.py` & `pyro-ppl-1.9.0/pyro/distributions/testing/special.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/torch.py` & `pyro-ppl-1.9.0/pyro/distributions/torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,9 +381,12 @@
     {0}
     ----------------------------------------------------------------
     .. autoclass:: pyro.distributions.{0}
     """.format(
             _name
         )
         for _name in sorted(__all__)
+        # Work around sphinx autodoc error in case two InverseGamma's are defined:
+        # "duplicate object description of pyro.distributions.InverseGamma"
+        if _name != "InverseGamma"
     ]
 )
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/torch_distribution.py` & `pyro-ppl-1.9.0/pyro/distributions/torch_distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 import warnings
 from collections import OrderedDict
+from typing import Callable
 
 import torch
 from torch.distributions.kl import kl_divergence, register_kl
 
 import pyro.distributions.torch
 
 from . import constraints
 from .distribution import Distribution
 from .score_parts import ScoreParts
 from .util import broadcast_shape, scale_and_mask
 
 
-class TorchDistributionMixin(Distribution):
+class TorchDistributionMixin(Distribution, Callable):
     """
     Mixin to provide Pyro compatibility for PyTorch distributions.
 
     You should instead use `TorchDistribution` for new distribution classes.
 
     This is mainly useful for wrapping existing PyTorch distributions for
     use in Pyro.  Derived classes must first inherit from
     :class:`torch.distributions.distribution.Distribution` and then inherit
     from :class:`TorchDistributionMixin`.
     """
 
-    def __call__(self, sample_shape=torch.Size()):
+    def __call__(self, sample_shape: torch.Size = torch.Size()) -> torch.Tensor:
         """
         Samples a random value.
 
         This is reparameterized whenever possible, calling
         :meth:`~torch.distributions.distribution.Distribution.rsample` for
         reparameterized distributions and
         :meth:`~torch.distributions.distribution.Distribution.sample` for
@@ -47,15 +48,31 @@
         return (
             self.rsample(sample_shape)
             if self.has_rsample
             else self.sample(sample_shape)
         )
 
     @property
-    def event_dim(self):
+    def batch_shape(self) -> torch.Size:
+        """
+        :return: The shape over which parameters are batched.
+        :rtype: torch.Size
+        """
+        raise NotImplementedError
+
+    @property
+    def event_shape(self) -> torch.Size:
+        """
+        :return: The shape of a single sample from the distribution (without batching).
+        :rtype: torch.Size
+        """
+        raise NotImplementedError
+
+    @property
+    def event_dim(self) -> int:
         """
         :return: Number of dimensions of individual events.
         :rtype: int
         """
         return len(self.event_shape)
 
     def shape(self, sample_shape=torch.Size()):
@@ -98,15 +115,15 @@
         for name, shape in arg_shapes.items():
             event_dim = cls.arg_constraints.get(name, constraints.real).event_dim
             batch_shapes.append(shape[: len(shape) - event_dim])
         batch_shape = torch.Size(broadcast_shape(*batch_shapes))
         event_shape = torch.Size()
         return batch_shape, event_shape
 
-    def expand(self, batch_shape, _instance=None):
+    def expand(self, batch_shape, _instance=None) -> "ExpandedDistribution":
         """
         Returns a new :class:`ExpandedDistribution` instance with batch
         dimensions expanded to `batch_shape`.
 
         :param tuple batch_shape: batch shape to expand to.
         :param _instance: unused argument for compatibility with
             :meth:`torch.distributions.Distribution.expand`
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/torch_patch.py` & `pyro-ppl-1.9.0/pyro/distributions/torch_patch.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/torch_transform.py` & `pyro-ppl-1.9.0/pyro/distributions/torch_transform.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/__init__.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 from .normalize import Normalize
 from .ordered import OrderedTransform
 from .permute import Permute, permute
 from .planar import ConditionalPlanar, Planar, conditional_planar, planar
 from .polynomial import Polynomial, polynomial
 from .power import PositivePowerTransform
 from .radial import ConditionalRadial, Radial, conditional_radial, radial
+from .simplex_to_ordered import SimplexToOrderedTransform
 from .softplus import SoftplusLowerCholeskyTransform, SoftplusTransform
 from .spline import ConditionalSpline, Spline, conditional_spline, spline
 from .spline_autoregressive import (
     ConditionalSplineAutoregressive,
     SplineAutoregressive,
     conditional_spline_autoregressive,
     spline_autoregressive,
@@ -180,14 +181,15 @@
     "Normalize",
     "OrderedTransform",
     "Permute",
     "Planar",
     "Polynomial",
     "PositivePowerTransform",
     "Radial",
+    "SimplexToOrderedTransform",
     "SoftplusLowerCholeskyTransform",
     "SoftplusTransform",
     "Spline",
     "SplineAutoregressive",
     "SplineCoupling",
     "Sylvester",
     "affine_autoregressive",
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/affine_autoregressive.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/affine_autoregressive.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/affine_coupling.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/affine_coupling.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/basic.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # TODO: Move upstream
 
 
 class ELUTransform(Transform):
     r"""
     Bijective transform via the mapping :math:`y = \text{ELU}(x)`.
     """
+
     domain = constraints.real
     codomain = constraints.positive
     bijective = True
     sign = +1
 
     def __eq__(self, other):
         return isinstance(other, ELUTransform)
@@ -48,16 +49,17 @@
 # TODO: Move upstream
 
 
 class LeakyReLUTransform(Transform):
     r"""
     Bijective transform via the mapping :math:`y = \text{LeakyReLU}(x)`.
     """
+
     domain = constraints.real
-    codomain = constraints.positive
+    codomain = constraints.real
     bijective = True
     sign = +1
 
     def __eq__(self, other):
         return isinstance(other, LeakyReLUTransform)
 
     def _call(self, x):
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/batchnorm.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/batchnorm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/block_autoregressive.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/block_autoregressive.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 
     References:
 
     [1] Nicola De Cao, Ivan Titov, Wilker Aziz. Block Neural Autoregressive Flow.
     [arXiv:1904.04676]
 
     """
+
     domain = constraints.real_vector
     codomain = constraints.real_vector
     bijective = True
     autoregressive = True
 
     def __init__(
         self, input_dim, hidden_factors=[8, 8], activation="tanh", residual=None
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/cholesky.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/cholesky.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 
 class CholeskyTransform(Transform):
     r"""
     Transform via the mapping :math:`y = safe_cholesky(x)`, where `x` is a
     positive definite matrix.
     """
+
     bijective = True
     domain = constraints.positive_definite
     codomain = constraints.lower_cholesky
 
     def __eq__(self, other):
         return isinstance(other, CholeskyTransform)
 
@@ -47,14 +48,15 @@
 
 
 class CorrMatrixCholeskyTransform(CholeskyTransform):
     r"""
     Transform via the mapping :math:`y = safe_cholesky(x)`, where `x` is a
     correlation matrix.
     """
+
     bijective = True
     domain = constraints.corr_matrix
     # TODO: change corr_cholesky_constraint to corr_cholesky when the latter is availabler
     codomain = constraints.corr_cholesky_constraint
 
     def __eq__(self, other):
         return isinstance(other, CorrMatrixCholeskyTransform)
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/discrete_cosine.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/discrete_cosine.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/generalized_channel_permute.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/generalized_channel_permute.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/haar.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/haar.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/householder.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/householder.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/lower_cholesky_affine.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/lower_cholesky_affine.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/matrix_exponential.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/matrix_exponential.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/neural_autoregressive.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/neural_autoregressive.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/normalize.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/normalize.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/ordered.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/ordered.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/permute.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/permute.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     :param permutation: a permutation ordering that is applied to the inputs.
     :type permutation: torch.LongTensor
     :param dim: the tensor dimension to permute. This value must be negative and
         defines the event dim as `abs(dim)`.
     :type dim: int
 
     """
+
     bijective = True
     volume_preserving = True
 
     def __init__(self, permutation, *, dim=-1, cache_size=1):
         super().__init__(cache_size=cache_size)
 
         if dim >= 0:
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/planar.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/planar.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/polynomial.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/polynomial.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/power.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/power.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
     Whereas :class:`~torch.distributions.transforms.PowerTransform` allows
     arbitrary ``exponent`` and restricts domain and codomain to postive values,
     this class restricts ``exponent > 0`` and allows real domain and codomain.
 
     .. warning:: The Jacobian is typically zero or infinite at the origin.
     """
+
     domain = constraints.real
     codomain = constraints.real
     bijective = True
     sign = +1
 
     def __init__(self, exponent, *, cache_size=0, validate_args=None):
         super().__init__(cache_size=cache_size)
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/radial.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/radial.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/softplus.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/softplus.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 
 # Backport of https://github.com/pytorch/pytorch/pull/52300
 class SoftplusTransform(Transform):
     r"""
     Transform via the mapping :math:`\text{Softplus}(x) = \log(1 + \exp(x))`.
     """
+
     domain = constraints.real
     codomain = constraints.positive
     bijective = True
     sign = +1
 
     def __eq__(self, other):
         return isinstance(other, SoftplusTransform)
```

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/spline.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/spline.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/spline_autoregressive.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/spline_autoregressive.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/spline_coupling.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/spline_coupling.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/sylvester.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/sylvester.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/transforms/unit_cholesky.py` & `pyro-ppl-1.9.0/pyro/distributions/transforms/unit_cholesky.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/unit.py` & `pyro-ppl-1.9.0/pyro/distributions/unit.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/util.py` & `pyro-ppl-1.9.0/pyro/distributions/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/von_mises_3d.py` & `pyro-ppl-1.9.0/pyro/distributions/von_mises_3d.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/distributions/zero_inflated.py` & `pyro-ppl-1.9.0/pyro/distributions/zero_inflated.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,19 +56,19 @@
 
     @constraints.dependent_property
     def support(self):
         return self.base_dist.support
 
     @lazy_property
     def gate(self):
-        return logits_to_probs(self.gate_logits)
+        return logits_to_probs(self.gate_logits, is_binary=True)
 
     @lazy_property
     def gate_logits(self):
-        return probs_to_logits(self.gate)
+        return probs_to_logits(self.gate, is_binary=True)
 
     def log_prob(self, value):
         if self._validate_args:
             self._validate_sample(value)
 
         if "gate" in self.__dict__:
             gate, value = broadcast_all(self.gate, value)
```

### Comparing `pyro-ppl-1.8.6/pyro/infer/__init__.py` & `pyro-ppl-1.9.0/pyro/infer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pyro.infer.elbo import ELBO
 from pyro.infer.energy_distance import EnergyDistance
 from pyro.infer.enum import config_enumerate
 from pyro.infer.importance import Importance
 from pyro.infer.mcmc.api import MCMC
 from pyro.infer.mcmc.hmc import HMC
 from pyro.infer.mcmc.nuts import NUTS
+from pyro.infer.mcmc.rwkernel import RandomWalkKernel
 from pyro.infer.predictive import Predictive
 from pyro.infer.renyi_elbo import RenyiELBO
 from pyro.infer.rws import ReweightedWakeSleep
 from pyro.infer.smcfilter import SMCFilter
 from pyro.infer.svgd import SVGD, IMQSteinKernel, RBFSteinKernel
 from pyro.infer.svi import SVI
 from pyro.infer.trace_elbo import JitTrace_ELBO, Trace_ELBO
@@ -41,14 +42,15 @@
     "JitTraceEnum_ELBO",
     "JitTraceGraph_ELBO",
     "JitTraceMeanField_ELBO",
     "JitTrace_ELBO",
     "MCMC",
     "NUTS",
     "Predictive",
+    "RandomWalkKernel",
     "RBFSteinKernel",
     "RenyiELBO",
     "ReweightedWakeSleep",
     "SMCFilter",
     "SVGD",
     "SVI",
     "TraceTMC_ELBO",
```

### Comparing `pyro-ppl-1.8.6/pyro/infer/abstract_infer.py` & `pyro-ppl-1.9.0/pyro/infer/abstract_infer.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/autoguide/__init__.py` & `pyro-ppl-1.9.0/pyro/infer/autoguide/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/autoguide/effect.py` & `pyro-ppl-1.9.0/pyro/infer/autoguide/effect.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     @torch.no_grad()
     def _adjust_plates(self, value: torch.Tensor, event_dim: int) -> torch.Tensor:
         """
         Adjusts plates for generating initial values of parameters.
         """
         for f in get_plates():
-            full_size = getattr(f, "full_size", f.size)
+            full_size = f.full_size or f.size
             dim = f.dim - event_dim
             if f in self._outer_plates or f.name in self.amortized_plates:
                 if -value.dim() <= dim:
                     value = value.mean(dim, keepdim=True)
             elif f.size != full_size:
                 value = periodic_repeat(value, full_size, dim).contiguous()
         for dim in range(value.dim() - event_dim):
```

### Comparing `pyro-ppl-1.8.6/pyro/infer/autoguide/gaussian.py` & `pyro-ppl-1.9.0/pyro/infer/autoguide/gaussian.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,17 +371,17 @@
                 v_index = _break_plates(v_index, self._plates[v], self._plates[d])
 
                 # Scatter global indices into the [u,v] block.
                 u_start = local_offsets[u]
                 u_stop = u_start + u_index.size(-1)
                 v_start = local_offsets[v]
                 v_stop = v_start + v_index.size(-1)
-                index2[
-                    ..., u_start:u_stop, v_start:v_stop
-                ] = self._dense_size * u_index.unsqueeze(-1) + v_index.unsqueeze(-2)
+                index2[..., u_start:u_stop, v_start:v_stop] = (
+                    self._dense_size * u_index.unsqueeze(-1) + v_index.unsqueeze(-2)
+                )
 
             self._dense_scatter[d] = index1.reshape(-1), index2.reshape(-1)
 
     def _sample_aux_values(self, *, temperature: float) -> Dict[str, torch.Tensor]:
         mvn = self._dense_get_mvn()
         if temperature == 0:
             # Simply return the mode.
```

### Comparing `pyro-ppl-1.8.6/pyro/infer/autoguide/guides.py` & `pyro-ppl-1.9.0/pyro/infer/autoguide/guides.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                     plates = [plates]
                 assert all(
                     isinstance(p, pyro.plate) for p in plates
                 ), "create_plates() returned a non-plate"
                 self.plates = {p.name: p for p in plates}
             for name, frame in sorted(self._prototype_frames.items()):
                 if name not in self.plates:
-                    full_size = getattr(frame, "full_size", frame.size)
+                    full_size = frame.full_size or frame.size
                     self.plates[name] = pyro.plate(
                         name, full_size, dim=frame.dim, subsample_size=frame.size
                     )
         else:
             assert (
                 self.create_plates is None
             ), "Cannot pass create_plates() to non-master guide"
@@ -178,15 +178,15 @@
         :rtype: dict
         """
         raise NotImplementedError
 
 
 class AutoGuideList(AutoGuide, nn.ModuleList):
     """
-    Container class to combine multiple automatic guides.
+    Container class to combine multiple automatic or custom guides.
 
     Example usage::
 
         guide = AutoGuideList(my_model)
         guide.append(AutoDiagonalNormal(poutine.block(model, hide=["assignment"])))
         guide.append(AutoDiscreteParallel(poutine.block(model, expose=["assignment"])))
         svi = SVI(model, guide, optim, Trace_ELBO())
@@ -199,15 +199,15 @@
             self_site = self.prototype_trace.nodes[name]
             assert part_site["fn"].batch_shape == self_site["fn"].batch_shape
             assert part_site["fn"].event_shape == self_site["fn"].event_shape
             assert part_site["value"].shape == self_site["value"].shape
 
     def append(self, part):
         """
-        Add an automatic guide for part of the model. The guide should
+        Add an automatic or custom guide for part of the model. The guide should
         have been created by blocking the model to restrict to a subset of
         sample sites. No two parts should operate on any one sample site.
 
         :param part: a partial guide to add
         :type part: AutoGuide or callable
         """
         if not isinstance(part, AutoGuide):
@@ -282,23 +282,23 @@
     This is used internally for composing autoguides with custom user-defined
     guides that are simple callables, e.g.::
 
         def my_local_guide(*args, **kwargs):
             ...
 
         guide = AutoGuideList(model)
-        guide.add(AutoDelta(poutine.block(model, expose=['my_global_param']))
-        guide.add(my_local_guide)  # automatically wrapped in an AutoCallable
+        guide.append(AutoDelta(poutine.block(model, expose=['my_global_param']))
+        guide.append(my_local_guide)  # automatically wrapped in an AutoCallable
 
     To specify a median callable, you can instead::
 
         def my_local_median(*args, **kwargs)
             ...
 
-        guide.add(AutoCallable(model, my_local_guide, my_local_median))
+        guide.append(AutoCallable(model, my_local_guide, my_local_median))
 
     For more complex guides that need e.g. access to plates, users should
     instead subclass ``AutoGuide``.
 
     :param callable model: a Pyro model
     :param callable guide: a Pyro guide (typically over only part of the model)
     :param callable median: an optional callable returning a dict mapping
@@ -359,15 +359,15 @@
         # Initialize guide params
         for name, site in self.prototype_trace.iter_stochastic_nodes():
             value = site["value"].detach()
             event_dim = site["fn"].event_dim
 
             # If subsampling, repeat init_value to full size.
             for frame in site["cond_indep_stack"]:
-                full_size = getattr(frame, "full_size", frame.size)
+                full_size = frame.full_size or frame.size
                 if full_size != frame.size:
                     dim = frame.dim - event_dim
                     value = periodic_repeat(value, full_size, dim).contiguous()
 
             value = PyroParam(value, site["fn"].support, event_dim)
             with helpful_support_errors(site):
                 deep_setattr(self, name, value)
@@ -471,15 +471,15 @@
                     biject_to(site["fn"].support).inv(site["value"].detach()).detach()
                 )
             event_dim = site["fn"].event_dim + init_loc.dim() - site["value"].dim()
             self._event_dims[name] = event_dim
 
             # If subsampling, repeat init_value to full size.
             for frame in site["cond_indep_stack"]:
-                full_size = getattr(frame, "full_size", frame.size)
+                full_size = frame.full_size or frame.size
                 if full_size != frame.size:
                     dim = frame.dim - event_dim
                     init_loc = periodic_repeat(init_loc, full_size, dim).contiguous()
             init_scale = torch.full_like(init_loc, self._init_scale)
 
             deep_setattr(
                 self.locs, name, PyroParam(init_loc, constraints.real, event_dim)
```

### Comparing `pyro-ppl-1.8.6/pyro/infer/autoguide/initialization.py` & `pyro-ppl-1.9.0/pyro/infer/autoguide/initialization.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/autoguide/structured.py` & `pyro-ppl-1.9.0/pyro/infer/autoguide/structured.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/autoguide/utils.py` & `pyro-ppl-1.9.0/pyro/infer/autoguide/utils.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/csis.py` & `pyro-ppl-1.9.0/pyro/infer/csis.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/discrete.py` & `pyro-ppl-1.9.0/pyro/infer/discrete.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/elbo.py` & `pyro-ppl-1.9.0/pyro/infer/elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/energy_distance.py` & `pyro-ppl-1.9.0/pyro/infer/energy_distance.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/enum.py` & `pyro-ppl-1.9.0/pyro/infer/enum.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/importance.py` & `pyro-ppl-1.9.0/pyro/infer/importance.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/inspect.py` & `pyro-ppl-1.9.0/pyro/infer/inspect.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 import itertools
 import os
 from collections import defaultdict
 from pathlib import Path
 from types import SimpleNamespace
-from typing import Callable, Dict, List, Optional, Union
+from typing import Callable, Collection, Dict, List, Optional, Union
 
 import torch
 
 import pyro
 import pyro.distributions as dist
 import pyro.poutine as poutine
 from pyro.ops.provenance import ProvenanceTensor, detach_provenance, get_provenance
@@ -19,37 +19,50 @@
 
 try:
     import graphviz
 except ImportError:
     graphviz = SimpleNamespace(Digraph=object)  # for type hints
 
 
-def is_sample_site(msg):
+def is_sample_site(msg, *, include_deterministic=False):
     if msg["type"] != "sample":
         return False
     if site_is_subsample(msg):
         return False
 
-    # Ignore masked observations.
-    if msg["is_observed"] and msg["mask"] is False:
-        return False
+    if not include_deterministic:
+        # Ignore masked observations.
+        if msg["is_observed"] and msg["mask"] is False:
+            return False
 
-    # Exclude deterministic sites.
-    fn = msg["fn"]
-    while hasattr(fn, "base_dist"):
-        fn = fn.base_dist
-    if type(fn).__name__ == "Delta":
-        return False
+        # Exclude deterministic sites.
+        fn = msg["fn"]
+        while hasattr(fn, "base_dist"):
+            fn = fn.base_dist
+        if type(fn).__name__ == "Delta":
+            return False
 
     return True
 
 
+def site_is_deterministic(msg: dict) -> bool:
+    return msg["type"] == "sample" and msg["infer"].get("_deterministic", False)
+
+
 class TrackProvenance(Messenger):
+    def __init__(self, *, include_deterministic=False):
+        self.include_deterministic = include_deterministic
+
     def _pyro_post_sample(self, msg):
-        if is_sample_site(msg):
+        if self.include_deterministic and site_is_deterministic(msg):
+            provenance = frozenset({msg["name"]})  # track only direct dependencies
+            value = detach_provenance(msg["value"])
+            msg["value"] = ProvenanceTensor(value, provenance)
+
+        elif is_sample_site(msg, include_deterministic=self.include_deterministic):
             provenance = frozenset({msg["name"]})  # track only direct dependencies
             value = detach_provenance(msg["value"])
             msg["value"] = ProvenanceTensor(value, provenance)
 
     def _pyro_post_param(self, msg):
         if msg["type"] == "param":
             provenance = frozenset({msg["name"]})  # track only direct dependencies
@@ -58,14 +71,15 @@
 
 
 @torch.enable_grad()
 def get_dependencies(
     model: Callable,
     model_args: Optional[tuple] = None,
     model_kwargs: Optional[dict] = None,
+    include_deterministic: bool = False,
 ) -> Dict[str, object]:
     r"""
     Infers dependency structure about a conditioned model.
 
     This returns a nested dictionary with structure like::
 
         {
@@ -165,25 +179,26 @@
     [1] S.Webb, A.Goliński, R.Zinkov, N.Siddharth, T.Rainforth, Y.W.Teh, F.Wood (2018)
         "Faithful inversion of generative models for effective amortized inference"
         https://dl.acm.org/doi/10.5555/3327144.3327229
 
     :param callable model: A model.
     :param tuple model_args: Optional tuple of model args.
     :param dict model_kwargs: Optional dict of model kwargs.
+    :param bool include_deterministic: Whether to include deterministic sites.
     :returns: A dictionary of metadata (see above).
     :rtype: dict
     """
     if model_args is None:
         model_args = ()
     if model_kwargs is None:
         model_kwargs = {}
 
     # Collect sites with tracked provenance.
     with torch.random.fork_rng(), torch.no_grad(), pyro.validation_enabled(False):
-        with TrackProvenance():
+        with TrackProvenance(include_deterministic=include_deterministic):
             trace = poutine.trace(model).get_trace(*model_args, **model_kwargs)
     sample_sites = [msg for msg in trace.nodes.values() if is_sample_site(msg)]
 
     # Collect observations.
     observed = {msg["name"] for msg in sample_sites if msg["is_observed"]}
     plates = {
         msg["name"]: {f.name for f in msg["cond_indep_stack"] if f.vectorized}
@@ -234,14 +249,15 @@
     }
 
 
 def get_model_relations(
     model: Callable,
     model_args: Optional[tuple] = None,
     model_kwargs: Optional[dict] = None,
+    include_deterministic: bool = False,
 ):
     """
     Infer relations of RVs and plates from given model and optionally data.
     See https://github.com/pyro-ppl/pyro/issues/949 for more details.
 
     This returns a dictionary with keys:
 
@@ -267,25 +283,26 @@
          'sample_dist': {'m': 'Normal', 'sd': 'LogNormal', 'obs': 'Normal'},
          'plate_sample': {'N': ['obs']},
          'observed': ['obs']}
 
     :param callable model: A model to inspect.
     :param model_args: Optional tuple of model args.
     :param model_kwargs: Optional dict of model kwargs.
+    :param bool include_deterministic: Whether to include deterministic sites.
     :rtype: dict
     """
     if model_args is None:
         model_args = ()
     if model_kwargs is None:
         model_kwargs = {}
     assert isinstance(model_args, tuple)
     assert isinstance(model_kwargs, dict)
 
     with torch.random.fork_rng(), torch.no_grad(), pyro.validation_enabled(False):
-        with TrackProvenance():
+        with TrackProvenance(include_deterministic=include_deterministic):
             trace = poutine.trace(model).get_trace(*model_args, **model_kwargs)
 
     sample_sample = {}
     sample_param = {}
     sample_dist = {}
     param_constraint = {}
     plate_sample = defaultdict(list)
@@ -297,27 +314,36 @@
     for name, site in trace.nodes.items():
         if site["type"] == "param":
             param_constraint[name] = str(site["kwargs"]["constraint"])
 
         if site["type"] != "sample" or site_is_subsample(site):
             continue
 
+        provenance = get_provenance(
+            site["fn"].log_prob(site["value"])
+            if not site_is_deterministic(site)
+            else site["fn"].base_dist.log_prob(site["value"])
+        )
         sample_sample[name] = [
             upstream
-            for upstream in get_provenance(site["fn"].log_prob(site["value"]))
+            for upstream in provenance
             if upstream != name and _get_type_from_frozenname(upstream) == "sample"
         ]
 
         sample_param[name] = [
             upstream
             for upstream in get_provenance(site["fn"].log_prob(site["value"]))
             if upstream != name and _get_type_from_frozenname(upstream) == "param"
         ]
 
-        sample_dist[name] = _get_dist_name(site["fn"])
+        sample_dist[name] = (
+            _get_dist_name(site["fn"])
+            if not site_is_deterministic(site)
+            else "Deterministic"
+        )
         for frame in site["cond_indep_stack"]:
             plate_sample[frame.name].append(name)
         if site["is_observed"]:
             observed.append(name)
 
     def _resolve_plate_samples(plate_samples):
         for p, pv in plate_samples.items():
@@ -328,18 +354,23 @@
                     plate_samples_ = plate_samples.copy()
                     plate_samples_[q] = pv & qv
                     plate_samples_[q + "__CLONE"] = qv - pv
                     return _resolve_plate_samples(plate_samples_)
         return plate_samples
 
     plate_sample = _resolve_plate_samples(plate_sample)
-    # convert set to list to keep order of variables
-    plate_sample = {
-        k: [name for name in trace.nodes if name in v] for k, v in plate_sample.items()
-    }
+
+    # Normalize order of variables.
+    def sort_by_time(names: Collection[str]) -> List[str]:
+        return [name for name in trace.nodes if name in names]
+
+    sample_sample = {k: sort_by_time(v) for k, v in sample_sample.items()}
+    sample_param = {k: sort_by_time(v) for k, v in sample_param.items()}
+    plate_sample = {k: sort_by_time(v) for k, v in plate_sample.items()}
+    observed = sort_by_time(observed)
 
     return {
         "sample_sample": sample_sample,
         "sample_param": sample_param,
         "sample_dist": sample_dist,
         "param_constraint": param_constraint,
         "plate_sample": dict(plate_sample),
@@ -506,19 +537,30 @@
 
         for rv in rv_list:
             color = colors[node_data[rv]["is_observed"]]
 
             # For sample_nodes - ellipse
             if node_data[rv]["distribution"]:
                 shape = "ellipse"
+                rv_label = rv
 
             # For param_nodes - No shape
             else:
                 shape = "plain"
-            cur_graph.node(rv, label=rv, shape=shape, style="filled", fillcolor=color)
+                rv_label = rv.replace("$params", "")
+
+            # use different symbol for Deterministic site
+            node_style = (
+                "filled,dashed"
+                if node_data[rv]["distribution"] == "Deterministic"
+                else "filled"
+            )
+            cur_graph.node(
+                rv, label=rv_label, shape=shape, style=node_style, fillcolor=color
+            )
 
     # add leaf nodes first
     while len(plate_data) >= 1:
         for plate, data in plate_data.items():
             parent_plate = data["parent"]
             is_leaf = True
 
@@ -556,14 +598,15 @@
 def render_model(
     model: Callable,
     model_args: Optional[Union[tuple, List[tuple]]] = None,
     model_kwargs: Optional[Union[dict, List[dict]]] = None,
     filename: Optional[str] = None,
     render_distributions: bool = False,
     render_params: bool = False,
+    render_deterministic: bool = False,
 ) -> "graphviz.Digraph":
     """
     Renders a model using `graphviz <https://graphviz.org>`_ .
 
     If ``filename`` is provided, this saves an image; otherwise this draws the
     graph. For example usage see the
     `model rendering tutorial <https://pyro.ai/examples/model_rendering.html>`_ .
@@ -573,29 +616,39 @@
         list of tuples for semisupervised models.
     :param model_kwargs: Dict of keyword arguments to pass to the model, or
         list of dicts for semisupervised models.
     :param str filename: Name of file or path to file to save rendered model in.
     :param bool render_distributions: Whether to include RV distribution
         annotations (and param constraints) in the plot.
     :param bool render_params: Whether to show params inthe plot.
+    :param bool render_deterministic: Whether to include deterministic sites.
     :returns: A model graph.
     :rtype: graphviz.Digraph
     """
     # Get model relations.
     if not isinstance(model_args, list) and not isinstance(model_kwargs, list):
-        relations = [get_model_relations(model, model_args, model_kwargs)]
+        relations = [
+            get_model_relations(
+                model,
+                model_args,
+                model_kwargs,
+                include_deterministic=render_deterministic,
+            )
+        ]
     else:  # semisupervised
         if isinstance(model_args, list):
             if not isinstance(model_kwargs, list):
                 model_kwargs = [model_kwargs] * len(model_args)
         elif not isinstance(model_args, list):
             model_args = [model_args] * len(model_kwargs)
         assert len(model_args) == len(model_kwargs)
         relations = [
-            get_model_relations(model, args, kwargs)
+            get_model_relations(
+                model, args, kwargs, include_deterministic=render_deterministic
+            )
             for args, kwargs in zip(model_args, model_kwargs)
         ]
 
     # Get graph specifications.
     graph_specs = [
         generate_graph_specification(r, render_params=render_params) for r in relations
     ]
```

### Comparing `pyro-ppl-1.8.6/pyro/infer/mcmc/adaptation.py` & `pyro-ppl-1.9.0/pyro/infer/mcmc/adaptation.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/mcmc/api.py` & `pyro-ppl-1.9.0/pyro/infer/mcmc/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,21 +103,23 @@
         if initial_params is not None:
             self.kernel.initial_params = initial_params
         self.num_samples = num_samples
         self.warmup_steps = warmup_steps
         self.rng_seed = (torch.initial_seed() + chain_id) % MAX_SEED
         self.log_queue = log_queue
         self.result_queue = result_queue
-        self.default_tensor_type = torch.Tensor().type()
+        self.default_dtype = torch.Tensor().dtype
+        self.default_device = torch.Tensor().device
         self.hook = hook
         self.event = event
 
     def run(self, *args, **kwargs):
         pyro.set_rng_seed(self.rng_seed)
-        torch.set_default_tensor_type(self.default_tensor_type)
+        torch.set_default_dtype(self.default_dtype)
+        torch.set_default_device(self.default_device)
         kwargs = kwargs
         logger = logging.getLogger("pyro.infer.mcmc")
         logger_id = "CHAIN:{}".format(self.chain_id)
         log_queue = self.log_queue
         logger = initialize_logger(logger, logger_id, None, log_queue)
         logging_hook = _add_logging_hook(logger, None, self.hook)
```

### Comparing `pyro-ppl-1.8.6/pyro/infer/mcmc/hmc.py` & `pyro-ppl-1.9.0/pyro/infer/mcmc/hmc.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/mcmc/logger.py` & `pyro-ppl-1.9.0/pyro/infer/mcmc/logger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/mcmc/mcmc_kernel.py` & `pyro-ppl-1.9.0/pyro/infer/mcmc/mcmc_kernel.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/mcmc/nuts.py` & `pyro-ppl-1.9.0/pyro/infer/mcmc/nuts.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/mcmc/util.py` & `pyro-ppl-1.9.0/pyro/infer/mcmc/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/predictive.py` & `pyro-ppl-1.9.0/pyro/infer/predictive.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/renyi_elbo.py` & `pyro-ppl-1.9.0/pyro/infer/renyi_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/reparam/__init__.py` & `pyro-ppl-1.9.0/pyro/infer/reparam/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/reparam/conjugate.py` & `pyro-ppl-1.9.0/pyro/infer/reparam/conjugate.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/reparam/discrete_cosine.py` & `pyro-ppl-1.9.0/pyro/infer/reparam/discrete_cosine.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/reparam/haar.py` & `pyro-ppl-1.9.0/pyro/infer/reparam/haar.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/reparam/hmm.py` & `pyro-ppl-1.9.0/pyro/infer/reparam/hmm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/reparam/loc_scale.py` & `pyro-ppl-1.9.0/pyro/infer/reparam/loc_scale.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/reparam/neutra.py` & `pyro-ppl-1.9.0/pyro/infer/reparam/neutra.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/reparam/projected_normal.py` & `pyro-ppl-1.9.0/pyro/infer/reparam/projected_normal.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/reparam/reparam.py` & `pyro-ppl-1.9.0/pyro/infer/reparam/reparam.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,37 +2,28 @@
 # SPDX-License-Identifier: Apache-2.0
 
 import warnings
 from abc import ABC
 from typing import Callable, Optional
 
 import torch
+from typing_extensions import TypedDict
 
-try:
-    from typing import TypedDict
-except ImportError:
-
-    def TypedDict(*args, **kwargs):
-        return dict
-
-
-ReparamMessage = TypedDict(
-    "ReparamMessage",
-    name=str,
-    fn=Callable,
-    value=Optional[torch.Tensor],
-    is_observed=Optional[bool],
-)
-
-ReparamResult = TypedDict(
-    "ReparamResult",
-    fn=Callable,
-    value=Optional[torch.Tensor],
-    is_observed=Optional[bool],
-)
+
+class ReparamMessage(TypedDict):
+    name: str
+    fn: Callable
+    value: Optional[torch.Tensor]
+    is_observed: Optional[bool]
+
+
+class ReparamResult(TypedDict):
+    fn: Callable
+    value: Optional[torch.Tensor]
+    is_observed: bool
 
 
 class Reparam(ABC):
     """
     Abstract base class for reparameterizers.
 
     Derived classes should implement :meth:`apply`.
```

### Comparing `pyro-ppl-1.8.6/pyro/infer/reparam/softmax.py` & `pyro-ppl-1.9.0/pyro/infer/reparam/softmax.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/reparam/split.py` & `pyro-ppl-1.9.0/pyro/infer/reparam/split.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/reparam/stable.py` & `pyro-ppl-1.9.0/pyro/infer/reparam/stable.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     This reparameterization works only for latent variables, not likelihoods.
     For likelihood-compatible reparameterization see
     :class:`SymmetricStableReparam` or :class:`StableReparam` .
 
     [1] J.P. Nolan (2017).
         Stable Distributions: Models for Heavy Tailed Data.
-        http://fs2.american.edu/jpnolan/www/stable/chap1.pdf
+        https://edspace.american.edu/jpnolan/wp-content/uploads/sites/1720/2020/09/Chap1.pdf
     """
 
     def apply(self, msg):
         name = msg["name"]
         fn = msg["fn"]
         # ignore msg["value"]
         is_observed = msg["is_observed"]
```

### Comparing `pyro-ppl-1.8.6/pyro/infer/reparam/strategies.py` & `pyro-ppl-1.9.0/pyro/infer/reparam/strategies.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/reparam/structured.py` & `pyro-ppl-1.9.0/pyro/infer/reparam/structured.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/reparam/studentt.py` & `pyro-ppl-1.9.0/pyro/infer/reparam/studentt.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/reparam/transform.py` & `pyro-ppl-1.9.0/pyro/infer/reparam/transform.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/reparam/unit_jacobian.py` & `pyro-ppl-1.9.0/pyro/infer/reparam/unit_jacobian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/resampler.py` & `pyro-ppl-1.9.0/pyro/infer/resampler.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/rws.py` & `pyro-ppl-1.9.0/pyro/infer/rws.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,17 +199,20 @@
             sleep_phi_loss = -_log_q / self.num_sleep_particles
             warn_if_nan(sleep_phi_loss, "sleep phi loss")
 
         # compute phi loss
         phi_loss = (
             sleep_phi_loss
             if self.insomnia == 0
-            else wake_phi_loss
-            if self.insomnia == 1
-            else self.insomnia * wake_phi_loss + (1.0 - self.insomnia) * sleep_phi_loss
+            else (
+                wake_phi_loss
+                if self.insomnia == 1
+                else self.insomnia * wake_phi_loss
+                + (1.0 - self.insomnia) * sleep_phi_loss
+            )
         )
 
         return wake_theta_loss, phi_loss
 
     def loss(self, model, guide, *args, **kwargs):
         """
         :returns: returns model loss and guide loss
```

### Comparing `pyro-ppl-1.8.6/pyro/infer/smcfilter.py` & `pyro-ppl-1.9.0/pyro/infer/smcfilter.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/svgd.py` & `pyro-ppl-1.9.0/pyro/infer/svgd.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/svi.py` & `pyro-ppl-1.9.0/pyro/infer/svi.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/trace_elbo.py` & `pyro-ppl-1.9.0/pyro/infer/trace_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/trace_mean_field_elbo.py` & `pyro-ppl-1.9.0/pyro/infer/trace_mean_field_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/trace_mmd.py` & `pyro-ppl-1.9.0/pyro/infer/trace_mmd.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/trace_tail_adaptive_elbo.py` & `pyro-ppl-1.9.0/pyro/infer/trace_tail_adaptive_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/traceenum_elbo.py` & `pyro-ppl-1.9.0/pyro/infer/traceenum_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/tracegraph_elbo.py` & `pyro-ppl-1.9.0/pyro/infer/tracegraph_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/tracetmc_elbo.py` & `pyro-ppl-1.9.0/pyro/infer/tracetmc_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/infer/util.py` & `pyro-ppl-1.9.0/pyro/infer/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/nn/__init__.py` & `pyro-ppl-1.9.0/pyro/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/nn/auto_reg_nn.py` & `pyro-ppl-1.9.0/pyro/nn/auto_reg_nn.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/nn/dense_nn.py` & `pyro-ppl-1.9.0/pyro/nn/dense_nn.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/nn/module.py` & `pyro-ppl-1.9.0/pyro/nn/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import weakref
 from collections import OrderedDict, namedtuple
 
 import torch
 from torch.distributions import constraints, transform_to
 
 import pyro
+import pyro.params.param_store
 from pyro.ops.provenance import detach_provenance
 from pyro.poutine.runtime import _PYRO_PARAM_STORE
 
 _MODULE_LOCAL_PARAMS: bool = False
 
 
 @pyro.settings.register("module_local_params", __name__, "_MODULE_LOCAL_PARAMS")
@@ -470,43 +471,52 @@
     def __getattr__(self, name):
         # PyroParams trigger pyro.param statements.
         if "_pyro_params" in self.__dict__:
             _pyro_params = self.__dict__["_pyro_params"]
             if name in _pyro_params:
                 constraint, event_dim = _pyro_params[name]
                 unconstrained_value = getattr(self, name + "_unconstrained")
-                if self._pyro_context.active:
+                if self._pyro_context.active and not _is_module_local_param_enabled():
                     fullname = self._pyro_get_fullname(name)
                     if fullname in _PYRO_PARAM_STORE:
                         if (
                             _PYRO_PARAM_STORE._params[fullname]
                             is not unconstrained_value
                         ):
                             # Update PyroModule <--- ParamStore.
                             unconstrained_value = _PYRO_PARAM_STORE._params[fullname]
                             if not isinstance(unconstrained_value, torch.nn.Parameter):
                                 # Update PyroModule ---> ParamStore (type only; data is preserved).
                                 unconstrained_value = torch.nn.Parameter(
                                     unconstrained_value
                                 )
-                                _PYRO_PARAM_STORE._params[
-                                    fullname
-                                ] = unconstrained_value
+                                _PYRO_PARAM_STORE._params[fullname] = (
+                                    unconstrained_value
+                                )
                                 _PYRO_PARAM_STORE._param_to_name[
                                     unconstrained_value
                                 ] = fullname
                             super().__setattr__(
                                 name + "_unconstrained", unconstrained_value
                             )
                     else:
                         # Update PyroModule ---> ParamStore.
                         _PYRO_PARAM_STORE._constraints[fullname] = constraint
                         _PYRO_PARAM_STORE._params[fullname] = unconstrained_value
                         _PYRO_PARAM_STORE._param_to_name[unconstrained_value] = fullname
                     return pyro.param(fullname, event_dim=event_dim)
+                elif self._pyro_context.active and _is_module_local_param_enabled():
+                    # fake param statement to ensure any handlers of pyro.param are applied,
+                    # even though we don't use the contents of the local parameter store
+                    fullname = self._pyro_get_fullname(name)
+                    constrained_value = transform_to(constraint)(unconstrained_value)
+                    constrained_value.unconstrained = weakref.ref(unconstrained_value)
+                    return pyro.poutine.runtime.effectful(type="param")(
+                        lambda *_, **__: constrained_value
+                    )(fullname, event_dim=event_dim, name=fullname)
                 else:  # Cannot determine supermodule and hence cannot compute fullname.
                     constrained_value = transform_to(constraint)(unconstrained_value)
                     constrained_value.unconstrained = weakref.ref(unconstrained_value)
                     return constrained_value
 
         # PyroSample trigger pyro.sample statements.
         if "_pyro_samples" in self.__dict__:
@@ -530,28 +540,46 @@
 
         result = super().__getattr__(name)
 
         # Regular nn.Parameters trigger pyro.param statements.
         if isinstance(result, torch.nn.Parameter) and not name.endswith(
             "_unconstrained"
         ):
-            if self._pyro_context.active:
+            if self._pyro_context.active and not _is_module_local_param_enabled():
                 pyro.param(self._pyro_get_fullname(name), result)
+            elif self._pyro_context.active and _is_module_local_param_enabled():
+                # fake param statement to ensure any handlers of pyro.param are applied,
+                # even though we don't use the contents of the local parameter store
+                fullname = self._pyro_get_fullname(name)
+                pyro.poutine.runtime.effectful(type="param")(lambda *_, **__: result)(
+                    fullname, result, name=fullname
+                )
 
         if isinstance(result, torch.nn.Module):
             if isinstance(result, PyroModule):
                 if not result._pyro_name:
                     # Update sub-PyroModules that were converted from nn.Modules in-place.
                     result._pyro_set_supermodule(
                         _make_name(self._pyro_name, name), self._pyro_context
                     )
             else:
                 # Regular nn.Modules trigger pyro.module statements.
-                if self._pyro_context.active:
+                if self._pyro_context.active and not _is_module_local_param_enabled():
                     pyro.module(self._pyro_get_fullname(name), result)
+                elif self._pyro_context.active and _is_module_local_param_enabled():
+                    # fake module statement to ensure any handlers of pyro.module are applied,
+                    # even though we don't use the contents of the local parameter store
+                    fullname_module = self._pyro_get_fullname(name)
+                    for param_name, param_value in result.named_parameters():
+                        fullname_param = pyro.params.param_store.param_with_module_name(
+                            fullname_module, param_name
+                        )
+                        pyro.poutine.runtime.effectful(type="param")(
+                            lambda *_, **__: param_value
+                        )(fullname_param, param_value, name=fullname_param)
 
         return result
 
     def __setattr__(self, name, value):
         if isinstance(value, PyroModule):
             # Create a new sub PyroModule, overwriting any old value.
             try:
@@ -565,48 +593,72 @@
             # Create a new PyroParam, overwriting any old value.
             try:
                 delattr(self, name)
             except AttributeError:
                 pass
             constrained_value, constraint, event_dim = value
             self._pyro_params[name] = constraint, event_dim
-            if self._pyro_context.active:
+            if self._pyro_context.active and not _is_module_local_param_enabled():
                 fullname = self._pyro_get_fullname(name)
                 pyro.param(
                     fullname,
                     constrained_value,
                     constraint=constraint,
                     event_dim=event_dim,
                 )
                 constrained_value = detach_provenance(pyro.param(fullname))
                 unconstrained_value = constrained_value.unconstrained()
                 if not isinstance(unconstrained_value, torch.nn.Parameter):
                     # Update PyroModule ---> ParamStore (type only; data is preserved).
                     unconstrained_value = torch.nn.Parameter(unconstrained_value)
                     _PYRO_PARAM_STORE._params[fullname] = unconstrained_value
                     _PYRO_PARAM_STORE._param_to_name[unconstrained_value] = fullname
+            elif self._pyro_context.active and _is_module_local_param_enabled():
+                # fake param statement to ensure any handlers of pyro.param are applied,
+                # even though we don't use the contents of the local parameter store
+                fullname = self._pyro_get_fullname(name)
+                constrained_value = detach_provenance(
+                    pyro.poutine.runtime.effectful(type="param")(
+                        lambda *_, **__: constrained_value
+                    )(
+                        fullname,
+                        constraint=constraint,
+                        event_dim=event_dim,
+                        name=fullname,
+                    )
+                )
+                unconstrained_value = _unconstrain(constrained_value, constraint)
             else:  # Cannot determine supermodule and hence cannot compute fullname.
                 unconstrained_value = _unconstrain(constrained_value, constraint)
             super().__setattr__(name + "_unconstrained", unconstrained_value)
             return
 
         if isinstance(value, torch.nn.Parameter):
             # Create a new nn.Parameter, overwriting any old value.
             try:
                 delattr(self, name)
             except AttributeError:
                 pass
-            if self._pyro_context.active:
+            if self._pyro_context.active and not _is_module_local_param_enabled():
                 fullname = self._pyro_get_fullname(name)
                 value = pyro.param(fullname, value)
                 if not isinstance(value, torch.nn.Parameter):
                     # Update PyroModule ---> ParamStore (type only; data is preserved).
                     value = torch.nn.Parameter(detach_provenance(value))
                     _PYRO_PARAM_STORE._params[fullname] = value
                     _PYRO_PARAM_STORE._param_to_name[value] = fullname
+            elif self._pyro_context.active and _is_module_local_param_enabled():
+                # fake param statement to ensure any handlers of pyro.param are applied,
+                # even though we don't use the contents of the local parameter store
+                fullname = self._pyro_get_fullname(name)
+                value = detach_provenance(
+                    pyro.poutine.runtime.effectful(type="param")(
+                        lambda *_, **__: value
+                    )(fullname, value, constraint=constraints.real, name=fullname)
+                )
             super().__setattr__(name, value)
             return
 
         if isinstance(value, torch.Tensor):
             if name in self._pyro_params:
                 # Update value of an existing PyroParam.
                 constraint, event_dim = self._pyro_params[name]
```

### Comparing `pyro-ppl-1.8.6/pyro/ops/arrowhead.py` & `pyro-ppl-1.9.0/pyro/ops/arrowhead.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/contract.py` & `pyro-ppl-1.9.0/pyro/ops/contract.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/dual_averaging.py` & `pyro-ppl-1.9.0/pyro/ops/dual_averaging.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/einsum/__init__.py` & `pyro-ppl-1.9.0/pyro/ops/einsum/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/einsum/adjoint.py` & `pyro-ppl-1.9.0/pyro/ops/einsum/adjoint.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/einsum/torch_log.py` & `pyro-ppl-1.9.0/pyro/ops/einsum/torch_log.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/einsum/torch_map.py` & `pyro-ppl-1.9.0/pyro/ops/einsum/torch_map.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/einsum/torch_marginal.py` & `pyro-ppl-1.9.0/pyro/ops/einsum/torch_marginal.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/einsum/torch_sample.py` & `pyro-ppl-1.9.0/pyro/ops/einsum/torch_sample.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/einsum/util.py` & `pyro-ppl-1.9.0/pyro/ops/einsum/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/gamma_gaussian.py` & `pyro-ppl-1.9.0/pyro/ops/gamma_gaussian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/gaussian.py` & `pyro-ppl-1.9.0/pyro/ops/gaussian.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 import math
-from typing import Optional, Tuple
+from typing import Optional, Tuple, Union
 
 import torch
 from torch.distributions.utils import lazy_property
 from torch.nn.functional import pad
 
 from pyro.distributions.util import broadcast_shape
 from pyro.ops.tensor_utils import matmul, matvecmul, safe_cholesky, triangular_solve
@@ -107,30 +107,30 @@
         """
         assert isinstance(perm, torch.Tensor)
         assert perm.shape == (self.dim(),)
         info_vec = self.info_vec[..., perm]
         precision = self.precision[..., perm][..., perm, :]
         return Gaussian(self.log_normalizer, info_vec, precision)
 
-    def __add__(self, other: "Gaussian") -> "Gaussian":
+    def __add__(self, other: Union["Gaussian", int, float, torch.Tensor]) -> "Gaussian":
         """
         Adds two Gaussians in log-density space.
         """
         if isinstance(other, Gaussian):
             assert self.dim() == other.dim()
             return Gaussian(
                 self.log_normalizer + other.log_normalizer,
                 self.info_vec + other.info_vec,
                 self.precision + other.precision,
             )
         if isinstance(other, (int, float, torch.Tensor)):
             return Gaussian(self.log_normalizer + other, self.info_vec, self.precision)
         raise ValueError("Unsupported type: {}".format(type(other)))
 
-    def __sub__(self, other: "Gaussian") -> "Gaussian":
+    def __sub__(self, other: Union["Gaussian", int, float, torch.Tensor]) -> "Gaussian":
         if isinstance(other, (int, float, torch.Tensor)):
             return Gaussian(self.log_normalizer - other, self.info_vec, self.precision)
         raise ValueError("Unsupported type: {}".format(type(other)))
 
     def log_density(self, value: torch.Tensor) -> torch.Tensor:
         """
         Evaluate the log density of this Gaussian at a point value::
```

### Comparing `pyro-ppl-1.8.6/pyro/ops/hessian.py` & `pyro-ppl-1.9.0/pyro/ops/hessian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/indexing.py` & `pyro-ppl-1.9.0/pyro/ops/indexing.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/integrator.py` & `pyro-ppl-1.9.0/pyro/ops/integrator.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/jit.py` & `pyro-ppl-1.9.0/pyro/ops/jit.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/linalg.py` & `pyro-ppl-1.9.0/pyro/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/newton.py` & `pyro-ppl-1.9.0/pyro/ops/newton.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/packed.py` & `pyro-ppl-1.9.0/pyro/ops/packed.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/provenance.py` & `pyro-ppl-1.9.0/pyro/ops/provenance.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,19 +89,14 @@
     return type(x)(track_provenance(part, provenance) for part in x)
 
 
 @track_provenance.register(list)
 @track_provenance.register(tuple)
 @track_provenance.register(dict)
 def _track_provenance_pytree(x, provenance: frozenset):
-    # avoid max-recursion depth error for torch<=2.0
-    flat_args, _ = tree_flatten(x)
-    if not flat_args or flat_args[0] is x:
-        return x
-
     return tree_map(partial(track_provenance, provenance=provenance), x)
 
 
 @track_provenance.register
 def _track_provenance_provenancetensor(x: ProvenanceTensor, provenance: frozenset):
     x_value, old_provenance = extract_provenance(x)
     return track_provenance(x_value, old_provenance | provenance)
@@ -139,19 +134,14 @@
     return value, provenance
 
 
 @extract_provenance.register(list)
 @extract_provenance.register(tuple)
 @extract_provenance.register(dict)
 def _extract_provenance_pytree(x):
-    # avoid max-recursion depth error for torch<=2.0
-    flat_args, _ = tree_flatten(x)
-    if not flat_args or flat_args[0] is x:
-        return x, frozenset()
-
     flat_args, spec = tree_flatten(x)
     xs = []
     provenance = frozenset()
     for x, p in map(extract_provenance, flat_args):
         xs.append(x)
         provenance |= p
     return tree_unflatten(xs, spec), provenance
```

### Comparing `pyro-ppl-1.8.6/pyro/ops/rings.py` & `pyro-ppl-1.9.0/pyro/ops/rings.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/special.py` & `pyro-ppl-1.9.0/pyro/ops/special.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/ssm_gp.py` & `pyro-ppl-1.9.0/pyro/ops/ssm_gp.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/stats.py` & `pyro-ppl-1.9.0/pyro/ops/stats.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/streaming.py` & `pyro-ppl-1.9.0/pyro/ops/streaming.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/tensor_utils.py` & `pyro-ppl-1.9.0/pyro/ops/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/ops/welford.py` & `pyro-ppl-1.9.0/pyro/ops/welford.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/optim/__init__.py` & `pyro-ppl-1.9.0/pyro/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/optim/adagrad_rmsprop.py` & `pyro-ppl-1.9.0/pyro/optim/adagrad_rmsprop.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/optim/clipped_adam.py` & `pyro-ppl-1.9.0/pyro/optim/clipped_adam.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/optim/dct_adam.py` & `pyro-ppl-1.9.0/pyro/optim/dct_adam.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/optim/horovod.py` & `pyro-ppl-1.9.0/pyro/optim/horovod.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/optim/lr_scheduler.py` & `pyro-ppl-1.9.0/pyro/optim/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/optim/multi.py` & `pyro-ppl-1.9.0/pyro/optim/multi.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/optim/optim.py` & `pyro-ppl-1.9.0/pyro/optim/optim.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/optim/pytorch_optimizers.py` & `pyro-ppl-1.9.0/pyro/optim/pytorch_optimizers.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,19 +30,15 @@
     )
 
     locals()[_name] = _PyroOptim
     __all__.append(_name)
     del _PyroOptim
 
 # Load all schedulers from PyTorch
-# breaking change in torch >= 1.14: LRScheduler is new base class
-if hasattr(torch.optim.lr_scheduler, "LRScheduler"):
-    _torch_scheduler_base = torch.optim.lr_scheduler.LRScheduler  # type: ignore
-else:  # for torch < 1.13, _LRScheduler is base class
-    _torch_scheduler_base = torch.optim.lr_scheduler._LRScheduler  # type: ignore
+_torch_scheduler_base = torch.optim.lr_scheduler.LRScheduler  # type: ignore
 
 for _name, _Optim in torch.optim.lr_scheduler.__dict__.items():
     if not isinstance(_Optim, type):
         continue
     if not issubclass(_Optim, _torch_scheduler_base) and _name != "ReduceLROnPlateau":
         continue
     if _Optim is torch.optim.Optimizer:
```

### Comparing `pyro-ppl-1.8.6/pyro/params/param_store.py` & `pyro-ppl-1.9.0/pyro/params/param_store.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,34 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 import re
 import warnings
 import weakref
 from contextlib import contextmanager
+from typing import (
+    Callable,
+    Dict,
+    ItemsView,
+    Iterator,
+    KeysView,
+    Optional,
+    Tuple,
+    Union,
+)
 
 import torch
 from torch.distributions import constraints, transform_to
+from torch.serialization import MAP_LOCATION
+from typing_extensions import TypedDict
+
+
+class StateDict(TypedDict):
+    params: Dict[str, torch.Tensor]
+    constraints: Dict[str, constraints.Constraint]
 
 
 class ParamStoreDict:
     """
     Global store for parameters in Pyro. This is basically a key-value store.
     The typical user interacts with the ParamStore primarily through the
     primitive `pyro.param`.
@@ -35,88 +52,94 @@
       example, under the hood a parameter that is constrained to be positive is represented as an
       unconstrained tensor in log space.
     """
 
     # -------------------------------------------------------------------------------
     # New dict-like interface
 
-    def __init__(self):
+    def __init__(self) -> None:
         """
         initialize ParamStore data structures
         """
-        self._params = {}  # dictionary from param name to param
-        self._param_to_name = {}  # dictionary from unconstrained param to param name
-        self._constraints = {}  # dictionary from param name to constraint object
+        self._params: Dict[str, torch.Tensor] = (
+            {}
+        )  # dictionary from param name to param
+        self._param_to_name: Dict[torch.Tensor, str] = (
+            {}
+        )  # dictionary from unconstrained param to param name
+        self._constraints: Dict[str, constraints.Constraint] = (
+            {}
+        )  # dictionary from param name to constraint object
 
-    def clear(self):
+    def clear(self) -> None:
         """
         Clear the ParamStore
         """
         self._params = {}
         self._param_to_name = {}
         self._constraints = {}
 
-    def items(self):
+    def items(self) -> Iterator[Tuple[str, torch.Tensor]]:
         """
         Iterate over ``(name, constrained_param)`` pairs. Note that `constrained_param` is
         in the constrained (i.e. user-facing) space.
         """
         for name in self._params:
             yield name, self[name]
 
-    def keys(self):
+    def keys(self) -> KeysView[str]:
         """
         Iterate over param names.
         """
         return self._params.keys()
 
-    def values(self):
+    def values(self) -> Iterator[torch.Tensor]:
         """
         Iterate over constrained parameter values.
         """
         for name, constrained_param in self.items():
             yield constrained_param
 
-    def __bool__(self):
+    def __bool__(self) -> bool:
         return bool(self._params)
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self._params)
 
-    def __contains__(self, name):
+    def __contains__(self, name: str) -> bool:
         return name in self._params
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[str]:
         """
         Iterate over param names.
         """
         return iter(self.keys())
 
-    def __delitem__(self, name):
+    def __delitem__(self, name) -> None:
         """
         Remove a parameter from the param store.
         """
         unconstrained_value = self._params.pop(name)
         self._param_to_name.pop(unconstrained_value)
         self._constraints.pop(name)
 
-    def __getitem__(self, name):
+    def __getitem__(self, name: str) -> torch.Tensor:
         """
         Get the *constrained* value of a named parameter.
         """
         unconstrained_value = self._params[name]
 
         # compute the constrained value
         constraint = self._constraints[name]
-        constrained_value = transform_to(constraint)(unconstrained_value)
-        constrained_value.unconstrained = weakref.ref(unconstrained_value)
+        constrained_value: torch.Tensor = transform_to(constraint)(unconstrained_value)
+        constrained_value.unconstrained = weakref.ref(unconstrained_value)  # type: ignore[attr-defined]
 
         return constrained_value
 
-    def __setitem__(self, name, new_constrained_value):
+    def __setitem__(self, name: str, new_constrained_value: torch.Tensor) -> None:
         """
         Set the constrained value of an existing parameter, or the value of a
         new *unconstrained* parameter. To declare a new parameter with
         constraint, use :meth:`setdefault`.
         """
         # store constraint, defaulting to unconstrained
         constraint = self._constraints.setdefault(name, constraints.real)
@@ -128,15 +151,20 @@
             unconstrained_value = unconstrained_value.contiguous()
         unconstrained_value.requires_grad_(True)
 
         # store a bidirectional mapping between name and unconstrained tensor
         self._params[name] = unconstrained_value
         self._param_to_name[unconstrained_value] = name
 
-    def setdefault(self, name, init_constrained_value, constraint=constraints.real):
+    def setdefault(
+        self,
+        name: str,
+        init_constrained_value: Union[torch.Tensor, Callable[[], torch.Tensor]],
+        constraint: constraints.Constraint = constraints.real,
+    ) -> torch.Tensor:
         """
         Retrieve a *constrained* parameter value from the if it exists, otherwise
         set the initial value. Note that this is a little fancier than
         :meth:`dict.setdefault`.
 
         If the parameter already exists, ``init_constrained_tensor`` will be ignored. To avoid
         expensive creation of ``init_constrained_tensor`` you can wrap it in a ``lambda`` that
@@ -166,40 +194,46 @@
 
         # get the param, which is guaranteed to exist
         return self[name]
 
     # -------------------------------------------------------------------------------
     # Old non-dict interface
 
-    def named_parameters(self):
+    def named_parameters(self) -> ItemsView[str, torch.Tensor]:
         """
         Returns an iterator over ``(name, unconstrained_value)`` tuples for
         each parameter in the ParamStore. Note that, in the event the parameter is constrained,
         `unconstrained_value` is in the unconstrained space implicitly used by the constraint.
         """
         return self._params.items()
 
-    def get_all_param_names(self):
+    def get_all_param_names(self) -> KeysView[str]:
         warnings.warn(
             "ParamStore.get_all_param_names() is deprecated; use .keys() instead.",
             DeprecationWarning,
         )
         return self.keys()
 
-    def replace_param(self, param_name, new_param, old_param):
+    def replace_param(
+        self, param_name: str, new_param: torch.Tensor, old_param: torch.Tensor
+    ) -> None:
         warnings.warn(
             "ParamStore.replace_param() is deprecated; use .__setitem__() instead.",
             DeprecationWarning,
         )
-        assert self._params[param_name] is old_param.unconstrained()
+        assert self._params[param_name] is old_param.unconstrained()  # type: ignore[attr-defined]
         self[param_name] = new_param
 
     def get_param(
-        self, name, init_tensor=None, constraint=constraints.real, event_dim=None
-    ):
+        self,
+        name: str,
+        init_tensor: Optional[torch.Tensor] = None,
+        constraint: constraints.Constraint = constraints.real,
+        event_dim: Optional[int] = None,
+    ) -> torch.Tensor:
         """
         Get parameter from its name. If it does not yet exist in the
         ParamStore, it will be created and stored.
         The Pyro primitive `pyro.param` dispatches to this method.
 
         :param name: parameter name
         :type name: str
@@ -212,49 +246,49 @@
         :rtype: torch.Tensor
         """
         if init_tensor is None:
             return self[name]
         else:
             return self.setdefault(name, init_tensor, constraint)
 
-    def match(self, name):
+    def match(self, name: str) -> Dict[str, torch.Tensor]:
         """
         Get all parameters that match regex. The parameter must exist.
 
         :param name: regular expression
         :type name: str
         :returns: dict with key param name and value torch Tensor
         """
         pattern = re.compile(name)
         return {name: self[name] for name in self if pattern.match(name)}
 
-    def param_name(self, p):
+    def param_name(self, p: torch.Tensor) -> Optional[str]:
         """
         Get parameter name from parameter
 
         :param p: parameter
         :returns: parameter name
         """
         return self._param_to_name.get(p)
 
     # -------------------------------------------------------------------------------
     # Persistence interface
 
-    def get_state(self) -> dict:
+    def get_state(self) -> StateDict:
         """
         Get the ParamStore state.
         """
         params = self._params.copy()
         # Remove weakrefs in preparation for pickling.
         for param in params.values():
             param.__dict__.pop("unconstrained", None)
-        state = {"params": params, "constraints": self._constraints.copy()}
+        state: StateDict = {"params": params, "constraints": self._constraints.copy()}
         return state
 
-    def set_state(self, state: dict):
+    def set_state(self, state: StateDict) -> None:
         """
         Set the ParamStore state using state from a previous :meth:`get_state` call
         """
         assert isinstance(state, dict), "malformed ParamStore state"
         assert set(state.keys()) == set(
             ["params", "constraints"]
         ), "malformed ParamStore keys {}".format(state.keys())
@@ -265,25 +299,25 @@
 
         for param_name, constraint in state["constraints"].items():
             if isinstance(constraint, type(constraints.real)):
                 # Work around lack of hash & equality comparison on constraints.
                 constraint = constraints.real
             self._constraints[param_name] = constraint
 
-    def save(self, filename):
+    def save(self, filename: str) -> None:
         """
         Save parameters to file
 
         :param filename: file name to save to
         :type filename: str
         """
         with open(filename, "wb") as output_file:
             torch.save(self.get_state(), output_file)
 
-    def load(self, filename, map_location=None):
+    def load(self, filename: str, map_location: MAP_LOCATION = None) -> None:
         """
         Loads parameters from file
 
         .. note::
 
            If using :meth:`pyro.module` on parameters loaded from
            disk, be sure to set the ``update_module_params`` flag::
@@ -297,15 +331,15 @@
         :type map_location: function, torch.device, string or a dict
         """
         with open(filename, "rb") as input_file:
             state = torch.load(input_file, map_location)
         self.set_state(state)
 
     @contextmanager
-    def scope(self, state=None) -> dict:
+    def scope(self, state: Optional[StateDict] = None) -> Iterator[StateDict]:
         """
         Context manager for using multiple parameter stores within the same process.
 
         This is a thin wrapper around :meth:`get_state`, :meth:`clear`, and
         :meth:`set_state`. For large models where memory space is limiting, you
         may want to instead manually use :meth:`save`, :meth:`clear`, and
         :meth:`load`.
@@ -339,23 +373,23 @@
             self.set_state(old_state)
 
 
 # used to create fully-formed param names, e.g. mymodule$$$mysubmodule.weight
 _MODULE_NAMESPACE_DIVIDER = "$$$"
 
 
-def param_with_module_name(pyro_name, param_name):
+def param_with_module_name(pyro_name: str, param_name: str) -> str:
     return _MODULE_NAMESPACE_DIVIDER.join([pyro_name, param_name])
 
 
-def module_from_param_with_module_name(param_name):
+def module_from_param_with_module_name(param_name: str) -> str:
     return param_name.split(_MODULE_NAMESPACE_DIVIDER)[0]
 
 
-def user_param_name(param_name):
+def user_param_name(param_name: str) -> str:
     if _MODULE_NAMESPACE_DIVIDER in param_name:
         return param_name.split(_MODULE_NAMESPACE_DIVIDER)[1]
     return param_name
 
 
-def normalize_param_name(name):
+def normalize_param_name(name: str) -> str:
     return name.replace(_MODULE_NAMESPACE_DIVIDER, ".")
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/__init__.py` & `pyro-ppl-1.9.0/pyro/poutine/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/poutine/block_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/block_messenger.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 from functools import partial
+from typing import TYPE_CHECKING, Callable, List, Optional
 
 from pyro.poutine.messenger import Messenger
 
+if TYPE_CHECKING:
+    from pyro.poutine.runtime import Message
 
-def _block_fn(expose, expose_types, hide, hide_types, hide_all, msg):
+
+def _block_fn(
+    expose: List[str],
+    expose_types: List[str],
+    hide: List[str],
+    hide_types: List[str],
+    hide_all: bool,
+    msg: "Message",
+) -> bool:
     # handle observes
     if msg["type"] == "sample" and msg["is_observed"]:
         msg_type = "observe"
     else:
         msg_type = msg["type"]
 
     is_not_exposed = (msg["name"] not in expose) and (msg_type not in expose_types)
@@ -23,15 +34,22 @@
     ):  # noqa: E129
         return True
     # otherwise expose
     else:
         return False
 
 
-def _make_default_hide_fn(hide_all, expose_all, hide, expose, hide_types, expose_types):
+def _make_default_hide_fn(
+    hide_all: bool,
+    expose_all: bool,
+    hide: Optional[List[str]],
+    expose: Optional[List[str]],
+    hide_types: Optional[List[str]],
+    expose_types: Optional[List[str]],
+) -> Callable[["Message"], bool]:
     # first, some sanity checks:
     # hide_all and expose_all intersect?
     assert (hide_all is False and expose_all is False) or (
         hide_all != expose_all
     ), "cannot hide and expose a site"
 
     # hide and expose intersect?
@@ -61,14 +79,24 @@
     assert set(hide_types).isdisjoint(
         set(expose_types)
     ), "cannot hide and expose a site type"
 
     return partial(_block_fn, expose, expose_types, hide, hide_types, hide_all)
 
 
+def _negate_fn(
+    fn: Callable[["Message"], Optional[bool]]
+) -> Callable[["Message"], bool]:
+    # typed version of lambda msg: not fn(msg)
+    def negated_fn(msg: "Message") -> bool:
+        return not fn(msg)
+
+    return negated_fn
+
+
 class BlockMessenger(Messenger):
     """
     This handler selectively hides Pyro primitive sites from the outside world.
     Default behavior: block everything.
 
     A site is hidden if at least one of the following holds:
 
@@ -106,37 +134,36 @@
         or False/None to hide it.  If specified, all other parameters are ignored.
         Only specify one of hide_fn or expose_fn, not both.
     :param bool hide_all: hide all sites
     :param bool expose_all: expose all sites normally
     :param list hide: list of site names to hide
     :param list expose: list of site names to be exposed while all others hidden
     :param list hide_types: list of site types to be hidden
-    :param lits expose_types: list of site types to be exposed while all others hidden
+    :param list expose_types: list of site types to be exposed while all others hidden
     :returns: stochastic function decorated with a :class:`~pyro.poutine.block_messenger.BlockMessenger`
     """
 
     def __init__(
         self,
-        hide_fn=None,
-        expose_fn=None,
-        hide_all=True,
-        expose_all=False,
-        hide=None,
-        expose=None,
-        hide_types=None,
-        expose_types=None,
-    ):
+        hide_fn: Optional[Callable[["Message"], Optional[bool]]] = None,
+        expose_fn: Optional[Callable[["Message"], Optional[bool]]] = None,
+        hide_all: bool = True,
+        expose_all: bool = False,
+        hide: Optional[List[str]] = None,
+        expose: Optional[List[str]] = None,
+        hide_types: Optional[List[str]] = None,
+        expose_types: Optional[List[str]] = None,
+    ) -> None:
         super().__init__()
         if not (hide_fn is None or expose_fn is None):
             raise ValueError("Only specify one of hide_fn or expose_fn")
         if hide_fn is not None:
             self.hide_fn = hide_fn
         elif expose_fn is not None:
-            self.hide_fn = lambda msg: not expose_fn(msg)
+            self.hide_fn = _negate_fn(expose_fn)
         else:
             self.hide_fn = _make_default_hide_fn(
                 hide_all, expose_all, hide, expose, hide_types, expose_types
             )
 
-    def _process_message(self, msg):
+    def _process_message(self, msg: "Message") -> None:
         msg["stop"] = bool(self.hide_fn(msg))
-        return None
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/broadcast_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/broadcast_messenger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
+from typing import TYPE_CHECKING, List, Optional
+
+from pyro.distributions.torch_distribution import TorchDistributionMixin
+from pyro.poutine.messenger import Messenger
 from pyro.util import ignore_jit_warnings
 
-from .messenger import Messenger
+if TYPE_CHECKING:
+    from pyro.poutine.runtime import Message
 
 
 class BroadcastMessenger(Messenger):
     """
     Automatically broadcasts the batch shape of the stochastic function
     at a sample site when inside a single or nested plate context.
     The existing `batch_shape` must be broadcastable with the size
@@ -34,51 +39,55 @@
     ...             sample = pyro.sample("sample", dist.Bernoulli(torch.tensor(0.5)))
     ...             assert sample.shape == torch.Size((100, 3))
     ...     return sample
     """
 
     @staticmethod
     @ignore_jit_warnings(["Converting a tensor to a Python boolean"])
-    def _pyro_sample(msg):
+    def _pyro_sample(msg: "Message") -> None:
         """
         :param msg: current message at a trace site.
         """
-        if msg["done"] or msg["type"] != "sample":
+        if (
+            msg["done"]
+            or msg["type"] != "sample"
+            or not isinstance(msg["fn"], TorchDistributionMixin)
+        ):
             return
 
         dist = msg["fn"]
-        actual_batch_shape = getattr(dist, "batch_shape", None)
-        if actual_batch_shape is not None:
-            target_batch_shape = [
-                None if size == 1 else size for size in actual_batch_shape
-            ]
-            for f in msg["cond_indep_stack"]:
-                if f.dim is None or f.size == -1:
-                    continue
-                assert f.dim < 0
-                target_batch_shape = [None] * (
-                    -f.dim - len(target_batch_shape)
-                ) + target_batch_shape
-                if (
-                    target_batch_shape[f.dim] is not None
-                    and target_batch_shape[f.dim] != f.size
-                ):
-                    raise ValueError(
-                        "Shape mismatch inside plate('{}') at site {} dim {}, {} vs {}".format(
-                            f.name,
-                            msg["name"],
-                            f.dim,
-                            f.size,
-                            target_batch_shape[f.dim],
-                        )
-                    )
-                target_batch_shape[f.dim] = f.size
-            # Starting from the right, if expected size is None at an index,
-            # set it to the actual size if it exists, else 1.
-            for i in range(-len(target_batch_shape) + 1, 1):
-                if target_batch_shape[i] is None:
-                    target_batch_shape[i] = (
-                        actual_batch_shape[i] if len(actual_batch_shape) >= -i else 1
+        actual_batch_shape = dist.batch_shape
+        target_batch_shape = [
+            None if size == 1 else size for size in actual_batch_shape
+        ]
+        for f in msg["cond_indep_stack"]:
+            if f.dim is None or f.size == -1:
+                continue
+            assert f.dim < 0
+            prefix_batch_shape: List[Optional[int]] = [None] * (
+                -f.dim - len(target_batch_shape)
+            )
+            target_batch_shape = prefix_batch_shape + target_batch_shape
+            if (
+                target_batch_shape[f.dim] is not None
+                and target_batch_shape[f.dim] != f.size
+            ):
+                raise ValueError(
+                    "Shape mismatch inside plate('{}') at site {} dim {}, {} vs {}".format(
+                        f.name,
+                        msg["name"],
+                        f.dim,
+                        f.size,
+                        target_batch_shape[f.dim],
                     )
-            msg["fn"] = dist.expand(target_batch_shape)
-            if msg["fn"].has_rsample != dist.has_rsample:
-                msg["fn"].has_rsample = dist.has_rsample  # copy custom attribute
+                )
+            target_batch_shape[f.dim] = f.size
+        # Starting from the right, if expected size is None at an index,
+        # set it to the actual size if it exists, else 1.
+        for i in range(-len(target_batch_shape) + 1, 1):
+            if target_batch_shape[i] is None:
+                target_batch_shape[i] = (
+                    actual_batch_shape[i] if len(actual_batch_shape) >= -i else 1
+                )
+        msg["fn"] = dist.expand(target_batch_shape)
+        if msg["fn"].has_rsample != dist.has_rsample:
+            msg["fn"].has_rsample = dist.has_rsample  # copy custom attribute
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/collapse_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/collapse_messenger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,40 @@
 # Copyright Contributors to the Pyro project.
 # SPDX-License-Identifier: Apache-2.0
 
+
 from functools import reduce, singledispatch
+from typing import TYPE_CHECKING, Any, FrozenSet, Tuple
+
+from typing_extensions import Self
 
 import pyro
 from pyro.distributions.distribution import COERCIONS
 from pyro.ops.linalg import ignore_torch_deprecation_warnings
+from pyro.poutine.runtime import _PYRO_STACK
+from pyro.poutine.trace_messenger import TraceMessenger
 from pyro.poutine.util import site_is_subsample
 
-from .runtime import _PYRO_STACK
-from .trace_messenger import TraceMessenger
-
 # TODO Remove import guard once funsor is a required dependency.
 try:
     import funsor
     from funsor.cnf import Contraction
     from funsor.delta import Delta
     from funsor.terms import Funsor, Variable
 except ImportError:
     # Create fake types for singledispatch.
     Contraction = type("Contraction", (), {})
     Delta = type("Delta", (), {})
     Funsor = type("Funsor", (), {})
     Variable = type("Variable", (), {})
 
+if TYPE_CHECKING:
+    from funsor.distribution import Distribution
 
-@singledispatch
-def _get_free_vars(x):
-    return x
-
-
-@_get_free_vars.register(Variable)
-def _(x):
-    return frozenset((x.name,))
-
-
-@_get_free_vars.register(tuple)
-def _(x, subs):
-    return frozenset().union(*map(_get_free_vars, x))
+    from pyro.poutine.runtime import Message
 
 
 @singledispatch
 def _substitute(x, subs):
     return x
 
 
@@ -88,53 +81,55 @@
         ``max_plate_nesting``. If any plates appear within the collapsed
         context, you should manually declare ``max_plate_nesting`` to your
         inference algorithm (e.g. ``Trace_ELBO(max_plate_nesting=1)``).
     """
 
     _coerce = None
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         if CollapseMessenger._coerce is None:
             import funsor
             from funsor.distribution import CoerceDistributionToFunsor
 
             funsor.set_backend("torch")
             CollapseMessenger._coerce = CoerceDistributionToFunsor("torch")
         self._block = False
         super().__init__(*args, **kwargs)
 
-    def _process_message(self, msg):
+    def _process_message(self, msg: "Message") -> None:
         if self._block:
             return
         if site_is_subsample(msg):
             return
         super()._process_message(msg)
 
-    def _pyro_sample(self, msg):
+    def _pyro_sample(self, msg: "Message") -> None:
         # Eagerly convert fn and value to Funsor.
         dim_to_name = {f.dim: f.name for f in msg["cond_indep_stack"]}
         dim_to_name.update(self.preserved_plates)
         msg["fn"] = funsor.to_funsor(msg["fn"], funsor.Real, dim_to_name)
+        if TYPE_CHECKING:
+            assert isinstance(msg["fn"], Distribution)
         domain = msg["fn"].inputs["value"]
         if msg["value"] is None:
             msg["value"] = funsor.Variable(msg["name"], domain)
         else:
             msg["value"] = funsor.to_funsor(msg["value"], domain, dim_to_name)
 
         msg["done"] = True
         msg["stop"] = True
 
-    def _pyro_post_sample(self, msg):
+    def _pyro_post_sample(self, msg: "Message") -> None:
         if self._block:
             return
         if site_is_subsample(msg):
             return
         super()._pyro_post_sample(msg)
 
-    def _pyro_barrier(self, msg):
+    def _pyro_barrier(self, msg: "Message") -> None:
         # Get log_prob and record factor.
         name, log_prob, log_joint, sampled_vars = self._get_log_prob()
         self._block = True
         pyro.factor(name, log_prob.data)
         self._block = False
 
         # Sample
@@ -147,45 +142,45 @@
 
         # Update value.
         assert len(msg["args"]) == 1
         value = msg["args"][0]
         value = _substitute(value, samples)
         msg["value"] = value
 
-    def __enter__(self):
+    def __enter__(self) -> Self:
         self.preserved_plates = {
             h.dim: h.name for h in _PYRO_STACK if isinstance(h, pyro.plate)
         }
         COERCIONS.append(self._coerce)
         return super().__enter__()
 
-    def __exit__(self, *args):
+    def __exit__(self, *args) -> None:
         _coerce = COERCIONS.pop()
         assert _coerce is self._coerce
         super().__exit__(*args)
 
         if any(site["type"] == "sample" for site in self.trace.nodes.values()):
             name, log_prob, _, _ = self._get_log_prob()
             pyro.factor(name, log_prob.data)
 
     @ignore_torch_deprecation_warnings()
-    def _get_log_prob(self):
+    def _get_log_prob(self) -> Tuple[str, Funsor, Funsor, FrozenSet[str]]:
         # Convert delayed statements to pyro.factor()
-        reduced_vars = []
+        reduced_vars_list = []
         log_prob_terms = []
-        plates = frozenset()
+        plates: FrozenSet[str] = frozenset()
         for name, site in self.trace.nodes.items():
             if not site["is_observed"]:
-                reduced_vars.append(name)
+                reduced_vars_list.append(name)
             log_prob_terms.append(site["fn"](value=site["value"]))
             plates |= frozenset(
                 f.name for f in site["cond_indep_stack"] if f.vectorized
             )
-        name = reduced_vars[0]
-        reduced_vars = frozenset(reduced_vars)
+        name = reduced_vars_list[0]
+        reduced_vars = frozenset(reduced_vars_list)
         assert log_prob_terms, "nothing to collapse"
         self.trace.nodes.clear()
         reduced_plates = plates - frozenset(self.preserved_plates.values())
         if reduced_plates:
             log_prob = funsor.sum_product.sum_product(
                 funsor.ops.logaddexp,
                 funsor.ops.add,
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/condition_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/condition_messenger.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
-from .messenger import Messenger
-from .trace_struct import Trace
+from typing import TYPE_CHECKING, Dict, Union
+
+import torch
+
+from pyro.poutine.messenger import Messenger
+from pyro.poutine.trace_struct import Trace
+
+if TYPE_CHECKING:
+    from pyro.poutine.runtime import Message
 
 
 class ConditionMessenger(Messenger):
     """
     Given a stochastic function with some sample statements
     and a dictionary of observations at names,
     change the sample statements at those names into observes
@@ -27,38 +34,38 @@
     to `pyro.sample("z", ...)` in `model`.
 
     :param fn: a stochastic function (callable containing Pyro primitive calls)
     :param data: a dict or a :class:`~pyro.poutine.Trace`
     :returns: stochastic function decorated with a :class:`~pyro.poutine.condition_messenger.ConditionMessenger`
     """
 
-    def __init__(self, data):
+    def __init__(self, data: Union[Dict[str, torch.Tensor], Trace]) -> None:
         """
         :param data: a dict or a Trace
 
         Constructor. Doesn't do much, just stores the stochastic function
         and the data to condition on.
         """
         super().__init__()
         self.data = data
 
-    def _pyro_sample(self, msg):
+    def _pyro_sample(self, msg: "Message") -> None:
         """
         :param msg: current message at a trace site.
         :returns: a sample from the stochastic function at the site.
 
         If msg["name"] appears in self.data,
         convert the sample site into an observe site
         whose observed value is the value from self.data[msg["name"]].
 
         Otherwise, implements default sampling behavior
         with no additional effects.
         """
+        assert isinstance(msg["name"], str)
         name = msg["name"]
 
         if name in self.data:
             if isinstance(self.data, Trace):
                 msg["value"] = self.data.nodes[name]["value"]
             else:
                 msg["value"] = self.data[name]
             msg["is_observed"] = msg["value"] is not None
-        return None
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/do_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/do_messenger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 import numbers
 import warnings
+from typing import Dict, Union
 
 import torch
 
-from .messenger import Messenger
-from .runtime import apply_stack
+from pyro.poutine.messenger import Messenger
+from pyro.poutine.runtime import Message, apply_stack
 
 
 class DoMessenger(Messenger):
     """
     Given a stochastic function with some sample statements
     and a dictionary of values at names,
     set the return values of those sites equal to the values
@@ -44,25 +45,26 @@
         Thomas Richardson, James Robins
 
     :param fn: a stochastic function (callable containing Pyro primitive calls)
     :param data: a ``dict`` mapping sample site names to interventions
     :returns: stochastic function decorated with a :class:`~pyro.poutine.do_messenger.DoMessenger`
     """
 
-    def __init__(self, data):
+    def __init__(self, data: Dict[str, Union[torch.Tensor, numbers.Number]]) -> None:
         super().__init__()
         self.data = data
         self._intervener_id = str(id(self))
 
-    def _pyro_sample(self, msg):
+    def _pyro_sample(self, msg: Message) -> None:
+        assert isinstance(msg["name"], str)
         if (
-            msg.get("_intervener_id", None) != self._intervener_id
+            msg.get("_intervener_id") != self._intervener_id
             and self.data.get(msg["name"]) is not None
         ):
-            if msg.get("_intervener_id", None) is not None:
+            if msg.get("_intervener_id") is not None:
                 warnings.warn(
                     "Attempting to intervene on variable {} multiple times,"
                     "this is almost certainly incorrect behavior".format(msg["name"]),
                     RuntimeWarning,
                 )
 
             msg["_intervener_id"] = self._intervener_id
@@ -72,19 +74,21 @@
             new_msg["cond_indep_stack"] = ()  # avoid entering plates twice
             apply_stack(new_msg)
 
             # apply intervention
             intervention = self.data[msg["name"]]
             msg["name"] = msg["name"] + "__CF"  # mangle old name
 
-            if isinstance(intervention, (numbers.Number, torch.Tensor)):
+            if isinstance(intervention, numbers.Number):
+                msg["value"] = torch.tensor(intervention)
+                msg["is_observed"] = True
+                msg["stop"] = True
+            elif isinstance(intervention, torch.Tensor):
                 msg["value"] = intervention
                 msg["is_observed"] = True
                 msg["stop"] = True
             else:
                 raise NotImplementedError(
                     "Interventions of type {} not implemented (yet)".format(
                         type(intervention)
                     )
                 )
-
-        return None
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/enum_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/enum_messenger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
+from typing import Any, Dict, List, Optional
+
 import torch
+from typing_extensions import Self
 
-from pyro.distributions import Categorical
+from pyro.distributions.torch import Categorical
 from pyro.distributions.torch_distribution import TorchDistributionMixin
 from pyro.ops.indexing import Vindex
+from pyro.poutine.messenger import Messenger
+from pyro.poutine.runtime import _ENUM_ALLOCATOR, Message
 from pyro.util import ignore_jit_warnings
 
-from .messenger import Messenger
-from .runtime import _ENUM_ALLOCATOR
-
 
-def _tmc_mixture_sample(msg):
-    dist, num_samples = msg["fn"], msg["infer"].get("num_samples")
+def _tmc_mixture_sample(msg: Message) -> torch.Tensor:
+    assert isinstance(msg["fn"], TorchDistributionMixin)
+    assert msg["infer"] is not None
+    dist, num_samples = msg["fn"], msg["infer"]["num_samples"]
 
     # find batch dims that aren't plate dims
     batch_shape = [1] * len(dist.batch_shape)
     for f in msg["cond_indep_stack"]:
         if f.vectorized:
+            assert f.dim is not None
             batch_shape[f.dim] = f.size if f.size > 0 else dist.batch_shape[f.dim]
-    batch_shape = tuple(batch_shape)
+    batch_shape_tuple = tuple(batch_shape)
 
     # sample a batch
     sample_shape = (num_samples,)
-    fat_sample = dist(sample_shape=sample_shape)  # TODO thin before sampling
+    fat_sample = dist(
+        sample_shape=torch.Size(sample_shape)
+    )  # TODO thin before sampling
     assert fat_sample.shape == sample_shape + dist.batch_shape + dist.event_shape
     assert any(d > 1 for d in fat_sample.shape)
 
-    target_shape = (num_samples,) + batch_shape + dist.event_shape
+    target_shape = (num_samples,) + batch_shape_tuple + dist.event_shape
 
     # if this site has any possible ancestors, sample ancestor indices uniformly
     thin_sample = fat_sample
     if thin_sample.shape != target_shape:
         index = [Ellipsis] + [slice(None)] * (len(thin_sample.shape) - 1)
         squashed_dims = []
         for squashed_dim, squashed_size in zip(
@@ -53,36 +60,41 @@
         for squashed_dim in squashed_dims:
             thin_sample = thin_sample.unsqueeze(squashed_dim)
 
     assert thin_sample.shape == target_shape
     return thin_sample
 
 
-def _tmc_diagonal_sample(msg):
-    dist, num_samples = msg["fn"], msg["infer"].get("num_samples")
+def _tmc_diagonal_sample(msg: Message) -> torch.Tensor:
+    assert isinstance(msg["fn"], TorchDistributionMixin)
+    assert msg["infer"] is not None
+    dist, num_samples = msg["fn"], msg["infer"]["num_samples"]
 
     # find batch dims that aren't plate dims
     batch_shape = [1] * len(dist.batch_shape)
     for f in msg["cond_indep_stack"]:
         if f.vectorized:
+            assert f.dim is not None
             batch_shape[f.dim] = f.size if f.size > 0 else dist.batch_shape[f.dim]
-    batch_shape = tuple(batch_shape)
+    batch_shape_tuple = tuple(batch_shape)
 
     # sample a batch
     sample_shape = (num_samples,)
-    fat_sample = dist(sample_shape=sample_shape)  # TODO thin before sampling
+    fat_sample = dist(
+        sample_shape=torch.Size(sample_shape)
+    )  # TODO thin before sampling
     assert fat_sample.shape == sample_shape + dist.batch_shape + dist.event_shape
     assert any(d > 1 for d in fat_sample.shape)
 
-    target_shape = (num_samples,) + batch_shape + dist.event_shape
+    target_shape = (num_samples,) + batch_shape_tuple + dist.event_shape
 
     # if this site has any ancestors, choose ancestors from diagonal approximation
     thin_sample = fat_sample
     if thin_sample.shape != target_shape:
-        index = [Ellipsis] + [slice(None)] * (len(thin_sample.shape) - 1)
+        index: List[Any] = [Ellipsis] + [slice(None)] * (len(thin_sample.shape) - 1)
         squashed_dims = []
         for squashed_dim, squashed_size in zip(
             range(1, len(thin_sample.shape)), thin_sample.shape[1:]
         ):
             if squashed_size > 1 and (
                 target_shape[squashed_dim] == 1 or squashed_dim == 0
             ):
@@ -95,31 +107,32 @@
         for squashed_dim in squashed_dims:
             thin_sample = thin_sample.unsqueeze(squashed_dim)
 
     assert thin_sample.shape == target_shape
     return thin_sample
 
 
-def enumerate_site(msg):
-    dist = msg["fn"]
-    num_samples = msg["infer"].get("num_samples", None)
+def enumerate_site(msg: Message) -> torch.Tensor:
+    assert isinstance(msg["fn"], TorchDistributionMixin)
+    assert msg["infer"] is not None
+    dist, num_samples = msg["fn"], msg["infer"].get("num_samples")
     if num_samples is None:
         # Enumerate over the support of the distribution.
         value = dist.enumerate_support(expand=msg["infer"].get("expand", False))
     elif num_samples > 1 and not msg["infer"].get("expand", False):
         tmc_strategy = msg["infer"].get("tmc", "diagonal")
         if tmc_strategy == "mixture":
             value = _tmc_mixture_sample(msg)
         elif tmc_strategy == "diagonal":
             value = _tmc_diagonal_sample(msg)
         else:
             raise ValueError("{} not a valid TMC strategy".format(tmc_strategy))
     elif num_samples > 1 and msg["infer"]["expand"]:
         # Monte Carlo sample the distribution.
-        value = dist(sample_shape=(num_samples,))
+        value = dist(sample_shape=torch.Size([num_samples]))
     assert value.dim() == 1 + len(dist.batch_shape) + len(dist.event_shape)
     return value
 
 
 class EnumMessenger(Messenger):
     """
     Enumerates in parallel over discrete sample sites marked
@@ -127,38 +140,46 @@
 
     :param int first_available_dim: The first tensor dimension (counting
         from the right) that is available for parallel enumeration. This
         dimension and all dimensions left may be used internally by Pyro.
         This should be a negative integer or None.
     """
 
-    def __init__(self, first_available_dim=None):
+    def __init__(self, first_available_dim: Optional[int] = None) -> None:
         assert (
             first_available_dim is None or first_available_dim < 0
         ), first_available_dim
         self.first_available_dim = first_available_dim
         super().__init__()
 
-    def __enter__(self):
+    def __enter__(self) -> Self:
         if self.first_available_dim is not None:
             _ENUM_ALLOCATOR.set_first_available_dim(self.first_available_dim)
-        self._markov_depths = {}  # site name -> depth (nonnegative integer)
-        self._param_dims = {}  # site name -> (enum dim -> unique id)
-        self._value_dims = {}  # site name -> (enum dim -> unique id)
+        self._markov_depths: Dict[str, int] = (
+            {}
+        )  # site name -> depth (nonnegative integer)
+        self._param_dims: Dict[str, Dict[int, int]] = (
+            {}
+        )  # site name -> (enum dim -> unique id)
+        self._value_dims: Dict[str, Dict[int, int]] = (
+            {}
+        )  # site name -> (enum dim -> unique id)
         return super().__enter__()
 
     @ignore_jit_warnings()
-    def _pyro_sample(self, msg):
+    def _pyro_sample(self, msg: Message) -> None:
         """
         :param msg: current message at a trace site.
         :returns: a sample from the stochastic function at the site.
         """
         if msg["done"] or not isinstance(msg["fn"], TorchDistributionMixin):
             return
 
+        assert isinstance(msg["name"], str)
+        assert msg["infer"] is not None
         # Compute upstream dims in scope; these are unsafe to use for this site's target_dim.
         scope = msg["infer"].get("_markov_scope")  # site name -> markov depth
         param_dims = _ENUM_ALLOCATOR.dim_to_id.copy()  # enum dim -> unique id
         if scope is not None:
             for name, depth in scope.items():
                 if (
                     self._markov_depths[name] == depth
@@ -171,24 +192,24 @@
 
         # Compute an enumerated value (at an arbitrary dim).
         value = enumerate_site(msg)
         actual_dim = -1 - len(msg["fn"].batch_shape)  # the leftmost dim of log_prob
 
         # Move actual_dim to a safe target_dim.
         target_dim, id_ = _ENUM_ALLOCATOR.allocate(
-            None if scope is None else param_dims
+            None if scope is None else set(param_dims)
         )
         event_dim = msg["fn"].event_dim
         categorical_support = getattr(value, "_pyro_categorical_support", None)
         if categorical_support is not None:
             # Preserve categorical supports to speed up Categorical.log_prob().
             # See pyro/distributions/torch.py for details.
             assert target_dim < 0
             value = value.reshape(value.shape[:1] + (1,) * (-1 - target_dim))
-            value._pyro_categorical_support = categorical_support
+            value._pyro_categorical_support = categorical_support  # type: ignore[attr-defined]
         elif actual_dim < target_dim:
             assert (
                 value.size(target_dim - event_dim) == 1
             ), "pyro.markov dim conflict at dim {}".format(actual_dim)
             value = value.transpose(target_dim - event_dim, actual_dim - event_dim)
             while value.dim() and value.size(0) == 1:
                 value = value.squeeze(0)
@@ -205,24 +226,27 @@
         value_dims[target_dim] = id_
 
         msg["infer"]["_enumerate_dim"] = target_dim
         msg["infer"]["_dim_to_id"] = value_dims
         msg["value"] = value
         msg["done"] = True
 
-    def _pyro_post_sample(self, msg):
+    def _pyro_post_sample(self, msg: Message) -> None:
         # Save all dims exposed in this sample value.
         # Whereas all of site["_dim_to_id"] are needed to interpret a
         # site's log_prob tensor, only a filtered subset self._value_dims[msg["name"]]
         # are needed to interpret a site's value.
         if not isinstance(msg["fn"], TorchDistributionMixin):
             return
         value = msg["value"]
         if value is None:
             return
+
+        assert isinstance(msg["name"], str)
+        assert msg["infer"] is not None
         shape = value.data.shape[: value.dim() - msg["fn"].event_dim]
         dim_to_id = msg["infer"].setdefault("_dim_to_id", {})
         dim_to_id.update(self._param_dims.get(msg["name"], {}))
         with ignore_jit_warnings():
             self._value_dims[msg["name"]] = {
                 dim: id_
                 for dim, id_ in dim_to_id.items()
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/escape_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/escape_messenger.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
-from .messenger import Messenger
-from .runtime import NonlocalExit
+from typing import Callable
+
+from pyro.poutine.messenger import Messenger
+from pyro.poutine.runtime import Message, NonlocalExit
 
 
 class EscapeMessenger(Messenger):
     """
     Messenger that does a nonlocal exit by raising a util.NonlocalExit exception
     """
 
-    def __init__(self, escape_fn):
+    def __init__(self, escape_fn: Callable[[Message], bool]) -> None:
         """
         :param escape_fn: function that takes a msg as input and returns True
             if the poutine should perform a nonlocal exit at that site.
 
         Constructor.  Stores fn and escape_fn.
         """
         super().__init__()
         self.escape_fn = escape_fn
 
-    def _pyro_sample(self, msg):
+    def _pyro_sample(self, msg: Message) -> None:
         """
         :param msg: current message at a trace site
         :returns: a sample from the stochastic function at the site.
 
         Evaluates self.escape_fn on the site (self.escape_fn(msg)).
 
         If this returns True, raises an exception NonlocalExit(msg).
         Else, implements default _pyro_sample behavior with no additional effects.
         """
         if self.escape_fn(msg):
             msg["done"] = True
             msg["stop"] = True
 
-            def cont(m):
+            def cont(m: Message) -> None:
                 raise NonlocalExit(m)
 
             msg["continuation"] = cont
-        return None
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/guide.py` & `pyro-ppl-1.9.0/pyro/poutine/guide.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 # Copyright Contributors to the Pyro project.
 # SPDX-License-Identifier: Apache-2.0
 
 from abc import ABC, abstractmethod
-from typing import Callable, Dict, Tuple, Union
+from typing import TYPE_CHECKING, Callable, Dict, Optional, Tuple, Union
 
 import torch
 
 import pyro.distributions as dist
-from pyro.distributions.distribution import Distribution
-
-from .trace_messenger import TraceMessenger
-from .trace_struct import Trace
-from .util import prune_subsample_sites, site_is_subsample
+from pyro.poutine.trace_messenger import TraceMessenger
+from pyro.poutine.trace_struct import Trace
+from pyro.poutine.util import prune_subsample_sites, site_is_subsample
+
+if TYPE_CHECKING:
+    from pyro.distributions.torch_distribution import TorchDistributionMixin
+    from pyro.poutine.runtime import Message
 
 
 class GuideMessenger(TraceMessenger, ABC):
     """
     Abstract base class for effect-based guides.
 
     Derived classes must implement the :meth:`get_posterior` method.
     """
 
-    def __init__(self, model: Callable):
+    def __init__(self, model: Callable) -> None:
         super().__init__()
         # Do not register model as submodule
         self._model = (model,)
 
     @property
-    def model(self):
+    def model(self) -> Callable:
         return self._model[0]
 
-    def __getstate__(self):
+    def __getstate__(self) -> Dict[str, object]:
         # Avoid pickling the trace.
-        state = super().__getstate__()
-        state.pop("trace")
+        state = self.__dict__.copy()
+        del state["trace"]
         return state
 
-    def __call__(self, *args, **kwargs) -> Dict[str, torch.Tensor]:
+    def __call__(self, *args, **kwargs) -> Dict[str, torch.Tensor]:  # type: ignore[override]
         """
         Draws posterior samples from the guide and replays the model against
         those samples.
 
         :returns: A dict mapping sample site name to sample value.
             This includes latent, deterministic, and observed values.
         :rtype: dict
@@ -49,44 +51,52 @@
         try:
             with self:
                 self.model(*args, **kwargs)
         finally:
             del self.args_kwargs
 
         model_trace, guide_trace = self.get_traces()
-        samples = {
-            name: site["value"]
-            for name, site in model_trace.nodes.items()
-            if site["type"] == "sample"
-        }
+        samples = {}
+        for name, site in model_trace.nodes.items():
+            if site["type"] == "sample":
+                assert isinstance(site["value"], torch.Tensor)
+                samples[name] = site["value"]
         return samples
 
-    def _pyro_sample(self, msg):
+    def _pyro_sample(self, msg: "Message") -> None:
         if msg["is_observed"] or site_is_subsample(msg):
             return
+        if TYPE_CHECKING:
+            assert isinstance(msg["name"], str)
+            assert isinstance(msg["fn"], TorchDistributionMixin)
+            assert msg["infer"] is not None
         prior = msg["fn"]
         msg["infer"]["prior"] = prior
         posterior = self.get_posterior(msg["name"], prior)
         if isinstance(posterior, torch.Tensor):
             posterior = dist.Delta(posterior, event_dim=prior.event_dim)
         if posterior.batch_shape != prior.batch_shape:
             posterior = posterior.expand(prior.batch_shape)
         msg["fn"] = posterior
 
-    def _pyro_post_sample(self, msg):
+    def _pyro_post_sample(self, msg: "Message") -> None:
         # Manually apply outer plates.
+        assert msg["infer"] is not None
         prior = msg["infer"].get("prior")
-        if prior is not None and prior.batch_shape != msg["fn"].batch_shape:
-            msg["infer"]["prior"] = prior.expand(msg["fn"].batch_shape)
+        if prior is not None:
+            if TYPE_CHECKING:
+                assert isinstance(msg["fn"], TorchDistributionMixin)
+            if prior.batch_shape != msg["fn"].batch_shape:
+                msg["infer"]["prior"] = prior.expand(msg["fn"].batch_shape)
         return super()._pyro_post_sample(msg)
 
     @abstractmethod
     def get_posterior(
-        self, name: str, prior: Distribution
-    ) -> Union[Distribution, torch.Tensor]:
+        self, name: str, prior: "TorchDistributionMixin"
+    ) -> Union["TorchDistributionMixin", torch.Tensor]:
         """
         Abstract method to compute a posterior distribution or sample a
         posterior value given a prior distribution conditioned on upstream
         posterior samples.
 
         Implementations may use ``pyro.param`` and ``pyro.sample`` inside this
         function, but ``pyro.sample`` statements should set
@@ -108,15 +118,15 @@
         :type prior: ~pyro.distributions.Distribution
         :returns: A posterior distribution or sample from the posterior
             distribution.
         :rtype: ~pyro.distributions.Distribution or torch.Tensor
         """
         raise NotImplementedError
 
-    def upstream_value(self, name: str) -> torch.Tensor:
+    def upstream_value(self, name: str) -> Optional[torch.Tensor]:
         """
         For use in :meth:`get_posterior` .
 
         :returns: The value of an upstream sample or deterministic site
         :rtype: torch.Tensor
         """
         return self.trace.nodes[name]["value"]
@@ -138,10 +148,11 @@
         guide_trace = prune_subsample_sites(self.trace)
         model_trace = model_trace = guide_trace.copy()
         for name, guide_site in list(guide_trace.nodes.items()):
             if guide_site["type"] != "sample" or guide_site["is_observed"]:
                 del guide_trace.nodes[name]
                 continue
             model_site = model_trace.nodes[name].copy()
+            assert guide_site["infer"] is not None
             model_site["fn"] = guide_site["infer"]["prior"]
             model_trace.nodes[name] = model_site
         return model_trace, guide_trace
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/indep_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/indep_messenger.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 import numbers
-from collections import namedtuple
+from typing import Iterator, NamedTuple, Optional, Tuple
 
 import torch
+from typing_extensions import Self
 
+from pyro.poutine.messenger import Messenger
+from pyro.poutine.runtime import _DIM_ALLOCATOR, Message
 from pyro.util import ignore_jit_warnings
 
-from .messenger import Messenger
-from .runtime import _DIM_ALLOCATOR
 
+class CondIndepStackFrame(NamedTuple):
+    name: str
+    dim: Optional[int]
+    size: int
+    counter: int
+    full_size: Optional[int] = None
 
-class CondIndepStackFrame(
-    namedtuple("CondIndepStackFrame", ["name", "dim", "size", "counter"])
-):
     @property
-    def vectorized(self):
+    def vectorized(self) -> bool:
         return self.dim is not None
 
-    def _key(self):
+    def _key(self) -> Tuple[str, Optional[int], int, int]:
+        size = self.size
         with ignore_jit_warnings(["Converting a tensor to a Python number"]):
-            size = (
-                self.size.item() if isinstance(self.size, torch.Tensor) else self.size
-            )
-            return self.name, self.dim, size, self.counter
-
-    def __eq__(self, other):
-        return type(self) == type(other) and self._key() == other._key()
+            if isinstance(size, torch.Tensor):  # type: ignore[unreachable]
+                size = size.item()  # type: ignore[unreachable]
+        return self.name, self.dim, size, self.counter
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, CondIndepStackFrame):
+            return False
+        return self._key() == other._key()
 
-    def __ne__(self, other):
+    def __ne__(self, other: object) -> bool:
         return not self.__eq__(other)
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash(self._key())
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name
 
 
 class IndepMessenger(Messenger):
     """
     This messenger keeps track of stack of independence information declared by
     nested ``plate`` contexts. This information is stored in a
@@ -55,73 +61,81 @@
         with y_axis:
             y_noise = sample("y_noise", dist.Normal(loc, scale).expand_by([200, 1]))
         with x_axis, y_axis:
             xy_noise = sample("xy_noise", dist.Normal(loc, scale).expand_by([200, 320]))
 
     """
 
-    def __init__(self, name=None, size=None, dim=None, device=None):
+    def __init__(
+        self,
+        name: str,
+        size: int,
+        dim: Optional[int] = None,
+        device: Optional[str] = None,
+    ) -> None:
         if not torch._C._get_tracing_state() and size == 0:
             raise ZeroDivisionError("size cannot be zero")
 
         super().__init__()
         self._vectorized = None
         if dim is not None:
             self._vectorized = True
 
-        self._indices = None
+        self._indices: Optional[torch.Tensor] = None
         self.name = name
         self.dim = dim
         self.size = size
         self.device = device
         self.counter = 0
 
-    def next_context(self):
+    def next_context(self) -> None:
         """
         Increments the counter.
         """
         self.counter += 1
 
-    def __enter__(self):
+    def __enter__(self) -> Self:
         if self._vectorized is not False:
             self._vectorized = True
 
         if self._vectorized is True:
             self.dim = _DIM_ALLOCATOR.allocate(self.name, self.dim)
 
         return super().__enter__()
 
-    def __exit__(self, *args):
+    def __exit__(self, *args) -> None:
         if self._vectorized is True:
+            assert self.dim is not None
             _DIM_ALLOCATOR.free(self.name, self.dim)
         return super().__exit__(*args)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[int]:
         if self._vectorized is True or self.dim is not None:
             raise ValueError(
                 "cannot use plate {} as both vectorized and non-vectorized"
                 "independence context".format(self.name)
             )
 
         self._vectorized = False
         self.dim = None
         with ignore_jit_warnings([("Iterating over a tensor", RuntimeWarning)]):
             for i in self.indices:
                 self.next_context()
                 with self:
                     yield i if isinstance(i, numbers.Number) else i.item()
 
-    def _reset(self):
+    def _reset(self) -> None:
         if self._vectorized:
+            assert self.dim is not None
             _DIM_ALLOCATOR.free(self.name, self.dim)
         self._vectorized = None
         self.counter = 0
 
     @property
-    def indices(self):
+    def indices(self) -> torch.Tensor:
         if self._indices is None:
             self._indices = torch.arange(self.size, dtype=torch.long).to(self.device)
         return self._indices
 
-    def _process_message(self, msg):
+    def _process_message(self, msg: Message) -> None:
         frame = CondIndepStackFrame(self.name, self.dim, self.size, self.counter)
         msg["cond_indep_stack"] = (frame,) + msg["cond_indep_stack"]
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/infer_config_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/infer_config_messenger.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
-from .messenger import Messenger
+from typing import TYPE_CHECKING, Callable
+
+from pyro.poutine.messenger import Messenger
+
+if TYPE_CHECKING:
+    from pyro.poutine.runtime import InferDict, Message
 
 
 class InferConfigMessenger(Messenger):
     """
     Given a callable `fn` that contains Pyro primitive calls
     and a callable `config_fn` taking a trace site and returning a dictionary,
     updates the value of the infer kwarg at a sample site to config_fn(site).
 
     :param fn: a stochastic function (callable containing Pyro primitive calls)
     :param config_fn: a callable taking a site and returning an infer dict
     :returns: stochastic function decorated with :class:`~pyro.poutine.infer_config_messenger.InferConfigMessenger`
     """
 
-    def __init__(self, config_fn):
+    def __init__(self, config_fn: Callable[["Message"], "InferDict"]) -> None:
         """
         :param config_fn: a callable taking a site and returning an infer dict
 
         Constructor. Doesn't do much, just stores the stochastic function
         and the config_fn.
         """
         super().__init__()
         self.config_fn = config_fn
 
-    def _pyro_sample(self, msg):
+    def _pyro_sample(self, msg: "Message") -> None:
         """
         :param msg: current message at a trace site.
 
         If self.config_fn is not None, calls self.config_fn on msg
         and stores the result in msg["infer"].
 
         Otherwise, implements default sampling behavior
         with no additional effects.
         """
+        assert msg["infer"] is not None
         msg["infer"].update(self.config_fn(msg))
-        return None
 
-    def _pyro_param(self, msg):
+    def _pyro_param(self, msg: "Message") -> None:
         """
         :param msg: current message at a trace site.
 
         If self.config_fn is not None, calls self.config_fn on msg
         and stores the result in msg["infer"].
 
         Otherwise, implements default param behavior
         with no additional effects.
         """
+        assert msg["infer"] is not None
         msg["infer"].update(self.config_fn(msg))
-        return None
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/lift_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/lift_messenger.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 import warnings
+from typing import TYPE_CHECKING, Callable, Dict, Set, Union
+
+from typing_extensions import Self
 
 from pyro import params
 from pyro.distributions.distribution import Distribution
+from pyro.poutine.messenger import Messenger
 from pyro.poutine.util import is_validation_enabled
 
-from .messenger import Messenger
+if TYPE_CHECKING:
+    from pyro.poutine.runtime import Message
 
 
 class LiftMessenger(Messenger):
     """
     Given a stochastic function with param calls and a prior distribution,
     create a stochastic function where all param calls are replaced by sampling from prior.
     Prior should be a callable or a dict of names to callables.
@@ -36,56 +41,60 @@
         False
 
     :param fn: function whose parameters will be lifted to random values
     :param prior: prior function in the form of a Distribution or a dict of stochastic fns
     :returns: ``fn`` decorated with a :class:`~pyro.poutine.lift_messenger.LiftMessenger`
     """
 
-    def __init__(self, prior):
+    def __init__(
+        self,
+        prior: Union[Callable, Distribution, Dict[str, Union[Distribution, Callable]]],
+    ) -> None:
         """
         :param prior: prior used to lift parameters. Prior can be of type
                       dict, pyro.distributions, or a python stochastic fn
 
         Constructor
         """
         super().__init__()
         self.prior = prior
-        self._samples_cache = {}
+        self._samples_cache: Dict[str, "Message"] = {}
 
-    def __enter__(self):
+    def __enter__(self) -> Self:
         self._samples_cache = {}
         if is_validation_enabled() and isinstance(self.prior, dict):
-            self._param_hits = set()
-            self._param_misses = set()
+            self._param_hits: Set[str] = set()
+            self._param_misses: Set[str] = set()
         return super().__enter__()
 
-    def __exit__(self, *args, **kwargs):
+    def __exit__(self, *args, **kwargs) -> None:
         self._samples_cache = {}
         if is_validation_enabled() and isinstance(self.prior, dict):
             extra = set(self.prior) - self._param_hits
             if extra:
                 warnings.warn(
                     "pyro.module prior did not find params ['{}']. "
                     "Did you instead mean one of ['{}']?".format(
                         "', '".join(extra), "', '".join(self._param_misses)
                     )
                 )
         return super().__exit__(*args, **kwargs)
 
-    def _pyro_sample(self, msg):
+    def _pyro_sample(self, msg: "Message") -> None:
         return None
 
-    def _pyro_param(self, msg):
+    def _pyro_param(self, msg: "Message") -> None:
         """
         Overrides the `pyro.param` call with samples sampled from the
         distribution specified in the prior. The prior can be a
         pyro.distributions object or a dict of distributions keyed
         on the param names. If the param name does not match the
         name the keys in the prior, that param name is unchanged.
         """
+        assert msg["name"] is not None
         name = msg["name"]
         param_name = params.user_param_name(name)
         if isinstance(self.prior, dict):
             # prior is a dict of distributions
             if param_name in self.prior.keys():
                 msg["fn"] = self.prior[param_name]
                 msg["args"] = msg["args"][1:]
@@ -107,16 +116,15 @@
             msg["infer"] = {}
         elif callable(self.prior):
             # prior is a stochastic fn. block sample
             msg["stop"] = True
             msg["fn"] = self.prior
             msg["args"] = msg["args"][1:]
         else:
-            # otherwise leave as is
-            return None
+            raise TypeError("unreachable")
         msg["type"] = "sample"
         if name in self._samples_cache:
             # Multiple pyro.param statements with the same
             # name. Block the site and fix the value.
             msg["value"] = self._samples_cache[name]["value"]
             msg["is_observed"] = True
             msg["stop"] = True
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/markov_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/markov_messenger.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 from collections import Counter
-from contextlib import ExitStack  # python 3
+from contextlib import ExitStack
+from typing import TYPE_CHECKING, Iterable, Iterator, List, Optional, Set
 
-from .reentrant_messenger import ReentrantMessenger
+from typing_extensions import Self
+
+from pyro.poutine.reentrant_messenger import ReentrantMessenger
+
+if TYPE_CHECKING:
+    from pyro.poutine.runtime import Message
 
 
 class MarkovMessenger(ReentrantMessenger):
     """
     Markov dependency declaration.
 
     This is a statistical equivalent of a memory management arena.
@@ -23,63 +29,72 @@
     :param int dim: An optional dimension to use for this independence index.
         Interface stub, behavior not yet implemented.
     :param str name: An optional unique name to help inference algorithms match
         :func:`pyro.markov` sites between models and guides.
         Interface stub, behavior not yet implemented.
     """
 
-    def __init__(self, history=1, keep=False, dim=None, name=None):
+    def __init__(
+        self,
+        history: int = 1,
+        keep: bool = False,
+        dim: Optional[int] = None,
+        name: Optional[str] = None,
+    ) -> None:
         assert history >= 0
         self.history = history
         self.keep = keep
         self.dim = dim
         self.name = name
         if dim is not None:
             raise NotImplementedError(
                 "vectorized markov not yet implemented, try setting dim to None"
             )
         if name is not None:
             raise NotImplementedError(
                 "vectorized markov not yet implemented, try setting name to None"
             )
-        self._iterable = None
+        self._iterable: Optional[Iterable[int]] = None
         self._pos = -1
-        self._stack = []
+        self._stack: List[Set[str]] = []
         super().__init__()
 
-    def generator(self, iterable):
+    def generator(self, iterable: Iterable[int]) -> Self:
         self._iterable = iterable
         return self
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[int]:
         with ExitStack() as stack:
+            assert self._iterable is not None
             for value in self._iterable:
                 stack.enter_context(self)
                 yield value
 
-    def __enter__(self):
+    def __enter__(self) -> Self:
         self._pos += 1
         if len(self._stack) <= self._pos:
             self._stack.append(set())
         return super().__enter__()
 
-    def __exit__(self, *args, **kwargs):
+    def __exit__(self, *args, **kwargs) -> None:
         if not self.keep:
             self._stack.pop()
         self._pos -= 1
         return super().__exit__(*args, **kwargs)
 
-    def _pyro_sample(self, msg):
+    def _pyro_sample(self, msg: "Message") -> None:
         if msg["done"] or type(msg["fn"]).__name__ == "_Subsample":
             return
 
         # We use a Counter rather than a set here so that sites can correctly
         # go out of scope when any one of their markov contexts exits.
         # This accounting can be done by users of these fields,
         # e.g. EnumMessenger.
+        assert msg["name"] is not None
+        assert msg["infer"] is not None
         infer = msg["infer"]
         scope = infer.setdefault(
             "_markov_scope", Counter()
         )  # site name -> markov depth
         for pos in range(max(0, self._pos - self.history), self._pos + 1):
             scope.update(self._stack[pos])
         infer["_markov_depth"] = 1 + infer.get("_markov_depth", 0)
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/mask_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/mask_messenger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
+from typing import TYPE_CHECKING, Union
+
 import torch
 
-from .messenger import Messenger
+from pyro.poutine.messenger import Messenger
+
+if TYPE_CHECKING:
+    from pyro.poutine.runtime import Message
 
 
 class MaskMessenger(Messenger):
     """
     Given a stochastic function with some batched sample statements and
     masking tensor, mask out some of the sample statements elementwise.
 
     :param fn: a stochastic function (callable containing Pyro primitive calls)
     :param torch.BoolTensor mask: a ``{0,1}``-valued masking tensor
         (1 includes a site, 0 excludes a site)
     :returns: stochastic function decorated with a :class:`~pyro.poutine.scale_messenger.MaskMessenger`
     """
 
-    def __init__(self, mask):
+    def __init__(self, mask: Union[bool, torch.BoolTensor]) -> None:
         if isinstance(mask, torch.Tensor):
             if mask.dtype != torch.bool:
                 raise ValueError(
                     "Expected mask to be a BoolTensor but got {}".format(type(mask))
                 )
 
         elif mask not in (True, False):
             raise ValueError(
                 "Expected mask to be a boolean but got {}".format(type(mask))
             )
         super().__init__()
         self.mask = mask
 
-    def _process_message(self, msg):
+    def _process_message(self, msg: "Message") -> None:
         msg["mask"] = self.mask if msg["mask"] is None else msg["mask"] & self.mask
-        return None
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/messenger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,37 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 from contextlib import contextmanager
 from functools import partial
-
-from .runtime import _PYRO_STACK
-
-
-def _context_wrap(context, fn, *args, **kwargs):
+from types import TracebackType
+from typing import (
+    Any,
+    Callable,
+    Iterator,
+    List,
+    Optional,
+    Type,
+    TypeVar,
+)
+
+from typing_extensions import ParamSpec, Self
+
+from pyro.poutine.runtime import _PYRO_STACK, Message
+
+_P = ParamSpec("_P")
+_T = TypeVar("_T")
+
+
+def _context_wrap(
+    context: "Messenger",
+    fn: Callable,
+    *args: Any,
+    **kwargs: Any,
+) -> Any:
     with context:
         return fn(*args, **kwargs)
 
 
 class _bound_partial(partial):
     """
     Converts a (possibly) bound method into a partial function to
@@ -22,21 +42,25 @@
     #   `_bound_partial(_bound_partial(f)).func is f`
     # in Python 3.10.
     __slots__ = "func"
 
     def __init__(self, func):
         self.func = func
 
-    def __get__(self, instance, owner):
+    def __get__(
+        self,
+        instance: Optional[object],
+        owner: Optional[Type[object]] = None,
+    ) -> object:
         if instance is None:
             return self
         return partial(self.func, instance)
 
 
-def unwrap(fn):
+def unwrap(fn: Callable) -> Callable:
     """
     Recursively unwraps poutines.
     """
     while True:
         if isinstance(fn, _bound_partial):
             fn = fn.func
             continue
@@ -57,25 +81,23 @@
     so that the joint distribution induced by a stochastic function fn
     is identical to the joint distribution induced by ``Messenger()(fn)``.
 
     Class of transformers for messages passed during inference.
     Most inference operations are implemented in subclasses of this.
     """
 
-    def __call__(self, fn):
+    def __call__(self, fn: Callable[_P, _T]) -> Callable[_P, _T]:
         if not callable(fn):
             raise ValueError(
-                "{} is not callable, did you mean to pass it as a keyword arg?".format(
-                    fn
-                )
+                f"{fn!r} is not callable, did you mean to pass it as a keyword arg?"
             )
         wraps = _bound_partial(partial(_context_wrap, self, fn))
         return wraps
 
-    def __enter__(self):
+    def __enter__(self) -> Self:
         """
         :returns: self
         :rtype: pyro.poutine.Messenger
 
         Installs this messenger at the bottom of the Pyro stack.
 
         Can be overloaded to add any additional per-call setup functionality,
@@ -99,15 +121,20 @@
             # and blocks recursive poutine execution patterns like
             # like calling self.__call__ inside of self.__call__
             # or with Handler(...) as p: with p: <BLOCK>
             # It's hard to imagine use cases for this pattern,
             # but it could in principle be enabled...
             raise ValueError("cannot install a Messenger instance twice")
 
-    def __exit__(self, exc_type, exc_value, traceback):
+    def __exit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_value: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> None:
         """
         :param exc_type: exception type, e.g. ValueError
         :param exc_value: exception instance?
         :param traceback: traceback for exception handling
         :returns: None
         :rtype: None
 
@@ -142,38 +169,41 @@
             # find this poutine's position in the stack,
             # then remove it and everything below it in the stack.
             if self in _PYRO_STACK:
                 loc = _PYRO_STACK.index(self)
                 for i in range(loc, len(_PYRO_STACK)):
                     _PYRO_STACK.pop()
 
-    def _reset(self):
+    def _reset(self) -> None:
         pass
 
-    def _process_message(self, msg):
+    def _process_message(self, msg: Message) -> None:
         """
         :param msg: current message at a trace site
         :returns: None
 
         Process the message by calling appropriate method of itself based
         on message type. The message is updated in place.
         """
-        method = getattr(self, "_pyro_{}".format(msg["type"]), None)
+        method = getattr(self, f"_pyro_{msg['type']}", None)
         if method is not None:
-            return method(msg)
-        return None
+            method(msg)
 
-    def _postprocess_message(self, msg):
-        method = getattr(self, "_pyro_post_{}".format(msg["type"]), None)
+    def _postprocess_message(self, msg: Message) -> None:
+        method = getattr(self, f"_pyro_post_{msg['type']}", None)
         if method is not None:
-            return method(msg)
-        return None
+            method(msg)
 
     @classmethod
-    def register(cls, fn=None, type=None, post=None):
+    def register(
+        cls,
+        fn: Optional[Callable] = None,
+        type: Optional[str] = None,
+        post: Optional[bool] = None,
+    ) -> Callable:
         """
         :param fn: function implementing operation
         :param str type: name of the operation
             (also passed to :func:`~pyro.poutine.runtime.effectful`)
         :param bool post: if `True`, use this operation as postprocess
 
         Dynamically add operations to an effect.
@@ -193,15 +223,19 @@
         if type is None:
             raise ValueError("An operation type name must be provided")
 
         setattr(cls, "_pyro_" + ("post_" if post else "") + type, staticmethod(fn))
         return fn
 
     @classmethod
-    def unregister(cls, fn=None, type=None):
+    def unregister(
+        cls,
+        fn: Optional[Callable] = None,
+        type: Optional[str] = None,
+    ) -> Optional[Callable]:
         """
         :param fn: function implementing operation
         :param str type: name of the operation
             (also passed to :func:`~pyro.poutine.runtime.effectful`)
 
         Dynamically remove operations from an effect.
         Useful for removing wrappers from libraries.
@@ -223,15 +257,17 @@
         except AttributeError:
             pass
 
         return fn
 
 
 @contextmanager
-def block_messengers(predicate):
+def block_messengers(
+    predicate: Callable[[Messenger], bool]
+) -> Iterator[List[Messenger]]:
     """
     EXPERIMENTAL Context manager to temporarily remove matching messengers from
     the _PYRO_STACK. Note this does not call the ``.__exit__()`` and
     ``.__enter__()`` methods.
 
     This is useful to selectively block enclosing handlers.
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/plate_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/plate_messenger.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 from contextlib import contextmanager
+from typing import TYPE_CHECKING, Iterator, Optional
 
-from .broadcast_messenger import BroadcastMessenger
-from .messenger import block_messengers
-from .subsample_messenger import SubsampleMessenger
+from pyro.poutine.broadcast_messenger import BroadcastMessenger
+from pyro.poutine.messenger import Messenger, block_messengers
+from pyro.poutine.subsample_messenger import SubsampleMessenger
+
+if TYPE_CHECKING:
+    import torch
+
+    from pyro.poutine.runtime import Message
 
 
 class PlateMessenger(SubsampleMessenger):
     """
     Swiss army knife of broadcasting amazingness:
     combines shape inference, independence annotation, and subsampling
     """
 
-    def _process_message(self, msg):
+    def _process_message(self, msg: "Message") -> None:
         super()._process_message(msg)
-        return BroadcastMessenger._pyro_sample(msg)
+        BroadcastMessenger._pyro_sample(msg)
 
-    def __enter__(self):
+    def __enter__(self) -> Optional["torch.Tensor"]:  # type: ignore[override]
         super().__enter__()
         if self._vectorized and self._indices is not None:
             return self.indices
         return None
 
 
 @contextmanager
-def block_plate(name=None, dim=None, *, strict=True):
+def block_plate(
+    name: Optional[str] = None, dim: Optional[int] = None, *, strict: bool = True
+) -> Iterator[None]:
     """
     EXPERIMENTAL Context manager to temporarily block a single enclosing plate.
 
     This is useful for sampling auxiliary variables or lazily sampling global
     variables that are needed in a plated context. For example the following
     models are equivalent:
 
@@ -59,21 +67,22 @@
         raise ValueError("Exactly one of name,dim must be specified")
     if name is not None:
         assert isinstance(name, str)
     if dim is not None:
         assert isinstance(dim, int)
         assert dim < 0
 
-    def predicate(messenger):
+    def predicate(messenger: Messenger) -> bool:
         if not isinstance(messenger, PlateMessenger):
             return False
         if name is not None:
             return messenger.name == name
         if dim is not None:
             return messenger.dim == dim
+        raise ValueError("Unreachable")
 
     with block_messengers(predicate) as matches:
         if strict and len(matches) != 1:
             raise ValueError(
                 f"block_plate matched {len(matches)} messengers. "
                 "Try either removing the block_plate or "
                 "setting strict=False."
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/reparam_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/reparam_messenger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,39 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 import warnings
-from typing import Callable, Dict, Union
+from typing import (
+    TYPE_CHECKING,
+    Callable,
+    Dict,
+    Generic,
+    List,
+    Optional,
+    TypeVar,
+    Union,
+)
 
 import torch
+from typing_extensions import ParamSpec
 
-from .messenger import Messenger
-from .runtime import effectful
+from pyro.poutine.messenger import Messenger
+from pyro.poutine.runtime import effectful
+
+if TYPE_CHECKING:
+    from pyro.distributions.torch_distribution import TorchDistributionMixin
+    from pyro.infer.reparam.reparam import Reparam
+    from pyro.poutine.runtime import Message
+
+_P = ParamSpec("_P")
+_T = TypeVar("_T")
 
 
 @effectful(type="get_init_messengers")
-def _get_init_messengers():
+def _get_init_messengers() -> List[Messenger]:
     return []
 
 
 class ReparamMessenger(Messenger):
     """
     Reparametrizes each affected sample site into one or more auxiliary sample
     sites followed by a deterministic transformation [1].
@@ -30,32 +48,38 @@
 
     [1] Maria I. Gorinova, Dave Moore, Matthew D. Hoffman (2019)
         "Automatic Reparameterisation of Probabilistic Programs"
         https://arxiv.org/pdf/1906.03028.pdf
 
     :param config: Configuration, either a dict mapping site name to
         :class:`~pyro.infer.reparam.reparam.Reparameterizer` , or a function
-        mapping site to :class:`~pyro.infer.reparam.reparam.Reparameterizer` or
+        mapping site to :class:`~pyro.infer.reparam.reparam.Reparam` or
         None. See :mod:`pyro.infer.reparam.strategies` for built-in
         configuration strategies.
     :type config: dict or callable
     """
 
-    def __init__(self, config: Union[Dict[str, object], Callable]):
+    def __init__(
+        self,
+        config: Union[Dict[str, "Reparam"], Callable[["Message"], Optional["Reparam"]]],
+    ) -> None:
         super().__init__()
         assert isinstance(config, dict) or callable(config)
         self.config = config
         self._args_kwargs = None
 
-    def __call__(self, fn):
+    def __call__(self, fn: Callable[_P, _T]) -> Callable[_P, _T]:
         return ReparamHandler(self, fn)
 
-    def _pyro_sample(self, msg):
+    def _pyro_sample(self, msg: "Message") -> None:
         if type(msg["fn"]).__name__ == "_Subsample":
             return
+        assert msg["name"] is not None
+        if TYPE_CHECKING:
+            assert isinstance(msg["fn"], TorchDistributionMixin)
         if isinstance(self.config, dict):
             reparam = self.config.get(msg["name"])
         else:
             reparam = self.config(msg)
         if reparam is None:
             return
 
@@ -75,30 +99,32 @@
         # called a second time, after ReparamMessenger, but that is ok because
         # InitMessenger does not overwrite values.
         #
         # To get this same logic to work for ConditionMessenger or
         # ReplayMessenger we would need to ensure those messengers can
         # similarly be safely applied twice, with the second application
         # avoiding overwriting the original application.
-        for m in _get_init_messengers():
-            m._pyro_sample(msg)
+        _get_init_messengers_iter = _get_init_messengers()
+        assert _get_init_messengers_iter is not None
+        for m in _get_init_messengers_iter:
+            m._process_message(msg)
 
         # Pass args_kwargs to the reparam via a side channel.
-        reparam.args_kwargs = self._args_kwargs
+        reparam.args_kwargs = self._args_kwargs  # type: ignore[attr-defined]
         try:
             new_msg = reparam.apply(
                 {
                     "name": msg["name"],
                     "fn": msg["fn"],
                     "value": msg["value"],
                     "is_observed": msg["is_observed"],
                 }
             )
         finally:
-            reparam.args_kwargs = None
+            reparam.args_kwargs = None  # type: ignore[attr-defined]
 
         if new_msg["value"] is not None:
             # Validate while the original msg["fn"] is known.
             if getattr(msg["fn"], "_validation_enabled", False):
                 msg["fn"]._validate_sample(new_msg["value"])
 
             if msg["value"] is not None and msg["value"] is not new_msg["value"]:
@@ -117,25 +143,25 @@
                     )
 
         msg["fn"] = new_msg["fn"]
         msg["value"] = new_msg["value"]
         msg["is_observed"] = new_msg["is_observed"]
 
 
-class ReparamHandler(object):
+class ReparamHandler(Generic[_P, _T]):
     """
     Reparameterization poutine.
     """
 
-    def __init__(self, msngr, fn):
+    def __init__(self, msngr, fn: Callable[_P, _T]) -> None:
         self.msngr = msngr
         self.fn = fn
         super().__init__()
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args: _P.args, **kwargs: _P.kwargs) -> _T:
         # This saves args,kwargs for optional use by reparameterizers.
         self.msngr._args_kwargs = args, kwargs
         try:
             with self.msngr:
                 return self.fn(*args, **kwargs)
         finally:
             self.msngr._args_kwargs = None
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/replay_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/replay_messenger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
-from .messenger import Messenger
+from typing import TYPE_CHECKING, Dict, Optional
+
+from pyro.poutine.messenger import Messenger
+
+if TYPE_CHECKING:
+    import torch
+
+    from pyro.poutine.runtime import Message
+    from pyro.poutine.trace_struct import Trace
 
 
 class ReplayMessenger(Messenger):
     """
     Given a callable that contains Pyro primitive calls,
     return a callable that runs the original, reusing the values at sites in trace
     at those sites in the new trace
@@ -28,52 +36,55 @@
     :param fn: a stochastic function (callable containing Pyro primitive calls)
     :param trace: a :class:`~pyro.poutine.Trace` data structure to replay against
     :param params: dict of names of param sites and constrained values
         in fn to replay against
     :returns: a stochastic function decorated with a :class:`~pyro.poutine.replay_messenger.ReplayMessenger`
     """
 
-    def __init__(self, trace=None, params=None):
+    def __init__(
+        self,
+        trace: Optional["Trace"] = None,
+        params: Optional[Dict[str, "torch.Tensor"]] = None,
+    ) -> None:
         """
         :param trace: a trace whose values should be reused
 
         Constructor.
         Stores trace in an attribute.
         """
         super().__init__()
         if trace is None and params is None:
             raise ValueError("must provide trace or params to replay against")
         self.trace = trace
         self.params = params
 
-    def _pyro_sample(self, msg):
+    def _pyro_sample(self, msg: "Message") -> None:
         """
         :param msg: current message at a trace site.
 
         At a sample site that appears in self.trace,
         returns the value from self.trace instead of sampling
         from the stochastic function at the site.
 
         At a sample site that does not appear in self.trace,
         reverts to default Messenger._pyro_sample behavior with no additional side effects.
         """
+        assert msg["name"] is not None
         name = msg["name"]
         if self.trace is not None and name in self.trace:
             guide_msg = self.trace.nodes[name]
             if msg["is_observed"]:
                 return None
             if guide_msg["type"] != "sample" or guide_msg["is_observed"]:
                 raise RuntimeError("site {} must be sampled in trace".format(name))
             msg["done"] = True
             msg["value"] = guide_msg["value"]
             msg["infer"] = guide_msg["infer"]
-        return None
 
-    def _pyro_param(self, msg):
+    def _pyro_param(self, msg: "Message") -> None:
         name = msg["name"]
         if self.params is not None and name in self.params:
             assert hasattr(
                 self.params[name], "unconstrained"
             ), "param {} must be constrained value".format(name)
             msg["done"] = True
             msg["value"] = self.params[name]
-        return None
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/scale_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/scale_messenger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
+from typing import TYPE_CHECKING, Union
+
 import torch
 
+from pyro.poutine.messenger import Messenger
 from pyro.poutine.util import is_validation_enabled
 
-from .messenger import Messenger
+if TYPE_CHECKING:
+    from pyro.poutine.runtime import Message
 
 
 class ScaleMessenger(Messenger):
     """
     Given a stochastic function with some sample statements and a positive
     scale factor, scale the score of all sample and observe sites in the
     function.
@@ -29,22 +33,21 @@
         True
 
     :param fn: a stochastic function (callable containing Pyro primitive calls)
     :param scale: a positive scaling factor
     :returns: stochastic function decorated with a :class:`~pyro.poutine.scale_messenger.ScaleMessenger`
     """
 
-    def __init__(self, scale):
+    def __init__(self, scale: Union[float, torch.Tensor]) -> None:
         if isinstance(scale, torch.Tensor):
             if is_validation_enabled() and not (scale > 0).all():
                 raise ValueError(
                     "Expected scale > 0 but got {}. ".format(scale)
                     + "Consider using poutine.mask() instead of poutine.scale()."
                 )
         elif not (scale > 0):
             raise ValueError("Expected scale > 0 but got {}".format(scale))
         super().__init__()
         self.scale = scale
 
-    def _process_message(self, msg):
+    def _process_message(self, msg: "Message") -> None:
         msg["scale"] = self.scale * msg["scale"]
-        return None
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/subsample_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/subsample_messenger.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
+from typing import Optional, Tuple
+
 import torch
 
 from pyro.distributions.distribution import Distribution
+from pyro.poutine.indep_messenger import CondIndepStackFrame, IndepMessenger
+from pyro.poutine.runtime import Message, apply_stack
 from pyro.poutine.util import is_validation_enabled
 from pyro.util import ignore_jit_warnings
 
-from .indep_messenger import CondIndepStackFrame, IndepMessenger
-from .runtime import apply_stack
-
 
 class _Subsample(Distribution):
     """
     Randomly select a subsample of a range of indices.
 
     Internal use only. This should only be used by `plate`.
     """
 
-    def __init__(self, size, subsample_size, use_cuda=None, device=None):
+    def __init__(
+        self,
+        size: int,
+        subsample_size: Optional[int],
+        use_cuda: Optional[bool] = None,
+        device: Optional[str] = None,
+    ) -> None:
         """
         :param int size: the size of the range to subsample from
         :param int subsample_size: the size of the returned subsample
         :param bool use_cuda: DEPRECATED, use the `device` arg instead.
             Whether to use cuda tensors.
         :param str device: device to place the `sample` and `log_prob`
             results on.
@@ -34,18 +41,18 @@
             if self.use_cuda ^ (device != "cpu"):
                 raise ValueError(
                     "Incompatible arg values use_cuda={}, device={}.".format(
                         use_cuda, device
                     )
                 )
         with ignore_jit_warnings(["torch.Tensor results are registered as constants"]):
-            self.device = torch.Tensor().device if not device else device
+            self.device = device or torch.Tensor().device
 
     @ignore_jit_warnings(["Converting a tensor to a Python boolean"])
-    def sample(self, sample_shape=torch.Size()):
+    def sample(self, sample_shape: torch.Size = torch.Size()) -> torch.Tensor:
         """
         :returns: a random subsample of `range(size)`
         :rtype: torch.LongTensor
         """
         if sample_shape:
             raise NotImplementedError
         subsample_size = self.subsample_size
@@ -53,85 +60,87 @@
             result = torch.arange(self.size, device=self.device)
         else:
             result = torch.randperm(self.size, device=self.device)[
                 :subsample_size
             ].clone()
         return result.cuda() if self.use_cuda else result
 
-    def log_prob(self, x):
+    def log_prob(self, x: torch.Tensor) -> torch.Tensor:
         # This is zero so that plate can provide an unbiased estimate of
         # the non-subsampled log_prob.
         result = torch.tensor(0.0, device=self.device)
         return result.cuda() if self.use_cuda else result
 
 
 class SubsampleMessenger(IndepMessenger):
     """
     Extension of IndepMessenger that includes subsampling.
     """
 
     def __init__(
         self,
-        name,
-        size=None,
-        subsample_size=None,
-        subsample=None,
-        dim=None,
-        use_cuda=None,
-        device=None,
-    ):
-        super().__init__(name, size, dim, device)
-        self.subsample_size = subsample_size
-        self._indices = subsample
-        self.use_cuda = use_cuda
-        self.device = device
-
-        self.size, self.subsample_size, self._indices = self._subsample(
-            self.name,
-            self.size,
-            self.subsample_size,
-            self._indices,
-            self.use_cuda,
-            self.device,
+        name: str,
+        size: Optional[int] = None,
+        subsample_size: Optional[int] = None,
+        subsample: Optional[torch.Tensor] = None,
+        dim: Optional[int] = None,
+        use_cuda: Optional[bool] = None,
+        device: Optional[str] = None,
+    ) -> None:
+        full_size, self.subsample_size, subsample = self._subsample(
+            name,
+            size,
+            subsample_size,
+            subsample,
+            use_cuda,
+            device,
         )
+        super().__init__(name, full_size, dim, device)
+        self._indices = subsample
 
     @staticmethod
     def _subsample(
-        name, size=None, subsample_size=None, subsample=None, use_cuda=None, device=None
-    ):
+        name: str,
+        size: Optional[int] = None,
+        subsample_size: Optional[int] = None,
+        subsample: Optional[torch.Tensor] = None,
+        use_cuda: Optional[bool] = None,
+        device: Optional[str] = None,
+    ) -> Tuple[int, int, Optional[torch.Tensor]]:
         """
         Helper function for plate. See its docstrings for details.
         """
         if size is None:
             assert subsample_size is None
             assert subsample is None
             size = -1  # This is PyTorch convention for "arbitrary size"
             subsample_size = -1
         else:
-            msg = {
-                "type": "sample",
-                "name": name,
-                "fn": _Subsample(size, subsample_size, use_cuda, device),
-                "is_observed": False,
-                "args": (),
-                "kwargs": {},
-                "value": subsample,
-                "infer": {},
-                "scale": 1.0,
-                "mask": None,
-                "cond_indep_stack": (),
-                "done": False,
-                "stop": False,
-                "continuation": None,
-            }
+            msg = Message(
+                type="sample",
+                name=name,
+                fn=_Subsample(size, subsample_size, use_cuda, device),
+                is_observed=False,
+                args=(),
+                kwargs={},
+                value=subsample,
+                infer={},
+                scale=1.0,
+                mask=None,
+                cond_indep_stack=(),
+                done=False,
+                stop=False,
+                continuation=None,
+            )
             apply_stack(msg)
             subsample = msg["value"]
 
         with ignore_jit_warnings():
             if subsample_size is None:
+                assert subsample is not None
                 subsample_size = (
                     subsample.size(0)
                     if isinstance(subsample, torch.Tensor)
                     else len(subsample)
                 )
             elif subsample is not None and subsample_size != len(subsample):
                 raise ValueError(
@@ -139,38 +148,42 @@
                         subsample_size, len(subsample)
                     )
                     + " Did you accidentally use different subsample_size in the model and guide?"
                 )
 
         return size, subsample_size, subsample
 
-    def _reset(self):
+    def _reset(self) -> None:
         self._indices = None
         super()._reset()
 
-    def _process_message(self, msg):
+    def _process_message(self, msg: Message) -> None:
         frame = CondIndepStackFrame(
-            self.name, self.dim, self.subsample_size, self.counter
+            name=self.name,
+            dim=self.dim,
+            size=self.subsample_size,
+            counter=self.counter,
+            full_size=self.size,  # used for param initialization
         )
-        frame.full_size = self.size  # Used for param initialization.
         msg["cond_indep_stack"] = (frame,) + msg["cond_indep_stack"]
-        if isinstance(self.size, torch.Tensor) or isinstance(
-            self.subsample_size, torch.Tensor
+        if isinstance(self.size, torch.Tensor) or isinstance(  # type: ignore[unreachable]
+            self.subsample_size, torch.Tensor  # type: ignore[unreachable]
         ):
-            if not isinstance(msg["scale"], torch.Tensor):
+            if not isinstance(msg["scale"], torch.Tensor):  # type: ignore[unreachable]
                 with ignore_jit_warnings():
                     msg["scale"] = torch.tensor(msg["scale"])
         msg["scale"] = msg["scale"] * self.size / self.subsample_size
 
-    def _postprocess_message(self, msg):
+    def _postprocess_message(self, msg: Message) -> None:
         if msg["type"] in ("param", "subsample") and self.dim is not None:
             event_dim = msg["kwargs"].get("event_dim")
             if event_dim is not None:
                 assert event_dim >= 0
                 dim = self.dim - event_dim
+                assert msg["value"] is not None
                 shape = msg["value"].shape
                 if len(shape) >= -dim and shape[dim] != 1:
                     if is_validation_enabled() and shape[dim] != self.size:
                         if msg["type"] == "param":
                             statement = "pyro.param({}, ..., event_dim={})".format(
                                 msg["name"], event_dim
                             )
@@ -182,22 +195,23 @@
                             "Inside pyro.plate({}, {}, dim={}) invalid shape of {}: {}".format(
                                 self.name, self.size, self.dim, statement, shape
                             )
                         )
                     # Subsample parameters with known batch semantics.
                     if self.subsample_size < self.size:
                         value = msg["value"]
+                        assert self._indices is not None
                         new_value = value.index_select(
                             dim, self._indices.to(value.device)
                         )
                         if msg["type"] == "param":
                             if hasattr(value, "_pyro_unconstrained_param"):
-                                param = value._pyro_unconstrained_param
+                                param = value._pyro_unconstrained_param  # type: ignore[attr-defined]
                             else:
-                                param = value.unconstrained()
+                                param = value.unconstrained()  # type: ignore[attr-defined]
 
                             if not hasattr(param, "_pyro_subsample"):
                                 param._pyro_subsample = {}
 
                             param._pyro_subsample[dim] = self._indices
-                            new_value._pyro_unconstrained_param = param
+                            new_value._pyro_unconstrained_param = param  # type: ignore[attr-defined]
                         msg["value"] = new_value
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/substitute_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/substitute_messenger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,83 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 import warnings
+from typing import TYPE_CHECKING, Dict, Set
+
+from typing_extensions import Self
 
 from pyro import params
 from pyro.poutine.messenger import Messenger
 from pyro.poutine.util import is_validation_enabled
 
+if TYPE_CHECKING:
+    import torch
+
+    from pyro.poutine.runtime import Message
+
 
 class SubstituteMessenger(Messenger):
     """
     Given a stochastic function with param calls and a set of parameter values,
     create a stochastic function where all param calls are substituted with
     the fixed values.
     data should be a dict of names to values.
     Consider the following Pyro program:
 
         >>> def model(x):
         ...     a = pyro.param("a", torch.tensor(0.5))
         ...     x = pyro.sample("x", dist.Bernoulli(probs=a))
         ...     return x
-        >>> substituted_model = pyro.poutine.substitute(model, data={"s": 0.3})
+        >>> substituted_model = pyro.poutine.substitute(model, data={"a": torch.tensor(0.3)})
 
-    In this example, site `a` will now have value `0.3`.
+    In this example, site `a` will now have value `torch.tensor(0.3)`.
     :param data: dictionary of values keyed by site names.
     :returns: ``fn`` decorated with a :class:`~pyro.poutine.substitute_messenger.SubstituteMessenger`
     """
 
-    def __init__(self, data):
+    def __init__(self, data: Dict[str, "torch.Tensor"]) -> None:
         """
         :param data: values for the parameters.
         Constructor
         """
         super().__init__()
         self.data = data
-        self._data_cache = {}
+        self._data_cache: Dict[str, "Message"] = {}
 
-    def __enter__(self):
+    def __enter__(self) -> Self:
         self._data_cache = {}
         if is_validation_enabled() and isinstance(self.data, dict):
-            self._param_hits = set()
-            self._param_misses = set()
+            self._param_hits: Set[str] = set()
+            self._param_misses: Set[str] = set()
         return super().__enter__()
 
-    def __exit__(self, *args, **kwargs):
+    def __exit__(self, *args, **kwargs) -> None:
         self._data_cache = {}
         if is_validation_enabled() and isinstance(self.data, dict):
             extra = set(self.data) - self._param_hits
             if extra:
                 warnings.warn(
                     "pyro.module data did not find params ['{}']. "
                     "Did you instead mean one of ['{}']?".format(
                         "', '".join(extra), "', '".join(self._param_misses)
                     )
                 )
         return super().__exit__(*args, **kwargs)
 
-    def _pyro_sample(self, msg):
+    def _pyro_sample(self, msg: "Message") -> None:
         return None
 
-    def _pyro_param(self, msg):
+    def _pyro_param(self, msg: "Message") -> None:
         """
         Overrides the `pyro.param` with substituted values.
         If the param name does not match the name the keys in `data`,
         that param value is unchanged.
         """
+        assert msg["name"] is not None
         name = msg["name"]
         param_name = params.user_param_name(name)
 
         if param_name in self.data.keys():
             msg["value"] = self.data[param_name]
             if is_validation_enabled():
                 self._param_hits.add(param_name)
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/trace_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/trace_messenger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 import sys
+from typing import TYPE_CHECKING, Callable, Generic, Literal, Optional, TypeVar
 
-from .messenger import Messenger
-from .trace_struct import Trace
-from .util import site_is_subsample
+from typing_extensions import ParamSpec, Self
 
+from pyro.poutine.messenger import Messenger
+from pyro.poutine.trace_struct import Trace
+from pyro.poutine.util import site_is_subsample
 
-def identify_dense_edges(trace):
+if TYPE_CHECKING:
+    from pyro.poutine.runtime import Message
+
+_P = ParamSpec("_P")
+_T = TypeVar("_T")
+
+
+def identify_dense_edges(trace: Trace) -> None:
     """
     Modifies a trace in-place by adding all edges based on the
     `cond_indep_stack` information stored at each site.
     """
     for name, node in trace.nodes.items():
         if site_is_subsample(node):
             continue
@@ -59,15 +68,19 @@
 
     :param fn: a stochastic function (callable containing Pyro primitive calls)
     :param graph_type: string that specifies the kind of graph to construct
     :param param_only: if true, only records params and not samples
     :returns: stochastic function decorated with a :class:`~pyro.poutine.trace_messenger.TraceMessenger`
     """
 
-    def __init__(self, graph_type=None, param_only=None):
+    def __init__(
+        self,
+        graph_type: Optional[Literal["flat", "dense"]] = None,
+        param_only: Optional[bool] = None,
+    ) -> None:
         """
         :param string graph_type: string that specifies the type of graph
             to construct (currently only "flat" or "dense" supported)
         :param param_only: boolean that specifies whether to record sample sites
         """
         super().__init__()
         if graph_type is None:
@@ -75,90 +88,94 @@
         if param_only is None:
             param_only = False
         assert graph_type in ("flat", "dense")
         self.graph_type = graph_type
         self.param_only = param_only
         self.trace = Trace(graph_type=self.graph_type)
 
-    def __enter__(self):
+    def __enter__(self) -> Self:
         self.trace = Trace(graph_type=self.graph_type)
         return super().__enter__()
 
-    def __exit__(self, *args, **kwargs):
+    def __exit__(self, *args, **kwargs) -> None:
         """
         Adds appropriate edges based on cond_indep_stack information
         upon exiting the context.
         """
         if self.param_only:
             for node in list(self.trace.nodes.values()):
                 if node["type"] != "param":
+                    assert node["name"] is not None
                     self.trace.remove_node(node["name"])
         if self.graph_type == "dense":
             identify_dense_edges(self.trace)
         return super().__exit__(*args, **kwargs)
 
-    def __call__(self, fn):
+    def __call__(self, fn: Callable[_P, _T]) -> Callable[_P, _T]:
         """
         TODO docs
         """
         return TraceHandler(self, fn)
 
-    def get_trace(self):
+    def get_trace(self) -> Trace:
         """
         :returns: data structure
         :rtype: pyro.poutine.Trace
 
         Helper method for a very common use case.
         Returns a shallow copy of ``self.trace``.
         """
         return self.trace.copy()
 
-    def _reset(self):
+    def _reset(self) -> None:
         tr = Trace(graph_type=self.graph_type)
         if "_INPUT" in self.trace.nodes:
             tr.add_node(
                 "_INPUT",
                 name="_INPUT",
                 type="input",
                 args=self.trace.nodes["_INPUT"]["args"],
                 kwargs=self.trace.nodes["_INPUT"]["kwargs"],
             )
         self.trace = tr
         super()._reset()
 
-    def _pyro_post_sample(self, msg):
+    def _pyro_post_sample(self, msg: "Message") -> None:
         if self.param_only:
             return
+        assert msg["name"] is not None
+        assert msg["infer"] is not None
         if msg["infer"].get("_do_not_trace"):
             assert msg["infer"].get("is_auxiliary")
             assert not msg["is_observed"]
             return
         self.trace.add_node(msg["name"], **msg.copy())
 
-    def _pyro_post_param(self, msg):
+    def _pyro_post_param(self, msg: "Message") -> None:
+        assert msg["name"] is not None
         self.trace.add_node(msg["name"], **msg.copy())
 
 
-class TraceHandler:
+class TraceHandler(Generic[_P, _T]):
     """
     Execution trace poutine.
 
     A TraceHandler records the input and output to every Pyro primitive
     and stores them as a site in a Trace().
     This should, in theory, be sufficient information for every inference algorithm
     (along with the implicit computational graph in the Variables?)
 
     We can also use this for visualization.
     """
 
-    def __init__(self, msngr, fn):
+    def __init__(self, msngr: TraceMessenger, fn: Callable[_P, _T]) -> None:
         self.fn = fn
         self.msngr = msngr
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args: _P.args, **kwargs: _P.kwargs) -> _T:
         """
         Runs the stochastic function stored in this poutine,
         with additional side effects.
 
         Resets self.trace to an empty trace,
         installs itself on the global execution stack,
         runs self.fn with the given arguments,
@@ -171,27 +188,28 @@
                 "_INPUT", name="_INPUT", type="args", args=args, kwargs=kwargs
             )
             try:
                 ret = self.fn(*args, **kwargs)
             except (ValueError, RuntimeError) as e:
                 exc_type, exc_value, traceback = sys.exc_info()
                 shapes = self.msngr.trace.format_shapes()
+                assert exc_type is not None
                 exc = exc_type("{}\n{}".format(exc_value, shapes))
                 exc = exc.with_traceback(traceback)
                 raise exc from e
             self.msngr.trace.add_node(
                 "_RETURN", name="_RETURN", type="return", value=ret
             )
         return ret
 
     @property
-    def trace(self):
+    def trace(self) -> Trace:
         return self.msngr.trace
 
-    def get_trace(self, *args, **kwargs):
+    def get_trace(self, *args, **kwargs) -> Trace:
         """
         :returns: data structure
         :rtype: pyro.poutine.Trace
 
         Helper method for a very common use case.
         Calls this poutine and returns its trace instead of the function's return value.
         """
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/trace_struct.py` & `pyro-ppl-1.9.0/pyro/poutine/trace_struct.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,45 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 import sys
 from collections import OrderedDict
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    Literal,
+    Optional,
+    Set,
+    Tuple,
+    Union,
+)
 
 import opt_einsum
 
 from pyro.distributions.score_parts import ScoreParts
 from pyro.distributions.util import scale_and_mask
 from pyro.ops.packed import pack
 from pyro.poutine.util import is_validation_enabled
 from pyro.util import warn_if_inf, warn_if_nan
 
+if TYPE_CHECKING:
+    import torch
+
+    from pyro.distributions.distribution import Distribution
+    from pyro.poutine.runtime import Message
+
+
+def allow_all_sites(name: str, site: "Message") -> bool:
+    return True
+
 
 class Trace:
     """
     Graph data structure denoting the relationships amongst different pyro primitives
     in the execution trace.
 
     An execution trace of a Pyro program is a record of every call
@@ -66,39 +90,39 @@
     ``'cond_indep_stack'`` contains data structures corresponding to ``pyro.plate`` contexts
     appearing in the execution.
     ``'done'``, ``'stop'``, and ``'continuation'`` are only used by Pyro's internals.
 
     :param string graph_type: string specifying the kind of trace graph to construct
     """
 
-    def __init__(self, graph_type="flat"):
+    def __init__(self, graph_type: Literal["flat", "dense"] = "flat") -> None:
         assert graph_type in ("flat", "dense"), "{} not a valid graph type".format(
             graph_type
         )
         self.graph_type = graph_type
-        self.nodes = OrderedDict()
-        self._succ = OrderedDict()
-        self._pred = OrderedDict()
+        self.nodes: OrderedDict[str, "Message"] = OrderedDict()
+        self._succ: OrderedDict[str, Set[str]] = OrderedDict()
+        self._pred: OrderedDict[str, Set[str]] = OrderedDict()
 
-    def __contains__(self, name):
+    def __contains__(self, name: str) -> bool:
         return name in self.nodes
 
-    def __iter__(self):
+    def __iter__(self) -> Iterable[str]:
         return iter(self.nodes.keys())
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.nodes)
 
     @property
-    def edges(self):
+    def edges(self) -> Iterable[Tuple[str, str]]:
         for site, adj_nodes in self._succ.items():
             for adj_node in adj_nodes:
                 yield site, adj_node
 
-    def add_node(self, site_name, **kwargs):
+    def add_node(self, site_name: str, **kwargs: Any) -> None:
         """
         :param string site_name: the name of the site to be added
 
         Adds a site to the trace.
 
         Raises an error when attempting to add a duplicate node
         instead of silently overwriting.
@@ -113,86 +137,91 @@
             elif kwargs["type"] != "param":
                 # Cannot sample after a previous sample statement.
                 raise RuntimeError(
                     "Multiple {} sites named '{}'".format(kwargs["type"], site_name)
                 )
 
         # XXX should copy in case site gets mutated, or dont bother?
-        self.nodes[site_name] = kwargs
+        self.nodes[site_name] = kwargs  # type: ignore[assignment]
         self._pred[site_name] = set()
         self._succ[site_name] = set()
 
-    def add_edge(self, site1, site2):
+    def add_edge(self, site1: str, site2: str) -> None:
         for site in (site1, site2):
             if site not in self.nodes:
                 self.add_node(site)
         self._succ[site1].add(site2)
         self._pred[site2].add(site1)
 
-    def remove_node(self, site_name):
+    def remove_node(self, site_name: str) -> None:
         self.nodes.pop(site_name)
         for p in self._pred[site_name]:
             self._succ[p].remove(site_name)
         for s in self._succ[site_name]:
             self._pred[s].remove(site_name)
         self._pred.pop(site_name)
         self._succ.pop(site_name)
 
-    def predecessors(self, site_name):
+    def predecessors(self, site_name: str) -> Set[str]:
         return self._pred[site_name]
 
-    def successors(self, site_name):
+    def successors(self, site_name: str) -> Set[str]:
         return self._succ[site_name]
 
-    def copy(self):
+    def copy(self) -> "Trace":
         """
         Makes a shallow copy of self with nodes and edges preserved.
         """
         new_tr = Trace(graph_type=self.graph_type)
         new_tr.nodes.update(self.nodes)
         new_tr._succ.update(self._succ)
         new_tr._pred.update(self._pred)
         return new_tr
 
-    def _dfs(self, site, visited):
+    def _dfs(self, site: str, visited: Set[str]) -> Iterable[str]:
         if site in visited:
             return
         for s in self._succ[site]:
             for node in self._dfs(s, visited):
                 yield node
         visited.add(site)
         yield site
 
-    def topological_sort(self, reverse=False):
+    def topological_sort(self, reverse: bool = False) -> List[str]:
         """
         Return a list of nodes (site names) in topologically sorted order.
 
         :param bool reverse: Return the list in reverse order.
         :return: list of topologically sorted nodes (site names).
         """
-        visited = set()
+        visited: Set[str] = set()
         top_sorted = []
         for s in self._succ:
             for node in self._dfs(s, visited):
                 top_sorted.append(node)
         return top_sorted if reverse else list(reversed(top_sorted))
 
-    def log_prob_sum(self, site_filter=lambda name, site: True):
+    def log_prob_sum(
+        self,
+        site_filter: Callable[[str, "Message"], bool] = allow_all_sites,
+    ) -> Union["torch.Tensor", float]:
         """
         Compute the site-wise log probabilities of the trace.
         Each ``log_prob`` has shape equal to the corresponding ``batch_shape``.
         Each ``log_prob_sum`` is a scalar.
         The computation of ``log_prob_sum`` is memoized.
 
         :returns: total log probability.
         :rtype: torch.Tensor
         """
         result = 0.0
         for name, site in self.nodes.items():
             if site["type"] == "sample" and site_filter(name, site):
+                if TYPE_CHECKING:
+                    assert isinstance(site["fn"], Distribution)
                 if "log_prob_sum" in site:
                     log_p = site["log_prob_sum"]
                 else:
                     try:
                         log_p = site["fn"].log_prob(
                             site["value"], *site["args"], **site["kwargs"]
                         )
@@ -209,26 +238,31 @@
                     if is_validation_enabled():
                         warn_if_nan(log_p, "log_prob_sum at site '{}'".format(name))
                         warn_if_inf(
                             log_p,
                             "log_prob_sum at site '{}'".format(name),
                             allow_neginf=True,
                         )
-                result = result + log_p
+                result = result + log_p  # type: ignore[assignment]
         return result
 
-    def compute_log_prob(self, site_filter=lambda name, site: True):
+    def compute_log_prob(
+        self,
+        site_filter: Callable[[str, "Message"], bool] = allow_all_sites,
+    ) -> None:
         """
         Compute the site-wise log probabilities of the trace.
         Each ``log_prob`` has shape equal to the corresponding ``batch_shape``.
         Each ``log_prob_sum`` is a scalar.
         Both computations are memoized.
         """
         for name, site in self.nodes.items():
             if site["type"] == "sample" and site_filter(name, site):
+                if TYPE_CHECKING:
+                    assert isinstance(site["fn"], Distribution)
                 if "log_prob" not in site:
                     try:
                         log_p = site["fn"].log_prob(
                             site["value"], *site["args"], **site["kwargs"]
                         )
                     except ValueError as e:
                         _, exc_value, traceback = sys.exc_info()
@@ -249,23 +283,25 @@
                         )
                         warn_if_inf(
                             site["log_prob_sum"],
                             "log_prob_sum at site '{}'".format(name),
                             allow_neginf=True,
                         )
 
-    def compute_score_parts(self):
+    def compute_score_parts(self) -> None:
         """
         Compute the batched local score parts at each site of the trace.
         Each ``log_prob`` has shape equal to the corresponding ``batch_shape``.
         Each ``log_prob_sum`` is a scalar.
         All computations are memoized.
         """
         for name, site in self.nodes.items():
             if site["type"] == "sample" and "score_parts" not in site:
+                if TYPE_CHECKING:
+                    assert isinstance(site["fn"], Distribution)
                 # Note that ScoreParts overloads the multiplication operator
                 # to correctly scale each of its three parts.
                 try:
                     value = site["fn"].score_parts(
                         site["value"], *site["args"], **site["kwargs"]
                     )
                 except ValueError as e:
@@ -287,125 +323,129 @@
                     )
                     warn_if_inf(
                         site["log_prob_sum"],
                         "log_prob_sum at site '{}'".format(name),
                         allow_neginf=True,
                     )
 
-    def detach_(self):
+    def detach_(self) -> None:
         """
         Detach values (in-place) at each sample site of the trace.
         """
         for _, site in self.nodes.items():
             if site["type"] == "sample":
+                assert site["value"] is not None
                 site["value"] = site["value"].detach()
 
     @property
-    def observation_nodes(self):
+    def observation_nodes(self) -> List[str]:
         """
         :return: a list of names of observe sites
         """
         return [
             name
             for name, node in self.nodes.items()
             if node["type"] == "sample" and node["is_observed"]
         ]
 
     @property
-    def param_nodes(self):
+    def param_nodes(self) -> List[str]:
         """
         :return: a list of names of param sites
         """
         return [name for name, node in self.nodes.items() if node["type"] == "param"]
 
     @property
-    def stochastic_nodes(self):
+    def stochastic_nodes(self) -> List[str]:
         """
         :return: a list of names of sample sites
         """
         return [
             name
             for name, node in self.nodes.items()
             if node["type"] == "sample" and not node["is_observed"]
         ]
 
     @property
-    def reparameterized_nodes(self):
+    def reparameterized_nodes(self) -> List[str]:
         """
         :return: a list of names of sample sites whose stochastic functions
             are reparameterizable primitive distributions
         """
         return [
             name
             for name, node in self.nodes.items()
             if node["type"] == "sample"
             and not node["is_observed"]
             and getattr(node["fn"], "has_rsample", False)
         ]
 
     @property
-    def nonreparam_stochastic_nodes(self):
+    def nonreparam_stochastic_nodes(self) -> List[str]:
         """
         :return: a list of names of sample sites whose stochastic functions
             are not reparameterizable primitive distributions
         """
         return list(set(self.stochastic_nodes) - set(self.reparameterized_nodes))
 
-    def iter_stochastic_nodes(self):
+    def iter_stochastic_nodes(self) -> Iterator[Tuple[str, "Message"]]:
         """
         :return: an iterator over stochastic nodes in the trace.
         """
         for name, node in self.nodes.items():
             if node["type"] == "sample" and not node["is_observed"]:
                 yield name, node
 
-    def symbolize_dims(self, plate_to_symbol=None):
+    def symbolize_dims(self, plate_to_symbol: Optional[Dict[str, str]] = None) -> None:
         """
         Assign unique symbols to all tensor dimensions.
         """
         plate_to_symbol = {} if plate_to_symbol is None else plate_to_symbol
         symbol_to_dim = {}
         for site in self.nodes.values():
             if site["type"] != "sample":
                 continue
 
             # allocate even symbols for plate dims
-            dim_to_symbol = {}
+            dim_to_symbol: Dict[int, str] = {}
             for frame in site["cond_indep_stack"]:
                 if frame.vectorized:
+                    assert frame.dim is not None
                     if frame.name in plate_to_symbol:
                         symbol = plate_to_symbol[frame.name]
                     else:
                         symbol = opt_einsum.get_symbol(2 * len(plate_to_symbol))
                         plate_to_symbol[frame.name] = symbol
                     symbol_to_dim[symbol] = frame.dim
                     dim_to_symbol[frame.dim] = symbol
 
             # allocate odd symbols for enum dims
+            assert site["infer"] is not None
             for dim, id_ in site["infer"].get("_dim_to_id", {}).items():
                 symbol = opt_einsum.get_symbol(1 + 2 * id_)
                 symbol_to_dim[symbol] = dim
                 dim_to_symbol[dim] = symbol
             enum_dim = site["infer"].get("_enumerate_dim")
             if enum_dim is not None:
                 site["infer"]["_enumerate_symbol"] = dim_to_symbol[enum_dim]
             site["infer"]["_dim_to_symbol"] = dim_to_symbol
 
         self.plate_to_symbol = plate_to_symbol
         self.symbol_to_dim = symbol_to_dim
 
-    def pack_tensors(self, plate_to_symbol=None):
+    def pack_tensors(self, plate_to_symbol: Optional[Dict[str, str]] = None) -> None:
         """
         Computes packed representations of tensors in the trace.
         This should be called after :meth:`compute_log_prob` or :meth:`compute_score_parts`.
         """
         self.symbolize_dims(plate_to_symbol)
         for site in self.nodes.values():
             if site["type"] != "sample":
                 continue
+            assert site["infer"] is not None
             dim_to_symbol = site["infer"]["_dim_to_symbol"]
             packed = site.setdefault("packed", {})
             try:
                 packed["mask"] = pack(site["mask"], dim_to_symbol)
                 if "score_parts" in site:
                     log_prob, score_function, entropy_term = site["score_parts"]
                     log_prob = pack(log_prob, dim_to_symbol)
@@ -428,26 +468,30 @@
                 shapes = self.format_shapes(last_site=site["name"])
                 raise ValueError(
                     "Error while packing tensors at site '{}':\n  {}\n{}".format(
                         site["name"], exc_value, shapes
                     )
                 ).with_traceback(traceback) from e
 
-    def format_shapes(self, title="Trace Shapes:", last_site=None):
+    def format_shapes(
+        self, title: str = "Trace Shapes:", last_site: Optional[str] = None
+    ) -> str:
         """
         Returns a string showing a table of the shapes of all sites in the
         trace.
         """
         if not self.nodes:
             return title
-        rows = [[title]]
+        rows: List[List[Optional[str]]] = [[title]]
 
         rows.append(["Param Sites:"])
         for name, site in self.nodes.items():
             if site["type"] == "param":
+                if TYPE_CHECKING:
+                    assert isinstance(site["value"], torch.Tensor)
                 rows.append([name, None] + [str(size) for size in site["value"].shape])
             if name == last_site:
                 break
 
         rows.append(["Sample Sites:"])
         for name, site in self.nodes.items():
             if site["type"] == "sample":
@@ -483,15 +527,15 @@
                     )
             if name == last_site:
                 break
 
         return _format_table(rows)
 
 
-def _format_table(rows):
+def _format_table(rows: List[List[Optional[str]]]) -> str:
     """
     Formats a right justified table using None as column separator.
     """
     # compute column widths
     column_widths = [0, 0, 0]
     for row in rows:
         widths = [0, 0, 0]
@@ -501,34 +545,37 @@
                 j += 1
             else:
                 widths[j] += 1
         for j in range(3):
             column_widths[j] = max(column_widths[j], widths[j])
 
     # justify columns
-    for i, row in enumerate(rows):
-        cols = [[], [], []]
+    justified_rows: List[List[str]] = []
+    for row in rows:
+        cols: List[List[str]] = [[], [], []]
         j = 0
         for cell in row:
             if cell is None:
                 j += 1
             else:
                 cols[j].append(cell)
         cols = [
-            [""] * (width - len(col)) + col
-            if direction == "r"
-            else col + [""] * (width - len(col))
+            (
+                [""] * (width - len(col)) + col
+                if direction == "r"
+                else col + [""] * (width - len(col))
+            )
             for width, col, direction in zip(column_widths, cols, "rrl")
         ]
-        rows[i] = sum(cols, [])
+        justified_rows.append(sum(cols, []))
 
     # compute cell widths
-    cell_widths = [0] * len(rows[0])
-    for row in rows:
-        for j, cell in enumerate(row):
+    cell_widths = [0] * len(justified_rows[0])
+    for justified_row in justified_rows:
+        for j, cell in enumerate(justified_row):
             cell_widths[j] = max(cell_widths[j], len(cell))
 
     # justify cells
     return "\n".join(
-        " ".join(cell.rjust(width) for cell, width in zip(row, cell_widths))
-        for row in rows
+        " ".join(cell.rjust(width) for cell, width in zip(justified_row, cell_widths))
+        for justified_row in justified_rows
     )
```

### Comparing `pyro-ppl-1.8.6/pyro/poutine/uncondition_messenger.py` & `pyro-ppl-1.9.0/pyro/poutine/uncondition_messenger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
-from .messenger import Messenger
+from typing import TYPE_CHECKING
+
+from pyro.poutine.messenger import Messenger
+
+if TYPE_CHECKING:
+    from pyro.poutine.runtime import Message
 
 
 class UnconditionMessenger(Messenger):
     """
     Messenger to force the value of observed nodes to be sampled from their
     distribution, ignoring observations.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
 
-    def _pyro_sample(self, msg):
+    def _pyro_sample(self, msg: "Message") -> None:
         """
         :param msg: current message at a trace site.
 
         Samples value from distribution, irrespective of whether or not the
         node has an observed value.
         """
         if msg["is_observed"]:
             msg["is_observed"] = False
+            assert msg["infer"] is not None
             msg["infer"]["was_observed"] = True
             msg["infer"]["obs"] = msg["value"]
             msg["value"] = None
             msg["done"] = False
-        return None
```

### Comparing `pyro-ppl-1.8.6/pyro/primitives.py` & `pyro-ppl-1.9.0/pyro/primitives.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,57 +2,67 @@
 # SPDX-License-Identifier: Apache-2.0
 
 import copy
 import warnings
 from collections import OrderedDict
 from contextlib import ExitStack, contextmanager
 from inspect import isclass
+from typing import Callable, Iterator, Optional, Sequence, Union
 
 import torch
+from torch.distributions import constraints
 
 import pyro.distributions as dist
 import pyro.infer as infer
 import pyro.poutine as poutine
-from pyro.distributions import constraints
+from pyro.distributions.torch_distribution import TorchDistributionMixin
 from pyro.params import param_with_module_name
+from pyro.params.param_store import ParamStoreDict
 from pyro.poutine.plate_messenger import PlateMessenger
 from pyro.poutine.runtime import (
     _MODULE_NAMESPACE_DIVIDER,
     _PYRO_PARAM_STORE,
+    InferDict,
+    Message,
     am_i_wrapped,
     apply_stack,
     effectful,
 )
 from pyro.poutine.subsample_messenger import SubsampleMessenger
 from pyro.util import deep_getattr, set_rng_seed  # noqa: F401
 
 
-def get_param_store():
+def get_param_store() -> ParamStoreDict:
     """
     Returns the global :class:`~pyro.params.param_store.ParamStoreDict`.
     """
     return _PYRO_PARAM_STORE
 
 
-def clear_param_store():
+def clear_param_store() -> None:
     """
     Clears the global :class:`~pyro.params.param_store.ParamStoreDict`.
 
     This is especially useful if you're working in a REPL. We recommend calling
     this before each training loop (to avoid leaking parameters from past
     models), and before each unit test (to avoid leaking parameters across
     tests).
     """
-    return _PYRO_PARAM_STORE.clear()
+    _PYRO_PARAM_STORE.clear()
 
 
 _param = effectful(_PYRO_PARAM_STORE.get_param, type="param")
 
 
-def param(name, init_tensor=None, constraint=constraints.real, event_dim=None):
+def param(
+    name: str,
+    init_tensor: Union[torch.Tensor, Callable[[], torch.Tensor], None] = None,
+    constraint: constraints.Constraint = constraints.real,
+    event_dim: Optional[int] = None,
+) -> torch.Tensor:
     """
     Saves the variable as a parameter in the param store.
     To interact with the param store or write to disk,
     see `Parameters <parameters.html>`_.
 
     :param str name: name of parameter
     :param init_tensor: initial tensor or lazy callable that returns a tensor.
@@ -71,22 +81,31 @@
     :returns: A constrained parameter. The underlying unconstrained parameter
         is accessible via ``pyro.param(...).unconstrained()``, where
         ``.unconstrained`` is a weakref attribute.
     :rtype: torch.Tensor
     """
     # Note effectful(-) requires the double passing of name below.
     args = (name,) if init_tensor is None else (name, init_tensor)
-    return _param(*args, constraint=constraint, event_dim=event_dim, name=name)
+    value = _param(*args, constraint=constraint, event_dim=event_dim, name=name)
+    assert value is not None  # type narrowing guaranteed by _param
+    return value
 
 
-def _masked_observe(name, fn, obs, obs_mask, *args, **kwargs):
+def _masked_observe(
+    name: str,
+    fn: TorchDistributionMixin,
+    obs: Optional[torch.Tensor],
+    obs_mask: torch.BoolTensor,
+    *args,
+    **kwargs,
+) -> torch.Tensor:
     # Split into two auxiliary sample sites.
     with poutine.mask(mask=obs_mask):
         observed = sample(f"{name}_observed", fn, *args, **kwargs, obs=obs)
-    with poutine.mask(mask=~obs_mask):
+    with poutine.mask(mask=~obs_mask):  # type: ignore[call-overload]
         unobserved = sample(f"{name}_unobserved", fn, *args, **kwargs)
 
     # Interleave observed and unobserved events.
     shape = obs_mask.shape + (1,) * fn.event_dim
     batch_mask = obs_mask.reshape(shape)
     try:
         value = torch.where(batch_mask, observed, unobserved)
@@ -95,18 +114,26 @@
             shape = torch.broadcast_shapes(observed.shape, unobserved.shape)
             batch_shape = shape[: len(shape) - fn.event_dim]
             raise ValueError(
                 f"Invalid obs_mask shape {tuple(obs_mask.shape)}; should be "
                 f"broadcastable to batch_shape = {tuple(batch_shape)}"
             ) from e
         raise
-    return deterministic(name, value)
+    return deterministic(name, value, event_dim=fn.event_dim)
 
 
-def sample(name, fn, *args, **kwargs):
+def sample(
+    name: str,
+    fn: TorchDistributionMixin,
+    *args,
+    obs: Optional[torch.Tensor] = None,
+    obs_mask: Optional[torch.BoolTensor] = None,
+    infer: Optional[InferDict] = None,
+    **kwargs,
+) -> torch.Tensor:
     """
     Calls the stochastic function ``fn`` with additional side-effects depending
     on ``name`` and the enclosing context (e.g. an inference algorithm).  See
     `Introduction to Pyro <http://pyro.ai/examples/intro_long.html>`_ for a discussion.
 
     :param name: name of sample
     :param fn: distribution class or function
@@ -119,56 +146,58 @@
         + "_unobserved"`` which should be used by guides.
     :type obs_mask: bool or ~torch.Tensor
     :param dict infer: Optional dictionary of inference parameters specified
         in kwargs. See inference documentation for details.
     :returns: sample
     """
     # Transform obs_mask into multiple sample statements.
-    obs = kwargs.pop("obs", None)
-    obs_mask = kwargs.pop("obs_mask", None)
     if obs_mask is not None:
         return _masked_observe(name, fn, obs, obs_mask, *args, **kwargs)
 
     # Check if stack is empty.
     # if stack empty, default behavior (defined here)
-    infer = kwargs.pop("infer", {}).copy()
+    infer = {} if infer is None else infer.copy()
     is_observed = infer.pop("is_observed", obs is not None)
+    assert isinstance(is_observed, bool)
     if not am_i_wrapped():
         if obs is not None and not infer.get("_deterministic"):
             warnings.warn(
                 "trying to observe a value outside of inference at " + name,
                 RuntimeWarning,
             )
             return obs
         return fn(*args, **kwargs)
     # if stack not empty, apply everything in the stack?
     else:
         # initialize data structure to pass up/down the stack
-        msg = {
-            "type": "sample",
-            "name": name,
-            "fn": fn,
-            "is_observed": is_observed,
-            "args": args,
-            "kwargs": kwargs,
-            "value": obs,
-            "infer": infer,
-            "scale": 1.0,
-            "mask": None,
-            "cond_indep_stack": (),
-            "done": False,
-            "stop": False,
-            "continuation": None,
-        }
+        msg = Message(
+            type="sample",
+            name=name,
+            fn=fn,
+            is_observed=is_observed,
+            args=args,
+            kwargs=kwargs,
+            value=obs,
+            infer=infer,
+            scale=1.0,
+            mask=None,
+            cond_indep_stack=(),
+            done=False,
+            stop=False,
+            continuation=None,
+        )
         # apply the stack and return its return value
         apply_stack(msg)
+        assert msg["value"] is not None  # type narrowing guaranteed by apply_stack
         return msg["value"]
 
 
-def factor(name, log_factor, *, has_rsample=None):
+def factor(
+    name: str, log_factor: torch.Tensor, *, has_rsample: Optional[bool] = None
+) -> None:
     """
     Factor statement to add arbitrary log probability factor to a
     probabilisitic model.
 
     .. warning:: When using factor statements in guides, you'll need to specify
         whether the factor statement originated from fully reparametrized
         sampling (e.g. the Jacobian determinant of a transformation of a
@@ -184,15 +213,17 @@
         must be specified for use in guides.
     """
     unit_dist = dist.Unit(log_factor, has_rsample=has_rsample)
     unit_value = unit_dist.sample()
     sample(name, unit_dist, obs=unit_value, infer={"is_auxiliary": True})
 
 
-def deterministic(name, value, event_dim=None):
+def deterministic(
+    name: str, value: torch.Tensor, event_dim: Optional[int] = None
+) -> torch.Tensor:
     """
     Deterministic statement to add a :class:`~pyro.distributions.Delta` site
     with name `name` and value `value` to the trace. This is useful when we
     want to record values which are completely determined by their parents.
     For example::
 
         x = pyro.sample("x", dist.Normal(0, 1))
@@ -211,15 +242,15 @@
         dist.Delta(value, event_dim=event_dim).mask(False),
         obs=value,
         infer={"_deterministic": True},
     )
 
 
 @effectful(type="subsample")
-def subsample(data, event_dim):
+def subsample(data: torch.Tensor, event_dim: int) -> torch.Tensor:
     """
     Subsampling statement to subsample data tensors based on enclosing
     :class:`plate` s.
 
     This is typically called on arguments to ``model()`` when subsampling is
     performed automatically by :class:`plate` s by passing either the
     ``subsample`` or ``subsample_size`` kwarg. For example the following are
@@ -370,15 +401,17 @@
         warnings.warn(
             "pyro.irange is deprecated; use pyro.plate instead", DeprecationWarning
         )
         super().__init__(*args, **kwargs)
 
 
 @contextmanager
-def plate_stack(prefix, sizes, rightmost_dim=-1):
+def plate_stack(
+    prefix: str, sizes: Sequence[int], rightmost_dim: int = -1
+) -> Iterator[None]:
     """
     Create a contiguous stack of :class:`plate` s with dimensions::
 
         rightmost_dim - len(sizes), ..., rightmost_dim
 
     :param str prefix: Name prefix for plates.
     :param iterable sizes: An iterable of plate sizes.
@@ -388,15 +421,17 @@
     with ExitStack() as stack:
         for i, size in enumerate(reversed(sizes)):
             plate_i = plate(f"{prefix}_{i}", size, dim=rightmost_dim - i)
             stack.enter_context(plate_i)
         yield
 
 
-def module(name, nn_module, update_module_params=False):
+def module(
+    name: str, nn_module: torch.nn.Module, update_module_params: bool = False
+) -> torch.nn.Module:
     """
     Registers all parameters of a :class:`torch.nn.Module` with Pyro's
     :mod:`~pyro.params.param_store`.  In conjunction with the
     :class:`~pyro.params.param_store.ParamStoreDict`
     :meth:`~pyro.params.param_store.ParamStoreDict.save` and
     :meth:`~pyro.params.param_store.ParamStoreDict.load` functionality, this
     allows the user to save and load modules.
@@ -454,19 +489,19 @@
             if len(name_arr) > 1:
                 mod_name, param_name = name_arr[0], name_arr[1]
             else:
                 is_param = True
                 mod_name = _name
             if _name in target_state_dict.keys():
                 if not is_param:
-                    deep_getattr(nn_module, mod_name)._parameters[
-                        param_name
-                    ] = target_state_dict[_name]
+                    deep_getattr(nn_module, mod_name)._parameters[param_name] = (
+                        target_state_dict[_name]
+                    )
                 else:
-                    nn_module._parameters[mod_name] = target_state_dict[_name]
+                    nn_module._parameters[mod_name] = target_state_dict[_name]  # type: ignore[assignment]
 
     return nn_module
 
 
 def random_module(name, nn_module, prior, *args, **kwargs):
     r"""
     .. warning::
@@ -504,24 +539,24 @@
         # update_module_params must be True or the lifted module will not update local params
         return lifted_fn(name, nn_copy, update_module_params=True, *args, **kwargs)
 
     return _fn
 
 
 @effectful(type="barrier")
-def barrier(data):
+def barrier(data: torch.Tensor) -> torch.Tensor:
     """
     EXPERIMENTAL Ensures all values in ``data`` are ground, rather than lazy
     funsor values. This is useful in combination with
     :func:`pyro.poutine.collapse`.
     """
     return data
 
 
-def enable_validation(is_validate=True):
+def enable_validation(is_validate: bool = True) -> None:
     """
     Enable or disable validation checks in Pyro. Validation checks provide
     useful warnings and errors, e.g. NaN checks, validating distribution
     arguments and support values, detecting incorrect use of ELBO and MCMC.
     Since some of these checks may be expensive, you may want to disable
     validation of mature models to speed up inference.
 
@@ -540,15 +575,15 @@
     """
     dist.enable_validation(is_validate)
     infer.enable_validation(is_validate)
     poutine.enable_validation(is_validate)
 
 
 @contextmanager
-def validation_enabled(is_validate=True):
+def validation_enabled(is_validate: bool = True) -> Iterator[None]:
     """
     Context manager that is useful when temporarily enabling/disabling
     validation checks.
 
     :param bool is_validate: (optional; defaults to True) temporary
         validation check override.
     """
```

### Comparing `pyro-ppl-1.8.6/pyro/settings.py` & `pyro-ppl-1.9.0/pyro/settings.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro/util.py` & `pyro-ppl-1.9.0/pyro/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/pyro_ppl.egg-info/SOURCES.txt` & `pyro-ppl-1.9.0/pyro_ppl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 setup.cfg
 setup.py
 pyro/__init__.py
 pyro/_version.py
 pyro/generic.py
 pyro/logger.py
 pyro/primitives.py
+pyro/py.typed
 pyro/settings.py
 pyro/util.py
 pyro/contrib/__init__.py
 pyro/contrib/autoguide.py
 pyro/contrib/minipyro.py
 pyro/contrib/util.py
+pyro/contrib/zuko.py
 pyro/contrib/autoname/__init__.py
 pyro/contrib/autoname/autoname.py
 pyro/contrib/autoname/named.py
 pyro/contrib/autoname/scoping.py
 pyro/contrib/bnn/__init__.py
 pyro/contrib/bnn/hidden_layer.py
 pyro/contrib/bnn/utils.py
@@ -183,14 +185,15 @@
 pyro/distributions/transforms/normalize.py
 pyro/distributions/transforms/ordered.py
 pyro/distributions/transforms/permute.py
 pyro/distributions/transforms/planar.py
 pyro/distributions/transforms/polynomial.py
 pyro/distributions/transforms/power.py
 pyro/distributions/transforms/radial.py
+pyro/distributions/transforms/simplex_to_ordered.py
 pyro/distributions/transforms/softplus.py
 pyro/distributions/transforms/spline.py
 pyro/distributions/transforms/spline_autoregressive.py
 pyro/distributions/transforms/spline_coupling.py
 pyro/distributions/transforms/sylvester.py
 pyro/distributions/transforms/unit_cholesky.py
 pyro/distributions/transforms/utils.py
@@ -228,14 +231,15 @@
 pyro/infer/mcmc/__init__.py
 pyro/infer/mcmc/adaptation.py
 pyro/infer/mcmc/api.py
 pyro/infer/mcmc/hmc.py
 pyro/infer/mcmc/logger.py
 pyro/infer/mcmc/mcmc_kernel.py
 pyro/infer/mcmc/nuts.py
+pyro/infer/mcmc/rwkernel.py
 pyro/infer/mcmc/util.py
 pyro/infer/reparam/__init__.py
 pyro/infer/reparam/conjugate.py
 pyro/infer/reparam/discrete_cosine.py
 pyro/infer/reparam/haar.py
 pyro/infer/reparam/hmm.py
 pyro/infer/reparam/loc_scale.py
```

### Comparing `pyro-ppl-1.8.6/setup.cfg` & `pyro-ppl-1.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,21 @@
 	benchmark
 
 [yapf]
 based_on_style = google
 column_limit = 120
 
 [mypy]
-python_version = 3.7
+python_version = 3.8
+explicit_package_bases = True
 warn_return_any = True
 warn_unused_configs = True
 warn_incomplete_stub = True
 ignore_missing_imports = True
+warn_unreachable = True
 
 [mypy-pyro._version.*]
 ignore_errors = True
 
 [mypy-pyro.contrib.*]
 ignore_errors = True
 
@@ -67,24 +69,18 @@
 ignore_errors = True
 warn_unused_ignores = True
 
 [mypy-pyro.ops.tensor_utils]
 ignore_errors = True
 warn_unused_ignores = True
 
-[mypy-pyro.optm.*]
-warn_unused_ignores = True
-
-[mypy-pyro.params.*]
+[mypy-pyro.optim.*]
 ignore_errors = True
 warn_unused_ignores = True
 
-[mypy-pyro.poutine.*]
-ignore_errors = True
-
 [mypy-pyro.util.*]
 ignore_errors = True
 warn_unused_ignores = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pyro-ppl-1.8.6/setup.py` & `pyro-ppl-1.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,22 +64,22 @@
 long_description = "\n".join([str(line) for line in long_description.split("\n")[12:]])
 
 # examples/tutorials
 EXTRAS_REQUIRE = [
     "jupyter>=1.0.0",
     "graphviz>=0.8",
     "matplotlib>=1.3",
-    "torchvision>=0.12.0",
+    "torchvision>=0.15.0",
     "visdom>=0.1.4,<0.2.2",  # FIXME visdom.utils is unavailable >=0.2.2
     "pandas",
-    "pillow==8.2.0",  # https://github.com/pytorch/pytorch/issues/61125
+    "pillow>=8.3.1",  # https://github.com/pytorch/pytorch/issues/61125
     "scikit-learn",
     "seaborn>=0.11.0",
     "wget",
-    "lap",  # Requires setuptools<60
+    "scipy>=1.1",
     # 'biopython>=1.54',
     # 'scanpy>=1.4',  # Requires HDF5
     # 'scvi>=0.6',  # Requires loopy and other fragile packages
 ]
 
 setup(
     name="pyro-ppl",
@@ -98,28 +98,27 @@
     install_requires=[
         # if you add any additional libraries, please also
         # add them to `docs/requirements.txt`
         # numpy is necessary for some functionality of PyTorch
         "numpy>=1.7",
         "opt_einsum>=2.3.2",
         "pyro-api>=0.1.1",
-        "torch>=1.11.0",
+        "torch>=2.0",
         "tqdm>=4.36",
     ],
     extras_require={
         "extras": EXTRAS_REQUIRE,
         "test": EXTRAS_REQUIRE
         + [
             "black>=21.4b0",
             "nbval",
             "pytest-cov",
             "pytest-xdist",
             "pytest>=5.0",
             "ruff",
-            "scipy>=1.1",
         ],
         "profile": ["prettytable", "pytest-benchmark", "snakeviz"],
         "dev": EXTRAS_REQUIRE
         + [
             "black>=21.4b0",
             "mypy>=0.812",
             "nbformat",
@@ -127,36 +126,34 @@
             "nbstripout",
             "nbval",
             "ninja",
             "pypandoc",
             "pytest-xdist",
             "pytest>=5.0",
             "ruff",
-            "scipy>=1.1",
             "sphinx",
             "sphinx_rtd_theme",
             "yapf",
         ],
         "horovod": ["horovod[pytorch]>=0.19"],
-        "lightning": ["pytorch_lightning"],
+        "lightning": ["lightning"],
         "funsor": [
-            # This must be a released version when Pyro is released.
-            # "funsor[torch] @ git+git://github.com/pyro-ppl/funsor.git@7bb52d0eae3046d08a20d1b288544e1a21b4f461",
             "funsor[torch]==0.4.4",
         ],
     },
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     keywords="machine learning statistics probabilistic programming bayesian modeling pytorch",
     license="Apache 2.0",
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     # yapf
 )
```

### Comparing `pyro-ppl-1.8.6/tests/test_examples.py` & `pyro-ppl-1.9.0/tests/test_examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,14 +106,15 @@
     "sir_hmc.py -t=2 -w=2 -n=4 -d=2 -m=1 --enum",
     "sir_hmc.py -t=2 -w=2 -n=4 -d=2 -p=10000 --sequential",
     "sir_hmc.py -t=2 -w=2 -n=4 -d=100 -p=10000 -f 2",
     "smcfilter.py --num-timesteps=3 --num-particles=10",
     "sparse_gamma_def.py --num-epochs=2 --eval-particles=2 --eval-frequency=1 --guide custom",
     "sparse_gamma_def.py --num-epochs=2 --eval-particles=2 --eval-frequency=1 --guide auto",
     "sparse_gamma_def.py --num-epochs=2 --eval-particles=2 --eval-frequency=1 --guide easy",
+    "svi_torch.py --num-epochs=2 --size=400",
     "svi_horovod.py --num-epochs=2 --size=400 --no-horovod",
     pytest.param(
         "svi_lightning.py --max_epochs=2 --size=400 --accelerator cpu --devices 1",
         marks=[requires_lightning],
     ),
     "toy_mixture_model_discrete_enumeration.py  --num-steps=1",
     "sparse_regression.py --num-steps=100 --num-data=100 --num-dimensions 11",
@@ -177,14 +178,15 @@
     "hmm.py --num-steps=1 --truncate=10 --model=4 --tmc --tmc-num-samples=2 --cuda",
     "hmm.py --num-steps=1 --truncate=10 --model=5 --tmc --tmc-num-samples=2 --cuda",
     "hmm.py --num-steps=1 --truncate=10 --model=6 --tmc --tmc-num-samples=2 --cuda",
     "scanvi/scanvi.py --num-epochs 1 --dataset mock --cuda",
     "sir_hmc.py -t=2 -w=2 -n=4 -d=2 -m=1 --enum --cuda",
     "sir_hmc.py -t=2 -w=2 -n=4 -d=2 -p=10000 --sequential --cuda",
     "sir_hmc.py -t=2 -w=2 -n=4 -d=100 -p=10000 --cuda",
+    "svi_torch.py --num-epochs=2 --size=400 --cuda",
     "svi_horovod.py --num-epochs=2 --size=400 --cuda --no-horovod",
     pytest.param(
         "svi_lightning.py --max_epochs=2 --size=400 --accelerator gpu --devices 1",
         marks=[requires_lightning],
     ),
     "vae/vae.py --num-epochs=1 --cuda",
     "vae/ss_vae_M2.py --num-epochs=1 --cuda",
```

### Comparing `pyro-ppl-1.8.6/tests/test_generic.py` & `pyro-ppl-1.9.0/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/tests/test_settings.py` & `pyro-ppl-1.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.6/tests/test_util.py` & `pyro-ppl-1.9.0/tests/test_util.py`

 * *Files identical despite different names*

