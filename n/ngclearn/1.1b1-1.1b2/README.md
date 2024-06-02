# Comparing `tmp/ngclearn-1.1b1.tar.gz` & `tmp/ngclearn-1.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngclearn-1.1b1.tar", last modified: Fri May 31 19:10:37 2024, max compression
+gzip compressed data, was "ngclearn-1.1b2.tar", last modified: Sun Jun  2 21:57:16 2024, max compression
```

## Comparing `ngclearn-1.1b1.tar` & `ngclearn-1.1b2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.012163 ngclearn-1.1b1/
--rw-rw-r--   0 ago       (1001) ago       (1001)      402 2024-05-31 17:48:58.000000 ngclearn-1.1b1/AUTHORS
--rw-rw-r--   0 ago       (1001) ago       (1001)     1548 2024-05-14 18:04:38.000000 ngclearn-1.1b1/LICENSE
--rw-r--r--   0 ago       (1001) ago       (1001)     8044 2024-05-31 19:10:37.012163 ngclearn-1.1b1/PKG-INFO
--rw-rw-r--   0 ago       (1001) ago       (1001)     6321 2024-05-31 19:10:16.000000 ngclearn-1.1b1/README.md
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.004164 ngclearn-1.1b1/ngclearn/
--rw-rw-r--   0 ago       (1001) ago       (1001)     1929 2024-05-31 18:09:26.000000 ngclearn-1.1b1/ngclearn/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.004164 ngclearn-1.1b1/ngclearn/commands/
--rw-rw-r--   0 ago       (1001) ago       (1001)       33 2024-05-14 18:04:38.000000 ngclearn-1.1b1/ngclearn/commands/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.004164 ngclearn-1.1b1/ngclearn/components/
--rw-rw-r--   0 ago       (1001) ago       (1001)     1295 2024-05-30 17:49:04.000000 ngclearn-1.1b1/ngclearn/components/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.004164 ngclearn-1.1b1/ngclearn/components/input_encoders/
--rw-rw-r--   0 ago       (1001) ago       (1001)      118 2024-05-14 18:04:38.000000 ngclearn-1.1b1/ngclearn/components/input_encoders/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     3787 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/components/input_encoders/bernoulliCell.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     9426 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/components/input_encoders/latencyCell.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     4123 2024-05-31 02:48:25.000000 ngclearn-1.1b1/ngclearn/components/input_encoders/poissonCell.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.004164 ngclearn-1.1b1/ngclearn/components/lava/
--rw-rw-r--   0 ago       (1001) ago       (1001)      331 2024-05-30 17:48:13.000000 ngclearn-1.1b1/ngclearn/components/lava/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.004164 ngclearn-1.1b1/ngclearn/components/lava/neurons/
--rw-rw-r--   0 ago       (1001) ago       (1001)     6339 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/components/lava/neurons/LIFCell.py
--rw-rw-r--   0 ago       (1001) ago       (1001)       29 2024-05-30 17:48:13.000000 ngclearn-1.1b1/ngclearn/components/lava/neurons/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.004164 ngclearn-1.1b1/ngclearn/components/lava/synapses/
--rw-rw-r--   0 ago       (1001) ago       (1001)      131 2024-05-30 17:48:13.000000 ngclearn-1.1b1/ngclearn/components/lava/synapses/__init__.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     4441 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/components/lava/synapses/hebbianSynapse.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     3339 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/components/lava/synapses/staticSynapse.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     5544 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/components/lava/synapses/traceSTDPSynapse.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.004164 ngclearn-1.1b1/ngclearn/components/lava/traces/
--rwxrwxr-x   0 ago       (1001) ago       (1001)       36 2024-05-30 17:48:13.000000 ngclearn-1.1b1/ngclearn/components/lava/traces/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     2190 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/components/lava/traces/gatedTrace.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.004164 ngclearn-1.1b1/ngclearn/components/neurons/
--rw-rw-r--   0 ago       (1001) ago       (1001)      566 2024-05-30 17:48:13.000000 ngclearn-1.1b1/ngclearn/components/neurons/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.004164 ngclearn-1.1b1/ngclearn/components/neurons/graded/
--rw-rw-r--   0 ago       (1001) ago       (1001)      178 2024-05-14 18:04:38.000000 ngclearn-1.1b1/ngclearn/components/neurons/graded/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     4442 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/components/neurons/graded/gaussianErrorCell.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     4447 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/components/neurons/graded/laplacianErrorCell.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     9107 2024-05-31 15:46:43.000000 ngclearn-1.1b1/ngclearn/components/neurons/graded/rateCell.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.008164 ngclearn-1.1b1/ngclearn/components/neurons/spiking/
--rw-rw-r--   0 ago       (1001) ago       (1001)    11905 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/components/neurons/spiking/LIFCell.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     6832 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/components/neurons/spiking/WTASCell.py
--rw-rw-r--   0 ago       (1001) ago       (1001)      311 2024-05-30 17:48:13.000000 ngclearn-1.1b1/ngclearn/components/neurons/spiking/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     7943 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/components/neurons/spiking/adExCell.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     8218 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/components/neurons/spiking/fitzhughNagumoCell.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)    10544 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/components/neurons/spiking/izhikevichCell.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)    10762 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/components/neurons/spiking/quadLIFCell.py
--rw-rw-r--   0 ago       (1001) ago       (1001)    13349 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/components/neurons/spiking/sLIFCell.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.008164 ngclearn-1.1b1/ngclearn/components/other/
--rw-rw-r--   0 ago       (1001) ago       (1001)       64 2024-05-26 02:51:19.000000 ngclearn-1.1b1/ngclearn/components/other/__init__.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     3882 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/components/other/expKernel.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     4921 2024-05-31 18:05:43.000000 ngclearn-1.1b1/ngclearn/components/other/varTrace.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.008164 ngclearn-1.1b1/ngclearn/components/synapses/
--rw-rw-r--   0 ago       (1001) ago       (1001)      258 2024-05-30 18:14:10.000000 ngclearn-1.1b1/ngclearn/components/synapses/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.008164 ngclearn-1.1b1/ngclearn/components/synapses/hebbian/
--rw-rw-r--   0 ago       (1001) ago       (1001)      184 2024-05-30 17:48:13.000000 ngclearn-1.1b1/ngclearn/components/synapses/hebbian/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     7020 2024-05-31 15:46:43.000000 ngclearn-1.1b1/ngclearn/components/synapses/hebbian/eventSTDPSynapse.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     8872 2024-05-31 15:46:43.000000 ngclearn-1.1b1/ngclearn/components/synapses/hebbian/expSTDPSynapse.py
--rw-rw-r--   0 ago       (1001) ago       (1001)    11041 2024-05-31 15:46:43.000000 ngclearn-1.1b1/ngclearn/components/synapses/hebbian/hebbianSynapse.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     9272 2024-05-31 15:46:43.000000 ngclearn-1.1b1/ngclearn/components/synapses/hebbian/traceSTDPSynapse.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     4614 2024-05-31 15:46:43.000000 ngclearn-1.1b1/ngclearn/components/synapses/staticSynapse.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.008164 ngclearn-1.1b1/ngclearn/operations/
--rw-rw-r--   0 ago       (1001) ago       (1001)       34 2024-05-31 14:19:32.000000 ngclearn-1.1b1/ngclearn/operations/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.008164 ngclearn-1.1b1/ngclearn/utils/
--rwxrwxr-x   0 ago       (1001) ago       (1001)       37 2024-05-30 17:48:13.000000 ngclearn-1.1b1/ngclearn/utils/__init__.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     3230 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/utils/data_loader.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.008164 ngclearn-1.1b1/ngclearn/utils/density/
--rw-rw-r--   0 ago       (1001) ago       (1001)        0 2024-05-14 18:04:38.000000 ngclearn-1.1b1/ngclearn/utils/density/__init__.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     2816 2024-05-14 18:04:38.000000 ngclearn-1.1b1/ngclearn/utils/density/gmm.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.008164 ngclearn-1.1b1/ngclearn/utils/diffeq/
--rw-rw-r--   0 ago       (1001) ago       (1001)        0 2024-05-14 18:04:38.000000 ngclearn-1.1b1/ngclearn/utils/diffeq/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     7349 2024-05-14 18:04:38.000000 ngclearn-1.1b1/ngclearn/utils/diffeq/ode_utils.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     1629 2024-05-14 18:04:38.000000 ngclearn-1.1b1/ngclearn/utils/io_utils.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     7970 2024-05-30 17:48:13.000000 ngclearn-1.1b1/ngclearn/utils/metric_utils.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)    16804 2024-05-31 14:06:30.000000 ngclearn-1.1b1/ngclearn/utils/model_utils.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.008164 ngclearn-1.1b1/ngclearn/utils/optim/
--rw-rw-r--   0 ago       (1001) ago       (1001)       59 2024-05-30 17:48:13.000000 ngclearn-1.1b1/ngclearn/utils/optim/__init__.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     3769 2024-05-30 17:48:13.000000 ngclearn-1.1b1/ngclearn/utils/optim/adam.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)      487 2024-05-30 17:48:13.000000 ngclearn-1.1b1/ngclearn/utils/optim/optim_utils.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     1583 2024-05-30 17:48:13.000000 ngclearn-1.1b1/ngclearn/utils/optim/sgd.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     3177 2024-05-31 15:46:43.000000 ngclearn-1.1b1/ngclearn/utils/patch_utils.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     5690 2024-05-14 18:04:38.000000 ngclearn-1.1b1/ngclearn/utils/surrogate_fx.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.008164 ngclearn-1.1b1/ngclearn/utils/viz/
--rw-rw-r--   0 ago       (1001) ago       (1001)        0 2024-05-14 18:04:38.000000 ngclearn-1.1b1/ngclearn/utils/viz/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     3485 2024-05-30 17:48:13.000000 ngclearn-1.1b1/ngclearn/utils/viz/dim_reduce.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     5418 2024-05-30 17:48:13.000000 ngclearn-1.1b1/ngclearn/utils/viz/raster.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     2673 2024-05-30 17:48:13.000000 ngclearn-1.1b1/ngclearn/utils/viz/spike_plot.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     6382 2024-05-31 14:19:32.000000 ngclearn-1.1b1/ngclearn/utils/viz/synapse_plot.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.012163 ngclearn-1.1b1/ngclearn.egg-info/
--rw-r--r--   0 ago       (1001) ago       (1001)     8044 2024-05-31 19:10:36.000000 ngclearn-1.1b1/ngclearn.egg-info/PKG-INFO
--rw-rw-r--   0 ago       (1001) ago       (1001)     3017 2024-05-31 19:10:37.000000 ngclearn-1.1b1/ngclearn.egg-info/SOURCES.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)        1 2024-05-31 19:10:36.000000 ngclearn-1.1b1/ngclearn.egg-info/dependency_links.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-05-31 19:10:36.000000 ngclearn-1.1b1/ngclearn.egg-info/requires.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)       54 2024-05-31 19:10:36.000000 ngclearn-1.1b1/ngclearn.egg-info/top_level.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)     1711 2024-05-31 18:09:08.000000 ngclearn-1.1b1/pyproject.toml
--rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-05-31 19:09:52.000000 ngclearn-1.1b1/requirements.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)       38 2024-05-31 19:10:37.012163 ngclearn-1.1b1/setup.cfg
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.012163 ngclearn-1.1b1/test_code/
--rwxr-xr-x   0 ago       (1001) ago       (1001)     3072 2024-05-28 21:11:49.000000 ngclearn-1.1b1/test_code/_run_trstdp.py
--rw-r--r--   0 ago       (1001) ago       (1001)      968 2024-05-18 01:01:58.000000 ngclearn-1.1b1/test_code/adex.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     1194 2024-05-25 16:47:53.000000 ngclearn-1.1b1/test_code/calc_fanoFactor.py
--rw-rw-r--   0 ago       (1001) ago       (1001)      971 2024-05-25 21:40:48.000000 ngclearn-1.1b1/test_code/run2_metrics.py
--rwxr-xr-x   0 ago       (1001) ago       (1001)     2634 2024-05-26 04:20:56.000000 ngclearn-1.1b1/test_code/run_expkernel.py
--rw-rw-r--   0 ago       (1001) ago       (1001)      889 2024-05-25 21:04:53.000000 ngclearn-1.1b1/test_code/run_metrics.py
--rwxr-xr-x   0 ago       (1001) ago       (1001)     2423 2024-05-25 23:21:31.000000 ngclearn-1.1b1/test_code/run_trace.py
--rwxr-xr-x   0 ago       (1001) ago       (1001)     3437 2024-05-29 02:43:08.000000 ngclearn-1.1b1/test_code/run_trstdp.py
--rw-r--r--   0 ago       (1001) ago       (1001)     5589 2024-05-18 01:04:05.000000 ngclearn-1.1b1/test_code/test_adex.py
--rw-r--r--   0 ago       (1001) ago       (1001)     4518 2024-05-16 23:45:02.000000 ngclearn-1.1b1/test_code/test_fhcell.py
--rwxr-xr-x   0 ago       (1001) ago       (1001)     5396 2024-05-18 00:09:30.000000 ngclearn-1.1b1/test_code/test_izhcell.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     1213 2024-05-25 22:26:28.000000 ngclearn-1.1b1/test_code/viz_data.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 19:10:37.012163 ngclearn-1.1b1/test_lava/
--rwxr-xr-x   0 ago       (1001) ago       (1001)     6684 2024-05-29 21:05:11.000000 ngclearn-1.1b1/test_lava/run_xotSNN.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.722972 ngclearn-1.1b2/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      402 2024-05-31 17:48:58.000000 ngclearn-1.1b2/AUTHORS
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1548 2024-05-14 18:04:38.000000 ngclearn-1.1b2/LICENSE
+-rw-r--r--   0 ago       (1001) ago       (1001)     8044 2024-06-02 21:57:16.722972 ngclearn-1.1b2/PKG-INFO
+-rw-rw-r--   0 ago       (1001) ago       (1001)     6321 2024-06-02 21:56:46.000000 ngclearn-1.1b2/README.md
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.714972 ngclearn-1.1b2/ngclearn/
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1929 2024-05-31 18:09:26.000000 ngclearn-1.1b2/ngclearn/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.714972 ngclearn-1.1b2/ngclearn/commands/
+-rw-rw-r--   0 ago       (1001) ago       (1001)       33 2024-05-14 18:04:38.000000 ngclearn-1.1b2/ngclearn/commands/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.714972 ngclearn-1.1b2/ngclearn/components/
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1295 2024-05-30 17:49:04.000000 ngclearn-1.1b2/ngclearn/components/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.714972 ngclearn-1.1b2/ngclearn/components/input_encoders/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      118 2024-05-14 18:04:38.000000 ngclearn-1.1b2/ngclearn/components/input_encoders/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     3955 2024-06-02 21:43:27.000000 ngclearn-1.1b2/ngclearn/components/input_encoders/bernoulliCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     9635 2024-06-02 21:43:27.000000 ngclearn-1.1b2/ngclearn/components/input_encoders/latencyCell.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     4285 2024-06-02 21:43:27.000000 ngclearn-1.1b2/ngclearn/components/input_encoders/poissonCell.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.714972 ngclearn-1.1b2/ngclearn/components/lava/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      331 2024-05-30 17:48:13.000000 ngclearn-1.1b2/ngclearn/components/lava/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.714972 ngclearn-1.1b2/ngclearn/components/lava/neurons/
+-rw-rw-r--   0 ago       (1001) ago       (1001)     6339 2024-05-31 14:06:30.000000 ngclearn-1.1b2/ngclearn/components/lava/neurons/LIFCell.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)       29 2024-05-30 17:48:13.000000 ngclearn-1.1b2/ngclearn/components/lava/neurons/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.714972 ngclearn-1.1b2/ngclearn/components/lava/synapses/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      131 2024-05-30 17:48:13.000000 ngclearn-1.1b2/ngclearn/components/lava/synapses/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     4441 2024-05-31 14:06:30.000000 ngclearn-1.1b2/ngclearn/components/lava/synapses/hebbianSynapse.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     3339 2024-05-31 14:06:30.000000 ngclearn-1.1b2/ngclearn/components/lava/synapses/staticSynapse.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     5544 2024-05-31 14:06:30.000000 ngclearn-1.1b2/ngclearn/components/lava/synapses/traceSTDPSynapse.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.714972 ngclearn-1.1b2/ngclearn/components/lava/traces/
+-rwxrwxr-x   0 ago       (1001) ago       (1001)       36 2024-05-30 17:48:13.000000 ngclearn-1.1b2/ngclearn/components/lava/traces/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     2190 2024-05-31 14:06:30.000000 ngclearn-1.1b2/ngclearn/components/lava/traces/gatedTrace.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.714972 ngclearn-1.1b2/ngclearn/components/neurons/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      566 2024-05-30 17:48:13.000000 ngclearn-1.1b2/ngclearn/components/neurons/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.714972 ngclearn-1.1b2/ngclearn/components/neurons/graded/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      178 2024-05-14 18:04:38.000000 ngclearn-1.1b2/ngclearn/components/neurons/graded/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     4810 2024-06-02 21:43:27.000000 ngclearn-1.1b2/ngclearn/components/neurons/graded/gaussianErrorCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     4815 2024-06-02 21:43:27.000000 ngclearn-1.1b2/ngclearn/components/neurons/graded/laplacianErrorCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     9850 2024-06-02 21:43:27.000000 ngclearn-1.1b2/ngclearn/components/neurons/graded/rateCell.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.718972 ngclearn-1.1b2/ngclearn/components/neurons/spiking/
+-rw-rw-r--   0 ago       (1001) ago       (1001)    12451 2024-06-02 21:43:27.000000 ngclearn-1.1b2/ngclearn/components/neurons/spiking/LIFCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     7150 2024-06-02 21:43:27.000000 ngclearn-1.1b2/ngclearn/components/neurons/spiking/WTASCell.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)      311 2024-05-30 17:48:13.000000 ngclearn-1.1b2/ngclearn/components/neurons/spiking/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     8231 2024-06-02 21:43:27.000000 ngclearn-1.1b2/ngclearn/components/neurons/spiking/adExCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     8506 2024-06-02 21:43:27.000000 ngclearn-1.1b2/ngclearn/components/neurons/spiking/fitzhughNagumoCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)    10832 2024-06-02 21:43:27.000000 ngclearn-1.1b2/ngclearn/components/neurons/spiking/izhikevichCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)    11230 2024-06-02 21:43:27.000000 ngclearn-1.1b2/ngclearn/components/neurons/spiking/quadLIFCell.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)    13782 2024-06-02 21:43:27.000000 ngclearn-1.1b2/ngclearn/components/neurons/spiking/sLIFCell.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.718972 ngclearn-1.1b2/ngclearn/components/other/
+-rw-rw-r--   0 ago       (1001) ago       (1001)       64 2024-05-26 02:51:19.000000 ngclearn-1.1b2/ngclearn/components/other/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     4070 2024-06-02 21:43:27.000000 ngclearn-1.1b2/ngclearn/components/other/expKernel.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     5098 2024-06-02 21:43:27.000000 ngclearn-1.1b2/ngclearn/components/other/varTrace.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.718972 ngclearn-1.1b2/ngclearn/components/synapses/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      258 2024-05-30 18:14:10.000000 ngclearn-1.1b2/ngclearn/components/synapses/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.718972 ngclearn-1.1b2/ngclearn/components/synapses/hebbian/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      184 2024-05-30 17:48:13.000000 ngclearn-1.1b2/ngclearn/components/synapses/hebbian/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     7678 2024-06-02 21:46:43.000000 ngclearn-1.1b2/ngclearn/components/synapses/hebbian/eventSTDPSynapse.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     9519 2024-06-02 21:46:43.000000 ngclearn-1.1b2/ngclearn/components/synapses/hebbian/expSTDPSynapse.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)    11772 2024-06-02 21:46:43.000000 ngclearn-1.1b2/ngclearn/components/synapses/hebbian/hebbianSynapse.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     9930 2024-06-02 21:46:43.000000 ngclearn-1.1b2/ngclearn/components/synapses/hebbian/traceSTDPSynapse.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     4788 2024-06-02 21:43:27.000000 ngclearn-1.1b2/ngclearn/components/synapses/staticSynapse.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.718972 ngclearn-1.1b2/ngclearn/operations/
+-rw-rw-r--   0 ago       (1001) ago       (1001)       34 2024-05-31 14:19:32.000000 ngclearn-1.1b2/ngclearn/operations/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.718972 ngclearn-1.1b2/ngclearn/utils/
+-rwxrwxr-x   0 ago       (1001) ago       (1001)       37 2024-05-30 17:48:13.000000 ngclearn-1.1b2/ngclearn/utils/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     3230 2024-05-31 14:06:30.000000 ngclearn-1.1b2/ngclearn/utils/data_loader.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.718972 ngclearn-1.1b2/ngclearn/utils/density/
+-rw-rw-r--   0 ago       (1001) ago       (1001)        0 2024-05-14 18:04:38.000000 ngclearn-1.1b2/ngclearn/utils/density/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     2816 2024-05-14 18:04:38.000000 ngclearn-1.1b2/ngclearn/utils/density/gmm.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.718972 ngclearn-1.1b2/ngclearn/utils/diffeq/
+-rw-rw-r--   0 ago       (1001) ago       (1001)        0 2024-05-14 18:04:38.000000 ngclearn-1.1b2/ngclearn/utils/diffeq/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     7349 2024-05-14 18:04:38.000000 ngclearn-1.1b2/ngclearn/utils/diffeq/ode_utils.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     1629 2024-05-14 18:04:38.000000 ngclearn-1.1b2/ngclearn/utils/io_utils.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     7970 2024-05-30 17:48:13.000000 ngclearn-1.1b2/ngclearn/utils/metric_utils.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)    17079 2024-06-02 19:15:44.000000 ngclearn-1.1b2/ngclearn/utils/model_utils.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.718972 ngclearn-1.1b2/ngclearn/utils/optim/
+-rw-rw-r--   0 ago       (1001) ago       (1001)       59 2024-05-30 17:48:13.000000 ngclearn-1.1b2/ngclearn/utils/optim/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     3769 2024-05-30 17:48:13.000000 ngclearn-1.1b2/ngclearn/utils/optim/adam.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)      487 2024-05-30 17:48:13.000000 ngclearn-1.1b2/ngclearn/utils/optim/optim_utils.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     1583 2024-05-30 17:48:13.000000 ngclearn-1.1b2/ngclearn/utils/optim/sgd.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     3220 2024-06-01 23:44:39.000000 ngclearn-1.1b2/ngclearn/utils/patch_utils.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     5690 2024-05-14 18:04:38.000000 ngclearn-1.1b2/ngclearn/utils/surrogate_fx.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.718972 ngclearn-1.1b2/ngclearn/utils/viz/
+-rw-rw-r--   0 ago       (1001) ago       (1001)        0 2024-05-14 18:04:38.000000 ngclearn-1.1b2/ngclearn/utils/viz/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     3485 2024-05-30 17:48:13.000000 ngclearn-1.1b2/ngclearn/utils/viz/dim_reduce.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     5489 2024-06-01 03:39:22.000000 ngclearn-1.1b2/ngclearn/utils/viz/raster.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     2673 2024-05-30 17:48:13.000000 ngclearn-1.1b2/ngclearn/utils/viz/spike_plot.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     6382 2024-05-31 14:19:32.000000 ngclearn-1.1b2/ngclearn/utils/viz/synapse_plot.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.722972 ngclearn-1.1b2/ngclearn.egg-info/
+-rw-r--r--   0 ago       (1001) ago       (1001)     8044 2024-06-02 21:57:16.000000 ngclearn-1.1b2/ngclearn.egg-info/PKG-INFO
+-rw-rw-r--   0 ago       (1001) ago       (1001)     3017 2024-06-02 21:57:16.000000 ngclearn-1.1b2/ngclearn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)        1 2024-06-02 21:57:16.000000 ngclearn-1.1b2/ngclearn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-06-02 21:57:16.000000 ngclearn-1.1b2/ngclearn.egg-info/requires.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)       54 2024-06-02 21:57:16.000000 ngclearn-1.1b2/ngclearn.egg-info/top_level.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1711 2024-06-02 21:55:51.000000 ngclearn-1.1b2/pyproject.toml
+-rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-05-31 19:12:45.000000 ngclearn-1.1b2/requirements.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)       38 2024-06-02 21:57:16.722972 ngclearn-1.1b2/setup.cfg
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.722972 ngclearn-1.1b2/test_code/
+-rwxr-xr-x   0 ago       (1001) ago       (1001)     3072 2024-05-28 21:11:49.000000 ngclearn-1.1b2/test_code/_run_trstdp.py
+-rw-r--r--   0 ago       (1001) ago       (1001)      968 2024-05-18 01:01:58.000000 ngclearn-1.1b2/test_code/adex.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1194 2024-05-25 16:47:53.000000 ngclearn-1.1b2/test_code/calc_fanoFactor.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)      971 2024-05-25 21:40:48.000000 ngclearn-1.1b2/test_code/run2_metrics.py
+-rwxr-xr-x   0 ago       (1001) ago       (1001)     2634 2024-05-26 04:20:56.000000 ngclearn-1.1b2/test_code/run_expkernel.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)      889 2024-05-25 21:04:53.000000 ngclearn-1.1b2/test_code/run_metrics.py
+-rwxr-xr-x   0 ago       (1001) ago       (1001)     2423 2024-05-25 23:21:31.000000 ngclearn-1.1b2/test_code/run_trace.py
+-rwxr-xr-x   0 ago       (1001) ago       (1001)     3437 2024-05-29 02:43:08.000000 ngclearn-1.1b2/test_code/run_trstdp.py
+-rw-r--r--   0 ago       (1001) ago       (1001)     5589 2024-05-18 01:04:05.000000 ngclearn-1.1b2/test_code/test_adex.py
+-rw-r--r--   0 ago       (1001) ago       (1001)     4518 2024-05-16 23:45:02.000000 ngclearn-1.1b2/test_code/test_fhcell.py
+-rwxr-xr-x   0 ago       (1001) ago       (1001)     5396 2024-05-18 00:09:30.000000 ngclearn-1.1b2/test_code/test_izhcell.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1213 2024-05-25 22:26:28.000000 ngclearn-1.1b2/test_code/viz_data.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-06-02 21:57:16.722972 ngclearn-1.1b2/test_lava/
+-rwxr-xr-x   0 ago       (1001) ago       (1001)     6684 2024-05-29 21:05:11.000000 ngclearn-1.1b2/test_lava/run_xotSNN.py
```

### Comparing `ngclearn-1.1b1/LICENSE` & `ngclearn-1.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/PKG-INFO` & `ngclearn-1.1b2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngclearn
-Version: 1.1b1
+Version: 1.1b2
 Summary: Simulation software for building and analyzing arbitrary predictive coding, spiking network, and biomimetic neural systems.
 Author-email: Alexander Ororbia <ago@cs.rit.edu>, William Gebhardt <wdg1351@rit.edu>
 License: BSD-3-Clause License
 Project-URL: Homepage, https://github.com/NACLab/ngc-learn
 Project-URL: Documentation, https://ngc-learn.readthedocs.io/
 Project-URL: Lab Page, https://www.cs.rit.edu/~ago/nac_lab.html
 Project-URL: Changelog, https://github.com/NACLab/ngc-learn/blob/main/history.txt
@@ -80,15 +80,15 @@
 5) scikit-learn (>=1.3.1) if using `ngclearn.utils.density`
 6) matplotlib (>=3.4.3) if using `ngclearn.utils.viz`
 6) networkx  (>=2.6.3) (currently optional but required if using `ngclearn.utils.experimental.viz_utils`)
 7) pyviz (>=0.2.0) (currently optional but required if using `ngclearn.utils.experimental.viz_utils`)
 -->
 
 ---
-ngc-learn 1.0.beta0 and later require Python 3.10 or newer as well as ngcsimlib >=0.2.b2.
+ngc-learn 1.1.beta2 and later require Python 3.10 or newer as well as ngcsimlib >=0.3.b1.
 ngc-learn's plotting capabilities (routines within `ngclearn.utils.viz`) require
 Matplotlib (>=3.8.0) and imageio (>=2.31.5) and both plotting and density estimation
 tools (routines within ``ngclearn.utils.density``) will require Scikit-learn (>=0.24.2).
 Many of the tutorials will require Matplotlib (>=3.8.0), imageio (>=2.31.5), and Scikit-learn (>=0.24.2).
 <!-- (Note: if using the `_generate_patch_set()` within the
 image patching utilities, then Patchify will be needed).-->
 
@@ -115,15 +115,15 @@
 right major and minor version of ngc-learn):
 
 ```console
 Python 3.11.4 (main, MONTH  DAY YEAR, TIME) [GCC XX.X.X] on linux
 Type "help", "copyright", "credits" or "license" for more information.
 >>> import ngclearn
 >>> ngclearn.__version__
-'1.0b3'
+'1.1b2'
 ```
 
 <i>Note:</i> For access to the previous Tensorflow-2 version of ngc-learn (of
 which we no longer support), please visit the repo for
 <a href="https://github.com/NACLab/ngc-learn-legacy"><i>ngc-learn-legacy</i></a>.
 
 ## <b>Attribution:</b>
@@ -162,15 +162,15 @@
 If you are working on and developing with ngc-learn pulled from the github
 repo, then run the following command to set up an editable install:
 <pre>
 $ python install -e .
 </pre>
 
 **Version:**<br>
-1.1.1-Beta <!-- -Alpha -->
+1.1.2-Beta <!-- -Alpha -->
 
 Author:
 Alexander G. Ororbia II<br>
 Director, Neural Adaptive Computing (NAC) Laboratory<br>
 Rochester Institute of Technology, Department of Computer Science
 
 ## <b>Copyright:</b>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ngclearn Version: 1.1b1 Summary: Simulation
+Metadata-Version: 2.1 Name: ngclearn Version: 1.1b2 Summary: Simulation
 software for building and analyzing arbitrary predictive coding, spiking
 network, and biomimetic neural systems. Author-email: Alexander Ororbia
 cs.rit.edu>, William Gebhardt
 rit.edu> License: BSD-3-Clause License Project-URL: Homepage, https://
 github.com/NACLab/ngc-learn Project-URL: Documentation, https://ngc-
 learn.readthedocs.io/ Project-URL: Lab Page, https://www.cs.rit.edu/~ago/
 nac_lab.html Project-URL: Changelog, https://github.com/NACLab/ngc-learn/blob/
@@ -42,16 +42,16 @@
 library can be found _h_e_r_e.
 You can find the related paper _r_i_g_h_t_ _h_e_r_e, which was selected to appear in the
 Nature Neuromorphic Hardware and Computing Collection in 2023 and was chosen as
 one of the Editors' Highlights for Applied Physics and Mathematics in 2022. ##
 Installation ### Dependencies ngc-learn requires: 1) Python (>=3.10) 2) NumPy
 (>=1.26.0) 3) SciPy (>=1.7.0) 4) ngcsimlib (>=0.2.b1), (visit official page
 _h_e_r_e) 5) JAX (>= 0.4.18) (to enable GPU use, make sure to install one of the
-CUDA variants) --- ngc-learn 1.0.beta0 and later require Python 3.10 or newer
-as well as ngcsimlib >=0.2.b2. ngc-learn's plotting capabilities (routines
+CUDA variants) --- ngc-learn 1.1.beta2 and later require Python 3.10 or newer
+as well as ngcsimlib >=0.3.b1. ngc-learn's plotting capabilities (routines
 within `ngclearn.utils.viz`) require Matplotlib (>=3.8.0) and imageio
 (>=2.31.5) and both plotting and density estimation tools (routines within
 ``ngclearn.utils.density``) will require Scikit-learn (>=0.24.2). Many of the
 tutorials will require Matplotlib (>=3.8.0), imageio (>=2.31.5), and Scikit-
 learn (>=0.24.2). ### User Installation Setup: The easiest way to install ngc-
 learn is through pip:
 $ pip install ngclearn
@@ -63,15 +63,15 @@
 library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and 20.04.
 If the installation was successful, you should see the following if you test it
 against your Python interpreter, i.e., run the $ python command and complete
 the following sequence of steps as depicted in the screenshot below (you should
 see at the bottom of your output something akin to the right major and minor
 version of ngc-learn): ```console Python 3.11.4 (main, MONTH DAY YEAR, TIME)
 [GCC XX.X.X] on linux Type "help", "copyright", "credits" or "license" for more
-information. >>> import ngclearn >>> ngclearn.__version__ '1.0b3' ``` Note: For
+information. >>> import ngclearn >>> ngclearn.__version__ '1.1b2' ``` Note: For
 access to the previous Tensorflow-2 version of ngc-learn (of which we no longer
 support), please visit the repo for _n_g_c_-_l_e_a_r_n_-_l_e_g_a_c_y. ## AAttttrriibbuuttiioonn:: If you
 use this code in any form in your project(s), please cite its source paper (as
 well as ngc-learn's official software citation):
 @article{Ororbia2022,
   author={Ororbia, Alexander and Kifer, Daniel},
   title={The neural coding framework for learning generative models},
@@ -91,15 +91,15 @@
 [contributing guidelines](CONTRIBUTING.md). SSoouurrccee CCooddee You can check/pull the
 latest source code for this library via:
 $ git clone https://github.com/NACLab/ngc-learn.git
 If you are working on and developing with ngc-learn pulled from the github
 repo, then run the following command to set up an editable install:
 $ python install -e .
 **Version:**
-1.1.1-Beta Author: Alexander G. Ororbia II
+1.1.2-Beta Author: Alexander G. Ororbia II
 Director, Neural Adaptive Computing (NAC) Laboratory
 Rochester Institute of Technology, Department of Computer Science ## CCooppyyrriigghhtt::
 Copyright (C) 2021 The Neural Adaptive Computing Laboratory - All Rights
 Reserved
 You may use, distribute and modify this code under the terms of the BSD 3-
 clause license. You should have received a copy of the BSD 3-clause license
 with this software.
```

### Comparing `ngclearn-1.1b1/README.md` & `ngclearn-1.1b2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 5) scikit-learn (>=1.3.1) if using `ngclearn.utils.density`
 6) matplotlib (>=3.4.3) if using `ngclearn.utils.viz`
 6) networkx  (>=2.6.3) (currently optional but required if using `ngclearn.utils.experimental.viz_utils`)
 7) pyviz (>=0.2.0) (currently optional but required if using `ngclearn.utils.experimental.viz_utils`)
 -->
 
 ---
-ngc-learn 1.0.beta0 and later require Python 3.10 or newer as well as ngcsimlib >=0.2.b2.
+ngc-learn 1.1.beta2 and later require Python 3.10 or newer as well as ngcsimlib >=0.3.b1.
 ngc-learn's plotting capabilities (routines within `ngclearn.utils.viz`) require
 Matplotlib (>=3.8.0) and imageio (>=2.31.5) and both plotting and density estimation
 tools (routines within ``ngclearn.utils.density``) will require Scikit-learn (>=0.24.2).
 Many of the tutorials will require Matplotlib (>=3.8.0), imageio (>=2.31.5), and Scikit-learn (>=0.24.2).
 <!-- (Note: if using the `_generate_patch_set()` within the
 image patching utilities, then Patchify will be needed).-->
 
@@ -77,15 +77,15 @@
 right major and minor version of ngc-learn):
 
 ```console
 Python 3.11.4 (main, MONTH  DAY YEAR, TIME) [GCC XX.X.X] on linux
 Type "help", "copyright", "credits" or "license" for more information.
 >>> import ngclearn
 >>> ngclearn.__version__
-'1.0b3'
+'1.1b2'
 ```
 
 <i>Note:</i> For access to the previous Tensorflow-2 version of ngc-learn (of
 which we no longer support), please visit the repo for
 <a href="https://github.com/NACLab/ngc-learn-legacy"><i>ngc-learn-legacy</i></a>.
 
 ## <b>Attribution:</b>
@@ -124,15 +124,15 @@
 If you are working on and developing with ngc-learn pulled from the github
 repo, then run the following command to set up an editable install:
 <pre>
 $ python install -e .
 </pre>
 
 **Version:**<br>
-1.1.1-Beta <!-- -Alpha -->
+1.1.2-Beta <!-- -Alpha -->
 
 Author:
 Alexander G. Ororbia II<br>
 Director, Neural Adaptive Computing (NAC) Laboratory<br>
 Rochester Institute of Technology, Department of Computer Science
 
 ## <b>Copyright:</b>
```

#### html2text {}

```diff
@@ -18,16 +18,16 @@
 behind this software library can be found _h_e_r_e.
 You can find the related paper _r_i_g_h_t_ _h_e_r_e, which was selected to appear in the
 Nature Neuromorphic Hardware and Computing Collection in 2023 and was chosen as
 one of the Editors' Highlights for Applied Physics and Mathematics in 2022. ##
 Installation ### Dependencies ngc-learn requires: 1) Python (>=3.10) 2) NumPy
 (>=1.26.0) 3) SciPy (>=1.7.0) 4) ngcsimlib (>=0.2.b1), (visit official page
 _h_e_r_e) 5) JAX (>= 0.4.18) (to enable GPU use, make sure to install one of the
-CUDA variants) --- ngc-learn 1.0.beta0 and later require Python 3.10 or newer
-as well as ngcsimlib >=0.2.b2. ngc-learn's plotting capabilities (routines
+CUDA variants) --- ngc-learn 1.1.beta2 and later require Python 3.10 or newer
+as well as ngcsimlib >=0.3.b1. ngc-learn's plotting capabilities (routines
 within `ngclearn.utils.viz`) require Matplotlib (>=3.8.0) and imageio
 (>=2.31.5) and both plotting and density estimation tools (routines within
 ``ngclearn.utils.density``) will require Scikit-learn (>=0.24.2). Many of the
 tutorials will require Matplotlib (>=3.8.0), imageio (>=2.31.5), and Scikit-
 learn (>=0.24.2). ### User Installation Setup: The easiest way to install ngc-
 learn is through pip:
 $ pip install ngclearn
@@ -39,15 +39,15 @@
 library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and 20.04.
 If the installation was successful, you should see the following if you test it
 against your Python interpreter, i.e., run the $ python command and complete
 the following sequence of steps as depicted in the screenshot below (you should
 see at the bottom of your output something akin to the right major and minor
 version of ngc-learn): ```console Python 3.11.4 (main, MONTH DAY YEAR, TIME)
 [GCC XX.X.X] on linux Type "help", "copyright", "credits" or "license" for more
-information. >>> import ngclearn >>> ngclearn.__version__ '1.0b3' ``` Note: For
+information. >>> import ngclearn >>> ngclearn.__version__ '1.1b2' ``` Note: For
 access to the previous Tensorflow-2 version of ngc-learn (of which we no longer
 support), please visit the repo for _n_g_c_-_l_e_a_r_n_-_l_e_g_a_c_y. ## AAttttrriibbuuttiioonn:: If you
 use this code in any form in your project(s), please cite its source paper (as
 well as ngc-learn's official software citation):
 @article{Ororbia2022,
   author={Ororbia, Alexander and Kifer, Daniel},
   title={The neural coding framework for learning generative models},
@@ -67,15 +67,15 @@
 [contributing guidelines](CONTRIBUTING.md). SSoouurrccee CCooddee You can check/pull the
 latest source code for this library via:
 $ git clone https://github.com/NACLab/ngc-learn.git
 If you are working on and developing with ngc-learn pulled from the github
 repo, then run the following command to set up an editable install:
 $ python install -e .
 **Version:**
-1.1.1-Beta Author: Alexander G. Ororbia II
+1.1.2-Beta Author: Alexander G. Ororbia II
 Director, Neural Adaptive Computing (NAC) Laboratory
 Rochester Institute of Technology, Department of Computer Science ## CCooppyyrriigghhtt::
 Copyright (C) 2021 The Neural Adaptive Computing Laboratory - All Rights
 Reserved
 You may use, distribute and modify this code under the terms of the BSD 3-
 clause license. You should have received a copy of the BSD 3-clause license
 with this software.
```

### Comparing `ngclearn-1.1b1/ngclearn/__init__.py` & `ngclearn-1.1b2/ngclearn/__init__.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn/components/__init__.py` & `ngclearn-1.1b2/ngclearn/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn/components/input_encoders/bernoulliCell.py` & `ngclearn-1.1b2/ngclearn/components/input_encoders/bernoulliCell.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,20 @@
     s_t = random.bernoulli(dkey, p=data).astype(jnp.float32)
     return s_t
 
 class BernoulliCell(Component):
     """
     A Bernoulli cell that produces Bernoulli-distributed spikes on-the-fly.
 
+    | --- Cell Compartments: ---
+    | inputs - input (takes in external signals)
+    | outputs - output
+    | tols - time-of-last-spike
+    | key - JAX RNG key
+
     Args:
         name: the string name of this cell
 
         n_units: number of cellular entities (neural population size)
 
         key: PRNG key to control determinism of any underlying synapses
             associated with this cell
```

### Comparing `ngclearn-1.1b1/ngclearn/components/input_encoders/latencyCell.py` & `ngclearn-1.1b2/ngclearn/components/input_encoders/latencyCell.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,14 +113,21 @@
     return spikes_t, _mask
 
 class LatencyCell(Component):
     """
     A (nonlinear) latency encoding (spike) cell; produces a time-lagged set of
     spikes on-the-fly.
 
+    | --- Cell Compartments: ---
+    | inputs - input (takes in external signals)
+    | outputs - output
+    | tols - time-of-last-spike
+    | targ_sp_times - target-spike-time
+    | key - JAX RNG key
+
     Args:
         name: the string name of this cell
 
         n_units: number of cellular entities (neural population size)
 
         tau: time constant for model used to calculate firing time (Default: 1 ms)
```

### Comparing `ngclearn-1.1b1/ngclearn/components/input_encoders/poissonCell.py` & `ngclearn-1.1b2/ngclearn/components/input_encoders/poissonCell.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,20 @@
     s_t = (eps < pspike).astype(jnp.float32)
     return s_t
 
 class PoissonCell(Component):
     """
     A Poisson cell that produces approximately Poisson-distributed spikes on-the-fly.
 
+    | --- Cell Compartments: ---
+    | inputs - input (takes in external signals)
+    | outputs - output
+    | tols - time-of-last-spike
+    | key - JAX RNG key
+
     Args:
         name: the string name of this cell
 
         n_units: number of cellular entities (neural population size)
 
         max_freq: maximum frequency (in Hertz) of this Poisson spike train (must be > 0.)
```

### Comparing `ngclearn-1.1b1/ngclearn/components/lava/neurons/LIFCell.py` & `ngclearn-1.1b2/ngclearn/components/lava/neurons/LIFCell.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn/components/lava/synapses/hebbianSynapse.py` & `ngclearn-1.1b2/ngclearn/components/lava/synapses/hebbianSynapse.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn/components/lava/synapses/staticSynapse.py` & `ngclearn-1.1b2/ngclearn/components/lava/synapses/staticSynapse.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn/components/lava/synapses/traceSTDPSynapse.py` & `ngclearn-1.1b2/ngclearn/components/lava/synapses/traceSTDPSynapse.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn/components/lava/traces/gatedTrace.py` & `ngclearn-1.1b2/ngclearn/components/lava/traces/gatedTrace.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn/components/neurons/__init__.py` & `ngclearn-1.1b2/ngclearn/components/neurons/__init__.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn/components/neurons/graded/gaussianErrorCell.py` & `ngclearn-1.1b2/ngclearn/components/neurons/graded/gaussianErrorCell.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,22 @@
     return dmu, dtarg, L
 
 class GaussianErrorCell(Component): ## Rate-coded/real-valued error unit/cell
     """
     A simple (non-spiking) Gaussian error cell - this is a fixed-point solution
     of a mismatch signal.
 
+    | --- Cell Compartments: ---
+    | mu - predicted value (takes in external signals)
+    | target - desired/goal value (takes in external signals)
+    | L - local loss function embodied by this cell
+    | dmu - derivative of L w.r.t. mu
+    | dtarget - derivative of L w.r.t. target
+    | modulator - modulation signal (takes in optional external signals)
+
     Args:
         name: the string name of this cell
 
         n_units: number of cellular entities (neural population size)
 
         tau_m: (Unused -- currently cell is a fixed-point model)
```

### Comparing `ngclearn-1.1b1/ngclearn/components/neurons/graded/laplacianErrorCell.py` & `ngclearn-1.1b2/ngclearn/components/neurons/graded/laplacianErrorCell.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,22 @@
     return dmu, dtarg, L
 
 class LaplacianErrorCell(Component): ## Rate-coded/real-valued error unit/cell
     """
     A simple (non-spiking) Laplacian error cell - this is a fixed-point solution
     of a mismatch/error signal.
 
+    | --- Cell Compartments: ---
+    | mu - predicted value (takes in external signals)
+    | target - desired/goal value (takes in external signals)
+    | L - local loss function embodied by this cell
+    | dmu - derivative of L w.r.t. mu
+    | dtarget - derivative of L w.r.t. target
+    | modulator - modulation signal (takes in optional external signals)
+
     Args:
         name: the string name of this cell
 
         n_units: number of cellular entities (neural population size)
 
         tau_m: (Unused -- currently cell is a fixed-point model)
```

### Comparing `ngclearn-1.1b1/ngclearn/components/neurons/graded/rateCell.py` & `ngclearn-1.1b2/ngclearn/components/neurons/graded/rateCell.py`

 * *Files 9% similar despite different names*

```diff
@@ -92,14 +92,28 @@
     return j + 0
 
 class RateCell(Component): ## Rate-coded/real-valued cell
     """
     A non-spiking cell driven by the gradient dynamics of neural generative
     coding-driven predictive processing.
 
+    The specific differential equation that characterizes this cell
+    is (for adjusting v, given current j, over time) is:
+
+    | tau_m * dz/dt = lambda * prior(z) + (j + j_td)
+    | where j is the set of general incoming input signals (e.g., message-passed signals)
+    | and j_td is taken to be the set of top-down pressure signals
+
+    | --- Cell Compartments: ---
+    | j - input (takes in external signals)
+    | j_td - input/top-down pressure input (takes in external signals)
+    | z - rate activity
+    | zF - post-activation function activity, i.e., fx(z)
+    | key - JAX RNG key
+
     Args:
         name: the string name of this cell
 
         n_units: number of cellular entities (neural population size)
 
         tau_m: membrane/state time constant (milliseconds)
 
@@ -151,18 +165,18 @@
 
         ##Layer Size Setup
         self.n_units = n_units
         self.batch_size = 1
         self.fx, self.dfx = create_function(fun_name=act_fx)
 
         # compartments (state of the cell, parameters, will be updated through stateless calls)
-        self.j = Compartment(jnp.zeros((1, n_units))) # electrical current
-        self.zF = Compartment(jnp.zeros((1, n_units))) # rate-coded output - activity
-        self.j_td = Compartment(jnp.zeros((1, n_units))) # top-down electrical current - pressure
-        self.z = Compartment(jnp.zeros((1, n_units))) # rate activity
+        self.j = Compartment(jnp.zeros((self.batch_size, n_units))) # electrical current
+        self.zF = Compartment(jnp.zeros((self.batch_size, n_units))) # rate-coded output - activity
+        self.j_td = Compartment(jnp.zeros((self.batch_size, n_units))) # top-down electrical current - pressure
+        self.z = Compartment(jnp.zeros((self.batch_size, n_units))) # rate activity
         self.key = Compartment(random.PRNGKey(time.time_ns()) if key is None else key)
 
     @staticmethod
     def _advance_state(t, dt, fx, dfx, tau_m, priorLeakRate, intgFlag, priorType,
                        thresholdType, thr_lmbda, j, j_td, z, zF):
         if tau_m > 0.:
             ### run a step of integration over neuronal dynamics
@@ -172,19 +186,19 @@
             dfx_val = dfx(z)
             j = modulate(j, dfx_val)
             tmp_z = run_cell(dt, j, j_td, z,
                          tau_m, leak_gamma=priorLeakRate,
                          integType=intgFlag, priorType=priorType)
             ## apply optional thresholding sub-dynamics
             if thresholdType == "soft_threshold":
-                tmp_z = threshold_soft(z, thr_lmbda)
+                tmp_z = threshold_soft(tmp_z, thr_lmbda)
             elif thresholdType == "cauchy_threshold":
-                tmp_z = threshold_cauchy(z, thr_lmbda)
-            z = tmp_z
-            zF = fx(z)
+                tmp_z = threshold_cauchy(tmp_z, thr_lmbda)
+            z = tmp_z ## pre-activation function value(s)
+            zF = fx(z) ## post-activation function value(s)
         else:
             ## run in "stateless" mode (when no membrane time constant provided)
             z = run_cell_stateless(j)
             zF = fx(z)
         return j, j_td, z, zF
 
     @resolver(_advance_state)
```

### Comparing `ngclearn-1.1b1/ngclearn/components/neurons/spiking/LIFCell.py` & `ngclearn-1.1b2/ngclearn/components/neurons/spiking/LIFCell.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     dv_dt = _dfv_internal(j, v, rfr, tau_m, refract_T, v_rest, v_decay)
     return dv_dt
 
 @partial(jit, static_argnums=[7,8,9,10,11])
 def run_cell(dt, j, v, v_thr, v_theta, rfr, skey, tau_m, v_rest, v_reset,
              v_decay, refract_T, integType=0):
     """
-    Runs leaky integrator neuronal dynamics
+    Runs leaky integrator (or leaky integrate-and-fire; LIF) neuronal dynamics.
 
     Args:
         dt: integration time constant (milliseconds, or ms)
 
         j: electrical current value
 
         v: membrane potential (voltage, in milliVolts or mV) value (at t)
@@ -138,19 +138,30 @@
     #_V_theta = V_theta + -V_theta * (dt/tau_theta) + S * alpha
     return _v_theta
 
 class LIFCell(Component): ## leaky integrate-and-fire cell
     """
     A spiking cell based on leaky integrate-and-fire (LIF) neuronal dynamics.
 
-    The specific differential equation that characterize this cell
+    The specific differential equation that characterizes this cell
     is (for adjusting v, given current j, over time) is:
 
     | tau_m * dv/dt = (v_rest - v) + j * R
     | where R is the membrane resistance and v_rest is the resting potential
+    | also, if a spike occurs, v is set to v_reset
+
+    | --- Cell Compartments: ---
+    | j - electrical current input (takes in external signals)
+    | v - membrane potential/voltage state
+    | s - emitted binary spikes/action potentials
+    | s_raw - raw spike signals before post-processing (only if one_spike = True, else s_raw = s)
+    | rfr - (relative) refractory variable state
+    | thr_theta - homeostatic/adaptive threshold increment state
+    | tols - time-of-last-spike
+    | key - JAX RNG key
 
     Args:
         name: the string name of this cell
 
         n_units: number of cellular entities (neural population size)
 
         tau_m: membrane time constant
```

### Comparing `ngclearn-1.1b1/ngclearn/components/neurons/spiking/WTASCell.py` & `ngclearn-1.1b2/ngclearn/components/neurons/spiking/WTASCell.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,22 @@
 
     The differential equation for adjusting this specific cell
     (for adjusting v, given current j, over time) is:
 
     | tau_m * dv/dt = j * R  ;  v_p = softmax(v)
     | where R is membrane resistance and v_p is a voltage probability vector
 
+    | --- Cell Compartments: ---
+    | j - electrical current input (takes in external signals)
+    | v - membrane potential/voltage state
+    | s - emitted binary spikes/action potentials
+    | rfr - (relative) refractory variable state
+    | thr - (adaptive) threshold state
+    | tols - time-of-last-spike
+
     Args:
         name: the string name of this cell
 
         n_units: number of cellular entities (neural population size)
 
         tau_m: membrane time constant
```

### Comparing `ngclearn-1.1b1/ngclearn/components/neurons/spiking/adExCell.py` & `ngclearn-1.1b2/ngclearn/components/neurons/spiking/adExCell.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,22 @@
     The specific pair of differential equations that characterize this cell
     are (for adjusting v and w, given current j, over time):
 
     | tau_m * dv/dt = -(v - v_rest) + sharpV * exp((v - vT)/sharpV) - R_m * w + R_m * j
     | tau_w * dw/dt =  -w + (v - v_rest) * a
     | where w = w + s * (w + b) [in the event of a spike]
 
+    | --- Cell Compartments: ---
+    | j - electrical current input (takes in external signals)
+    | v - membrane potential/voltage state
+    | w - recovery variable state
+    | s - emitted binary spikes/action potentials
+    | tols - time-of-last-spike
+    | key - JAX RNG key
+
 
     | References:
     | Brette, Romain, and Wulfram Gerstner. "Adaptive exponential integrate-and-fire
     | model as an effective description of neuronal activity." Journal of
     | neurophysiology 94.5 (2005): 3637-3642.
 
     Args:
```

### Comparing `ngclearn-1.1b1/ngclearn/components/neurons/spiking/fitzhughNagumoCell.py` & `ngclearn-1.1b2/ngclearn/components/neurons/spiking/fitzhughNagumoCell.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,22 @@
 
     The specific pair of differential equations that characterize this cell
     are (for adjusting v and w, given current j, over time):
 
     | tau_m * dv/dt = v - (v^3)/3 - w + j
     | tau_w * dw/dt = v + a - b * w
 
+    | --- Cell Compartments: ---
+    | j - electrical current input (takes in external signals)
+    | v - membrane potential/voltage state
+    | w - recovery variable state
+    | s - emitted binary spikes/action potentials
+    | tols - time-of-last-spike
+    | key - JAX RNG key
+
     | References:
     | FitzHugh, Richard. "Impulses and physiological states in theoretical
     | models of nerve membrane." Biophysical journal 1.6 (1961): 445-466.
     |
     | Nagumo, Jinichi, Suguru Arimoto, and Shuji Yoshizawa. "An active pulse
     | transmission line simulating nerve axon." Proceedings of the IRE 50.10
     | (1962): 2061-2070.
```

### Comparing `ngclearn-1.1b1/ngclearn/components/neurons/spiking/izhikevichCell.py` & `ngclearn-1.1b2/ngclearn/components/neurons/spiking/izhikevichCell.py`

 * *Files 7% similar despite different names*

```diff
@@ -134,14 +134,22 @@
 
     The specific pair of differential equations that characterize this cell
     are (for adjusting v and w, given current j, over time):
 
     | tau_m * dv/dt = 0.04 v^2 + 5v + 140 - w + j * R_m
     | tau_w * dw/dt = (v * b - w),  where tau_w = 1/a
 
+    | --- Cell Compartments: ---
+    | j - electrical current input (takes in external signals)
+    | v - membrane potential/voltage state
+    | w - recovery variable state
+    | s - emitted binary spikes/action potentials
+    | tols - time-of-last-spike
+    | key - JAX RNG key
+
     | References:
     | Izhikevich, Eugene M. "Simple model of spiking neurons." IEEE Transactions
     | on neural networks 14.6 (2003): 1569-1572.
 
     Note: Izhikevich's constants/hyper-parameters 'a', 'b', 'c', and 'd' have
     been remapped/renamed (see arguments below). Note that the default settings
     for this component cell is for a regular spiking cell; to recover other
```

### Comparing `ngclearn-1.1b1/ngclearn/components/neurons/spiking/quadLIFCell.py` & `ngclearn-1.1b2/ngclearn/components/neurons/spiking/quadLIFCell.py`

 * *Files 11% similar despite different names*

```diff
@@ -151,14 +151,24 @@
     | d.Vz/d.t = a0 * (V - V_rest) * (V - V_c) + Jz * R) * (dt/tau_mem)
 
     where:
 
     |   a0 - scaling factor for voltage accumulation
     |   V_c - critical voltage (value)
 
+    | --- Cell Compartments: ---
+    | j - electrical current input (takes in external signals)
+    | v - membrane potential/voltage state
+    | s - emitted binary spikes/action potentials
+    | s_raw - raw spike signals before post-processing (only if one_spike = True, else s_raw = s)
+    | rfr - (relative) refractory variable state
+    | thr_theta - homeostatic/adaptive threshold increment state
+    | tols - time-of-last-spike
+    | key - JAX RNG key
+
     Args:
         name: the string name of this cell
 
         n_units: number of cellular entities (neural population size)
 
         tau_m: membrane time constant
```

### Comparing `ngclearn-1.1b1/ngclearn/components/neurons/spiking/sLIFCell.py` & `ngclearn-1.1b2/ngclearn/components/neurons/spiking/sLIFCell.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,24 @@
     A spiking cell based on a simplified leaky integrate-and-fire (sLIF) model.
     This neuronal cell notably contains functionality required by the computational
     model employed by (Samadi et al., 2017, i.e., a surrogate derivative function
     and "sticky spikes") as well as the additional incorporation of an adaptive
     threshold (per unit) scheme. (Note that this particular spiking cell only
     supports Euler integration of its voltage dynamics.)
 
+    | --- Cell Compartments: ---
+    | j - electrical current input (takes in external signals)
+    | v - membrane potential/voltage state
+    | s - emitted binary spikes/action potentials
+    | rfr - (relative) refractory variable state
+    | thr - (adaptive) threshold state
+    | surrogate - state of surrogate function output signals (currently, the secant LIF estimator)
+    | tols - time-of-last-spike
+    | key - JAX RNG key
+
     | Reference:
     | Samadi, Arash, Timothy P. Lillicrap, and Douglas B. Tweed. "Deep learning with
     | dynamic spiking neurons and fixed feedback weights." Neural computation 29.3
     | (2017): 578-602.
 
     Args:
         name: the string name of this cell
```

### Comparing `ngclearn-1.1b1/ngclearn/components/other/expKernel.py` & `ngclearn-1.1b2/ngclearn/components/other/expKernel.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,19 @@
     return tf, epsp
 
 class ExpKernel(Component): ## exponential kernel
     """
     A spiking function based on an exponential kernel applied to
     a moving window of spike times.
 
+    | --- Cell Compartments: ---
+    | inputs - input (takes in external signals)
+    | epsp - excitatory postsynaptic potential/pulse
+    | tf - maintained local window of pulse signals
+
     Args:
         name: the string name of this operator
 
         n_units: number of calculating entities or units
 
         dt: integration time constant (the kernel needs access to this value)
```

### Comparing `ngclearn-1.1b1/ngclearn/components/other/varTrace.py` & `ngclearn-1.1b2/ngclearn/components/other/varTrace.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,19 @@
         #_x_tr = ( x_tr + (-x_tr) * (dt / tau_tr) ) * (1. - x) + x
     return _x_tr
 
 class VarTrace(Component): ## low-pass filter
     """
     A variable trace (filter) functional node.
 
+    | --- Cell Compartments: ---
+    | inputs - input (takes in external signals)
+    | outputs - output signal (same as "trace" compartment)
+    | trace - traced value signal
+
     Args:
         name: the string name of this operator
 
         n_units: number of calculating entities or units
 
         tau_tr: trace time constant (in milliseconds, or ms)
```

### Comparing `ngclearn-1.1b1/ngclearn/components/synapses/hebbian/eventSTDPSynapse.py` & `ngclearn-1.1b2/ngclearn/components/synapses/hebbian/eventSTDPSynapse.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,25 @@
     return jnp.matmul(inp, weight * scale)
 
 class EventSTDPSynapse(Component): # event-driven, post-synaptic STDP
     """
     A synaptic cable that adjusts its efficacies via event-driven, post-synaptic
     spike-timing-dependent plasticity (STDP).
 
+    | --- Synapse Compartments: ---
+    | inputs - input (takes in external signals)
+    | outputs - output signal (transformation induced by synapses)
+    | weights - current value matrix of synaptic efficacies
+    | --- Synaptic Plasticity Compartments: ---
+    | preSpike - pre-synaptic spike to drive 1st term of STDP update
+    | postSpike - post-synaptic spike to drive 2nd term of STDP update
+    | preTrace - pre-synaptic trace value to drive 1st term of STDP update
+    | postTrace - post-synaptic trace value to drive 2nd term of STDP update
+    | dWeights - current delta matrix containing changes to be applied to synaptic efficacies
+
     | References:
     | Tavanaei, Amirhossein, Timothée Masquelier, and Anthony Maida.
     | "Representation learning using event-based STDP." Neural Networks 105
     | (2018): 294-303.
 
     Args:
         name: the string name of this cell
```

### Comparing `ngclearn-1.1b1/ngclearn/components/synapses/hebbian/expSTDPSynapse.py` & `ngclearn-1.1b2/ngclearn/components/synapses/hebbian/expSTDPSynapse.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,14 +76,25 @@
 
 class ExpSTDPSynapse(Component):
     """
     A synaptic cable that adjusts its efficacies via trace-based form of
     spike-timing-dependent plasticity (STDP) based on an exponential weight
     dependence (the strength of which is controlled by a factor).
 
+    | --- Synapse Compartments: ---
+    | inputs - input (takes in external signals)
+    | outputs - output signal (transformation induced by synapses)
+    | weights - current value matrix of synaptic efficacies
+    | --- Synaptic Plasticity Compartments: ---
+    | preSpike - pre-synaptic spike to drive 1st term of STDP update
+    | postSpike - post-synaptic spike to drive 2nd term of STDP update
+    | preTrace - pre-synaptic trace value to drive 1st term of STDP update
+    | postTrace - post-synaptic trace value to drive 2nd term of STDP update
+    | dWeights - current delta matrix containing changes to be applied to synaptic efficacies
+
     | References:
     | Nessler, Bernhard, et al. "Bayesian computation emerges in generic cortical
     | microcircuits through spike-timing-dependent plasticity." PLoS computational
     | biology 9.4 (2013): e1003037.
     |
     | Bi, Guo-qiang, and Mu-ming Poo. "Synaptic modification by correlated
     | activity: Hebb's postulate revisited." Annual review of neuroscience 24.1
```

### Comparing `ngclearn-1.1b1/ngclearn/components/synapses/hebbian/hebbianSynapse.py` & `ngclearn-1.1b2/ngclearn/components/synapses/hebbian/hebbianSynapse.py`

 * *Files 10% similar despite different names*

```diff
@@ -91,14 +91,26 @@
     return jnp.matmul(inp, weight * Rscale) + biases
 
 class HebbianSynapse(Component):
     """
     A synaptic cable that adjusts its efficacies via a two-factor Hebbian
     adjustment rule.
 
+    | --- Synapse Compartments: ---
+    | inputs - input (takes in external signals)
+    | outputs - output signal (transformation induced by synapses)
+    | weights - current value matrix of synaptic efficacies
+    | biases - current value vector of synaptic bias values
+    | --- Synaptic Plasticity Compartments: ---
+    | pre - pre-synaptic signal to drive first term of Hebbian update
+    | post - post-synaptic signal to drive 2nd term of Hebbian update
+    | dW - current delta matrix containing changes to be applied to synaptic efficacies
+    | db - current delta vector containing changes to be applied to bias value
+    | opt_params - locally-embedded optimizer statisticis (e.g., Adam 1st/2nd moments if adam is used)
+
     Args:
         name: the string name of this cell
 
         shape: tuple specifying shape of this synaptic cable (usually a 2-tuple
             with number of inputs by number of outputs)
 
         eta: global learning rate
```

### Comparing `ngclearn-1.1b1/ngclearn/components/synapses/hebbian/traceSTDPSynapse.py` & `ngclearn-1.1b2/ngclearn/components/synapses/hebbian/traceSTDPSynapse.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,25 @@
 class TraceSTDPSynapse(Component): # power-law / trace-based STDP
     """
     A synaptic cable that adjusts its efficacies via trace-based form of
     spike-timing-dependent plasticity (STDP), including an optional power-scale
     dependence that can be equipped to the Hebbian adjustment (the strength of
     which is controlled by a scalar factor).
 
+    | --- Synapse Compartments: ---
+    | inputs - input (takes in external signals)
+    | outputs - output signal (transformation induced by synapses)
+    | weights - current value matrix of synaptic efficacies
+    | --- Synaptic Plasticity Compartments: ---
+    | preSpike - pre-synaptic spike to drive 1st term of STDP update
+    | postSpike - post-synaptic spike to drive 2nd term of STDP update
+    | preTrace - pre-synaptic trace value to drive 1st term of STDP update
+    | postTrace - post-synaptic trace value to drive 2nd term of STDP update
+    | dWeights - current delta matrix containing changes to be applied to synaptic efficacies
+
     | References:
     | Morrison, Abigail, Ad Aertsen, and Markus Diesmann. "Spike-timing-dependent
     | plasticity in balanced random networks." Neural computation 19.6 (2007): 1437-1467.
     |
     | Bi, Guo-qiang, and Mu-ming Poo. "Synaptic modification by correlated
     | activity: Hebb's postulate revisited." Annual review of neuroscience 24.1
     | (2001): 139-166.
```

### Comparing `ngclearn-1.1b1/ngclearn/components/synapses/staticSynapse.py` & `ngclearn-1.1b2/ngclearn/components/synapses/staticSynapse.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,19 @@
     return jnp.matmul(inp, weight * scale)
 
 class StaticSynapse(Component): ## static non-learnable synaptic cable
     """
     A static (dense) synaptic cable; no form of synaptic evolution/adaptation
     is in-built to this component.
 
+    | --- Synapse Compartments: ---
+    | inputs - input (takes in external signals)
+    | outputs - output
+    | weights - current value matrix of synaptic efficacies
+
     Args:
         name: the string name of this cell
 
         shape: tuple specifying shape of this synaptic cable (usually a 2-tuple
             with number of inputs by number of outputs)
 
         wInit: a kernel to drive initialization of this synaptic cable's values;
```

### Comparing `ngclearn-1.1b1/ngclearn/utils/data_loader.py` & `ngclearn-1.1b2/ngclearn/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn/utils/density/gmm.py` & `ngclearn-1.1b2/ngclearn/utils/density/gmm.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn/utils/diffeq/ode_utils.py` & `ngclearn-1.1b2/ngclearn/utils/diffeq/ode_utils.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn/utils/io_utils.py` & `ngclearn-1.1b2/ngclearn/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn/utils/metric_utils.py` & `ngclearn-1.1b2/ngclearn/utils/metric_utils.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn/utils/model_utils.py` & `ngclearn-1.1b2/ngclearn/utils/model_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,15 @@
         initKernel: triplet/3-tuple with 1st element as a string calling the name
             of initialization scheme to use
 
             :Note: Currently supported kernel schemes include:
                 ("hollow", off_diagonal_scale, ~ignored~);
                 ("eye", diagonal_scale, ~ignored~);
                 ("uniform", min_val, max_val);
+                ("fan_in_gaussian", ~ignored, ~ignored~);
                 ("gaussian", mu, sigma) OR ("normal", mu, sigma);
                 ("constant", magnitude, ~ignored~)
 
         shape: tuple containing the dimensions/shape of the tensor to initialize
 
     Returns:
         output (tensor) value
@@ -138,14 +139,18 @@
         params = (1. - jnp.eye(N=shape[0], M=shape[1])) * eyeScale
     elif initType == "eye":
         eyeScale, _ = args
         params = jnp.eye(N=shape[0], M=shape[1]) * eyeScale
     elif initType == "uniform": ## uniformly distributed values
         lb, ub = args
         params = random.uniform(dkey, shape, minval=lb, maxval=ub)
+    elif initType == "fan_in_gaussian":
+        Phi = random.normal(dkey, shape)
+        Phi = Phi * jnp.sqrt(1.0 / (shape[0] * 1.))
+        params = Phi.astype(jnp.float32)
     elif initType == "gaussian" or initType == "normal": ## gaussian distributed values
         mu, sigma = args
         params = random.normal(dkey, shape) * sigma + mu
     elif initType == "constant": ## constant value(s)
         scale, _ = args
         params = jnp.ones(shape) * scale
     else:
@@ -169,17 +174,17 @@
 
         axis: 0 (apply to column vectors), 1 (apply to row vectors)
 
     Returns:
         a normalized value matrix
     """
     if order == 2: ## denominator is L2 norm
-        wOrdSum = jnp.square(jnp.sum(jnp.square(M), axis=axis, keepdims=True))
+        wOrdSum = jnp.maximum(jnp.sum(jnp.square(M), axis=axis, keepdims=True), 1e-8)
     else: ## denominator is L1 norm
-        wOrdSum = jnp.sum(jnp.abs(M), axis=axis, keepdims=True)
+        wOrdSum = jnp.maximum(jnp.sum(jnp.abs(M), axis=axis, keepdims=True), 1e-8)
     m = (wOrdSum == 0.).astype(dtype=jnp.float32)
     wOrdSum = wOrdSum * (1. - m) + m #wAbsSum[wAbsSum == 0.] = 1.
     _M = M * (wnorm/wOrdSum)
     return _M
 
 @jit
 def clamp_min(x, min_val):
@@ -494,14 +499,15 @@
     """
     if tau > 0.0:
         x = x / tau
     max_x = jnp.max(x, axis=1, keepdims=True)
     exp_x = jnp.exp(x - max_x)
     return exp_x / jnp.sum(exp_x, axis=1, keepdims=True)
 
+@jit
 def threshold_soft(x, lmbda):
     """
     A soft threshold routine applied to each dimension of input
 
     Args:
         x: data to apply threshold function over
 
@@ -510,14 +516,15 @@
     Returns:
         thresholded x
     """
     # soft thresholding fx - S(x) = (|x| - lmbda) *@ sign(x)
     ## legacy ngclearn: tf.math.maximum(x - lmbda, 0.) - tf.math.maximum(-x - lmbda, 0.)
     return jnp.maximum(x - lmbda, 0.) - jnp.maximum(-x - lmbda, 0.)
 
+@jit
 def threshold_cauchy(x, lmbda):
     """
     A Cauchy distributional threshold routine applied to each dimension of input
 
     Args:
         x: data to apply threshold function over
```

### Comparing `ngclearn-1.1b1/ngclearn/utils/optim/adam.py` & `ngclearn-1.1b2/ngclearn/utils/optim/adam.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn/utils/optim/sgd.py` & `ngclearn-1.1b2/ngclearn/utils/optim/sgd.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn/utils/patch_utils.py` & `ngclearn-1.1b2/ngclearn/utils/patch_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,16 @@
         xs = xs.reshape(px, py)
         patches = extract_patches_2d(xs, patch_size, max_patches=max_patches)#, random_state=69)
         patches = np.reshape(patches, (len(patches), -1)) # flatten each patch in set
         if s > 0:
             p_batch = np.concatenate((p_batch,patches),axis=0)
         else:
             p_batch = patches
-    if center == True:
-        mu = np.mean(p_batch,axis=1,keepdims=True)
+    if center: ## center patches by subtracting out their means
+        mu = np.mean(p_batch, axis=1, keepdims=True)
         p_batch = p_batch - mu
     return jnp.array(p_batch)
 
 def generate_pacthify_patch_set(x_batch_, patch_size=(5, 5), center=True): ## patchify
     ## this is a patchify-specific function (only use if you have patchify installed...)
     import patchify as ptch
     """
```

### Comparing `ngclearn-1.1b1/ngclearn/utils/surrogate_fx.py` & `ngclearn-1.1b2/ngclearn/utils/surrogate_fx.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn/utils/viz/dim_reduce.py` & `ngclearn-1.1b2/ngclearn/utils/viz/dim_reduce.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn/utils/viz/raster.py` & `ngclearn-1.1b2/ngclearn/utils/viz/raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 import matplotlib.pyplot as plt
 from matplotlib import gridspec
 import numpy as np
 import imageio.v3 as iio
 import jax.numpy as jnp
 
 def create_raster_plot(spike_train, ax=None, s=0.5, c="black",
-                       plot_fname=None, indices=None, tag="", suffix='.jpg'):
+                       plot_fname=None, indices=None, tag="", suffix='.jpg', 
+                       title_font_size=20):
     """
     Generates a raster plot of a given (binary) spike train (row dimension
     corresponds to the discrete time dimension).
 
     Args:
         spike_train: a numpy binary array of shape (number_neurons x 1 x T) OR
             shape (number_neurons x T)
@@ -48,15 +49,15 @@
     if ax is None:
         if plot_fname is None:
             plot_fname = "raster_plot" + suffix
 
         nc = n_count if indices is None else len(indices)
         fig_size = 5 if nc < 25 else int(nc / 5)
         plt.figure(figsize=(fig_size, fig_size)) # (fig_size * K, fig_size)
-        plt.title("Spike Train Raster Plot, {}".format(tag))
+        plt.title("Spike Train Raster Plot, {}".format(tag), fontsize=title_font_size)
         plt.xlabel("Time Step")
         # plt.ylabel("Neuron Index")
         save = True
 
     ax = ax if ax is not None else plt
 
     events = []
```

### Comparing `ngclearn-1.1b1/ngclearn/utils/viz/spike_plot.py` & `ngclearn-1.1b2/ngclearn/utils/viz/spike_plot.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn/utils/viz/synapse_plot.py` & `ngclearn-1.1b2/ngclearn/utils/viz/synapse_plot.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/ngclearn.egg-info/PKG-INFO` & `ngclearn-1.1b2/ngclearn.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngclearn
-Version: 1.1b1
+Version: 1.1b2
 Summary: Simulation software for building and analyzing arbitrary predictive coding, spiking network, and biomimetic neural systems.
 Author-email: Alexander Ororbia <ago@cs.rit.edu>, William Gebhardt <wdg1351@rit.edu>
 License: BSD-3-Clause License
 Project-URL: Homepage, https://github.com/NACLab/ngc-learn
 Project-URL: Documentation, https://ngc-learn.readthedocs.io/
 Project-URL: Lab Page, https://www.cs.rit.edu/~ago/nac_lab.html
 Project-URL: Changelog, https://github.com/NACLab/ngc-learn/blob/main/history.txt
@@ -80,15 +80,15 @@
 5) scikit-learn (>=1.3.1) if using `ngclearn.utils.density`
 6) matplotlib (>=3.4.3) if using `ngclearn.utils.viz`
 6) networkx  (>=2.6.3) (currently optional but required if using `ngclearn.utils.experimental.viz_utils`)
 7) pyviz (>=0.2.0) (currently optional but required if using `ngclearn.utils.experimental.viz_utils`)
 -->
 
 ---
-ngc-learn 1.0.beta0 and later require Python 3.10 or newer as well as ngcsimlib >=0.2.b2.
+ngc-learn 1.1.beta2 and later require Python 3.10 or newer as well as ngcsimlib >=0.3.b1.
 ngc-learn's plotting capabilities (routines within `ngclearn.utils.viz`) require
 Matplotlib (>=3.8.0) and imageio (>=2.31.5) and both plotting and density estimation
 tools (routines within ``ngclearn.utils.density``) will require Scikit-learn (>=0.24.2).
 Many of the tutorials will require Matplotlib (>=3.8.0), imageio (>=2.31.5), and Scikit-learn (>=0.24.2).
 <!-- (Note: if using the `_generate_patch_set()` within the
 image patching utilities, then Patchify will be needed).-->
 
@@ -115,15 +115,15 @@
 right major and minor version of ngc-learn):
 
 ```console
 Python 3.11.4 (main, MONTH  DAY YEAR, TIME) [GCC XX.X.X] on linux
 Type "help", "copyright", "credits" or "license" for more information.
 >>> import ngclearn
 >>> ngclearn.__version__
-'1.0b3'
+'1.1b2'
 ```
 
 <i>Note:</i> For access to the previous Tensorflow-2 version of ngc-learn (of
 which we no longer support), please visit the repo for
 <a href="https://github.com/NACLab/ngc-learn-legacy"><i>ngc-learn-legacy</i></a>.
 
 ## <b>Attribution:</b>
@@ -162,15 +162,15 @@
 If you are working on and developing with ngc-learn pulled from the github
 repo, then run the following command to set up an editable install:
 <pre>
 $ python install -e .
 </pre>
 
 **Version:**<br>
-1.1.1-Beta <!-- -Alpha -->
+1.1.2-Beta <!-- -Alpha -->
 
 Author:
 Alexander G. Ororbia II<br>
 Director, Neural Adaptive Computing (NAC) Laboratory<br>
 Rochester Institute of Technology, Department of Computer Science
 
 ## <b>Copyright:</b>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ngclearn Version: 1.1b1 Summary: Simulation
+Metadata-Version: 2.1 Name: ngclearn Version: 1.1b2 Summary: Simulation
 software for building and analyzing arbitrary predictive coding, spiking
 network, and biomimetic neural systems. Author-email: Alexander Ororbia
 cs.rit.edu>, William Gebhardt
 rit.edu> License: BSD-3-Clause License Project-URL: Homepage, https://
 github.com/NACLab/ngc-learn Project-URL: Documentation, https://ngc-
 learn.readthedocs.io/ Project-URL: Lab Page, https://www.cs.rit.edu/~ago/
 nac_lab.html Project-URL: Changelog, https://github.com/NACLab/ngc-learn/blob/
@@ -42,16 +42,16 @@
 library can be found _h_e_r_e.
 You can find the related paper _r_i_g_h_t_ _h_e_r_e, which was selected to appear in the
 Nature Neuromorphic Hardware and Computing Collection in 2023 and was chosen as
 one of the Editors' Highlights for Applied Physics and Mathematics in 2022. ##
 Installation ### Dependencies ngc-learn requires: 1) Python (>=3.10) 2) NumPy
 (>=1.26.0) 3) SciPy (>=1.7.0) 4) ngcsimlib (>=0.2.b1), (visit official page
 _h_e_r_e) 5) JAX (>= 0.4.18) (to enable GPU use, make sure to install one of the
-CUDA variants) --- ngc-learn 1.0.beta0 and later require Python 3.10 or newer
-as well as ngcsimlib >=0.2.b2. ngc-learn's plotting capabilities (routines
+CUDA variants) --- ngc-learn 1.1.beta2 and later require Python 3.10 or newer
+as well as ngcsimlib >=0.3.b1. ngc-learn's plotting capabilities (routines
 within `ngclearn.utils.viz`) require Matplotlib (>=3.8.0) and imageio
 (>=2.31.5) and both plotting and density estimation tools (routines within
 ``ngclearn.utils.density``) will require Scikit-learn (>=0.24.2). Many of the
 tutorials will require Matplotlib (>=3.8.0), imageio (>=2.31.5), and Scikit-
 learn (>=0.24.2). ### User Installation Setup: The easiest way to install ngc-
 learn is through pip:
 $ pip install ngclearn
@@ -63,15 +63,15 @@
 library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and 20.04.
 If the installation was successful, you should see the following if you test it
 against your Python interpreter, i.e., run the $ python command and complete
 the following sequence of steps as depicted in the screenshot below (you should
 see at the bottom of your output something akin to the right major and minor
 version of ngc-learn): ```console Python 3.11.4 (main, MONTH DAY YEAR, TIME)
 [GCC XX.X.X] on linux Type "help", "copyright", "credits" or "license" for more
-information. >>> import ngclearn >>> ngclearn.__version__ '1.0b3' ``` Note: For
+information. >>> import ngclearn >>> ngclearn.__version__ '1.1b2' ``` Note: For
 access to the previous Tensorflow-2 version of ngc-learn (of which we no longer
 support), please visit the repo for _n_g_c_-_l_e_a_r_n_-_l_e_g_a_c_y. ## AAttttrriibbuuttiioonn:: If you
 use this code in any form in your project(s), please cite its source paper (as
 well as ngc-learn's official software citation):
 @article{Ororbia2022,
   author={Ororbia, Alexander and Kifer, Daniel},
   title={The neural coding framework for learning generative models},
@@ -91,15 +91,15 @@
 [contributing guidelines](CONTRIBUTING.md). SSoouurrccee CCooddee You can check/pull the
 latest source code for this library via:
 $ git clone https://github.com/NACLab/ngc-learn.git
 If you are working on and developing with ngc-learn pulled from the github
 repo, then run the following command to set up an editable install:
 $ python install -e .
 **Version:**
-1.1.1-Beta Author: Alexander G. Ororbia II
+1.1.2-Beta Author: Alexander G. Ororbia II
 Director, Neural Adaptive Computing (NAC) Laboratory
 Rochester Institute of Technology, Department of Computer Science ## CCooppyyrriigghhtt::
 Copyright (C) 2021 The Neural Adaptive Computing Laboratory - All Rights
 Reserved
 You may use, distribute and modify this code under the terms of the BSD 3-
 clause license. You should have received a copy of the BSD 3-clause license
 with this software.
```

### Comparing `ngclearn-1.1b1/ngclearn.egg-info/SOURCES.txt` & `ngclearn-1.1b2/ngclearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/pyproject.toml` & `ngclearn-1.1b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ngclearn"
-version = "1.1.beta1"
+version = "1.1.beta2" 
 description = "Simulation software for building and analyzing arbitrary predictive coding, spiking network, and biomimetic neural systems."
 authors = [
   {name = "Alexander Ororbia", email = "ago@cs.rit.edu"},
   {name = "William Gebhardt", email = "wdg1351@rit.edu"},
 ]
 readme = "README.md"
 keywords = ['python', 'ngc-learn', 'predictive-processing', 'predictive-coding',
             'jax', 'spiking-neural-networks', 'biomimetics', 'bionics', 'computational-neuroscience']
-requires-python = ">=3.8" # 3.10
+requires-python = ">=3.8" #3.10
 license = {text = "BSD-3-Clause License"}
 classifiers=[
   "Development Status :: 4 - Beta", #3 - Alpha", # 5 - Production/Stable
   "Intended Audience :: Education",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
```

### Comparing `ngclearn-1.1b1/test_code/_run_trstdp.py` & `ngclearn-1.1b2/test_code/_run_trstdp.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/test_code/adex.py` & `ngclearn-1.1b2/test_code/adex.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/test_code/calc_fanoFactor.py` & `ngclearn-1.1b2/test_code/calc_fanoFactor.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/test_code/run2_metrics.py` & `ngclearn-1.1b2/test_code/run2_metrics.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/test_code/run_expkernel.py` & `ngclearn-1.1b2/test_code/run_expkernel.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/test_code/run_metrics.py` & `ngclearn-1.1b2/test_code/run_metrics.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/test_code/run_trace.py` & `ngclearn-1.1b2/test_code/run_trace.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/test_code/run_trstdp.py` & `ngclearn-1.1b2/test_code/run_trstdp.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/test_code/test_adex.py` & `ngclearn-1.1b2/test_code/test_adex.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/test_code/test_fhcell.py` & `ngclearn-1.1b2/test_code/test_fhcell.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/test_code/test_izhcell.py` & `ngclearn-1.1b2/test_code/test_izhcell.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/test_code/viz_data.py` & `ngclearn-1.1b2/test_code/viz_data.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.1b1/test_lava/run_xotSNN.py` & `ngclearn-1.1b2/test_lava/run_xotSNN.py`

 * *Files identical despite different names*

