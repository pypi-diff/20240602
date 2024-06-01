# Comparing `tmp/pyscf-2.5.0.tar.gz` & `tmp/pyscf-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscf-2.5.0.tar", last modified: Mon Feb  5 22:40:40 2024, max compression
+gzip compressed data, was "pyscf-2.6.0.tar", last modified: Sat Jun  1 22:08:54 2024, max compression
```

## Comparing `pyscf-2.5.0.tar` & `pyscf-2.6.0.tar`

### file list

```diff
@@ -1,1067 +1,1114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.187690 pyscf-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    52243 2024-02-05 22:40:38.000000 pyscf-2.5.0/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-05 22:40:38.000000 pyscf-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-02-05 22:40:38.000000 pyscf-2.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-02-05 22:40:38.000000 pyscf-2.5.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-02-05 22:40:40.187690 pyscf-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-02-05 22:40:38.000000 pyscf-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.015693 pyscf-2.5.0/pyscf/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/__all__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/__config__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.019693 pyscf-2.5.0/pyscf/adc/
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/adc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/adc/dfadc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15076 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/adc/radc.py
--rw-r--r--   0 runner    (1001) docker     (127)    29868 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/adc/radc_amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/adc/radc_ao2mo.py
--rw-r--r--   0 runner    (1001) docker     (127)    43387 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/adc/radc_ea.py
--rw-r--r--   0 runner    (1001) docker     (127)    38433 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/adc/radc_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)    44715 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/adc/radc_ip_cvs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15399 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/adc/uadc.py
--rw-r--r--   0 runner    (1001) docker     (127)    41215 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/adc/uadc_amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (127)    22683 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/adc/uadc_ao2mo.py
--rw-r--r--   0 runner    (1001) docker     (127)    89288 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/adc/uadc_ea.py
--rw-r--r--   0 runner    (1001) docker     (127)    81944 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/adc/uadc_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)   110124 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/adc/uadc_ip_cvs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.023692 pyscf-2.5.0/pyscf/agf2/
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/agf2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18199 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/agf2/_agf2.py
--rw-r--r--   0 runner    (1001) docker     (127)    22821 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/agf2/aux_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/agf2/chempot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/agf2/chkfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/agf2/dfragf2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/agf2/dfuagf2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/agf2/mpi_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    36377 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/agf2/ragf2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/agf2/ragf2_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)    36449 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/agf2/uagf2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10447 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/agf2/uagf2_slow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.023692 pyscf-2.5.0/pyscf/ao2mo/
--rw-r--r--   0 runner    (1001) docker     (127)    20567 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/ao2mo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11212 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/ao2mo/_ao2mo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7708 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/ao2mo/addons.py
--rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/ao2mo/incore.py
--rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/ao2mo/nrr_outcore.py
--rw-r--r--   0 runner    (1001) docker     (127)    34082 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/ao2mo/outcore.py
--rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/ao2mo/r_outcore.py
--rw-r--r--   0 runner    (1001) docker     (127)    13157 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/ao2mo/semi_incore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.031692 pyscf-2.5.0/pyscf/cc/
--rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/_ccsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/addons.py
--rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/bccd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/ccd.py
--rw-r--r--   0 runner    (1001) docker     (127)    68628 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/ccsd.py
--rw-r--r--   0 runner    (1001) docker     (127)    17726 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/ccsd_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)    21249 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/ccsd_rdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/ccsd_rdm_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)    11081 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/ccsd_t.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/ccsd_t_lambda_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/ccsd_t_rdm_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/ccsd_t_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     9459 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/dfccsd.py
--rw-r--r--   0 runner    (1001) docker     (127)    25619 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/eom_gccsd.py
--rw-r--r--   0 runner    (1001) docker     (127)    81419 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/eom_rccsd.py
--rw-r--r--   0 runner    (1001) docker     (127)   117956 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/eom_uccsd.py
--rw-r--r--   0 runner    (1001) docker     (127)    22352 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/gccsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/gccsd_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)    10804 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/gccsd_rdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/gccsd_t.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/gccsd_t_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/gccsd_t_rdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/gccsd_t_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     9609 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/gintermediates.py
--rw-r--r--   0 runner    (1001) docker     (127)    28323 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/momgfccsd.py
--rw-r--r--   0 runner    (1001) docker     (127)    14466 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/qcisd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/qcisd_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/qcisd_t.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/qcisd_t_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)    16241 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/rccsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/rccsd_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)    44692 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/rccsd_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)    12025 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/rintermediates.py
--rw-r--r--   0 runner    (1001) docker     (127)    58458 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/uccsd.py
--rw-r--r--   0 runner    (1001) docker     (127)    23359 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/uccsd_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)    27641 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/uccsd_rdm.py
--rw-r--r--   0 runner    (1001) docker     (127)    29028 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/uccsd_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)    18576 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/uccsd_t.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/uccsd_t_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/uccsd_t_rdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9259 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/uccsd_t_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)    38860 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/uintermediates.py
--rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/cc/uintermediates_slow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.031692 pyscf-2.5.0/pyscf/ci/
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/ci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/ci/addons.py
--rw-r--r--   0 runner    (1001) docker     (127)    44261 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/ci/cisd.py
--rw-r--r--   0 runner    (1001) docker     (127)    18108 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/ci/gcisd.py
--rw-r--r--   0 runner    (1001) docker     (127)    38974 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/ci/ucisd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.031692 pyscf-2.5.0/pyscf/data/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37852 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/data/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/data/gyro.py
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/data/gyromagnetic_ratio.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/data/nist.py
--rw-r--r--   0 runner    (1001) docker     (127)    23505 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/data/nuclear_g_factor.dat
--rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/data/nucprop.py
--rw-r--r--   0 runner    (1001) docker     (127)    13797 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/data/radii.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/data/solvents.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.031692 pyscf-2.5.0/pyscf/df/
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/addons.py
--rw-r--r--   0 runner    (1001) docker     (127)    14154 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/df.py
--rw-r--r--   0 runner    (1001) docker     (127)    21885 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/df_jk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.035692 pyscf-2.5.0/pyscf/df/grad/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/grad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26202 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/grad/casdm2_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9507 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/grad/casscf.py
--rw-r--r--   0 runner    (1001) docker     (127)    21609 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/grad/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/grad/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/grad/rohf.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/grad/roks.py
--rw-r--r--   0 runner    (1001) docker     (127)    17452 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/grad/sacasscf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/grad/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/grad/uks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.035692 pyscf-2.5.0/pyscf/df/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22329 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/hessian/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/hessian/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)    25233 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/hessian/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/hessian/uks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/incore.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/outcore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/df/r_incore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.043692 pyscf-2.5.0/pyscf/dft/
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/dks.py
--rw-r--r--   0 runner    (1001) docker     (127)    24925 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/gen_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/gen_libxc_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/gen_xcfun_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/gks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/gks_symm.py
--rw-r--r--   0 runner    (1001) docker     (127)   122275 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/libxc.py
--rw-r--r--   0 runner    (1001) docker     (127)   119578 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/numint.py
--rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/numint2c.py
--rw-r--r--   0 runner    (1001) docker     (127)    29777 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/r_numint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/radi.py
--rw-r--r--   0 runner    (1001) docker     (127)    19135 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/rks_symm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/roks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/sap.py
--rw-r--r--   0 runner    (1001) docker     (127)  3933728 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/sap_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/uks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/uks_symm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.043692 pyscf-2.5.0/pyscf/dft/xc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/xc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/xc/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23090 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/xc_deriv.py
--rw-r--r--   0 runner    (1001) docker     (127)    38914 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/dft/xcfun.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.043692 pyscf-2.5.0/pyscf/eph/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/eph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/eph/eph_fd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/eph/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/eph/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/eph/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/eph/uks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.047692 pyscf-2.5.0/pyscf/fci/
--rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27361 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/addons.py
--rw-r--r--   0 runner    (1001) docker     (127)    16832 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/cistring.py
--rw-r--r--   0 runner    (1001) docker     (127)    15408 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/direct_ep.py
--rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/direct_nosym.py
--rw-r--r--   0 runner    (1001) docker     (127)    18049 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/direct_spin0.py
--rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/direct_spin0_symm.py
--rw-r--r--   0 runner    (1001) docker     (127)    40720 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/direct_spin1.py
--rw-r--r--   0 runner    (1001) docker     (127)    24755 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/direct_spin1_cyl_sym.py
--rw-r--r--   0 runner    (1001) docker     (127)    33137 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/direct_spin1_symm.py
--rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/direct_uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/fci_dhf_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/fci_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)    15210 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/rdm.py
--rw-r--r--   0 runner    (1001) docker     (127)    42090 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/selected_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)    16283 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/selected_ci_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/selected_ci_spin0.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/selected_ci_spin0_symm.py
--rw-r--r--   0 runner    (1001) docker     (127)    13363 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/selected_ci_symm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/fci/spin_op.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.047692 pyscf-2.5.0/pyscf/geomopt/
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/geomopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/geomopt/addons.py
--rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/geomopt/berny_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/geomopt/geometric_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/geomopt/log.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.051692 pyscf-2.5.0/pyscf/grad/
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13914 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/casci.py
--rw-r--r--   0 runner    (1001) docker     (127)     8572 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/casscf.py
--rw-r--r--   0 runner    (1001) docker     (127)    17892 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/ccsd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13169 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/ccsd_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/ccsd_t.py
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/cisd.py
--rw-r--r--   0 runner    (1001) docker     (127)    10726 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/dhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/dispersion.py
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/lagrange.py
--rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/mp2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16884 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    24139 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/rohf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/roks.py
--rw-r--r--   0 runner    (1001) docker     (127)    41710 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/sacasscf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/tdrhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    14982 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/tdrks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/tduhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    16963 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/tduks.py
--rw-r--r--   0 runner    (1001) docker     (127)    21754 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/uccsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/uccsd_t.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/ucisd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11126 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/uks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/grad/ump2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.051692 pyscf-2.5.0/pyscf/gto/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.103691 pyscf-2.5.0/pyscf/gto/basis/
--rw-r--r--   0 runner    (1001) docker     (127)   137396 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/Burkatzi-Filippi-Dolg-PP.dat
--rw-r--r--   0 runner    (1001) docker     (127)    47103 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/DgaussA1_dft_cfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)    47104 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/DgaussA1_dft_xfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)    22868 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/DgaussA2_dft_cfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)    22870 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/DgaussA2_dft_xfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)    31249 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   141928 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/adzp.dat
--rw-r--r--   0 runner    (1001) docker     (127)    83566 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ahlrichs_cfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)  1389925 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ano.dat
--rw-r--r--   0 runner    (1001) docker     (127)   127274 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aqzp.dat
--rw-r--r--   0 runner    (1001) docker     (127)   108802 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/atzp.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pV5Z-PP.dat
--rw-r--r--   0 runner    (1001) docker     (127)   124241 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pV5Z_MP2FIT.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pVDZ-PP.dat
--rw-r--r--   0 runner    (1001) docker     (127)   134863 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pVQZ-DK3.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pVQZ-PP.dat
--rw-r--r--   0 runner    (1001) docker     (127)   108901 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pVQZ_MP2FIT.dat
--rw-r--r--   0 runner    (1001) docker     (127)   110807 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pVTZ-DK3.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pVTZ-PP.dat
--rw-r--r--   0 runner    (1001) docker     (127)   190050 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pv5z-dk.dat
--rw-r--r--   0 runner    (1001) docker     (127)    53483 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pv5z-jkfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)    97411 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pv5z-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)   190020 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pv5z.dat
--rw-r--r--   0 runner    (1001) docker     (127)   117453 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvdpdz.dat
--rw-r--r--   0 runner    (1001) docker     (127)    98649 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvdz-dk.dat
--rw-r--r--   0 runner    (1001) docker     (127)    41742 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvdz-jkfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)    30634 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvdz-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)    98569 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvdz.dat
--rw-r--r--   0 runner    (1001) docker     (127)    40752 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvdzp-jkfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)    29379 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvdzp-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)   290273 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvqz-dk.dat
--rw-r--r--   0 runner    (1001) docker     (127)    48952 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvqz-jkfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)    48083 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvqz-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)   155183 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvqz.dat
--rw-r--r--   0 runner    (1001) docker     (127)   314115 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvtz-dk.dat
--rw-r--r--   0 runner    (1001) docker     (127)    45670 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvtz-jkfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)    39435 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvtz-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)   122314 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvtz.dat
--rw-r--r--   0 runner    (1001) docker     (127)   346258 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwCVQZ-DK.dat
--rw-r--r--   0 runner    (1001) docker     (127)   183629 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwCVQZ-DK3.dat
--rw-r--r--   0 runner    (1001) docker     (127)   410566 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwCVTZ-DK.dat
--rw-r--r--   0 runner    (1001) docker     (127)   139736 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwCVTZ-DK3.dat
--rw-r--r--   0 runner    (1001) docker     (127)   124542 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwCVTZ_MP2FIT.dat
--rw-r--r--   0 runner    (1001) docker     (127)   182677 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwcv5z-dk.dat
--rw-r--r--   0 runner    (1001) docker     (127)   363886 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwcv5z.dat
--rw-r--r--   0 runner    (1001) docker     (127)    37069 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwcvdz.dat
--rw-r--r--   0 runner    (1001) docker     (127)   285250 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwcvqz.dat
--rw-r--r--   0 runner    (1001) docker     (127)   192834 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwcvtz.dat
--rw-r--r--   0 runner    (1001) docker     (127)    48451 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-pc-0.dat
--rw-r--r--   0 runner    (1001) docker     (127)   112718 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-pc-1.dat
--rw-r--r--   0 runner    (1001) docker     (127)   173735 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-pc-2.dat
--rw-r--r--   0 runner    (1001) docker     (127)   267909 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-pc-3.dat
--rw-r--r--   0 runner    (1001) docker     (127)   390219 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-pc-4.dat
--rw-r--r--   0 runner    (1001) docker     (127)    87863 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-pcseg-0.dat
--rw-r--r--   0 runner    (1001) docker     (127)   122797 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-pcseg-1.dat
--rw-r--r--   0 runner    (1001) docker     (127)   194490 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-pcseg-2.dat
--rw-r--r--   0 runner    (1001) docker     (127)   312944 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-pcseg-3.dat
--rw-r--r--   0 runner    (1001) docker     (127)   437986 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/aug-pcseg-4.dat
--rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/bfd_pp.dat
--rw-r--r--   0 runner    (1001) docker     (127)    46296 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/bfd_v5z.dat
--rw-r--r--   0 runner    (1001) docker     (127)    31518 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/bfd_vdz.dat
--rw-r--r--   0 runner    (1001) docker     (127)    65568 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/bfd_vqz.dat
--rw-r--r--   0 runner    (1001) docker     (127)    57266 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/bfd_vtz.dat
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/bse.py
--rw-r--r--   0 runner    (1001) docker     (127)   200095 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pCV5Z.dat
--rw-r--r--   0 runner    (1001) docker     (127)    54500 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pCV6Z.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pCVDZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pCVQZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pCVTZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)   103871 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pV5Z_MP2FIT.dat
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pVDZ-PP-NR.dat
--rw-r--r--   0 runner    (1001) docker     (127)   114741 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pVQZ-DK3.dat
--rw-r--r--   0 runner    (1001) docker     (127)    90211 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pVQZ_MP2FIT.dat
--rw-r--r--   0 runner    (1001) docker     (127)    93193 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pVTZ-DK3.dat
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pVTZ-PP-NR.dat
--rw-r--r--   0 runner    (1001) docker     (127)   189349 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pv5z-dk.dat
--rw-r--r--   0 runner    (1001) docker     (127)    45383 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pv5z-jkfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)   222905 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pv5z-pp.dat
--rw-r--r--   0 runner    (1001) docker     (127)    41961 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pv5z-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)   194433 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pv5z.dat
--rw-r--r--   0 runner    (1001) docker     (127)   115228 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pvdpdz.dat
--rw-r--r--   0 runner    (1001) docker     (127)   377366 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pvdz-dk.dat
--rw-r--r--   0 runner    (1001) docker     (127)    36718 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pvdz-jkfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)    94731 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pvdz-pp.dat
--rw-r--r--   0 runner    (1001) docker     (127)    30544 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pvdz-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)    94827 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pvdz.dat
--rw-r--r--   0 runner    (1001) docker     (127)    11311 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pvdz_fit.dat
--rw-r--r--   0 runner    (1001) docker     (127)   850318 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pvqz-dk.dat
--rw-r--r--   0 runner    (1001) docker     (127)    41794 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pvqz-jkfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)   177582 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pvqz-pp.dat
--rw-r--r--   0 runner    (1001) docker     (127)    48631 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pvqz-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)   149280 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pvqz.dat
--rw-r--r--   0 runner    (1001) docker     (127)   914722 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pvtz-dk.dat
--rw-r--r--   0 runner    (1001) docker     (127)    39454 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pvtz-jkfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)   132320 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pvtz-pp.dat
--rw-r--r--   0 runner    (1001) docker     (127)    39711 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pvtz-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)   117771 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pvtz.dat
--rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pvtz_fit.dat
--rw-r--r--   0 runner    (1001) docker     (127)   106072 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pwCV5Z-DK.dat
--rw-r--r--   0 runner    (1001) docker     (127)    98164 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pwCV5Z-PP.dat
--rw-r--r--   0 runner    (1001) docker     (127)   232487 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pwCV5Z.dat
--rw-r--r--   0 runner    (1001) docker     (127)    53340 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pwCVDZ-DK.dat
--rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pwCVDZ-PP.dat
--rw-r--r--   0 runner    (1001) docker     (127)    18284 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pwCVDZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)   241499 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pwCVQZ-DK.dat
--rw-r--r--   0 runner    (1001) docker     (127)   160567 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pwCVQZ-DK3.dat
--rw-r--r--   0 runner    (1001) docker     (127)    32332 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pwCVQZ-PP.dat
--rw-r--r--   0 runner    (1001) docker     (127)    84240 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pwCVQZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)   240607 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pwCVTZ-DK.dat
--rw-r--r--   0 runner    (1001) docker     (127)   120526 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pwCVTZ-DK3.dat
--rw-r--r--   0 runner    (1001) docker     (127)    22290 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pwCVTZ-PP.dat
--rw-r--r--   0 runner    (1001) docker     (127)    99466 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pwCVTZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)   104732 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/cc-pwCVTZ_MP2FIT.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.011693 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.103691 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/
--rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP.dat
--rw-r--r--   0 runner    (1001) docker     (127)    80494 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pV5Z.dat
--rw-r--r--   0 runner    (1001) docker     (127)    36684 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pV6Z.dat
--rw-r--r--   0 runner    (1001) docker     (127)    41351 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pVDZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)    66515 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pVQZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)    53428 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pVTZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)    75421 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pV5Z.dat
--rw-r--r--   0 runner    (1001) docker     (127)    34550 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pV6Z.dat
--rw-r--r--   0 runner    (1001) docker     (127)    38752 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pVDZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)    62219 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pVQZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)    49967 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pVTZ.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.107691 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP.dat
--rw-r--r--   0 runner    (1001) docker     (127)    13000 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_aug-cc-pV5Z.dat
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_aug-cc-pV6Z.dat
--rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_aug-cc-pVDZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_aug-cc-pVQZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10426 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_aug-cc-pVTZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)    11812 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_cc-pV5Z.dat
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_cc-pV6Z.dat
--rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_cc-pVDZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_cc-pVQZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_cc-pVTZ.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.107691 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_aug-cc-pV5Z.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_aug-cc-pVDZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_aug-cc-pVQZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_aug-cc-pVTZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_cc-pV5Z.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_cc-pVDZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_cc-pVQZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_cc-pVTZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)   262035 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/crenbl.dat
--rw-r--r--   0 runner    (1001) docker     (127)   129690 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/crenbs.dat
--rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/crystal-cc-pvdz.dat
--rw-r--r--   0 runner    (1001) docker     (127)    37024 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-qzvp-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)   180299 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-qzvp.dat
--rw-r--r--   0 runner    (1001) docker     (127)   185113 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-qzvpd.dat
--rw-r--r--   0 runner    (1001) docker     (127)    43496 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-qzvpp-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)   184475 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-qzvpp.dat
--rw-r--r--   0 runner    (1001) docker     (127)    45242 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-qzvppd-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)   189343 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-qzvppd.dat
--rw-r--r--   0 runner    (1001) docker     (127)    57404 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-svp-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)   110762 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-svp.dat
--rw-r--r--   0 runner    (1001) docker     (127)    60367 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-svpd-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)   117659 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-svpd.dat
--rw-r--r--   0 runner    (1001) docker     (127)    71708 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-tzvp-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)   132134 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-tzvp.dat
--rw-r--r--   0 runner    (1001) docker     (127)    74591 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-tzvpd-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)   138427 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-tzvpd.dat
--rw-r--r--   0 runner    (1001) docker     (127)    59466 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-tzvpp-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)   136623 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-tzvpp.dat
--rw-r--r--   0 runner    (1001) docker     (127)    62380 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-tzvppd-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)   142965 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-tzvppd.dat
--rw-r--r--   0 runner    (1001) docker     (127)   130384 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-universal-jfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)   235329 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/def2-universal-jkfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)    47198 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/demon_cfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/dyall_dz.py
--rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/dyall_qz.py
--rw-r--r--   0 runner    (1001) docker     (127)    13052 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/dyall_tz.py
--rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/dz.dat
--rw-r--r--   0 runner    (1001) docker     (127)   131530 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/dzp-dkh.dat
--rw-r--r--   0 runner    (1001) docker     (127)   132516 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/dzp.dat
--rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/dzp_dunning.py
--rw-r--r--   0 runner    (1001) docker     (127)   178866 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/dzvp.dat
--rw-r--r--   0 runner    (1001) docker     (127)    71969 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/dzvp2.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.111691 pyscf-2.5.0/pyscf/gto/basis/f12-basis/
--rw-r--r--   0 runner    (1001) docker     (127)    20014 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/f12-basis/aug-cc-pV5Z-OptRI.dat
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/f12-basis/aug-cc-pVDZ-OptRI.dat
--rw-r--r--   0 runner    (1001) docker     (127)    17248 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/f12-basis/aug-cc-pVQZ-OptRI.dat
--rw-r--r--   0 runner    (1001) docker     (127)    15259 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/f12-basis/aug-cc-pVTZ-OptRI.dat
--rw-r--r--   0 runner    (1001) docker     (127)    28721 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pCVDZ-F12-OptRI.dat
--rw-r--r--   0 runner    (1001) docker     (127)    26437 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pCVQZ-F12-OptRI.dat
--rw-r--r--   0 runner    (1001) docker     (127)    25757 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pCVTZ-F12-OptRI.dat
--rw-r--r--   0 runner    (1001) docker     (127)    56899 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pV5Z-F12.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pV5Z-F12rev2.dat
--rw-r--r--   0 runner    (1001) docker     (127)    12587 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pVDZ-F12-OptRI.dat
--rw-r--r--   0 runner    (1001) docker     (127)    26302 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pVDZ-F12-nZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pVDZ-F12rev2.dat
--rw-r--r--   0 runner    (1001) docker     (127)    13769 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pVQZ-F12-OptRI.dat
--rw-r--r--   0 runner    (1001) docker     (127)    48697 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pVQZ-F12-nZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pVQZ-F12rev2.dat
--rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pVTZ-F12-OptRI.dat
--rw-r--r--   0 runner    (1001) docker     (127)    35324 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pVTZ-F12-nZ.dat
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pVTZ-F12rev2.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/faegre_dz.py
--rw-r--r--   0 runner    (1001) docker     (127)    43856 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/heavy-aug-cc-pvdz-jkfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)    30481 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/heavy-aug-cc-pvdz-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)    47735 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/heavy-aug-cc-pvtz-jkfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)    39167 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/heavy-aug-cc-pvtz-ri.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/iglo3.py
--rw-r--r--   0 runner    (1001) docker     (127)    92388 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/lanl08.dat
--rw-r--r--   0 runner    (1001) docker     (127)   109544 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/lanl2dz.dat
--rw-r--r--   0 runner    (1001) docker     (127)    52603 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/lanl2tz.dat
--rw-r--r--   0 runner    (1001) docker     (127)   117876 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/minao.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/parse_bfd_pp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/parse_cp2k.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/parse_cp2k_pp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/parse_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/parse_molpro.py
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/parse_nwchem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/parse_nwchem_ecp.py
--rw-r--r--   0 runner    (1001) docker     (127)    35344 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pc-0.dat
--rw-r--r--   0 runner    (1001) docker     (127)    82701 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pc-1.dat
--rw-r--r--   0 runner    (1001) docker     (127)   132372 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pc-2.dat
--rw-r--r--   0 runner    (1001) docker     (127)   211146 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pc-3.dat
--rw-r--r--   0 runner    (1001) docker     (127)   315764 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pc-4.dat
--rw-r--r--   0 runner    (1001) docker     (127)    65047 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pcseg-0.dat
--rw-r--r--   0 runner    (1001) docker     (127)    91188 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pcseg-1.dat
--rw-r--r--   0 runner    (1001) docker     (127)   150241 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pcseg-2.dat
--rw-r--r--   0 runner    (1001) docker     (127)   250673 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pcseg-3.dat
--rw-r--r--   0 runner    (1001) docker     (127)   357977 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pcseg-4.dat
--rw-r--r--   0 runner    (1001) docker     (127)    35826 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pob-tzvp.dat
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pob-tzvpp.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.119691 pyscf-2.5.0/pyscf/gto/basis/pople-basis/
--rw-r--r--   0 runner    (1001) docker     (127)    55204 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/3-21++G.dat
--rw-r--r--   0 runner    (1001) docker     (127)    55937 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/3-21++Gs.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/3-21G-diffuse.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/3-21G-polarization.dat
--rw-r--r--   0 runner    (1001) docker     (127)    53526 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/3-21G.dat
--rw-r--r--   0 runner    (1001) docker     (127)    54234 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/3-21Gs.dat
--rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/4-31G.dat
--rw-r--r--   0 runner    (1001) docker     (127)    36010 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31++G.dat
--rw-r--r--   0 runner    (1001) docker     (127)    21162 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31++Gs.dat
--rw-r--r--   0 runner    (1001) docker     (127)    38362 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31++Gss.dat
--rw-r--r--   0 runner    (1001) docker     (127)    21734 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31+G.dat
--rw-r--r--   0 runner    (1001) docker     (127)    20062 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31+Gs.dat
--rw-r--r--   0 runner    (1001) docker     (127)    22947 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31+Gss.dat
--rw-r--r--   0 runner    (1001) docker     (127)    20190 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311++G.dat
--rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311++Gs.dat
--rw-r--r--   0 runner    (1001) docker     (127)    34756 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311++Gss.dat
--rw-r--r--   0 runner    (1001) docker     (127)    20634 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311+G.dat
--rw-r--r--   0 runner    (1001) docker     (127)    22361 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311+Gs.dat
--rw-r--r--   0 runner    (1001) docker     (127)    22104 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311+Gss.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311G-diffuse.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311G-polarization-2d.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311G-polarization-2p.dat
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311G-polarization-3d.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311G-polarization-3p.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311G-polarization-d.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311G-polarization-f.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311G-polarization-p.dat
--rw-r--r--   0 runner    (1001) docker     (127)    31263 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311G.dat
--rw-r--r--   0 runner    (1001) docker     (127)    33384 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311Gs.dat
--rw-r--r--   0 runner    (1001) docker     (127)    33056 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311Gss.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31G-diffuse.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31G-polarization-2d.dat
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31G-polarization-2p.dat
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31G-polarization-3d.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31G-polarization-3p.dat
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31G-polarization-d.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31G-polarization-f.dat
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31G-polarization-p.dat
--rw-r--r--   0 runner    (1001) docker     (127)    34316 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31G.dat
--rw-r--r--   0 runner    (1001) docker     (127)    44932 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31Gs.dat
--rw-r--r--   0 runner    (1001) docker     (127)    36668 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31Gss.dat
--rw-r--r--   0 runner    (1001) docker     (127)   117420 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/qzp-dkh.dat
--rw-r--r--   0 runner    (1001) docker     (127)   117314 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/qzp.dat
--rw-r--r--   0 runner    (1001) docker     (127)   139676 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/roos-dz.dat
--rw-r--r--   0 runner    (1001) docker     (127)   169498 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/roos-tz.dat
--rw-r--r--   0 runner    (1001) docker     (127)   142994 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/sarc-dkh2.dat
--rw-r--r--   0 runner    (1001) docker     (127)    72840 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/sbkjc.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.119691 pyscf-2.5.0/pyscf/gto/basis/soecp/
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/soecp/ECPDS10MDFSO.dat
--rw-r--r--   0 runner    (1001) docker     (127)    12273 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/soecp/ECPDS28MDFSO.dat
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/soecp/ECPDS28MWBSO.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/soecp/ECPDS46MDFSO.dat
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/soecp/ECPDS60MDFSO.dat
--rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/soecp/ECPDS60MWBSO.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/soecp/ECPDS78MDFSO.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/soecp/ECPDS92MDFBQSO.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10955 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/soecp/ECPDS92MDFBSO.dat
--rw-r--r--   0 runner    (1001) docker     (127)    49513 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/sto-3g.dat
--rw-r--r--   0 runner    (1001) docker     (127)    50158 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/sto-6g.dat
--rw-r--r--   0 runner    (1001) docker     (127)    70653 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/stuttgart_dz.dat
--rw-r--r--   0 runner    (1001) docker     (127)   140417 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/stuttgart_rsc.dat
--rw-r--r--   0 runner    (1001) docker     (127)   100829 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/tzp-dkh.dat
--rw-r--r--   0 runner    (1001) docker     (127)   100810 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/tzp.dat
--rw-r--r--   0 runner    (1001) docker     (127)    48273 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/tzv.dat
--rw-r--r--   0 runner    (1001) docker     (127)   130384 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/basis/weigend_cfit.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/cmd_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/ecp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/eval_gto.py
--rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/ft_ao.py
--rw-r--r--   0 runner    (1001) docker     (127)   146926 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/mole.py
--rw-r--r--   0 runner    (1001) docker     (127)    37978 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/moleintor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gto/pp_int.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.119691 pyscf-2.5.0/pyscf/gw/
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15523 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gw/gw_ac.py
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gw/gw_cd.py
--rw-r--r--   0 runner    (1001) docker     (127)    14559 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gw/gw_exact.py
--rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gw/gw_slow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9192 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gw/rpa.py
--rw-r--r--   0 runner    (1001) docker     (127)    18642 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gw/ugw_ac.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7562 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/gw/urpa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.119691 pyscf-2.5.0/pyscf/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/hessian/dispersion.py
--rw-r--r--   0 runner    (1001) docker     (127)    26294 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/hessian/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    25692 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/hessian/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)    14633 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/hessian/thermo.py
--rw-r--r--   0 runner    (1001) docker     (127)    21119 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/hessian/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    35698 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/hessian/uks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.123691 pyscf-2.5.0/pyscf/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.123691 pyscf-2.5.0/pyscf/lib/agf2/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/agf2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13242 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/agf2/ragf2.c
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/agf2/ragf2.h
--rw-r--r--   0 runner    (1001) docker     (127)    12519 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/agf2/uagf2.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.123691 pyscf-2.5.0/pyscf/lib/ao2mo/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/ao2mo/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    46111 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/ao2mo/nr_ao2mo.c
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/ao2mo/nr_ao2mo.h
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/ao2mo/nr_incore.c
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/ao2mo/nr_incore.h
--rw-r--r--   0 runner    (1001) docker     (127)    10926 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/ao2mo/nrr_ao2mo.c
--rw-r--r--   0 runner    (1001) docker     (127)    34149 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/ao2mo/r_ao2mo.c
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/ao2mo/r_ao2mo.h
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/ao2mo/restore_eri.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.127691 pyscf-2.5.0/pyscf/lib/cc/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/cc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/cc/ccsd_grad.c
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/cc/ccsd_pack.c
--rw-r--r--   0 runner    (1001) docker     (127)    45611 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/cc/ccsd_t.c
--rw-r--r--   0 runner    (1001) docker     (127)    36526 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/cc/uccsd_t.c
--rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/chkfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/config.h.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.127691 pyscf-2.5.0/pyscf/lib/dft/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/dft/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)   173239 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/dft/CxLebedevGrid.c
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/dft/grid_basis.c
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/dft/grid_basis.h
--rw-r--r--   0 runner    (1001) docker     (127)    35436 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/dft/libxc_itrf.c
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/dft/nr_numint.c
--rw-r--r--   0 runner    (1001) docker     (127)    54245 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/dft/nr_numint_sparse.c
--rw-r--r--   0 runner    (1001) docker     (127)   105128 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/dft/numint_uniform_grid.c
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/dft/r_numint.c
--rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/dft/xc_deriv.c
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/dft/xcfun_itrf.c
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/diis.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.131691 pyscf-2.5.0/pyscf/lib/gto/
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.131691 pyscf-2.5.0/pyscf/lib/gto/autocode/
--rw-r--r--   0 runner    (1001) docker     (127)    57483 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/autocode/auto_eval1.c
--rw-r--r--   0 runner    (1001) docker     (127)    26701 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/deriv1.c
--rw-r--r--   0 runner    (1001) docker     (127)    63100 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/deriv2.c
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/fastexp.c
--rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/fill_grids_int2c.c
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/fill_int2c.c
--rw-r--r--   0 runner    (1001) docker     (127)    24491 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/fill_int2e.c
--rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/fill_nr_3c.c
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/fill_r_3c.c
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/fill_r_4c.c
--rw-r--r--   0 runner    (1001) docker     (127)    51411 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/ft_ao.c
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/ft_ao.h
--rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/ft_ao_deriv.c
--rw-r--r--   0 runner    (1001) docker     (127)    20944 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/grid_ao_drv.c
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/grid_ao_drv.h
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/gto.h
--rw-r--r--   0 runner    (1001) docker     (127)  1014868 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/nr_ecp.c
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/nr_ecp.h
--rw-r--r--   0 runner    (1001) docker     (127)    45488 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/gto/nr_ecp_deriv.c
--rw-r--r--   0 runner    (1001) docker     (127)    61502 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/linalg_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.131691 pyscf-2.5.0/pyscf/lib/mcscf/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/mcscf/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/mcscf/fci.h
--rw-r--r--   0 runner    (1001) docker     (127)    23910 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/mcscf/fci_4pdm.c
--rw-r--r--   0 runner    (1001) docker     (127)    41828 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/mcscf/fci_contract.c
--rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/mcscf/fci_contract_nosym.c
--rw-r--r--   0 runner    (1001) docker     (127)    30335 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/mcscf/fci_rdm.c
--rw-r--r--   0 runner    (1001) docker     (127)    14715 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/mcscf/fci_string.c
--rw-r--r--   0 runner    (1001) docker     (127)     9579 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/mcscf/nevpt_contract.c
--rw-r--r--   0 runner    (1001) docker     (127)    25231 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/mcscf/select_ci.c
--rw-r--r--   0 runner    (1001) docker     (127)    45514 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.135691 pyscf-2.5.0/pyscf/lib/np_helper/
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/np_helper/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/np_helper/condense.c
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/np_helper/np_helper.c
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/np_helper/np_helper.h
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/np_helper/npdot.c
--rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/np_helper/omp_reduce.c
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/np_helper/pack_tril.c
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/np_helper/transpose.c
--rw-r--r--   0 runner    (1001) docker     (127)    45876 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/numpy_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.135691 pyscf-2.5.0/pyscf/lib/pbc/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/pbc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14428 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/pbc/cint2e.c
--rw-r--r--   0 runner    (1001) docker     (127)    14523 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/pbc/cint3c2e.c
--rw-r--r--   0 runner    (1001) docker     (127)    58339 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/pbc/fill_ints.c
--rw-r--r--   0 runner    (1001) docker     (127)    77592 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/pbc/fill_ints_sr.c
--rw-r--r--   0 runner    (1001) docker     (127)    36806 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/pbc/ft_ao.c
--rw-r--r--   0 runner    (1001) docker     (127)    30687 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/pbc/grid_ao.c
--rw-r--r--   0 runner    (1001) docker     (127)    31483 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/pbc/inner_dot.c
--rw-r--r--   0 runner    (1001) docker     (127)    50426 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/pbc/nr_direct.c
--rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/pbc/nr_ecp.c
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/pbc/optimizer.c
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/pbc/optimizer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/pbc/pbc.h
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/pbc/symmetry.c
--rw-r--r--   0 runner    (1001) docker     (127)    14078 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/pbc/transform_mo.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.135691 pyscf-2.5.0/pyscf/lib/ri/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/ri/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/ri/r_df_incore.c
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/scipy_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.139691 pyscf-2.5.0/pyscf/lib/vhf/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/cvhf.h
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/fblas.h
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/fill_nr_s8.c
--rw-r--r--   0 runner    (1001) docker     (127)    13464 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/hessian_screen.c
--rw-r--r--   0 runner    (1001) docker     (127)    26469 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/nr_direct.c
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/nr_direct.h
--rw-r--r--   0 runner    (1001) docker     (127)   135778 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/nr_direct_dot.c
--rw-r--r--   0 runner    (1001) docker     (127)    29999 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/nr_incore.c
--rw-r--r--   0 runner    (1001) docker     (127)    20984 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/nr_sgx_direct.c
--rw-r--r--   0 runner    (1001) docker     (127)    41654 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/nr_sr_vhf.c
--rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/optimizer.c
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/optimizer.h
--rw-r--r--   0 runner    (1001) docker     (127)    24284 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/r_direct_dot.c
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/r_direct_dot.h
--rw-r--r--   0 runner    (1001) docker     (127)    12689 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/r_direct_o1.c
--rw-r--r--   0 runner    (1001) docker     (127)    14446 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/rah_direct_dot.c
--rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/rha_direct_dot.c
--rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/rkb_screen.c
--rw-r--r--   0 runner    (1001) docker     (127)    25499 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/time_rev.c
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lib/vhf/time_rev.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.139691 pyscf-2.5.0/pyscf/lo/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lo/boys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lo/cholesky.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lo/edmiston.py
--rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lo/iao.py
--rw-r--r--   0 runner    (1001) docker     (127)    16583 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lo/ibo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lo/nao.py
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lo/orth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11596 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lo/pipek.py
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lo/pipek_jacobi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/lo/vvo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.143691 pyscf-2.5.0/pyscf/mcscf/
--rw-r--r--   0 runner    (1001) docker     (127)    20800 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/PiOS.py
--rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63576 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/addons.py
--rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/apc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10115 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/avas.py
--rw-r--r--   0 runner    (1001) docker     (127)    49443 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/casci.py
--rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/casci_symm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/chkfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    16428 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/df.py
--rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/dmet_cas.py
--rw-r--r--   0 runner    (1001) docker     (127)    59639 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/mc1step.py
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/mc1step_symm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7967 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/mc2step.py
--rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/mc_ao2mo.py
--rw-r--r--   0 runner    (1001) docker     (127)    39340 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/newton_casscf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/newton_casscf_symm.py
--rw-r--r--   0 runner    (1001) docker     (127)    20208 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/ucasci.py
--rw-r--r--   0 runner    (1001) docker     (127)    37853 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/umc1step.py
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/umc2step.py
--rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mcscf/umc_ao2mo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.143691 pyscf-2.5.0/pyscf/md/
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/md/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/md/distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21000 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/md/integrators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.147691 pyscf-2.5.0/pyscf/mp/
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mp/dfgmp2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mp/dfmp2.py
--rw-r--r--   0 runner    (1001) docker     (127)    30565 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mp/dfmp2_native.py
--rw-r--r--   0 runner    (1001) docker     (127)    26264 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mp/dfump2_native.py
--rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mp/gmp2.py
--rw-r--r--   0 runner    (1001) docker     (127)    30846 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mp/mp2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mp/mp2f12_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)    30465 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mp/ump2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.147691 pyscf-2.5.0/pyscf/mrpt/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mrpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43034 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/mrpt/nevpt2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.147691 pyscf-2.5.0/pyscf/nac/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/nac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13593 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/nac/sacasscf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.147691 pyscf-2.5.0/pyscf/pbc/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/__all__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.147691 pyscf-2.5.0/pyscf/pbc/adc/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/adc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/adc/dfadc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13136 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/adc/kadc_ao2mo.py
--rw-r--r--   0 runner    (1001) docker     (127)    11411 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/adc/kadc_rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/adc/kadc_rhf_amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (127)    62323 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/adc/kadc_rhf_ea.py
--rw-r--r--   0 runner    (1001) docker     (127)    46652 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/adc/kadc_rhf_ip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.147691 pyscf-2.5.0/pyscf/pbc/ao2mo/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/ao2mo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/ao2mo/eris.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.151691 pyscf-2.5.0/pyscf/pbc/cc/
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/ccsd.py
--rw-r--r--   0 runner    (1001) docker     (127)    82519 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/eom_kccsd_ghf.py
--rw-r--r--   0 runner    (1001) docker     (127)    68243 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/eom_kccsd_rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/eom_kccsd_rhf_ea.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/eom_kccsd_rhf_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)    57971 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/eom_kccsd_uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    35071 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/kccsd.py
--rw-r--r--   0 runner    (1001) docker     (127)    50332 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/kccsd_rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    31944 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/kccsd_rhf_ksymm.py
--rw-r--r--   0 runner    (1001) docker     (127)    15664 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/kccsd_t.py
--rw-r--r--   0 runner    (1001) docker     (127)    28804 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/kccsd_t_rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/kccsd_t_rhf_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)    48953 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/kccsd_uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    22273 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/kintermediates.py
--rw-r--r--   0 runner    (1001) docker     (127)    42214 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/kintermediates_rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/kintermediates_rhf_ksymm.py
--rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/kintermediates_uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/cc/kuccsd_rdm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.151691 pyscf-2.5.0/pyscf/pbc/ci/
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/ci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/ci/cisd.py
--rw-r--r--   0 runner    (1001) docker     (127)    26419 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/ci/kcis_rhf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.155691 pyscf-2.5.0/pyscf/pbc/df/
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28912 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/aft.py
--rw-r--r--   0 runner    (1001) docker     (127)    17682 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/aft_ao2mo.py
--rw-r--r--   0 runner    (1001) docker     (127)    31911 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/aft_jk.py
--rw-r--r--   0 runner    (1001) docker     (127)    33902 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/df.py
--rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/df_ao2mo.py
--rw-r--r--   0 runner    (1001) docker     (127)    68892 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/df_jk.py
--rw-r--r--   0 runner    (1001) docker     (127)    13866 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/fft.py
--rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/fft_ao2mo.py
--rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/fft_jk.py
--rw-r--r--   0 runner    (1001) docker     (127)    32436 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/ft_ao.py
--rw-r--r--   0 runner    (1001) docker     (127)    45554 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/gdf_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/incore.py
--rw-r--r--   0 runner    (1001) docker     (127)    18156 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/mdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/mdf_ao2mo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/mdf_jk.py
--rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/outcore.py
--rw-r--r--   0 runner    (1001) docker     (127)    29064 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/rsdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    69541 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/rsdf_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    53162 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/rsdf_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/df/rsdf_jk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.155691 pyscf-2.5.0/pyscf/pbc/dft/
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/cdft.py
--rw-r--r--   0 runner    (1001) docker     (127)     9978 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/gen_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/gks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/kgks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/krks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/krks_ksymm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/krkspu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/krkspu_ksymm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/kroks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/kuks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/kuks_ksymm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/kukspu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/kukspu_ksymm.py
--rw-r--r--   0 runner    (1001) docker     (127)    73837 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/multigrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    51723 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/numint.py
--rw-r--r--   0 runner    (1001) docker     (127)    26935 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/numint2c.py
--rw-r--r--   0 runner    (1001) docker     (127)    13364 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/roks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/dft/uks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.155691 pyscf-2.5.0/pyscf/pbc/eph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/eph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/eph/eph_fd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.155691 pyscf-2.5.0/pyscf/pbc/geomopt/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/geomopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/geomopt/geometric_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.159691 pyscf-2.5.0/pyscf/pbc/grad/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/grad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17337 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/grad/krhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/grad/krks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/grad/kuhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/grad/kuks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.159691 pyscf-2.5.0/pyscf/pbc/gto/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/_pbcintor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.163691 pyscf-2.5.0/pyscf/pbc/gto/basis/
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-aug-dzvp.dat
--rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-aug-qzv2p.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-aug-qzv3p.dat
--rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-aug-tzv2p.dat
--rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-aug-tzvp.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-cc-dzvp.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-cc-qzvp.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-cc-tzvp.dat
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-dzv.dat
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-dzvp-molopt-sr-q9.dat
--rw-r--r--   0 runner    (1001) docker     (127)    53413 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-dzvp-molopt-sr.dat
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-dzvp-molopt.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10728 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-dzvp.dat
--rw-r--r--   0 runner    (1001) docker     (127)    18881 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-qzv2p.dat
--rw-r--r--   0 runner    (1001) docker     (127)    20609 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-qzv3p.dat
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-szv-molopt-sr-q9.dat
--rw-r--r--   0 runner    (1001) docker     (127)    31790 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-szv-molopt-sr.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-szv-molopt.dat
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-szv.dat
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-szvp-molopt-sr-q9.dat
--rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-tzv2p-molopt.dat
--rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-tzv2p.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-tzv2px-molopt.dat
--rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-tzvp-molopt.dat
--rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/gth-tzvp.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/split_BASIS_MOLOPT.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/split_GTH_BASIS_SETS.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/basis/split_HFX_BASIS.py
--rw-r--r--   0 runner    (1001) docker     (127)    59906 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/ecp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/eval_gto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.163691 pyscf-2.5.0/pyscf/pbc/gto/pseudo/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/pseudo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24006 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-blyp.dat
--rw-r--r--   0 runner    (1001) docker     (127)    14867 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-bp.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-hcth120.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-hcth407.dat
--rw-r--r--   0 runner    (1001) docker     (127)    90523 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-hf-rev.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-hf.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-olyp.dat
--rw-r--r--   0 runner    (1001) docker     (127)    54113 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-pade.dat
--rw-r--r--   0 runner    (1001) docker     (127)    42074 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-pbe.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-pbesol.dat
--rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/pseudo/pp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/pseudo/pp_int.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gto/pseudo/split_GTH_POTENTIALS.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.167691 pyscf-2.5.0/pyscf/pbc/gw/
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gw/gw_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gw/kgw_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gw/kgw_slow_supercell.py
--rw-r--r--   0 runner    (1001) docker     (127)    23938 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gw/krgw_ac.py
--rw-r--r--   0 runner    (1001) docker     (127)    26680 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gw/krgw_cd.py
--rw-r--r--   0 runner    (1001) docker     (127)    31709 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/gw/kugw_ac.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.167691 pyscf-2.5.0/pyscf/pbc/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/lib/arnoldi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/lib/chkfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    41502 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/lib/kpts.py
--rw-r--r--   0 runner    (1001) docker     (127)    21741 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/lib/kpts_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12221 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/lib/ktensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    29306 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/lib/linalg_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.167691 pyscf-2.5.0/pyscf/pbc/mp/
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/mp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30953 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/mp/kmp2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/mp/kmp2_ksymm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16730 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/mp/kmp2_stagger.py
--rw-r--r--   0 runner    (1001) docker     (127)    17429 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/mp/kump2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/mp/mp2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.167691 pyscf-2.5.0/pyscf/pbc/mpicc/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/mpicc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   160408 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/mpicc/kccsd_rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    70288 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/mpicc/kintermediates_rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/mpicc/mpi_kpoint_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.171691 pyscf-2.5.0/pyscf/pbc/mpitools/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/mpitools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/mpitools/mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/mpitools/mpi_blksize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/mpitools/mpi_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/mpitools/mpi_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/mpitools/mpi_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.171691 pyscf-2.5.0/pyscf/pbc/scf/
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/_response_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20864 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/addons.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/chkfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/cphf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/ghf.py
--rw-r--r--   0 runner    (1001) docker     (127)    33722 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10955 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/kghf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/kghf_ksymm.py
--rw-r--r--   0 runner    (1001) docker     (127)    28273 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/khf.py
--rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/khf_ksymm.py
--rw-r--r--   0 runner    (1001) docker     (127)    15198 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/krohf.py
--rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/kuhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/kuhf_ksymm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/newton_ah.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/rohf.py
--rw-r--r--   0 runner    (1001) docker     (127)    61474 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/rsjk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/scfint.py
--rw-r--r--   0 runner    (1001) docker     (127)    11808 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/stability.py
--rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/scf/uhf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.175691 pyscf-2.5.0/pyscf/pbc/symm/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/symm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/symm/basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/symm/geom.py
--rw-r--r--   0 runner    (1001) docker     (127)    14926 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/symm/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/symm/pyscf_spglib.py
--rw-r--r--   0 runner    (1001) docker     (127)    12557 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/symm/space_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/symm/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/symm/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.175691 pyscf-2.5.0/pyscf/pbc/tddft/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tddft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.175691 pyscf-2.5.0/pyscf/pbc/tdscf/
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tdscf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tdscf/kproxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    26753 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tdscf/kproxy_supercell.py
--rw-r--r--   0 runner    (1001) docker     (127)    16962 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tdscf/krhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tdscf/krhf_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tdscf/krhf_slow_gamma.py
--rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tdscf/krhf_slow_supercell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tdscf/krks.py
--rw-r--r--   0 runner    (1001) docker     (127)    14816 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tdscf/kuhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tdscf/kuks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tdscf/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tdscf/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tdscf/rhf_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tdscf/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tdscf/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tdscf/uks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.175691 pyscf-2.5.0/pyscf/pbc/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tools/k2gamma.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tools/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tools/make_test_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    27495 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tools/pbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tools/print_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tools/pyscf_ase.py
--rw-r--r--   0 runner    (1001) docker     (127)    52879 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tools/pywannier90.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/tools/tril.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.175691 pyscf-2.5.0/pyscf/pbc/x2c/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/x2c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/x2c/sfx2c1e.py
--rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/pbc/x2c/x2c1e.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/post_scf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.179690 pyscf-2.5.0/pyscf/qmmm/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/qmmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/qmmm/itrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/qmmm/mm_mole.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.179690 pyscf-2.5.0/pyscf/scf/
--rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11809 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/_response_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30113 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/_vhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    48676 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/addons.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/atom_hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/atom_ks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/chkfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/cphf.py
--rw-r--r--   0 runner    (1001) docker     (127)    36697 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/dhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/diis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/dispersion.py
--rw-r--r--   0 runner    (1001) docker     (127)    20608 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/ghf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12904 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/ghf_symm.py
--rw-r--r--   0 runner    (1001) docker     (127)    80267 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)    39175 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/hf_symm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/jk.py
--rw-r--r--   0 runner    (1001) docker     (127)    20066 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/rohf.py
--rw-r--r--   0 runner    (1001) docker     (127)    24292 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/stability.py
--rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/stability_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/ucphf.py
--rw-r--r--   0 runner    (1001) docker     (127)    42278 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/scf/uhf_symm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.179690 pyscf-2.5.0/pyscf/sgx/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13492 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/sgx/sgx.py
--rw-r--r--   0 runner    (1001) docker     (127)    13133 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/sgx/sgx_jk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.183690 pyscf-2.5.0/pyscf/solvent/
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/solvent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25347 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/solvent/_attach_solvent.py
--rw-r--r--   0 runner    (1001) docker     (127)    57125 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/solvent/_ddcosmo_tdscf_grad.py
--rw-r--r--   0 runner    (1001) docker     (127)    36384 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/solvent/ddcosmo.py
--rw-r--r--   0 runner    (1001) docker     (127)    14715 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/solvent/ddcosmo_grad.py
--rw-r--r--   0 runner    (1001) docker     (127)    13456 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/solvent/ddpcm.py
--rw-r--r--   0 runner    (1001) docker     (127)    13849 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/solvent/pcm.py
--rw-r--r--   0 runner    (1001) docker     (127)    18233 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/solvent/pol_embed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.183690 pyscf-2.5.0/pyscf/soscf/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/soscf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12242 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/soscf/ciah.py
--rw-r--r--   0 runner    (1001) docker     (127)    41186 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/soscf/newton_ah.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.183690 pyscf-2.5.0/pyscf/symm/
--rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/symm/Dmatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/symm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24620 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/symm/addons.py
--rw-r--r--   0 runner    (1001) docker     (127)    25106 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/symm/basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/symm/cg.py
--rw-r--r--   0 runner    (1001) docker     (127)    34292 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/symm/geom.py
--rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/symm/msym.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/symm/param.py
--rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/symm/sph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.183690 pyscf-2.5.0/pyscf/tddft/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tddft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.187690 pyscf-2.5.0/pyscf/tdscf/
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tdscf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23983 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tdscf/common_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)    28165 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tdscf/dhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tdscf/dks.py
--rw-r--r--   0 runner    (1001) docker     (127)    25563 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tdscf/ghf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tdscf/gks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tdscf/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    39713 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tdscf/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tdscf/rhf_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tdscf/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)    34416 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tdscf/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8816 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tdscf/uks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.187690 pyscf-2.5.0/pyscf/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tools/c60struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     9579 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tools/chgcar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tools/chkfile_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    14652 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tools/cubegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tools/dump_mat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14567 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tools/fcidump.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tools/mo_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tools/molden.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tools/ring.py
--rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/tools/wfn_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.187690 pyscf-2.5.0/pyscf/x2c/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/x2c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/x2c/_response_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/x2c/dft.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/x2c/newton_ah.py
--rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/x2c/sfx2c1e.py
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/x2c/sfx2c1e_grad.py
--rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/x2c/sfx2c1e_hess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/x2c/stability.py
--rw-r--r--   0 runner    (1001) docker     (127)    15463 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/x2c/tdscf.py
--rw-r--r--   0 runner    (1001) docker     (127)    36155 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf/x2c/x2c.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:40:40.019693 pyscf-2.5.0/pyscf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    28096 2024-02-05 22:40:40.000000 pyscf-2.5.0/pyscf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-05 22:40:39.000000 pyscf-2.5.0/pyscf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-05 22:40:40.191690 pyscf-2.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6679 2024-02-05 22:40:39.000000 pyscf-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.755082 pyscf-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    53192 2024-06-01 22:08:47.000000 pyscf-2.6.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-01 22:08:47.000000 pyscf-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-06-01 22:08:47.000000 pyscf-2.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-06-01 22:08:47.000000 pyscf-2.6.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-06-01 22:08:54.755082 pyscf-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-06-01 22:08:47.000000 pyscf-2.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.547077 pyscf-2.6.0/pyscf/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/__all__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/__config__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.551077 pyscf-2.6.0/pyscf/adc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/adc/dfadc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15076 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/adc/radc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29868 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/adc/radc_amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/adc/radc_ao2mo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43387 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/adc/radc_ea.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38433 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/adc/radc_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44715 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/adc/radc_ip_cvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15399 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/adc/uadc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41215 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/adc/uadc_amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22683 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/adc/uadc_ao2mo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89288 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/adc/uadc_ea.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81944 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/adc/uadc_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110124 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/adc/uadc_ip_cvs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.551077 pyscf-2.6.0/pyscf/agf2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/agf2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18199 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/agf2/_agf2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22821 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/agf2/aux_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/agf2/chempot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/agf2/chkfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/agf2/dfragf2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/agf2/dfuagf2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/agf2/mpi_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36377 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/agf2/ragf2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/agf2/ragf2_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36449 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/agf2/uagf2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10447 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/agf2/uagf2_slow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.551077 pyscf-2.6.0/pyscf/ao2mo/
+-rw-r--r--   0 runner    (1001) docker     (127)    20567 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/ao2mo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11212 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/ao2mo/_ao2mo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7708 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/ao2mo/addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/ao2mo/incore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/ao2mo/nrr_outcore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34252 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/ao2mo/outcore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/ao2mo/r_outcore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13157 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/ao2mo/semi_incore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.559077 pyscf-2.6.0/pyscf/cc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/_ccsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/bccd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/ccd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68956 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/ccsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17726 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/ccsd_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21249 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/ccsd_rdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/ccsd_rdm_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11081 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/ccsd_t.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/ccsd_t_lambda_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/ccsd_t_rdm_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/ccsd_t_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/dfccsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25619 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/eom_gccsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81419 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/eom_rccsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)   117956 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/eom_uccsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22377 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/gccsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/gccsd_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10804 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/gccsd_rdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/gccsd_t.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/gccsd_t_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/gccsd_t_rdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/gccsd_t_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9609 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/gintermediates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28323 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/momgfccsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14466 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/qcisd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/qcisd_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/qcisd_t.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/qcisd_t_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16241 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/rccsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/rccsd_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44692 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/rccsd_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12025 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/rintermediates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58483 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/uccsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23359 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/uccsd_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27641 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/uccsd_rdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29028 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/uccsd_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18576 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/uccsd_t.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/uccsd_t_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/uccsd_t_rdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9259 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/uccsd_t_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38860 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/uintermediates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/cc/uintermediates_slow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.563077 pyscf-2.6.0/pyscf/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/ci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/ci/addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44286 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/ci/cisd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18108 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/ci/gcisd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38974 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/ci/ucisd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.563077 pyscf-2.6.0/pyscf/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37852 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/data/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/data/gyro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/data/gyromagnetic_ratio.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/data/nist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23505 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/data/nuclear_g_factor.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/data/nucprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13797 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/data/radii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/data/solvents.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.563077 pyscf-2.6.0/pyscf/df/
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14048 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/df.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21735 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/df_jk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.567077 pyscf-2.6.0/pyscf/df/grad/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/grad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26214 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/grad/casdm2_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/grad/casscf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21559 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/grad/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/grad/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/grad/rohf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/grad/roks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17477 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/grad/sacasscf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/grad/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/grad/uks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.567077 pyscf-2.6.0/pyscf/df/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22412 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/hessian/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/hessian/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25220 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/hessian/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/hessian/uks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/incore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12439 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/outcore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/df/r_incore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.575077 pyscf-2.6.0/pyscf/dft/
+-rw-r--r--   0 runner    (1001) docker     (127)   164350 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/LebedevGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/dft_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/dks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24192 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/gen_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/gen_libxc_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/gen_xcfun_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/gks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/gks_symm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   122701 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/libxc.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119618 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/numint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/numint2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29777 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/r_numint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/radi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20133 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/rks_symm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/roks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/sap.py
+-rw-r--r--   0 runner    (1001) docker     (127)  3933728 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/sap_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/uks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/uks_symm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.575077 pyscf-2.6.0/pyscf/dft/xc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/xc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/xc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23140 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/xc_deriv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39251 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/dft/xcfun.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.579078 pyscf-2.6.0/pyscf/eph/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/eph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/eph/eph_fd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/eph/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/eph/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/eph/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/eph/uks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.579078 pyscf-2.6.0/pyscf/fci/
+-rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27266 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16832 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/cistring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15408 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/direct_ep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/direct_nosym.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18153 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/direct_spin0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/direct_spin0_symm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40884 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/direct_spin1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24755 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/direct_spin1_cyl_sym.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33137 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/direct_spin1_symm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/direct_uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/fci_dhf_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/fci_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15210 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/rdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42090 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/selected_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16283 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/selected_ci_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/selected_ci_spin0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/selected_ci_spin0_symm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13363 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/selected_ci_symm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/fci/spin_op.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.583078 pyscf-2.6.0/pyscf/geomopt/
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/geomopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/geomopt/addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/geomopt/berny_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/geomopt/geometric_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/geomopt/log.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.587078 pyscf-2.6.0/pyscf/grad/
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/casci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/casscf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17917 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/ccsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13169 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/ccsd_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/ccsd_t.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/cisd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10751 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/dhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/lagrange.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/mp2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17028 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23745 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/rohf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/roks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41710 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/sacasscf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/tdrhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14982 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/tdrks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/tduhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16963 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/tduks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21754 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/uccsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/uccsd_t.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/ucisd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10992 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/uks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/grad/ump2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.587078 pyscf-2.6.0/pyscf/gto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.643079 pyscf-2.6.0/pyscf/gto/basis/
+-rw-r--r--   0 runner    (1001) docker     (127)   137396 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/Burkatzi-Filippi-Dolg-PP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    47103 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/DgaussA1_dft_cfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    47104 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/DgaussA1_dft_xfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    22868 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/DgaussA2_dft_cfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    22870 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/DgaussA2_dft_xfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    31249 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   141928 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/adzp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    83566 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ahlrichs_cfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)  1389925 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ano.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   127274 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aqzp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   108802 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/atzp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pV5Z-PP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   124241 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pV5Z_MP2FIT.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pVDZ-PP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   134863 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pVQZ-DK3.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pVQZ-PP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   108901 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pVQZ_MP2FIT.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   110807 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pVTZ-DK3.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pVTZ-PP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   190050 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pv5z-dk.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    53483 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pv5z-jkfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    97411 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pv5z-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   190020 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pv5z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   117453 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvdpdz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    98649 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvdz-dk.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    41742 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvdz-jkfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    30634 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvdz-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    98569 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvdz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    40752 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvdzp-jkfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    29379 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvdzp-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   290273 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvqz-dk.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    48952 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvqz-jkfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    48083 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvqz-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   155183 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvqz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   314115 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvtz-dk.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    45670 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvtz-jkfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    39435 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvtz-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   122314 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvtz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   346258 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwCVQZ-DK.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   183629 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwCVQZ-DK3.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   410566 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwCVTZ-DK.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   139736 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwCVTZ-DK3.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   124542 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwCVTZ_MP2FIT.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   182677 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwcv5z-dk.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   363886 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwcv5z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    37069 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwcvdz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   285250 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwcvqz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   192834 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwcvtz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    48451 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-pc-0.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   112718 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-pc-1.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   173735 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-pc-2.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   267909 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-pc-3.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   390219 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-pc-4.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    87863 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-pcseg-0.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   122797 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-pcseg-1.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   194490 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-pcseg-2.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   312944 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-pcseg-3.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   437986 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/aug-pcseg-4.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/bfd_pp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    46296 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/bfd_v5z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    31518 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/bfd_vdz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    65568 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/bfd_vqz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    57266 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/bfd_vtz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/bse.py
+-rw-r--r--   0 runner    (1001) docker     (127)   200095 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pCV5Z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    54500 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pCV6Z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pCVDZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pCVQZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pCVTZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   103871 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pV5Z_MP2FIT.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pVDZ-PP-NR.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   114741 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pVQZ-DK3.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    90211 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pVQZ_MP2FIT.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    93193 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pVTZ-DK3.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pVTZ-PP-NR.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   189349 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pv5z-dk.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    45383 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pv5z-jkfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   222905 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pv5z-pp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    41961 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pv5z-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   194433 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pv5z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   115228 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pvdpdz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   377366 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pvdz-dk.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    36718 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pvdz-jkfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    94731 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pvdz-pp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    30544 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pvdz-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    94827 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pvdz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    11311 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pvdz_fit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   850318 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pvqz-dk.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    41794 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pvqz-jkfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   177582 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pvqz-pp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    48631 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pvqz-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   149280 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pvqz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   914722 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pvtz-dk.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    39454 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pvtz-jkfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   132320 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pvtz-pp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    39711 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pvtz-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   117771 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pvtz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pvtz_fit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   106072 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pwCV5Z-DK.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    98164 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pwCV5Z-PP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   232487 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pwCV5Z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    53340 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pwCVDZ-DK.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pwCVDZ-PP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    18284 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pwCVDZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   241499 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pwCVQZ-DK.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   160567 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pwCVQZ-DK3.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    32332 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pwCVQZ-PP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    84240 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pwCVQZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   240607 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pwCVTZ-DK.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   120526 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pwCVTZ-DK3.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    22290 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pwCVTZ-PP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    99466 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pwCVTZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   104732 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/cc-pwCVTZ_MP2FIT.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.535076 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.647079 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    80494 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pV5Z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    36684 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pV6Z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    41351 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pVDZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    66515 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pVQZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    53428 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pVTZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    75421 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pV5Z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    34550 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pV6Z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    38752 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pVDZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    62219 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pVQZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    49967 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pVTZ.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.651079 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    13000 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_aug-cc-pV5Z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_aug-cc-pV6Z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_aug-cc-pVDZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_aug-cc-pVQZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10426 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_aug-cc-pVTZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    11812 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_cc-pV5Z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_cc-pV6Z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_cc-pVDZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_cc-pVQZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_cc-pVTZ.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.651079 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_aug-cc-pV5Z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_aug-cc-pVDZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_aug-cc-pVQZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_aug-cc-pVTZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_cc-pV5Z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_cc-pVDZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_cc-pVQZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_cc-pVTZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   262035 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/crenbl.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   129690 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/crenbs.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/crystal-cc-pvdz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    37024 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-qzvp-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   180299 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-qzvp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   185113 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-qzvpd.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    43496 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-qzvpp-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   184475 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-qzvpp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    45242 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-qzvppd-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   189343 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-qzvppd.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    57404 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-svp-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   110762 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-svp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    60367 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-svpd-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   117659 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-svpd.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    71708 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-tzvp-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   132134 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-tzvp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    74591 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-tzvpd-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   138427 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-tzvpd.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    59466 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-tzvpp-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   136623 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-tzvpp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    62380 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-tzvppd-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   142965 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-tzvppd.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   130384 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-universal-jfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   235329 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/def2-universal-jkfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    47198 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/demon_cfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/dyall_dz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/dyall_qz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13052 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/dyall_tz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/dz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   131530 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/dzp-dkh.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   132516 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/dzp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/dzp_dunning.py
+-rw-r--r--   0 runner    (1001) docker     (127)   178866 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/dzvp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    71969 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/dzvp2.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.655079 pyscf-2.6.0/pyscf/gto/basis/f12-basis/
+-rw-r--r--   0 runner    (1001) docker     (127)    20014 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/f12-basis/aug-cc-pV5Z-OptRI.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/f12-basis/aug-cc-pVDZ-OptRI.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    17248 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/f12-basis/aug-cc-pVQZ-OptRI.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    15259 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/f12-basis/aug-cc-pVTZ-OptRI.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    28721 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pCVDZ-F12-OptRI.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    26437 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pCVQZ-F12-OptRI.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    25757 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pCVTZ-F12-OptRI.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    56899 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pV5Z-F12.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pV5Z-F12rev2.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    12587 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pVDZ-F12-OptRI.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    26302 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pVDZ-F12-nZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pVDZ-F12rev2.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    13769 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pVQZ-F12-OptRI.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    48697 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pVQZ-F12-nZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pVQZ-F12rev2.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pVTZ-F12-OptRI.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    35324 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pVTZ-F12-nZ.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pVTZ-F12rev2.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/faegre_dz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43856 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/heavy-aug-cc-pvdz-jkfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    30481 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/heavy-aug-cc-pvdz-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    47735 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/heavy-aug-cc-pvtz-jkfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    39167 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/heavy-aug-cc-pvtz-ri.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/iglo3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92388 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/lanl08.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   109544 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/lanl2dz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    52603 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/lanl2tz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   117876 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/minao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/parse_bfd_pp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/parse_cp2k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/parse_cp2k_pp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/parse_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/parse_molpro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/parse_nwchem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/parse_nwchem_ecp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35344 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pc-0.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    82701 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pc-1.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   132372 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pc-2.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   211146 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pc-3.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   315764 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pc-4.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    65047 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pcseg-0.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    91188 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pcseg-1.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   150241 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pcseg-2.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   250673 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pcseg-3.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   357977 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pcseg-4.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    35826 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pob-tzvp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pob-tzvpp.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.663080 pyscf-2.6.0/pyscf/gto/basis/pople-basis/
+-rw-r--r--   0 runner    (1001) docker     (127)    55204 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/3-21++G.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    55937 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/3-21++Gs.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/3-21G-diffuse.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/3-21G-polarization.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    53526 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/3-21G.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    54234 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/3-21Gs.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/4-31G.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    36010 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31++G.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    21162 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31++Gs.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    38362 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31++Gss.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    21734 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31+G.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    20062 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31+Gs.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    22947 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31+Gss.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    20190 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311++G.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311++Gs.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    34756 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311++Gss.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    20634 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311+G.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    22361 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311+Gs.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    22104 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311+Gss.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311G-diffuse.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311G-polarization-2d.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311G-polarization-2p.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311G-polarization-3d.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311G-polarization-3p.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311G-polarization-d.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311G-polarization-f.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311G-polarization-p.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    31263 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311G.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    33384 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311Gs.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    33056 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311Gss.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31G-diffuse.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31G-polarization-2d.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31G-polarization-2p.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31G-polarization-3d.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31G-polarization-3p.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31G-polarization-d.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31G-polarization-f.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31G-polarization-p.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    34316 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31G.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    44932 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31Gs.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    36668 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31Gss.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   117420 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/qzp-dkh.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   117314 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/qzp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   139676 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/roos-dz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   169498 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/roos-tz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   142994 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/sarc-dkh2.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    72840 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/sbkjc.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.663080 pyscf-2.6.0/pyscf/gto/basis/soecp/
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/soecp/ECPDS10MDFSO.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    12273 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/soecp/ECPDS28MDFSO.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/soecp/ECPDS28MWBSO.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/soecp/ECPDS46MDFSO.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/soecp/ECPDS60MDFSO.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/soecp/ECPDS60MWBSO.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/soecp/ECPDS78MDFSO.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/soecp/ECPDS92MDFBQSO.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10955 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/soecp/ECPDS92MDFBSO.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    49513 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/sto-3g.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    50158 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/sto-6g.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    70653 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/stuttgart_dz.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   140417 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/stuttgart_rsc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   100829 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/tzp-dkh.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   100810 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/tzp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    48273 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/tzv.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   130384 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/basis/weigend_cfit.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/cmd_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/ecp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/eval_gto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/ft_ao.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146622 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/mole.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38020 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/moleintor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gto/pp_int.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.667080 pyscf-2.6.0/pyscf/gw/
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15523 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gw/gw_ac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gw/gw_cd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14559 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gw/gw_exact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gw/gw_slow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13237 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gw/rpa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18642 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gw/ugw_ac.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7309 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/gw/urpa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.667080 pyscf-2.6.0/pyscf/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/hessian/dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26493 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/hessian/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25552 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/hessian/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14633 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/hessian/thermo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21117 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/hessian/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35620 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/hessian/uks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.671080 pyscf-2.6.0/pyscf/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)    11165 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.671080 pyscf-2.6.0/pyscf/lib/agf2/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/agf2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13242 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/agf2/ragf2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/agf2/ragf2.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12519 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/agf2/uagf2.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.671080 pyscf-2.6.0/pyscf/lib/ao2mo/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/ao2mo/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    46111 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/ao2mo/nr_ao2mo.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/ao2mo/nr_ao2mo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/ao2mo/nr_incore.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/ao2mo/nr_incore.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10926 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/ao2mo/nrr_ao2mo.c
+-rw-r--r--   0 runner    (1001) docker     (127)    34149 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/ao2mo/r_ao2mo.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/ao2mo/r_ao2mo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/ao2mo/restore_eri.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.671080 pyscf-2.6.0/pyscf/lib/cc/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/cc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/cc/ccsd_grad.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/cc/ccsd_pack.c
+-rw-r--r--   0 runner    (1001) docker     (127)    45611 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/cc/ccsd_t.c
+-rw-r--r--   0 runner    (1001) docker     (127)    36526 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/cc/uccsd_t.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/chkfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/config.h.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.675080 pyscf-2.6.0/pyscf/lib/dft/
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   173239 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/CxLebedevGrid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/grid_basis.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/grid_basis.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22950 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/grid_collocate.c
+-rw-r--r--   0 runner    (1001) docker     (127)    19133 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/grid_common.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/grid_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    47159 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/grid_integrate.c
+-rw-r--r--   0 runner    (1001) docker     (127)    44950 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/libxc_itrf.c
+-rw-r--r--   0 runner    (1001) docker     (127)    20720 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/multigrid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/multigrid.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/nr_numint.c
+-rw-r--r--   0 runner    (1001) docker     (127)    54245 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/nr_numint_sparse.c
+-rw-r--r--   0 runner    (1001) docker     (127)   105128 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/numint_uniform_grid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/r_numint.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/utils.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/xc_deriv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/dft/xcfun_itrf.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12071 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/diis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.679080 pyscf-2.6.0/pyscf/lib/gto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.679080 pyscf-2.6.0/pyscf/lib/gto/autocode/
+-rw-r--r--   0 runner    (1001) docker     (127)    57483 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/autocode/auto_eval1.c
+-rw-r--r--   0 runner    (1001) docker     (127)    26701 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/deriv1.c
+-rw-r--r--   0 runner    (1001) docker     (127)    63100 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/deriv2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/fastexp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/fill_grids_int2c.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/fill_int2c.c
+-rw-r--r--   0 runner    (1001) docker     (127)    24491 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/fill_int2e.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/fill_nr_3c.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/fill_r_3c.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/fill_r_4c.c
+-rw-r--r--   0 runner    (1001) docker     (127)    51411 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/ft_ao.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/ft_ao.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/ft_ao_deriv.c
+-rw-r--r--   0 runner    (1001) docker     (127)    20944 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/grid_ao_drv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/grid_ao_drv.h
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/gto.h
+-rw-r--r--   0 runner    (1001) docker     (127)  1014868 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/nr_ecp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/nr_ecp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    45488 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/gto/nr_ecp_deriv.c
+-rw-r--r--   0 runner    (1001) docker     (127)    61502 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/linalg_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.683080 pyscf-2.6.0/pyscf/lib/mcscf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/mcscf/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/mcscf/fci.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23910 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/mcscf/fci_4pdm.c
+-rw-r--r--   0 runner    (1001) docker     (127)    41828 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/mcscf/fci_contract.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/mcscf/fci_contract_nosym.c
+-rw-r--r--   0 runner    (1001) docker     (127)    30335 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/mcscf/fci_rdm.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14569 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/mcscf/fci_string.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9579 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/mcscf/nevpt_contract.c
+-rw-r--r--   0 runner    (1001) docker     (127)    25231 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/mcscf/select_ci.c
+-rw-r--r--   0 runner    (1001) docker     (127)    48287 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.683080 pyscf-2.6.0/pyscf/lib/np_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/np_helper/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/np_helper/condense.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/np_helper/np_helper.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/np_helper/np_helper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/np_helper/npdot.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/np_helper/omp_reduce.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/np_helper/pack_tril.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/np_helper/transpose.c
+-rw-r--r--   0 runner    (1001) docker     (127)    46180 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/numpy_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.687080 pyscf-2.6.0/pyscf/lib/pbc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/cell.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/cell.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14428 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/cint2e.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14523 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/cint3c2e.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/fft.c
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/fft.h
+-rw-r--r--   0 runner    (1001) docker     (127)    58318 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/fill_ints.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/fill_ints.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40928 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/fill_ints_screened.c
+-rw-r--r--   0 runner    (1001) docker     (127)    77592 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/fill_ints_sr.c
+-rw-r--r--   0 runner    (1001) docker     (127)    36806 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/ft_ao.c
+-rw-r--r--   0 runner    (1001) docker     (127)    30687 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/grid_ao.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/hf_grad.c
+-rw-r--r--   0 runner    (1001) docker     (127)    31483 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/inner_dot.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/neighbor_list.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/neighbor_list.h
+-rw-r--r--   0 runner    (1001) docker     (127)    50426 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/nr_direct.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/nr_ecp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/optimizer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/optimizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/pbc.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14899 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/pp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/symmetry.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14078 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/pbc/transform_mo.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.687080 pyscf-2.6.0/pyscf/lib/ri/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/ri/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/ri/r_df_incore.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/scipy_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.687080 pyscf-2.6.0/pyscf/lib/solvent/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/solvent/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.691080 pyscf-2.6.0/pyscf/lib/vhf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/cvhf.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/fblas.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/fill_nr_s8.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13464 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/hessian_screen.c
+-rw-r--r--   0 runner    (1001) docker     (127)    26469 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/nr_direct.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/nr_direct.h
+-rw-r--r--   0 runner    (1001) docker     (127)   135778 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/nr_direct_dot.c
+-rw-r--r--   0 runner    (1001) docker     (127)    29999 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/nr_incore.c
+-rw-r--r--   0 runner    (1001) docker     (127)    20984 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/nr_sgx_direct.c
+-rw-r--r--   0 runner    (1001) docker     (127)    41654 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/nr_sr_vhf.c
+-rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/optimizer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/optimizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24284 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/r_direct_dot.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/r_direct_dot.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12689 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/r_direct_o1.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14446 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/rah_direct_dot.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/rha_direct_dot.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/rkb_screen.c
+-rw-r--r--   0 runner    (1001) docker     (127)    25499 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/time_rev.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lib/vhf/time_rev.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.691080 pyscf-2.6.0/pyscf/lo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lo/boys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lo/cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lo/edmiston.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lo/iao.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16583 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lo/ibo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lo/nao.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lo/orth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11596 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lo/pipek.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lo/pipek_jacobi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/lo/vvo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.695080 pyscf-2.6.0/pyscf/mcscf/
+-rw-r--r--   0 runner    (1001) docker     (127)    20800 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/PiOS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11555 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63576 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/apc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10115 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/avas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49472 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/casci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/casci_symm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/chkfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16428 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/dmet_cas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59699 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/mc1step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/mc1step_symm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7967 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/mc2step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/mc_ao2mo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39340 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/newton_casscf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/newton_casscf_symm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20212 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/ucasci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37857 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/umc1step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/umc2step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mcscf/umc_ao2mo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.695080 pyscf-2.6.0/pyscf/md/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/md/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/md/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21000 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/md/integrators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.699080 pyscf-2.6.0/pyscf/mp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mp/dfgmp2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mp/dfmp2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30590 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mp/dfmp2_native.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26289 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mp/dfump2_native.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14989 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mp/gmp2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31992 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mp/mp2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mp/mp2f12_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31638 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mp/ump2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.699080 pyscf-2.6.0/pyscf/mrpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mrpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43034 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/mrpt/nevpt2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.699080 pyscf-2.6.0/pyscf/nac/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/nac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13593 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/nac/sacasscf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.699080 pyscf-2.6.0/pyscf/pbc/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/__all__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.699080 pyscf-2.6.0/pyscf/pbc/adc/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/adc/dfadc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13136 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/adc/kadc_ao2mo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11411 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/adc/kadc_rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/adc/kadc_rhf_amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62323 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/adc/kadc_rhf_ea.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46652 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/adc/kadc_rhf_ip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.699080 pyscf-2.6.0/pyscf/pbc/ao2mo/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/ao2mo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/ao2mo/eris.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.703080 pyscf-2.6.0/pyscf/pbc/cc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/ccsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82519 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/eom_kccsd_ghf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68243 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/eom_kccsd_rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/eom_kccsd_rhf_ea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/eom_kccsd_rhf_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57971 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/eom_kccsd_uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35096 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/kccsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50357 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/kccsd_rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31944 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/kccsd_rhf_ksymm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15664 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/kccsd_t.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28804 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/kccsd_t_rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/kccsd_t_rhf_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48978 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/kccsd_uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22273 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/kintermediates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42214 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/kintermediates_rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/kintermediates_rhf_ksymm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/kintermediates_uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/cc/kuccsd_rdm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.703080 pyscf-2.6.0/pyscf/pbc/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/ci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/ci/cisd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26419 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/ci/kcis_rhf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.707080 pyscf-2.6.0/pyscf/pbc/df/
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28912 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/aft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17682 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/aft_ao2mo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31914 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/aft_jk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34033 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/df.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/df_ao2mo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68786 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/df_jk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13997 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/fft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/fft_ao2mo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/fft_jk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32436 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/ft_ao.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45554 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/gdf_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27818 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/incore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18262 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/mdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/mdf_ao2mo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/mdf_jk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/outcore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29064 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/rsdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69541 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/rsdf_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53162 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/rsdf_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/df/rsdf_jk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.711081 pyscf-2.6.0/pyscf/pbc/dft/
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/cdft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/gen_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/gks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/kgks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/krks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/krks_ksymm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/krkspu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/krkspu_ksymm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/kroks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/kuks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/kuks_ksymm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/kukspu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/kukspu_ksymm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.711081 pyscf-2.6.0/pyscf/pbc/dft/multigrid/
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/multigrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73827 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/multigrid/multigrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49778 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/multigrid/multigrid_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/multigrid/pp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/multigrid/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51773 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/numint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26935 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/numint2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13310 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/roks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/dft/uks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.711081 pyscf-2.6.0/pyscf/pbc/eph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/eph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/eph/eph_fd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.711081 pyscf-2.6.0/pyscf/pbc/geomopt/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/geomopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/geomopt/geometric_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.715081 pyscf-2.6.0/pyscf/pbc/grad/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/grad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17510 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/grad/krhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/grad/krks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/grad/kuhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/grad/kuks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/grad/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/grad/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/grad/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/grad/uks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.715081 pyscf-2.6.0/pyscf/pbc/gto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/_pbcintor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.719081 pyscf-2.6.0/pyscf/pbc/gto/basis/
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-aug-dzvp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-aug-qzv2p.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-aug-qzv3p.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-aug-tzv2p.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-aug-tzvp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-cc-dzvp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-cc-qzvp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-cc-tzvp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-dzv.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-dzvp-molopt-sr-q9.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    53413 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-dzvp-molopt-sr.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-dzvp-molopt.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10728 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-dzvp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    18881 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-qzv2p.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    20609 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-qzv3p.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-szv-molopt-sr-q9.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    31790 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-szv-molopt-sr.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-szv-molopt.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-szv.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-szvp-molopt-sr-q9.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-tzv2p-molopt.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-tzv2p.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-tzv2px-molopt.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-tzvp-molopt.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/gth-tzvp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/split_BASIS_MOLOPT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/split_GTH_BASIS_SETS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/basis/split_HFX_BASIS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67489 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/ecp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/eval_gto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10613 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/ewald_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/neighborlist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.723081 pyscf-2.6.0/pyscf/pbc/gto/pseudo/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/pseudo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24006 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-blyp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    14867 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-bp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-hcth120.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-hcth407.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    90523 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-hf-rev.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-hf.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-olyp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    54113 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-pade.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    42074 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-pbe.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-pbesol.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/pseudo/pp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24021 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/pseudo/pp_int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gto/pseudo/split_GTH_POTENTIALS.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.723081 pyscf-2.6.0/pyscf/pbc/gw/
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gw/gw_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gw/kgw_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gw/kgw_slow_supercell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23938 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gw/krgw_ac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26680 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gw/krgw_cd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31709 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/gw/kugw_ac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.723081 pyscf-2.6.0/pyscf/pbc/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/lib/arnoldi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/lib/chkfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41502 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/lib/kpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21741 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/lib/kpts_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12221 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/lib/ktensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29306 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/lib/linalg_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.727081 pyscf-2.6.0/pyscf/pbc/mp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/mp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30978 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/mp/kmp2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/mp/kmp2_ksymm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16730 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/mp/kmp2_stagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17429 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/mp/kump2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/mp/mp2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.727081 pyscf-2.6.0/pyscf/pbc/mpicc/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/mpicc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   160408 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/mpicc/kccsd_rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70288 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/mpicc/kintermediates_rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/mpicc/mpi_kpoint_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.727081 pyscf-2.6.0/pyscf/pbc/mpitools/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/mpitools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/mpitools/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/mpitools/mpi_blksize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/mpitools/mpi_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/mpitools/mpi_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/mpitools/mpi_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.731081 pyscf-2.6.0/pyscf/pbc/scf/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/_response_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21121 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/chkfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/cphf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/ghf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34227 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/kghf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/kghf_ksymm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28390 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/khf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15072 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/khf_ksymm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15222 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/krohf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23003 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/kuhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9288 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/kuhf_ksymm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/newton_ah.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/rohf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61499 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/rsjk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/scfint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11808 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/stability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9322 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/scf/uhf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.731081 pyscf-2.6.0/pyscf/pbc/symm/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/symm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/symm/basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/symm/geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14926 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/symm/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/symm/pyscf_spglib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12557 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/symm/space_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/symm/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/symm/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.731081 pyscf-2.6.0/pyscf/pbc/tddft/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tddft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.735081 pyscf-2.6.0/pyscf/pbc/tdscf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tdscf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tdscf/kproxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26753 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tdscf/kproxy_supercell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16962 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tdscf/krhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tdscf/krhf_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tdscf/krhf_slow_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tdscf/krhf_slow_supercell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tdscf/krks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14816 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tdscf/kuhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tdscf/kuks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tdscf/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tdscf/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tdscf/rhf_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tdscf/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tdscf/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tdscf/uks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.735081 pyscf-2.6.0/pyscf/pbc/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tools/k2gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tools/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tools/make_test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28920 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tools/pbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tools/print_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tools/pyscf_ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52879 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tools/pywannier90.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/tools/tril.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.735081 pyscf-2.6.0/pyscf/pbc/x2c/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/x2c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/x2c/sfx2c1e.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/pbc/x2c/x2c1e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/post_scf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.739081 pyscf-2.6.0/pyscf/qmmm/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/qmmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16248 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/qmmm/itrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/qmmm/mm_mole.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.743081 pyscf-2.6.0/pyscf/scf/
+-rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11746 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/_response_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30113 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/_vhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48927 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/atom_hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/atom_hf_pp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/atom_ks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/chkfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/cphf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36522 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/dhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/diis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20443 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/ghf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12872 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/ghf_symm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80773 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39111 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/hf_symm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/jk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19972 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/rohf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24292 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/stability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/stability_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/ucphf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42218 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23392 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/scf/uhf_symm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.743081 pyscf-2.6.0/pyscf/sgx/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/sgx/sgx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13133 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/sgx/sgx_jk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.743081 pyscf-2.6.0/pyscf/solvent/
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/solvent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26898 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/solvent/_attach_solvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57130 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/solvent/_ddcosmo_tdscf_grad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36308 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/solvent/ddcosmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13486 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/solvent/ddpcm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.743081 pyscf-2.6.0/pyscf/solvent/grad/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/solvent/grad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14715 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/solvent/grad/ddcosmo_grad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/solvent/grad/pcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/solvent/grad/smd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/solvent/grad/smd_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.743081 pyscf-2.6.0/pyscf/solvent/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/solvent/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/solvent/hessian/pcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/solvent/hessian/smd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/solvent/hessian/smd_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16565 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/solvent/pcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18233 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/solvent/pol_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22579 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/solvent/smd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/solvent/smd_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.747081 pyscf-2.6.0/pyscf/soscf/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/soscf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12242 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/soscf/ciah.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41251 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/soscf/newton_ah.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.747081 pyscf-2.6.0/pyscf/symm/
+-rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/symm/Dmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/symm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24620 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/symm/addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25106 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/symm/basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/symm/cg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34171 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/symm/geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/symm/msym.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/symm/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/symm/sph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.747081 pyscf-2.6.0/pyscf/tddft/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tddft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.747081 pyscf-2.6.0/pyscf/tdscf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tdscf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23914 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tdscf/common_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28144 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tdscf/dhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tdscf/dks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25542 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tdscf/ghf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tdscf/gks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tdscf/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39799 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tdscf/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tdscf/rhf_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tdscf/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34445 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tdscf/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8816 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tdscf/uks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.751082 pyscf-2.6.0/pyscf/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tools/c60struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9509 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tools/chgcar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tools/chkfile_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14652 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tools/cubegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tools/dump_mat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14567 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tools/fcidump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tools/mo_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tools/molden.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tools/ring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/tools/wfn_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.751082 pyscf-2.6.0/pyscf/x2c/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/x2c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/x2c/_response_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/x2c/dft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/x2c/newton_ah.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11025 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/x2c/sfx2c1e.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/x2c/sfx2c1e_grad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/x2c/sfx2c1e_hess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/x2c/stability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15442 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/x2c/tdscf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36312 2024-06-01 22:08:47.000000 pyscf-2.6.0/pyscf/x2c/x2c.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:08:54.751082 pyscf-2.6.0/pyscf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-06-01 22:08:54.000000 pyscf-2.6.0/pyscf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    29277 2024-06-01 22:08:54.000000 pyscf-2.6.0/pyscf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 22:08:54.000000 pyscf-2.6.0/pyscf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-06-01 22:08:54.000000 pyscf-2.6.0/pyscf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-01 22:08:54.000000 pyscf-2.6.0/pyscf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:08:54.755082 pyscf-2.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4488 2024-06-01 22:08:47.000000 pyscf-2.6.0/setup.py
```

### Comparing `pyscf-2.5.0/CHANGELOG` & `pyscf-2.6.0/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+PySCF 2.6.0 (2024-06-01)
+------------------------
+* Added
+  - SMD and PCM solvent model
+  - Nuclear Hessian for SMD and PCM solvent models
+* Improved
+  - DFT-D3 and DFT-D4 interfaces. Supporting assigning the acronym such as
+    WB97M-D3BJ, WB97M-D4 to the xc attribute.
+  - Optimized density fitting performance.
+  - Memory usage for RPA.
+  - FCI coefficients transformation for more than 64 orbitals.
+  - Multi-grid DFT performance greatly optimized.
+* Fixes
+  - CASCI/CASSCF calculations when mixing C1 symmetry and symmetry=False .
+  - "atom" initial guess for ECP with super-heavy atoms.
+  - Complex conjugation issues in single k-point JK-build in PBC DF.
+  - CCSD(T) for complex orbitals.
+  - Dipole moment in SFX2C.
+  - High-order XC derivatives.
+  - Integer overflow in FCI large address.
+  - Multi-collinear XC higher order derivatives.
+  - Smearing with predefined chemical potential.
+  - Fix frozen attribute for MP2 density matrices.
+
+
 PySCF 2.5.0 (2024-02-03)
 ------------------------
 * Added
   - SA-CASSCF Nonadiabatic Coupling Vectors 
   - The to_gpu function to convert pyscf objects to gpu4pyscf objects.
   - 4th, and 5th order XC derivatives.
 * Improved
```

### Comparing `pyscf-2.5.0/LICENSE` & `pyscf-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/MANIFEST.in` & `pyscf-2.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/NOTICE` & `pyscf-2.6.0/NOTICE`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,18 @@
 Pavel Pokhilko
 Frédéric Chapoton
 Daniel King
 Jiachen Li
 Felipe S. S. Schneider
 Aniruddha Seal
 Peter Reinholdt
+Christopher Hillenbrand
+scohenjanes5
+Michal Krompiec
+Victor Yu
 
 
 ---
 * This list is not the contribution order. The order is roughly based on the
   time of the first commit from each contributor.
 * Affiliations may not be the present affiliation of each contributor. If you
   wish to update your affiliation to any form you like, please write email to
```

### Comparing `pyscf-2.5.0/README.md` & `pyscf-2.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,40 +3,44 @@
 </div>
 
 Python-based Simulations of Chemistry Framework
 -----------------------------------------------
 [![Build Status](https://github.com/pyscf/pyscf/workflows/CI/badge.svg)](https://github.com/pyscf/pyscf/actions?query=workflow%3ACI)
 [![codecov](https://codecov.io/gh/pyscf/pyscf/branch/master/graph/badge.svg)](https://codecov.io/gh/pyscf/pyscf)
 
-2024-02-03
+2024-06-01
 
-* [Stable release 2.5.0](https://github.com/pyscf/pyscf/releases/tag/v2.5.0)
+* [Stable release 2.6.0](https://github.com/pyscf/pyscf/releases/tag/v2.6.0)
 * [Changelog](../master/CHANGELOG)
 * [Documentation](http://www.pyscf.org)
 * [Installation](#installation)
 * [Features](../master/FEATURES)
 
 
 # Installation
 
-* Install stable release
+* Install stable release:
 
         pip install pyscf
 
-* (Optionally) Extensions projects geomopt, dmrgscf, doci, fciqmc, icmpspt,
-  properties, semiempirical, shciscf ... (more on https://github.com/pyscf) can
-  be installed using pip
+* New features developed in recent years are available in the pyscf-forge package:
+
+        pip install pyscf-forge
+
+* Certain modules are maintained as extensions of PySCF, such as dispersion,
+  dmrgscf, fciqmc, icmpspt, properties, semiempirical, shciscf ... (more on
+  https://github.com/pyscf) can be installed using pip:
 
         pip install pyscf[all]
 
-  Install an individual extension
+  An individual extension can be installed:
 
-        pip install pyscf[geomopt]
+        pip install pyscf[dispersion]
 
-* More details of custom install can be found in
+* More details of custom installation can be found in
   [installation manual](http://pyscf.org/install.html#compiling-from-source-code)
 
 
 # Citing PySCF
 
 ## Base PySCF
 The following paper should be cited in publications utilizing the PySCF program package:
```

### Comparing `pyscf-2.5.0/pyscf/__all__.py` & `pyscf-2.6.0/pyscf/__all__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/__config__.py` & `pyscf-2.6.0/pyscf/__config__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/__init__.py` & `pyscf-2.6.0/pyscf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     >>> mol = pyscf.M(atom='H 0 0 0; H 0 0 1.2', basis='cc-pvdz')
     >>> mol.RHF().run()
     converged SCF energy = -1.06111199785749
     -1.06111199786
 
 '''
 
-__version__ = '2.5.0'
+__version__ = '2.6.0'
 
 import os
 import sys
 
 # Load modules which are developed as plugins of the namespace package
 PYSCF_EXT_PATH = os.getenv('PYSCF_EXT_PATH')
 if PYSCF_EXT_PATH:
```

### Comparing `pyscf-2.5.0/pyscf/adc/__init__.py` & `pyscf-2.6.0/pyscf/adc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/adc/dfadc.py` & `pyscf-2.6.0/pyscf/adc/dfadc.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/adc/radc.py` & `pyscf-2.6.0/pyscf/adc/radc.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/adc/radc_amplitudes.py` & `pyscf-2.6.0/pyscf/adc/radc_amplitudes.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/adc/radc_ao2mo.py` & `pyscf-2.6.0/pyscf/adc/radc_ao2mo.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/adc/radc_ea.py` & `pyscf-2.6.0/pyscf/adc/radc_ea.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/adc/radc_ip.py` & `pyscf-2.6.0/pyscf/adc/radc_ip.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/adc/radc_ip_cvs.py` & `pyscf-2.6.0/pyscf/adc/radc_ip_cvs.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/adc/uadc.py` & `pyscf-2.6.0/pyscf/adc/uadc.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/adc/uadc_amplitudes.py` & `pyscf-2.6.0/pyscf/adc/uadc_amplitudes.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/adc/uadc_ao2mo.py` & `pyscf-2.6.0/pyscf/adc/uadc_ao2mo.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/adc/uadc_ea.py` & `pyscf-2.6.0/pyscf/adc/uadc_ea.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/adc/uadc_ip.py` & `pyscf-2.6.0/pyscf/adc/uadc_ip.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/adc/uadc_ip_cvs.py` & `pyscf-2.6.0/pyscf/adc/uadc_ip_cvs.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/agf2/__init__.py` & `pyscf-2.6.0/pyscf/agf2/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/agf2/_agf2.py` & `pyscf-2.6.0/pyscf/agf2/_agf2.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/agf2/aux_space.py` & `pyscf-2.6.0/pyscf/agf2/aux_space.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/agf2/chempot.py` & `pyscf-2.6.0/pyscf/agf2/chempot.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/agf2/chkfile.py` & `pyscf-2.6.0/pyscf/agf2/chkfile.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/agf2/dfragf2.py` & `pyscf-2.6.0/pyscf/agf2/dfragf2.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/agf2/dfuagf2.py` & `pyscf-2.6.0/pyscf/agf2/dfuagf2.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/agf2/mpi_helper.py` & `pyscf-2.6.0/pyscf/agf2/mpi_helper.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/agf2/ragf2.py` & `pyscf-2.6.0/pyscf/agf2/ragf2.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/agf2/ragf2_slow.py` & `pyscf-2.6.0/pyscf/agf2/ragf2_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/agf2/uagf2.py` & `pyscf-2.6.0/pyscf/agf2/uagf2.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/agf2/uagf2_slow.py` & `pyscf-2.6.0/pyscf/agf2/uagf2_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/ao2mo/__init__.py` & `pyscf-2.6.0/pyscf/ao2mo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/ao2mo/_ao2mo.py` & `pyscf-2.6.0/pyscf/ao2mo/_ao2mo.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/ao2mo/addons.py` & `pyscf-2.6.0/pyscf/ao2mo/addons.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/ao2mo/incore.py` & `pyscf-2.6.0/pyscf/ao2mo/incore.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/ao2mo/nrr_outcore.py` & `pyscf-2.6.0/pyscf/ao2mo/nrr_outcore.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/ao2mo/outcore.py` & `pyscf-2.6.0/pyscf/ao2mo/outcore.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,24 +482,24 @@
     nkeys = len(h5group)
     dat = h5group['0']
     ncol = sum(h5group[str(key)].shape[-1] for key in range(nkeys))
     if dat.ndim == 2:
         out = numpy.ndarray((row1-row0, ncol), dat.dtype, buffer=out)
         col1 = 0
         for key in range(nkeys):
-            dat = h5group[str(key)][row0:row1]
-            col0, col1 = col1, col1 + dat.shape[1]
-            out[:,col0:col1] = dat
+            col0, col1 = col1, col1 + h5group[str(key)].shape[1]
+            h5group[str(key)].read_direct(out, dest_sel=numpy.s_[:,col0:col1],
+                                          source_sel=numpy.s_[row0:row1])
     else:  # multiple components
         out = numpy.ndarray((dat.shape[0], row1-row0, ncol), dat.dtype, buffer=out)
         col1 = 0
         for key in range(nkeys):
-            dat = h5group[str(key)][:,row0:row1]
-            col0, col1 = col1, col1 + dat.shape[2]
-            out[:,:,col0:col1] = dat
+            col0, col1 = col1, col1 + h5group[str(key)].shape[2]
+            h5group[str(key)].read_direct(out, dest_sel=numpy.s_[:,:,col0:col1],
+                                          source_sel=numpy.s_[:,row0:row1])
     return out
 
 def _transpose_to_h5g(h5group, key, dat, blksize, chunks=None):
     nrow, ncol = dat.shape
     dset = h5group.create_dataset(key, (ncol,nrow), 'f8', chunks=chunks)
     for col0, col1 in prange(0, ncol, blksize):
         dset[col0:col1] = lib.transpose(dat[:,col0:col1])
```

### Comparing `pyscf-2.5.0/pyscf/ao2mo/r_outcore.py` & `pyscf-2.6.0/pyscf/ao2mo/r_outcore.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/ao2mo/semi_incore.py` & `pyscf-2.6.0/pyscf/ao2mo/semi_incore.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/__init__.py` & `pyscf-2.6.0/pyscf/cc/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -190,23 +190,17 @@
             Threshold on NO occupation numbers. Default is 1e-6 (very conservative).
         pct_occ : float
             Percentage of total occupation number. Default is None. If present, overrides `thresh`.
         nvir_act : int
             Number of virtual NOs to keep. Default is None. If present, overrides `thresh` and `pct_occ`.
     """
     import numpy
-    if frozen is None:
-        frozenocc = 0
-    else:
-        assert(isinstance(frozen, (int,numpy.int64)))
-        frozenocc = frozen
     from pyscf import mp
-    pt = mp.MP2(mf).set(verbose=0).run()
+    pt = mp.MP2(mf, frozen=frozen).set(verbose=0).run()
     frozen, no_coeff = pt.make_fno(thresh=thresh, pct_occ=pct_occ, nvir_act=nvir_act)
-    frozen = numpy.hstack([numpy.arange(frozenocc),frozen])
     if len(frozen) == 0: frozen = None
     pt_no = mp.MP2(mf, frozen=frozen, mo_coeff=no_coeff).set(verbose=0).run()
     mycc = CCSD(mf, frozen=frozen, mo_coeff=no_coeff)
     mycc.delta_emp2 = pt.e_corr - pt_no.e_corr
     from pyscf.lib import logger
     def _finalize(self):
         '''Hook for dumping results and clearing up the object.'''
```

### Comparing `pyscf-2.5.0/pyscf/cc/_ccsd.py` & `pyscf-2.6.0/pyscf/cc/_ccsd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/addons.py` & `pyscf-2.6.0/pyscf/cc/addons.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/bccd.py` & `pyscf-2.6.0/pyscf/cc/bccd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/ccd.py` & `pyscf-2.6.0/pyscf/cc/ccd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/ccsd.py` & `pyscf-2.6.0/pyscf/cc/ccsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1236,14 +1236,23 @@
 
     def density_fit(self, auxbasis=None, with_df=None):
         raise NotImplementedError
 
     def nuc_grad_method(self):
         raise NotImplementedError
 
+    # to_gpu can be reused only when __init__ still takes mf
+    def to_gpu(self):
+        mf = self.base.to_gpu()
+        from importlib import import_module
+        mod = import_module(self.__module__.replace('pyscf', 'gpu4pyscf'))
+        cls = getattr(mod, self.__class__.__name__)
+        obj = cls(mf)
+        return obj
+
 class CCSD(CCSDBase):
     __doc__ = CCSDBase.__doc__
 
     def dump_flags(self, verbose=None):
         CCSDBase.dump_flags(self, verbose)
         if self.verbose >= logger.DEBUG1 and self.__class__ == CCSD:
             nocc = self.nocc
```

### Comparing `pyscf-2.5.0/pyscf/cc/ccsd_lambda.py` & `pyscf-2.6.0/pyscf/cc/ccsd_lambda.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/ccsd_rdm.py` & `pyscf-2.6.0/pyscf/cc/ccsd_rdm.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/ccsd_rdm_slow.py` & `pyscf-2.6.0/pyscf/cc/ccsd_rdm_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/ccsd_t.py` & `pyscf-2.6.0/pyscf/cc/ccsd_t.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
                 bufopv, buf1 = buf1, bufopv
             cpu1 = log.timer_debug1('transpose %d:%d'%(j0,j1), *cpu1)
 
     return orbsym
 
 def _sort_t2_vooo_(mycc, orbsym, t1, t2, eris):
     assert (t2.flags.c_contiguous)
-    vooo = numpy.asarray(eris.ovoo).transpose(1,0,3,2).conj().copy()
+    vooo = numpy.asarray(eris.ovoo).transpose(1,0,2,3).conj().copy()
     nocc, nvir = t1.shape
     if mycc.mol.symmetry:
         orbsym = numpy.asarray(orbsym, dtype=numpy.int32)
         o_sorted = _irrep_argsort(orbsym[:nocc])
         v_sorted = _irrep_argsort(orbsym[nocc:])
         mo_energy = eris.mo_energy
         mo_energy = numpy.hstack((mo_energy[:nocc][o_sorted],
```

### Comparing `pyscf-2.5.0/pyscf/cc/ccsd_t_lambda_slow.py` & `pyscf-2.6.0/pyscf/cc/ccsd_t_lambda_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/ccsd_t_rdm_slow.py` & `pyscf-2.6.0/pyscf/cc/ccsd_t_rdm_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/ccsd_t_slow.py` & `pyscf-2.6.0/pyscf/cc/ccsd_t_slow.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     nocc, nvir = t1.shape
     mo_e = eris.mo_energy
     e_occ, e_vir = mo_e[:nocc], mo_e[nocc:]
     eijk = lib.direct_sum('i,j,k->ijk', e_occ, e_occ, e_occ)
 
     eris_vvov = eris.get_ovvv().conj().transpose(1,3,0,2)
-    eris_vooo = numpy.asarray(eris.ovoo).conj().transpose(1,0,3,2)
+    eris_vooo = numpy.asarray(eris.ovoo).conj().transpose(1,0,2,3)
     eris_vvoo = numpy.asarray(eris.ovov).conj().transpose(1,3,0,2)
     fvo = eris.fock[nocc:,:nocc]
     def get_w(a, b, c):
         w = numpy.einsum('if,fkj->ijk', eris_vvov[a,b], t2T[c,:])
         w-= numpy.einsum('ijm,mk->ijk', eris_vooo[a,:], t2T[b,c])
         return w
     def get_v(a, b, c):
```

### Comparing `pyscf-2.5.0/pyscf/cc/dfccsd.py` & `pyscf-2.6.0/pyscf/cc/dfccsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,16 @@
     def ao2mo(self, mo_coeff=None):
         return _make_df_eris(self, mo_coeff)
 
     def _add_vvvv(self, t1, t2, eris, out=None, with_ovvv=False, t2sym=None):
         assert (not self.direct)
         return ccsd.CCSD._add_vvvv(self, t1, t2, eris, out, with_ovvv, t2sym)
 
+    to_gpu = lib.to_gpu
+
 
 def _contract_vvvv_t2(mycc, mol, vvL, t2, out=None, verbose=None):
     '''Ht2 = numpy.einsum('ijcd,acdb->ijab', t2, vvvv)
 
     Args:
         vvvv : None or integral object
             if vvvv is None, contract t2 to AO-integrals using AO-direct algorithm
```

### Comparing `pyscf-2.5.0/pyscf/cc/eom_gccsd.py` & `pyscf-2.6.0/pyscf/cc/eom_gccsd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/eom_rccsd.py` & `pyscf-2.6.0/pyscf/cc/eom_rccsd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/eom_uccsd.py` & `pyscf-2.6.0/pyscf/cc/eom_uccsd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/gccsd.py` & `pyscf-2.6.0/pyscf/cc/gccsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,14 +285,16 @@
     def spin2spatial(self, tx, orbspin=None):
         if orbspin is None:
             orbspin = getattr(self.mo_coeff, 'orbspin', None)
             if orbspin is not None:
                 orbspin = orbspin[self.get_frozen_mask()]
         return spin2spatial(tx, orbspin)
 
+    to_gpu = lib.to_gpu
+
 CCSD = GCCSD
 
 
 class _PhysicistsERIs:
     '''<pq||rs> = <pq|rs> - <pq|sr>'''
     def __init__(self, mol=None):
         self.mol = mol
```

### Comparing `pyscf-2.5.0/pyscf/cc/gccsd_lambda.py` & `pyscf-2.6.0/pyscf/cc/gccsd_lambda.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/gccsd_rdm.py` & `pyscf-2.6.0/pyscf/cc/gccsd_rdm.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/gccsd_t.py` & `pyscf-2.6.0/pyscf/cc/gccsd_t.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/gccsd_t_lambda.py` & `pyscf-2.6.0/pyscf/cc/gccsd_t_lambda.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/gccsd_t_rdm.py` & `pyscf-2.6.0/pyscf/cc/gccsd_t_rdm.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/gccsd_t_slow.py` & `pyscf-2.6.0/pyscf/cc/gccsd_t_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/gintermediates.py` & `pyscf-2.6.0/pyscf/cc/gintermediates.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/momgfccsd.py` & `pyscf-2.6.0/pyscf/cc/momgfccsd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/qcisd.py` & `pyscf-2.6.0/pyscf/cc/qcisd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/qcisd_slow.py` & `pyscf-2.6.0/pyscf/cc/qcisd_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/qcisd_t.py` & `pyscf-2.6.0/pyscf/cc/qcisd_t.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/qcisd_t_slow.py` & `pyscf-2.6.0/pyscf/cc/qcisd_t_slow.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     nocc, nvir = t1.shape
     mo_e = eris.fock.diagonal().real
     e_occ, e_vir = mo_e[:nocc], mo_e[nocc:]
     eijk = lib.direct_sum('i,j,k->ijk', e_occ, e_occ, e_occ)
 
     eris_vvov = eris.get_ovvv().conj().transpose(1,3,0,2)
-    eris_vooo = numpy.asarray(eris.ovoo).conj().transpose(1,0,3,2)
+    eris_vooo = numpy.asarray(eris.ovoo).conj().transpose(1,0,2,3)
     eris_vvoo = numpy.asarray(eris.ovov).conj().transpose(1,3,0,2)
     fvo = eris.fock[nocc:,:nocc]
     def get_w(a, b, c):
         w = numpy.einsum('if,fkj->ijk', eris_vvov[a,b], t2T[c,:])
         w-= numpy.einsum('ijm,mk->ijk', eris_vooo[a,:], t2T[b,c])
         return w
     def get_v(a, b, c):
```

### Comparing `pyscf-2.5.0/pyscf/cc/rccsd.py` & `pyscf-2.6.0/pyscf/cc/rccsd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/rccsd_lambda.py` & `pyscf-2.6.0/pyscf/cc/rccsd_lambda.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/rccsd_slow.py` & `pyscf-2.6.0/pyscf/cc/rccsd_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/rintermediates.py` & `pyscf-2.6.0/pyscf/cc/rintermediates.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/uccsd.py` & `pyscf-2.6.0/pyscf/cc/uccsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -754,14 +754,16 @@
         sizeb = noccb * nvirb + noccb*(noccb-1)//2*nvirb*(nvirb-1)//2
         sizeab = nocca * noccb * nvira * nvirb
         return sizea + sizeb + sizeab
 
     def amplitudes_from_rccsd(self, t1, t2):
         return amplitudes_from_rccsd(t1, t2)
 
+    to_gpu = lib.to_gpu
+
 CCSD = UCCSD
 
 
 class _ChemistsERIs(ccsd._ChemistsERIs):
     def __init__(self, mol=None):
         ccsd._ChemistsERIs.__init__(self, mol)
         self.OOOO = None
```

### Comparing `pyscf-2.5.0/pyscf/cc/uccsd_lambda.py` & `pyscf-2.6.0/pyscf/cc/uccsd_lambda.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/uccsd_rdm.py` & `pyscf-2.6.0/pyscf/cc/uccsd_rdm.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/uccsd_slow.py` & `pyscf-2.6.0/pyscf/cc/uccsd_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/uccsd_t.py` & `pyscf-2.6.0/pyscf/cc/uccsd_t.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/uccsd_t_lambda.py` & `pyscf-2.6.0/pyscf/cc/uccsd_t_lambda.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/uccsd_t_rdm.py` & `pyscf-2.6.0/pyscf/cc/uccsd_t_rdm.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/uccsd_t_slow.py` & `pyscf-2.6.0/pyscf/cc/uccsd_t_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/uintermediates.py` & `pyscf-2.6.0/pyscf/cc/uintermediates.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/cc/uintermediates_slow.py` & `pyscf-2.6.0/pyscf/cc/uintermediates_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/ci/__init__.py` & `pyscf-2.6.0/pyscf/ci/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/ci/addons.py` & `pyscf-2.6.0/pyscf/ci/addons.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/ci/cisd.py` & `pyscf-2.6.0/pyscf/ci/cisd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1127,14 +1127,16 @@
     def density_fit(self):
         raise NotImplementedError
 
     def nuc_grad_method(self):
         from pyscf.grad import cisd
         return cisd.Gradients(self)
 
+    to_gpu = lib.to_gpu
+
 class RCISD(CISD):
     pass
 
 from pyscf import scf
 scf.hf.RHF.CISD = lib.class_as_method(RCISD)
 scf.rohf.ROHF.CISD = None
```

### Comparing `pyscf-2.5.0/pyscf/ci/gcisd.py` & `pyscf-2.6.0/pyscf/ci/gcisd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/ci/ucisd.py` & `pyscf-2.6.0/pyscf/ci/ucisd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/data/__init__.py` & `pyscf-2.6.0/pyscf/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/data/elements.py` & `pyscf-2.6.0/pyscf/data/elements.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/data/gyro.py` & `pyscf-2.6.0/pyscf/data/gyro.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/data/gyromagnetic_ratio.dat` & `pyscf-2.6.0/pyscf/data/gyromagnetic_ratio.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/data/nist.py` & `pyscf-2.6.0/pyscf/data/nist.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/data/nuclear_g_factor.dat` & `pyscf-2.6.0/pyscf/data/nuclear_g_factor.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/data/nucprop.py` & `pyscf-2.6.0/pyscf/data/nucprop.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/data/radii.py` & `pyscf-2.6.0/pyscf/data/radii.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/data/solvents.dat` & `pyscf-2.6.0/pyscf/data/solvents.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/df/__init__.py` & `pyscf-2.6.0/pyscf/df/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/df/addons.py` & `pyscf-2.6.0/pyscf/df/addons.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         _basis = {a: mol.basis for a in uniq_atoms}
     elif 'default' in mol.basis:
         default_basis = mol.basis['default']
         _basis = {a: default_basis for a in uniq_atoms}
         _basis.update(mol.basis)
         del (_basis['default'])
     else:
-        _basis = mol._basis
+        _basis = mol._basis or {}
 
     auxbasis = {}
     for k in _basis:
         if isinstance(_basis[k], str):
             balias = gto.basis._format_basis_name(_basis[k])
             if gto.basis._is_pople_basis(balias):
                 balias = balias.split('g')[0] + 'g'
```

### Comparing `pyscf-2.5.0/pyscf/df/df.py` & `pyscf-2.6.0/pyscf/df/df.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,15 +280,15 @@
             omega = 0
         key = '%.6f' % omega
         if key in self._rsh_df:
             rsh_df = self._rsh_df[key]
         else:
             rsh_df = self._rsh_df[key] = self.copy().reset()
             if hasattr(self, '_dataname'):
-                rsh_df._dataname = f'{self._dataname}/lr/{key}'
+                rsh_df._dataname = f'{self._dataname}-lr/{key}'
             logger.info(self, 'Create RSH-DF object %s for omega=%s', rsh_df, omega)
 
         mol = self.mol
         auxmol = self.auxmol
 
         mol_omega = mol.omega
         mol.omega = omega
@@ -304,17 +304,15 @@
         try:
             yield rsh_df
         finally:
             mol.omega = mol_omega
             if auxmol_omega is not None:
                 auxmol.omega = auxmol_omega
 
-    def to_gpu(self):
-        from gpu4pyscf.df.df import DF as DF
-        return lib.to_gpu(self.__class__.reset(self.view(DF)))
+    to_gpu = lib.to_gpu
 
 GDF = DF
 
 
 class DF4C(DF):
     '''Relativistic 4-component'''
     def build(self):
```

### Comparing `pyscf-2.5.0/pyscf/df/df_jk.py` & `pyscf-2.6.0/pyscf/df/df_jk.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,16 +224,15 @@
 
     def CASSCF(self, ncas, nelecas, auxbasis=None, ncore=None, frozen=None):
         from pyscf import mcscf
         return mcscf.DFCASSCF(self, ncas, nelecas, auxbasis, ncore, frozen)
 
     def to_gpu(self):
         obj = self.undo_df().to_gpu().density_fit()
-        obj.__dict__.update(self.__dict__)
-        return lib.to_gpu(obj)
+        return lib.to_gpu(self, obj)
 
 
 def get_jk(dfobj, dm, hermi=1, with_j=True, with_k=True, direct_scf_tol=1e-13):
     assert (with_j or with_k)
     if (not with_k and not dfobj.mol.incore_anyway and
         # 3-center integral tensor is not initialized
         dfobj._cderi is None):
@@ -257,16 +256,17 @@
     if with_j:
         idx = numpy.arange(nao)
         dmtril = lib.pack_tril(dms + dms.conj().transpose(0,2,1))
         dmtril[:,idx*(idx+1)//2+idx] *= .5
 
     if not with_k:
         for eri1 in dfobj.loop():
-            rho = numpy.einsum('ix,px->ip', dmtril, eri1)
-            vj += numpy.einsum('ip,px->ix', rho, eri1)
+            # uses numpy.matmul
+            vj += (dmtril @ eri1.T) @ eri1
+
 
     elif getattr(dm, 'mo_coeff', None) is not None:
         #TODO: test whether dm.mo_coeff matching dm
         mo_coeff = numpy.asarray(dm.mo_coeff, order='F')
         mo_occ   = numpy.asarray(dm.mo_occ)
         nmo = mo_occ.shape[-1]
         mo_coeff = mo_coeff.reshape(-1,nao,nmo)
@@ -287,17 +287,16 @@
         max_memory = dfobj.max_memory - lib.current_memory()[0]
         blksize = max(4, int(min(dfobj.blockdim, max_memory*.3e6/8/nao**2)))
         buf = numpy.empty((blksize*nao,nao))
         for eri1 in dfobj.loop(blksize):
             naux, nao_pair = eri1.shape
             assert (nao_pair == nao*(nao+1)//2)
             if with_j:
-                rho = numpy.einsum('ix,px->ip', dmtril, eri1)
-                vj += numpy.einsum('ip,px->ix', rho, eri1)
-
+                # uses numpy.matmul
+                vj += (dmtril @ eri1.T) @ eri1
             for k in range(nset):
                 nocc = orbo[k].shape[1]
                 if nocc > 0:
                     buf1 = buf[:naux*nocc]
                     fdrv(ftrans, fmmm,
                          buf1.ctypes.data_as(ctypes.c_void_p),
                          eri1.ctypes.data_as(ctypes.c_void_p),
@@ -315,16 +314,17 @@
         dms = [numpy.asarray(x, order='F') for x in dms]
         max_memory = dfobj.max_memory - lib.current_memory()[0]
         blksize = max(4, int(min(dfobj.blockdim, max_memory*.22e6/8/nao**2)))
         buf = numpy.empty((2,blksize,nao,nao))
         for eri1 in dfobj.loop(blksize):
             naux, nao_pair = eri1.shape
             if with_j:
-                rho = numpy.einsum('ix,px->ip', dmtril, eri1)
-                vj += numpy.einsum('ip,px->ix', rho, eri1)
+                # uses numpy.matmul
+                vj += (dmtril @ eri1.T) @ eri1
+
 
             for k in range(nset):
                 buf1 = buf[0,:naux]
                 fdrv(ftrans, fmmm,
                      buf1.ctypes.data_as(ctypes.c_void_p),
                      eri1.ctypes.data_as(ctypes.c_void_p),
                      dms[k].ctypes.data_as(ctypes.c_void_p),
```

### Comparing `pyscf-2.5.0/pyscf/df/grad/casdm2_util.py` & `pyscf-2.6.0/pyscf/df/grad/casdm2_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,15 +472,15 @@
         intbuf = lib.einsum ('xuvp,vj->xupj', int3c, mo_cas[0])
         dm2buf = lib.einsum ('uj,npij->nupi', mo_cas[1], dfcasdm2[:,p0:p1,:,:])
         dE -= np.einsum ('nupj,xupj->nux', dm2buf, intbuf)
         intbuf = dm2buf = int3c = None
 
     aoslices = mol.aoslice_by_atom ()
     dE = np.array ([dE[:,p0:p1].sum (axis=1) for p0, p1 in aoslices[:,2:]]).transpose (1,0,2)
-    return np.ascontiguousarray (dE)
+    return np.ascontiguousarray (dE)[:,atmlst,:]
 
 if __name__ == '__main__':
     from pyscf.tools import molden
     from pyscf.lib import logger, param
     h2co_casscf66_631g_xyz = '''C  0.534004  0.000000  0.000000
     O -0.676110  0.000000  0.000000
     H  1.102430  0.000000  0.920125
```

### Comparing `pyscf-2.5.0/pyscf/df/grad/casscf.py` & `pyscf-2.6.0/pyscf/df/grad/casscf.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,16 @@
             logger.note(self, '--------------- %s gradients ---------------',
                         self.base.__class__.__name__)
             self._write(self.mol, self.de, self.atmlst)
             logger.note(self, '----------------------------------------------')
 
     as_scanner = as_scanner
 
+    to_gpu = lib.to_gpu
+
 Grad = Gradients
 
 #from pyscf import mcscf
 #mcscf.mc1step.CASSCF.Gradients = lib.class_as_method(Gradients)
 
 
 if __name__ == '__main__':
```

### Comparing `pyscf-2.5.0/pyscf/df/grad/rhf.py` & `pyscf-2.6.0/pyscf/df/grad/rhf.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,17 @@
 from pyscf.gto.moleintor import getints, make_cintopt
 from pyscf.lib import logger
 from pyscf.grad import rhf as rhf_grad
 from functools import reduce
 from itertools import product
 from pyscf.ao2mo import _ao2mo
 from pyscf.df import df_jk
+from pyscf.df.incore import LINEAR_DEP_THR
 
-LINEAR_DEP_THRESHOLD = 1e-9
+LINEAR_DEP_THRESHOLD = LINEAR_DEP_THR
 
 def get_jk(mf_grad, mol=None, dm=None, hermi=0, with_j=True, with_k=True,
            decompose_j2c='CD', lindep=LINEAR_DEP_THRESHOLD):
     '''
     Computes J and K derivatives with density fitting
 
     Args:
@@ -478,20 +479,23 @@
 
 class Gradients(rhf_grad.Gradients):
     '''Restricted density-fitting Hartree-Fock gradients'''
 
     _keys = {'with_df', 'auxbasis_response'}
 
     def __init__(self, mf):
-        assert isinstance(mf, df.df_jk._DFHF)
-        # Whether to include the response of DF auxiliary basis when computing
-        # nuclear gradients of J/K matrices
-        self.auxbasis_response = True
         rhf_grad.Gradients.__init__(self, mf)
 
+    # Whether to include the response of DF auxiliary basis when computing
+    # nuclear gradients of J/K matrices
+    auxbasis_response = True
+
+    def check_sanity(self):
+        assert isinstance(self.base, df.df_jk._DFHF)
+
     def get_jk(self, mol=None, dm=None, hermi=0, with_j=True, with_k=True,
                omega=None):
         if omega is None:
             return get_jk(self, mol, dm, hermi, with_j, with_k)
 
         with self.base.with_df.range_coulomb(omega):
             return get_jk(self, mol, dm, hermi, with_j, with_k)
@@ -517,12 +521,8 @@
 
     def extra_force(self, atom_id, envs):
         if self.auxbasis_response:
             return envs['vhf'].aux[atom_id]
         else:
             return 0
 
-    def to_gpu(self):
-        from gpu4pyscf.df.grad.rhf import Gradients
-        return lib.to_gpu(self.view(Gradients))
-
 Grad = Gradients
```

### Comparing `pyscf-2.5.0/pyscf/df/grad/rks.py` & `pyscf-2.6.0/pyscf/df/grad/rks.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,30 +42,30 @@
 
     mem_now = lib.current_memory()[0]
     max_memory = max(2000, ks_grad.max_memory*.9-mem_now)
     if ks_grad.grid_response:
         exc, vxc = rks_grad.get_vxc_full_response(
             ni, mol, grids, mf.xc, dm,
             max_memory=max_memory, verbose=ks_grad.verbose)
-        if mf.nlc or ni.libxc.is_nlc(mf.xc):
+        if mf.do_nlc():
             if ni.libxc.is_nlc(mf.xc):
                 xc = mf.xc
             else:
                 xc = mf.nlc
             enlc, vnlc = rks_grad.get_nlc_vxc_full_response(
                 ni, mol, nlcgrids, xc, dm,
                 max_memory=max_memory, verbose=ks_grad.verbose)
             exc += enlc
             vxc += vnlc
         logger.debug1(ks_grad, 'sum(grids response) %s', exc.sum(axis=0))
     else:
         exc, vxc = rks_grad.get_vxc(
             ni, mol, grids, mf.xc, dm,
             max_memory=max_memory, verbose=ks_grad.verbose)
-        if mf.nlc or ni.libxc.is_nlc(mf.xc):
+        if mf.do_nlc():
             if ni.libxc.is_nlc(mf.xc):
                 xc = mf.xc
             else:
                 xc = mf.nlc
             enlc, vnlc = rks_grad.get_nlc_vxc(
                 ni, mol, nlcgrids, xc, dm,
                 max_memory=max_memory, verbose=ks_grad.verbose)
@@ -103,28 +103,25 @@
 
 
 class Gradients(rks_grad.Gradients):
 
     _keys = {'with_df', 'auxbasis_response'}
 
     def __init__(self, mf):
-        # Whether to include the response of DF auxiliary basis when computing
-        # nuclear gradients of J/K matrices
-        self.auxbasis_response = True
         rks_grad.Gradients.__init__(self, mf)
 
+    # Whether to include the response of DF auxiliary basis when computing
+    # nuclear gradients of J/K matrices
+    auxbasis_response = True
+
     get_jk = df_rhf_grad.Gradients.get_jk
     get_j = df_rhf_grad.Gradients.get_j
     get_k = df_rhf_grad.Gradients.get_k
     get_veff = get_veff
 
     def extra_force(self, atom_id, envs):
         e1 = rks_grad.Gradients.extra_force(self, atom_id, envs)
         if self.auxbasis_response:
             e1 += envs['vhf'].aux[atom_id]
         return e1
 
-    def to_gpu(self):
-        from gpu4pyscf.df.grad.rks import Gradients
-        return lib.to_gpu(self.view(Gradients))
-
 Grad = Gradients
```

### Comparing `pyscf-2.5.0/pyscf/df/grad/sacasscf.py` & `pyscf-2.6.0/pyscf/df/grad/sacasscf.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,7 +366,9 @@
         # But on the other hand maybe it can be even simpler?
         with lib.temporary_env (casscf_grad, Gradients=dfcasscf_grad.Gradients):
             return sacasscf_grad.Gradients.kernel (self, **kwargs)
 
     def get_LdotJnuc (self, Lvec, **kwargs):
         with lib.temporary_env (sacasscf_grad, Lci_dot_dgci_dx=Lci_dot_dgci_dx, Lorb_dot_dgorb_dx=Lorb_dot_dgorb_dx):
             return sacasscf_grad.Gradients.get_LdotJnuc (self, Lvec, **kwargs)
+
+    to_gpu = lib.to_gpu
```

### Comparing `pyscf-2.5.0/pyscf/df/grad/uhf.py` & `pyscf-2.6.0/pyscf/df/grad/uhf.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,20 @@
 
 class Gradients(uhf_grad.Gradients):
     '''Unrestricted density-fitting Hartree-Fock gradients'''
 
     _keys = {'with_df', 'auxbasis_response'}
 
     def __init__(self, mf):
-        # Whether to include the response of DF auxiliary basis when computing
-        # nuclear gradients of J/K matrices
-        self.auxbasis_response = True
         uhf_grad.Gradients.__init__(self, mf)
 
+    # Whether to include the response of DF auxiliary basis when computing
+    # nuclear gradients of J/K matrices
+    auxbasis_response = True
+
     get_jk = df_rhf_grad.Gradients.get_jk
     get_j = df_rhf_grad.Gradients.get_j
     get_k = df_rhf_grad.Gradients.get_k
 
     def get_veff(self, mol=None, dm=None):
         vj, vk = self.get_jk(mol, dm)
         vhf = vj[0]+vj[1] - vk
```

### Comparing `pyscf-2.5.0/pyscf/df/grad/uks.py` & `pyscf-2.6.0/pyscf/df/grad/uks.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,30 +44,30 @@
 
     mem_now = lib.current_memory()[0]
     max_memory = max(2000, ks_grad.max_memory*.9-mem_now)
     if ks_grad.grid_response:
         exc, vxc = uks_grad.get_vxc_full_response(
                 ni, mol, grids, mf.xc, dm,
                 max_memory=max_memory, verbose=ks_grad.verbose)
-        if mf.nlc or ni.libxc.is_nlc(mf.xc):
+        if mf.do_nlc():
             if ni.libxc.is_nlc(mf.xc):
                 xc = mf.xc
             else:
                 xc = mf.nlc
             enlc, vnlc = rks_grad.get_nlc_vxc_full_response(
                 ni, mol, nlcgrids, xc, dm[0]+dm[1],
                 max_memory=max_memory, verbose=ks_grad.verbose)
             exc += enlc
             vxc += vnlc
         logger.debug1(ks_grad, 'sum(grids response) %s', exc.sum(axis=0))
     else:
         exc, vxc = uks_grad.get_vxc(
                 ni, mol, grids, mf.xc, dm,
                 max_memory=max_memory, verbose=ks_grad.verbose)
-        if mf.nlc or ni.libxc.is_nlc(mf.xc):
+        if mf.do_nlc():
             if ni.libxc.is_nlc(mf.xc):
                 xc = mf.xc
             else:
                 xc = mf.nlc
             enlc, vnlc = rks_grad.get_nlc_vxc(
                 ni, mol, nlcgrids, xc, dm[0]+dm[1],
                 max_memory=max_memory, verbose=ks_grad.verbose)
@@ -104,19 +104,19 @@
 
 
 class Gradients(uks_grad.Gradients):
 
     _keys = {'with_df', 'auxbasis_response'}
 
     def __init__(self, mf):
-        # Whether to include the response of DF auxiliary basis when computing
-        # nuclear gradients of J/K matrices
-        self.auxbasis_response = True
         uks_grad.Gradients.__init__(self, mf)
 
+    # Whether to include the response of DF auxiliary basis when computing
+    # nuclear gradients of J/K matrices
+    auxbasis_response = True
     get_jk = df_rhf_grad.Gradients.get_jk
     get_j = df_rhf_grad.Gradients.get_j
     get_k = df_rhf_grad.Gradients.get_k
     get_veff = get_veff
 
     def extra_force(self, atom_id, envs):
         e1 = uks_grad.Gradients.extra_force(self, atom_id, envs)
```

### Comparing `pyscf-2.5.0/pyscf/df/hessian/rhf.py` & `pyscf-2.6.0/pyscf/df/hessian/rhf.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,21 @@
 from pyscf import lib
 from pyscf.lib import logger
 from pyscf import ao2mo
 from pyscf.hessian import rhf as rhf_hess
 from pyscf.df.grad.rhf import (_int3c_wrapper, _gen_metric_solver,
                                LINEAR_DEP_THRESHOLD)
 
+def _pinv(a, lindep=LINEAR_DEP_THRESHOLD):
+    '''Similar to pinv (v1.7.0) with atol=lindep and rtol=0'''
+    w, v = scipy.linalg.eigh(a)
+    mask = w > lindep
+    v1 = v[:, mask]
+    return lib.dot(v1/w[mask], v1.conj().T)
+
 def partial_hess_elec(hessobj, mo_energy=None, mo_coeff=None, mo_occ=None,
                       atmlst=None, max_memory=4000, verbose=None):
     e1, ej, ek = _partial_hess_ejk(hessobj, mo_energy, mo_coeff, mo_occ,
                                    atmlst, max_memory, verbose, True)
     return e1 + ej - ek
 
 def _partial_hess_ejk(hessobj, mo_energy=None, mo_coeff=None, mo_occ=None,
@@ -170,15 +177,15 @@
                 wk_ip2_P__[p0:p1] = lib.einsum('xuvp,ui,vj->pxij', int3c_ip2, mocc_2, mocc_2)
         int3c_ip2 = None
 
     if hessobj.auxbasis_response > 1:
         get_int3c_ipip2 = _int3c_wrapper(mol, auxmol, 'int3c2e_ipip2', 's1')
         rhok0_P__ = lib.einsum('plj,li->pij', rhok0_Pl_, mocc_2)
         rho2c_0 = lib.einsum('pij,qji->pq', rhok0_P__, rhok0_P__)
-        int2c_inv = numpy.linalg.pinv(int2c, rcond=LINEAR_DEP_THRESHOLD)
+        int2c_inv = _pinv(int2c, lindep=LINEAR_DEP_THRESHOLD)
         int2c_ipip1 = auxmol.intor('int2c2e_ipip1', aosym='s1')
         int2c_ip_ip  = lib.einsum('xpq,qr,ysr->xyps', int2c_ip1, int2c_inv, int2c_ip1)
         int2c_ip_ip -= auxmol.intor('int2c2e_ip1ip2', aosym='s1').reshape(3,3,naux,naux)
     int2c = solve_j2c = None
 
     get_int3c_ipvip1 = _int3c_wrapper(mol, auxmol, 'int3c2e_ipvip1', 's1')
     get_int3c_ip1ip2 = _int3c_wrapper(mol, auxmol, 'int3c2e_ip1ip2', 's1')
@@ -471,24 +478,20 @@
 def _load_dim0(dat, p0, p1):
     return np.hstack([dat[x][p0:p1] for x in dat])
 
 
 class Hessian(rhf_hess.Hessian):
     '''Non-relativistic restricted Hartree-Fock hessian'''
     def __init__(self, mf):
-        self.auxbasis_response = 1
         rhf_hess.Hessian.__init__(self, mf)
 
+    auxbasis_response = 1
     partial_hess_elec = partial_hess_elec
     make_h1 = make_h1
 
-    def to_gpu(self):
-        from gpu4pyscf.df.hessian.rhf import Hessian
-        return lib.to_gpu(self.view(Hessian))
-
 #TODO: Insert into DF class
 
 
 if __name__ == '__main__':
     from pyscf import gto
     from pyscf import scf
```

### Comparing `pyscf-2.5.0/pyscf/df/hessian/rks.py` & `pyscf-2.6.0/pyscf/df/hessian/rks.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                       atmlst=None, max_memory=4000, verbose=None):
     log = logger.new_logger(hessobj, verbose)
     time0 = t1 = (logger.process_clock(), logger.perf_counter())
 
     mol = hessobj.mol
     mf = hessobj.base
     ni = mf._numint
-    if mf.nlc or ni.libxc.is_nlc(mf.xc):
+    if mf.do_nlc():
         raise NotImplementedError('RKS Hessian for NLC functional')
 
     if mo_energy is None: mo_energy = mf.mo_energy
     if mo_occ is None:    mo_occ = mf.mo_occ
     if mo_coeff is None:  mo_coeff = mf.mo_coeff
     if atmlst is None: atmlst = range(mol.natm)
 
@@ -117,24 +117,20 @@
             lib.chkfile.save(chkfile, 'scf_f1ao/%d'%ia, h1ao[ia])
         return chkfile
 
 
 class Hessian(rks_hess.Hessian):
     '''Non-relativistic RKS hessian'''
     def __init__(self, mf):
-        self.auxbasis_response = 1
         rks_hess.Hessian.__init__(self, mf)
 
+    auxbasis_response = 1
     partial_hess_elec = partial_hess_elec
     make_h1 = make_h1
 
-    def to_gpu(self):
-        from gpu4pyscf.df.hessian.rks import Hessian
-        return lib.to_gpu(self.view(Hessian))
-
 
 if __name__ == '__main__':
     from pyscf import gto
     from pyscf import dft
     #dft.numint.NumInt.libxc = dft.xcfun
     xc_code = 'b3lyp'
```

### Comparing `pyscf-2.5.0/pyscf/df/hessian/uhf.py` & `pyscf-2.6.0/pyscf/df/hessian/uhf.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 import numpy as np
 import scipy.linalg
 from pyscf import lib
 from pyscf.lib import logger
 from pyscf import ao2mo
 from pyscf.hessian import rhf as rhf_hess
 from pyscf.hessian import uhf as uhf_hess
-from pyscf.df.hessian.rhf import _load_dim0
+from pyscf.df.hessian.rhf import _load_dim0, _pinv
 from pyscf.df.grad.rhf import (_int3c_wrapper, _gen_metric_solver,
                                LINEAR_DEP_THRESHOLD)
 
 
 def partial_hess_elec(hessobj, mo_energy=None, mo_coeff=None, mo_occ=None,
                       atmlst=None, max_memory=4000, verbose=None):
     e1, ej, ek = _partial_hess_ejk(hessobj, mo_energy, mo_coeff, mo_occ,
@@ -193,15 +193,15 @@
 
     if hessobj.auxbasis_response > 1:
         get_int3c_ipip2 = _int3c_wrapper(mol, auxmol, 'int3c2e_ipip2', 's1')
         rhok0a_P__ = lib.einsum('plj,li->pij', rhok0a_Pl_, mocca)
         rhok0b_P__ = lib.einsum('plj,li->pij', rhok0b_Pl_, moccb)
         rho2c_0  = lib.einsum('pij,qij->pq', rhok0a_P__, rhok0a_P__)
         rho2c_0 += lib.einsum('pij,qij->pq', rhok0b_P__, rhok0b_P__)
-        int2c_inv = numpy.linalg.pinv(int2c, rcond=LINEAR_DEP_THRESHOLD)
+        int2c_inv = _pinv(int2c, lindep=LINEAR_DEP_THRESHOLD)
         int2c_ipip1 = auxmol.intor('int2c2e_ipip1', aosym='s1')
         int2c_ip_ip  = lib.einsum('xpq,qr,ysr->xyps', int2c_ip1, int2c_inv, int2c_ip1)
         int2c_ip_ip -= auxmol.intor('int2c2e_ip1ip2', aosym='s1').reshape(3,3,naux,naux)
     int2c = solve_j2c = None
 
     get_int3c_ipvip1 = _int3c_wrapper(mol, auxmol, 'int3c2e_ipvip1', 's1')
     get_int3c_ip1ip2 = _int3c_wrapper(mol, auxmol, 'int3c2e_ip1ip2', 's1')
@@ -522,17 +522,17 @@
         h1 = hcore_deriv(ia)
         yield ia, h1, vj1, (vk1a, vk1b)
 
 
 class Hessian(uhf_hess.Hessian):
     '''Non-relativistic UHF hessian'''
     def __init__(self, mf):
-        self.auxbasis_response = 1
         uhf_hess.Hessian.__init__(self, mf)
 
+    auxbasis_response = 1
     partial_hess_elec = partial_hess_elec
     make_h1 = make_h1
 
 #TODO: Insert into DF class
 
 
 if __name__ == '__main__':
```

### Comparing `pyscf-2.5.0/pyscf/df/hessian/uks.py` & `pyscf-2.6.0/pyscf/df/hessian/uks.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                       atmlst=None, max_memory=4000, verbose=None):
     log = logger.new_logger(hessobj, verbose)
     time0 = t1 = (logger.process_clock(), logger.perf_counter())
 
     mol = hessobj.mol
     mf = hessobj.base
     ni = mf._numint
-    if mf.nlc or ni.libxc.is_nlc(mf.xc):
+    if mf.do_nlc():
         raise NotImplementedError('RKS Hessian for NLC functional')
 
     if mo_energy is None: mo_energy = mf.mo_energy
     if mo_occ is None:    mo_occ = mf.mo_occ
     if mo_coeff is None:  mo_coeff = mf.mo_coeff
     if atmlst is None: atmlst = range(mol.natm)
 
@@ -130,17 +130,17 @@
             lib.chkfile.save(chkfile, 'scf_f1ao/1/%d'%ia, h1aob[ia])
         return chkfile
 
 
 class Hessian(uks_hess.Hessian):
     '''Non-relativistic RKS hessian'''
     def __init__(self, mf):
-        self.auxbasis_response = 1
         uks_hess.Hessian.__init__(self, mf)
 
+    auxbasis_response = 1
     partial_hess_elec = partial_hess_elec
     make_h1 = make_h1
 
 
 if __name__ == '__main__':
     from pyscf import gto
     from pyscf import dft
```

### Comparing `pyscf-2.5.0/pyscf/df/incore.py` & `pyscf-2.6.0/pyscf/df/incore.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from pyscf import gto
 from pyscf.df import addons
 from pyscf.gto.moleintor import getints
 from pyscf import __config__
 
 
 MAX_MEMORY = getattr(__config__, 'df_outcore_max_memory', 2000)  # 2GB
-LINEAR_DEP_THR = getattr(__config__, 'df_df_DF_lindep', 1e-12)
+LINEAR_DEP_THR = getattr(__config__, 'df_df_DF_lindep', 1e-9)
 
 
 # This function is aliased for backward compatibility.
 format_aux_basis = addons.make_auxmol
 
 
 def aux_e2(mol, auxmol_or_auxbasis, intor='int3c2e', aosym='s1', comp=None, out=None,
@@ -175,18 +175,19 @@
             bufs1, bufs2 = bufs2, bufs1
         else:
             ints = ints.reshape((-1,naoaux)).T
 
         p0, p1 = p1, p1 + nrow
         if decompose_j2c == 'cd':
             if ints.flags.c_contiguous:
-                ints = lib.transpose(ints, out=bufs2).T
-                bufs1, bufs2 = bufs2, bufs1
-            dat = scipy.linalg.solve_triangular(low, ints, lower=True,
-                                                overwrite_b=True, check_finite=False)
+                trsm, = scipy.linalg.get_blas_funcs(('trsm',), (low, ints))
+                dat = trsm(1.0, low, ints.T, lower=True, trans_a = 1, side = 1, overwrite_b=True).T
+            else:
+                dat = scipy.linalg.solve_triangular(low, ints, lower=True,
+                                                   overwrite_b=True, check_finite=False)
             if dat.flags.f_contiguous:
                 dat = lib.transpose(dat.T, out=bufs2)
             cderi[:,p0:p1] = dat
         else:
             dat = numpy.ndarray((naux, ints.shape[1]), buffer=bufs2)
             cderi[:,p0:p1] = lib.dot(low, ints, c=dat)
         dat = ints = None
```

### Comparing `pyscf-2.5.0/pyscf/df/outcore.py` & `pyscf-2.6.0/pyscf/df/outcore.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,14 +89,19 @@
             h5d_eri[row0:row1] = dat
         else:
             h5d_eri[:,row0:row1] = dat
         dat = None
         ti0 = log.timer('step 2 [%d/%d], [%d:%d], row = %d'%
                         (istep+1, totstep, row0, row1, nrow), *ti0)
 
+    # A bug in NFS / HDF5 may cause .close() not to
+    # flush properly, hanging the calculation. Flush manually
+    fswap.flush()
+    feri.flush()
+
     fswap.close()
     feri.close()
     log.timer('cholesky_eri', *time0)
     return erifile
 
 def cholesky_eri_b(mol, erifile, auxbasis='weigend+etb', dataname='j3c',
                    int3c='int3c2e', aosym='s2ij', int2c='int2c2e', comp=1,
@@ -159,40 +164,47 @@
     # the opt for the 3rd index.
     #if '3c2e' in int3c:
     #    cintopt = gto.moleintor.make_cintopt(atm, mol._bas, env, int3c)
     #else:
     #    cintopt = gto.moleintor.make_cintopt(atm, bas, env, int3c)
     cintopt = gto.moleintor.make_cintopt(atm, bas, env, int3c)
     bufs1 = numpy.empty((comp*max([x[2] for x in shranges]),naoaux))
+    bufs2 = numpy.empty_like(bufs1)
 
     def transform(b):
         if b.ndim == 3 and b.flags.f_contiguous:
             b = lib.transpose(b.T, axes=(0,2,1)).reshape(naoaux,-1)
         else:
             b = b.reshape((-1,naoaux)).T
         if decompose_j2c != 'CD':
             return lib.dot(low, b)
 
         if b.flags.c_contiguous:
-            b = lib.transpose(b).T
-        return scipy.linalg.solve_triangular(low, b, lower=True,
+            trsm, = scipy.linalg.get_blas_funcs(('trsm',), (low, b))
+            return trsm(1.0, low, b.T, lower=True, trans_a = 1, side = 1,
+                     overwrite_b=True).T
+        else:
+            return scipy.linalg.solve_triangular(low, b, lower=True,
                                              overwrite_b=True, check_finite=False)
 
     def process(sh_range):
+        nonlocal bufs1, bufs2
+        bufs2, bufs1 = bufs1, bufs2
         bstart, bend, nrow = sh_range
         shls_slice = (bstart, bend, 0, mol.nbas, mol.nbas, mol.nbas+auxmol.nbas)
         ints = gto.moleintor.getints3c(int3c, atm, bas, env, shls_slice, comp,
                                        aosym, ao_loc, cintopt, out=bufs1)
         if comp == 1:
             dat = transform(ints)
         else:
             dat = [transform(x) for x in ints]
         return dat
 
     feri = _create_h5file(erifile, dataname)
+
     for istep, dat in enumerate(lib.map_with_prefetch(process, shranges)):
         sh_range = shranges[istep]
         label = '%s/%d'%(dataname,istep)
         if comp == 1:
             feri[label] = dat
         else:
             shape = (len(dat),) + dat[0].shape
@@ -200,14 +212,16 @@
             for i, b in enumerate(dat):
                 fdat[i] = b
         dat = None
         log.debug('int3c2e [%d/%d], AO [%d:%d], nrow = %d',
                   istep+1, len(shranges), *sh_range)
         time1 = log.timer('gen CD eri [%d/%d]' % (istep+1,len(shranges)), *time1)
     bufs1 = None
+    bufs2 = None
+    feri.flush()
     feri.close()
     return erifile
 
 
 def general(mol, mo_coeffs, erifile, auxbasis='weigend+etb', dataname='eri_mo', tmpdir=None,
             int3c='int3c2e', aosym='s2ij', int2c='int2c2e', comp=1,
             max_memory=MAX_MEMORY, verbose=0, compact=True):
```

### Comparing `pyscf-2.5.0/pyscf/df/r_incore.py` & `pyscf-2.6.0/pyscf/df/r_incore.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/dft/__init__.py` & `pyscf-2.6.0/pyscf/dft/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,8 +121,9 @@
     '''X2C Kohn-Sham'''
     from pyscf.scf import dhf
     from pyscf.x2c import dft
     if dhf.zquatev and mol.spin == 0:
         return dft.RKS(mol, *args)
     else:
         return dft.UKS(mol, *args)
+X2C_KS = X2C
 gto.Mole.X2C_KS = property(X2C)
```

### Comparing `pyscf-2.5.0/pyscf/dft/dks.py` & `pyscf-2.6.0/pyscf/dft/dks.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from pyscf.dft import rks
 from pyscf.dft import gks
 from pyscf.dft import r_numint
 
 
 @lib.with_doc(gks.get_veff.__doc__)
 def get_veff(ks, mol=None, dm=None, dm_last=0, vhf_last=0, hermi=1):
-    if ks.nlc or ks._numint.libxc.is_nlc(ks.xc):
+    if ks.do_nlc():
         raise NotImplementedError(f'NLC functional {ks.xc} + {ks.nlc}')
     return gks.get_veff(ks, mol, dm, dm_last, vhf_last, hermi)
 
 
 def energy_elec(ks, dm=None, h1e=None, vhf=None):
     r'''Electronic part of DKS energy.
 
@@ -80,14 +80,21 @@
     @property
     def collinear(self):
         return self._numint.collinear
     @collinear.setter
     def collinear(self, val):
         self._numint.collinear = val
 
+    @property
+    def spin_samples(self):
+        return self._numint.spin_samples
+    @spin_samples.setter
+    def spin_samples(self, val):
+        self._numint.spin_samples = val
+
     def to_rhf(self):
         raise RuntimeError
 
     def to_uhf(self):
         raise RuntimeError
 
     def to_ghf(self):
@@ -139,14 +146,16 @@
     def x2c1e(self):
         from pyscf.x2c import dft
         x2chf = dft.UKS(self.mol)
         x2chf.__dict__.update(self.__dict__)
         return x2chf
     x2c = x2c1e
 
+    to_gpu = lib.to_gpu
+
 UKS = UDKS = DKS
 
 class RDKS(DKS, dhf.RDHF):
     '''Kramers restricted Dirac-Kohn-Sham'''
     def __init__(self, mol, xc='LDA,VWN'):
         dhf.RDHF.__init__(self, mol)
         KohnShamDFT.__init__(self, xc)
```

### Comparing `pyscf-2.5.0/pyscf/dft/gen_grid.py` & `pyscf-2.6.0/pyscf/dft/gen_grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,64 +27,27 @@
 
 import sys
 import ctypes
 import numpy
 from pyscf import lib
 from pyscf.lib import logger
 from pyscf.dft import radi
+from pyscf.dft.LebedevGrid import LEBEDEV_ORDER, LEBEDEV_NGRID, MakeAngularGrid
 from pyscf import gto
 from pyscf.gto.eval_gto import BLKSIZE, NBINS, CUTOFF, make_screen_index
 from pyscf import __config__
 
 libdft = lib.load_library('libdft')
 
 GROUP_BOX_SIZE = 1.2
 GROUP_BOUNDARY_PENALTY = 4.2
 # Padding grids to make the AO value generated by eval_gto aligned in memory
 ALIGNMENT_UNIT = 8
 NELEC_ERROR_TOL = getattr(__config__, 'dft_rks_prune_error_tol', 0.02)
 
-# ~= (L+1)**2/3
-LEBEDEV_ORDER = {
-    0  : 1   ,
-    3  : 6   ,
-    5  : 14  ,
-    7  : 26  ,
-    9  : 38  ,
-    11 : 50  ,
-    13 : 74  ,
-    15 : 86  ,
-    17 : 110 ,
-    19 : 146 ,
-    21 : 170 ,
-    23 : 194 ,
-    25 : 230 ,
-    27 : 266 ,
-    29 : 302 ,
-    31 : 350 ,
-    35 : 434 ,
-    41 : 590 ,
-    47 : 770 ,
-    53 : 974 ,
-    59 : 1202,
-    65 : 1454,
-    71 : 1730,
-    77 : 2030,
-    83 : 2354,
-    89 : 2702,
-    95 : 3074,
-    101: 3470,
-    107: 3890,
-    113: 4334,
-    119: 4802,
-    125: 5294,
-    131: 5810
-}
-LEBEDEV_NGRID = numpy.array(list(LEBEDEV_ORDER.values()))
-
 # SG0
 # S. Chien and P. Gill,  J. Comput. Chem. 27 (2006) 730-739.
 
 
 def sg1_prune(nuc, rads, n_ang, radii=radi.SG1RADII):
     '''SG1, CPL, 209, 506
 
@@ -261,17 +224,15 @@
             logger.debug(mol, 'atom %s rad-grids = %d, ang-grids = %s',
                          symb, n_rad, angs)
 
             angs = numpy.array(angs)
             coords = []
             vol = []
             for n in sorted(set(angs)):
-                grid = numpy.empty((n,4))
-                libdft.MakeAngularGrid(grid.ctypes.data_as(ctypes.c_void_p),
-                                       ctypes.c_int(n))
+                grid = MakeAngularGrid(n)
                 idx = numpy.where(angs==n)[0]
                 #coords.append(numpy.einsum('i,jk->jik', rad[idx], grid[:,:3]).reshape(-1,3))
                 #vol.append(numpy.einsum('i,j->ji', rad_weight[idx], grid[:,3]).ravel())
                 for i0, i1 in lib.prange(0, len(idx), 12):  # 12 radi-grids as a group
                     coords.append(numpy.einsum('i,jk->jik',rad[idx[i0:i1]],
                                                grid[:,:3]).reshape(-1,3))
                     vol.append(numpy.einsum('i,j->ji', rad_weight[idx[i0:i1]],
@@ -622,17 +583,15 @@
                     self.coords = numpy.vstack(
                         [self.coords, numpy.repeat([[1e-4]*3], padding, axis=0)])
                     self.weights = numpy.hstack([self.weights, numpy.zeros(padding)])
             self.non0tab = self.make_mask(mol, self.coords)
             self.screen_index = self.non0tab
         return self
 
-    def to_gpu(self):
-        from gpu4pyscf.dft.gen_grid import Grids
-        return lib.to_gpu(self.view(Grids))
+    to_gpu = lib.to_gpu
 
 
 def _default_rad(nuc, level=3):
     '''Number of radial grids '''
     tab   = numpy.array( (2 , 10, 18, 36, 54, 86, 118))
     period = (nuc > tab).sum()
     return RAD_GRIDS[level,period]
```

### Comparing `pyscf-2.5.0/pyscf/dft/gen_libxc_param.py` & `pyscf-2.6.0/pyscf/dft/gen_libxc_param.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/dft/gen_xcfun_param.py` & `pyscf-2.6.0/pyscf/dft/gen_xcfun_param.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/dft/gks.py` & `pyscf-2.6.0/pyscf/dft/gks.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         n, exc, vxc = 0, 0, 0
     else:
         max_memory = ks.max_memory - lib.current_memory()[0]
         ni = ks._numint
         n, exc, vxc = ni.get_vxc(mol, ks.grids, ks.xc, dm,
                                  hermi=hermi, max_memory=max_memory)
         logger.debug(ks, 'nelec by numeric integration = %s', n)
-        if ks.nlc or ni.libxc.is_nlc(ks.xc):
+        if ks.do_nlc():
             if ni.libxc.is_nlc(ks.xc):
                 xc = ks.xc
             else:
                 assert ni.libxc.is_nlc(ks.nlc)
                 xc = ks.nlc
             n, enlc, vnlc = ni.nr_nlc_vxc(mol, ks.nlcgrids, xc, dm,
                                           hermi=hermi, max_memory=max_memory)
@@ -173,16 +173,15 @@
     def nuc_grad_method(self):
         raise NotImplementedError
 
     def to_hf(self):
         '''Convert to GHF object.'''
         return self._transfer_attrs_(self.mol.GHF())
 
-    def to_gpu(self):
-        raise NotImplementedError
+    to_gpu = lib.to_gpu
 
 
 if __name__ == '__main__':
     from pyscf import gto
     mol = gto.Mole()
     mol.verbose = 3
     mol.atom = 'H 0 0 0; H 0 0 1; O .5 .6 .2'
```

### Comparing `pyscf-2.5.0/pyscf/dft/gks_symm.py` & `pyscf-2.6.0/pyscf/dft/gks_symm.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # Author: Qiming Sun <osirpt.sun@gmail.com>
 #
 
 '''
 Generalized Kohn-Sham
 '''
 
+from pyscf import lib
 from pyscf.lib import logger
 from pyscf.scf import ghf_symm
 from pyscf.dft import gks
 from pyscf.dft import rks
 from pyscf.dft.numint2c import NumInt2C
 
 
@@ -53,14 +54,16 @@
     @collinear.setter
     def collinear(self, val):
         self._numint.collinear = val
 
     def nuc_grad_method(self):
         raise NotImplementedError
 
+    to_gpu = lib.to_gpu
+
 
 if __name__ == '__main__':
     import numpy
     from pyscf import gto
     mol = gto.Mole()
     mol.verbose = 3
     mol.atom = 'H 0 0 0; H 0 0 1; O .5 .6 .2'
```

### Comparing `pyscf-2.5.0/pyscf/dft/libxc.py` & `pyscf-2.6.0/pyscf/dft/libxc.py`

 * *Files 2% similar despite different names*

```diff
@@ -918,14 +918,15 @@
     return xc_type(xc_code) == 'MGGA'
 
 def is_gga(xc_code):
     return xc_type(xc_code) == 'GGA'
 
 @lru_cache(100)
 def is_nlc(xc_code):
+    # identify nlc by xc_code itself if enable_nlc is None
     if isinstance(xc_code, str):
         if xc_code.isdigit():
             return _itrf.LIBXC_is_nlc(ctypes.c_int(int(xc_code)))
         else:
             fn_facs = parse_xc(xc_code)[1]
             return any(_itrf.LIBXC_is_nlc(ctypes.c_int(xid)) for xid, fac in fn_facs)
     elif numpy.issubdtype(type(xc_code), numpy.integer):
@@ -1083,23 +1084,30 @@
             The X and C functional are separated by comma like '.8*LDA+.2*B86,VWN'.
             If "HF" was appeared in the string, it stands for the exact exchange.
 
     Returns:
         decoded XC description, with the data structure
         (hybrid, alpha, omega), ((libxc-Id, fac), (libxc-Id, fac), ...)
     '''  # noqa: E501
+
     hyb = [0, 0, 0]  # hybrid, alpha, omega (== SR_HF, LR_HF, omega)
     if description is None:
         return tuple(hyb), ()
     elif numpy.issubdtype(type(description), numpy.integer):
         return tuple(hyb), ((description, 1.),)
     elif not isinstance(description, str): #isinstance(description, (tuple,list)):
         return parse_xc('%s,%s' % tuple(description))
 
-    if (description.upper() in ('B3P86', 'B3LYP', 'X3LYP') and
+    description = description.upper()
+    if '-D3' in description or '-D4' in description:
+        from pyscf.scf.dispersion import parse_dft
+        description, _, _ = parse_dft(description)
+        description = description.upper()
+
+    if (description in ('B3P86', 'B3LYP', 'X3LYP') and
         not getattr(parse_xc, 'b3lyp5_warned', False) and
         not hasattr(__config__, 'B3LYP_WITH_VWN5')):
         parse_xc.b3lyp5_warned = True
         warnings.warn('Since PySCF-2.3, B3LYP (and B3P86) are changed to the VWN-RPA variant, '
                       'corresponding to the original definition by Stephens et al. (issue 1480) '
                       'and the same as the B3LYP functional in Gaussian. '
                       'To restore the VWN5 definition, you can put the setting '
@@ -1178,16 +1186,16 @@
                                              % (key, key, key))
                         else:
                             x_id = possible_xc.pop()
                         x_id = XC_CODES[x_id]
                     else:
                         # Some libxc functionals may not be listed in the
                         # XC_CODES table. Query libxc directly
-                        func_id = _itrf.xc_functional_get_number(ctypes.c_char_p(key.encode()))
-                        if func_id == -1:
+                        x_id = _itrf.xc_functional_get_number(ctypes.c_char_p(key.encode()))
+                        if x_id == -1:
                             raise KeyError(f"LibXCFunctional: name '{key}' not found.")
                 if isinstance(x_id, str):
                     hyb1, fn_facs1 = parse_xc(x_id)
                     # Recursively scale the composed functional, to support e.g. '0.5*b3lyp'
                     if hyb1[0] != 0 or hyb1[1] != 0:
                         assign_omega(hyb1[2], hyb1[0]*fac, hyb1[1]*fac)
                     fn_facs.extend([(xid, c*fac) for xid, c in fn_facs1])
@@ -1227,14 +1235,16 @@
         x_code, c_code = description.split(',')
         for token in x_code.replace('-', '+-').replace(';+', ';').split('+'):
             parse_token(token, 'X or K')
         for token in c_code.replace('-', '+-').replace(';+', ';').split('+'):
             parse_token(token, 'C')
     else:
         for token in description.replace('-', '+-').replace(';+', ';').split('+'):
+            # dftd3 cannot be used in a custom xc description
+            assert '-d3' not in token
             parse_token(token, 'compound XC', search_xc_alias=True)
     if hyb[2] == 0: # No omega is assigned. LR_HF is 0 for normal Coulomb operator
         hyb[1] = 0
     return tuple(hyb), tuple(remove_dup(fn_facs))
 
 _NAME_WITH_DASH = {'SR-HF'    : 'SR_HF',
                    'LR-HF'    : 'LR_HF',
@@ -1247,14 +1257,15 @@
                    'HCTH-93'  : 'HCTH_93',
                    'HCTH-120' : 'HCTH_120',
                    'HCTH-147' : 'HCTH_147',
                    'HCTH-407' : 'HCTH_407',
                    'WB97X-D'  : 'WB97X_D',
                    'WB97X-V'  : 'WB97X_V',
                    'WB97M-V'  : 'WB97M_V',
+                   'WB97X-D3' : 'WB97X_D3',
                    'B97M-V'   : 'B97M_V',
                    'M05-2X'   : 'M05_2X',
                    'M06-L'    : 'M06_L',
                    'M06-HF'   : 'M06_HF',
                    'M06-2X'   : 'M06_2X',
                    'M08-HX'   : 'M08_HX',
                    'M08-SO'   : 'M08_SO',
```

### Comparing `pyscf-2.5.0/pyscf/dft/numint.py` & `pyscf-2.6.0/pyscf/dft/numint.py`

 * *Files 1% similar despite different names*

```diff
@@ -2862,18 +2862,19 @@
                                       sindex, xctype, with_lapl)
             else:
                 return self.eval_rho(mol, ao, dms[idm], sindex, xctype, hermi,
                                      with_lapl)
         return make_rho, ndms, nao
 
     def to_gpu(self):
-        from gpu4pyscf.dft.numint import NumInt
-        # Note: gpu4pyscf NumInt initializes additional things in __init__.py
-        return NumInt()
-
+        try:
+            from gpu4pyscf.dft import numint # type: ignore
+            return numint.NumInt()
+        except ImportError:
+            raise ImportError('Cannot find GPU4PySCF')
 _NumInt = NumInt
 
 
 if __name__ == '__main__':
     from pyscf import gto
     from pyscf import dft
```

### Comparing `pyscf-2.5.0/pyscf/dft/numint2c.py` & `pyscf-2.6.0/pyscf/dft/numint2c.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/dft/r_numint.py` & `pyscf-2.6.0/pyscf/dft/r_numint.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/dft/radi.py` & `pyscf-2.6.0/pyscf/dft/radi.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/dft/rks.py` & `pyscf-2.6.0/pyscf/dft/rks.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 import numpy
 from pyscf import lib
 from pyscf.lib import logger
 from pyscf import scf
 from pyscf.scf import hf
 from pyscf.scf import _vhf
 from pyscf.scf import jk
+from pyscf.scf.dispersion import parse_dft
 from pyscf.dft import gen_grid
 from pyscf.dft import numint
 from pyscf import __config__
 
-
 def get_veff(ks, mol=None, dm=None, dm_last=0, vhf_last=0, hermi=1):
     '''Coulomb + XC functional
 
     .. note::
         This function will modify the input ks object.
 
     Args:
@@ -75,15 +75,15 @@
     ni = ks._numint
     if hermi == 2:  # because rho = 0
         n, exc, vxc = 0, 0, 0
     else:
         max_memory = ks.max_memory - lib.current_memory()[0]
         n, exc, vxc = ni.nr_rks(mol, ks.grids, ks.xc, dm, max_memory=max_memory)
         logger.debug(ks, 'nelec by numeric integration = %s', n)
-        if ks.nlc or ni.libxc.is_nlc(ks.xc):
+        if ks.do_nlc():
             if ni.libxc.is_nlc(ks.xc):
                 xc = ks.xc
             else:
                 assert ni.libxc.is_nlc(ks.nlc)
                 xc = ks.nlc
             n, enlc, vnlc = ni.nr_nlc_vxc(mol, ks.nlcgrids, xc, dm,
                                           max_memory=max_memory)
@@ -256,15 +256,14 @@
     return grids.prune_by_density_(rho, ks.small_rho_cutoff)
 
 def define_xc_(ks, description, xctype='LDA', hyb=0, rsh=(0,0,0)):
     libxc = ks._numint.libxc
     ks._numint = libxc.define_xc_(ks._numint, description, xctype, hyb, rsh)
     return ks
 
-
 def _dft_common_init_(mf, xc='LDA,VWN'):
     raise DeprecationWarning
 
 class KohnShamDFT:
     '''
     Attributes for Kohn-Sham DFT:
         xc : str
@@ -317,19 +316,21 @@
     >>> mol = gto.M(atom='O 0 0 0; H 0 0 1; H 0 1 0', basis='ccpvdz', verbose=0)
     >>> mf = dft.RKS(mol)
     >>> mf.xc = 'b3lyp'
     >>> mf.kernel()
     -76.415443079840458
     '''
 
-    _keys = {'xc', 'nlc', 'grids', 'nlcgrids', 'small_rho_cutoff'}
+    _keys = {'xc', 'nlc', 'grids', 'disp', 'nlcgrids', 'small_rho_cutoff'}
 
     def __init__(self, xc='LDA,VWN'):
+        # By default, self.nlc = '' and self.disp = None
         self.xc = xc
         self.nlc = ''
+        self.disp = None
         self.grids = gen_grid.Grids(self.mol)
         self.grids.level = getattr(
             __config__, 'dft_rks_RKS_grids_level', self.grids.level)
         self.nlcgrids = gen_grid.Grids(self.mol)
         self.nlcgrids.level = getattr(
             __config__, 'dft_rks_RKS_nlcgrids_level', self.nlcgrids.level)
         # Use rho to filter grids
@@ -356,27 +357,49 @@
         if log.verbose >= logger.INFO:
             log.info('XC functionals = %s', self.xc)
             if hasattr(self._numint.libxc, 'xc_reference'):
                 log.info(textwrap.indent('\n'.join(self._numint.libxc.xc_reference(self.xc)), '    '))
 
         self.grids.dump_flags(verbose)
 
-        if self.nlc or self._numint.libxc.is_nlc(self.xc):
+        if self.do_nlc():
             log.info('** Following is NLC and NLC Grids **')
             if self.nlc:
                 log.info('NLC functional = %s', self.nlc)
             else:
                 log.info('NLC functional = %s', self.xc)
             self.nlcgrids.dump_flags(verbose)
 
         log.info('small_rho_cutoff = %g', self.small_rho_cutoff)
         return self
 
     define_xc_ = define_xc_
 
+    def do_nlc(self):
+        '''Check if the object needs to do nlc calculations
+
+        if self.nlc == False (or 0), nlc is disabled regardless the value of self.xc
+        if self.nlc == 'vv10', do nlc (vv10) regardless the value of self.xc
+        if self.nlc == '', determined by self.xc, certain xc allows the nlc part
+        '''
+        xc, nlc, _ = parse_dft(self.xc)
+        # If nlc is disabled via self.xc
+        if nlc == 0:
+            if self.nlc == '' or self.nlc == 0:
+                return False
+            else:
+                raise RuntimeError('Conflict found between dispersion and xc.')
+
+        # If nlc is disabled via self.nlc
+        if self.nlc == 0:
+            return False
+
+        xc_has_nlc = self._numint.libxc.is_nlc(xc)
+        return self.nlc == 'vv10' or xc_has_nlc
+
     def to_rhf(self):
         '''Convert the input mean-field object to a RHF/ROHF object.
 
         Note this conversion only changes the class of the mean-field object.
         The total energy and wave-function are the same as them in the input
         mean-field object.
         '''
@@ -453,29 +476,37 @@
 
     def reset(self, mol=None):
         hf.SCF.reset(self, mol)
         self.grids.reset(mol)
         self.nlcgrids.reset(mol)
         return self
 
+    def check_sanity(self):
+        out = super().check_sanity()
+        if self.do_nlc() and self.do_disp() and self._numint.libxc.is_nlc(self.xc):
+            import warnings
+            warnings.warn(
+                f'nlc-type xc {self.xc} and disp {self.disp} may lead to'
+                'double counting in NLC.')
+        return out
+
     def initialize_grids(self, mol=None, dm=None):
         '''Initialize self.grids the first time call get_veff'''
         if mol is None: mol = self.mol
 
         ground_state = getattr(dm, 'ndim', 0) == 2
         if self.grids.coords is None:
             t0 = (logger.process_clock(), logger.perf_counter())
             self.grids.build(with_non0tab=True)
             if self.small_rho_cutoff > 1e-20 and ground_state:
                 # Filter grids the first time setup grids
                 self.grids = prune_small_rho_grids_(self, self.mol, dm,
                                                     self.grids)
             t0 = logger.timer(self, 'setting up grids', *t0)
-
-        is_nlc = self.nlc or self._numint.libxc.is_nlc(self.xc)
+        is_nlc = self.do_nlc()
         if is_nlc and self.nlcgrids.coords is None:
             t0 = (logger.process_clock(), logger.perf_counter())
             self.nlcgrids.build(with_non0tab=True)
             if self.small_rho_cutoff > 1e-20 and ground_state:
                 # Filter grids the first time setup grids
                 self.nlcgrids = prune_small_rho_grids_(self, self.mol, dm,
                                                        self.nlcgrids)
@@ -527,13 +558,8 @@
         from pyscf.grad import rks as rks_grad
         return rks_grad.Gradients(self)
 
     def to_hf(self):
         '''Convert to RHF object.'''
         return self._transfer_attrs_(self.mol.RHF())
 
-    def to_gpu(self):
-        from gpu4pyscf.dft.rks import RKS
-        obj = lib.to_gpu(hf.SCF.reset(self.view(RKS)))
-        # Attributes only defined in gpu4pyscf.RKS
-        obj.screen_tol = 1e-14
-        return obj
+    to_gpu = lib.to_gpu
```

### Comparing `pyscf-2.5.0/pyscf/dft/rks_symm.py` & `pyscf-2.6.0/pyscf/dft/rks_symm.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # Author: Qiming Sun <osirpt.sun@gmail.com>
 #
 
 '''
 Non-relativistic Restricted Kohn-Sham
 '''
 
+from pyscf import lib
 from pyscf.scf import hf_symm
 from pyscf.dft import rks
 from pyscf.dft import uks
 
 
 class SymAdaptedRKS(rks.KohnShamDFT, hf_symm.SymAdaptedRHF):
     ''' Restricted Kohn-Sham '''
@@ -42,20 +43,22 @@
 
     init_guess_by_vsap = rks.init_guess_by_vsap
 
     def nuc_grad_method(self):
         from pyscf.grad import rks
         return rks.Gradients(self)
 
+    to_gpu = lib.to_gpu
+
 RKS = SymAdaptedRKS
 
 
 class SymAdaptedROKS(rks.KohnShamDFT, hf_symm.SymAdaptedROHF):
     ''' Restricted Kohn-Sham '''
-    def __init__(self, mol, xc='LDA,VWN'):
+    def __init__(self, mol=None, xc='LDA,VWN'):
         hf_symm.ROHF.__init__(self, mol)
         rks.KohnShamDFT.__init__(self, xc)
 
     def dump_flags(self, verbose=None):
         hf_symm.ROHF.dump_flags(self, verbose)
         rks.KohnShamDFT.dump_flags(self, verbose)
         return self
@@ -66,14 +69,16 @@
 
     init_guess_by_vsap = rks.init_guess_by_vsap
 
     def nuc_grad_method(self):
         from pyscf.grad import roks
         return roks.Gradients(self)
 
+    to_gpu = lib.to_gpu
+
 ROKS = SymAdaptedROKS
 
 
 if __name__ == '__main__':
     from pyscf import gto
     mol = gto.Mole()
     mol.verbose = 2
```

### Comparing `pyscf-2.5.0/pyscf/dft/roks.py` & `pyscf-2.6.0/pyscf/dft/roks.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,22 +61,15 @@
         from pyscf.grad import roks
         return roks.Gradients(self)
 
     def to_hf(self):
         '''Convert to ROHF object.'''
         return self._transfer_attrs_(self.mol.ROHF())
 
-    def to_gpu(self):
-        from pyscf.scf.hf import SCF
-        from gpu4pyscf.dft.roks import ROKS
-        obj = lib.to_gpu(SCF.reset(self.view(ROKS)))
-        # Attributes only defined in gpu4pyscf.RKS
-        obj.screen_tol = 1e-14
-        obj.disp = None
-        return obj
+    to_gpu = lib.to_gpu
 
 
 if __name__ == '__main__':
     from pyscf import gto
     from pyscf.dft import xcfun
     mol = gto.Mole()
     mol.verbose = 7
```

### Comparing `pyscf-2.5.0/pyscf/dft/sap.py` & `pyscf-2.6.0/pyscf/dft/sap.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/dft/sap_data.py` & `pyscf-2.6.0/pyscf/dft/sap_data.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/dft/uks.py` & `pyscf-2.6.0/pyscf/dft/uks.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     ni = ks._numint
     if hermi == 2:  # because rho = 0
         n, exc, vxc = (0,0), 0, 0
     else:
         max_memory = ks.max_memory - lib.current_memory()[0]
         n, exc, vxc = ni.nr_uks(mol, ks.grids, ks.xc, dm, max_memory=max_memory)
         logger.debug(ks, 'nelec by numeric integration = %s', n)
-        if ks.nlc or ni.libxc.is_nlc(ks.xc):
+        if ks.do_nlc():
             if ni.libxc.is_nlc(ks.xc):
                 xc = ks.xc
             else:
                 assert ni.libxc.is_nlc(ks.nlc)
                 xc = ks.nlc
             n, enlc, vnlc = ni.nr_nlc_vxc(mol, ks.nlcgrids, xc, dm[0]+dm[1],
                                           max_memory=max_memory)
@@ -193,14 +193,8 @@
         from pyscf.grad import uks
         return uks.Gradients(self)
 
     def to_hf(self):
         '''Convert to UHF object.'''
         return self._transfer_attrs_(self.mol.UHF())
 
-    def to_gpu(self):
-        from pyscf.scf.hf import SCF
-        from gpu4pyscf.dft.uks import UKS
-        obj = lib.to_gpu(SCF.reset(self.view(UKS)))
-        # Attributes only defined in gpu4pyscf.RKS
-        obj.screen_tol = 1e-14
-        return obj
+    to_gpu = lib.to_gpu
```

### Comparing `pyscf-2.5.0/pyscf/dft/uks_symm.py` & `pyscf-2.6.0/pyscf/dft/uks_symm.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # Author: Qiming Sun <osirpt.sun@gmail.com>
 #
 
 '''
 Non-relativistic Unrestricted Kohn-Sham
 '''
 
+from pyscf import lib
 from pyscf.lib import logger
 from pyscf.scf import uhf_symm
 from pyscf.dft import uks
 from pyscf.dft import rks
 
 
 class SymAdaptedUKS(rks.KohnShamDFT, uhf_symm.UHF):
@@ -43,14 +44,16 @@
 
     init_guess_by_vsap = rks.init_guess_by_vsap
 
     def nuc_grad_method(self):
         from pyscf.grad import uks
         return uks.Gradients(self)
 
+    to_gpu = lib.to_gpu
+
 UKS = SymAdaptedUKS
 
 
 if __name__ == '__main__':
     from pyscf import gto
     mol = gto.Mole()
     mol.verbose = 7
```

### Comparing `pyscf-2.5.0/pyscf/dft/xc/utils.py` & `pyscf-2.6.0/pyscf/dft/xc/utils.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/dft/xc_deriv.py` & `pyscf-2.6.0/pyscf/dft/xc_deriv.py`

 * *Files 1% similar despite different names*

```diff
@@ -576,26 +576,27 @@
             for dim_lst in low_sigmas:
                 rest_dims = [i for i in range(xc_tensor.ndim) if i not in dim_lst]
                 for pair_comb in pair_combs:
                     xc_tensor_1 = xc_tensor.transpose(
                         [dim_lst[i] for i in pair_comb] + rest_dims)
                     xc_tensor_1[diag_idx] += xc_sub
     else:
+        i3to2x2 = _product_uniq_indices(2, 2)
         for n_pairs in range(1, order//2+1):
             p0, p1 = offsets[order-n_pairs:order-n_pairs+2]
             xc_sub = _unfold_gga(rho, xc_val[p0:p1], spin, order-n_pairs,
                                  nvar, xlen, n_pairs)
             # Just the sigma components
             xc_sub = xc_sub[(slice(2,5),) * n_pairs]
             for i in range(n_pairs):
                 xc_sub[(slice(None),)*i+(0,)] *= 2
                 xc_sub[(slice(None),)*i+(2,)] *= 2
-            sigma_idx = _product_uniq_indices(2, n_pairs*2)
-            xc_sub = xc_sub.reshape((3**n_pairs,) + xc_sub.shape[n_pairs:])
-            xc_sub = xc_sub[sigma_idx]
+            sigma_idx = (i3to2x2[(slice(None),)*2 + (np.newaxis,)*(i*2)]
+                         for i in reversed(range(n_pairs)))
+            xc_sub = xc_sub[tuple(sigma_idx)]
 
             low_sigmas = itertools.combinations(range(order), n_pairs*2)
             pair_combs = [list(itertools.chain(*p[::-1]))
                           for p in _pair_combinations(list(range(n_pairs*2)))]
             diag_idx = _diagonal_indices(nabla_idx, n_pairs)
 
             for dim_lst in low_sigmas:
```

### Comparing `pyscf-2.5.0/pyscf/dft/xcfun.py` & `pyscf-2.6.0/pyscf/dft/xcfun.py`

 * *Files 1% similar despite different names*

```diff
@@ -416,24 +416,31 @@
     if description is None:
         return tuple(hyb), ()
     elif numpy.issubdtype(type(description), numpy.integer):
         return tuple(hyb), ((description, 1.),)
     elif not isinstance(description, str): #isinstance(description, (tuple,list)):
         return parse_xc('%s,%s' % tuple(description))
 
+    description = description.upper()
+    if '-D3' in description or '-D4' in description:
+        from pyscf.scf.dispersion import parse_dft
+        description, _, _ = parse_dft(description)
+        description = description.upper()
+
     def assign_omega(omega, hyb_or_sr, lr=0):
         if hyb[2] == omega or omega == 0:
             hyb[0] += hyb_or_sr
             hyb[1] += lr
         elif hyb[2] == 0:
             hyb[0] += hyb_or_sr
             hyb[1] += lr
             hyb[2] = omega
         else:
             raise ValueError('Different values of omega found for RSH functionals')
+
     fn_facs = []
     def parse_token(token, suffix, search_xc_alias=False):
         if token:
             if token[0] == '-':
                 sign = -1
                 token = token[1:]
             else:
@@ -499,14 +506,16 @@
         x_code, c_code = description.split(',')
         for token in x_code.replace('-', '+-').replace(';+', ';').split('+'):
             parse_token(token, 'X')
         for token in c_code.replace('-', '+-').replace(';+', ';').split('+'):
             parse_token(token, 'C')
     else:
         for token in description.replace('-', '+-').replace(';+', ';').split('+'):
+            # dftd3 cannot be used in a custom xc description
+            assert '-d3' not in token
             parse_token(token, 'XC', search_xc_alias=True)
     if hyb[2] == 0: # No omega is assigned. LR_HF is 0 for normal Coulomb operator
         hyb[1] = 0
     return tuple(hyb), tuple(remove_dup(fn_facs))
 
 _NAME_WITH_DASH = {'SR-HF'  : 'SR_HF',
                    'LR-HF'  : 'LR_HF',
```

### Comparing `pyscf-2.5.0/pyscf/eph/__init__.py` & `pyscf-2.6.0/pyscf/eph/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/eph/eph_fd.py` & `pyscf-2.6.0/pyscf/eph/eph_fd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/eph/rhf.py` & `pyscf-2.6.0/pyscf/eph/rhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/eph/rks.py` & `pyscf-2.6.0/pyscf/eph/rks.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/eph/uhf.py` & `pyscf-2.6.0/pyscf/eph/uhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/eph/uks.py` & `pyscf-2.6.0/pyscf/eph/uks.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/fci/__init__.py` & `pyscf-2.6.0/pyscf/fci/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/fci/addons.py` & `pyscf-2.6.0/pyscf/fci/addons.py`

 * *Files 5% similar despite different names*

```diff
@@ -654,30 +654,23 @@
     norb_old, norb_new = ua.shape
     na_old = cistring.num_strings(norb_old, neleca)
     nb_old = cistring.num_strings(norb_old, nelecb)
     na_new = cistring.num_strings(norb_new, neleca)
     nb_new = cistring.num_strings(norb_new, nelecb)
     ci = ci.reshape(na_old, nb_old)
 
-    one_particle_strs_old = numpy.asarray([1 << i for i in range(norb_old)])
-    one_particle_strs_new = numpy.asarray([1 << i for i in range(norb_new)])
-
     if neleca == 0:
         trans_ci_a = numpy.ones((1, 1))
     else:
         trans_ci_a = numpy.zeros((na_old, na_new), dtype=ua.dtype)
-        strs_old = numpy.asarray(cistring.make_strings(range(norb_old), neleca))
-
-        # Unitary transformation array trans_ci is the overlap between two sets of CI basis.
-        occ_masks_old = (strs_old[:,None] & one_particle_strs_old) != 0
+        occ_masks_old = _init_occ_masks(norb_old, neleca, na_old)
         if norb_old == norb_new:
             occ_masks_new = occ_masks_old
         else:
-            strs_new = numpy.asarray(cistring.make_strings(range(norb_new), neleca))
-            occ_masks_new = (strs_new[:,None] & one_particle_strs_new) != 0
+            occ_masks_new = _init_occ_masks(norb_new, neleca, na_new)
 
         # Perform
         #for i in range(na_old): # old basis
         #    for j in range(na_new): # new basis
         #        uij = u[occ_masks_old[i]][:,occ_masks_new[j]]
         #        trans_ci_a[i,j] = numpy.linalg.det(uij)
         occ_idx_all_strs = numpy.where(occ_masks_new)[1].reshape(na_new,neleca)
@@ -688,22 +681,19 @@
 
     if neleca == nelecb and numpy.allclose(ua, ub):
         trans_ci_b = trans_ci_a
     elif nelecb == 0:
         trans_ci_b = numpy.ones((1, 1))
     else:
         trans_ci_b = numpy.zeros((nb_old, nb_new), dtype=ub.dtype)
-        strs_old = numpy.asarray(cistring.make_strings(range(norb_old), nelecb))
-
-        occ_masks_old = (strs_old[:,None] & one_particle_strs_old) != 0
+        occ_masks_old = _init_occ_masks(norb_old, nelecb, nb_old)
         if norb_old == norb_new:
             occ_masks_new = occ_masks_old
         else:
-            strs_new = numpy.asarray(cistring.make_strings(range(norb_new), nelecb))
-            occ_masks_new = (strs_new[:,None] & one_particle_strs_new) != 0
+            occ_masks_new = _init_occ_masks(norb_new, nelecb, nb_new)
 
         occ_idx_all_strs = numpy.where(occ_masks_new)[1].reshape(nb_new,nelecb)
         for i in range(nb_old):
             ui = ub[occ_masks_old[i]].T.copy()
             minors = ui[occ_idx_all_strs]
             trans_ci_b[i,:] = numpy.linalg.det(minors)
 
@@ -721,8 +711,21 @@
         nelec = int(numpy.sum(nelec))
     if isinstance(nelec, (int, numpy.number)):
         nelecb = (nelec-spin)//2
         neleca = nelec - nelecb
         nelec = neleca, nelecb
     return nelec
 
+def _init_occ_masks(norb, nelec, nci):
+    one_particle_strs = numpy.asarray(cistring.make_strings(range(norb), 1))
+    strs = numpy.asarray(cistring.make_strings(range(norb), nelec))
+    if norb < 64:
+        occ_masks = (strs[:,None] & one_particle_strs) != 0
+    else:
+        occ_masks = numpy.zeros((nci, norb), dtype=bool)
+        for i in range(nci):
+            for j in range(norb):
+                if one_particle_strs[j][0] in strs[i]:
+                    occ_masks[i,j] = True
+    return occ_masks
+
 del (LARGE_CI_TOL, RETURN_STRS, PENALTY)
```

### Comparing `pyscf-2.5.0/pyscf/fci/cistring.py` & `pyscf-2.6.0/pyscf/fci/cistring.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/fci/direct_ep.py` & `pyscf-2.6.0/pyscf/fci/direct_ep.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/fci/direct_nosym.py` & `pyscf-2.6.0/pyscf/fci/direct_nosym.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,15 +45,16 @@
 def contract_1e(h1e, fcivec, norb, nelec, link_index=None):
     h1e = numpy.asarray(h1e, order='C')
     fcivec = numpy.asarray(fcivec, order='C')
     link_indexa, link_indexb = _unpack(norb, nelec, link_index)
 
     na, nlinka = link_indexa.shape[:2]
     nb, nlinkb = link_indexb.shape[:2]
-    assert (fcivec.size == na*nb)
+    assert fcivec.size == na*nb
+    assert fcivec.dtype == h1e.dtype == numpy.float64
     ci1 = numpy.zeros_like(fcivec)
 
     libfci.FCIcontract_a_1e_nosym(h1e.ctypes.data_as(ctypes.c_void_p),
                                   fcivec.ctypes.data_as(ctypes.c_void_p),
                                   ci1.ctypes.data_as(ctypes.c_void_p),
                                   ctypes.c_int(norb),
                                   ctypes.c_int(na), ctypes.c_int(nb),
@@ -91,53 +92,75 @@
 
     .. math::
 
         eri_{pq,rs} = (pq|rs) - (.5/Nelec) [\sum_q (pq|qs) + \sum_p (pq|rp)]
 
     See also :func:`direct_nosym.absorb_h1e`
     '''
-    fcivec = numpy.asarray(fcivec, order='C')
     link_indexa, link_indexb = _unpack(norb, nelec, link_index)
-
     na, nlinka = link_indexa.shape[:2]
     nb, nlinkb = link_indexb.shape[:2]
-    assert (fcivec.size == na*nb)
-    ci1 = numpy.empty_like(fcivec)
-
-    libfci.FCIcontract_2es1(eri.ctypes.data_as(ctypes.c_void_p),
-                            fcivec.ctypes.data_as(ctypes.c_void_p),
-                            ci1.ctypes.data_as(ctypes.c_void_p),
-                            ctypes.c_int(norb),
-                            ctypes.c_int(na), ctypes.c_int(nb),
-                            ctypes.c_int(nlinka), ctypes.c_int(nlinkb),
-                            link_indexa.ctypes.data_as(ctypes.c_void_p),
-                            link_indexb.ctypes.data_as(ctypes.c_void_p))
-    return ci1.view(direct_spin1.FCIvector)
+    assert fcivec.size == na*nb
+    if fcivec.dtype == eri.dtype == numpy.float64:
+        fcivec = numpy.asarray(fcivec, order='C')
+        eri = numpy.asarray(eri, order='C')
+        ci1 = numpy.empty_like(fcivec)
+        libfci.FCIcontract_2es1(eri.ctypes.data_as(ctypes.c_void_p),
+                                fcivec.ctypes.data_as(ctypes.c_void_p),
+                                ci1.ctypes.data_as(ctypes.c_void_p),
+                                ctypes.c_int(norb),
+                                ctypes.c_int(na), ctypes.c_int(nb),
+                                ctypes.c_int(nlinka), ctypes.c_int(nlinkb),
+                                link_indexa.ctypes.data_as(ctypes.c_void_p),
+                                link_indexb.ctypes.data_as(ctypes.c_void_p))
+        return ci1.view(direct_spin1.FCIvector)
+
+    ciR = numpy.asarray(fcivec.real, order='C')
+    ciI = numpy.asarray(fcivec.imag, order='C')
+    eriR = numpy.asarray(eri.real, order='C')
+    eriI = numpy.asarray(eri.imag, order='C')
+    link_index = (link_indexa, link_indexb)
+    outR  = contract_2e(eriR, ciR, norb, nelec, link_index=link_index)
+    outR -= contract_2e(eriI, ciI, norb, nelec, link_index=link_index)
+    outI  = contract_2e(eriR, ciI, norb, nelec, link_index=link_index)
+    outI += contract_2e(eriI, ciR, norb, nelec, link_index=link_index)
+    out = outR.astype(numpy.complex128)
+    out.imag = outI
+    return outR
 
 def absorb_h1e(h1e, eri, norb, nelec, fac=1):
     '''Modify 2e Hamiltonian to include 1e Hamiltonian contribution.
     '''
     if not isinstance(nelec, (int, numpy.number)):
         nelec = sum(nelec)
-    h2e = ao2mo.restore(1, eri.copy(), norb).astype(h1e.dtype, copy=False)
+    if h1e.dtype == eri.dtype == numpy.float64:
+        h2e = ao2mo.restore(1, eri.copy(), norb)
+    else:
+        assert eri.ndim == 4
+        h2e = eri.astype(dtype=numpy.result_type(h1e, eri), copy=True)
     f1e = h1e - numpy.einsum('jiik->jk', h2e) * .5
     f1e = f1e * (1./(nelec+1e-100))
     for k in range(norb):
         h2e[k,k,:,:] += f1e
         h2e[:,:,k,k] += f1e
     return h2e * fac
 
 def energy(h1e, eri, fcivec, norb, nelec, link_index=None):
     '''Compute the FCI electronic energy for given Hamiltonian and FCI vector.
     '''
     h2e = absorb_h1e(h1e, eri, norb, nelec, .5)
     ci1 = contract_2e(h2e, fcivec, norb, nelec, link_index)
     return numpy.dot(fcivec.reshape(-1), ci1.reshape(-1))
 
-make_hdiag = direct_spin1.make_hdiag
+def make_hdiag(h1e, eri, norb, nelec, compress=False):
+    if h1e.dtype == numpy.complex128:
+        h1e = h1e.real.copy()
+    if eri.dtype == numpy.complex128:
+        eri = eri.real.copy()
+    return direct_spin1.make_hdiag(h1e, eri, norb, nelec, compress)
 
 
 class FCISolver(direct_spin1.FCISolver):
     def __init__(self, *args, **kwargs):
         direct_spin1.FCISolver.__init__(self, *args, **kwargs)
         # pspace constructor only supports Hermitian Hamiltonian
         self.davidson_only = True
@@ -147,23 +170,28 @@
 
     def contract_2e(self, eri, fcivec, norb, nelec, link_index=None):
         return contract_2e(eri, fcivec, norb, nelec, link_index)
 
     def absorb_h1e(self, h1e, eri, norb, nelec, fac=1):
         return absorb_h1e(h1e, eri, norb, nelec, fac)
 
+    def make_hdiag(self, h1e, eri, norb, nelec, compress=False):
+        nelec = direct_spin1._unpack_nelec(nelec, self.spin)
+        return make_hdiag(h1e, eri, norb, nelec, compress)
+
     def kernel(self, h1e, eri, norb, nelec, ci0=None,
                tol=None, lindep=None, max_cycle=None, max_space=None,
                nroots=None, davidson_only=None, pspace_size=None,
                orbsym=None, wfnsym=None, ecore=0, **kwargs):
         if isinstance(nelec, (int, numpy.number)):
             nelecb = nelec//2
             neleca = nelec - nelecb
         else:
             neleca, nelecb = nelec
+        davidson_only = True
         link_indexa = cistring.gen_linkstr_index(range(norb), neleca)
         link_indexb = cistring.gen_linkstr_index(range(norb), nelecb)
         e, c = direct_spin1.kernel_ms1(self, h1e, eri, norb, nelec, ci0,
                                        (link_indexa,link_indexb),
                                        tol, lindep, max_cycle, max_space, nroots,
                                        davidson_only, pspace_size, ecore=ecore,
                                        **kwargs)
@@ -202,46 +230,7 @@
         else:
             neleca, nelecb = nelec
         link_indexa = cistring.gen_linkstr_index(range(norb), neleca)
         link_indexb = cistring.gen_linkstr_index(range(norb), nelecb)
         return link_indexa, link_indexb
     else:
         return link_index
-
-
-if __name__ == '__main__':
-    from functools import reduce
-    from pyscf import gto
-    from pyscf import scf
-
-    mol = gto.Mole()
-    mol.verbose = 0
-    mol.output = None#"out_h2o"
-    mol.atom = [
-        ['H', ( 1.,-1.    , 0.   )],
-        ['H', ( 0.,-1.    ,-1.   )],
-        ['H', ( 1.,-0.5   ,-1.   )],
-        #['H', ( 0.,-0.5   ,-1.   )],
-        #['H', ( 0.,-0.5   ,-0.   )],
-        ['H', ( 0.,-0.    ,-1.   )],
-        ['H', ( 1.,-0.5   , 0.   )],
-        ['H', ( 0., 1.    , 1.   )],
-    ]
-
-    mol.basis = {'H': 'sto-3g'}
-    mol.build()
-
-    m = scf.RHF(mol)
-    ehf = m.scf()
-
-    cis = FCISolver(mol)
-    norb = m.mo_coeff.shape[1]
-    nelec = mol.nelectron - 2
-    h1e = reduce(numpy.dot, (m.mo_coeff.T, m.get_hcore(), m.mo_coeff))
-    eri = ao2mo.incore.general(m._eri, (m.mo_coeff,)*4, compact=False)
-    eri = eri.reshape(norb,norb,norb,norb)
-    nea = nelec//2 + 1
-    neb = nelec//2 - 1
-    nelec = (nea, neb)
-
-    e1 = cis.kernel(h1e, eri, norb, nelec)[0]
-    print(e1, e1 - -7.7466756526056004)
```

### Comparing `pyscf-2.5.0/pyscf/fci/direct_spin0.py` & `pyscf-2.6.0/pyscf/fci/direct_spin0.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,16 @@
 def contract_1e(f1e, fcivec, norb, nelec, link_index=None):
     fcivec = numpy.asarray(fcivec, order='C')
     link_index = direct_spin1._unpack(norb, nelec, link_index)
     if not isinstance(link_index, numpy.ndarray):
         # Handle computability. link_index should be (nparray, nparray)
         link_index = link_index[0]
     na, nlink = link_index.shape[:2]
-    assert (fcivec.size == na**2)
+    assert fcivec.size == na**2
+    assert fcivec.dtype == f1e.dtype == numpy.float64
     ci1 = numpy.empty_like(fcivec)
     f1e_tril = lib.pack_tril(f1e)
     libfci.FCIcontract_1e_spin0(f1e_tril.ctypes.data_as(ctypes.c_void_p),
                                 fcivec.ctypes.data_as(ctypes.c_void_p),
                                 ci1.ctypes.data_as(ctypes.c_void_p),
                                 ctypes.c_int(norb), ctypes.c_int(na),
                                 ctypes.c_int(nlink),
@@ -88,15 +89,16 @@
     lib.transpose_sum(eri, inplace=True)
     eri *= .5
     link_index = direct_spin1._unpack(norb, nelec, link_index)
     if not isinstance(link_index, numpy.ndarray):
         # Handle computability. link_index should be (nparray, nparray)
         link_index = link_index[0]
     na, nlink = link_index.shape[:2]
-    assert (fcivec.size == na**2)
+    assert fcivec.size == na**2
+    assert fcivec.dtype == eri.dtype == numpy.float64
     ci1 = numpy.empty((na,na))
 
     libfci.FCIcontract_2e_spin0(eri.ctypes.data_as(ctypes.c_void_p),
                                 fcivec.ctypes.data_as(ctypes.c_void_p),
                                 ci1.ctypes.data_as(ctypes.c_void_p),
                                 ctypes.c_int(norb), ctypes.c_int(na),
                                 ctypes.c_int(nlink),
```

### Comparing `pyscf-2.5.0/pyscf/fci/direct_spin0_symm.py` & `pyscf-2.6.0/pyscf/fci/direct_spin0_symm.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/fci/direct_spin1.py` & `pyscf-2.6.0/pyscf/fci/direct_spin1.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,16 @@
     '''Contract the 1-electron Hamiltonian with a FCI vector to get a new FCI
     vector.
     '''
     fcivec = numpy.asarray(fcivec, order='C')
     link_indexa, link_indexb = _unpack(norb, nelec, link_index)
     na, nlinka = link_indexa.shape[:2]
     nb, nlinkb = link_indexb.shape[:2]
-    assert (fcivec.size == na*nb)
+    assert fcivec.size == na*nb
+    assert fcivec.dtype == f1e.dtype == numpy.float64
     f1e_tril = lib.pack_tril(f1e)
     ci1 = numpy.zeros_like(fcivec)
     libfci.FCIcontract_a_1e(f1e_tril.ctypes.data_as(ctypes.c_void_p),
                             fcivec.ctypes.data_as(ctypes.c_void_p),
                             ci1.ctypes.data_as(ctypes.c_void_p),
                             ctypes.c_int(norb),
                             ctypes.c_int(na), ctypes.c_int(nb),
@@ -119,19 +120,20 @@
     .. math::
 
         eri_{pq,rs} = (pq|rs) - (.5/Nelec) [\sum_q (pq|qs) + \sum_p (pq|rp)]
 
     See also :func:`direct_spin1.absorb_h1e`
     '''
     fcivec = numpy.asarray(fcivec, order='C')
-    eri = ao2mo.restore(4, eri, norb)
+    eri = numpy.asarray(ao2mo.restore(4, eri, norb), order='C')
     link_indexa, link_indexb = _unpack(norb, nelec, link_index)
     na, nlinka = link_indexa.shape[:2]
     nb, nlinkb = link_indexb.shape[:2]
-    assert (fcivec.size == na*nb)
+    assert fcivec.size == na*nb
+    assert fcivec.dtype == eri.dtype == numpy.float64
     ci1 = numpy.empty_like(fcivec)
 
     libfci.FCIcontract_2e_spin1(eri.ctypes.data_as(ctypes.c_void_p),
                                 fcivec.ctypes.data_as(ctypes.c_void_p),
                                 ci1.ctypes.data_as(ctypes.c_void_p),
                                 ctypes.c_int(norb),
                                 ctypes.c_int(na), ctypes.c_int(nb),
@@ -142,20 +144,20 @@
 
 def make_hdiag(h1e, eri, norb, nelec, compress=False):
     '''Diagonal Hamiltonian for Davidson preconditioner
 
     Kwargs:
         compress (bool) : whether to remove symmetry forbidden elements
     '''
-    if h1e.dtype == numpy.complex128 or eri.dtype == numpy.complex128:
+    if not (h1e.dtype == eri.dtype == numpy.float64):
         raise NotImplementedError('Complex Hamiltonian')
 
     neleca, nelecb = _unpack_nelec(nelec)
     h1e = numpy.asarray(h1e, order='C')
-    eri = ao2mo.restore(1, eri, norb)
+    eri = numpy.asarray(ao2mo.restore(1, eri, norb), order='C')
     occslsta = occslstb = cistring.gen_occslst(range(norb), neleca)
     if neleca != nelecb:
         occslstb = cistring.gen_occslst(range(norb), nelecb)
     na = len(occslsta)
     nb = len(occslstb)
 
     hdiag = numpy.empty(na*nb)
@@ -939,14 +941,16 @@
 class FCISolver(FCIBase):
     # transform_ci_for_orbital_rotation only available for FCI wavefunctions.
     # Some approx FCI solver does not have this functionality.
     def transform_ci_for_orbital_rotation(self, fcivec, norb, nelec, u):
         nelec = _unpack_nelec(nelec, self.spin)
         return addons.transform_ci_for_orbital_rotation(fcivec, norb, nelec, u)
 
+    to_gpu = lib.to_gpu
+
 FCI = FCISolver
 
 class FCIvector(numpy.ndarray):
     '''An 2D np array for FCI coefficients'''
 
     # Special cases for ndarray when the array was modified (through ufunc)
     def __array_wrap__(self, out):
```

### Comparing `pyscf-2.5.0/pyscf/fci/direct_spin1_cyl_sym.py` & `pyscf-2.6.0/pyscf/fci/direct_spin1_cyl_sym.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/fci/direct_spin1_symm.py` & `pyscf-2.6.0/pyscf/fci/direct_spin1_symm.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/fci/direct_uhf.py` & `pyscf-2.6.0/pyscf/fci/direct_uhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/fci/fci_dhf_slow.py` & `pyscf-2.6.0/pyscf/fci/fci_dhf_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/fci/fci_slow.py` & `pyscf-2.6.0/pyscf/fci/fci_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/fci/rdm.py` & `pyscf-2.6.0/pyscf/fci/rdm.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/fci/selected_ci.py` & `pyscf-2.6.0/pyscf/fci/selected_ci.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/fci/selected_ci_slow.py` & `pyscf-2.6.0/pyscf/fci/selected_ci_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/fci/selected_ci_spin0.py` & `pyscf-2.6.0/pyscf/fci/selected_ci_spin0.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/fci/selected_ci_spin0_symm.py` & `pyscf-2.6.0/pyscf/fci/selected_ci_spin0_symm.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/fci/selected_ci_symm.py` & `pyscf-2.6.0/pyscf/fci/selected_ci_symm.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/fci/spin_op.py` & `pyscf-2.6.0/pyscf/fci/spin_op.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/geomopt/__init__.py` & `pyscf-2.6.0/pyscf/geomopt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/geomopt/addons.py` & `pyscf-2.6.0/pyscf/geomopt/addons.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/geomopt/berny_solver.py` & `pyscf-2.6.0/pyscf/geomopt/berny_solver.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/geomopt/geometric_solver.py` & `pyscf-2.6.0/pyscf/geomopt/geometric_solver.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/grad/__init__.py` & `pyscf-2.6.0/pyscf/grad/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     >>> grad.RHF(mf).kernel()
 '''
 
 from . import rhf
 from . import dhf
 from . import uhf
 from . import rohf
-from . import dispersion
 from .rhf import Gradients as RHF
 from .dhf import Gradients as DHF
 from .uhf import Gradients as UHF
 from .rohf import Gradients as ROHF
 
 grad_nuc = rhf.grad_nuc
 
@@ -59,10 +58,11 @@
     from . import ucisd
     from . import uks
     from . import ump2
 
     from .rks import Gradients as RKS
     from .uks import Gradients as UKS
     from .roks import Gradients as ROKS
+    from . import dispersion
 
 except (ImportError, OSError):
     pass
```

### Comparing `pyscf-2.5.0/pyscf/grad/casci.py` & `pyscf-2.6.0/pyscf/grad/casci.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,11 +338,13 @@
                 logger.note(self, '--------- %s gradients for state %d ----------',
                             self.base.__class__.__name__, self.state)
             self._write(self.mol, self.de, self.atmlst)
             logger.note(self, '----------------------------------------------')
 
     as_scanner = as_scanner
 
+    to_gpu = lib.to_gpu
+
 Grad = Gradients
 
 from pyscf import mcscf
 mcscf.casci.CASCI.Gradients = lib.class_as_method(Gradients)
```

### Comparing `pyscf-2.5.0/pyscf/grad/casscf.py` & `pyscf-2.6.0/pyscf/grad/casscf.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,11 +216,13 @@
             logger.note(self, '--------------- %s gradients ---------------',
                         self.base.__class__.__name__)
             self._write(self.mol, self.de, self.atmlst)
             logger.note(self, '----------------------------------------------')
 
     as_scanner = as_scanner
 
+    to_gpu = lib.to_gpu
+
 Grad = Gradients
 
 from pyscf import mcscf
 mcscf.mc1step.CASSCF.Gradients = lib.class_as_method(Gradients)
```

### Comparing `pyscf-2.5.0/pyscf/grad/ccsd.py` & `pyscf-2.6.0/pyscf/grad/ccsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,10 +452,12 @@
     # by external modules (e.g. QM/MM, solvent)
     def grad_nuc(self, mol=None, atmlst=None):
         mf_grad = self.base._scf.nuc_grad_method()
         return mf_grad.grad_nuc(mol, atmlst)
 
     as_scanner = as_scanner
 
+    to_gpu = lib.to_gpu
+
 Grad = Gradients
 
 ccsd.CCSD.Gradients = lib.class_as_method(Gradients)
```

### Comparing `pyscf-2.5.0/pyscf/grad/ccsd_slow.py` & `pyscf-2.6.0/pyscf/grad/ccsd_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/grad/ccsd_t.py` & `pyscf-2.6.0/pyscf/grad/ccsd_t.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/grad/cisd.py` & `pyscf-2.6.0/pyscf/grad/cisd.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,10 +199,12 @@
             logger.note(self, '--------- %s gradients for state %d ----------',
                         self.base.__class__.__name__, self.state)
             self._write(self.mol, self.de, self.atmlst)
             logger.note(self, '----------------------------------------------')
 
     as_scanner = as_scanner
 
+    to_gpu = lib.to_gpu
+
 Grad = Gradients
 
 cisd.CISD.Gradients = lib.class_as_method(Gradients)
```

### Comparing `pyscf-2.5.0/pyscf/grad/dhf.py` & `pyscf-2.6.0/pyscf/grad/dhf.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,14 +213,16 @@
             self.de = self.symmetrize(self.de, atmlst)
         logger.timer(self, 'SCF gradients', *cput0)
         self._finalize()
         return self.de
 
     as_scanner = rhf_grad.as_scanner
 
+    to_gpu = lib.to_gpu
+
 Grad = Gradients
 
 from pyscf import scf
 scf.dhf.UHF.Gradients = lib.class_as_method(Gradients)
 
 
 def _call_vhf1_llll(mol, dm):
```

### Comparing `pyscf-2.5.0/pyscf/grad/lagrange.py` & `pyscf-2.6.0/pyscf/grad/lagrange.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/grad/mp2.py` & `pyscf-2.6.0/pyscf/grad/mp2.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,11 +305,13 @@
     # by external modules (e.g. QM/MM, solvent)
     def grad_nuc(self, mol=None, atmlst=None):
         mf_grad = self.base._scf.nuc_grad_method()
         return mf_grad.grad_nuc(mol, atmlst)
 
     as_scanner = as_scanner
 
+    to_gpu = lib.to_gpu
+
 Grad = Gradients
 
 # Inject to RMP2 class
 mp2.MP2.Gradients = lib.class_as_method(Gradients)
```

### Comparing `pyscf-2.5.0/pyscf/grad/rhf.py` & `pyscf-2.6.0/pyscf/grad/rhf.py`

 * *Files 2% similar despite different names*

```diff
@@ -412,15 +412,15 @@
         if self.verbose >= logger.INFO:
             self.dump_flags()
 
         de = self.grad_elec(mo_energy, mo_coeff, mo_occ, atmlst)
         self.de = de + self.grad_nuc(atmlst=atmlst)
         if self.mol.symmetry:
             self.de = self.symmetrize(self.de, atmlst)
-        if self.base.disp is not None:
+        if self.base.do_disp():
             self.de += self.get_dispersion()
         logger.timer(self, 'SCF gradients', *cput0)
         self._finalize()
         return self.de
 
     grad = lib.alias(kernel, alias_name='grad')
 
@@ -436,16 +436,22 @@
     as_scanner = as_scanner
 
     def _tag_rdm1 (self, dm, mo_coeff, mo_occ):
         '''Tagging is necessary in DF subclass. Tagged arrays need
         to be split into alpha,beta in DF-ROHF subclass'''
         return lib.tag_array (dm, mo_coeff=mo_coeff, mo_occ=mo_occ)
 
+    # to_gpu can be reused only when __init__ still takes mf
     def to_gpu(self):
-        raise NotImplementedError
+        mf = self.base.to_gpu()
+        from importlib import import_module
+        mod = import_module(self.__module__.replace('pyscf', 'gpu4pyscf'))
+        cls = getattr(mod, self.__class__.__name__)
+        obj = cls(mf)
+        return obj
 
 # export the symbol GradientsMixin for backward compatibility.
 # GradientsMixin should be dropped in the future.
 GradientsMixin = GradientsBase
 
 class Gradients(GradientsBase):
     '''Non-relativistic restricted Hartree-Fock gradients'''
@@ -459,16 +465,12 @@
         if mo_energy is None: mo_energy = self.base.mo_energy
         if mo_coeff is None: mo_coeff = self.base.mo_coeff
         if mo_occ is None: mo_occ = self.base.mo_occ
         return make_rdm1e(mo_energy, mo_coeff, mo_occ)
 
     grad_elec = grad_elec
 
-    def to_gpu(self):
-        from gpu4pyscf.grad.rhf import Gradients
-        return lib.to_gpu(self.view(Gradients))
-
 Grad = Gradients
 
 from pyscf import scf
 # Inject to RHF class
 scf.hf.RHF.Gradients = lib.class_as_method(Gradients)
```

### Comparing `pyscf-2.5.0/pyscf/grad/rks.py` & `pyscf-2.6.0/pyscf/grad/rks.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,29 +48,29 @@
 
     mem_now = lib.current_memory()[0]
     max_memory = max(2000, ks_grad.max_memory*.9-mem_now)
     if ks_grad.grid_response:
         exc, vxc = get_vxc_full_response(ni, mol, grids, mf.xc, dm,
                                          max_memory=max_memory,
                                          verbose=ks_grad.verbose)
-        if mf.nlc or ni.libxc.is_nlc(mf.xc):
+        if mf.do_nlc():
             if ni.libxc.is_nlc(mf.xc):
                 xc = mf.xc
             else:
                 xc = mf.nlc
             enlc, vnlc = get_nlc_vxc_full_response(
                 ni, mol, nlcgrids, xc, dm,
                 max_memory=max_memory, verbose=ks_grad.verbose)
             exc += enlc
             vxc += vnlc
         logger.debug1(ks_grad, 'sum(grids response) %s', exc.sum(axis=0))
     else:
         exc, vxc = get_vxc(ni, mol, grids, mf.xc, dm,
                            max_memory=max_memory, verbose=ks_grad.verbose)
-        if mf.nlc or ni.libxc.is_nlc(mf.xc):
+        if mf.do_nlc():
             if ni.libxc.is_nlc(mf.xc):
                 xc = mf.xc
             else:
                 xc = mf.nlc
             enlc, vnlc = get_nlc_vxc(
                 ni, mol, nlcgrids, xc, dm,
                 max_memory=max_memory, verbose=ks_grad.verbose)
@@ -88,24 +88,23 @@
             vk += ks_grad.get_k(mol, dm, omega=omega) * (alpha - hyb)
         vxc += vj - vk * .5
 
     return lib.tag_array(vxc, exc1_grid=exc)
 
 def _initialize_grids(ks_grad):
     mf = ks_grad.base
-    ni = mf._numint
     if ks_grad.grids is not None:
         grids = ks_grad.grids
     else:
         grids = mf.grids
     if grids.coords is None:
         grids.build(with_non0tab=True)
 
     nlcgrids = None
-    if mf.nlc or ni.libxc.is_nlc(mf.xc):
+    if mf.do_nlc():
         if ks_grad.nlcgrids is not None:
             nlcgrids = ks_grad.nlcgrids
         else:
             nlcgrids = mf.nlcgrids
         if nlcgrids.coords is None:
             nlcgrids.build(with_non0tab=True)
     return grids, nlcgrids
@@ -587,17 +586,14 @@
 
     _keys = {'grid_response', 'grids', 'nlcgrids'}
 
     def __init__(self, mf):
         rhf_grad.Gradients.__init__(self, mf)
         self.grids = None
         self.nlcgrids = None
-        # This parameter has no effects for HF gradients. Add this attribute so that
-        # the kernel function can be reused in the DFT gradients code.
-        self.grid_response = False
 
     def dump_flags(self, verbose=None):
         rhf_grad.Gradients.dump_flags(self, verbose)
         logger.info(self, 'grid_response = %s', self.grid_response)
         #if callable(self.base.grids.prune):
         #    logger.info(self, 'Grid pruning %s may affect DFT gradients accuracy.'
         #                'Call mf.grids.run(prune=False) to mute grid pruning',
@@ -618,15 +614,11 @@
             log = envs['log']
             log.debug('grids response for atom %d %s',
                       atom_id, vhf.exc1_grid[atom_id])
             return vhf.exc1_grid[atom_id]
         else:
             return 0
 
-    def to_gpu(self):
-        from gpu4pyscf.grad.rks import Gradients
-        return lib.to_gpu(self.view(Gradients))
-
 Grad = Gradients
 
 from pyscf import dft
 dft.rks.RKS.Gradients = dft.rks_symm.RKS.Gradients = lib.class_as_method(Gradients)
```

### Comparing `pyscf-2.5.0/pyscf/grad/rohf.py` & `pyscf-2.6.0/pyscf/grad/rohf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/grad/roks.py` & `pyscf-2.6.0/pyscf/grad/roks.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/grad/sacasscf.py` & `pyscf-2.6.0/pyscf/grad/sacasscf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/grad/tdrhf.py` & `pyscf-2.6.0/pyscf/grad/tdrhf.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,11 +321,13 @@
             logger.note(self, '--------- %s gradients for state %d ----------',
                         self.base.__class__.__name__, self.state)
             self._write(self.mol, self.de, self.atmlst)
             logger.note(self, '----------------------------------------------')
 
     as_scanner = as_scanner
 
+    to_gpu = lib.to_gpu
+
 Grad = Gradients
 
 from pyscf import tdscf
 tdscf.rhf.TDA.Gradients = tdscf.rhf.TDHF.Gradients = lib.class_as_method(Gradients)
```

### Comparing `pyscf-2.5.0/pyscf/grad/tdrks.py` & `pyscf-2.6.0/pyscf/grad/tdrks.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/grad/tduhf.py` & `pyscf-2.6.0/pyscf/grad/tduhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/grad/tduks.py` & `pyscf-2.6.0/pyscf/grad/tduks.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/grad/uccsd.py` & `pyscf-2.6.0/pyscf/grad/uccsd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/grad/uccsd_t.py` & `pyscf-2.6.0/pyscf/grad/uccsd_t.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/grad/ucisd.py` & `pyscf-2.6.0/pyscf/grad/ucisd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/grad/uhf.py` & `pyscf-2.6.0/pyscf/grad/uhf.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,11 @@
         if mo_energy is None: mo_energy = self.base.mo_energy
         if mo_coeff is None: mo_coeff = self.base.mo_coeff
         if mo_occ is None: mo_occ = self.base.mo_occ
         return make_rdm1e(mo_energy, mo_coeff, mo_occ)
 
     grad_elec = grad_elec
 
-    def to_gpu(self):
-        raise NotImplementedError
-
 Grad = Gradients
 
 from pyscf import scf
 scf.uhf.UHF.Gradients = lib.class_as_method(Gradients)
```

### Comparing `pyscf-2.5.0/pyscf/grad/uks.py` & `pyscf-2.6.0/pyscf/grad/uks.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,29 +46,29 @@
     ni = mf._numint
     mem_now = lib.current_memory()[0]
     max_memory = max(2000, ks_grad.max_memory*.9-mem_now)
     if ks_grad.grid_response:
         exc, vxc = get_vxc_full_response(ni, mol, grids, mf.xc, dm,
                                          max_memory=max_memory,
                                          verbose=ks_grad.verbose)
-        if mf.nlc or ni.libxc.is_nlc(mf.xc):
+        if mf.do_nlc():
             if ni.libxc.is_nlc(mf.xc):
                 xc = mf.xc
             else:
                 xc = mf.nlc
             enlc, vnlc = rks_grad.get_nlc_vxc_full_response(
                 ni, mol, nlcgrids, xc, dm[0]+dm[1],
                 max_memory=max_memory, verbose=ks_grad.verbose)
             exc += enlc
             vxc += vnlc
         logger.debug1(ks_grad, 'sum(grids response) %s', exc.sum(axis=0))
     else:
         exc, vxc = get_vxc(ni, mol, grids, mf.xc, dm,
                            max_memory=max_memory, verbose=ks_grad.verbose)
-        if mf.nlc or ni.libxc.is_nlc(mf.xc):
+        if mf.do_nlc():
             if ni.libxc.is_nlc(mf.xc):
                 xc = mf.xc
             else:
                 xc = mf.nlc
             enlc, vnlc = rks_grad.get_nlc_vxc(
                 ni, mol, nlcgrids, xc, dm[0]+dm[1],
                 max_memory=max_memory, verbose=ks_grad.verbose)
@@ -246,15 +246,14 @@
 
     _keys = {'grid_response', 'grids', 'nlcgrids'}
 
     def __init__(self, mf):
         uhf_grad.Gradients.__init__(self, mf)
         self.grids = None
         self.nlcgrids = None
-        self.grid_response = False
 
     def dump_flags(self, verbose=None):
         uhf_grad.Gradients.dump_flags(self, verbose)
         logger.info(self, 'grid_response = %s', self.grid_response)
         return self
 
     get_veff = get_veff
@@ -271,14 +270,11 @@
             log = envs['log']
             log.debug('grids response for atom %d %s',
                       atom_id, vhf.exc1_grid[atom_id])
             return vhf.exc1_grid[atom_id]
         else:
             return 0
 
-    def to_gpu(self):
-        raise NotImplementedError
-
 Grad = Gradients
 
 from pyscf import dft
 dft.uks.UKS.Gradients = dft.uks_symm.UKS.Gradients = lib.class_as_method(Gradients)
```

### Comparing `pyscf-2.5.0/pyscf/grad/ump2.py` & `pyscf-2.6.0/pyscf/grad/ump2.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/__init__.py` & `pyscf-2.6.0/pyscf/gto/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/Burkatzi-Filippi-Dolg-PP.dat` & `pyscf-2.6.0/pyscf/gto/basis/Burkatzi-Filippi-Dolg-PP.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/DgaussA1_dft_cfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/DgaussA1_dft_cfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/DgaussA1_dft_xfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/DgaussA1_dft_xfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/DgaussA2_dft_cfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/DgaussA2_dft_cfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/DgaussA2_dft_xfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/DgaussA2_dft_xfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/__init__.py` & `pyscf-2.6.0/pyscf/gto/basis/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/adzp.dat` & `pyscf-2.6.0/pyscf/gto/basis/adzp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ahlrichs_cfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/ahlrichs_cfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ano.dat` & `pyscf-2.6.0/pyscf/gto/basis/ano.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aqzp.dat` & `pyscf-2.6.0/pyscf/gto/basis/aqzp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/atzp.dat` & `pyscf-2.6.0/pyscf/gto/basis/atzp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pV5Z-PP.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pV5Z-PP.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pV5Z_MP2FIT.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pV5Z_MP2FIT.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pVDZ-PP.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pVDZ-PP.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pVQZ-DK3.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pVQZ-DK3.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pVQZ-PP.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pVQZ-PP.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pVQZ_MP2FIT.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pVQZ_MP2FIT.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pVTZ-DK3.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pVTZ-DK3.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pVTZ-PP.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pVTZ-PP.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pv5z-dk.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pv5z-dk.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pv5z-jkfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pv5z-jkfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pv5z-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pv5z-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pv5z.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pv5z.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvdpdz.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvdpdz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvdz-dk.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvdz-dk.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvdz-jkfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvdz-jkfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvdz-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvdz-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvdz.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvdz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvdzp-jkfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvdzp-jkfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvdzp-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvdzp-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvqz-dk.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvqz-dk.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvqz-jkfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvqz-jkfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvqz-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvqz-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvqz.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvqz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvtz-dk.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvtz-dk.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvtz-jkfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvtz-jkfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvtz-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvtz-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pvtz.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pvtz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwCVQZ-DK.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwCVQZ-DK.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwCVQZ-DK3.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwCVQZ-DK3.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwCVTZ-DK.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwCVTZ-DK.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwCVTZ-DK3.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwCVTZ-DK3.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwCVTZ_MP2FIT.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwCVTZ_MP2FIT.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwcv5z-dk.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwcv5z-dk.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwcv5z.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwcv5z.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwcvdz.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwcvdz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwcvqz.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwcvqz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-cc-pwcvtz.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-cc-pwcvtz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-pc-0.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-pc-0.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-pc-1.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-pc-1.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-pc-2.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-pc-2.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-pc-3.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-pc-3.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-pc-4.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-pc-4.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-pcseg-0.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-pcseg-0.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-pcseg-1.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-pcseg-1.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-pcseg-2.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-pcseg-2.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-pcseg-3.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-pcseg-3.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/aug-pcseg-4.dat` & `pyscf-2.6.0/pyscf/gto/basis/aug-pcseg-4.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/bfd_pp.dat` & `pyscf-2.6.0/pyscf/gto/basis/bfd_pp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/bfd_v5z.dat` & `pyscf-2.6.0/pyscf/gto/basis/bfd_v5z.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/bfd_vdz.dat` & `pyscf-2.6.0/pyscf/gto/basis/bfd_vdz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/bfd_vqz.dat` & `pyscf-2.6.0/pyscf/gto/basis/bfd_vqz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/bfd_vtz.dat` & `pyscf-2.6.0/pyscf/gto/basis/bfd_vtz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/bse.py` & `pyscf-2.6.0/pyscf/gto/basis/bse.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pCV5Z.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pCV5Z.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pCV6Z.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pCV6Z.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pCVDZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pCVDZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pCVQZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pCVQZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pCVTZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pCVTZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pV5Z_MP2FIT.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pV5Z_MP2FIT.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pVDZ-PP-NR.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pVDZ-PP-NR.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pVQZ-DK3.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pVQZ-DK3.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pVQZ_MP2FIT.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pVQZ_MP2FIT.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pVTZ-DK3.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pVTZ-DK3.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pVTZ-PP-NR.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pVTZ-PP-NR.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pv5z-dk.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pv5z-dk.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pv5z-jkfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pv5z-jkfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pv5z-pp.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pv5z-pp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pv5z-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pv5z-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pv5z.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pv5z.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pvdpdz.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pvdpdz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pvdz-dk.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pvdz-dk.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pvdz-jkfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pvdz-jkfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pvdz-pp.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pvdz-pp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pvdz-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pvdz-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pvdz.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pvdz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pvdz_fit.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pvdz_fit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pvqz-dk.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pvqz-dk.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pvqz-jkfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pvqz-jkfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pvqz-pp.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pvqz-pp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pvqz-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pvqz-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pvqz.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pvqz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pvtz-dk.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pvtz-dk.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pvtz-jkfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pvtz-jkfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pvtz-pp.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pvtz-pp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pvtz-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pvtz-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pvtz.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pvtz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pvtz_fit.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pvtz_fit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pwCV5Z-DK.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pwCV5Z-DK.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pwCV5Z-PP.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pwCV5Z-PP.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pwCV5Z.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pwCV5Z.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pwCVDZ-DK.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pwCVDZ-DK.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pwCVDZ-PP.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pwCVDZ-PP.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pwCVDZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pwCVDZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pwCVQZ-DK.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pwCVQZ-DK.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pwCVQZ-DK3.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pwCVQZ-DK3.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pwCVQZ-PP.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pwCVQZ-PP.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pwCVQZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pwCVQZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pwCVTZ-DK.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pwCVTZ-DK.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pwCVTZ-DK3.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pwCVTZ-DK3.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pwCVTZ-PP.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pwCVTZ-PP.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pwCVTZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pwCVTZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/cc-pwCVTZ_MP2FIT.dat` & `pyscf-2.6.0/pyscf/gto/basis/cc-pwCVTZ_MP2FIT.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pV5Z.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pV5Z.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pV6Z.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pV6Z.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pVDZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pVDZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pVQZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pVQZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pVTZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_aug-cc-pVTZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pV5Z.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pV5Z.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pV6Z.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pV6Z.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pVDZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pVDZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pVQZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pVQZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pVTZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP/ccECP_cc-pVTZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_aug-cc-pV5Z.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_aug-cc-pV5Z.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_aug-cc-pVDZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_aug-cc-pVDZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_aug-cc-pVQZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_aug-cc-pVQZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_aug-cc-pVTZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_aug-cc-pVTZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_cc-pV5Z.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_cc-pV5Z.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_cc-pVDZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_cc-pVDZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_cc-pVQZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_cc-pVQZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_cc-pVTZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_He_core/ccECP_cc-pVTZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_aug-cc-pV5Z.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_aug-cc-pV5Z.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_aug-cc-pVDZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_aug-cc-pVDZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_aug-cc-pVQZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_aug-cc-pVQZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_aug-cc-pVTZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_aug-cc-pVTZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_cc-pV5Z.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_cc-pV5Z.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_cc-pVDZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_cc-pVDZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_cc-pVQZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_cc-pVQZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_cc-pVTZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/ccecp-basis/ccECP_reg/ccECP_cc-pVTZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/crenbl.dat` & `pyscf-2.6.0/pyscf/gto/basis/crenbl.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/crenbs.dat` & `pyscf-2.6.0/pyscf/gto/basis/crenbs.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/crystal-cc-pvdz.dat` & `pyscf-2.6.0/pyscf/gto/basis/crystal-cc-pvdz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-qzvp-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-qzvp-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-qzvp.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-qzvp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-qzvpd.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-qzvpd.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-qzvpp-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-qzvpp-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-qzvpp.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-qzvpp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-qzvppd-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-qzvppd-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-qzvppd.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-qzvppd.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-svp-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-svp-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-svp.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-svp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-svpd-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-svpd-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-svpd.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-svpd.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-tzvp-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-tzvp-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-tzvp.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-tzvp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-tzvpd-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-tzvpd-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-tzvpd.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-tzvpd.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-tzvpp-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-tzvpp-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-tzvpp.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-tzvpp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-tzvppd-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-tzvppd-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-tzvppd.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-tzvppd.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-universal-jfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-universal-jfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/def2-universal-jkfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/def2-universal-jkfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/demon_cfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/demon_cfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/dyall_dz.py` & `pyscf-2.6.0/pyscf/gto/basis/dyall_dz.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/dyall_qz.py` & `pyscf-2.6.0/pyscf/gto/basis/dyall_qz.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/dyall_tz.py` & `pyscf-2.6.0/pyscf/gto/basis/dyall_tz.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/dz.dat` & `pyscf-2.6.0/pyscf/gto/basis/dz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/dzp-dkh.dat` & `pyscf-2.6.0/pyscf/gto/basis/dzp-dkh.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/dzp.dat` & `pyscf-2.6.0/pyscf/gto/basis/dzp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/dzp_dunning.py` & `pyscf-2.6.0/pyscf/gto/basis/dzp_dunning.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/dzvp.dat` & `pyscf-2.6.0/pyscf/gto/basis/dzvp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/dzvp2.dat` & `pyscf-2.6.0/pyscf/gto/basis/dzvp2.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/f12-basis/aug-cc-pV5Z-OptRI.dat` & `pyscf-2.6.0/pyscf/gto/basis/f12-basis/aug-cc-pV5Z-OptRI.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/f12-basis/aug-cc-pVDZ-OptRI.dat` & `pyscf-2.6.0/pyscf/gto/basis/f12-basis/aug-cc-pVDZ-OptRI.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/f12-basis/aug-cc-pVQZ-OptRI.dat` & `pyscf-2.6.0/pyscf/gto/basis/f12-basis/aug-cc-pVQZ-OptRI.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/f12-basis/aug-cc-pVTZ-OptRI.dat` & `pyscf-2.6.0/pyscf/gto/basis/f12-basis/aug-cc-pVTZ-OptRI.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pCVDZ-F12-OptRI.dat` & `pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pCVDZ-F12-OptRI.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pCVQZ-F12-OptRI.dat` & `pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pCVQZ-F12-OptRI.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pCVTZ-F12-OptRI.dat` & `pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pCVTZ-F12-OptRI.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pV5Z-F12.dat` & `pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pV5Z-F12.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pV5Z-F12rev2.dat` & `pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pV5Z-F12rev2.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pVDZ-F12-OptRI.dat` & `pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pVDZ-F12-OptRI.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pVDZ-F12-nZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pVDZ-F12-nZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pVDZ-F12rev2.dat` & `pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pVDZ-F12rev2.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pVQZ-F12-OptRI.dat` & `pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pVQZ-F12-OptRI.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pVQZ-F12-nZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pVQZ-F12-nZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pVQZ-F12rev2.dat` & `pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pVQZ-F12rev2.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pVTZ-F12-OptRI.dat` & `pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pVTZ-F12-OptRI.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pVTZ-F12-nZ.dat` & `pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pVTZ-F12-nZ.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/f12-basis/cc-pVTZ-F12rev2.dat` & `pyscf-2.6.0/pyscf/gto/basis/f12-basis/cc-pVTZ-F12rev2.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/faegre_dz.py` & `pyscf-2.6.0/pyscf/gto/basis/faegre_dz.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/heavy-aug-cc-pvdz-jkfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/heavy-aug-cc-pvdz-jkfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/heavy-aug-cc-pvdz-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/heavy-aug-cc-pvdz-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/heavy-aug-cc-pvtz-jkfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/heavy-aug-cc-pvtz-jkfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/heavy-aug-cc-pvtz-ri.dat` & `pyscf-2.6.0/pyscf/gto/basis/heavy-aug-cc-pvtz-ri.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/iglo3.py` & `pyscf-2.6.0/pyscf/gto/basis/iglo3.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/lanl08.dat` & `pyscf-2.6.0/pyscf/gto/basis/lanl08.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/lanl2dz.dat` & `pyscf-2.6.0/pyscf/gto/basis/lanl2dz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/lanl2tz.dat` & `pyscf-2.6.0/pyscf/gto/basis/lanl2tz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/minao.py` & `pyscf-2.6.0/pyscf/gto/basis/minao.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/parse_bfd_pp.py` & `pyscf-2.6.0/pyscf/gto/basis/parse_bfd_pp.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/parse_cp2k.py` & `pyscf-2.6.0/pyscf/gto/basis/parse_cp2k.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/parse_cp2k_pp.py` & `pyscf-2.6.0/pyscf/gto/basis/parse_cp2k_pp.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/parse_gaussian.py` & `pyscf-2.6.0/pyscf/gto/basis/parse_gaussian.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/parse_molpro.py` & `pyscf-2.6.0/pyscf/gto/basis/parse_molpro.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/parse_nwchem.py` & `pyscf-2.6.0/pyscf/gto/basis/parse_nwchem.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/parse_nwchem_ecp.py` & `pyscf-2.6.0/pyscf/gto/basis/parse_nwchem_ecp.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pc-0.dat` & `pyscf-2.6.0/pyscf/gto/basis/pc-0.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pc-1.dat` & `pyscf-2.6.0/pyscf/gto/basis/pc-1.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pc-2.dat` & `pyscf-2.6.0/pyscf/gto/basis/pc-2.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pc-3.dat` & `pyscf-2.6.0/pyscf/gto/basis/pc-3.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pc-4.dat` & `pyscf-2.6.0/pyscf/gto/basis/pc-4.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pcseg-0.dat` & `pyscf-2.6.0/pyscf/gto/basis/pcseg-0.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pcseg-1.dat` & `pyscf-2.6.0/pyscf/gto/basis/pcseg-1.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pcseg-2.dat` & `pyscf-2.6.0/pyscf/gto/basis/pcseg-2.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pcseg-3.dat` & `pyscf-2.6.0/pyscf/gto/basis/pcseg-3.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pcseg-4.dat` & `pyscf-2.6.0/pyscf/gto/basis/pcseg-4.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pob-tzvp.dat` & `pyscf-2.6.0/pyscf/gto/basis/pob-tzvp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pob-tzvpp.dat` & `pyscf-2.6.0/pyscf/gto/basis/pob-tzvpp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/3-21++G.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/3-21++G.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/3-21++Gs.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/3-21++Gs.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/3-21G-diffuse.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/3-21G-diffuse.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/3-21G-polarization.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/3-21G-polarization.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/3-21G.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/3-21G.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/3-21Gs.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/3-21Gs.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/4-31G.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/4-31G.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31++G.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31++G.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31++Gs.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31++Gs.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31++Gss.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31++Gss.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31+G.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31+G.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31+Gs.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31+Gs.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31+Gss.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31+Gss.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311++G.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311++G.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311++Gs.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311++Gs.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311++Gss.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311++Gss.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311+G.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311+G.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311+Gs.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311+Gs.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311+Gss.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311+Gss.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311G-diffuse.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311G-diffuse.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311G-polarization-2d.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311G-polarization-2d.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311G-polarization-2p.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311G-polarization-2p.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311G-polarization-3d.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311G-polarization-3d.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311G-polarization-3p.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311G-polarization-3p.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311G-polarization-d.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311G-polarization-d.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311G-polarization-f.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311G-polarization-f.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311G-polarization-p.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311G-polarization-p.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311G.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311G.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311Gs.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311Gs.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-311Gss.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-311Gss.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31G-diffuse.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31G-diffuse.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31G-polarization-2d.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31G-polarization-2d.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31G-polarization-2p.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31G-polarization-2p.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31G-polarization-3d.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31G-polarization-3d.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31G-polarization-3p.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31G-polarization-3p.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31G-polarization-d.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31G-polarization-d.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31G-polarization-f.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31G-polarization-f.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31G.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31G.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31Gs.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31Gs.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/pople-basis/6-31Gss.dat` & `pyscf-2.6.0/pyscf/gto/basis/pople-basis/6-31Gss.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/qzp-dkh.dat` & `pyscf-2.6.0/pyscf/gto/basis/qzp-dkh.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/qzp.dat` & `pyscf-2.6.0/pyscf/gto/basis/qzp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/roos-dz.dat` & `pyscf-2.6.0/pyscf/gto/basis/roos-dz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/roos-tz.dat` & `pyscf-2.6.0/pyscf/gto/basis/roos-tz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/sarc-dkh2.dat` & `pyscf-2.6.0/pyscf/gto/basis/sarc-dkh2.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/sbkjc.dat` & `pyscf-2.6.0/pyscf/gto/basis/sbkjc.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/soecp/ECPDS10MDFSO.dat` & `pyscf-2.6.0/pyscf/gto/basis/soecp/ECPDS10MDFSO.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/soecp/ECPDS28MDFSO.dat` & `pyscf-2.6.0/pyscf/gto/basis/soecp/ECPDS28MDFSO.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/soecp/ECPDS28MWBSO.dat` & `pyscf-2.6.0/pyscf/gto/basis/soecp/ECPDS28MWBSO.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/soecp/ECPDS46MDFSO.dat` & `pyscf-2.6.0/pyscf/gto/basis/soecp/ECPDS46MDFSO.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/soecp/ECPDS60MDFSO.dat` & `pyscf-2.6.0/pyscf/gto/basis/soecp/ECPDS60MDFSO.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/soecp/ECPDS60MWBSO.dat` & `pyscf-2.6.0/pyscf/gto/basis/soecp/ECPDS60MWBSO.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/soecp/ECPDS78MDFSO.dat` & `pyscf-2.6.0/pyscf/gto/basis/soecp/ECPDS78MDFSO.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/soecp/ECPDS92MDFBQSO.dat` & `pyscf-2.6.0/pyscf/gto/basis/soecp/ECPDS92MDFBQSO.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/soecp/ECPDS92MDFBSO.dat` & `pyscf-2.6.0/pyscf/gto/basis/soecp/ECPDS92MDFBSO.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/sto-3g.dat` & `pyscf-2.6.0/pyscf/gto/basis/sto-3g.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/sto-6g.dat` & `pyscf-2.6.0/pyscf/gto/basis/sto-6g.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/stuttgart_dz.dat` & `pyscf-2.6.0/pyscf/gto/basis/stuttgart_dz.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/stuttgart_rsc.dat` & `pyscf-2.6.0/pyscf/gto/basis/stuttgart_rsc.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/tzp-dkh.dat` & `pyscf-2.6.0/pyscf/gto/basis/tzp-dkh.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/tzp.dat` & `pyscf-2.6.0/pyscf/gto/basis/tzp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/tzv.dat` & `pyscf-2.6.0/pyscf/gto/basis/tzv.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/basis/weigend_cfit.dat` & `pyscf-2.6.0/pyscf/gto/basis/weigend_cfit.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/cmd_args.py` & `pyscf-2.6.0/pyscf/gto/cmd_args.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/ecp.py` & `pyscf-2.6.0/pyscf/gto/ecp.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/eval_gto.py` & `pyscf-2.6.0/pyscf/gto/eval_gto.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/ft_ao.py` & `pyscf-2.6.0/pyscf/gto/ft_ao.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gto/mole.py` & `pyscf-2.6.0/pyscf/gto/mole.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,14 @@
 integrals. This module serves the interface to the integral library libcint.
 '''
 
 import os
 import sys
 import types
 import re
-import platform
-import gc
-import time
 
 import json
 import ctypes
 import numpy
 import numpy as np
 import h5py
 import scipy.special
@@ -59,14 +56,15 @@
 
 # for _atm, _bas, _env
 CHARGE_OF  = 0
 PTR_COORD  = 1
 NUC_MOD_OF = 2
 PTR_ZETA   = 3
 PTR_FRAC_CHARGE = 4
+PTR_RADIUS = 5
 ATM_SLOTS  = 6
 ATOM_OF    = 0
 ANG_OF     = 1
 NPRIM_OF   = 2
 NCTR_OF    = 3
 RADI_POWER = 3 # for ECP
 KAPPA_OF   = 4
@@ -987,18 +985,18 @@
         angl = b[0]
         if angl > 14:
             sys.stderr.write('Warning: integral library does not support basis '
                              'with angular momentum > 14\n')
 
         if isinstance(b[1], int):
             kappa = b[1]
-            b_coeff = numpy.array(sorted(list(b[2:]), reverse=True))
+            b_coeff = numpy.array(sorted(b[2:], reverse=True))
         else:
             kappa = 0
-            b_coeff = numpy.array(sorted(list(b[1:]), reverse=True))
+            b_coeff = numpy.array(sorted(b[1:], reverse=True))
         es = b_coeff[:,0]
         cs = b_coeff[:,1:]
         nprim, nctr = cs.shape
         cs = numpy.einsum('pi,p->pi', cs, gto_norm(angl, es))
         if NORMALIZE_GTO:
             cs = _nomalize_contracted_ao(angl, es, cs)
 
@@ -1205,15 +1203,15 @@
     newmol._atom   = copy.deepcopy(mol._atom)
     newmol.basis   = copy.deepcopy(mol.basis)
     newmol._basis  = copy.deepcopy(mol._basis)
     newmol.ecp     = copy.deepcopy(mol.ecp)
     newmol._ecp    = copy.deepcopy(mol._ecp)
     newmol.pseudo  = copy.deepcopy(mol.pseudo)
     newmol._pseudo = copy.deepcopy(mol._pseudo)
-    if mol.magmom:
+    if mol.magmom is not None:
         newmol.magmom  = list(mol.magmom)
     return newmol
 
 def pack(mol):
     '''Pack the input args of :class:`Mole` to a dict.
 
     Note this function only pack the input arguments (not the entire Mole
@@ -2410,14 +2408,23 @@
     @ms.setter
     def ms(self, x):
         if x is None:
             self.spin = None
         else:
             self.spin = int(round(2*x, 4))
 
+    @property
+    def enuc(self):
+        '''nuclear repulsion energy'''
+        if self._enuc is None:
+            self._enuc = self.energy_nuc()
+        return self._enuc
+    @enuc.setter
+    def enuc(self, x):
+        self._enuc = x
 
     copy = copy
 
     pack = pack
 
     @classmethod
     @lib.with_doc(unpack.__doc__)
@@ -2574,14 +2581,17 @@
         if self.spin is None:
             self.spin = self.nelectron % 2
         else:
             # Access self.nelec in which the code checks whether the spin and
             # number of electrons are consistent.
             self.nelec
 
+        # reset nuclear energy
+        self.enuc = None
+
         if not self.magmom:
             self.magmom = [0,] * self.natm
         elif len(self.magmom) != self.natm:
             logger.warn(self, 'len(magmom) != natm. Set magmom to zero')
             self.magmom = [0,] * self.natm
         elif isinstance(self.magmom, np.ndarray):
             self.magmom = self.magmom.tolist()
@@ -2691,41 +2701,30 @@
 
     @lib.with_doc(gto_norm.__doc__)
     def gto_norm(self, l, expnt):
         return gto_norm(l, expnt)
 
     def dump_input(self):
         import __main__
-        import pyscf
         if hasattr(__main__, '__file__'):
             try:
                 filename = os.path.abspath(__main__.__file__)
                 finput = open(filename, 'r')
                 self.stdout.write('#INFO: **** input file is %s ****\n' % filename)
                 self.stdout.write(finput.read())
                 self.stdout.write('#INFO: ******************** input file end ********************\n')
                 self.stdout.write('\n')
                 self.stdout.write('\n')
                 finput.close()
             except IOError:
                 logger.warn(self, 'input file does not exist')
 
-        self.stdout.write('System: %s  Threads %s\n' %
-                          (str(platform.uname()), lib.num_threads()))
-        self.stdout.write('Python %s\n' % sys.version)
-        self.stdout.write('numpy %s  scipy %s\n' %
-                          (numpy.__version__, scipy.__version__))
-        self.stdout.write('Date: %s\n' % time.ctime())
-        self.stdout.write('PySCF version %s\n' % pyscf.__version__)
-        info = lib.repo_info(os.path.join(__file__, '..', '..'))
-        self.stdout.write('PySCF path  %s\n' % info['path'])
-        if 'git' in info:
-            self.stdout.write(info['git'] + '\n')
+        self.stdout.write('\n'.join(lib.misc.format_sys_info()))
 
-        self.stdout.write('\n')
+        self.stdout.write('\n\n')
         for key in os.environ:
             if 'PYSCF' in key:
                 self.stdout.write('[ENV] %s %s\n' % (key, os.environ[key]))
         if self.verbose >= logger.DEBUG2:
             for key in dir(__config__):
                 if key[:2] != '__':
                     self.stdout.write('[CONFIG] %s = %s\n' %
@@ -2793,15 +2792,16 @@
                             self.stdout.write(' '*32+'%-15.12g  ' % x[0])
                         for c in x[1:]:
                             self.stdout.write(' %4.12g' % c)
                         self.stdout.write('\n')
 
         if self.verbose >= logger.INFO:
             self.stdout.write('\n')
-            logger.info(self, 'nuclear repulsion = %.15g', self.energy_nuc())
+            logger.info(self, 'nuclear repulsion = %.15g', self.enuc)
+
             if self.symmetry:
                 if self.topgroup == self.groupname:
                     logger.info(self, 'point group symmetry = %s', self.topgroup)
                 else:
                     logger.info(self, 'point group symmetry = %s, use subgroup %s',
                                 self.topgroup, self.groupname)
                 logger.info(self, "symmetry origin: %s", self._symm_orig)
@@ -3059,14 +3059,17 @@
             mol._env[ptr+0] = unit * atoms_or_coords[:,0]
             mol._env[ptr+1] = unit * atoms_or_coords[:,1]
             mol._env[ptr+2] = unit * atoms_or_coords[:,2]
         else:
             mol.symmetry = symmetry
             mol.build(False, False)
 
+        # reset nuclear energy
+        mol.enuc = None
+
         if mol.verbose >= logger.INFO:
             logger.info(mol, 'New geometry')
             for ia, atom in enumerate(mol._atom):
                 coorda = tuple([x * param.BOHR for x in atom[1]])
                 coordb = tuple([x for x in atom[1]])
                 coords = coorda + coordb
                 logger.info(mol, ' %3d %-4s %16.12f %16.12f %16.12f AA  '
@@ -3551,15 +3554,17 @@
         else:
             bas = self._bas
         return moleintor.getints_by_shell(intor, shells, self._atm, bas,
                                           self._env, comp)
 
     eval_ao = eval_gto = eval_gto
 
-    energy_nuc = get_enuc = energy_nuc
+    energy_nuc = energy_nuc
+    def get_enuc(self):
+        return self.enuc
 
     def get_ao_indices(self, bas_list, ao_loc=None):
         '''
         Generate (dis-continued) AO indices for basis specified in bas_list
         '''
         if ao_loc is None:
             ao_loc = self.ao_loc
@@ -3699,20 +3704,19 @@
         return self
 
     def __getattr__(self, key):
         '''To support accessing methods (mol.HF, mol.KS, mol.CCSD, mol.CASSCF, ...)
         from Mole object.
         '''
         if key[0] == '_':  # Skip private attributes and Python builtins
-            raise AttributeError('Mole object does not have attribute %s' % key)
-        elif key in ('_ipython_canary_method_should_not_exist_',
-                     '_repr_mimebundle_'):
-            # https://github.com/mewwts/addict/issues/26
-            # https://github.com/jupyter/notebook/issues/2014
-            raise AttributeError(f'Mole object has no attribute {key}')
+            # https://bugs.python.org/issue45985
+            # https://github.com/python/cpython/issues/103936
+            # @property and __getattr__ conflicts. As a temporary fix, call
+            # object.__getattribute__ method to re-raise AttributeError
+            return object.__getattribute__(self, key)
 
         # Import all available modules. Some methods are registered to other
         # classes/modules when importing modules in __all__.
         from pyscf import __all__  # noqa
         from pyscf import scf, dft
 
         for mod in (scf, dft):
@@ -3728,15 +3732,15 @@
                 xc = key.split('TD', 1)[1]
                 if xc in dft.XC:
                     mf.xc = xc
                     key = 'TDDFT'
         elif 'CI' in key or 'CC' in key or 'CAS' in key or 'MP' in key:
             mf = scf.HF(self)
         else:
-            raise AttributeError(f'Mole object has no attribute {key}')
+            return object.__getattribute__(self, key)
 
         method = getattr(mf, key)
 
         # Initialize SCF object for post-SCF methods if applicable
         if self.nelectron != 0:
             mf.run()
         return method
```

### Comparing `pyscf-2.5.0/pyscf/gto/moleintor.py` & `pyscf-2.6.0/pyscf/gto/moleintor.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,14 +425,15 @@
     'int3c2e_ipip1'             : (9, 9),
     'int3c2e_ipip2'             : (9, 9),
     'int3c2e_ipvip1'            : (9, 9),
     'int3c2e_ip1ip2'            : (9, 9),
     'int2c2e_ip1ip2'            : (9, 9),
     'int2c2e_ipip1'             : (9, 9),
     'int3c1e'                   : (1, 1),
+    'int3c1e_ip1'               : (3, 3),
     'int3c1e_p2'                : (1, 1),
     'int3c1e_iprinv'            : (3, 3),
     'int2c2e'                   : (1, 1),
     'int2e_yp'                  : (1, 1),
     'int2e_stg'                 : (1, 1),
     'int2e_coulerf'             : (1, 1),
     "int1e_grids"               : (1, 1),
```

### Comparing `pyscf-2.5.0/pyscf/gto/pp_int.py` & `pyscf-2.6.0/pyscf/gto/pp_int.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gw/__init__.py` & `pyscf-2.6.0/pyscf/gw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gw/gw_ac.py` & `pyscf-2.6.0/pyscf/gw/gw_ac.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gw/gw_cd.py` & `pyscf-2.6.0/pyscf/gw/gw_cd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gw/gw_exact.py` & `pyscf-2.6.0/pyscf/gw/gw_exact.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gw/gw_slow.py` & `pyscf-2.6.0/pyscf/gw/gw_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/gw/rpa.py` & `pyscf-2.6.0/pyscf/pbc/scf/kuhf_ksymm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,293 +1,219 @@
 #!/usr/bin/env python
-# Copyright 2014-2021 The PySCF Developers. All Rights Reserved.
+# Copyright 2020-2023 The PySCF Developers. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-# Author: Tianyu Zhu <zhutianyu1991@gmail.com>
+# Author: Xing Zhang <zhangxing.nju@gmail.com>
 #
 
-"""
-Spin-restricted random phase approximation (direct RPA/dRPA in chemistry)
-with N^4 scaling
-
-Method:
-    Main routines are based on GW-AC method descirbed in:
-    T. Zhu and G.K.-L. Chan, J. Chem. Theory. Comput. 17, 727-741 (2021)
-    X. Ren et al., New J. Phys. 14, 053020 (2012)
-"""
-
 import numpy as np
+from pyscf import __config__
 from pyscf import lib
 from pyscf.lib import logger
-from pyscf.ao2mo import _ao2mo
-from pyscf import df, scf
-from pyscf.mp.mp2 import get_nocc, get_nmo, get_frozen_mask
-
-einsum = lib.einsum
-
-# ****************************************************************************
-# core routines, kernel, rpa_ecorr, rho_response
-# ****************************************************************************
-
-def kernel(rpa, mo_energy, mo_coeff, Lpq=None, nw=40, x0=0.5, verbose=logger.NOTE):
-    """
-    RPA correlation and total energy
-
-    Args:
-        Lpq : density fitting 3-center integral in MO basis.
-        nw : number of frequency point on imaginary axis.
-        x0: scaling factor for frequency grid.
-
-    Returns:
-        e_tot : RPA total energy
-        e_hf : EXX energy
-        e_corr : RPA correlation energy
-    """
-    mf = rpa._scf
-    # only support frozen core
-    if rpa.frozen is not None:
-        assert isinstance(rpa.frozen, int)
-        assert rpa.frozen < rpa.nocc
-
-    if Lpq is None:
-        Lpq = rpa.ao2mo(mo_coeff)
-
-    # Grids for integration on imaginary axis
-    freqs, wts = _get_scaled_legendre_roots(nw, x0)
-
-    # Compute HF exchange energy (EXX)
-    dm = mf.make_rdm1()
-    rhf = scf.RHF(rpa.mol)
-    e_hf = rhf.energy_elec(dm=dm)[0]
-    e_hf += mf.energy_nuc()
-
-    # Compute RPA correlation energy
-    e_corr = get_rpa_ecorr(rpa, Lpq, freqs, wts)
-
-    # Compute total energy
-    e_tot = e_hf + e_corr
-
-    logger.debug(rpa, '  RPA total energy = %s', e_tot)
-    logger.debug(rpa, '  EXX energy = %s, RPA corr energy = %s', e_hf, e_corr)
-
-    return e_tot, e_hf, e_corr
-
-def get_rpa_ecorr(rpa, Lpq, freqs, wts):
-    """
-    Compute RPA correlation energy
-    """
-    mo_energy = _mo_energy_without_core(rpa, rpa._scf.mo_energy)
-    nocc = rpa.nocc
-    nw = len(freqs)
-    naux = Lpq.shape[0]
-
-    if (mo_energy[nocc] - mo_energy[nocc-1]) < 1e-3:
-        logger.warn(rpa, 'Current RPA code not well-defined for degeneracy!')
-
-    e_corr = 0.
-    for w in range(nw):
-        Pi = get_rho_response(freqs[w], mo_energy, Lpq[:, :nocc, nocc:])
-        ec_w = np.log(np.linalg.det(np.eye(naux) - Pi))
-        ec_w += np.trace(Pi)
-        e_corr += 1./(2.*np.pi) * ec_w * wts[w]
-
-    return e_corr
-
-def get_rho_response(omega, mo_energy, Lpq):
-    """
-    Compute density response function in auxiliary basis at freq iw.
-    """
-    naux, nocc, nvir = Lpq.shape
-    eia = mo_energy[:nocc, None] - mo_energy[None, nocc:]
-    eia = eia / (omega**2 + eia * eia)
-    # Response from both spin-up and spin-down density
-    Pia = Lpq * (eia * 4.0)
-    Pi = einsum('Pia, Qia -> PQ', Pia, Lpq)
-    return Pi
-
-# ****************************************************************************
-# frequency integral quadrature, legendre, clenshaw_curtis
-# ****************************************************************************
-
-def _get_scaled_legendre_roots(nw, x0=0.5):
-    """
-    Scale nw Legendre roots, which lie in the
-    interval [-1, 1], so that they lie in [0, inf)
-    Ref: www.cond-mat.de/events/correl19/manuscripts/ren.pdf
-
-    Returns:
-        freqs : 1D array
-        wts : 1D array
-    """
-    freqs, wts = np.polynomial.legendre.leggauss(nw)
-    freqs_new = x0 * (1.0 + freqs) / (1.0 - freqs)
-    wts = wts * 2.0 * x0 / (1.0 - freqs)**2
-    return freqs_new, wts
-
-def _get_clenshaw_curtis_roots(nw):
-    """
-    Clenshaw-Curtis qaudrature on [0,inf)
-    Ref: J. Chem. Phys. 132, 234114 (2010)
-    Returns:
-        freqs : 1D array
-        wts : 1D array
-    """
-    freqs = np.zeros(nw)
-    wts = np.zeros(nw)
-    a = 0.2
-    for w in range(nw):
-        t = (w + 1.0) / nw * np.pi * 0.5
-        freqs[w] = a / np.tan(t)
-        if w != nw - 1:
-            wts[w] = a*np.pi * 0.5 / nw / (np.sin(t)**2)
+from pyscf.scf import hf as mol_hf
+from pyscf.pbc.lib import kpts as libkpts
+from pyscf.pbc.scf import khf_ksymm, khf, kuhf
+from pyscf.pbc.lib.kpts import KPoints
+
+@lib.with_doc(kuhf.get_occ.__doc__)
+def get_occ(mf, mo_energy_kpts=None, mo_coeff_kpts=None):
+    if mo_energy_kpts is None:
+        mo_energy_kpts = mf.mo_energy
+    kpts = mf.kpts
+    assert isinstance(kpts, KPoints)
+
+    nocc_a, nocc_b = mf.nelec
+    mo_energy_kpts = kpts.transform_mo_energy(mo_energy_kpts)
+    mo_energy = np.sort(np.hstack(mo_energy_kpts[0]))
+    fermi_a = mo_energy[nocc_a-1]
+    mo_occ_kpts = [[], []]
+    for mo_e in mo_energy_kpts[0]:
+        mo_occ_kpts[0].append((mo_e <= fermi_a).astype(np.double))
+    if nocc_a < len(mo_energy):
+        logger.info(mf, 'alpha HOMO = %.12g  LUMO = %.12g', fermi_a, mo_energy[nocc_a])
+    else:
+        logger.info(mf, 'alpha HOMO = %.12g  (no LUMO because of small basis) ', fermi_a)
+
+    if nocc_b > 0:
+        mo_energy = np.sort(np.hstack(mo_energy_kpts[1]))
+        fermi_b = mo_energy[nocc_b-1]
+        for mo_e in mo_energy_kpts[1]:
+            mo_occ_kpts[1].append((mo_e <= fermi_b).astype(np.double))
+        if nocc_b < len(mo_energy):
+            logger.info(mf, 'beta HOMO = %.12g  LUMO = %.12g', fermi_b, mo_energy[nocc_b])
         else:
-            wts[w] = a*np.pi * 0.25 / nw / (np.sin(t)**2)
-    return freqs[::-1], wts[::-1]
-
-def _mo_energy_without_core(rpa, mo_energy):
-    return mo_energy[get_frozen_mask(rpa)]
-
-def _mo_without_core(rpa, mo):
-    return mo[:,get_frozen_mask(rpa)]
-
-class RPA(lib.StreamObject):
-
-    _keys = {
-        'mol', 'frozen',
-        'with_df', 'mo_energy', 'mo_coeff', 'mo_occ', 'e_corr', 'e_hf', 'e_tot',
-    }
-
-    def __init__(self, mf, frozen=None, auxbasis=None):
-        self.mol = mf.mol
-        self._scf = mf
-        self.verbose = self.mol.verbose
-        self.stdout = self.mol.stdout
-        self.max_memory = mf.max_memory
-        self.frozen = frozen
-
-        # DF-RPA must use density fitting integrals
-        if getattr(mf, 'with_df', None):
-            self.with_df = mf.with_df
-        else:
-            self.with_df = df.DF(mf.mol)
-            if auxbasis:
-                self.with_df.auxbasis = auxbasis
+            logger.info(mf, 'beta HOMO = %.12g  (no LUMO because of small basis) ', fermi_b)
+    else:
+        for mo_e in mo_energy_kpts[1]:
+            mo_occ_kpts[1].append(np.zeros_like(mo_e))
+
+    if mf.verbose >= logger.DEBUG:
+        np.set_printoptions(threshold=len(mo_energy))
+        logger.debug(mf, '     k-point                  alpha mo_energy')
+        for k,kpt in enumerate(mf.cell.get_scaled_kpts(kpts, kpts_in_ibz=False)):
+            if (np.count_nonzero(mo_occ_kpts[0][k]) > 0 and
+                np.count_nonzero(mo_occ_kpts[0][k] == 0) > 0):
+                logger.debug(mf, '  %2d (%6.3f %6.3f %6.3f)   %s %s',
+                             k, kpt[0], kpt[1], kpt[2],
+                             np.sort(mo_energy_kpts[0][k][mo_occ_kpts[0][k]> 0]),
+                             np.sort(mo_energy_kpts[0][k][mo_occ_kpts[0][k]==0]))
             else:
-                self.with_df.auxbasis = df.make_auxbasis(mf.mol, mp2fit=True)
-
-##################################################
-# don't modify the following attributes, they are not input options
-        self._nocc = None
-        self._nmo = None
-        self.mo_energy = mf.mo_energy
-        self.mo_coeff = mf.mo_coeff
-        self.mo_occ = mf.mo_occ
-        self.e_corr = None
-        self.e_hf = None
-        self.e_tot = None
-
-    def dump_flags(self):
-        log = logger.Logger(self.stdout, self.verbose)
-        log.info('')
-        log.info('******** %s ********', self.__class__)
-        log.info('method = %s', self.__class__.__name__)
-        nocc = self.nocc
-        nvir = self.nmo - nocc
-        log.info('RPA nocc = %d, nvir = %d', nocc, nvir)
-        if self.frozen is not None:
-            log.info('frozen orbitals = %d', self.frozen)
-        return self
-
-    @property
-    def nocc(self):
-        return self.get_nocc()
-    @nocc.setter
-    def nocc(self, n):
-        self._nocc = n
+                logger.debug(mf, '  %2d (%6.3f %6.3f %6.3f)   %s',
+                             k, kpt[0], kpt[1], kpt[2], mo_energy_kpts[0][k])
+        logger.debug(mf, '     k-point                  beta  mo_energy')
+        for k,kpt in enumerate(mf.cell.get_scaled_kpts(kpts, kpts_in_ibz=False)):
+            if (np.count_nonzero(mo_occ_kpts[1][k]) > 0 and
+                np.count_nonzero(mo_occ_kpts[1][k] == 0) > 0):
+                logger.debug(mf, '  %2d (%6.3f %6.3f %6.3f)   %s %s',
+                             k, kpt[0], kpt[1], kpt[2],
+                             np.sort(mo_energy_kpts[1][k][mo_occ_kpts[1][k]> 0]),
+                             np.sort(mo_energy_kpts[1][k][mo_occ_kpts[1][k]==0]))
+            else:
+                logger.debug(mf, '  %2d (%6.3f %6.3f %6.3f)   %s',
+                             k, kpt[0], kpt[1], kpt[2], mo_energy_kpts[1][k])
+        np.set_printoptions(threshold=1000)
+
+    if isinstance(kpts, KPoints):
+        mo_occ_kpts[0] = kpts.check_mo_occ_symmetry(mo_occ_kpts[0], tol=1e-4)
+        mo_occ_kpts[1] = kpts.check_mo_occ_symmetry(mo_occ_kpts[1], tol=1e-4)
+    return mo_occ_kpts
+
+@lib.with_doc(kuhf.energy_elec.__doc__)
+def energy_elec(mf, dm_kpts=None, h1e_kpts=None, vhf_kpts=None):
+    if dm_kpts is None: dm_kpts = mf.make_rdm1()
+    if h1e_kpts is None: h1e_kpts = mf.get_hcore()
+    if vhf_kpts is None: vhf_kpts = mf.get_veff(mf.cell, dm_kpts)
+    wtk = mf.kpts.weights_ibz
+
+    e1 = np.einsum('k,kij,kji', wtk, dm_kpts[0], h1e_kpts)
+    e1+= np.einsum('k,kij,kji', wtk, dm_kpts[1], h1e_kpts)
+    e_coul = np.einsum('k,kij,kji', wtk, dm_kpts[0], vhf_kpts[0]) * 0.5
+    e_coul+= np.einsum('k,kij,kji', wtk, dm_kpts[1], vhf_kpts[1]) * 0.5
+    mf.scf_summary['e1'] = e1.real
+    mf.scf_summary['e2'] = e_coul.real
+    logger.debug(mf, 'E1 = %s  E_coul = %s', e1, e_coul)
+    if kuhf.CHECK_COULOMB_IMAG and abs(e_coul.imag > mf.cell.precision*10):
+        logger.warn(mf, "Coulomb energy has imaginary part %s. "
+                    "Coulomb integrals (e-e, e-N) may not converge !",
+                    e_coul.imag)
+    return (e1+e_coul).real, e_coul.real
+
+get_rho = khf_ksymm.get_rho
+
+
+class KsymAdaptedKUHF(khf_ksymm.KsymAdaptedKSCF, kuhf.KUHF):
+    """
+    KUHF with k-point symmetry
+    """
+
+    get_occ = get_occ
+    energy_elec = energy_elec
+    get_rho = get_rho
+
+    to_ks = kuhf.KUHF.to_ks
+    convert_from_ = kuhf.KUHF.convert_from_
+
+    def __init__(self, cell, kpts=libkpts.KPoints(),
+                 exxdiv=getattr(__config__, 'pbc_scf_SCF_exxdiv', 'ewald'),
+                 use_ao_symmetry=True):
+        khf_ksymm.ksymm_scf_common_init(self, cell, kpts, use_ao_symmetry)
+        kuhf.KUHF.__init__(self, cell, kpts, exxdiv)
 
     @property
-    def nmo(self):
-        return self.get_nmo()
-    @nmo.setter
-    def nmo(self, n):
-        self._nmo = n
-
-    get_nocc = get_nocc
-    get_nmo = get_nmo
-    get_frozen_mask = get_frozen_mask
-
-    def kernel(self, mo_energy=None, mo_coeff=None, Lpq=None, nw=40, x0=0.5):
-        """
-        Args:
-            mo_energy : 1D array (nmo), mean-field mo energy
-            mo_coeff : 2D array (nmo, nmo), mean-field mo coefficient
-            Lpq : 3D array (naux, nmo, nmo), 3-index ERI
-            nw: integer, grid number
-            x0: real, scaling factor for frequency grid
-
-        Returns:
-            self.e_tot : RPA total eenrgy
-            self.e_hf : EXX energy
-            self.e_corr : RPA correlation energy
-        """
-        if mo_coeff is None:
-            mo_coeff = _mo_without_core(self, self._scf.mo_coeff)
-        if mo_energy is None:
-            mo_energy = _mo_energy_without_core(self, self._scf.mo_energy)
-
-        cput0 = (logger.process_clock(), logger.perf_counter())
-        self.dump_flags()
-        self.e_tot, self.e_hf, self.e_corr = \
-                        kernel(self, mo_energy, mo_coeff, Lpq=Lpq, nw=nw, x0=x0, verbose=self.verbose)
+    def nelec(self):
+        if self._nelec is not None:
+            return self._nelec
+        else:
+            cell = self.cell
+            nkpts = self.kpts.nkpts
+            ne = cell.tot_electrons(nkpts)
+            nalpha = (ne + cell.spin) // 2
+            nbeta = nalpha - cell.spin
+            if nalpha + nbeta != ne:
+                raise RuntimeError('Electron number %d and spin %d are not consistent\n'
+                                   'Note cell.spin = 2S = Nalpha - Nbeta, not 2S+1' %
+                                   (ne, cell.spin))
+            return nalpha, nbeta
+
+    @nelec.setter
+    def nelec(self, x):
+        self._nelec = x
+
+    def dump_flags(self, verbose=None):
+        khf_ksymm.KsymAdaptedKSCF.dump_flags(self, verbose)
+        logger.info(self, 'number of electrons per unit cell  '
+                    'alpha = %d beta = %d', *self.nelec)
+        return self
 
-        logger.timer(self, 'RPA', *cput0)
-        return self.e_corr
+    def get_init_guess(self, cell=None, key='minao', s1e=None):
+        if s1e is None:
+            s1e = self.get_ovlp(cell)
+        dm_kpts = mol_hf.SCF.get_init_guess(self, cell, key)
+        assert dm_kpts.shape[0]==2
+        if dm_kpts.ndim != 4:
+            nkpts = self.kpts.nkpts_ibz
+            # dm[spin,nao,nao] at gamma point -> dm_kpts[spin,nkpts,nao,nao]
+            dm_kpts = np.repeat(dm_kpts[:,None,:,:], nkpts, axis=1)
+        elif dm_kpts.shape[1] != self.kpts.nkpts_ibz:
+            dm_kpts = dm_kpts[:,self.kpts.ibz2bz]
+
+        ne = lib.einsum('k,xkij,kji->x', self.kpts.weights_ibz, dm_kpts, s1e).real
+        nkpts = self.kpts.nkpts
+        ne *= nkpts
+        nelec = np.asarray(self.nelec)
+        if np.any(abs(ne - nelec) > 0.01*nkpts):
+            logger.debug(self, 'Big error detected in the electron number '
+                         'of initial guess density matrix (Ne/cell = %g)!\n'
+                         '  This can cause huge error in Fock matrix and '
+                         'lead to instability in SCF for low-dimensional '
+                         'systems.\n  DM is normalized wrt the number '
+                         'of electrons %s', ne.mean()/nkpts, nelec/nkpts)
+            dm_kpts *= (nelec / ne).reshape(2,-1,1,1)
+        return dm_kpts
+
+    def eig(self, h_kpts, s_kpts):
+        e_a, c_a = khf_ksymm.KsymAdaptedKSCF.eig(self, h_kpts[0], s_kpts)
+        e_b, c_b = khf_ksymm.KsymAdaptedKSCF.eig(self, h_kpts[1], s_kpts)
+        return (e_a,e_b), (c_a,c_b)
 
-    def ao2mo(self, mo_coeff=None):
+    def get_orbsym(self, mo_coeff=None, s=None):
         if mo_coeff is None:
             mo_coeff = self.mo_coeff
-        nmo = self.nmo
-        naux = self.with_df.get_naoaux()
-        mem_incore = (2 * nmo**2*naux) * 8 / 1e6
-        mem_now = lib.current_memory()[0]
-
-        mo = np.asarray(mo_coeff, order='F')
-        ijslice = (0, nmo, 0, nmo)
-        Lpq = None
-        if (mem_incore + mem_now < 0.99 * self.max_memory) or self.mol.incore_anyway:
-            Lpq = _ao2mo.nr_e2(self.with_df._cderi, mo, ijslice, aosym='s2', out=Lpq)
-            return Lpq.reshape(naux, nmo, nmo)
-        else:
-            logger.warn(self, 'Memory may not be enough!')
-            raise NotImplementedError
+        if s is None:
+            s = self.get_ovlp()
+
+        orbsym_a = khf_ksymm.KsymAdaptedKSCF.get_orbsym(self, mo_coeff[0], s)
+        orbsym_b = khf_ksymm.KsymAdaptedKSCF.get_orbsym(self, mo_coeff[1], s)
+        return (orbsym_a, orbsym_b)
+
+    orbsym = property(get_orbsym)
+
+    def _finalize(self):
+        from pyscf.scf import chkfile as mol_chkfile
+        kuhf.KUHF._finalize(self)
+        if not self.use_ao_symmetry:
+            return
+
+        orbsym = self.get_orbsym()
+        for s in range(2):
+            for k, mo_e in enumerate(self.mo_energy[s]):
+                idx = np.argsort(mo_e.round(9), kind='stable')
+                self.mo_energy[s][k] = self.mo_energy[s][k][idx]
+                self.mo_occ[s][k] = self.mo_occ[s][k][idx]
+                self.mo_coeff[s][k] = lib.tag_array(self.mo_coeff[s][k][:,idx],
+                                                    orbsym=orbsym[s][k][idx])
+        self.dump_chk({'e_tot': self.e_tot, 'mo_energy': self.mo_energy,
+                       'mo_coeff': self.mo_coeff, 'mo_occ': self.mo_occ})
+        return self
 
-if __name__ == '__main__':
-    from pyscf import gto, dft
-    mol = gto.Mole()
-    mol.verbose = 4
-    mol.atom = [
-        [8 , (0. , 0.     , 0.)],
-        [1 , (0. , -0.7571 , 0.5861)],
-        [1 , (0. , 0.7571 , 0.5861)]]
-    mol.basis = 'def2-svp'
-    mol.build()
-
-    mf = dft.RKS(mol)
-    mf.xc = 'pbe'
-    mf.kernel()
-
-    rpa = RPA(mf)
-    rpa.kernel()
-    print ('RPA e_tot, e_hf, e_corr = ', rpa.e_tot, rpa.e_hf, rpa.e_corr)
-    assert (abs(rpa.e_corr- -0.30783004035780076) < 1e-6)
-    assert (abs(rpa.e_tot- -76.26428191794182) < 1e-6)
+KUHF = KsymAdaptedKUHF
```

### Comparing `pyscf-2.5.0/pyscf/gw/ugw_ac.py` & `pyscf-2.6.0/pyscf/gw/ugw_ac.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/hessian/__init__.py` & `pyscf-2.6.0/pyscf/hessian/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 # limitations under the License.
 #
 # Author: Qiming Sun <osirpt.sun@gmail.com>
 #
 
 from pyscf.hessian import rhf
 from pyscf.hessian import uhf
-from pyscf.hessian import dispersion
 from pyscf.hessian.rhf import Hessian as RHF
 from pyscf.hessian.uhf import Hessian as UHF
 from pyscf.hessian.rhf import hess_nuc
 
 try:
     from . import rks
     from . import uks
+    from . import dispersion
 except (ImportError, IOError):
     pass
```

### Comparing `pyscf-2.5.0/pyscf/hessian/rhf.py` & `pyscf-2.6.0/pyscf/hessian/rhf.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,16 +340,17 @@
                 h1ao = lib.chkfile.load(h1ao_or_chkfile, key)
             else:
                 h1ao = h1ao_or_chkfile[ia]
             h1vo.append(_ao2mo(h1ao))
 
         h1vo = numpy.vstack(h1vo)
         s1vo = numpy.vstack(s1vo)
+        tol = mf.conv_tol_cpscf * (ia1 - ia0)
         mo1, e1 = cphf.solve(fx, mo_energy, mo_occ, h1vo, s1vo,
-                             max_cycle=max_cycle, level_shift=level_shift)
+                             max_cycle=max_cycle, level_shift=level_shift, tol=tol)
         mo1 = numpy.einsum('pq,xqi->xpi', mo_coeff, mo1).reshape(-1,3,nao,nocc)
         e1 = e1.reshape(-1,3,nocc,nocc)
 
         for k in range(ia1-ia0):
             ia = atmlst[k+ia0]
             if isinstance(h1ao_or_chkfile, str):
                 key = 'scf_mo1/%d' % ia
@@ -483,17 +484,17 @@
         'mol', 'base', 'chkfile', 'atmlst', 'de', 'max_cycle', 'level_shift'
     }
 
     def __init__(self, scf_method):
         self.verbose = scf_method.verbose
         self.stdout = scf_method.stdout
         self.mol = scf_method.mol
-        self.base = scf_method
         self.chkfile = scf_method.chkfile
         self.max_memory = self.mol.max_memory
+        self.base = scf_method
         self.atmlst = range(self.mol.natm)
         self.de = numpy.zeros((0,0,3,3))  # (A,B,dR_A,dR_B)
 
     def hess_elec(self, *args, **kwargs):
         raise NotImplementedError
 
     def make_h1(self, *args, **kwargs):
@@ -588,35 +589,36 @@
         if atmlst is None:
             atmlst = self.atmlst
         else:
             self.atmlst = atmlst
 
         de = self.hess_elec(mo_energy, mo_coeff, mo_occ, atmlst=atmlst)
         self.de = de + self.hess_nuc(self.mol, atmlst=atmlst)
-        if self.base.disp is not None:
+        if self.base.do_disp():
             self.de += self.get_dispersion()
         return self.de
     hess = kernel
 
     gen_hop = gen_hop
 
+    # to_gpu can be reused only when __init__ still takes mf
     def to_gpu(self):
-        raise NotImplementedError
-
+        mf = self.base.to_gpu()
+        from importlib import import_module
+        mod = import_module(self.__module__.replace('pyscf', 'gpu4pyscf'))
+        cls = getattr(mod, self.__class__.__name__)
+        obj = cls(mf)
+        return obj
 
 class Hessian(HessianBase):
 
     partial_hess_elec = partial_hess_elec
     hess_elec = hess_elec
     make_h1 = make_h1
 
-    def to_gpu(self):
-        from gpu4pyscf.hessian.rhf import Hessian
-        return lib.to_gpu(self.view(Hessian))
-
 # Inject to RHF class
 from pyscf import scf
 scf.hf.RHF.Hessian = lib.class_as_method(Hessian)
 
 
 if __name__ == '__main__':
     from pyscf import scf
```

### Comparing `pyscf-2.5.0/pyscf/hessian/rks.py` & `pyscf-2.6.0/pyscf/hessian/rks.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                       atmlst=None, max_memory=4000, verbose=None):
     log = logger.new_logger(hessobj, verbose)
     time0 = t1 = (logger.process_clock(), logger.perf_counter())
 
     mol = hessobj.mol
     mf = hessobj.base
     ni = mf._numint
-    if mf.nlc or ni.libxc.is_nlc(mf.xc):
+    if mf.do_nlc():
         raise NotImplementedError('RKS Hessian for NLC functional')
 
     if mo_energy is None: mo_energy = mf.mo_energy
     if mo_occ is None:    mo_occ = mf.mo_occ
     if mo_coeff is None:  mo_coeff = mf.mo_coeff
     if atmlst is None: atmlst = range(mol.natm)
 
@@ -587,13 +587,9 @@
         self.grids = None
         self.grid_response = False
 
     partial_hess_elec = partial_hess_elec
     hess_elec = rhf_hess.hess_elec
     make_h1 = make_h1
 
-    def to_gpu(self):
-        from gpu4pyscf.hessian.rks import Hessian
-        return lib.to_gpu(self.view(Hessian))
-
 from pyscf import dft
 dft.rks.RKS.Hessian = dft.rks_symm.RKS.Hessian = lib.class_as_method(Hessian)
```

### Comparing `pyscf-2.5.0/pyscf/hessian/thermo.py` & `pyscf-2.6.0/pyscf/hessian/thermo.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/hessian/uhf.py` & `pyscf-2.6.0/pyscf/hessian/uhf.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,16 +303,17 @@
                 h1aoa = h1ao_or_chkfile[0][ia]
                 h1aob = h1ao_or_chkfile[1][ia]
             h1voa.append(_ao2mo(h1aoa, mo_coeff[0], mocca))
             h1vob.append(_ao2mo(h1aob, mo_coeff[1], moccb))
 
         h1vo = (numpy.vstack(h1voa), numpy.vstack(h1vob))
         s1vo = (numpy.vstack(s1voa), numpy.vstack(s1vob))
+        tol = mf.conv_tol_cpscf * (ia1 - ia0)
         mo1, e1 = ucphf.solve(fx, mo_energy, mo_occ, h1vo, s1vo,
-                              max_cycle=max_cycle, level_shift=level_shift)
+                              max_cycle=max_cycle, level_shift=level_shift, tol=tol)
         mo1a = numpy.einsum('pq,xqi->xpi', mo_coeff[0], mo1[0]).reshape(-1,3,nao,nocca)
         mo1b = numpy.einsum('pq,xqi->xpi', mo_coeff[1], mo1[1]).reshape(-1,3,nao,noccb)
         e1a = e1[0].reshape(-1,3,nocca,nocca)
         e1b = e1[1].reshape(-1,3,noccb,noccb)
 
         for k in range(ia1-ia0):
             ia = atmlst[k+ia0]
@@ -450,17 +451,14 @@
 
     def solve_mo1(self, mo_energy, mo_coeff, mo_occ, h1ao_or_chkfile,
                   fx=None, atmlst=None, max_memory=4000, verbose=None):
         return solve_mo1(self.base, mo_energy, mo_coeff, mo_occ, h1ao_or_chkfile,
                          fx, atmlst, max_memory, verbose,
                          max_cycle=self.max_cycle, level_shift=self.level_shift)
 
-    def to_gpu(self):
-        raise NotImplementedError
-
 from pyscf import scf
 scf.uhf.UHF.Hessian = lib.class_as_method(Hessian)
 
 if __name__ == '__main__':
     from pyscf import gto
     from pyscf import scf
```

### Comparing `pyscf-2.5.0/pyscf/hessian/uks.py` & `pyscf-2.6.0/pyscf/hessian/uks.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                       atmlst=None, max_memory=4000, verbose=None):
     log = logger.new_logger(hessobj, verbose)
     time0 = t1 = (logger.process_clock(), logger.perf_counter())
 
     mol = hessobj.mol
     mf = hessobj.base
     ni = mf._numint
-    if mf.nlc or ni.libxc.is_nlc(mf.xc):
+    if mf.do_nlc():
         raise NotImplementedError('RKS Hessian for NLC functional')
 
     if mo_energy is None: mo_energy = mf.mo_energy
     if mo_occ is None:    mo_occ = mf.mo_occ
     if mo_coeff is None:  mo_coeff = mf.mo_coeff
     if atmlst is None: atmlst = range(mol.natm)
 
@@ -664,17 +664,14 @@
 
     hess_elec = uhf_hess.hess_elec
     gen_hop = uhf_hess.gen_hop
     solve_mo1 = uhf_hess.Hessian.solve_mo1
     partial_hess_elec = partial_hess_elec
     make_h1 = make_h1
 
-    def to_gpu(self):
-        raise NotImplementedError
-
 from pyscf import dft
 dft.uks.UKS.Hessian = dft.uks_symm.UKS.Hessian = lib.class_as_method(Hessian)
 
 
 if __name__ == '__main__':
     from pyscf import gto
     from pyscf import dft
```

### Comparing `pyscf-2.5.0/pyscf/lib/CMakeLists.txt` & `pyscf-2.6.0/pyscf/lib/CMakeLists.txt`

 * *Files 12% similar despite different names*

```diff
@@ -132,25 +132,33 @@
   set(CMAKE_BUILD_RPATH "@loader_path;@loader_path/deps/lib;@loader_path/deps/lib64")
 else ()
   set(CMAKE_SKIP_BUILD_RPATH  True)
   set(CMAKE_BUILD_WITH_INSTALL_RPATH True)
   set(CMAKE_INSTALL_RPATH "\$ORIGIN:\$ORIGIN/deps/lib:\$ORIGIN/deps/lib64")
 endif ()
 
+option(ENABLE_FFTW "Using fftw3" OFF)
+option(BUILD_FFTW "Building fftw3" OFF)
+
 add_subdirectory(np_helper)
 add_subdirectory(gto)
 add_subdirectory(vhf)
 add_subdirectory(ao2mo)
 add_subdirectory(mcscf)
 add_subdirectory(cc)
 add_subdirectory(ri)
 #add_subdirectory(localizer)
 add_subdirectory(pbc)
 add_subdirectory(agf2)
 
+option(ENABLE_SMD "Compiling SMD Fortran code" OFF)
+if(ENABLE_SMD)
+  add_subdirectory(solvent)
+endif(ENABLE_SMD)
+
 # Overwrite CMAKE_C_CREATE_SHARED_LIBRARY in Modules/CMakeCInformation.cmake
 # to remove the SONAME flag in the so file. The soname information causes
 # dynamic link error when importing libcint library.
 set(C_LINK_TEMPLATE "<CMAKE_C_COMPILER> <CMAKE_SHARED_LIBRARY_C_FLAGS> <LANGUAGE_COMPILE_FLAGS> <LINK_FLAGS> <CMAKE_SHARED_LIBRARY_CREATE_C_FLAGS> -o <TARGET> <OBJECTS> <LINK_LIBRARIES>")
 set(CXX_LINK_TEMPLATE "<CMAKE_CXX_COMPILER> <CMAKE_SHARED_LIBRARY_CXX_FLAGS> <LANGUAGE_COMPILE_FLAGS> <LINK_FLAGS> <CMAKE_SHARED_LIBRARY_CREATE_CXX_FLAGS> -o <TARGET> <OBJECTS> <LINK_LIBRARIES>")
 
 include(ExternalProject)
@@ -161,15 +169,15 @@
 if(BUILD_LIBCINT)
   set(LIBCINT_GIT https://github.com/sunqm/libcint.git) # libcint is a portable, cross-platform implementation
   set(LIBCINT_VERSION v6.1.1)
   if (USE_QCINT)
     set(LIBCINT_GIT https://github.com/sunqm/qcint.git) # qcint is an optimized implementation for x86-64 architecture
     set(LIBCINT_VERSION v6.1.2)
     if(NOT BUILD_MARCH_NATIVE)
-      message(WARNING "The BUILD_MARCH_NATIVE option is not specified! qcint may not compile unless you explicitly pass compiler flags that turn on vectorization!")    
+      message(WARNING "The BUILD_MARCH_NATIVE option is not specified! qcint may not compile unless you explicitly pass compiler flags that turn on vectorization!")
     endif()
   endif()
 
   ExternalProject_Add(libcint
     GIT_REPOSITORY ${LIBCINT_GIT}
     GIT_TAG ${LIBCINT_VERSION}
     PREFIX ${PROJECT_BINARY_DIR}/deps
@@ -194,14 +202,20 @@
 endif() # BUILD_LIBCINT
 
 option(ENABLE_LIBXC "Using libxc for XC functional library" ON)
 option(ENABLE_XCFUN "Using xcfun for XC functional library" ON)
 option(BUILD_LIBXC "Download and build libxc library" ON)
 option(BUILD_XCFUN "Download and build xcfun library" ON)
 
+option(ENABLE_LIBXSMM "Using libxsmm" OFF)
+option(BUILD_LIBXSMM "Building libxsmm" OFF)
+if(APPLE)
+    set(ENABLE_LIBXSMM OFF)
+endif()
+
 if(NOT DISABLE_DFT)
 add_subdirectory(dft)
 
 if(ENABLE_LIBXC AND BUILD_LIBXC)
   ExternalProject_Add(libxc
     #GIT_REPOSITORY https://gitlab.com/libxc/libxc.git
     #GIT_TAG master
@@ -233,12 +247,43 @@
             -DCMAKE_INSTALL_PREFIX:PATH=<INSTALL_DIR>
             -DCMAKE_CXX_CREATE_SHARED_LIBRARY=${CXX_LINK_TEMPLATE}
             -DCMAKE_CXX_COMPILER=${CMAKE_CXX_COMPILER}
   )
   add_dependencies(xcfun_itrf libxcfun)
   add_dependencies(dft libxcfun)
 endif() # ENABLE_XCFUN
+
+if(ENABLE_LIBXSMM AND BUILD_LIBXSMM)
+  if(NOT EXISTS "${PROJECT_SOURCE_DIR}/deps/include/libxsmm.h")
+    ExternalProject_Add(libxsmm
+      GIT_REPOSITORY https://github.com/hfp/libxsmm.git
+      GIT_TAG 1.17
+      PREFIX ${PROJECT_BINARY_DIR}/deps
+      INSTALL_DIR ${PROJECT_SOURCE_DIR}/deps
+      CONFIGURE_COMMAND ""
+      BUILD_IN_SOURCE True
+      BUILD_COMMAND make -j4 PREFIX=<INSTALL_DIR> CXX=${CMAKE_CXX_COMPILER} CC=${CMAKE_C_COMPILER} STATIC=0 MALLOC=0 INTRINSICS=2 install
+      INSTALL_COMMAND ""
+    )
+    add_dependencies(dft libxsmm)
+  endif()
+endif()
 endif() # DISABLE_DFT
 
+if(ENABLE_FFTW AND BUILD_FFTW)
+#  if(NOT EXISTS "${PROJECT_SOURCE_DIR}/deps/include/fftw3.h")
+    ExternalProject_Add(libfftw3
+      URL https://www.fftw.org/fftw-3.3.10.tar.gz
+      PREFIX ${PROJECT_BINARY_DIR}/deps
+      INSTALL_DIR ${PROJECT_SOURCE_DIR}/deps
+      BUILD_IN_SOURCE True
+      CONFIGURE_COMMAND ./configure --enable-static=no --enable-shared=yes --enable-threads CXX=${CMAKE_CXX_COMPILER} CC=${CMAKE_C_COMPILER} prefix=<INSTALL_DIR>
+      BUILD_COMMAND make -j4 install
+    )
+    add_dependencies(fft libfftw3)
+    add_dependencies(pbc libfftw3)
+#  endif()
+endif()
+
 if(EXISTS "${PROJECT_SOURCE_DIR}/cmake.user.inc")
   include("${PROJECT_SOURCE_DIR}/cmake.user.inc")
 endif()
```

### Comparing `pyscf-2.5.0/pyscf/lib/__init__.py` & `pyscf-2.6.0/pyscf/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/agf2/CMakeLists.txt` & `pyscf-2.6.0/pyscf/lib/agf2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/agf2/ragf2.c` & `pyscf-2.6.0/pyscf/lib/agf2/ragf2.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/agf2/ragf2.h` & `pyscf-2.6.0/pyscf/lib/agf2/ragf2.h`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/agf2/uagf2.c` & `pyscf-2.6.0/pyscf/lib/agf2/uagf2.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/ao2mo/CMakeLists.txt` & `pyscf-2.6.0/pyscf/lib/ao2mo/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/ao2mo/nr_ao2mo.c` & `pyscf-2.6.0/pyscf/lib/ao2mo/nr_ao2mo.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/ao2mo/nr_ao2mo.h` & `pyscf-2.6.0/pyscf/lib/ao2mo/nr_ao2mo.h`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/ao2mo/nr_incore.c` & `pyscf-2.6.0/pyscf/lib/ao2mo/nr_incore.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/ao2mo/nr_incore.h` & `pyscf-2.6.0/pyscf/lib/ao2mo/nr_incore.h`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/ao2mo/nrr_ao2mo.c` & `pyscf-2.6.0/pyscf/lib/ao2mo/nrr_ao2mo.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/ao2mo/r_ao2mo.c` & `pyscf-2.6.0/pyscf/lib/ao2mo/r_ao2mo.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/ao2mo/r_ao2mo.h` & `pyscf-2.6.0/pyscf/lib/ao2mo/r_ao2mo.h`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/ao2mo/restore_eri.c` & `pyscf-2.6.0/pyscf/lib/ao2mo/restore_eri.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/cc/CMakeLists.txt` & `pyscf-2.6.0/pyscf/lib/cc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/cc/ccsd_grad.c` & `pyscf-2.6.0/pyscf/lib/cc/ccsd_grad.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/cc/ccsd_pack.c` & `pyscf-2.6.0/pyscf/lib/cc/ccsd_pack.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/cc/ccsd_t.c` & `pyscf-2.6.0/pyscf/lib/cc/ccsd_t.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/cc/uccsd_t.c` & `pyscf-2.6.0/pyscf/lib/cc/uccsd_t.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/chkfile.py` & `pyscf-2.6.0/pyscf/lib/chkfile.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/dft/CMakeLists.txt` & `pyscf-2.6.0/pyscf/lib/dft/CMakeLists.txt`

 * *Files 16% similar despite different names*

```diff
@@ -11,30 +11,34 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 add_library(dft SHARED
   CxLebedevGrid.c grid_basis.c nr_numint.c r_numint.c
   numint_uniform_grid.c xc_deriv.c nr_numint_sparse.c
-  )
-add_dependencies(dft cgto cvhf np_helper)
+  multigrid.c grid_common.c grid_collocate.c grid_integrate.c utils.c
+)
+add_dependencies(dft cgto cvhf np_helper pbc)
 
 set_target_properties(dft PROPERTIES
   LIBRARY_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR})
 
-target_link_libraries(dft cvhf cgto cint np_helper ${BLAS_LIBRARIES} ${OPENMP_C_PROPERTIES})
-
+if(ENABLE_LIBXSMM)
+  add_definitions(-DHAVE_LIBXSMM)
+  target_link_libraries(dft cvhf cgto cint np_helper pbc xsmm ${BLAS_LIBRARIES} ${OPENMP_C_PROPERTIES})
+else()
+  target_link_libraries(dft cvhf cgto cint np_helper pbc ${BLAS_LIBRARIES} ${OPENMP_C_PROPERTIES})
+endif()
 
 if(ENABLE_LIBXC)
 add_library(xc_itrf SHARED libxc_itrf.c)
 set_target_properties(xc_itrf PROPERTIES
   LIBRARY_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR})
 target_link_libraries(xc_itrf xc ${OPENMP_C_PROPERTIES})
 endif()
 
 if(ENABLE_XCFUN)
 add_library(xcfun_itrf SHARED xcfun_itrf.c)
 set_target_properties(xcfun_itrf PROPERTIES
   LIBRARY_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR})
 target_link_libraries(xcfun_itrf xcfun ${OPENMP_C_PROPERTIES})
 endif()
-
```

### Comparing `pyscf-2.5.0/pyscf/lib/dft/CxLebedevGrid.c` & `pyscf-2.6.0/pyscf/lib/dft/CxLebedevGrid.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/dft/grid_basis.c` & `pyscf-2.6.0/pyscf/lib/dft/grid_basis.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/dft/grid_basis.h` & `pyscf-2.6.0/pyscf/lib/dft/grid_basis.h`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/dft/libxc_itrf.c` & `pyscf-2.6.0/pyscf/lib/dft/libxc_itrf.c`

 * *Files 21% similar despite different names*

```diff
@@ -11,24 +11,28 @@
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
  *
  * Authors: Qiming Sun <osirpt.sun@gmail.com>
  *          Susi Lehtola <susi.lehtola@gmail.com>
+ *          Xing Zhang <zhangxing.nju@gmail.com>
  *
  * libxc from
  * http://www.tddft.org/programs/octopus/wiki/index.php/Libxc:manual
  */
 
 #include <stdio.h>
 #include <stdlib.h>
 #include <assert.h>
 #include <xc.h>
+#include "config.h"
 #define MAX(X,Y) ((X) > (Y) ? (X) : (Y))
+#define MIN(X,Y) ((X) < (Y) ? (X) : (Y))
+#define MAX_THREADS     256
 
 // TODO: register python signal
 #define raise_error     return
 
 /* Extracted from comments of libxc:gga.c
 
     sigma_st          = grad rho_s . grad rho_t
@@ -79,21 +83,21 @@
 #define MGGA_NVAR       5
 
 /*
  * rho_u/rho_d = (den,grad_x,grad_y,grad_z,laplacian,tau)
  * In spin restricted case (spin == 1), rho_u is assumed to be the
  * spin-free quantities, rho_d is not used.
  */
-static void _eval_rho(double *rho, double *rho_u, int spin, int nvar, int np)
+static void _eval_rho(double *rho, double *rho_u, int spin, int nvar, int np, int ld_rho_u)
 {
         int i;
         double *sigma, *tau;
         double *gxu, *gyu, *gzu, *gxd, *gyd, *gzd;
         double *tau_u, *tau_d;
-        double *rho_d = rho_u + np * nvar;
+        double *rho_d = rho_u + ld_rho_u * nvar;
 
         switch (nvar) {
         case LDA_NVAR:
                 if (spin == 1) {
                         for (i = 0; i < np; i++) {
                                 rho[i*2+0] = rho_u[i];
                                 rho[i*2+1] = rho_d[i];
@@ -103,79 +107,79 @@
                                 rho[i] = rho_u[i];
                         }
                 }
                 break;
         case GGA_NVAR:
                 if (spin == 1) {
                         sigma = rho + np * 2;
-                        gxu = rho_u + np;
-                        gyu = rho_u + np * 2;
-                        gzu = rho_u + np * 3;
-                        gxd = rho_d + np;
-                        gyd = rho_d + np * 2;
-                        gzd = rho_d + np * 3;
+                        gxu = rho_u + ld_rho_u;
+                        gyu = rho_u + ld_rho_u * 2;
+                        gzu = rho_u + ld_rho_u * 3;
+                        gxd = rho_d + ld_rho_u;
+                        gyd = rho_d + ld_rho_u * 2;
+                        gzd = rho_d + ld_rho_u * 3;
                         for (i = 0; i < np; i++) {
                                 rho[i*2+0] = rho_u[i];
                                 rho[i*2+1] = rho_d[i];
                                 sigma[i*3+0] = gxu[i]*gxu[i] + gyu[i]*gyu[i] + gzu[i]*gzu[i];
                                 sigma[i*3+1] = gxu[i]*gxd[i] + gyu[i]*gyd[i] + gzu[i]*gzd[i];
                                 sigma[i*3+2] = gxd[i]*gxd[i] + gyd[i]*gyd[i] + gzd[i]*gzd[i];
                         }
                 } else {
                         sigma = rho + np;
-                        gxu = rho_u + np;
-                        gyu = rho_u + np * 2;
-                        gzu = rho_u + np * 3;
+                        gxu = rho_u + ld_rho_u;
+                        gyu = rho_u + ld_rho_u * 2;
+                        gzu = rho_u + ld_rho_u * 3;
                         for (i = 0; i < np; i++) {
                                 rho[i] = rho_u[i];
                                 sigma[i] = gxu[i]*gxu[i] + gyu[i]*gyu[i] + gzu[i]*gzu[i];
                         }
                 }
                 break;
         case MGGA_NVAR:
                 if (spin == 1) {
                         sigma = rho + np * 2;
                         tau = sigma + np * 3;
-                        gxu = rho_u + np;
-                        gyu = rho_u + np * 2;
-                        gzu = rho_u + np * 3;
-                        gxd = rho_d + np;
-                        gyd = rho_d + np * 2;
-                        gzd = rho_d + np * 3;
-                        tau_u  = rho_u + np * 4;
-                        tau_d  = rho_d + np * 4;
+                        gxu = rho_u + ld_rho_u;
+                        gyu = rho_u + ld_rho_u * 2;
+                        gzu = rho_u + ld_rho_u * 3;
+                        gxd = rho_d + ld_rho_u;
+                        gyd = rho_d + ld_rho_u * 2;
+                        gzd = rho_d + ld_rho_u * 3;
+                        tau_u  = rho_u + ld_rho_u * 4;
+                        tau_d  = rho_d + ld_rho_u * 4;
                         for (i = 0; i < np; i++) {
                                 rho[i*2+0] = rho_u[i];
                                 rho[i*2+1] = rho_d[i];
                                 tau[i*2+0] = tau_u[i];
                                 tau[i*2+1] = tau_d[i];
                         }
                         for (i = 0; i < np; i++) {
                                 sigma[i*3+0] = gxu[i]*gxu[i] + gyu[i]*gyu[i] + gzu[i]*gzu[i];
                                 sigma[i*3+1] = gxu[i]*gxd[i] + gyu[i]*gyd[i] + gzu[i]*gzd[i];
                                 sigma[i*3+2] = gxd[i]*gxd[i] + gyd[i]*gyd[i] + gzd[i]*gzd[i];
                         }
                 } else {
                         sigma = rho + np;
                         tau  = sigma + np;
-                        gxu = rho_u + np;
-                        gyu = rho_u + np * 2;
-                        gzu = rho_u + np * 3;
-                        tau_u = rho_u + np * 4;
+                        gxu = rho_u + ld_rho_u;
+                        gyu = rho_u + ld_rho_u * 2;
+                        gzu = rho_u + ld_rho_u * 3;
+                        tau_u = rho_u + ld_rho_u * 4;
                         for (i = 0; i < np; i++) {
                                 rho[i] = rho_u[i];
                                 sigma[i] = gxu[i]*gxu[i] + gyu[i]*gyu[i] + gzu[i]*gzu[i];
                                 tau[i] = tau_u[i];
                         }
                 }
                 break;
         }
 }
 static void _eval_xc(xc_func_type *func_x, int spin, int deriv, int np,
-                     double *rho, double *exc)
+                     double *rho, double *exc, int offset, int blksize)
 {
         double *sigma, *tau;
         double *lapl = rho;
         double *vrho   = NULL;
         double *vsigma = NULL;
         double *vlapl  = NULL;
         double *vtau   = NULL;
@@ -262,36 +266,66 @@
                         }
                         if (deriv > 2) {
                                 v3rho3 = v2rho2 + np * 3;
                         }
                         if (deriv > 3) {
                                 v4rho4 = v3rho3 + np * 4;
                         }
+
+                        // set offset
+                        exc += offset;
+                        if (deriv > 0) {
+                                vrho += offset * 2;
+                        }
+                        if (deriv > 1) {
+                                v2rho2 += offset * 3;
+                        }
+                        if (deriv > 2) {
+                                v3rho3 += offset * 4;
+                        }
+                        if (deriv > 3) {
+                                v4rho4 += offset * 5;
+                        }
                 } else {
                         if (deriv > 0) {
                                 vrho = exc + np;
                         }
                         if (deriv > 1) {
                                 v2rho2 = vrho + np;
                         }
                         if (deriv > 2) {
                                 v3rho3 = v2rho2 + np;
                         }
                         if (deriv > 3) {
                                 v4rho4 = v3rho3 + np;
                         }
+
+                        // set offset
+                        exc += offset;
+                        if (deriv > 0) {
+                                vrho += offset;
+                        }
+                        if (deriv > 1) {
+                                v2rho2 += offset;
+                        }
+                        if (deriv > 2) {
+                                v3rho3 += offset;
+                        }
+                        if (deriv > 3) {
+                                v4rho4 += offset;
+                        }
                 }
-                xc_lda(func_x, np, rho, exc, vrho, v2rho2, v3rho3, v4rho4);
+                xc_lda(func_x, blksize, rho, exc, vrho, v2rho2, v3rho3, v4rho4);
                 break;
         case XC_FAMILY_GGA:
 #ifdef XC_FAMILY_HYB_GGA
         case XC_FAMILY_HYB_GGA:
 #endif
                 if (spin == 1) {
-                        sigma = rho + np * 2;
+                        sigma = rho + blksize * 2;
                         if (deriv > 0) {
                                 vrho = exc + np;
                                 vsigma = vrho + np * 2;
                         }
                         if (deriv > 1) {
                                 v2rho2 = vsigma + np * 3;
                                 v2rhosigma = v2rho2 + np * 3;
@@ -306,16 +340,41 @@
                         if (deriv > 3) {
                                 v4rho4       = v3sigma3     + np * 10  ;
                                 v4rho3sigma  = v4rho4       + np * 5   ;
                                 v4rho2sigma2 = v4rho3sigma  + np * 4*3 ;
                                 v4rhosigma3  = v4rho2sigma2 + np * 3*6 ;
                                 v4sigma4     = v4rhosigma3  + np * 2*10;
                         }
+
+                        // set offset
+                        exc += offset;
+                        if (deriv > 0) {
+                                vrho += offset * 2;
+                                vsigma += offset * 3;
+                        }
+                        if (deriv > 1) {
+                                v2rho2 += offset * 3;
+                                v2rhosigma += offset * 6;
+                                v2sigma2 += offset * 6;
+                        }
+                        if (deriv > 2) {
+                                v3rho3 += offset * 4;
+                                v3rho2sigma += offset * 9;
+                                v3rhosigma2 += offset * 12;
+                                v3sigma3 += offset * 10;
+                        }
+                        if (deriv > 3) {
+                                v4rho4 += offset * 5;
+                                v4rho3sigma += offset * 4*3;
+                                v4rho2sigma2 += offset * 3*6;
+                                v4rhosigma3 += offset * 2*10;
+                                v4sigma4 += offset * 15;
+                        }
                 } else {
-                        sigma = rho + np;
+                        sigma = rho + blksize;
                         if (deriv > 0) {
                                 vrho = exc + np;
                                 vsigma = vrho + np;
                         }
                         if (deriv > 1) {
                                 v2rho2 = vsigma + np;
                                 v2rhosigma = v2rho2 + np;
@@ -330,28 +389,53 @@
                         if (deriv > 3) {
                                 v4rho4       = v3sigma3     + np;
                                 v4rho3sigma  = v4rho4       + np;
                                 v4rho2sigma2 = v4rho3sigma  + np;
                                 v4rhosigma3  = v4rho2sigma2 + np;
                                 v4sigma4     = v4rhosigma3  + np;
                         }
+
+                        // set offset
+                        exc += offset;
+                        if (deriv > 0) {
+                                vrho += offset;
+                                vsigma += offset;
+                        }
+                        if (deriv > 1) {
+                                v2rho2 += offset;
+                                v2rhosigma += offset;
+                                v2sigma2 += offset;
+                        }
+                        if (deriv > 2) {
+                                v3rho3 += offset;
+                                v3rho2sigma += offset;
+                                v3rhosigma2 += offset;
+                                v3sigma3 += offset;
+                        }
+                        if (deriv > 3) {
+                                v4rho4 += offset;
+                                v4rho3sigma += offset;
+                                v4rho2sigma2 += offset;
+                                v4rhosigma3 += offset;
+                                v4sigma4 += offset;
+                        }
                 }
-                xc_gga(func_x, np, rho, sigma,
+                xc_gga(func_x, blksize, rho, sigma,
                        exc, vrho, vsigma,
                        v2rho2, v2rhosigma, v2sigma2,
                        v3rho3, v3rho2sigma, v3rhosigma2, v3sigma3,
                        v4rho4, v4rho3sigma, v4rho2sigma2, v4rhosigma3, v4sigma4);
                 break;
         case XC_FAMILY_MGGA:
 #ifdef XC_FAMILY_HYB_MGGA
         case XC_FAMILY_HYB_MGGA:
 #endif
                 if (spin == 1) {
-                        sigma = rho + np * 2;
-                        tau = sigma + np * 3;
+                        sigma = rho + blksize * 2;
+                        tau = sigma + blksize * 3;
                         if (deriv > 0) {
                                 vrho = exc + np;
                                 vsigma = vrho + np * 2;
                                 vtau = vsigma + np * 3;
                         }
                         if (deriv > 1) {
                                 v2rho2      = vtau        + np * 2;
@@ -386,17 +470,62 @@
                                 v4rhosigmatau2 = v4rhosigma2tau + np * 2*6*2;
                                 v4rhotau3      = v4rhosigmatau2 + np * 2*3*3;
                                 v4sigma3tau    = v4rhotau3      + np * 2*4  ;
                                 v4sigma2tau2   = v4sigma3tau    + np * 10*2 ;
                                 v4sigmatau3    = v4sigma2tau2   + np * 6*3  ;
                                 v4tau4         = v4sigmatau3    + np * 3*4  ;
                         }
+
+                        // set offset
+                        exc += offset;
+                        if (deriv > 0) {
+                                vrho   += offset * 2;
+                                vsigma += offset * 3;
+                                vtau   += offset * 2;
+                        }
+                        if (deriv > 1) {
+                                v2rho2      += offset * 3;
+                                v2rhosigma  += offset * 6;
+                                v2sigma2    += offset * 6;
+                                v2rhotau    += offset * 4;
+                                v2sigmatau  += offset * 6;
+                                v2tau2      += offset * 3;
+                        }
+                        if (deriv > 2) {
+                                v3rho3         += offset * 4 ;
+                                v3rho2sigma    += offset * 9 ;
+                                v3rhosigma2    += offset * 12;
+                                v3sigma3       += offset * 10;
+                                v3rho2tau      += offset * 6 ;
+                                v3rhosigmatau  += offset * 12;
+                                v3rhotau2      += offset * 6 ;
+                                v3sigma2tau    += offset * 12;
+                                v3sigmatau2    += offset * 9 ;
+                                v3tau3         += offset * 4 ;
+                        }
+                        if (deriv > 3) {
+                                v4rho4         += offset * 5    ;
+                                v4rho3sigma    += offset * 4*3  ;
+                                v4rho2sigma2   += offset * 3*6  ;
+                                v4rhosigma3    += offset * 2*10 ;
+                                v4sigma4       += offset * 15   ;
+                                v4rho3tau      += offset * 4*2  ;
+                                v4rho2sigmatau += offset * 3*3*2;
+                                v4rho2tau2     += offset * 3*3  ;
+                                v4rhosigma2tau += offset * 2*6*2;
+                                v4rhosigmatau2 += offset * 2*3*3;
+                                v4rhotau3      += offset * 2*4  ;
+                                v4sigma3tau    += offset * 10*2 ;
+                                v4sigma2tau2   += offset * 6*3  ;
+                                v4sigmatau3    += offset * 3*4  ;
+                                v4tau4         += offset * 5    ;
+                        }
                 } else {
-                        sigma = rho + np;
-                        tau = sigma + np;
+                        sigma = rho + blksize;
+                        tau = sigma + blksize;
                         if (deriv > 0) {
                                 vrho = exc + np;
                                 vsigma = vrho + np;
                                 vtau = vsigma + np;
                         }
                         if (deriv > 1) {
                                 v2rho2      = vtau        + np;
@@ -431,16 +560,61 @@
                                 v4rhosigmatau2 = v4rhosigma2tau + np;
                                 v4rhotau3      = v4rhosigmatau2 + np;
                                 v4sigma3tau    = v4rhotau3      + np;
                                 v4sigma2tau2   = v4sigma3tau    + np;
                                 v4sigmatau3    = v4sigma2tau2   + np;
                                 v4tau4         = v4sigmatau3    + np;
                         }
+
+                        // set offset
+                        exc += offset;
+                        if (deriv > 0) {
+                                vrho   += offset;
+                                vsigma += offset;
+                                vtau   += offset;
+                        }
+                        if (deriv > 1) {
+                                v2rho2      += offset;
+                                v2rhosigma  += offset;
+                                v2sigma2    += offset;
+                                v2rhotau    += offset;
+                                v2sigmatau  += offset;
+                                v2tau2      += offset;
+                        }
+                        if (deriv > 2) {
+                                v3rho3         += offset;
+                                v3rho2sigma    += offset;
+                                v3rhosigma2    += offset;
+                                v3sigma3       += offset;
+                                v3rho2tau      += offset;
+                                v3rhosigmatau  += offset;
+                                v3rhotau2      += offset;
+                                v3sigma2tau    += offset;
+                                v3sigmatau2    += offset;
+                                v3tau3         += offset;
+                        }
+                        if (deriv > 3) {
+                                v4rho4         += offset;
+                                v4rho3sigma    += offset;
+                                v4rho2sigma2   += offset;
+                                v4rhosigma3    += offset;
+                                v4sigma4       += offset;
+                                v4rho3tau      += offset;
+                                v4rho2sigmatau += offset;
+                                v4rho2tau2     += offset;
+                                v4rhosigma2tau += offset;
+                                v4rhosigmatau2 += offset;
+                                v4rhotau3      += offset;
+                                v4sigma3tau    += offset;
+                                v4sigma2tau2   += offset;
+                                v4sigmatau3    += offset;
+                                v4tau4         += offset;
+                        }
                 }
-                xc_mgga(func_x, np, rho, sigma, lapl, tau,
+                xc_mgga(func_x, blksize, rho, sigma, lapl, tau,
                      exc, vrho, vsigma, vlapl, vtau,
                      v2rho2, v2rhosigma, v2rholapl, v2rhotau, v2sigma2,
                      v2sigmalapl, v2sigmatau, v2lapl2, v2lapltau, v2tau2,
                      v3rho3, v3rho2sigma, v3rho2lapl, v3rho2tau, v3rhosigma2,
                      v3rhosigmalapl, v3rhosigmatau, v3rholapl2, v3rholapltau,
                      v3rhotau2, v3sigma3, v3sigma2lapl, v3sigma2tau,
                      v3sigmalapl2, v3sigmalapltau, v3sigmatau2, v3lapl3,
@@ -701,14 +875,15 @@
 static int xc_nvar7_offsets[] = {0, 1, 8, 36, 120, 330};
 
 static void axpy(double *dst, double *src, double fac,
                  int np, int nsrc)
 {
         int i, j;
         for (j = 0; j < nsrc; j++) {
+                #pragma omp parallel for schedule(static)
                 for (i = 0; i < np; i++) {
                         dst[j*np+i] += fac * src[i*nsrc+j];
                 }
         }
 }
 static int vseg1[] = {2, 3, 2};
 static int fseg1[] = {3, 6, 6, 4, 6, 3};
@@ -756,14 +931,15 @@
                         break;
                 }
 
                 for (order = 1; order <= deriv; order++) {
                         pout = dst + offsets1[order] * np;
                         pin = ebuf + offsets0[order] * np;
                         nsrc = offsets0[order+1] - offsets0[order];
+                        #pragma omp parallel for schedule(static)
                         for (i = 0; i < np * nsrc; i++) {
                                 pout[i] += fac * pin[i];
                         }
                 }
                 return;
         }
 
@@ -798,18 +974,44 @@
 // omega is the range separation parameter mu in xcfun
 void LIBXC_eval_xc(int nfn, int *fn_id, double *fac, double *omega,
                    int spin, int deriv, int nvar, int np, int outlen,
                    double *rho_u, double *output, double dens_threshold)
 {
         assert(deriv <= 4);
         double *ebuf = malloc(sizeof(double) * np * outlen);
-        double *rho = malloc(sizeof(double) * np * 7);
-        _eval_rho(rho, rho_u, spin, nvar, np);
-        int nspin = spin + 1;
 
+        double *rhobufs[MAX_THREADS];
+        int offsets[MAX_THREADS+1];
+#pragma omp parallel
+{
+        int iblk = omp_get_thread_num();
+        int nblk = omp_get_num_threads();
+        assert(nblk <= MAX_THREADS);
+
+        int blksize = np / nblk;
+        int ioff = iblk * blksize;
+        int np_mod = np % nblk;
+        if (iblk < np_mod) {
+            blksize += 1;
+        }
+        if (np_mod > 0) {
+            ioff += MIN(iblk, np_mod);
+        }
+        offsets[iblk] = ioff;
+        if (iblk == nblk-1) {
+            offsets[nblk] = np;
+            assert(ioff + blksize == np);
+        }
+
+        double *rho_priv = malloc(sizeof(double) * blksize * 7);
+        rhobufs[iblk] = rho_priv;
+        _eval_rho(rho_priv, rho_u+ioff, spin, nvar, blksize, np);
+}
+
+        int nspin = spin + 1;
         int i, j;
         xc_func_type func;
         for (i = 0; i < nfn; i++) {
                 if (xc_func_init(&func, fn_id[i], nspin) != 0) {
                         fprintf(stderr, "XC functional %d not found\n",
                                 fn_id[i]);
                         raise_error;
@@ -853,21 +1055,33 @@
                 //func->cam_beta  = beta;
                 // However, the parameters can be set with the libxc function
                 //void xc_func_set_ext_params_name(xc_func_type *p, const char *name, double par);
                 // since libxc 5.1.0
 #if defined XC_SET_RELATIVITY
                 xc_lda_x_set_params(&func, relativity);
 #endif
-                _eval_xc(&func, spin, deriv, np, rho, ebuf);
+
+#pragma omp parallel
+{
+                int iblk = omp_get_thread_num();
+                int offset = offsets[iblk];
+                int blksize = offsets[iblk+1] - offset;
+                _eval_xc(&func, spin, deriv, np, rhobufs[iblk], ebuf, offset, blksize);
+}
+
                 merge_xc(output, ebuf, fac[i],
                          spin, deriv, nvar, np, outlen, func.info->family);
                 xc_func_end(&func);
         }
         free(ebuf);
-        free(rho);
+#pragma omp parallel
+{
+        int iblk = omp_get_thread_num();
+        free(rhobufs[iblk]);
+}
 }
 
 int LIBXC_max_deriv_order(int xc_id)
 {
         xc_func_type func;
         int ord;
         if(xc_func_init(&func, xc_id, XC_UNPOLARIZED) != 0){
```

### Comparing `pyscf-2.5.0/pyscf/lib/dft/nr_numint.c` & `pyscf-2.6.0/pyscf/lib/dft/nr_numint.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/dft/nr_numint_sparse.c` & `pyscf-2.6.0/pyscf/lib/dft/nr_numint_sparse.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/dft/numint_uniform_grid.c` & `pyscf-2.6.0/pyscf/lib/dft/numint_uniform_grid.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/dft/r_numint.c` & `pyscf-2.6.0/pyscf/lib/dft/r_numint.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/dft/xc_deriv.c` & `pyscf-2.6.0/pyscf/lib/dft/xc_deriv.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/dft/xcfun_itrf.c` & `pyscf-2.6.0/pyscf/lib/dft/xcfun_itrf.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/diis.py` & `pyscf-2.6.0/pyscf/lib/diis.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,11 +330,13 @@
 
         space = max(nd, self.space)
         self._H = numpy.zeros((space+1,space+1), e_mat.dtype)
         self._H[0,1:] = self._H[1:,0] = 1
         self._H[1:nd+1,1:nd+1] = e_mat
         return self
 
+    to_gpu = misc.to_gpu
+
 
 def restore(filename):
     '''Restore/construct diis object based on a diis file'''
     return DIIS().restore(filename)
```

### Comparing `pyscf-2.5.0/pyscf/lib/exceptions.py` & `pyscf-2.6.0/pyscf/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/CMakeLists.txt` & `pyscf-2.6.0/pyscf/lib/gto/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/autocode/auto_eval1.c` & `pyscf-2.6.0/pyscf/lib/gto/autocode/auto_eval1.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/deriv1.c` & `pyscf-2.6.0/pyscf/lib/gto/deriv1.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/deriv2.c` & `pyscf-2.6.0/pyscf/lib/gto/deriv2.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/fastexp.c` & `pyscf-2.6.0/pyscf/lib/gto/fastexp.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/fill_grids_int2c.c` & `pyscf-2.6.0/pyscf/lib/gto/fill_grids_int2c.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/fill_int2c.c` & `pyscf-2.6.0/pyscf/lib/gto/fill_int2c.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/fill_int2e.c` & `pyscf-2.6.0/pyscf/lib/gto/fill_int2e.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/fill_nr_3c.c` & `pyscf-2.6.0/pyscf/lib/gto/fill_nr_3c.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/fill_r_3c.c` & `pyscf-2.6.0/pyscf/lib/gto/fill_r_3c.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/fill_r_4c.c` & `pyscf-2.6.0/pyscf/lib/gto/fill_r_4c.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/ft_ao.c` & `pyscf-2.6.0/pyscf/lib/gto/ft_ao.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/ft_ao.h` & `pyscf-2.6.0/pyscf/lib/gto/ft_ao.h`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/ft_ao_deriv.c` & `pyscf-2.6.0/pyscf/lib/gto/ft_ao_deriv.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/grid_ao_drv.c` & `pyscf-2.6.0/pyscf/lib/gto/grid_ao_drv.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/grid_ao_drv.h` & `pyscf-2.6.0/pyscf/lib/gto/grid_ao_drv.h`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/gto.h` & `pyscf-2.6.0/pyscf/lib/gto/gto.h`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/nr_ecp.c` & `pyscf-2.6.0/pyscf/lib/gto/nr_ecp.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/nr_ecp.h` & `pyscf-2.6.0/pyscf/lib/gto/nr_ecp.h`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/gto/nr_ecp_deriv.c` & `pyscf-2.6.0/pyscf/lib/gto/nr_ecp_deriv.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/linalg_helper.py` & `pyscf-2.6.0/pyscf/lib/linalg_helper.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/logger.py` & `pyscf-2.6.0/pyscf/lib/logger.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/mcscf/CMakeLists.txt` & `pyscf-2.6.0/pyscf/lib/mcscf/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/mcscf/fci.h` & `pyscf-2.6.0/pyscf/lib/mcscf/fci.h`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/mcscf/fci_4pdm.c` & `pyscf-2.6.0/pyscf/lib/mcscf/fci_4pdm.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/mcscf/fci_contract.c` & `pyscf-2.6.0/pyscf/lib/mcscf/fci_contract.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/mcscf/fci_contract_nosym.c` & `pyscf-2.6.0/pyscf/lib/mcscf/fci_contract_nosym.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/mcscf/fci_rdm.c` & `pyscf-2.6.0/pyscf/lib/mcscf/fci_rdm.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/mcscf/fci_string.c` & `pyscf-2.6.0/pyscf/lib/mcscf/fci_string.c`

 * *Files 1% similar despite different names*

```diff
@@ -126,20 +126,15 @@
                 return 1;
         } else if (n <= 20) {
                 return _binomial_cache[n*(n-1)/2+m];
         } else {
                 if (m*2 <= n) {
                         m = n - m;
                 }
-                uint64_t i;
-                uint64_t val = 1;
-                for (i = m; i <= n; i++) {
-                        val *= i;
-                        val /= i - m;
-                }
+		int val = binomial(n-1,m-1) + binomial(n-1,m);
                 return val;
         }
 }
 
 int FCIstr2addr(int norb, int nelec, uint64_t string)
 {
         size_t addr = 0;
```

### Comparing `pyscf-2.5.0/pyscf/lib/mcscf/nevpt_contract.c` & `pyscf-2.6.0/pyscf/lib/mcscf/nevpt_contract.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/mcscf/select_ci.c` & `pyscf-2.6.0/pyscf/lib/mcscf/select_ci.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/misc.py` & `pyscf-2.6.0/pyscf/lib/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,25 @@
 
 '''
 Some helper functions
 '''
 
 import os
 import sys
+import time
+import platform
 import warnings
 import tempfile
 import functools
 import itertools
 import inspect
 import collections
 import ctypes
 import numpy
+import scipy
 import h5py
 from threading import Thread
 from multiprocessing import Queue, Process
 try:
     from concurrent.futures import ThreadPoolExecutor
 except ImportError:
     ThreadPoolExecutor = None
@@ -1299,14 +1302,31 @@
             branch = os.path.basename(head)
             with open(os.path.join(repo_path, '.git', head.split(' ')[1]), 'r') as f:
                 head = f.read().strip()
     except IOError:
         pass
     return orig_head, head, branch
 
+def format_sys_info():
+    '''Format a list of system information for printing.'''
+    import pyscf
+    info = repo_info(os.path.join(__file__, '..', '..'))
+    result = [
+        f'System: {platform.uname()}  Threads {num_threads()}',
+        f'Python {sys.version}',
+        f'numpy {numpy.__version__}  scipy {scipy.__version__}  '
+        f'h5py {h5py.__version__}',
+        f'Date: {time.ctime()}',
+        f'PySCF version {pyscf.__version__}',
+        f'PySCF path  {info["path"]}',
+    ]
+    if 'git' in info:
+        result.append(info['git'])
+    return result
+
 
 def isinteger(obj):
     '''
     Check if an object is an integer.
     '''
     # A bool is also an int in python, but we don't want that.
     # On the other hand, numpy.bool_ is probably not a numpy.integer, but just to be sure...
@@ -1337,21 +1357,79 @@
         return issubclass(obj.dtype.type, numpy.integer)
     else:
         are_ints = True
         for i in obj:
             are_ints = are_ints and isinteger(i)
         return are_ints
 
-def to_gpu(method):
-    '''Recursively converts all attributes of a method to cupy objects or
-    gpu4pyscf objects.
+class _OmniObject:
+    '''Class with default attributes. When accessing an attribute that is not
+    initialized, a default value will be returned than raising an AttributeError.
+    '''
+    verbose = 0
+    max_memory = param.MAX_MEMORY
+    stdout = sys.stdout
+
+    def __init__(self, default_factory=None):
+        self._default = default_factory
+
+    def __getattr__(self, key):
+        return self._default
+
+# Many methods requires a mol or mf object in initialization.
+# These objects can be as the default arguments for these methods.
+# Then class can be instantiated easily like cls(omniobj) in the following
+# to_gpu function.
+omniobj = _OmniObject()
+omniobj._built = True
+omniobj.mol = omniobj
+omniobj._scf = omniobj
+omniobj.base = omniobj
+
+def to_gpu(method, out=None):
+    '''Convert a method to its corresponding GPU variant, and recursively
+    converts all attributes of a method to cupy objects or gpu4pyscf objects.
     '''
     import cupy
     from pyscf import gto
-    for key, val in method.__dict__.items():
-        if isinstance(val, gto.MoleBase):
-            continue
+
+    # If a GPU class inherits a CPU code, the "to_gpu" method may be resolved
+    # and available in the GPU class. Skip the conversion in this case.
+    if method.__module__.startswith('gpu4pyscf'):
+        return method
+
+    if out is None:
+        try:
+            import gpu4pyscf
+        except ImportError:
+            print('Library gpu4pyscf not found. You can install this package via\n'
+                  '    pip install gpu4pyscf-cuda11x\n'
+                  'See more installation info at https://github.com/pyscf/gpu4pyscf')
+            raise
+
+        # TODO: Is it necessary to implement scanner in gpu4pyscf?
+        if isinstance(method, (SinglePointScanner, GradScanner)):
+            method = method.undo_scanner()
+
+        from importlib import import_module
+        mod = import_module(method.__module__.replace('pyscf', 'gpu4pyscf'))
+        cls = getattr(mod, method.__class__.__name__)
+        # A temporary GPU instance. This ensures to initialize private
+        # attributes that are only available for GPU code.
+        out = cls(omniobj)
+
+    # Convert only the keys that are defined in the corresponding GPU class
+    cls_keys = [getattr(cls, '_keys', ()) for cls in out.__class__.__mro__[:-1]]
+    out_keys = set(out.__dict__).union(*cls_keys)
+    # Only overwrite the attributes of the same name.
+    keys = set(method.__dict__).intersection(out_keys)
+
+    for key in keys:
+        val = getattr(method, key)
         if isinstance(val, numpy.ndarray):
-            setattr(method, key, cupy.asarray(val))
+            val = cupy.asarray(val)
         elif hasattr(val, 'to_gpu'):
-            setattr(method, key, val.to_gpu())
-    return method
+            val = val.to_gpu()
+        setattr(out, key, val)
+    out.reset()
+    return out
+
```

### Comparing `pyscf-2.5.0/pyscf/lib/np_helper/CMakeLists.txt` & `pyscf-2.6.0/pyscf/lib/np_helper/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/np_helper/condense.c` & `pyscf-2.6.0/pyscf/lib/np_helper/condense.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/np_helper/np_helper.c` & `pyscf-2.6.0/pyscf/lib/np_helper/np_helper.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/np_helper/np_helper.h` & `pyscf-2.6.0/pyscf/lib/np_helper/np_helper.h`

 * *Files 4% similar despite different names*

```diff
@@ -57,7 +57,14 @@
 void NPomp_zsum_reduce_inplace(double complex **vec, size_t count);
 void NPomp_zprod_reduce_inplace(double complex **vec, size_t count);
 
 void NPdset0(double *p, const size_t n);
 void NPzset0(double complex *p, const size_t n);
 void NPdcopy(double *out, const double *in, const size_t n);
 void NPzcopy(double complex *out, const double complex *in, const size_t n);
+
+void NPdgemm(const char trans_a, const char trans_b,
+             const int m, const int n, const int k,
+             const int lda, const int ldb, const int ldc,
+             const int offseta, const int offsetb, const int offsetc,
+             double *a, double *b, double *c,
+             const double alpha, const double beta);
```

### Comparing `pyscf-2.5.0/pyscf/lib/np_helper/npdot.c` & `pyscf-2.6.0/pyscf/lib/np_helper/npdot.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/np_helper/omp_reduce.c` & `pyscf-2.6.0/pyscf/lib/np_helper/omp_reduce.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/np_helper/pack_tril.c` & `pyscf-2.6.0/pyscf/lib/np_helper/pack_tril.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/np_helper/transpose.c` & `pyscf-2.6.0/pyscf/lib/np_helper/transpose.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/numpy_helper.py` & `pyscf-2.6.0/pyscf/lib/numpy_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # Author: Qiming Sun <osirpt.sun@gmail.com>
 #
 
 '''
 Extension to numpy and scipy
 '''
 
-import string
 import ctypes
 import math
 import numpy
 from pyscf.lib import misc
 from numpy import asarray  # For backward compatibility
 
 EINSUM_MAX_SIZE = getattr(misc.__config__, 'lib_einsum_max_size', 2000)
@@ -153,15 +152,15 @@
         print("rangeA =", rangeA)
         print("rangeB =", rangeB)
 
     idxAt = list(idxA)
     idxBt = list(idxB)
     inner_shape = 1
     insert_B_loc = 0
-    shared_idxAB = sorted(list(shared_idxAB))
+    shared_idxAB = sorted(shared_idxAB)
     for n in shared_idxAB:
         if rangeA[n] != rangeB[n]:
             err = ('ERROR: In index string %s, the range of index %s is '
                    'different in A (%d) and B (%d)' %
                    (idx_str, n, rangeA[n], rangeB[n]))
             raise ValueError(err)
 
@@ -1112,14 +1111,22 @@
         y += b
     buf, bs = bs[0], None
     for i in range(n):
         ddot(y, y, 1, buf, 0)
         y, buf = buf, y
     return y
 
+def ndarray_pointer_2d(array):
+    '''Return an array that contains the addresses of the first element in each
+    row of the input 2d array.
+    '''
+    assert array.ndim == 2
+    assert array.flags.c_contiguous
+    i = numpy.arange(array.shape[0])
+    return array.ctypes.data + (i * array.strides[0]).astype(numpy.uintp)
 
 class NPArrayWithTag(numpy.ndarray):
     # Initialize kwargs in function tag_array
     #def __new__(cls, a, **kwargs):
     #    obj = numpy.asarray(a).view(cls)
     #    obj.__dict__.update(kwargs)
     #    return obj
```

### Comparing `pyscf-2.5.0/pyscf/lib/parameters.py` & `pyscf-2.6.0/pyscf/lib/parameters.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/pbc/CMakeLists.txt` & `pyscf-2.6.0/pyscf/lib/pbc/CMakeLists.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 add_library(pbc SHARED ft_ao.c fill_ints.c fill_ints_sr.c optimizer.c grid_ao.c
-  nr_direct.c symmetry.c inner_dot.c cint2e.c cint3c2e.c nr_ecp.c transform_mo.c)
+  nr_direct.c symmetry.c inner_dot.c cint2e.c cint3c2e.c nr_ecp.c transform_mo.c
+  neighbor_list.c cell.c pp.c hf_grad.c fill_ints_screened.c)
 add_dependencies(pbc cgto cvhf np_helper)
 
 set_target_properties(pbc PROPERTIES
   LIBRARY_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR})
 
 target_link_libraries(pbc cgto cint cvhf np_helper ${BLAS_LIBRARIES} ${OPENMP_C_PROPERTIES})
+
+if(ENABLE_FFTW)
+add_library(fft SHARED fft.c)
+set_target_properties(fft PROPERTIES
+  LIBRARY_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}
+  COMPILE_FLAGS ${OpenMP_C_FLAGS}
+  LINK_FLAGS ${OpenMP_C_FLAGS})
+target_link_libraries(fft fftw3_threads fftw3 ${BLAS_LIBRARIES})
+endif()
```

### Comparing `pyscf-2.5.0/pyscf/lib/pbc/cint2e.c` & `pyscf-2.6.0/pyscf/lib/pbc/cint2e.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/pbc/cint3c2e.c` & `pyscf-2.6.0/pyscf/lib/pbc/cint3c2e.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/pbc/fill_ints.c` & `pyscf-2.6.0/pyscf/lib/pbc/fill_ints.c`

 * *Files 0% similar despite different names*

```diff
@@ -1256,17 +1256,17 @@
 static void shift_bas(double *env_loc, double *env, double *Ls, int ptr, int iL)
 {
         env_loc[ptr+0] = env[ptr+0] + Ls[iL*3+0];
         env_loc[ptr+1] = env[ptr+1] + Ls[iL*3+1];
         env_loc[ptr+2] = env[ptr+2] + Ls[iL*3+2];
 }
 
-static void sort2c_ks1(double complex *out, double *bufr, double *bufi,
-                       int *shls_slice, int *ao_loc, int nkpts, int comp,
-                       int jsh, int msh0, int msh1)
+void sort2c_ks1(double complex *out, double *bufr, double *bufi,
+                int *shls_slice, int *ao_loc, int nkpts, int comp,
+                int jsh, int msh0, int msh1)
 {
         const int ish0 = shls_slice[0];
         const int ish1 = shls_slice[1];
         const int jsh0 = shls_slice[2];
         const int jsh1 = shls_slice[3];
         const size_t naoi = ao_loc[ish1] - ao_loc[ish0];
         const size_t naoj = ao_loc[jsh1] - ao_loc[jsh0];
```

### Comparing `pyscf-2.5.0/pyscf/lib/pbc/fill_ints_sr.c` & `pyscf-2.6.0/pyscf/lib/pbc/fill_ints_sr.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/pbc/ft_ao.c` & `pyscf-2.6.0/pyscf/lib/pbc/ft_ao.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/pbc/grid_ao.c` & `pyscf-2.6.0/pyscf/lib/pbc/grid_ao.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/pbc/inner_dot.c` & `pyscf-2.6.0/pyscf/lib/pbc/inner_dot.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/pbc/nr_direct.c` & `pyscf-2.6.0/pyscf/lib/pbc/nr_direct.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/pbc/nr_ecp.c` & `pyscf-2.6.0/pyscf/lib/pbc/nr_ecp.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/pbc/optimizer.c` & `pyscf-2.6.0/pyscf/lib/pbc/optimizer.c`

 * *Files 19% similar despite different names*

```diff
@@ -13,43 +13,47 @@
     limitations under the License.
 
  *
  * Author: Qiming Sun <osirpt.sun@gmail.com>
  */
 
 #include <stdlib.h>
+#include <math.h>
 #include "cint.h"
 #include "pbc/optimizer.h"
 
 #define SQUARE(r)       (r[0]*r[0]+r[1]*r[1]+r[2]*r[2])
 
 void PBCinit_optimizer(PBCOpt **opt, int *atm, int natm,
                         int *bas, int nbas, double *env)
 {
         PBCOpt *opt0 = malloc(sizeof(PBCOpt));
         opt0->rrcut = NULL;
+        opt0->rcut = NULL;
         opt0->fprescreen = &PBCnoscreen;
         *opt = opt0;
 }
 
 void PBCdel_optimizer(PBCOpt **opt)
 {
         PBCOpt *opt0 = *opt;
         if (opt0 == NULL) {
                 return;
         }
 
         if (opt0->rrcut != NULL) {
                 free(opt0->rrcut);
         }
+        if (!opt0->rcut) {
+                free(opt0->rcut);
+        }
         free(opt0);
         *opt = NULL;
 }
 
-
 int PBCnoscreen(int *shls, PBCOpt *opt, int *atm, int *bas, double *env)
 {
         return 1;
 }
 
 int PBCrcut_screen(int *shls, PBCOpt *opt, int *atm, int *bas, double *env)
 {
@@ -64,21 +68,53 @@
         rirj[0] = ri[0] - rj[0];
         rirj[1] = ri[1] - rj[1];
         rirj[2] = ri[2] - rj[2];
         double rr = SQUARE(rirj);
         return (rr < opt->rrcut[ish] || rr < opt->rrcut[jsh]);
 }
 
+int PBCrcut_screen_loose(int *shls, PBCOpt *opt, int *atm, int *bas, double *env)
+{
+        if (opt == NULL) {
+                return 1; // no screen
+        }
+        const int ish = shls[0];
+        const int jsh = shls[1];
+        const double *ri = env + atm[bas[ATOM_OF+ish*BAS_SLOTS]*ATM_SLOTS+PTR_COORD];
+        const double *rj = env + atm[bas[ATOM_OF+jsh*BAS_SLOTS]*ATM_SLOTS+PTR_COORD];
+        double rirj[3];
+        rirj[0] = ri[0] - rj[0];
+        rirj[1] = ri[1] - rj[1];
+        rirj[2] = ri[2] - rj[2];
+        double r = sqrt(SQUARE(rirj));
+        return r < opt->rcut[ish] + opt->rcut[jsh];
+}
+
 void PBCset_rcut_cond(PBCOpt *opt, double *rcut,
                       int *atm, int natm, int *bas, int nbas, double *env)
 {
         if (opt->rrcut != NULL) {
                 free(opt->rrcut);
         }
         opt->rrcut = (double *)malloc(sizeof(double) * nbas);
         opt->fprescreen = &PBCrcut_screen;
 
         int i;
         for (i = 0; i < nbas; i++) {
                 opt->rrcut[i] = rcut[i] * rcut[i];
         }
 }
+
+void PBCset_rcut_cond_loose(PBCOpt *opt, double *rcut,
+                            int *atm, int natm, int *bas, int nbas, double *env)
+{
+        if (opt->rcut != NULL) {
+                free(opt->rcut);
+        }
+        opt->rcut = (double *)malloc(sizeof(double) * nbas);
+        opt->fprescreen = &PBCrcut_screen_loose;
+
+        int i;
+        for (i = 0; i < nbas; i++) {
+                opt->rcut[i] = rcut[i];
+        }
+}
```

### Comparing `pyscf-2.5.0/pyscf/lib/pbc/optimizer.h` & `pyscf-2.6.0/pyscf/lib/pbc/optimizer.h`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,19 @@
     See the License for the specific language governing permissions and
     limitations under the License.
 
  *
  * Author: Qiming Sun <osirpt.sun@gmail.com>
  */
 
-#if !defined(HAVE_DEFINED_CVHFOPT_H)
-#define HAVE_DEFINED_CVHFOPT_H
+#if !defined(HAVE_DEFINED_PBCOPT_H)
+#define HAVE_DEFINED_PBCOPT_H
 typedef struct PBCOpt_struct {
     double *rrcut;
+    double *rcut;
     int (*fprescreen)(int *shls, struct PBCOpt_struct *opt,
                       int *atm, int *bas, double *env);
 } PBCOpt;
 #endif
 
 int PBCnoscreen(int *shls, PBCOpt *opt, int *atm, int *bas, double *env);
 int PBCrcut_screen(int *shls, PBCOpt *opt, int *atm, int *bas, double *env);
-
```

### Comparing `pyscf-2.5.0/pyscf/lib/pbc/pbc.h` & `pyscf-2.6.0/pyscf/lib/pbc/pbc.h`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/pbc/symmetry.c` & `pyscf-2.6.0/pyscf/lib/pbc/symmetry.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/pbc/transform_mo.c` & `pyscf-2.6.0/pyscf/lib/pbc/transform_mo.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/ri/CMakeLists.txt` & `pyscf-2.6.0/pyscf/lib/ri/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/ri/r_df_incore.c` & `pyscf-2.6.0/pyscf/lib/ri/r_df_incore.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/scipy_helper.py` & `pyscf-2.6.0/pyscf/lib/scipy_helper.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/CMakeLists.txt` & `pyscf-2.6.0/pyscf/lib/vhf/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/cvhf.h` & `pyscf-2.6.0/pyscf/lib/vhf/cvhf.h`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/fblas.h` & `pyscf-2.6.0/pyscf/lib/vhf/fblas.h`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/fill_nr_s8.c` & `pyscf-2.6.0/pyscf/lib/vhf/fill_nr_s8.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/hessian_screen.c` & `pyscf-2.6.0/pyscf/lib/vhf/hessian_screen.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/nr_direct.c` & `pyscf-2.6.0/pyscf/lib/vhf/nr_direct.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/nr_direct.h` & `pyscf-2.6.0/pyscf/lib/vhf/nr_direct.h`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/nr_direct_dot.c` & `pyscf-2.6.0/pyscf/lib/vhf/nr_direct_dot.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/nr_incore.c` & `pyscf-2.6.0/pyscf/lib/vhf/nr_incore.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/nr_sgx_direct.c` & `pyscf-2.6.0/pyscf/lib/vhf/nr_sgx_direct.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/nr_sr_vhf.c` & `pyscf-2.6.0/pyscf/lib/vhf/nr_sr_vhf.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/optimizer.c` & `pyscf-2.6.0/pyscf/lib/vhf/optimizer.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/optimizer.h` & `pyscf-2.6.0/pyscf/lib/vhf/optimizer.h`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/r_direct_dot.c` & `pyscf-2.6.0/pyscf/lib/vhf/r_direct_dot.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/r_direct_dot.h` & `pyscf-2.6.0/pyscf/lib/vhf/r_direct_dot.h`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/r_direct_o1.c` & `pyscf-2.6.0/pyscf/lib/vhf/r_direct_o1.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/rah_direct_dot.c` & `pyscf-2.6.0/pyscf/lib/vhf/rah_direct_dot.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/rha_direct_dot.c` & `pyscf-2.6.0/pyscf/lib/vhf/rha_direct_dot.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/rkb_screen.c` & `pyscf-2.6.0/pyscf/lib/vhf/rkb_screen.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/time_rev.c` & `pyscf-2.6.0/pyscf/lib/vhf/time_rev.c`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lib/vhf/time_rev.h` & `pyscf-2.6.0/pyscf/lib/vhf/time_rev.h`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lo/__init__.py` & `pyscf-2.6.0/pyscf/lo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lo/boys.py` & `pyscf-2.6.0/pyscf/lo/boys.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lo/cholesky.py` & `pyscf-2.6.0/pyscf/lo/cholesky.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lo/edmiston.py` & `pyscf-2.6.0/pyscf/lo/edmiston.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lo/iao.py` & `pyscf-2.6.0/pyscf/lo/iao.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lo/ibo.py` & `pyscf-2.6.0/pyscf/lo/ibo.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lo/nao.py` & `pyscf-2.6.0/pyscf/lo/nao.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lo/orth.py` & `pyscf-2.6.0/pyscf/lo/orth.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lo/pipek.py` & `pyscf-2.6.0/pyscf/lo/pipek.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lo/pipek_jacobi.py` & `pyscf-2.6.0/pyscf/lo/pipek_jacobi.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/lo/vvo.py` & `pyscf-2.6.0/pyscf/lo/vvo.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/mcscf/PiOS.py` & `pyscf-2.6.0/pyscf/mcscf/PiOS.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/mcscf/__init__.py` & `pyscf-2.6.0/pyscf/mcscf/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,65 +77,51 @@
 
 The Following attributes are used for CASSCF
 
     conv_tol : float
         Converge threshold.  Default is 1e-7
     conv_tol_grad : float
         Converge threshold for CI gradients and orbital rotation gradients.
-        Default is 1e-4
+        If not specified, it is set to sqrt(conv_tol).
     max_stepsize : float
         The step size for orbital rotation.  Small step size is prefered.
-        Default is 0.03.  
+        Default is 0.02.  
         (NOTE although the default step size is small enough for many systems,
         it happens that the orbital optimizor crosses the barriar of local
         minimum and converge to the neighbour solution, e.g. the CAS(4,4) for
         C2H4 in the test files.  In these systems, adjusting max_stepsize,
-        max_ci_stepsize and max_cycle_micro, max_cycle_micro_inner and
-        ah_start_tol may be helpful)
+        max_ci_stepsize and max_cycle_micro and ah_start_tol may be helpful)
 
         >>> mc = mcscf.CASSCF(mf, 6, 6)
         >>> mc.max_stepsize = .01
         >>> mc.max_cycle_micro = 1
         >>> mc.max_cycle_macro = 100
-        >>> mc.max_cycle_micro_inner = 1
         >>> mc.ah_start_tol = 1e-6
 
-    max_ci_stepsize : float
-        The max size for approximate CI updates.  The approximate updates are
-        used in 1-step algorithm, to estimate the change of CI wavefunction wrt
-        the orbital rotation.  Small step size is prefered.  Default is 0.01.
     max_cycle_macro : int
         Max number of macro iterations.  Default is 50.
     max_cycle_micro : int
         Max number of micro iterations in each macro iteration.  Depending on
         systems, increasing this value might reduce the total macro
-        iterations.  Generally, 2 - 3 steps should be enough.  Default is 2.
-    max_cycle_micro_inner : int
-        Max number of steps for the orbital rotations allowed for the augmented
-        hessian solver.  It can affect the actual size of orbital rotation.
-        Even with a small max_stepsize, a few max_cycle_micro_inner can
-        accumulate the rotation and leads to a significant change of the CAS
-        space.  Depending on systems, increasing this value migh reduce the
-        total number of macro iterations.  The value between 2 - 8 is preferred.
-        Default is 4.
+        iterations.  Generally, 2 - 5 steps should be enough.  Default is 4.
     frozen : int or list
         If integer is given, the inner-most orbitals are excluded from optimization.
         Given the orbital indices (0-based) in a list, any doubly occupied core
         orbitals, active orbitals and external orbitals can be frozen.
     ah_level_shift : float, for AH solver.
         Level shift for the Davidson diagonalization in AH solver.  Default is 0.
     ah_conv_tol : float, for AH solver.
         converge threshold for Davidson diagonalization in AH solver.  Default is 1e-8.
     ah_max_cycle : float, for AH solver.
         Max number of iterations allowd in AH solver.  Default is 20.
     ah_lindep : float, for AH solver.
         Linear dependence threshold for AH solver.  Default is 1e-16.
     ah_start_tol : flat, for AH solver.
         In AH solver, the orbital rotation is started without completely solving the AH problem.
-        This value is to control the start point. Default is 1e-4.
+        This value is to control the start point. Default is 2.5.
     ah_start_cycle : int, for AH solver.
         In AH solver, the orbital rotation is started without completely solving the AH problem.
         This value is to control the start point. Default is 3.
 
         ``ah_conv_tol``, ``ah_max_cycle``, ``ah_lindep``, ``ah_start_tol`` and ``ah_start_cycle``
         can affect the accuracy and performance of CASSCF solver.  Lower
         ``ah_conv_tol`` and ``ah_lindep`` can improve the accuracy of CASSCF
@@ -200,15 +186,15 @@
         mf = mf_or_mol
 
     if isinstance(mf, scf.uhf.UHF):
         mf = mf.to_rhf()
     if isinstance(mf, _DFHF) and mf.with_df:
         return DFCASSCF(mf, ncas, nelecas, ncore, frozen)
 
-    if mf.mol.symmetry:
+    if mf.mol.symmetry and mf.mol.groupname != 'C1':
         mc = mc1step_symm.CASSCF(mf, ncas, nelecas, ncore, frozen)
     else:
         mc = mc1step.CASSCF(mf, ncas, nelecas, ncore, frozen)
     return mc
 
 RCASSCF = CASSCF
 
@@ -224,15 +210,15 @@
 
     if isinstance(mf, scf.uhf.UHF):
         mf = mf.to_rhf()
 
     if isinstance(mf, _DFHF) and mf.with_df:
         return DFCASCI(mf, ncas, nelecas, ncore)
 
-    if mf.mol.symmetry:
+    if mf.mol.symmetry and mf.mol.groupname != 'C1':
         mc = casci_symm.CASCI(mf, ncas, nelecas, ncore)
     else:
         mc = casci.CASCI(mf, ncas, nelecas, ncore)
     return mc
 
 RCASCI = CASCI
 
@@ -289,15 +275,15 @@
         mf = mf_or_mol.RHF().density_fit()
     else:
         mf = mf_or_mol
 
     if isinstance(mf, scf.uhf.UHF):
         mf = mf.to_rhf()
 
-    if mf.mol.symmetry:
+    if mf.mol.symmetry and mf.mol.groupname != 'C1':
         mc = mc1step_symm.CASSCF(mf, ncas, nelecas, ncore, frozen)
     else:
         mc = mc1step.CASSCF(mf, ncas, nelecas, ncore, frozen)
     return df.density_fit(mc, auxbasis)
 
 def DFCASCI(mf_or_mol, ncas, nelecas, auxbasis=None, ncore=None):
     from pyscf import gto
@@ -306,15 +292,15 @@
         mf = mf_or_mol.RHF().density_fit()
     else:
         mf = mf_or_mol
 
     if isinstance(mf, scf.uhf.UHF):
         mf = mf.to_rhf()
 
-    if mf.mol.symmetry:
+    if mf.mol.symmetry and mf.mol.groupname != 'C1':
         mc = casci_symm.CASCI(mf, ncas, nelecas, ncore)
     else:
         mc = casci.CASCI(mf, ncas, nelecas, ncore)
     return df.density_fit(mc, auxbasis)
 
 approx_hessian = df.approx_hessian
```

### Comparing `pyscf-2.5.0/pyscf/mcscf/addons.py` & `pyscf-2.6.0/pyscf/mcscf/addons.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/mcscf/apc.py` & `pyscf-2.6.0/pyscf/mcscf/apc.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/mcscf/avas.py` & `pyscf-2.6.0/pyscf/mcscf/avas.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/mcscf/casci.py` & `pyscf-2.6.0/pyscf/mcscf/casci.py`

 * *Files 0% similar despite different names*

```diff
@@ -766,15 +766,15 @@
 
     _keys = {
         'natorb', 'canonicalization', 'sorting_mo_energy', 'mol', 'max_memory',
         'ncas', 'nelecas', 'ncore', 'fcisolver', 'frozen', 'extrasym',
         'e_tot', 'e_cas', 'ci', 'mo_coeff', 'mo_energy', 'mo_occ', 'converged',
     }
 
-    def __init__(self, mf_or_mol, ncas, nelecas, ncore=None):
+    def __init__(self, mf_or_mol, ncas=0, nelecas=0, ncore=None):
         if isinstance(mf_or_mol, gto.Mole):
             mf = scf.RHF(mf_or_mol)
         else:
             mf = mf_or_mol
 
         mol = mf.mol
         self.mol = mol
@@ -1166,11 +1166,13 @@
 
     as_scanner = as_scanner
 
     def nuc_grad_method(self):
         from pyscf.grad import casci
         return casci.Gradients(self)
 
+    to_gpu = lib.to_gpu
+
 scf.hf.RHF.CASCI = scf.rohf.ROHF.CASCI = lib.class_as_method(CASCI)
 scf.uhf.UHF.CASCI = None
 
 del (WITH_META_LOWDIN, LARGE_CI_TOL, PENALTY)
```

### Comparing `pyscf-2.5.0/pyscf/mcscf/casci_symm.py` & `pyscf-2.6.0/pyscf/mcscf/casci_symm.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from pyscf import symm
 from pyscf import fci
 from pyscf.mcscf import casci
 from pyscf.mcscf import addons
 from pyscf.scf.hf_symm import map_degeneracy
 
 class SymAdaptedCASCI(casci.CASCI):
-    def __init__(self, mf_or_mol, ncas, nelecas, ncore=None):
+    def __init__(self, mf_or_mol, ncas=0, nelecas=0, ncore=None):
         casci.CASCI.__init__(self, mf_or_mol, ncas, nelecas, ncore)
 
         assert (self.mol.symmetry)
         fcisolver = self.fcisolver
         if isinstance(fcisolver, fci.direct_spin0.FCISolver):
             self.fcisolver = fci.direct_spin0_symm.FCISolver(self.mol)
         else:
@@ -70,14 +70,16 @@
         '''Select active space based on symmetry information.
         See also :func:`pyscf.mcscf.addons.sort_mo_by_irrep`
         '''
         if mo_coeff is None: mo_coeff = self.mo_coeff
         return addons.sort_mo_by_irrep(self, mo_coeff, cas_irrep_nocc,
                                        cas_irrep_ncore, s)
 
+    to_gpu = lib.to_gpu
+
 CASCI = SymAdaptedCASCI
 
 def eig(mat, orbsym):
     orbsym = numpy.asarray(orbsym)
     norb = mat.shape[0]
     e = numpy.zeros(norb)
     c = numpy.zeros((norb,norb))
```

### Comparing `pyscf-2.5.0/pyscf/mcscf/chkfile.py` & `pyscf-2.6.0/pyscf/mcscf/chkfile.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/mcscf/df.py` & `pyscf-2.6.0/pyscf/mcscf/df.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/mcscf/dmet_cas.py` & `pyscf-2.6.0/pyscf/mcscf/dmet_cas.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/mcscf/mc1step.py` & `pyscf-2.6.0/pyscf/mcscf/mc1step.py`

 * *Files 1% similar despite different names*

```diff
@@ -591,24 +591,24 @@
 
     Extra attributes for CASSCF:
 
         conv_tol : float
             Converge threshold.  Default is 1e-7
         conv_tol_grad : float
             Converge threshold for CI gradients and orbital rotation gradients.
-            Default is 1e-4
+            If not specified, it is set to sqrt(conv_tol).
         max_stepsize : float
             The step size for orbital rotation.  Small step (0.005 - 0.05) is prefered.
-            Default is 0.03.
+            Default is 0.02.
         max_cycle_macro : int
             Max number of macro iterations.  Default is 50.
         max_cycle_micro : int
             Max number of micro iterations in each macro iteration.  Depending on
             systems, increasing this value might reduce the total macro
-            iterations.  Generally, 2 - 5 steps should be enough.  Default is 3.
+            iterations.  Generally, 2 - 5 steps should be enough.  Default is 4.
         small_rot_tol : float
             Threshold for orbital rotation to be considered small. If the largest orbital
             rotation is smaller than this value, the CI solver will restart from the
             previous iteration if supported.
             Default is 0.01
         ah_level_shift : float, for AH solver.
             Level shift for the Davidson diagonalization in AH solver.  Default is 1e-8.
@@ -616,18 +616,18 @@
             converge threshold for AH solver.  Default is 1e-12.
         ah_max_cycle : float, for AH solver.
             Max number of iterations allowd in AH solver.  Default is 30.
         ah_lindep : float, for AH solver.
             Linear dependence threshold for AH solver.  Default is 1e-14.
         ah_start_tol : flat, for AH solver.
             In AH solver, the orbital rotation is started without completely solving the AH problem.
-            This value is to control the start point. Default is 0.2.
+            This value is to control the start point. Default is 2.5.
         ah_start_cycle : int, for AH solver.
             In AH solver, the orbital rotation is started without completely solving the AH problem.
-            This value is to control the start point. Default is 2.
+            This value is to control the start point. Default is 3.
 
             ``ah_conv_tol``, ``ah_max_cycle``, ``ah_lindep``, ``ah_start_tol`` and ``ah_start_cycle``
             can affect the accuracy and performance of CASSCF solver.  Lower
             ``ah_conv_tol`` and ``ah_lindep`` might improve the accuracy of CASSCF
             optimization, but decrease the performance.
 
             >>> from pyscf import gto, scf, mcscf
@@ -751,15 +751,15 @@
         'fcisolver_max_cycle', 'fcisolver_conv_tol', 'natorb',
         'canonicalization', 'sorting_mo_energy', 'scale_restoration',
         'small_rot_tol', 'extrasym', 'callback',
         'frozen', 'chkfile', 'fcisolver', 'e_tot', 'e_cas', 'ci', 'mo_coeff',
         'mo_energy', 'converged',
     }
 
-    def __init__(self, mf_or_mol, ncas, nelecas, ncore=None, frozen=None):
+    def __init__(self, mf_or_mol, ncas=0, nelecas=0, ncore=None, frozen=None):
         casci.CASBase.__init__(self, mf_or_mol, ncas, nelecas, ncore)
         self.frozen = frozen
 
         self.callback = None
         self.chkfile = self._scf.chkfile
 
         self.fcisolver.max_cycle = getattr(__config__,
@@ -1292,14 +1292,16 @@
             mc1 = mc1.state_average_(self.weights, wfnsym)
         return mc1
 
     def reset(self, mol=None):
         casci.CASBase.reset(self, mol=mol)
         self._max_stepsize = None
 
+    to_gpu = lib.to_gpu
+
 scf.hf.RHF.CASSCF = scf.rohf.ROHF.CASSCF = lib.class_as_method(CASSCF)
 scf.uhf.UHF.CASSCF = None
 
 
 # to avoid calculating AO integrals
 def _fake_h_for_fast_casci(casscf, mo, eris):
     mc = casscf.view(CASCI)
```

### Comparing `pyscf-2.5.0/pyscf/mcscf/mc1step_symm.py` & `pyscf-2.6.0/pyscf/mcscf/mc1step_symm.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/mcscf/mc2step.py` & `pyscf-2.6.0/pyscf/mcscf/mc2step.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/mcscf/mc_ao2mo.py` & `pyscf-2.6.0/pyscf/mcscf/mc_ao2mo.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/mcscf/newton_casscf.py` & `pyscf-2.6.0/pyscf/mcscf/newton_casscf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/mcscf/newton_casscf_symm.py` & `pyscf-2.6.0/pyscf/mcscf/newton_casscf_symm.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from pyscf.mcscf import newton_casscf
 from pyscf.mcscf import casci_symm
 from pyscf import fci
 
 
 class CASSCF(newton_casscf.CASSCF):
     __doc__ = newton_casscf.CASSCF.__doc__
-    def __init__(self, mf_or_mol, ncas, nelecas, ncore=None, frozen=None):
+    def __init__(self, mf_or_mol, ncas=0, nelecas=0, ncore=None, frozen=None):
         newton_casscf.CASSCF.__init__(self, mf_or_mol, ncas, nelecas, ncore, frozen)
         assert (self.mol.symmetry)
         self.fcisolver = fci.solver(self.mol, False, True)
         self.fcisolver.max_cycle = 25
         #self.fcisolver.max_space = 25
 
     def kernel(self, mo_coeff=None, ci0=None, callback=None, _kern=None):
```

### Comparing `pyscf-2.5.0/pyscf/mcscf/ucasci.py` & `pyscf-2.6.0/pyscf/mcscf/ucasci.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     t1 = log.timer('FCI solver', *t1)
     e_cas = e_tot - energy_core
     return e_tot, e_cas, fcivec
 
 
 class UCASBase(CASBase):
     # nelecas is tuple of (nelecas_alpha, nelecas_beta)
-    def __init__(self, mf_or_mol, ncas, nelecas, ncore=None):
+    def __init__(self, mf_or_mol, ncas=0, nelecas=0, ncore=None):
         #assert ('UHF' == mf.__class__.__name__)
         if isinstance(mf_or_mol, gto.Mole):
             mf = scf.UHF(mf_or_mol)
         else:
             mf = mf_or_mol
 
         mol = mf.mol
```

### Comparing `pyscf-2.5.0/pyscf/mcscf/umc1step.py` & `pyscf-2.6.0/pyscf/mcscf/umc1step.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,15 +375,15 @@
         'conv_tol_grad', 'ah_level_shift', 'ah_conv_tol', 'ah_max_cycle',
         'ah_lindep', 'ah_start_tol', 'ah_start_cycle', 'ah_grad_trust_region',
         'internal_rotation', 'ci_response_space', 'with_dep4', 'chk_ci',
         'kf_interval', 'kf_trust_region', 'natorb', 'callback',
         'canonicalization', 'sorting_mo_energy',
     }
 
-    def __init__(self, mf_or_mol, ncas, nelecas, ncore=None, frozen=None):
+    def __init__(self, mf_or_mol, ncas=0, nelecas=0, ncore=None, frozen=None):
         ucasci.UCASBase.__init__(self, mf_or_mol, ncas, nelecas, ncore)
         self.frozen = frozen
 
         self.chkfile = self._scf.chkfile
 
         self.fcisolver.max_cycle = getattr(__config__,
                                            'mcscf_umc1step_UCASSCF_fcisolver_max_cycle', 50)
```

### Comparing `pyscf-2.5.0/pyscf/mcscf/umc2step.py` & `pyscf-2.6.0/pyscf/mcscf/umc2step.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/mcscf/umc_ao2mo.py` & `pyscf-2.6.0/pyscf/mcscf/umc_ao2mo.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/md/__init__.py` & `pyscf-2.6.0/pyscf/md/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/md/distributions.py` & `pyscf-2.6.0/pyscf/md/distributions.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/md/integrators.py` & `pyscf-2.6.0/pyscf/md/integrators.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/mp/__init__.py` & `pyscf-2.6.0/pyscf/mp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         return dfmp2.DFMP2(mf, frozen, mo_coeff, mo_occ)
     else:
         return mp2.RMP2(mf, frozen, mo_coeff, mo_occ)
 RMP2.__doc__ = mp2.RMP2.__doc__
 
 def UMP2(mf, frozen=None, mo_coeff=None, mo_occ=None):
     mf = mf.remove_soscf()
-    if mf.istype('UHF'):
+    if not mf.istype('UHF'):
         mf = mf.to_uhf()
 
     if getattr(mf, 'with_df', None):
         #raise NotImplementedError('DF-UMP2')
         return ump2.UMP2(mf, frozen, mo_coeff, mo_occ)
     else:
         return ump2.UMP2(mf, frozen, mo_coeff, mo_occ)
```

### Comparing `pyscf-2.5.0/pyscf/mp/dfgmp2.py` & `pyscf-2.6.0/pyscf/mp/dfgmp2.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,19 +146,19 @@
 
     def ao2mo(self, mo_coeff=None):
         eris = gmp2._PhysicistsERIs()
         # Initialize only the mo_coeff and
         eris._common_init_(self, mo_coeff)
         return eris
 
-    def make_rdm1(self, t2=None, ao_repr=False):
+    def make_rdm1(self, t2=None, ao_repr=False, with_frozen=True):
         if t2 is None:
             t2 = self.t2
         assert t2 is not None
-        return make_rdm1(self, t2, ao_repr=ao_repr)
+        return make_rdm1(self, t2, ao_repr=ao_repr, with_frozen=with_frozen)
 
     def make_rdm2(self, t2=None, ao_repr=False):
         if t2 is None:
             t2 = self.t2
         assert t2 is not None
         return make_rdm2(self, t2, ao_repr=ao_repr)
```

### Comparing `pyscf-2.5.0/pyscf/mp/dfmp2.py` & `pyscf-2.6.0/pyscf/mp/dfmp2.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,19 +114,19 @@
 
     def ao2mo(self, mo_coeff=None):
         eris = mp2._ChemistsERIs()
         # Initialize only the mo_coeff
         eris._common_init_(self, mo_coeff)
         return eris
 
-    def make_rdm1(self, t2=None, ao_repr=False):
+    def make_rdm1(self, t2=None, ao_repr=False, with_frozen=True):
         if t2 is None:
             t2 = self.t2
         assert t2 is not None
-        return make_rdm1(self, t2, ao_repr=ao_repr)
+        return make_rdm1(self, t2, ao_repr=ao_repr, with_frozen=with_frozen)
 
     def make_rdm2(self, t2=None, ao_repr=False):
         if t2 is None:
             t2 = self.t2
         assert t2 is not None
         return make_rdm2(self, t2, ao_repr=ao_repr)
```

### Comparing `pyscf-2.5.0/pyscf/mp/dfmp2_native.py` & `pyscf-2.6.0/pyscf/mp/dfmp2_native.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,14 +232,16 @@
         '''
         self.dump_flags()
         return self.calculate_energy()
 
     def nuc_grad_method(self):
         raise NotImplementedError
 
+    to_gpu = lib.to_gpu
+
 
 MP2 = RMP2 = DFMP2 = DFRMP2
 
 
 class SCSDFRMP2(DFRMP2):
     '''
     RHF-DF-MP2 with spin-component scaling
```

### Comparing `pyscf-2.5.0/pyscf/mp/dfump2_native.py` & `pyscf-2.6.0/pyscf/mp/dfump2_native.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,14 +222,16 @@
         Delete the temporary file(s).
         '''
         self._intsfile = []
 
     def nuc_grad_method(self):
         raise NotImplementedError
 
+    to_gpu = lib.to_gpu
+
 
 MP2 = UMP2 = DFMP2 = DFUMP2
 
 
 class SCSDFUMP2(DFUMP2):
     '''
     UHF-DF-MP2 with spin-component scaling
```

### Comparing `pyscf-2.5.0/pyscf/mp/gmp2.py` & `pyscf-2.6.0/pyscf/mp/gmp2.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     t2new += numpy.asarray(eris.oovv).conj()
 
     eia = mo_e_o[:,None] - mo_e_v
     t2new /= lib.direct_sum('ia,jb->ijab', eia, eia)
     return t2new
 
 
-def make_rdm1(mp, t2=None, ao_repr=False):
+def make_rdm1(mp, t2=None, ao_repr=False, with_frozen=True):
     r'''
     One-particle density matrix in the molecular spin-orbital representation
     (the occupied-virtual blocks from the orbital response contribution are
     not included).
 
     dm1[p,q] = <q^\dagger p>  (p,q are spin-orbitals)
 
@@ -102,15 +102,15 @@
     '''
     from pyscf.cc import gccsd_rdm
     if t2 is None: t2 = mp.t2
     doo, dvv = _gamma1_intermediates(mp, t2)
     nocc, nvir = t2.shape[1:3]
     dov = numpy.zeros((nocc,nvir))
     d1 = doo, dov, dov.T, dvv
-    return gccsd_rdm._make_rdm1(mp, d1, with_frozen=True, ao_repr=ao_repr)
+    return gccsd_rdm._make_rdm1(mp, d1, with_frozen=with_frozen, ao_repr=ao_repr)
 
 def _gamma1_intermediates(mp, t2):
     doo = lib.einsum('imef,jmef->ij', t2.conj(), t2) *-.5
     dvv = lib.einsum('mnea,mneb->ab', t2, t2.conj()) * .5
     return doo, dvv
 
 # spin-orbital rdm2 in Chemist's notation
@@ -210,14 +210,16 @@
 
     # For non-canonical MP2
     energy = energy
     update_amps = update_amps
     def init_amps(self, mo_energy=None, mo_coeff=None, eris=None, with_t2=WITH_T2):
         return kernel(self, mo_energy, mo_coeff, eris, with_t2)
 
+    to_gpu = lib.to_gpu
+
 MP2 = GMP2
 
 scf.ghf.GHF.MP2 = lib.class_as_method(MP2)
 
 
 #TODO: Merge this _PhysicistsERIs class with gccsd._PhysicistsERIs class
 class _PhysicistsERIs:
```

### Comparing `pyscf-2.5.0/pyscf/mp/mp2.py` & `pyscf-2.6.0/pyscf/mp/mp2.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     eris_ovov = None
 
     eia = mo_e_o[:,None] - mo_e_v
     t2new /= lib.direct_sum('ia,jb->ijab', eia, eia)
     return t2new
 
 
-def make_rdm1(mp, t2=None, eris=None, ao_repr=False):
+def make_rdm1(mp, t2=None, eris=None, ao_repr=False, with_frozen=True):
     r'''Spin-traced one-particle density matrix.
     The occupied-virtual orbital response is not included.
 
     dm1[p,q] = <q_alpha^\dagger p_alpha> + <q_beta^\dagger p_beta>
 
     The convention of 1-pdm is based on McWeeney's book, Eq (5.4.20).
     The contraction between 1-particle Hamiltonian and rdm1 is
@@ -165,15 +165,15 @@
     '''
     from pyscf.cc import ccsd_rdm
     doo, dvv = _gamma1_intermediates(mp, t2, eris)
     nocc = doo.shape[0]
     nvir = dvv.shape[0]
     dov = numpy.zeros((nocc,nvir), dtype=doo.dtype)
     dvo = dov.T
-    return ccsd_rdm._make_rdm1(mp, (doo, dov, dvo, dvv), with_frozen=True,
+    return ccsd_rdm._make_rdm1(mp, (doo, dov, dvo, dvv), with_frozen=with_frozen,
                                ao_repr=ao_repr)
 
 def _gamma1_intermediates(mp, t2=None, eris=None):
     if t2 is None: t2 = mp.t2
     nmo = mp.nmo
     nocc = mp.nocc
     nvir = nmo - nocc
@@ -199,14 +199,25 @@
         dm1vir += lib.einsum('jca,jcb->ba', l2i, t2i) * 2 \
                 - lib.einsum('jca,jbc->ba', l2i, t2i)
         dm1occ += lib.einsum('iab,jab->ij', l2i, t2i) * 2 \
                 - lib.einsum('iab,jba->ij', l2i, t2i)
     return -dm1occ, dm1vir
 
 
+def _mo_splitter(mp):
+    maskact = mp.get_frozen_mask()
+    maskocc = mp.mo_occ>1e-6
+    masks = [
+        maskocc  & ~maskact,    # frz occ
+        maskocc  &  maskact,    # act occ
+        ~maskocc &  maskact,    # act vir
+        ~maskocc & ~maskact,    # frz vir
+    ]
+    return masks
+
 def make_fno(mp, thresh=1e-6, pct_occ=None, nvir_act=None, t2=None):
     r'''
     Frozen natural orbitals
 
     Attributes:
         thresh : float
             Threshold on NO occupation numbers. Default is 1e-6 (very conservative).
@@ -218,38 +229,50 @@
     Returns:
         frozen : list or ndarray
             List of orbitals to freeze
         no_coeff : ndarray
             Semicanonical NO coefficients in the AO basis
     '''
     mf = mp._scf
-    dm = mp.make_rdm1(t2=t2)
+    dm = mp.make_rdm1(t2=t2, with_frozen=False)
 
     nmo = mp.nmo
     nocc = mp.nocc
+    nvir = nmo - nocc
     n,v = numpy.linalg.eigh(dm[nocc:,nocc:])
     idx = numpy.argsort(n)[::-1]
     n,v = n[idx], v[:,idx]
 
     if nvir_act is None:
         if pct_occ is None:
-            nvir_act = numpy.count_nonzero(n>thresh)
+            nvir_keep = numpy.count_nonzero(n>thresh)
         else:
-            print(numpy.cumsum(n/numpy.sum(n)))
-            nvir_act = numpy.count_nonzero(numpy.cumsum(n/numpy.sum(n))<pct_occ)
+            cumsum = numpy.cumsum(n/numpy.sum(n))
+            logger.debug(mp, 'Sum(pct_occ): %s', cumsum)
+            nvir_keep = numpy.count_nonzero(cumsum<pct_occ)
+    else:
+        nvir_keep = min(nvir, nvir_act)
 
-    fvv = numpy.diag(mf.mo_energy[nocc:])
+    masks = _mo_splitter(mp)
+    moeoccfrz0, moeocc, moevir, moevirfrz0 = [mf.mo_energy[m] for m in masks]
+    orboccfrz0, orbocc, orbvir, orbvirfrz0 = [mf.mo_coeff[:,m] for m in masks]
+
+    fvv = numpy.diag(moevir)
     fvv_no = numpy.dot(v.T, numpy.dot(fvv, v))
-    _, v_canon = numpy.linalg.eigh(fvv_no[:nvir_act,:nvir_act])
+    _, v_canon = numpy.linalg.eigh(fvv_no[:nvir_keep,:nvir_keep])
 
-    no_coeff_1 = numpy.dot(mf.mo_coeff[:,nocc:], numpy.dot(v[:,:nvir_act], v_canon))
-    no_coeff_2 = numpy.dot(mf.mo_coeff[:,nocc:], v[:,nvir_act:])
-    no_coeff = numpy.concatenate((mf.mo_coeff[:,:nocc], no_coeff_1, no_coeff_2), axis=1)
+    orbviract = numpy.dot(orbvir, numpy.dot(v[:,:nvir_keep], v_canon))
+    orbvirfrz = numpy.dot(orbvir, v[:,nvir_keep:])
+    no_comp = (orboccfrz0, orbocc, orbviract, orbvirfrz, orbvirfrz0)
+    no_coeff = numpy.hstack(no_comp)
+    nocc_loc = numpy.cumsum([0]+[x.shape[1] for x in no_comp]).astype(int)
+    no_frozen = numpy.hstack((numpy.arange(nocc_loc[0], nocc_loc[1]),
+                              numpy.arange(nocc_loc[3], nocc_loc[5]))).astype(int)
 
-    return numpy.arange(nocc+nvir_act,nmo), no_coeff
+    return no_frozen, no_coeff
 
 
 def make_rdm2(mp, t2=None, eris=None, ao_repr=False):
     r'''
     Spin-traced two-particle density matrix in MO basis
 
     dm2[p,q,r,s] = \sum_{sigma,tau} <p_sigma^\dagger r_tau^\dagger s_tau q_sigma>
@@ -645,14 +668,23 @@
 
     # For non-canonical MP2
     energy = energy
     update_amps = update_amps
     def init_amps(self, mo_energy=None, mo_coeff=None, eris=None, with_t2=WITH_T2):
         return kernel(self, mo_energy, mo_coeff, eris, with_t2)
 
+    # to_gpu can be reused only when __init__ still takes mf
+    def to_gpu(self):
+        mf = self._scf.to_gpu()
+        from importlib import import_module
+        mod = import_module(self.__module__.replace('pyscf', 'gpu4pyscf'))
+        cls = getattr(mod, self.__class__.__name__)
+        obj = cls(mf)
+        return obj
+
 RMP2 = MP2
 
 from pyscf import scf
 scf.hf.RHF.MP2 = lib.class_as_method(MP2)
 scf.rohf.ROHF.MP2 = None
```

### Comparing `pyscf-2.5.0/pyscf/mp/mp2f12_slow.py` & `pyscf-2.6.0/pyscf/mp/mp2f12_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/mp/ump2.py` & `pyscf-2.6.0/pyscf/mp/ump2.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,15 +236,15 @@
             frozen = (frozen, frozen)
         moidxa[list(frozen[0])] = False
         moidxb[list(frozen[1])] = False
     else:
         raise NotImplementedError
     return moidxa,moidxb
 
-def make_rdm1(mp, t2=None, ao_repr=False):
+def make_rdm1(mp, t2=None, ao_repr=False, with_frozen=True):
     r'''
     One-particle spin density matrices dm1a, dm1b in MO basis (the
     occupied-virtual blocks due to the orbital response contribution are not
     included).
 
     dm1a[p,q] = <q_alpha^\dagger p_alpha>
     dm1b[p,q] = <q_beta^\dagger p_beta>
@@ -254,15 +254,15 @@
     from pyscf.cc import uccsd_rdm
     if t2 is None: t2 = mp.t2
     doo, dvv = _gamma1_intermediates(mp, t2)
     nocca, noccb, nvira, nvirb = t2[1].shape
     dov = numpy.zeros((nocca,nvira))
     dOV = numpy.zeros((noccb,nvirb))
     d1 = (doo, (dov, dOV), (dov.T, dOV.T), dvv)
-    return uccsd_rdm._make_rdm1(mp, d1, with_frozen=True, ao_repr=ao_repr)
+    return uccsd_rdm._make_rdm1(mp, d1, with_frozen=with_frozen, ao_repr=ao_repr)
 
 def _gamma1_intermediates(mp, t2):
     t2aa, t2ab, t2bb = t2
     dooa  = lib.einsum('imef,jmef->ij', t2aa.conj(), t2aa) *-.5
     dooa -= lib.einsum('imef,jmef->ij', t2ab.conj(), t2ab)
     doob  = lib.einsum('imef,jmef->ij', t2bb.conj(), t2bb) *-.5
     doob -= lib.einsum('mief,mjef->ij', t2ab.conj(), t2ab)
@@ -270,54 +270,83 @@
     dvva  = lib.einsum('mnae,mnbe->ba', t2aa.conj(), t2aa) * .5
     dvva += lib.einsum('mnae,mnbe->ba', t2ab.conj(), t2ab)
     dvvb  = lib.einsum('mnae,mnbe->ba', t2bb.conj(), t2bb) * .5
     dvvb += lib.einsum('mnea,mneb->ba', t2ab.conj(), t2ab)
     return ((dooa, doob), (dvva, dvvb))
 
 
-def make_fno(mp, thresh=1e-6, pct_occ=None, t2=None, eris=None):
+def _mo_splitter(mp):
+    maskact = mp.get_frozen_mask()
+    maskocc = [mp.mo_occ[s]>1e-6 for s in [0,1]]
+    masks = []
+    for s in [0,1]:
+        masks.append([
+            maskocc[s]  & ~maskact[s],  # frz occ
+            maskocc[s]  &  maskact[s],  # act occ
+            ~maskocc[s] &  maskact[s],  # act vir
+            ~maskocc[s] & ~maskact[s],  # frz vir
+        ])
+    return masks
+
+def make_fno(mp, thresh=1e-6, pct_occ=None, nvir_act=None, t2=None, eris=None):
     r'''
     Frozen natural orbitals
 
     Returns:
         frozen : list or ndarray
             Length-2 list of orbitals to freeze
         no_coeff : ndarray
             Length-2 list of semicanonical NO coefficients in the AO basis
     '''
     mf = mp._scf
-    dmab = mp.make_rdm1(t2=t2)
+    dmab = mp.make_rdm1(t2=t2, with_frozen=False)
+
+    masks = _mo_splitter(mp)
+
+    if nvir_act is not None:
+        if isinstance(nvir_act, (int,numpy.int)):
+            nvir_act = [nvir_act]*2
 
-    frozen = []
+    no_frozen = []
     no_coeff = []
     for s,dm in enumerate(dmab):
         nocc = mp.nocc[s]
         nmo = mp.nmo[s]
+        nvir = nmo - nocc
         n,v = numpy.linalg.eigh(dm[nocc:,nocc:])
         idx = numpy.argsort(n)[::-1]
         n,v = n[idx], v[:,idx]
+        n *= 2  # to match RHF when using same thresh
 
-        if pct_occ is None:
-            nvir_act = numpy.count_nonzero(n>thresh)
+        if nvir_act is None:
+            if pct_occ is None:
+                nvir_keep = numpy.count_nonzero(n>thresh)
+            else:
+                cumsum = numpy.cumsum(n/numpy.sum(n))
+                logger.debug(mp, 'Sum(pct_occ): %s', cumsum)
+                nvir_keep = numpy.count_nonzero(cumsum<pct_occ)
         else:
-            print(numpy.cumsum(n/numpy.sum(n)))
-            nvir_act = numpy.count_nonzero(numpy.cumsum(n/numpy.sum(n))<pct_occ)
+            nvir_keep = min(nvir, nvir_act[s])
 
-        fvv = numpy.diag(mf.mo_energy[s][nocc:])
-        fvv_no = numpy.dot(v.T, numpy.dot(fvv, v))
-        _, v_canon = numpy.linalg.eigh(fvv_no[:nvir_act,:nvir_act])
+        moeoccfrz0, moeocc, moevir, moevirfrz0 = [mf.mo_energy[s][m] for m in masks[s]]
+        orboccfrz0, orbocc, orbvir, orbvirfrz0 = [mf.mo_coeff[s][:,m] for m in masks[s]]
 
-        no_coeff_1 = numpy.dot(mf.mo_coeff[s][:,nocc:], numpy.dot(v[:,:nvir_act], v_canon))
-        no_coeff_2 = numpy.dot(mf.mo_coeff[s][:,nocc:], v[:,nvir_act:])
-        no_coeff_s = numpy.concatenate((mf.mo_coeff[s][:,:nocc], no_coeff_1, no_coeff_2), axis=1)
+        fvv = numpy.diag(moevir)
+        fvv_no = numpy.dot(v.T, numpy.dot(fvv, v))
+        _, v_canon = numpy.linalg.eigh(fvv_no[:nvir_keep,:nvir_keep])
 
-        frozen.append(numpy.arange(nocc+nvir_act,nmo))
-        no_coeff.append(no_coeff_s)
+        orbviract = numpy.dot(orbvir, numpy.dot(v[:,:nvir_keep], v_canon))
+        orbvirfrz = numpy.dot(orbvir, v[:,nvir_keep:])
+        no_comp = (orboccfrz0, orbocc, orbviract, orbvirfrz, orbvirfrz0)
+        no_coeff.append(numpy.hstack(no_comp))
+        nocc_loc = numpy.cumsum([0]+[x.shape[1] for x in no_comp]).astype(int)
+        no_frozen.append(numpy.hstack((numpy.arange(nocc_loc[0], nocc_loc[1]),
+                                       numpy.arange(nocc_loc[3], nocc_loc[5]))).astype(int))
 
-    return frozen, no_coeff
+    return no_frozen, no_coeff
 
 
 # spin-orbital rdm2 in Chemist's notation
 def make_rdm2(mp, t2=None, ao_repr=False):
     r'''
     Two-particle spin density matrices dm2aa, dm2ab, dm2bb in MO basis
 
@@ -446,14 +475,16 @@
 
     # For non-canonical MP2
     energy = energy
     update_amps = update_amps
     def init_amps(self, mo_energy=None, mo_coeff=None, eris=None, with_t2=WITH_T2):
         return kernel(self, mo_energy, mo_coeff, eris, with_t2)
 
+    to_gpu = lib.to_gpu
+
 MP2 = UMP2
 
 from pyscf import scf
 scf.uhf.UHF.MP2 = lib.class_as_method(MP2)
 
 
 #TODO: Merge this _ChemistsERIs class with uccsd._ChemistsERIs class
```

### Comparing `pyscf-2.5.0/pyscf/mrpt/__init__.py` & `pyscf-2.6.0/pyscf/mrpt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/mrpt/nevpt2.py` & `pyscf-2.6.0/pyscf/mrpt/nevpt2.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/nac/__init__.py` & `pyscf-2.6.0/pyscf/nac/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/nac/sacasscf.py` & `pyscf-2.6.0/pyscf/nac/sacasscf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/__init__.py` & `pyscf-2.6.0/pyscf/pbc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/adc/__init__.py` & `pyscf-2.6.0/pyscf/pbc/adc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/adc/dfadc.py` & `pyscf-2.6.0/pyscf/pbc/adc/dfadc.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/adc/kadc_ao2mo.py` & `pyscf-2.6.0/pyscf/pbc/adc/kadc_ao2mo.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/adc/kadc_rhf.py` & `pyscf-2.6.0/pyscf/pbc/adc/kadc_rhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/adc/kadc_rhf_amplitudes.py` & `pyscf-2.6.0/pyscf/pbc/adc/kadc_rhf_amplitudes.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/adc/kadc_rhf_ea.py` & `pyscf-2.6.0/pyscf/pbc/adc/kadc_rhf_ea.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/adc/kadc_rhf_ip.py` & `pyscf-2.6.0/pyscf/pbc/adc/kadc_rhf_ip.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/ao2mo/__init__.py` & `pyscf-2.6.0/pyscf/pbc/ao2mo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/ao2mo/eris.py` & `pyscf-2.6.0/pyscf/pbc/ao2mo/eris.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/__init__.py` & `pyscf-2.6.0/pyscf/pbc/cc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/ccsd.py` & `pyscf-2.6.0/pyscf/pbc/cc/ccsd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/eom_kccsd_ghf.py` & `pyscf-2.6.0/pyscf/pbc/cc/eom_kccsd_ghf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/eom_kccsd_rhf.py` & `pyscf-2.6.0/pyscf/pbc/cc/eom_kccsd_rhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/eom_kccsd_rhf_ea.py` & `pyscf-2.6.0/pyscf/pbc/cc/eom_kccsd_rhf_ea.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/eom_kccsd_rhf_ip.py` & `pyscf-2.6.0/pyscf/pbc/cc/eom_kccsd_rhf_ip.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/eom_kccsd_uhf.py` & `pyscf-2.6.0/pyscf/pbc/cc/eom_kccsd_uhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/kccsd.py` & `pyscf-2.6.0/pyscf/pbc/cc/kccsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,14 +459,16 @@
 
     def from_uccsd(self, t1, t2, orbspin=None):
         return self.spatial2spin(t1, orbspin), self.spatial2spin(t2, orbspin)
 
     def to_uccsd(self, t1, t2, orbspin=None):
         return spin2spatial(t1, orbspin), spin2spatial(t2, orbspin)
 
+    to_gpu = lib.to_gpu
+
 CCSD = KCCSD = KGCCSD = GCCSD
 
 
 def _make_eris_incore(cc, mo_coeff=None):
     from pyscf.pbc import tools
     from pyscf.pbc.cc.ccsd import _adjust_occ
```

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/kccsd_rhf.py` & `pyscf-2.6.0/pyscf/pbc/cc/kccsd_rhf.py`

 * *Files 0% similar despite different names*

```diff
@@ -649,14 +649,16 @@
                                                 koopmans=koopmans, guess=guess,
                                                 partition=partition, eris=eris,
                                                 kptlist=kptlist)
 
     def ao2mo(self, mo_coeff=None):
         return _ERIS(self, mo_coeff)
 
+    to_gpu = lib.to_gpu
+
 #####################################
 # Wrapper functions for IP/EA-EOM
 #####################################
 # TODO: ip/ea _matvec and _diag functions are not needed in pyscf-1.7 or
 # higher. Remove these wrapper functions in future release
     def ipccsd_matvec(self, vector, kshift):
         from pyscf.pbc.cc import eom_kccsd_rhf
```

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/kccsd_rhf_ksymm.py` & `pyscf-2.6.0/pyscf/pbc/cc/kccsd_rhf_ksymm.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/kccsd_t.py` & `pyscf-2.6.0/pyscf/pbc/cc/kccsd_t.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/kccsd_t_rhf.py` & `pyscf-2.6.0/pyscf/pbc/cc/kccsd_t_rhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/kccsd_t_rhf_slow.py` & `pyscf-2.6.0/pyscf/pbc/cc/kccsd_t_rhf_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/kccsd_uhf.py` & `pyscf-2.6.0/pyscf/pbc/cc/kccsd_uhf.py`

 * *Files 0% similar despite different names*

```diff
@@ -757,14 +757,16 @@
 
     def vector_to_amplitudes(self, vec, nmo=None, nocc=None, nkpts=None):
         if nocc is None: nocc = self.nocc
         if nmo is None: nmo = self.nmo
         if nkpts is None: nkpts = self.nkpts
         return vector_to_amplitudes(vec, nmo, nocc, nkpts)
 
+    to_gpu = lib.to_gpu
+
 UCCSD = KUCCSD
 
 
 #######################################
 #
 # _ERIS.
 #
```

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/kintermediates.py` & `pyscf-2.6.0/pyscf/pbc/cc/kintermediates.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/kintermediates_rhf.py` & `pyscf-2.6.0/pyscf/pbc/cc/kintermediates_rhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/kintermediates_rhf_ksymm.py` & `pyscf-2.6.0/pyscf/pbc/cc/kintermediates_rhf_ksymm.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/kintermediates_uhf.py` & `pyscf-2.6.0/pyscf/pbc/cc/kintermediates_uhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/cc/kuccsd_rdm.py` & `pyscf-2.6.0/pyscf/pbc/cc/kuccsd_rdm.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/ci/__init__.py` & `pyscf-2.6.0/pyscf/pbc/ci/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/ci/cisd.py` & `pyscf-2.6.0/pyscf/pbc/ci/cisd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/ci/kcis_rhf.py` & `pyscf-2.6.0/pyscf/pbc/ci/kcis_rhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/df/__init__.py` & `pyscf-2.6.0/pyscf/pbc/df/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/df/aft.py` & `pyscf-2.6.0/pyscf/pbc/df/aft.py`

 * *Files 1% similar despite different names*

```diff
@@ -534,15 +534,15 @@
         '''
         key = '%.6f' % omega
         if key in self._rsh_df:
             rsh_df = self._rsh_df[key]
         else:
             rsh_df = self._rsh_df[key] = self.copy().reset()
             if hasattr(self, '_dataname'):
-                rsh_df._dataname = f'{self._dataname}/lr/{key}'
+                rsh_df._dataname = f'{self._dataname}-lr/{key}'
             logger.info(self, 'Create RSH-DF object %s for omega=%s', rsh_df, omega)
 
         cell = self.cell
         auxcell = getattr(self, 'auxcell', None)
 
         cell_omega = cell.omega
         cell.omega = omega
```

### Comparing `pyscf-2.5.0/pyscf/pbc/df/aft_ao2mo.py` & `pyscf-2.6.0/pyscf/pbc/df/aft_ao2mo.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/df/aft_jk.py` & `pyscf-2.6.0/pyscf/pbc/df/aft_jk.py`

 * *Files 0% similar despite different names*

```diff
@@ -728,15 +728,15 @@
                 else:
                     zdotNN(pLqR, pLqI, dmsR[i], dmsI[i], 1,
                            iLkR.reshape(-1,nao), iLkI.reshape(-1,nao))
                     iLkR *= vkcoulG[p0:p1].reshape(1,nG,1)
                     iLkI *= vkcoulG[p0:p1].reshape(1,nG,1)
                     zdotNC(iLkR.reshape(nao,-1), iLkI.reshape(nao,-1),
                            pLqR.reshape(nao,-1).T, pLqI.reshape(nao,-1).T,
-                           1, vkR[i], vkI[i])
+                           1, vkR[i], vkI[i], 1)
             #t2 = log.timer_debug1('        with_k', *t2)
         pqkR = pqkI = pLqR = pLqI = iLkR = iLkI = None
         #t2 = log.timer_debug1('%d:%d'%(p0,p1), *t2)
     t1 = log.timer_debug1('aft_jk.get_jk', *t1)
 
     if with_j:
         if j_real:
```

### Comparing `pyscf-2.5.0/pyscf/pbc/df/df.py` & `pyscf-2.6.0/pyscf/pbc/df/df.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 from pyscf.pbc.df import outcore
 from pyscf.pbc.df import ft_ao
 from pyscf.pbc.df import aft
 from pyscf.pbc.df import df_jk
 from pyscf.pbc.df import df_ao2mo
 from pyscf.pbc.df.aft import estimate_eta, _check_kpts
 from pyscf.pbc.df.df_jk import zdotCN
+from pyscf.pbc.lib.kpts import KPoints
 from pyscf.pbc.lib.kpts_helper import (is_zero, gamma_point, member, unique,
                                        KPT_DIFF_TOL)
 from pyscf.pbc.df.gdf_builder import libpbc, _CCGDFBuilder, _CCNucBuilder
 from pyscf.pbc.df.rsdf_builder import _RSGDFBuilder, _RSNucBuilder
 from pyscf import __config__
 
 LINEAR_DEP_THR = getattr(__config__, 'pbc_df_df_DF_lindep', 1e-9)
@@ -142,14 +143,16 @@
 
     def __init__(self, cell, kpts=numpy.zeros((1,3))):
         self.cell = cell
         self.stdout = cell.stdout
         self.verbose = cell.verbose
         self.max_memory = cell.max_memory
 
+        if isinstance(kpts, KPoints):
+            kpts = kpts.kpts
         self.kpts = kpts  # default is gamma point
         self.kpts_band = None
         self._auxbasis = None
 
         self.eta = None
         self.mesh = None
 
@@ -520,14 +523,16 @@
                 dat = feri[f'{self._dataname}-/{key}']
                 if isinstance(dat, h5py.Group):
                     naux += dat['0'].shape[0]
                 else:
                     naux += dat.shape[0]
         return naux
 
+    to_gpu = lib.to_gpu
+
 DF = GDF
 
 class CDERIArray:
     '''
     Provide numpy APIs to access cderi tensor. This object can be viewed as an
     5-dimension array [kpt-i, kpt-j, aux-index, ao-i, ao-j]
     '''
```

### Comparing `pyscf-2.5.0/pyscf/pbc/df/df_ao2mo.py` & `pyscf-2.6.0/pyscf/pbc/df/df_ao2mo.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/df/df_jk.py` & `pyscf-2.6.0/pyscf/pbc/df/df_jk.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 
 from functools import reduce
 import numpy
 from pyscf import lib
 from pyscf.lib import logger, zdotNN, zdotCN, zdotNC
 from pyscf.pbc import tools
-from pyscf.pbc.lib.kpts import KPoints
 from pyscf.pbc.lib.kpts_helper import is_zero, gamma_point, member, get_kconserv_ria
 from pyscf import __config__
 
 DM2MO_PREC = getattr(__config__, 'pbc_gto_df_df_jk_dm2mo_prec', 1e-10)
 
 def density_fit(mf, auxbasis=None, mesh=None, with_df=None):
     '''Generte density-fitting SCF object
@@ -49,16 +48,14 @@
     from pyscf.pbc.df import df
     if with_df is None:
         if getattr(mf, 'kpts', None) is not None:
             kpts = mf.kpts
         else:
             kpts = numpy.reshape(mf.kpt, (1,3))
 
-        if isinstance(kpts, KPoints):
-            kpts = kpts.kpts
         with_df = df.DF(mf.cell, kpts)
         with_df.max_memory = mf.max_memory
         with_df.stdout = mf.stdout
         with_df.verbose = mf.verbose
         with_df.auxbasis = auxbasis
         if mesh is not None:
             with_df.mesh = mesh
@@ -1260,20 +1257,20 @@
     for LpqR, LpqI, sign in mydf.sr_loop(kptii, max_memory, False):
         LpqR = LpqR.reshape(-1,nao,nao)
         tock = numpy.asarray((logger.process_clock(), logger.perf_counter()))
         tspans[0] += tock - tick
         if with_j:
             #:rho_coeff = numpy.einsum('Lpq,xqp->xL', Lpq, dms)
             #:vj += numpy.dot(rho_coeff, Lpq.reshape(-1,nao**2))
-            rhoR  = numpy.einsum('Lpq,xpq->xL', LpqR, dmsR)
+            rhoR  = numpy.einsum('Lpq,xqp->xL', LpqR, dmsR)
             if not j_real:
                 LpqI = LpqI.reshape(-1,nao,nao)
-                rhoR -= numpy.einsum('Lpq,xpq->xL', LpqI, dmsI)
-                rhoI  = numpy.einsum('Lpq,xpq->xL', LpqR, dmsI)
-                rhoI += numpy.einsum('Lpq,xpq->xL', LpqI, dmsR)
+                rhoR -= numpy.einsum('Lpq,xqp->xL', LpqI, dmsI)
+                rhoI  = numpy.einsum('Lpq,xqp->xL', LpqR, dmsI)
+                rhoI += numpy.einsum('Lpq,xqp->xL', LpqI, dmsR)
             vjR += sign * numpy.einsum('xL,Lpq->xpq', rhoR, LpqR)
             if not j_real:
                 vjR -= sign * numpy.einsum('xL,Lpq->xpq', rhoI, LpqI)
                 vjI += sign * numpy.einsum('xL,Lpq->xpq', rhoR, LpqI)
                 vjI += sign * numpy.einsum('xL,Lpq->xpq', rhoI, LpqR)
 
         tick = numpy.asarray((logger.process_clock(), logger.perf_counter()))
```

### Comparing `pyscf-2.5.0/pyscf/pbc/df/fft.py` & `pyscf-2.6.0/pyscf/pbc/df/fft.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from pyscf.pbc import gto as pbcgto
 from pyscf.pbc.gto import pseudo, error_for_ke_cutoff, estimate_ke_cutoff
 from pyscf.pbc.df import ft_ao
 from pyscf.pbc.df import fft_ao2mo
 from pyscf.pbc.df import fft_jk
 from pyscf.pbc.df import aft
 from pyscf.pbc.df.aft import _check_kpts
+from pyscf.pbc.lib.kpts import KPoints
 from pyscf.pbc.lib.kpts_helper import is_zero
 from pyscf import __config__
 
 KE_SCALING = getattr(__config__, 'pbc_df_aft_ke_cutoff_scaling', 0.75)
 
 
 def get_nuc(mydf, kpts=None):
@@ -164,14 +165,16 @@
         from pyscf.pbc.dft import gen_grid
         from pyscf.pbc.dft import numint
         self.cell = cell
         self.stdout = cell.stdout
         self.verbose = cell.verbose
         self.max_memory = cell.max_memory
 
+        if isinstance(kpts, KPoints):
+            kpts = kpts.kpts
         self.kpts = kpts
 
         self.grids = gen_grid.UniformGrids(cell)
         # FFT from real space density distributes error to every rho_ij(G) than
         # the one with largest Gaussian exponent. Therefore the error for FFT-ERI
         # ~ Nele * error[rho(Ecut)] while in AFT the error is ~ error[rho(Ecut)]^2.
         # This is a first order error, same to the error estimation for nuclear
@@ -351,7 +354,9 @@
 
     def get_naoaux(self):
         mesh = numpy.asarray(self.mesh)
         ngrids = numpy.prod(mesh)
         return ngrids * 2
 
     range_coulomb = aft.AFTDF.range_coulomb
+
+    to_gpu = lib.to_gpu
```

### Comparing `pyscf-2.5.0/pyscf/pbc/df/fft_ao2mo.py` & `pyscf-2.6.0/pyscf/pbc/df/fft_ao2mo.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/df/fft_jk.py` & `pyscf-2.6.0/pyscf/pbc/df/fft_jk.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/df/ft_ao.py` & `pyscf-2.6.0/pyscf/pbc/df/ft_ao.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/df/gdf_builder.py` & `pyscf-2.6.0/pyscf/pbc/df/gdf_builder.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/df/mdf.py` & `pyscf-2.6.0/pyscf/pbc/df/mdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from pyscf.pbc.df import ft_ao
 from pyscf.pbc.df import df
 from pyscf.pbc.df import aft
 from pyscf.pbc.df.aft import _check_kpts
 from pyscf.pbc.df.gdf_builder import _CCGDFBuilder
 from pyscf.pbc.df.rsdf_builder import _RSGDFBuilder
 from pyscf.pbc.df.incore import libpbc, make_auxcell
+from pyscf.pbc.lib.kpts import KPoints
 from pyscf.pbc.lib.kpts_helper import is_zero, member, unique
 from pyscf.pbc.df import mdf_jk
 from pyscf.pbc.df import mdf_ao2mo
 from pyscf.pbc.df.aft import _sub_df_jk_
 from pyscf import __config__
 
 
@@ -51,14 +52,16 @@
 
     def __init__(self, cell, kpts=np.zeros((1,3))):
         self.cell = cell
         self.stdout = cell.stdout
         self.verbose = cell.verbose
         self.max_memory = cell.max_memory
 
+        if isinstance(kpts, KPoints):
+            kpts = kpts.kpts
         self.kpts = kpts  # default is gamma point
         self.kpts_band = None
         self._auxbasis = None
 
         # In MDF, fitting PWs (self.mesh), and parameters eta and exp_to_discard
         # are related to each other. The compensated function does not need to
         # be very smooth. It just needs to be expanded by the specified PWs
```

### Comparing `pyscf-2.5.0/pyscf/pbc/df/mdf_ao2mo.py` & `pyscf-2.6.0/pyscf/pbc/df/mdf_ao2mo.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/df/mdf_jk.py` & `pyscf-2.6.0/pyscf/pbc/df/mdf_jk.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 J. Chem. Phys. 147, 164119 (2017)
 '''
 
 import numpy
 from pyscf.lib import logger
 from pyscf.pbc.df import df_jk
 from pyscf.pbc.df import aft_jk
-from pyscf.pbc.lib.kpts import KPoints
 
 #
 # Divide the Coulomb potential to two parts.  Computing short range part in
 # real space, long range part in reciprocal space.
 #
 
 def density_fit(mf, auxbasis=None, mesh=None, with_df=None):
@@ -48,16 +47,14 @@
     from pyscf.pbc.df import mdf
     if with_df is None:
         if getattr(mf, 'kpts', None) is not None:
             kpts = mf.kpts
         else:
             kpts = numpy.reshape(mf.kpt, (1,3))
 
-        if isinstance(kpts, KPoints):
-            kpts = kpts.kpts
         with_df = mdf.MDF(mf.cell, kpts)
         with_df.max_memory = mf.max_memory
         with_df.stdout = mf.stdout
         with_df.verbose = mf.verbose
         with_df.auxbasis = auxbasis
         if mesh is not None:
             with_df.mesh = mesh
```

### Comparing `pyscf-2.5.0/pyscf/pbc/df/outcore.py` & `pyscf-2.6.0/pyscf/pbc/df/outcore.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/df/rsdf.py` & `pyscf-2.6.0/pyscf/pbc/df/rsdf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/df/rsdf_builder.py` & `pyscf-2.6.0/pyscf/pbc/df/rsdf_builder.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/df/rsdf_helper.py` & `pyscf-2.6.0/pyscf/pbc/df/rsdf_helper.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/df/rsdf_jk.py` & `pyscf-2.6.0/pyscf/pbc/df/rsdf_jk.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/__init__.py` & `pyscf-2.6.0/pyscf/pbc/dft/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/cdft.py` & `pyscf-2.6.0/pyscf/pbc/dft/cdft.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/gen_grid.py` & `pyscf-2.6.0/pyscf/pbc/dft/gen_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,16 @@
     @lib.with_doc(make_mask.__doc__)
     def make_mask(self, cell=None, coords=None, relativity=0, shls_slice=None,
                   verbose=None):
         if cell is None: cell = self.cell
         if coords is None: coords = self.coords
         return make_mask(cell, coords, relativity, shls_slice, verbose)
 
+    to_gpu = lib.to_gpu
+
 
 # modified from pyscf.dft.gen_grid.gen_partition
 def get_becke_grids(cell, atom_grid={}, radi_method=dft.radi.gauss_chebyshev,
                     level=3, prune=nwchem_prune):
     '''real-space grids using Becke scheme
 
     Args:
@@ -253,14 +255,16 @@
     @lib.with_doc(make_mask.__doc__)
     def make_mask(self, cell=None, coords=None, relativity=0, shls_slice=None,
                   verbose=None):
         if cell is None: cell = self.cell
         if coords is None: coords = self.coords
         return make_mask(cell, coords, relativity, shls_slice, verbose)
 
+    to_gpu = lib.to_gpu
+
 AtomicGrids = BeckeGrids
 
 
 if __name__ == '__main__':
     import pyscf.pbc.gto as pgto
 
     n = 7
```

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/gks.py` & `pyscf-2.6.0/pyscf/pbc/dft/gks.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     '''Coulomb + XC functional for GKS.'''
     if cell is None: cell = ks.cell
     if dm is None: dm = ks.make_rdm1()
     if kpt is None: kpt = ks.kpt
     t0 = (logger.process_clock(), logger.perf_counter())
 
     ni = ks._numint
-    if ks.nlc or ni.libxc.is_nlc(ks.xc):
+    if ks.do_nlc():
         raise NotImplementedError(f'NLC functional {ks.xc} + {ks.nlc}')
 
     hybrid = ni.libxc.is_hybrid_xc(ks.xc)
 
     # TODO GKS with hybrid functional
     if hybrid:
         raise NotImplementedError
@@ -73,15 +73,15 @@
     ground_state = (dm.ndim == 2 and kpts_band is None)
 
     # vxc = (vxc_aa, vxc_bb). vxc_ab is neglected in collinear DFT.
     max_memory = ks.max_memory - lib.current_memory()[0]
     ni = ks._numint
     n, exc, vxc = ni.get_vxc(cell, ks.grids, ks.xc, dm, hermi=hermi, kpt=kpt,
                              kpts_band=kpts_band, max_memory=max_memory)
-    logger.debug(ks, 'nelec by numeric integration = %s', n)
+    logger.info(ks, 'nelec by numeric integration = %s', n)
     t0 = logger.timer(ks, 'vxc', *t0)
 
     if not hybrid:
         vj = ks.get_j(cell, dm, hermi, kpt, kpts_band)
         vxc += vj
     else:
         omega, alpha, hyb = ks._numint.rsh_and_hybrid_coeff(ks.xc, spin=cell.spin)
@@ -139,7 +139,9 @@
     def nuc_grad_method(self):
         raise NotImplementedError
 
     def to_hf(self):
         '''Convert to GHF object.'''
         from pyscf.pbc import scf
         return self._transfer_attrs_(scf.GHF(self.cell, self.kpt))
+
+    to_gpu = lib.to_gpu
```

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/kgks.py` & `pyscf-2.6.0/pyscf/pbc/dft/kgks.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     '''
     if cell is None: cell = ks.cell
     if dm is None: dm = ks.make_rdm1()
     if kpts is None: kpts = ks.kpts
     t0 = (logger.process_clock(), logger.perf_counter())
 
     ni = ks._numint
-    if ks.nlc or ni.libxc.is_nlc(ks.xc):
+    if ks.do_nlc():
         raise NotImplementedError(f'NLC functional {ks.xc} + {ks.nlc}')
 
     hybrid = ni.libxc.is_hybrid_xc(ks.xc)
 
     # TODO GKS with hybrid functional
     hybrid = ks._numint.libxc.is_hybrid_xc(ks.xc)
     if hybrid:
@@ -80,15 +80,15 @@
     # TODO: support non-symmetric density matrix
     assert (hermi == 1)
 
     max_memory = ks.max_memory - lib.current_memory()[0]
     ni = ks._numint
     n, exc, vxc = ni.get_vxc(cell, ks.grids, ks.xc, dm, hermi=hermi, kpts=kpts,
                              kpts_band=kpts_band, max_memory=max_memory)
-    logger.debug(ks, 'nelec by numeric integration = %s', n)
+    logger.info(ks, 'nelec by numeric integration = %s', n)
     t0 = logger.timer(ks, 'vxc', *t0)
 
     nkpts = len(kpts)
     weight = 1. / nkpts
     if not hybrid:
         vj = ks.get_j(cell, dm, hermi, kpts, kpts_band)
         vxc += vj
@@ -142,9 +142,18 @@
         raise NotImplementedError
 
     def nuc_grad_method(self):
         raise NotImplementedError
 
     def to_hf(self):
         '''Convert to KGHF object.'''
-        from pyscf.pbc import scf
-        return self._transfer_attrs_(scf.KGHF(self.cell, self.kpts))
+        from pyscf.pbc import scf, df
+        out = self._transfer_attrs_(scf.KGHF(self.cell, self.kpts))
+
+        # Pure functionals only construct J-type integrals. Enable all integrals for KHF.
+        if (not self._numint.libxc.is_hybrid_xc(self.xc) and
+            len(self.kpts) > 1 and getattr(self.with_df, '_j_only', False)):
+            out.with_df._j_only = False
+            out.with_df.reset()
+        return out
+
+    to_gpu = lib.to_gpu
```

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/krks.py` & `pyscf-2.6.0/pyscf/pbc/dft/krks.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,46 +60,46 @@
     if kpts is None: kpts = ks.kpts
     t0 = (logger.process_clock(), logger.perf_counter())
 
     ni = ks._numint
     hybrid = ni.libxc.is_hybrid_xc(ks.xc)
 
     if not hybrid and isinstance(ks.with_df, multigrid.MultiGridFFTDF):
-        if ks.nlc or ni.libxc.is_nlc(ks.xc):
+        if ks.do_nlc():
             raise NotImplementedError(f'MultiGrid for NLC functional {ks.xc} + {ks.nlc}')
         n, exc, vxc = multigrid.nr_rks(ks.with_df, ks.xc, dm, hermi,
                                        kpts, kpts_band,
                                        with_j=True, return_j=False)
-        logger.debug(ks, 'nelec by numeric integration = %s', n)
+        logger.info(ks, 'nelec by numeric integration = %s', n)
         t0 = logger.timer(ks, 'vxc', *t0)
         return vxc
 
     # ndim = 3 : dm.shape = (nkpts, nao, nao)
     ground_state = (isinstance(dm, np.ndarray) and dm.ndim == 3 and
                     kpts_band is None)
     ks.initialize_grids(cell, dm, kpts, ground_state)
 
     if hermi == 2:  # because rho = 0
         n, exc, vxc = 0, 0, 0
     else:
         max_memory = ks.max_memory - lib.current_memory()[0]
         n, exc, vxc = ni.nr_rks(cell, ks.grids, ks.xc, dm, 0, hermi,
                                 kpts, kpts_band, max_memory=max_memory)
-        logger.debug(ks, 'nelec by numeric integration = %s', n)
-        if ks.nlc or ni.libxc.is_nlc(ks.xc):
+        logger.info(ks, 'nelec by numeric integration = %s', n)
+        if ks.do_nlc():
             if ni.libxc.is_nlc(ks.xc):
                 xc = ks.xc
             else:
                 assert ni.libxc.is_nlc(ks.nlc)
                 xc = ks.nlc
             n, enlc, vnlc = ni.nr_nlc_vxc(cell, ks.nlcgrids, xc, dm, 0, hermi, kpts,
                                           max_memory=max_memory)
             exc += enlc
             vxc += vnlc
-            logger.debug(ks, 'nelec with nlc grids = %s', n)
+            logger.info(ks, 'nelec with nlc grids = %s', n)
         t0 = logger.timer(ks, 'vxc', *t0)
 
     nkpts = len(kpts)
     weight = 1. / nkpts
     if not hybrid:
         vj = ks.get_j(cell, dm, hermi, kpts, kpts_band)
         vxc += vj
@@ -177,27 +177,17 @@
 
     def nuc_grad_method(self):
         from pyscf.pbc.grad import krks
         return krks.Gradients(self)
 
     def to_hf(self):
         '''Convert to KRHF object.'''
-        from pyscf.pbc import scf
-        return self._transfer_attrs_(scf.KRHF(self.cell, self.kpts))
+        from pyscf.pbc import scf, df
+        out = self._transfer_attrs_(scf.KRHF(self.cell, self.kpts))
+        # Pure functionals only construct J-type integrals. Enable all integrals for KHF.
+        if (not self._numint.libxc.is_hybrid_xc(self.xc) and
+            len(self.kpts) > 1 and getattr(self.with_df, '_j_only', False)):
+            out.with_df._j_only = False
+            out.with_df.reset()
+        return out
 
-
-if __name__ == '__main__':
-    from pyscf.pbc import gto
-    cell = gto.Cell()
-    cell.unit = 'A'
-    cell.atom = 'C 0.,  0.,  0.; C 0.8917,  0.8917,  0.8917'
-    cell.a = '''0.      1.7834  1.7834
-                1.7834  0.      1.7834
-                1.7834  1.7834  0.    '''
-
-    cell.basis = 'gth-szv'
-    cell.pseudo = 'gth-pade'
-    cell.verbose = 7
-    cell.output = '/dev/null'
-    cell.build()
-    mf = KRKS(cell, cell.make_kpts([2,1,1]))
-    print(mf.kernel())
+    to_gpu = lib.to_gpu
```

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/krks_ksymm.py` & `pyscf-2.6.0/pyscf/pbc/dft/krks_ksymm.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,44 +50,44 @@
                        'match the number of IBZ k-points: '
                        f'{len(dm)} vs {kpts.nkpts_ibz}.')
     dm_bz = kpts.transform_dm(dm)
 
     hybrid = ni.libxc.is_hybrid_xc(ks.xc)
 
     if not hybrid and isinstance(ks.with_df, multigrid.MultiGridFFTDF):
-        if ks.nlc or ni.libxc.is_nlc(ks.xc):
+        if ks.do_nlc():
             raise NotImplementedError(f'MultiGrid for NLC functional {ks.xc} + {ks.nlc}')
         n, exc, vxc = multigrid.nr_rks(ks.with_df, ks.xc, dm_bz, hermi,
                                        kpts.kpts, kpts_band,
                                        with_j=True, return_j=False)
-        logger.debug(ks, 'nelec by numeric integration = %s', n)
+        logger.info(ks, 'nelec by numeric integration = %s', n)
         t0 = logger.timer(ks, 'vxc', *t0)
         return vxc
 
     ks.initialize_grids(cell, dm_bz, kpts.kpts, ground_state)
 
     if hermi == 2:  # because rho = 0
         n, exc, vxc = 0, 0, 0
     else:
         max_memory = ks.max_memory - lib.current_memory()[0]
         n, exc, vxc = ni.nr_rks(cell, ks.grids, ks.xc, dm_bz,
                                 kpts=kpts.kpts, kpts_band=kpts_band,
                                 max_memory=max_memory)
-        logger.debug(ks, 'nelec by numeric integration = %s', n)
-        if ks.nlc or ni.libxc.is_nlc(ks.xc):
+        logger.info(ks, 'nelec by numeric integration = %s', n)
+        if ks.do_nlc():
             if ni.libxc.is_nlc(ks.xc):
                 xc = ks.xc
             else:
                 assert ni.libxc.is_nlc(ks.nlc)
                 xc = ks.nlc
             n, enlc, vnlc = ni.nr_nlc_vxc(cell, ks.nlcgrids, xc, dm_bz,
                                           0, hermi, kpts.kpts, max_memory=max_memory)
             exc += enlc
             vxc += vnlc
-            logger.debug(ks, 'nelec with nlc grids = %s', n)
+            logger.info(ks, 'nelec with nlc grids = %s', n)
         t0 = logger.timer(ks, 'vxc', *t0)
 
     weight = kpts.weights_ibz
     if not hybrid:
         vj = ks.get_j(cell, dm, hermi, kpts, kpts_band)
         vxc += vj
     else:
```

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/krkspu.py` & `pyscf-2.6.0/pyscf/pbc/dft/krkspu.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/krkspu_ksymm.py` & `pyscf-2.6.0/pyscf/pbc/dft/krkspu_ksymm.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/kroks.py` & `pyscf-2.6.0/pyscf/pbc/dft/roks.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,64 +9,70 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-# Authors: Qiming Sun <osirpt.sun@gmail.com>
+# Author: Qiming Sun <osirpt.sun@gmail.com>
 #
 
 '''
-Restricted open-shell Kohn-Sham for periodic systems with k-point sampling
+Restricted open-shell Kohn-Sham for periodic systems at a single k-point
 '''
 
-import numpy as np
+import numpy
+import pyscf.dft
 from pyscf import lib
-from pyscf.pbc.scf import krohf
+from pyscf.pbc.scf import rohf
 from pyscf.pbc.dft import rks
-from pyscf.pbc.dft import kuks
-from pyscf.pbc.dft.kuks import energy_elec
+from pyscf.pbc.dft import uks
 from pyscf import __config__
 
 
-@lib.with_doc(kuks.get_veff.__doc__)
+@lib.with_doc(uks.get_veff.__doc__)
 def get_veff(ks, cell=None, dm=None, dm_last=0, vhf_last=0, hermi=1,
-             kpts=None, kpts_band=None):
+             kpt=None, kpts_band=None):
     if getattr(dm, 'mo_coeff', None) is not None:
         mo_coeff = dm.mo_coeff
-        mo_occ_a = [(x > 0).astype(np.double) for x in dm.mo_occ]
-        mo_occ_b = [(x ==2).astype(np.double) for x in dm.mo_occ]
+        mo_occ_a = (dm.mo_occ > 0).astype(numpy.double)
+        mo_occ_b = (dm.mo_occ ==2).astype(numpy.double)
         dm = lib.tag_array(dm, mo_coeff=(mo_coeff,mo_coeff),
                            mo_occ=(mo_occ_a,mo_occ_b))
-    return kuks.get_veff(ks, cell, dm, dm_last, vhf_last, hermi, kpts, kpts_band)
+    return uks.get_veff(ks, cell, dm, dm_last, vhf_last, hermi, kpt, kpts_band)
 
 
-class KROKS(rks.KohnShamDFT, krohf.KROHF):
-    '''RKS class adapted for PBCs with k-point sampling.
+class ROKS(rks.KohnShamDFT, rohf.ROHF):
+    '''UKS class adapted for PBCs.
+
+    This is a literal duplication of the molecular UKS class with some `mol`
+    variables replaced by `cell`.
     '''
 
+    get_vsap = rks.RKS.get_vsap
+    init_guess_by_vsap = rks.RKS.init_guess_by_vsap
     get_veff = get_veff
-    energy_elec = energy_elec
-    get_rho = kuks.get_rho
+    energy_elec = pyscf.dft.uks.energy_elec
 
-    def __init__(self, cell, kpts=np.zeros((1,3)), xc='LDA,VWN',
+    def __init__(self, cell, kpt=numpy.zeros(3), xc='LDA,VWN',
                  exxdiv=getattr(__config__, 'pbc_scf_SCF_exxdiv', 'ewald')):
-        krohf.KROHF.__init__(self, cell, kpts, exxdiv=exxdiv)
+        rohf.ROHF.__init__(self, cell, kpt, exxdiv=exxdiv)
         rks.KohnShamDFT.__init__(self, xc)
 
     def dump_flags(self, verbose=None):
-        krohf.KROHF.dump_flags(self, verbose)
+        rohf.ROHF.dump_flags(self, verbose)
         rks.KohnShamDFT.dump_flags(self, verbose)
         return self
 
     def to_hf(self):
-        '''Convert to KROHF object.'''
+        '''Convert to RHF object.'''
         from pyscf.pbc import scf
-        return self._transfer_attrs_(scf.KROHF(self.cell, self.kpts))
+        return self._transfer_attrs_(scf.ROHF(self.cell, self.kpt))
+
+    to_gpu = lib.to_gpu
 
 
 if __name__ == '__main__':
     from pyscf.pbc import gto
     cell = gto.Cell()
     cell.unit = 'A'
     cell.atom = 'C 0.,  0.,  0.; C 0.8917,  0.8917,  0.8917'
@@ -75,9 +81,9 @@
                 1.7834  1.7834  0.    '''
 
     cell.basis = 'gth-szv'
     cell.pseudo = 'gth-pade'
     cell.verbose = 7
     cell.output = '/dev/null'
     cell.build()
-    mf = KROKS(cell, cell.make_kpts([2,1,1]))
+    mf = ROKS(cell)
     print(mf.kernel())
```

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/kuks.py` & `pyscf-2.6.0/pyscf/pbc/dft/kuks.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,44 +46,44 @@
     if kpts is None: kpts = ks.kpts
     t0 = (logger.process_clock(), logger.perf_counter())
 
     ni = ks._numint
     hybrid = ni.libxc.is_hybrid_xc(ks.xc)
 
     if not hybrid and isinstance(ks.with_df, multigrid.MultiGridFFTDF):
-        if ks.nlc or ni.libxc.is_nlc(ks.xc):
+        if ks.do_nlc():
             raise NotImplementedError(f'MultiGrid for NLC functional {ks.xc} + {ks.nlc}')
         n, exc, vxc = multigrid.nr_uks(ks.with_df, ks.xc, dm, hermi,
                                        kpts, kpts_band,
                                        with_j=True, return_j=False)
-        logger.debug(ks, 'nelec by numeric integration = %s', n)
+        logger.info(ks, 'nelec by numeric integration = %s', n)
         t0 = logger.timer(ks, 'vxc', *t0)
         return vxc
 
     # ndim = 4 : dm.shape = ([alpha,beta], nkpts, nao, nao)
     ground_state = (dm.ndim == 4 and dm.shape[0] == 2 and kpts_band is None)
     ks.initialize_grids(cell, dm, kpts, ground_state)
 
     if hermi == 2:  # because rho = 0
         n, exc, vxc = (0,0), 0, 0
     else:
         max_memory = ks.max_memory - lib.current_memory()[0]
         n, exc, vxc = ni.nr_uks(cell, ks.grids, ks.xc, dm, 0, hermi,
                                 kpts, kpts_band, max_memory=max_memory)
-        if ks.nlc or ni.libxc.is_nlc(ks.xc):
+        if ks.do_nlc():
             if ni.libxc.is_nlc(ks.xc):
                 xc = ks.xc
             else:
                 assert ni.libxc.is_nlc(ks.nlc)
                 xc = ks.nlc
             n, enlc, vnlc = ni.nr_nlc_vxc(cell, ks.nlcgrids, xc, dm[0]+dm[1],
                                           0, hermi, kpts, max_memory=max_memory)
             exc += enlc
             vxc += vnlc
-        logger.debug(ks, 'nelec by numeric integration = %s', n)
+        logger.info(ks, 'nelec by numeric integration = %s', n)
         t0 = logger.timer(ks, 'vxc', *t0)
 
     nkpts = len(kpts)
     weight = 1. / nkpts
 
     if not hybrid:
         vj = ks.get_j(cell, dm[0]+dm[1], hermi, kpts, kpts_band)
@@ -153,27 +153,17 @@
 
     def nuc_grad_method(self):
         from pyscf.pbc.grad import kuks
         return kuks.Gradients(self)
 
     def to_hf(self):
         '''Convert to KUHF object.'''
-        from pyscf.pbc import scf
-        return self._transfer_attrs_(scf.KUHF(self.cell, self.kpts))
+        from pyscf.pbc import scf, df
+        out = self._transfer_attrs_(scf.KUHF(self.cell, self.kpts))
+        # Pure functionals only construct J-type integrals. Enable all integrals for KHF.
+        if (not self._numint.libxc.is_hybrid_xc(self.xc) and
+            len(self.kpts) > 1 and getattr(self.with_df, '_j_only', False)):
+            out.with_df._j_only = False
+            out.with_df.reset()
+        return out
 
-
-if __name__ == '__main__':
-    from pyscf.pbc import gto
-    cell = gto.Cell()
-    cell.unit = 'A'
-    cell.atom = 'C 0.,  0.,  0.; C 0.8917,  0.8917,  0.8917'
-    cell.a = '''0.      1.7834  1.7834
-                1.7834  0.      1.7834
-                1.7834  1.7834  0.    '''
-
-    cell.basis = 'gth-szv'
-    cell.pseudo = 'gth-pade'
-    cell.verbose = 7
-    cell.output = '/dev/null'
-    cell.build()
-    mf = KUKS(cell, cell.make_kpts([2,1,1]))
-    print(mf.kernel())
+    to_gpu = lib.to_gpu
```

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/kuks_ksymm.py` & `pyscf-2.6.0/pyscf/pbc/dft/kuks_ksymm.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,44 +49,44 @@
                        'match the number of IBZ k-points: '
                        f'{len(dm[0])} vs {kpts.nkpts_ibz}.')
     dm_bz = kpts.transform_dm(dm)
 
     hybrid = ni.libxc.is_hybrid_xc(ks.xc)
 
     if not hybrid and isinstance(ks.with_df, multigrid.MultiGridFFTDF):
-        if ks.nlc or ni.libxc.is_nlc(ks.xc):
+        if ks.do_nlc():
             raise NotImplementedError(f'MultiGrid for NLC functional {ks.xc} + {ks.nlc}')
         n, exc, vxc = multigrid.nr_uks(ks.with_df, ks.xc, dm_bz, hermi,
                                        kpts.kpts, kpts_band,
                                        with_j=True, return_j=False)
-        logger.debug(ks, 'nelec by numeric integration = %s', n)
+        logger.info(ks, 'nelec by numeric integration = %s', n)
         t0 = logger.timer(ks, 'vxc', *t0)
         return vxc
 
     ks.initialize_grids(cell, dm_bz, kpts.kpts, ground_state)
 
     if hermi == 2:  # because rho = 0
         n, exc, vxc = (0,0), 0, 0
     else:
         max_memory = ks.max_memory - lib.current_memory()[0]
         n, exc, vxc = ni.nr_uks(cell, ks.grids, ks.xc, dm_bz,
                                 kpts=kpts.kpts, kpts_band=kpts_band,
                                 max_memory=max_memory)
-        logger.debug(ks, 'nelec by numeric integration = %s', n)
-        if ks.nlc or ni.libxc.is_nlc(ks.xc):
+        logger.info(ks, 'nelec by numeric integration = %s', n)
+        if ks.do_nlc():
             if ni.libxc.is_nlc(ks.xc):
                 xc = ks.xc
             else:
                 assert ni.libxc.is_nlc(ks.nlc)
                 xc = ks.nlc
             n, enlc, vnlc = ni.nr_nlc_vxc(cell, ks.nlcgrids, xc, dm_bz[0]+dm_bz[1],
                                           0, hermi, kpts.kpts, max_memory=max_memory)
             exc += enlc
             vxc += vnlc
-            logger.debug(ks, 'nelec with nlc grids = %s', n)
+            logger.info(ks, 'nelec with nlc grids = %s', n)
         t0 = logger.timer(ks, 'vxc', *t0)
 
     weight = kpts.weights_ibz
 
     if not hybrid:
         vj = ks.get_j(cell, dm[0]+dm[1], hermi, kpts, kpts_band)
         vxc += vj
```

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/kukspu.py` & `pyscf-2.6.0/pyscf/pbc/dft/kukspu.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/kukspu_ksymm.py` & `pyscf-2.6.0/pyscf/pbc/dft/kukspu_ksymm.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/multigrid.py` & `pyscf-2.6.0/pyscf/pbc/dft/multigrid/multigrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# Copyright 2014-2021 The PySCF Developers. All Rights Reserved.
+# Copyright 2014-2024 The PySCF Developers. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,27 +18,37 @@
 
 '''Multigrid to compute DFT integrals'''
 
 import ctypes
 import numpy
 import scipy.linalg
 
+from pyscf import __config__
 from pyscf import lib
 from pyscf.lib import logger
 from pyscf.gto import ATOM_OF, ANG_OF, NPRIM_OF, PTR_EXP, PTR_COEFF
 from pyscf.dft.numint import libdft, BLKSIZE, MGGA_DENSITY_LAPL
 from pyscf.pbc import tools
 from pyscf.pbc import gto
 from pyscf.pbc.gto import pseudo
+from pyscf.pbc.gto.pseudo import pp_int
 from pyscf.pbc.dft import numint, gen_grid
-from pyscf.pbc.df.df_jk import _format_dms, _format_kpts_band, _format_jks
+from pyscf.pbc.df.df_jk import (
+    _format_dms,
+    _format_kpts_band,
+    _format_jks,
+)
 from pyscf.pbc.lib.kpts_helper import gamma_point
-from pyscf.pbc.df import fft
-from pyscf.pbc.df import ft_ao
-from pyscf import __config__
+from pyscf.pbc.df import fft, ft_ao
+from pyscf.pbc.dft.multigrid.utils import (
+    _take_4d,
+    _take_5d,
+    _takebak_4d,
+    _takebak_5d,
+)
 
 #sys.stderr.write('WARN: multigrid is an experimental feature. It is still in '
 #                 'testing\nFeatures and APIs may be changed in the future.\n')
 
 EXTRA_PREC = getattr(__config__, 'pbc_gto_eval_gto_extra_precision', 1e-2)
 TO_EVEN_GRIDS = getattr(__config__, 'pbc_dft_multigrid_to_even', False)
 RMAX_FACTOR_ORTH = getattr(__config__, 'pbc_dft_multigrid_rmax_factor_orth', 1.1)
@@ -363,102 +373,134 @@
     hermi = 1
     vne = _get_j_pass2(mydf, vneG, hermi, kpts)[0]
 
     if is_single_kpt:
         vne = vne[0]
     return numpy.asarray(vne)
 
-def get_pp(mydf, kpts=None):
+def get_pp(mydf, kpts=None, max_memory=4000):
     '''Get the periodic pseudotential nuc-el AO matrix, with G=0 removed.
     '''
     from pyscf import gto
     kpts, is_single_kpt = fft._check_kpts(mydf, kpts)
     cell = mydf.cell
     mesh = mydf.mesh
-    SI = cell.get_SI()
     Gv = cell.get_Gv(mesh)
-    vpplocG = pseudo.get_vlocG(cell, Gv)
-    vpplocG = -numpy.einsum('ij,ij->j', SI, vpplocG)
-    # from get_jvloc_G0 function
-    vpplocG[0] = numpy.sum(pseudo.get_alphas(cell))
-    ngrids = len(vpplocG)
+
+    ngrids = len(Gv)
+    vpplocG = numpy.empty((ngrids,), dtype=numpy.complex128)
+
+    mem_avail = max(max_memory, mydf.max_memory-lib.current_memory()[0])
+    blksize = int(mem_avail*1e6/((cell.natm*2)*16))
+    blksize = min(ngrids, max(21**3, blksize))
+    for ig0, ig1 in lib.prange(0, ngrids, blksize):
+        vpplocG_batch = pp_int.get_gth_vlocG_part1(cell, Gv[ig0:ig1])
+        SI = cell.get_SI(Gv[ig0:ig1])
+        vpplocG[ig0:ig1] = -numpy.einsum('ij,ij->j', SI, vpplocG_batch)
 
     hermi = 1
     vpp = _get_j_pass2(mydf, vpplocG, hermi, kpts)[0]
+    vpp2 = pp_int.get_pp_loc_part2(cell, kpts)
+    for k, kpt in enumerate(kpts):
+        vpp[k] += vpp2[k]
 
     # vppnonloc evaluated in reciprocal space
     fakemol = gto.Mole()
     fakemol._atm = numpy.zeros((1,gto.ATM_SLOTS), dtype=numpy.int32)
     fakemol._bas = numpy.zeros((1,gto.BAS_SLOTS), dtype=numpy.int32)
     ptr = gto.PTR_ENV_START
     fakemol._env = numpy.zeros(ptr+10)
     fakemol._bas[0,gto.NPRIM_OF ] = 1
     fakemol._bas[0,gto.NCTR_OF  ] = 1
     fakemol._bas[0,gto.PTR_EXP  ] = ptr+3
     fakemol._bas[0,gto.PTR_COEFF] = ptr+4
 
-    # buf for SPG_lmi upto l=0..3 and nl=3
-    buf = numpy.empty((48,ngrids), dtype=numpy.complex128)
-
     def vppnl_by_k(kpt):
-        Gk = Gv + kpt
-        G_rad = lib.norm(Gk, axis=1)
-        aokG = ft_ao.ft_ao(cell, Gv, kpt=kpt) * (ngrids/cell.vol)
-        vppnl = 0
+        SPG_lm_aoGs = []
         for ia in range(cell.natm):
             symb = cell.atom_symbol(ia)
             if symb not in cell._pseudo:
+                SPG_lm_aoGs.append(None)
                 continue
             pp = cell._pseudo[symb]
             p1 = 0
             for l, proj in enumerate(pp[5:]):
                 rl, nl, hl = proj
                 if nl > 0:
-                    fakemol._bas[0,gto.ANG_OF] = l
-                    fakemol._env[ptr+3] = .5*rl**2
-                    fakemol._env[ptr+4] = rl**(l+1.5)*numpy.pi**1.25
-                    pYlm_part = fakemol.eval_gto('GTOval', Gk)
+                    p1 = p1+nl*(l*2+1)
+            SPG_lm_aoGs.append(numpy.zeros((p1, cell.nao), dtype=numpy.complex128))
 
-                    p0, p1 = p1, p1+nl*(l*2+1)
-                    # pYlm is real, SI[ia] is complex
-                    pYlm = numpy.ndarray((nl,l*2+1,ngrids), dtype=numpy.complex128, buffer=buf[p0:p1])
-                    for k in range(nl):
-                        qkl = pseudo.pp._qli(G_rad*rl, l, k)
-                        pYlm[k] = pYlm_part.T * qkl
-                    #:SPG_lmi = numpy.einsum('g,nmg->nmg', SI[ia].conj(), pYlm)
-                    #:SPG_lm_aoG = numpy.einsum('nmg,gp->nmp', SPG_lmi, aokG)
-                    #:tmp = numpy.einsum('ij,jmp->imp', hl, SPG_lm_aoG)
-                    #:vppnl += numpy.einsum('imp,imq->pq', SPG_lm_aoG.conj(), tmp)
-            if p1 > 0:
-                SPG_lmi = buf[:p1]
-                SPG_lmi *= SI[ia].conj()
-                SPG_lm_aoGs = lib.zdot(SPG_lmi, aokG)
+        mem_avail = max(max_memory, mydf.max_memory-lib.current_memory()[0])
+        blksize = int(mem_avail*1e6/((48+cell.nao+13+3)*16))
+        blksize = min(ngrids, max(21**3, blksize))
+        vppnl = 0
+        for ig0, ig1 in lib.prange(0, ngrids, blksize):
+            ng = ig1 - ig0
+            # buf for SPG_lmi upto l=0..3 and nl=3
+            buf = numpy.empty((48,ng), dtype=numpy.complex128)
+            Gk = Gv[ig0:ig1] + kpt
+            G_rad = numpy.linalg.norm(Gk, axis=1)
+            aokG = ft_ao.ft_ao(cell, Gv[ig0:ig1], kpt=kpt) * (ngrids/cell.vol)
+            for ia in range(cell.natm):
+                symb = cell.atom_symbol(ia)
+                if symb not in cell._pseudo:
+                    continue
+                pp = cell._pseudo[symb]
                 p1 = 0
                 for l, proj in enumerate(pp[5:]):
                     rl, nl, hl = proj
                     if nl > 0:
+                        fakemol._bas[0,gto.ANG_OF] = l
+                        fakemol._env[ptr+3] = .5*rl**2
+                        fakemol._env[ptr+4] = rl**(l+1.5)*numpy.pi**1.25
+                        pYlm_part = fakemol.eval_gto('GTOval', Gk)
+
                         p0, p1 = p1, p1+nl*(l*2+1)
-                        hl = numpy.asarray(hl)
-                        SPG_lm_aoG = SPG_lm_aoGs[p0:p1].reshape(nl,l*2+1,-1)
-                        tmp = numpy.einsum('ij,jmp->imp', hl, SPG_lm_aoG)
-                        vppnl += numpy.einsum('imp,imq->pq', SPG_lm_aoG.conj(), tmp)
+                        # pYlm is real, SI[ia] is complex
+                        pYlm = numpy.ndarray((nl,l*2+1,ng), dtype=numpy.complex128, buffer=buf[p0:p1])
+                        for k in range(nl):
+                            qkl = pseudo.pp._qli(G_rad*rl, l, k)
+                            pYlm[k] = pYlm_part.T * qkl
+                        #:SPG_lmi = numpy.einsum('g,nmg->nmg', SI[ia].conj(), pYlm)
+                        #:SPG_lm_aoG = numpy.einsum('nmg,gp->nmp', SPG_lmi, aokG)
+                        #:tmp = numpy.einsum('ij,jmp->imp', hl, SPG_lm_aoG)
+                        #:vppnl += numpy.einsum('imp,imq->pq', SPG_lm_aoG.conj(), tmp)
+                if p1 > 0:
+                    SPG_lmi = buf[:p1]
+                    SPG_lmi *= cell.get_SI(Gv[ig0:ig1], atmlst=[ia,]).conj()
+                    SPG_lm_aoGs[ia] += lib.zdot(SPG_lmi, aokG)
+            buf = None
+        for ia in range(cell.natm):
+            symb = cell.atom_symbol(ia)
+            if symb not in cell._pseudo:
+                continue
+            pp = cell._pseudo[symb]
+            p1 = 0
+            for l, proj in enumerate(pp[5:]):
+                rl, nl, hl = proj
+                if nl > 0:
+                    p0, p1 = p1, p1+nl*(l*2+1)
+                    hl = numpy.asarray(hl)
+                    SPG_lm_aoG = SPG_lm_aoGs[ia][p0:p1].reshape(nl,l*2+1,-1)
+                    tmp = numpy.einsum('ij,jmp->imp', hl, SPG_lm_aoG)
+                    vppnl += numpy.einsum('imp,imq->pq', SPG_lm_aoG.conj(), tmp)
+        SPG_lm_aoGs=None
         return vppnl * (1./ngrids**2)
 
     for k, kpt in enumerate(kpts):
         vppnl = vppnl_by_k(kpt)
         if gamma_point(kpt):
             vpp[k] = vpp[k].real + vppnl.real
         else:
             vpp[k] += vppnl
 
     if is_single_kpt:
         vpp = vpp[0]
     return numpy.asarray(vpp)
 
-
 def get_j_kpts(mydf, dm_kpts, hermi=1, kpts=numpy.zeros((1,3)), kpts_band=None):
     '''Get the Coulomb (J) AO matrix at sampled k-points.
 
     Args:
         dm_kpts : (nkpts, nao, nao) ndarray or a list of (nkpts,nao,nao) ndarray
             Density matrix at each k-point.  If a list of k-point DMs, eg,
             UHF alpha and beta DM, the alpha and beta DMs are contracted
@@ -1855,68 +1897,19 @@
             if with_j:
                 vj = get_j_kpts(self, dm, hermi, kpts, kpts_band)
         return vj, vk
 
     get_rho = get_rho
 
 
-def multigrid(mf):
+def multigrid_fftdf(mf):
     '''Use MultiGridFFTDF to replace the default FFTDF integration method in
     the DFT object.
     '''
     mf.with_df, old_df = MultiGridFFTDF(mf.cell), mf.with_df
     mf.with_df.__dict__.update(old_df.__dict__)
     return mf
 
+multigrid = multigrid_fftdf # for backward compatibility
 
 def _pgto_shells(cell):
     return cell._bas[:,NPRIM_OF].sum()
-
-def _take_4d(a, indices):
-    a_shape = a.shape
-    ranges = []
-    for i, s in enumerate(indices):
-        if s is None:
-            idx = numpy.arange(a_shape[i], dtype=numpy.int32)
-        else:
-            idx = numpy.asarray(s, dtype=numpy.int32)
-            idx[idx < 0] += a_shape[i]
-        ranges.append(idx)
-    idx = ranges[0][:,None] * a_shape[1] + ranges[1]
-    idy = ranges[2][:,None] * a_shape[3] + ranges[3]
-    a = a.reshape(a_shape[0]*a_shape[1], a_shape[2]*a_shape[3])
-    out = lib.take_2d(a, idx.ravel(), idy.ravel())
-    return out.reshape([len(s) for s in ranges])
-
-def _takebak_4d(out, a, indices):
-    out_shape = out.shape
-    a_shape = a.shape
-    ranges = []
-    for i, s in enumerate(indices):
-        if s is None:
-            idx = numpy.arange(a_shape[i], dtype=numpy.int32)
-        else:
-            idx = numpy.asarray(s, dtype=numpy.int32)
-            idx[idx < 0] += out_shape[i]
-        assert (len(idx) == a_shape[i])
-        ranges.append(idx)
-    idx = ranges[0][:,None] * out_shape[1] + ranges[1]
-    idy = ranges[2][:,None] * out_shape[3] + ranges[3]
-    nx = idx.size
-    ny = idy.size
-    out = out.reshape(out_shape[0]*out_shape[1], out_shape[2]*out_shape[3])
-    lib.takebak_2d(out, a.reshape(nx,ny), idx.ravel(), idy.ravel())
-    return out
-
-def _take_5d(a, indices):
-    a_shape = a.shape
-    a = a.reshape((a_shape[0]*a_shape[1],) + a_shape[2:])
-    indices = (None,) + indices[2:]
-    return _take_4d(a, indices)
-
-def _takebak_5d(out, a, indices):
-    a_shape = a.shape
-    out_shape = out.shape
-    a = a.reshape((a_shape[0]*a_shape[1],) + a_shape[2:])
-    out = out.reshape((out_shape[0]*out_shape[1],) + out_shape[2:])
-    indices = (None,) + indices[2:]
-    return _takebak_4d(out, a, indices)
```

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/numint.py` & `pyscf-2.6.0/pyscf/pbc/dft/numint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1078,14 +1078,16 @@
     get_rho = get_rho
 
     def eval_rho1(self, cell, ao, dm, screen_index=None, xctype='LDA', hermi=0,
                   with_lapl=True, cutoff=None, ao_cutoff=None, verbose=None):
         return self.eval_rho(cell, ao, dm, screen_index, xctype, hermi,
                              with_lapl, verbose)
 
+    to_gpu = lib.to_gpu
+
 _NumInt = NumInt
 
 
 class KNumInt(lib.StreamObject, numint.LibXCMixin):
     '''Generalization of pyscf's NumInt class for k-point sampling and
     periodic images.
     '''
@@ -1283,8 +1285,10 @@
     nr_rks_fxc = nr_rks_fxc
     nr_uks_fxc = nr_uks_fxc
     nr_rks_fxc_st = nr_rks_fxc_st
     cache_xc_kernel  = cache_xc_kernel
     cache_xc_kernel1 = cache_xc_kernel1
     get_rho = get_rho
 
+    to_gpu = lib.to_gpu
+
 _KNumInt = KNumInt
```

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/numint2c.py` & `pyscf-2.6.0/pyscf/pbc/dft/numint2c.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/rks.py` & `pyscf-2.6.0/pyscf/pbc/dft/rks.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,45 +64,45 @@
     if kpt is None: kpt = ks.kpt
     t0 = (logger.process_clock(), logger.perf_counter())
 
     ni = ks._numint
     hybrid = ni.libxc.is_hybrid_xc(ks.xc)
 
     if not hybrid and isinstance(ks.with_df, multigrid.MultiGridFFTDF):
-        if ks.nlc or ni.libxc.is_nlc(ks.xc):
+        if ks.do_nlc():
             raise NotImplementedError(f'MultiGrid for NLC functional {ks.xc} + {ks.nlc}')
         n, exc, vxc = multigrid.nr_rks(ks.with_df, ks.xc, dm, hermi,
                                        kpt.reshape(1,3), kpts_band,
                                        with_j=True, return_j=False)
-        logger.debug(ks, 'nelec by numeric integration = %s', n)
+        logger.info(ks, 'nelec by numeric integration = %s', n)
         t0 = logger.timer(ks, 'vxc', *t0)
         return vxc
 
     ground_state = (isinstance(dm, numpy.ndarray) and dm.ndim == 2
                     and kpts_band is None)
     ks.initialize_grids(cell, dm, kpt, ground_state)
 
     if hermi == 2:  # because rho = 0
         n, exc, vxc = 0, 0, 0
     else:
         max_memory = ks.max_memory - lib.current_memory()[0]
         n, exc, vxc = ni.nr_rks(cell, ks.grids, ks.xc, dm, 0, hermi,
                                 kpt, kpts_band, max_memory=max_memory)
-        logger.debug(ks, 'nelec by numeric integration = %s', n)
-        if ks.nlc or ni.libxc.is_nlc(ks.xc):
+        logger.info(ks, 'nelec by numeric integration = %s', n)
+        if ks.do_nlc():
             if ni.libxc.is_nlc(ks.xc):
                 xc = ks.xc
             else:
                 assert ni.libxc.is_nlc(ks.nlc)
                 xc = ks.nlc
             n, enlc, vnlc = ni.nr_nlc_vxc(cell, ks.nlcgrids, xc, dm, 0, hermi, kpt,
                                           max_memory=max_memory)
             exc += enlc
             vxc += vnlc
-            logger.debug(ks, 'nelec with nlc grids = %s', n)
+            logger.info(ks, 'nelec with nlc grids = %s', n)
         t0 = logger.timer(ks, 'vxc', *t0)
 
     if not hybrid:
         vj = ks.get_j(cell, dm, hermi, kpt, kpts_band)
         vxc += vj
     else:
         omega, alpha, hyb = ni.rsh_and_hybrid_coeff(ks.xc, spin=cell.spin)
@@ -296,16 +296,15 @@
             t0 = (logger.process_clock(), logger.perf_counter())
             self.grids.build(with_non0tab=True)
             if (isinstance(self.grids, gen_grid.BeckeGrids) and
                 self.small_rho_cutoff > 1e-20 and ground_state):
                 self.grids = prune_small_rho_grids_(
                     self, self.cell, dm, self.grids, kpts)
             t0 = logger.timer(self, 'setting up grids', *t0)
-
-        is_nlc = self.nlc or self._numint.libxc.is_nlc(self.xc)
+        is_nlc = self.do_nlc()
         if is_nlc and self.nlcgrids.coords is None:
             t0 = (logger.process_clock(), logger.perf_counter())
             self.nlcgrids.build(with_non0tab=True)
             if (isinstance(self.grids, gen_grid.BeckeGrids) and
                 self.small_rho_cutoff > 1e-20 and ground_state):
                 self.nlcgrids = prune_small_rho_grids_(
                     self, self.cell, dm, self.nlcgrids, kpts)
@@ -342,14 +341,16 @@
         return self
 
     def to_hf(self):
         '''Convert to RHF object.'''
         from pyscf.pbc import scf
         return self._transfer_attrs_(scf.RHF(self.cell, self.kpt))
 
+    to_gpu = lib.to_gpu
+
 
 if __name__ == '__main__':
     from pyscf.pbc import gto
     cell = gto.Cell()
     cell.unit = 'A'
     cell.atom = 'C 0.,  0.,  0.; C 0.8917,  0.8917,  0.8917'
     cell.a = '''0.      1.7834  1.7834
```

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/roks.py` & `pyscf-2.6.0/pyscf/pbc/dft/kroks.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,79 +9,65 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-# Author: Qiming Sun <osirpt.sun@gmail.com>
+# Authors: Qiming Sun <osirpt.sun@gmail.com>
 #
 
 '''
-Restricted open-shell Kohn-Sham for periodic systems at a single k-point
+Restricted open-shell Kohn-Sham for periodic systems with k-point sampling
 '''
 
-import numpy
-import pyscf.dft
+import numpy as np
 from pyscf import lib
-from pyscf.pbc.scf import rohf
+from pyscf.pbc.scf import krohf
 from pyscf.pbc.dft import rks
-from pyscf.pbc.dft import uks
+from pyscf.pbc.dft import kuks
+from pyscf.pbc.dft.kuks import energy_elec
 from pyscf import __config__
 
 
-@lib.with_doc(uks.get_veff.__doc__)
+@lib.with_doc(kuks.get_veff.__doc__)
 def get_veff(ks, cell=None, dm=None, dm_last=0, vhf_last=0, hermi=1,
-             kpt=None, kpts_band=None):
+             kpts=None, kpts_band=None):
     if getattr(dm, 'mo_coeff', None) is not None:
         mo_coeff = dm.mo_coeff
-        mo_occ_a = (dm.mo_occ > 0).astype(numpy.double)
-        mo_occ_b = (dm.mo_occ ==2).astype(numpy.double)
+        mo_occ_a = [(x > 0).astype(np.double) for x in dm.mo_occ]
+        mo_occ_b = [(x ==2).astype(np.double) for x in dm.mo_occ]
         dm = lib.tag_array(dm, mo_coeff=(mo_coeff,mo_coeff),
                            mo_occ=(mo_occ_a,mo_occ_b))
-    return uks.get_veff(ks, cell, dm, dm_last, vhf_last, hermi, kpt, kpts_band)
+    return kuks.get_veff(ks, cell, dm, dm_last, vhf_last, hermi, kpts, kpts_band)
 
 
-class ROKS(rks.KohnShamDFT, rohf.ROHF):
-    '''UKS class adapted for PBCs.
-
-    This is a literal duplication of the molecular UKS class with some `mol`
-    variables replaced by `cell`.
+class KROKS(rks.KohnShamDFT, krohf.KROHF):
+    '''RKS class adapted for PBCs with k-point sampling.
     '''
 
-    get_vsap = rks.RKS.get_vsap
-    init_guess_by_vsap = rks.RKS.init_guess_by_vsap
     get_veff = get_veff
-    energy_elec = pyscf.dft.uks.energy_elec
+    energy_elec = energy_elec
+    get_rho = kuks.get_rho
 
-    def __init__(self, cell, kpt=numpy.zeros(3), xc='LDA,VWN',
+    def __init__(self, cell, kpts=np.zeros((1,3)), xc='LDA,VWN',
                  exxdiv=getattr(__config__, 'pbc_scf_SCF_exxdiv', 'ewald')):
-        rohf.ROHF.__init__(self, cell, kpt, exxdiv=exxdiv)
+        krohf.KROHF.__init__(self, cell, kpts, exxdiv=exxdiv)
         rks.KohnShamDFT.__init__(self, xc)
 
     def dump_flags(self, verbose=None):
-        rohf.ROHF.dump_flags(self, verbose)
+        krohf.KROHF.dump_flags(self, verbose)
         rks.KohnShamDFT.dump_flags(self, verbose)
         return self
 
     def to_hf(self):
-        '''Convert to RHF object.'''
-        from pyscf.pbc import scf
-        return self._transfer_attrs_(scf.ROHF(self.cell, self.kpt))
-
-
-if __name__ == '__main__':
-    from pyscf.pbc import gto
-    cell = gto.Cell()
-    cell.unit = 'A'
-    cell.atom = 'C 0.,  0.,  0.; C 0.8917,  0.8917,  0.8917'
-    cell.a = '''0.      1.7834  1.7834
-                1.7834  0.      1.7834
-                1.7834  1.7834  0.    '''
-
-    cell.basis = 'gth-szv'
-    cell.pseudo = 'gth-pade'
-    cell.verbose = 7
-    cell.output = '/dev/null'
-    cell.build()
-    mf = ROKS(cell)
-    print(mf.kernel())
+        '''Convert to KROHF object.'''
+        from pyscf.pbc import scf, df
+        out = self._transfer_attrs_(scf.KROHF(self.cell, self.kpts))
+        # Pure functionals only construct J-type integrals. Enable all integrals for KHF.
+        if (not self._numint.libxc.is_hybrid_xc(self.xc) and
+            len(self.kpts) > 1 and getattr(self.with_df, '_j_only', False)):
+            out.with_df._j_only = False
+            out.with_df.reset()
+        return out
+
+    to_gpu = lib.to_gpu
```

### Comparing `pyscf-2.5.0/pyscf/pbc/dft/uks.py` & `pyscf-2.6.0/pyscf/pbc/dft/uks.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,20 +48,20 @@
     if kpt is None: kpt = ks.kpt
     t0 = (logger.process_clock(), logger.perf_counter())
 
     ni = ks._numint
     hybrid = ni.libxc.is_hybrid_xc(ks.xc)
 
     if not hybrid and isinstance(ks.with_df, multigrid.MultiGridFFTDF):
-        if ks.nlc or ni.libxc.is_nlc(ks.xc):
+        if ks.do_nlc():
             raise NotImplementedError(f'MultiGrid for NLC functional {ks.xc} + {ks.nlc}')
         n, exc, vxc = multigrid.nr_uks(ks.with_df, ks.xc, dm, hermi,
                                        kpt.reshape(1,3), kpts_band,
                                        with_j=True, return_j=False)
-        logger.debug(ks, 'nelec by numeric integration = %s', n)
+        logger.info(ks, 'nelec by numeric integration = %s', n)
         t0 = logger.timer(ks, 'vxc', *t0)
         return vxc
 
     if not isinstance(dm, numpy.ndarray):
         dm = numpy.asarray(dm)
     if dm.ndim == 2:  # RHF DM
         dm = numpy.asarray((dm*.5,dm*.5))
@@ -72,25 +72,25 @@
 
     if hermi == 2:  # because rho = 0
         n, exc, vxc = (0,0), 0, 0
     else:
         max_memory = ks.max_memory - lib.current_memory()[0]
         n, exc, vxc = ni.nr_uks(cell, ks.grids, ks.xc, dm, 0, hermi,
                                 kpt, kpts_band, max_memory=max_memory)
-        if ks.nlc or ni.libxc.is_nlc(ks.xc):
+        if ks.do_nlc():
             if ni.libxc.is_nlc(ks.xc):
                 xc = ks.xc
             else:
                 assert ni.libxc.is_nlc(ks.nlc)
                 xc = ks.nlc
             n, enlc, vnlc = ni.nr_nlc_vxc(cell, ks.nlcgrids, xc, dm[0]+dm[1],
                                           0, hermi, kpt, max_memory=max_memory)
             exc += enlc
             vxc += vnlc
-        logger.debug(ks, 'nelec by numeric integration = %s', n)
+        logger.info(ks, 'nelec by numeric integration = %s', n)
         t0 = logger.timer(ks, 'vxc', *t0)
 
     if not hybrid:
         vj = ks.get_j(cell, dm[0]+dm[1], hermi, kpt, kpts_band)
         vxc += vj
     else:
         omega, alpha, hyb = ni.rsh_and_hybrid_coeff(ks.xc, spin=cell.spin)
@@ -140,14 +140,16 @@
         return self
 
     def to_hf(self):
         '''Convert to UHF object.'''
         from pyscf.pbc import scf
         return self._transfer_attrs_(scf.UHF(self.cell, self.kpt))
 
+    to_gpu = lib.to_gpu
+
 
 if __name__ == '__main__':
     from pyscf.pbc import gto
     cell = gto.Cell()
     cell.unit = 'A'
     cell.atom = 'C 0.,  0.,  0.; C 0.8917,  0.8917,  0.8917'
     cell.a = '''0.      1.7834  1.7834
```

### Comparing `pyscf-2.5.0/pyscf/pbc/eph/eph_fd.py` & `pyscf-2.6.0/pyscf/pbc/eph/eph_fd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/geomopt/__init__.py` & `pyscf-2.6.0/pyscf/pbc/geomopt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/geomopt/geometric_solver.py` & `pyscf-2.6.0/pyscf/pbc/geomopt/geometric_solver.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/grad/krhf.py` & `pyscf-2.6.0/pyscf/pbc/grad/krhf.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,18 @@
             hcore[:,kn,:,p0:p1] -= h1[kn,:,p0:p1].transpose(0,2,1).conj()
         return hcore
     return hcore_deriv
 
 def grad_nuc(cell, atmlst):
     '''
     Derivatives of nuclear repulsion energy wrt nuclear coordinates
+
+    Notes:
+        An optimized version of this function is available in
+        `pbc.gto.ewald_methods.ewald_nuc_grad`
     '''
     chargs = cell.atom_charges()
     ew_eta, ew_cut = cell.get_ewald_params()
     log_precision = np.log(cell.precision / (chargs.sum()*16*np.pi**2))
     ke_cutoff = -2*ew_eta**2*log_precision
     mesh = cell.cutoff_to_mesh(ke_cutoff)
     logger.debug1(cell, 'mesh for ewald %s', mesh)
@@ -240,20 +244,22 @@
                                      np.exp(-ew_eta**2 * r ** 2).reshape(len(r),1), axis = 0)
 
     Gv, Gvbase, weights = cell.get_Gv_weights(mesh)
     absG2 = np.einsum('gi,gi->g', Gv, Gv)
     absG2[absG2==0] = 1e200
     ewg_grad = np.zeros([natom,3])
     SI = cell.get_SI(Gv)
-    if cell.low_dim_ft_type is None or cell.dimension == 3:
+    if cell.dimension != 2 or cell.low_dim_ft_type == 'inf_vacuum':
         coulG = 4*np.pi / absG2
         coulG *= weights
         ZSI = np.einsum("i,ij->j", chargs, SI)
         ZexpG2 = coulG * np.exp(-absG2/(4*ew_eta**2))
         ZexpG2_mod = ZexpG2.reshape(len(ZexpG2),1) * Gv
+    else:
+        raise NotImplementedError
     for i, qi in enumerate(chargs):
         Zfac = np.imag(ZSI * SI[i].conj()) * qi
         ewg_grad[i] = - np.sum(Zfac.reshape((len(Zfac),1)) * ZexpG2_mod, axis = 0)
 
     ew_grad = ewg_grad + ewovrl_grad
     if atmlst is not None:
         ew_grad = ew_grad[atmlst]
```

### Comparing `pyscf-2.5.0/pyscf/pbc/grad/krks.py` & `pyscf-2.6.0/pyscf/pbc/grad/krks.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/grad/kuhf.py` & `pyscf-2.6.0/pyscf/pbc/grad/kuhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/grad/kuks.py` & `pyscf-2.6.0/pyscf/pbc/grad/kuks.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/__init__.py` & `pyscf-2.6.0/pyscf/pbc/gto/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,10 +18,11 @@
 #
 
 from pyscf.pbc.gto import cell
 from pyscf.pbc.gto import basis
 from pyscf.pbc.gto.basis import parse, load, parse_ecp, load_ecp
 from pyscf.pbc.gto import pseudo
 from pyscf.pbc.gto.cell import *
+from pyscf.pbc.gto.neighborlist import *
 
 parse_pp = parsepp = pseudo.parse
 load_pp = loadpp = pseudo.load
```

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/_pbcintor.py` & `pyscf-2.6.0/pyscf/pbc/gto/_pbcintor.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,31 +29,38 @@
         libpbc.PBCinit_optimizer(ctypes.byref(self._this),
                                  cell._atm.ctypes.data_as(ctypes.c_void_p), natm,
                                  cell._bas.ctypes.data_as(ctypes.c_void_p), nbas,
                                  cell._env.ctypes.data_as(ctypes.c_void_p))
 
     def init_rcut_cond(self, cell, precision=None):
         if precision is None: precision = cell.precision
-        rcut = numpy.array([cell.bas_rcut(ib, precision)
-                            for ib in range(cell.nbas)])
+        if cell.use_loose_rcut:
+            rcut = cell.rcut_by_shells(precision)
+            fn_set_rcut_cond = getattr(libpbc, 'PBCset_rcut_cond_loose')
+        else:
+            rcut = numpy.array([cell.bas_rcut(ib, precision)
+                                for ib in range(cell.nbas)])
+            fn_set_rcut_cond = getattr(libpbc, 'PBCset_rcut_cond')
+
         natm = ctypes.c_int(cell._atm.shape[0])
         nbas = ctypes.c_int(cell._bas.shape[0])
-        libpbc.PBCset_rcut_cond(self._this,
-                                rcut.ctypes.data_as(ctypes.c_void_p),
-                                cell._atm.ctypes.data_as(ctypes.c_void_p), natm,
-                                cell._bas.ctypes.data_as(ctypes.c_void_p), nbas,
-                                cell._env.ctypes.data_as(ctypes.c_void_p))
+        fn_set_rcut_cond(self._this,
+                         rcut.ctypes.data_as(ctypes.c_void_p),
+                         cell._atm.ctypes.data_as(ctypes.c_void_p), natm,
+                         cell._bas.ctypes.data_as(ctypes.c_void_p), nbas,
+                         cell._env.ctypes.data_as(ctypes.c_void_p))
         return self
 
     def del_rcut_cond(self):
         self._this.contents.fprescreen = _fpointer('PBCnoscreen')
         return self
 
     def __del__(self):
         try:
             libpbc.PBCdel_optimizer(ctypes.byref(self._this))
         except AttributeError:
             pass
 
 class _CPBCOpt(ctypes.Structure):
     _fields_ = [('rrcut', ctypes.c_void_p),
+                ('rcut', ctypes.c_void_p),
                 ('fprescreen', ctypes.c_void_p)]
```

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/__init__.py` & `pyscf-2.6.0/pyscf/pbc/gto/basis/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-aug-dzvp.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-aug-dzvp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-aug-qzv2p.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-aug-qzv2p.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-aug-qzv3p.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-aug-qzv3p.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-aug-tzv2p.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-aug-tzv2p.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-aug-tzvp.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-aug-tzvp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-cc-dzvp.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-cc-dzvp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-cc-qzvp.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-cc-qzvp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-cc-tzvp.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-cc-tzvp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-dzv.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-dzv.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-dzvp-molopt-sr-q9.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-dzvp-molopt-sr-q9.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-dzvp-molopt-sr.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-dzvp-molopt-sr.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-dzvp-molopt.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-dzvp-molopt.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-dzvp.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-dzvp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-qzv2p.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-qzv2p.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-qzv3p.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-qzv3p.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-szv-molopt-sr.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-szv-molopt-sr.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-szv-molopt.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-szv-molopt.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-szv.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-szv.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-szvp-molopt-sr-q9.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-szvp-molopt-sr-q9.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-tzv2p-molopt.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-tzv2p-molopt.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-tzv2p.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-tzv2p.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-tzv2px-molopt.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-tzv2px-molopt.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-tzvp-molopt.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-tzvp-molopt.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/gth-tzvp.dat` & `pyscf-2.6.0/pyscf/pbc/gto/basis/gth-tzvp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/split_BASIS_MOLOPT.py` & `pyscf-2.6.0/pyscf/pbc/gto/basis/split_BASIS_MOLOPT.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/split_GTH_BASIS_SETS.py` & `pyscf-2.6.0/pyscf/pbc/gto/basis/split_GTH_BASIS_SETS.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/basis/split_HFX_BASIS.py` & `pyscf-2.6.0/pyscf/pbc/gto/basis/split_HFX_BASIS.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/cell.py` & `pyscf-2.6.0/pyscf/pbc/gto/cell.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# Copyright 2014-2021 The PySCF Developers. All Rights Reserved.
+# Copyright 2014-2024 The PySCF Developers. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -37,14 +37,17 @@
 from pyscf import __config__
 
 INTEGRAL_PRECISION = getattr(__config__, 'pbc_gto_cell_Cell_precision', 1e-8)
 WRAP_AROUND = getattr(__config__, 'pbc_gto_cell_make_kpts_wrap_around', False)
 WITH_GAMMA = getattr(__config__, 'pbc_gto_cell_make_kpts_with_gamma', True)
 EXP_DELIMITER = getattr(__config__, 'pbc_gto_cell_split_basis_exp_delimiter',
                         [1.0, 0.5, 0.25, 0.1, 0])
+# defined in lib/pbc/cell.h
+RCUT_EPS = 1e-3
+RCUT_MAX_CYCLE = 10
 
 libpbc = _pbcintor.libpbc
 
 def M(*args, **kwargs):
     r'''This is a shortcut to build up Cell object.
 
     Examples:
@@ -277,14 +280,97 @@
             v = v.real
         mat.append(v)
 
     if kpts is None or np.shape(kpts) == (3,):  # A single k-point
         mat = mat[0]
     return mat
 
+def _intor_cross_screened(
+        intor, cell1, cell2, comp=None, hermi=0, kpts=None, kpt=None,
+        shls_slice=None, **kwargs):
+    '''`intor_cross` with prescreening.
+
+    Notes:
+         This function may be subject to change.
+    '''
+    from pyscf.pbc.gto.neighborlist import NeighborListOpt
+    intor, comp = moleintor._get_intor_and_comp(cell1._add_suffix(intor), comp)
+
+    if kpts is None:
+        if kpt is not None:
+            kpts_lst = np.reshape(kpt, (1,3))
+        else:
+            kpts_lst = np.zeros((1,3))
+    else:
+        kpts_lst = np.reshape(kpts, (-1,3))
+    nkpts = len(kpts_lst)
+
+    pcell = cell1.copy(deep=False)
+    pcell.precision = min(cell1.precision, cell2.precision)
+    pcell._atm, pcell._bas, pcell._env = \
+            atm, bas, env = conc_env(cell1._atm, cell1._bas, cell1._env,
+                                     cell2._atm, cell2._bas, cell2._env)
+    if shls_slice is None:
+        shls_slice = (0, cell1.nbas, 0, cell2.nbas)
+    i0, i1, j0, j1 = shls_slice[:4]
+    j0 += cell1.nbas
+    j1 += cell1.nbas
+    ao_loc = moleintor.make_loc(bas, intor)
+    ni = ao_loc[i1] - ao_loc[i0]
+    nj = ao_loc[j1] - ao_loc[j0]
+    out = np.empty((nkpts,comp,ni,nj), dtype=np.complex128)
+
+    if hermi == 0:
+        aosym = 's1'
+    else:
+        aosym = 's2'
+    fill = getattr(libpbc, 'PBCnr2c_screened_fill_k'+aosym)
+    fintor = getattr(moleintor.libcgto, intor)
+    drv = libpbc.PBCnr2c_screened_drv
+
+    rcut = max(cell1.rcut, cell2.rcut)
+    Ls = cell1.get_lattice_Ls(rcut=rcut)
+    expkL = np.asarray(np.exp(1j*np.dot(kpts_lst, Ls.T)), order='C')
+
+    neighbor_list = kwargs.get('neighbor_list', None)
+    if neighbor_list is None:
+        nlopt = NeighborListOpt(cell1)
+        nlopt.build(cell1, cell2, Ls, set_optimizer=False)
+        neighbor_list = nlopt.nl
+
+    cintopt = lib.c_null_ptr()
+
+    drv(fintor, fill, out.ctypes.data_as(ctypes.c_void_p),
+        ctypes.c_int(nkpts), ctypes.c_int(comp), ctypes.c_int(len(Ls)),
+        Ls.ctypes.data_as(ctypes.c_void_p),
+        expkL.ctypes.data_as(ctypes.c_void_p),
+        (ctypes.c_int*4)(i0, i1, j0, j1),
+        ao_loc.ctypes.data_as(ctypes.c_void_p), cintopt,
+        atm.ctypes.data_as(ctypes.c_void_p), ctypes.c_int(pcell.natm),
+        bas.ctypes.data_as(ctypes.c_void_p), ctypes.c_int(pcell.nbas),
+        env.ctypes.data_as(ctypes.c_void_p), ctypes.c_int(env.size),
+        ctypes.byref(neighbor_list))
+
+    nlopt = None
+
+    mat = []
+    for k, kpt in enumerate(kpts_lst):
+        v = out[k]
+        if hermi != 0:
+            for ic in range(comp):
+                lib.hermi_triu(v[ic], hermi=hermi, inplace=True)
+        if comp == 1:
+            v = v[0]
+        if abs(kpt).sum() < 1e-9:  # gamma_point
+            v = v.real
+        mat.append(v)
+
+    if kpts is None or np.shape(kpts) == (3,):  # A single k-point
+        mat = mat[0]
+    return mat
 
 def get_nimgs(cell, precision=None):
     r'''Choose number of basis function images in lattice sums
     to include for given precision in overlap, using
 
     precision ~ \int r^l e^{-\alpha r^2} (r-rcut)^l e^{-\alpha (r-rcut)^2}
     ~ (rcut^2/(2\alpha))^l e^{\alpha/2 rcut^2}
@@ -335,14 +421,17 @@
 
 def estimate_rcut(cell, precision=None):
     '''Lattice-sum cutoff for the entire system'''
     if cell.nbas == 0:
         return 0.01
     if precision is None:
         precision = cell.precision
+    if cell.use_loose_rcut:
+        return cell.rcut_by_shells(precision).max()
+
     exps, cs = _extract_pgto_params(cell, 'min')
     ls = cell._bas[:,mole.ANG_OF]
     rcut = _estimate_rcut(exps, ls, cs, precision)
     return rcut.max()
 
 def _estimate_ke_cutoff(alpha, l, c, precision=INTEGRAL_PRECISION, omega=0):
     '''Energy cutoff estimation for nuclear attraction integrals'''
@@ -487,41 +576,63 @@
             area = np.linalg.norm(np.cross(b[0], b[1]))
             wxy = np.repeat(area, mesh[0]*mesh[1])
             rz, wz = _non_uniform_Gv_base(mesh[2]//2)
             rz /= np.linalg.norm(b[2])
             weights = np.einsum('i,k->ik', wxy, wz).reshape(-1)
 
     Gvbase = (rx, ry, rz)
-    Gv = np.dot(lib.cartesian_prod(Gvbase), b)
+
+    #:Gv = np.dot(lib.cartesian_prod(Gvbase), b)
+    # NOTE mesh can be different from the input mesh
+    mesh = np.asarray((len(rx),len(ry),len(rz)), dtype=np.int32)
+    Gv = np.empty((*mesh,3), order='C', dtype=float)
+    b = np.asarray(b, order='C')
+    rx = np.asarray(rx, order='C')
+    ry = np.asarray(ry, order='C')
+    rz = np.asarray(rz, order='C')
+    fn = libpbc.get_Gv
+    fn(Gv.ctypes.data_as(ctypes.c_void_p),
+       rx.ctypes.data_as(ctypes.c_void_p),
+       ry.ctypes.data_as(ctypes.c_void_p),
+       rz.ctypes.data_as(ctypes.c_void_p),
+       mesh.ctypes.data_as(ctypes.c_void_p),
+       b.ctypes.data_as(ctypes.c_void_p))
+    Gv = Gv.reshape(-1, 3)
+
     # 1/cell.vol == det(b)/(2pi)^3
     weights *= 1/(2*np.pi)**3
     return Gv, Gvbase, weights
 
 def _non_uniform_Gv_base(n):
     #rs, ws = radi.delley(n)
     #rs, ws = radi.treutler_ahlrichs(n)
     #rs, ws = radi.mura_knowles(n)
     rs, ws = radi.gauss_chebyshev(n)
     #return np.hstack((0,rs,-rs[::-1])), np.hstack((0,ws,ws[::-1]))
     return np.hstack((rs,-rs[::-1])), np.hstack((ws,ws[::-1]))
 
-def get_SI(cell, Gv=None, mesh=None):
+def get_SI(cell, Gv=None, mesh=None, atmlst=None):
     '''Calculate the structure factor (0D, 1D, 2D, 3D) for all atoms; see MH (3.34).
 
     Args:
         cell : instance of :class:`Cell`
 
         Gv : (N,3) array
             G vectors
 
+        atmlst : list of ints, optional
+            Indices of atoms for which the structure factors are computed.
+
     Returns:
         SI : (natm, ngrids) ndarray, dtype=np.complex128
             The structure factor for each atom at each G-vector.
     '''
     coords = cell.atom_coords()
+    if atmlst is not None:
+        coords = coords[np.asarray(atmlst)]
     if Gv is None:
         if mesh is None:
             mesh = cell.mesh
         basex, basey, basez = cell.get_Gv_weights(mesh)[1]
         b = cell.reciprocal_vectors()
         rb = np.dot(coords, b.T)
         SIx = np.exp(-1j*np.einsum('z,g->zg', rb[:,0], basex))
@@ -594,14 +705,18 @@
     # object. The nuclear repulsion energy is computed.
     if cell.a is None:
         return mole.energy_nuc(cell)
 
     if cell.natm == 0:
         return 0
 
+    if cell.dimension == 3 and cell.use_particle_mesh_ewald:
+        from pyscf.pbc.gto import ewald_methods
+        return ewald_methods.particle_mesh_ewald(cell, ew_eta, ew_cut)
+
     chargs = cell.atom_charges()
 
     if ew_eta is None or ew_cut is None:
         ew_eta, ew_cut = cell.get_ewald_params()
     log_precision = np.log(cell.precision / (chargs.sum()*16*np.pi**2))
     ke_cutoff = -2*ew_eta**2*log_precision
     mesh = cell.cutoff_to_mesh(ke_cutoff)
@@ -635,15 +750,24 @@
     absG2[absG2==0] = 1e200
 
     if cell.dimension != 2 or cell.low_dim_ft_type == 'inf_vacuum':
         # TODO: truncated Coulomb for 0D. The non-uniform grids for inf-vacuum
         # have relatively large error
         coulG = 4*np.pi / absG2
         coulG *= weights
-        ZSI = np.einsum("i,ij->j", chargs, cell.get_SI(Gv))
+
+        #:ZSI = np.einsum('i,ij->j', chargs, cell.get_SI(Gv))
+        ngrids = len(Gv)
+        ZSI = np.empty((ngrids,), dtype=np.complex128)
+        mem_avail = cell.max_memory - lib.current_memory()[0]
+        blksize = int((mem_avail*1e6 - cell.natm*24)/((3+cell.natm*2)*8))
+        blksize = min(ngrids, max(mesh[2], blksize))
+        for ig0, ig1 in lib.prange(0, ngrids, blksize):
+            np.einsum('i,ij->j', chargs, cell.get_SI(Gv[ig0:ig1]), out=ZSI[ig0:ig1])
+
         ZexpG2 = ZSI * np.exp(-absG2/(4*ew_eta**2))
         ewg = .5 * np.einsum('i,i,i', ZSI.conj(), ZexpG2, coulG).real
 
     elif cell.dimension == 2:  # Truncated Coulomb
         # The following 2D ewald summation is taken from:
         # R. Sundararaman and T. Arias PRB 87, 2013
         def fn(eta,Gnorm,z):
@@ -831,14 +955,67 @@
 
 def _mesh_inf_vaccum(cell):
     #prec ~ exp(-0.436392335*mesh -2.99944305)*nelec
     meshz = (np.log(cell.nelectron/cell.precision)-2.99944305)/0.436392335
     # meshz has to be even number due to the symmetry on z+ and z-
     return int(meshz*.5 + .999) * 2
 
+def pgf_rcut(l, alpha, coeff, precision=INTEGRAL_PRECISION,
+             rcut=0, max_cycle=RCUT_MAX_CYCLE, eps=RCUT_EPS):
+    '''Estimate the cutoff radii of primitive Gaussian functions
+    based on their values in real space:
+    `c*rcut^(l+2)*exp(-alpha*rcut^2) ~ precision`.
+    '''
+    c = np.log(coeff / precision)
+
+    rmin = np.sqrt(.5 * (l+2) / alpha) * 2
+    eps = np.minimum(rmin/10, eps)
+    rcut = np.maximum(rcut, rmin+eps)
+    for i in range(max_cycle):
+        rcut_last = rcut
+        rcut = np.sqrt(((l+2) * np.log(rcut) + c) / alpha)
+        if np.all(abs(rcut - rcut_last) < eps):
+            return rcut
+    warnings.warn(f'cell.pgf_rcut failed to converge in {max_cycle} cycles.')
+    return rcut
+
+def rcut_by_shells(cell, precision=None, rcut=0,
+                   return_pgf_radius=False):
+    '''Compute shell and primitive gaussian function radii.
+    '''
+    # TODO the internal implementation loops over all shells,
+    # which can be optimized to loop over atom types.
+    if precision is None:
+        precision = cell.precision
+
+    bas = np.asarray(cell._bas, order='C')
+    env = np.asarray(cell._env, order='C')
+    nbas = len(bas)
+    shell_radius = np.empty((nbas,), order='C', dtype=float)
+    if return_pgf_radius:
+        nprim = bas[:,mole.NPRIM_OF].max()
+        # be careful that the unused memory blocks are not initialized
+        pgf_radius = np.empty((nbas,nprim), order='C', dtype=np.double)
+        ptr_pgf_radius = lib.ndarray_pointer_2d(pgf_radius).ctypes
+    else:
+        ptr_pgf_radius = lib.c_null_ptr()
+    fn = getattr(libpbc, 'rcut_by_shells', None)
+    try:
+        fn(shell_radius.ctypes.data_as(ctypes.c_void_p),
+           ptr_pgf_radius,
+           bas.ctypes.data_as(ctypes.c_void_p),
+           env.ctypes.data_as(ctypes.c_void_p),
+           ctypes.c_int(nbas), ctypes.c_double(rcut),
+           ctypes.c_double(precision))
+    except Exception as e:
+        raise RuntimeError(f'Failed to get shell radii.\n{e}')
+    if return_pgf_radius:
+        return shell_radius, pgf_radius
+    return shell_radius
+
 
 class Cell(mole.MoleBase):
     '''A Cell object holds the basic information of a crystal.
 
     Attributes:
         a : (3,3) ndarray
             Lattice primitive vectors. Each row represents a lattice vector
@@ -860,14 +1037,22 @@
             Periodic dimensions. Default is 3
         low_dim_ft_type : str
             For semi-empirical periodic systems, whether to calculate
             integrals at the non-PBC dimension using the sampled mesh grids in
             infinity vacuum (inf_vacuum) or truncated Coulomb potential
             (analytic_2d_1). Unless explicitly specified, analytic_2d_1 is
             used for 2D system and inf_vacuum is assumed for 1D and 0D.
+        use_loose_rcut : bool
+            If set to True, a loose `rcut` determined by shell radius is used,
+            which is usually accurate enough for pure DFT calculations;
+            otherwise, a tight `rcut` determined by overlap integral is used.
+            Default value is False. Has no effect if `rcut` is set manually.
+        use_particle_mesh_ewald : bool
+            If set to True, use particle-mesh Ewald to compute the nuclear repulsion.
+            Default value is False, meaning to use classical Ewald summation.
         space_group_symmetry : bool
             Whether to consider space group symmetry. Default is False.
         symmorphic : bool
             Whether the lattice is symmorphic. If set to True, even if the
             lattice is non-symmorphic, only symmorphic space group symmetry
             will be considered. Default is False, meaning the space group is
             determined by the lattice symmetry to be symmorphic or non-symmorphic.
@@ -888,28 +1073,31 @@
     precision = getattr(__config__, 'pbc_gto_cell_Cell_precision', 1e-8)
     exp_to_discard = getattr(__config__, 'pbc_gto_cell_Cell_exp_to_discard', None)
 
     _keys = {
         'precision', 'exp_to_discard',
         'a', 'ke_cutoff', 'pseudo', 'dimension', 'low_dim_ft_type',
         'space_group_symmetry', 'symmorphic', 'lattice_symmetry', 'mesh', 'rcut',
+        'use_loose_rcut', 'use_particle_mesh_ewald',
     }
 
     def __init__(self, **kwargs):
         mole.MoleBase.__init__(self)
         self.a = None # lattice vectors, (a1,a2,a3)
         # if set, defines a spherical cutoff
         # of fourier components, with .5 * G**2 < ke_cutoff
         self.ke_cutoff = None
 
         self.dimension = 3
         # TODO: Simple hack for now; the implementation of ewald depends on the
         #       density-fitting class.  This determines how the ewald produces
         #       its energy.
         self.low_dim_ft_type = None
+        self.use_loose_rcut = False
+        self.use_particle_mesh_ewald = False
         self.space_group_symmetry = False
         self.symmorphic = False
         self.lattice_symmetry = None
 
 ##################################################
 # These attributes are initialized by build function if not specified
         self.mesh = None
@@ -965,20 +1153,19 @@
         return nalpha, nbeta
 
     def __getattr__(self, key):
         '''To support accessing methods (cell.HF, cell.KKS, cell.KUCCSD, ...)
         from Cell object.
         '''
         if key[0] == '_':  # Skip private attributes and Python builtins
-            raise AttributeError('Cell object does not have attribute %s' % key)
-        elif key in ('_ipython_canary_method_should_not_exist_',
-                     '_repr_mimebundle_'):
-            # https://github.com/mewwts/addict/issues/26
-            # https://github.com/jupyter/notebook/issues/2014
-            raise AttributeError(f'Cell object has no attribute {key}')
+            # https://bugs.python.org/issue45985
+            # https://github.com/python/cpython/issues/103936
+            # @property and __getattr__ conflicts. As a temporary fix, call
+            # object.__getattribute__ method to re-raise AttributeError
+            return object.__getattribute__(self, key)
 
         # Import all available modules. Some methods are registered to other
         # classes/modules when importing modules in __all__.
         from pyscf.pbc import __all__  # noqa
         from pyscf.pbc import scf, dft
         from pyscf.dft import XC
 
@@ -996,15 +1183,15 @@
                     xc = key.split('TD', 1)[1]
                     if xc in XC:
                         mf.xc = xc
                         key = 'KTDDFT'
             elif 'CI' in key or 'CC' in key or 'MP' in key:
                 mf = scf.KHF(self)
             else:
-                raise AttributeError(f'Cell object has no attribute {key}')
+                return object.__getattribute__(self, key)
             # Remove prefix 'K' because methods are registered without the leading 'K'
             key = key[1:]
         else:
             if 'TD' in key[:3]:
                 if key in ('TDHF', 'TDA'):
                     mf = scf.HF(self)
                 else:
@@ -1012,15 +1199,15 @@
                     xc = key.split('TD', 1)[1]
                     if xc in XC:
                         mf.xc = xc
                         key = 'TDDFT'
             elif 'CI' in key or 'CC' in key or 'MP' in key:
                 mf = scf.HF(self)
             else:
-                raise AttributeError(f'Cell object has no attribute {key}')
+                return object.__getattribute__(self, key)
 
         method = getattr(mf, key)
 
         if self.nelectron != 0:
             mf.run()
         return method
 
@@ -1078,15 +1265,17 @@
             self._mesh_from_build = _mesh_from_build
         return self
 
 #Note: Exculde dump_input, parse_arg, basis from kwargs to avoid parsing twice
     def build(self, dump_input=True, parse_arg=mole.ARGPARSE,
               a=None, mesh=None, ke_cutoff=None, precision=None, nimgs=None,
               h=None, dimension=None, rcut= None, low_dim_ft_type=None,
-              space_group_symmetry=None, symmorphic=None, *args, **kwargs):
+              space_group_symmetry=None, symmorphic=None,
+              use_loose_rcut=None, use_particle_mesh_ewald=None,
+              *args, **kwargs):
         '''Setup Mole molecule and Cell and initialize some control parameters.
         Whenever you change the value of the attributes of :class:`Cell`,
         you need call this function to refresh the internal data of Cell.
 
         Kwargs:
             a : (3,3) ndarray
                 The real-space cell lattice vectors. Each row represents
@@ -1129,14 +1318,18 @@
         if mesh is not None: self.mesh = mesh
         if nimgs is not None: self.nimgs = nimgs
         if dimension is not None: self.dimension = dimension
         if precision is not None: self.precision = precision
         if rcut is not None: self.rcut = rcut
         if ke_cutoff is not None: self.ke_cutoff = ke_cutoff
         if low_dim_ft_type is not None: self.low_dim_ft_type = low_dim_ft_type
+        if use_loose_rcut is not None:
+            self.use_loose_rcut = use_loose_rcut
+        if use_particle_mesh_ewald is not None:
+            self.use_particle_mesh_ewald = use_particle_mesh_ewald
         if space_group_symmetry is not None:
             self.space_group_symmetry = space_group_symmetry
         if symmorphic is not None:
             self.symmorphic = symmorphic
 
         dump_input = dump_input and not self._built and self.verbose > logger.NOTE
         mole.MoleBase.build(self, dump_input, parse_arg, *args, **kwargs)
@@ -1261,15 +1454,15 @@
             logger.info(self, '                 a2 [%.9f, %.9f, %.9f]', *_a[1])
             logger.info(self, '                 a3 [%.9f, %.9f, %.9f]', *_a[2])
             logger.info(self, 'dimension = %s', self.dimension)
             logger.info(self, 'low_dim_ft_type = %s', self.low_dim_ft_type)
             logger.info(self, 'Cell volume = %g', self.vol)
             # Check atoms coordinates
             if self.dimension > 0 and self.natm > 0:
-                scaled_atom_coords = np.linalg.solve(_a.T, self.atom_coords().T).T
+                scaled_atom_coords = self.get_scaled_atom_coords(_a)
                 atom_boundary_max = scaled_atom_coords[:,:self.dimension].max(axis=0)
                 atom_boundary_min = scaled_atom_coords[:,:self.dimension].min(axis=0)
                 if (np.any(atom_boundary_max > 1) or np.any(atom_boundary_min < -1)):
                     logger.warn(self, 'Atoms found out of the primitive cell.')
 
             if self.exp_to_discard is not None:
                 logger.info(self, 'exp_to_discard = %s', self.exp_to_discard)
@@ -1363,21 +1556,20 @@
             if is_au(self.unit):
                 return a
             else:
                 return a/param.BOHR
         else:
             return a/self.unit
 
-    def get_scaled_positions(self):
-        ''' Get scaled atom positions.
+    def get_scaled_atom_coords(self, a=None):
+        ''' Get scaled atomic coordinates.
         '''
-        a = self.lattice_vectors()
-        atm_pos = self.atom_coords()
-        scaled_atm_pos = np.dot(atm_pos,np.linalg.inv(a))
-        return scaled_atm_pos
+        if a is None:
+            a = self.lattice_vectors()
+        return np.dot(self.atom_coords(), np.linalg.inv(a))
 
     def reciprocal_vectors(self, norm_to=2*np.pi):
         r'''
         .. math::
 
             \begin{align}
             \mathbf{b_1} &= 2\pi \frac{\mathbf{a_2} \times \mathbf{a_3}}{\mathbf{a_1} \cdot (\mathbf{a_2} \times \mathbf{a_3})} \\
@@ -1471,14 +1663,15 @@
 
     @lib.with_doc(unpack.__doc__)
     def loads_(self, molstr):
         self.__dict__.update(loads(molstr).__dict__)
         return self
 
     bas_rcut = bas_rcut
+    rcut_by_shells = rcut_by_shells
 
     get_lattice_Ls = pbctools.get_lattice_Ls
 
     get_nimgs = get_nimgs
 
     get_ewald_params = get_ewald_params
 
@@ -1507,14 +1700,18 @@
         See also Mole.intor
         '''
         if not self._built:
             logger.warn(self, 'Warning: intor envs of %s not initialized.', self)
             # FIXME: Whether to check _built and call build?  ._bas and .basis
             # may not be consistent. calling .build() may leads to wrong intor env.
             #self.build(False, False)
+        if self.use_loose_rcut:
+            return _intor_cross_screened(
+                            intor, self, self, comp, hermi, kpts, kpt,
+                            shls_slice, **kwargs)
         return intor_cross(intor, self, self, comp, hermi, kpts, kpt,
                            shls_slice, **kwargs)
 
     pbc_eval_ao = pbc_eval_gto = pbc_eval_gto
 
     @lib.with_doc(pbc_eval_gto.__doc__)
     def eval_gto(self, eval_name, coords, comp=None, kpts=None, kpt=None,
@@ -1547,12 +1744,13 @@
         '''
         #FIXME: should cell be converted to mole object?  If cell is converted
         # and a mole object is returned, many attributes (e.g. the GTH basis,
         # gth-PP) will not be recognized by mole.build function.
         mol = self.view(mole.Mole)
         delattr(mol, 'a')
         delattr(mol, '_mesh')
+        mol.enuc = None #reset nuclear energy
         if mol.symmetry:
             mol._build_symmetry()
         return mol
 
 del (INTEGRAL_PRECISION, WRAP_AROUND, WITH_GAMMA, EXP_DELIMITER)
```

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/ecp.py` & `pyscf-2.6.0/pyscf/pbc/gto/ecp.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/eval_gto.py` & `pyscf-2.6.0/pyscf/pbc/gto/eval_gto.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/pseudo/__init__.py` & `pyscf-2.6.0/pyscf/pbc/gto/pseudo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-blyp.dat` & `pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-blyp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-bp.dat` & `pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-bp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-hcth120.dat` & `pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-hcth120.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-hcth407.dat` & `pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-hcth407.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-hf-rev.dat` & `pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-hf-rev.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-hf.dat` & `pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-hf.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-olyp.dat` & `pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-olyp.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-pade.dat` & `pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-pade.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-pbe.dat` & `pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-pbe.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/pseudo/gth-pbesol.dat` & `pyscf-2.6.0/pyscf/pbc/gto/pseudo/gth-pbesol.dat`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/pseudo/pp.py` & `pyscf-2.6.0/pyscf/pbc/gto/pseudo/pp.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gto/pseudo/split_GTH_POTENTIALS.py` & `pyscf-2.6.0/pyscf/pbc/gto/pseudo/split_GTH_POTENTIALS.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gw/__init__.py` & `pyscf-2.6.0/pyscf/pbc/gw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gw/gw_slow.py` & `pyscf-2.6.0/pyscf/pbc/gw/gw_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gw/kgw_slow.py` & `pyscf-2.6.0/pyscf/pbc/gw/kgw_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gw/kgw_slow_supercell.py` & `pyscf-2.6.0/pyscf/pbc/gw/kgw_slow_supercell.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gw/krgw_ac.py` & `pyscf-2.6.0/pyscf/pbc/gw/krgw_ac.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gw/krgw_cd.py` & `pyscf-2.6.0/pyscf/pbc/gw/krgw_cd.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/gw/kugw_ac.py` & `pyscf-2.6.0/pyscf/pbc/gw/kugw_ac.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/lib/__init__.py` & `pyscf-2.6.0/pyscf/pbc/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/lib/arnoldi.py` & `pyscf-2.6.0/pyscf/pbc/lib/arnoldi.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/lib/chkfile.py` & `pyscf-2.6.0/pyscf/pbc/lib/chkfile.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/lib/kpts.py` & `pyscf-2.6.0/pyscf/pbc/lib/kpts.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/lib/kpts_helper.py` & `pyscf-2.6.0/pyscf/pbc/lib/kpts_helper.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/lib/ktensor.py` & `pyscf-2.6.0/pyscf/pbc/lib/ktensor.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/lib/linalg_helper.py` & `pyscf-2.6.0/pyscf/pbc/lib/linalg_helper.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/mp/__init__.py` & `pyscf-2.6.0/pyscf/pbc/mp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/mp/kmp2.py` & `pyscf-2.6.0/pyscf/pbc/mp/kmp2.py`

 * *Files 1% similar despite different names*

```diff
@@ -779,14 +779,16 @@
         self.e_corr_os = getattr(self.e_corr, 'e_corr_os', 0)
         self.e_corr = float(self.e_corr)
 
         self._finalize()
 
         return self.e_corr, self.t2
 
+    to_gpu = lib.to_gpu
+
 KRMP2 = KMP2
 
 
 from pyscf.pbc import scf
 scf.khf.KRHF.MP2 = lib.class_as_method(KRMP2)
 scf.kghf.KGHF.MP2 = None
 scf.krohf.KROHF.MP2 = None
```

### Comparing `pyscf-2.5.0/pyscf/pbc/mp/kmp2_ksymm.py` & `pyscf-2.6.0/pyscf/pbc/mp/kmp2_ksymm.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/mp/kmp2_stagger.py` & `pyscf-2.6.0/pyscf/pbc/mp/kmp2_stagger.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/mp/kump2.py` & `pyscf-2.6.0/pyscf/pbc/mp/kump2.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/mp/mp2.py` & `pyscf-2.6.0/pyscf/pbc/mp/mp2.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/mpicc/__init__.py` & `pyscf-2.6.0/pyscf/pbc/mpicc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/mpicc/kccsd_rhf.py` & `pyscf-2.6.0/pyscf/pbc/mpicc/kccsd_rhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/mpicc/kintermediates_rhf.py` & `pyscf-2.6.0/pyscf/pbc/mpicc/kintermediates_rhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/mpicc/mpi_kpoint_helper.py` & `pyscf-2.6.0/pyscf/pbc/mpicc/mpi_kpoint_helper.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/mpitools/__init__.py` & `pyscf-2.6.0/pyscf/pbc/mpitools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/mpitools/mpi.py` & `pyscf-2.6.0/pyscf/pbc/mpitools/mpi.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/mpitools/mpi_blksize.py` & `pyscf-2.6.0/pyscf/pbc/mpitools/mpi_blksize.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/mpitools/mpi_helper.py` & `pyscf-2.6.0/pyscf/pbc/mpitools/mpi_helper.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/mpitools/mpi_load_balancer.py` & `pyscf-2.6.0/pyscf/pbc/mpitools/mpi_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/mpitools/mpi_pool.py` & `pyscf-2.6.0/pyscf/pbc/mpitools/mpi_pool.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/__init__.py` & `pyscf-2.6.0/pyscf/pbc/scf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/_response_functions.py` & `pyscf-2.6.0/pyscf/pbc/scf/_response_functions.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/addons.py` & `pyscf-2.6.0/pyscf/pbc/scf/addons.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,20 +117,25 @@
                 mo_energy_kpts = (mo_energy_kpts, mo_energy_kpts)
             mo_es = [numpy.hstack(mo_energy_kpts[0]),
                      numpy.hstack(mo_energy_kpts[1])]
             nocc = self.nelec
             if self.mu0 is None:
                 mu_a, occa = mol_addons._smearing_optimize(f_occ, mo_es[0], nocc[0], sigma)
                 mu_b, occb = mol_addons._smearing_optimize(f_occ, mo_es[1], nocc[1], sigma)
-                mu = [mu_a, mu_b]
-                mo_occs = [occa, occb]
             else:
-                mu = self.mu0
-                mo_occs = f_occ(mu[0], mo_es[0], sigma)
-                mo_occs = f_occ(mu[1], mo_es[1], sigma)
+                if numpy.isscalar(self.mu0):
+                    mu_a = mu_b = self.mu0
+                elif len(self.mu0) == 2:
+                    mu_a, mu_b = self.mu0
+                else:
+                    raise TypeError(f'Unsupported mu0: {self.mu0}')
+                occa = f_occ(mu_a, mo_es[0], sigma)
+                occb = f_occ(mu_b, mo_es[1], sigma)
+            mu = [mu_a, mu_b]
+            mo_occs = [occa, occb]
             self.entropy  = self._get_entropy(mo_es[0], mo_occs[0], mu[0])
             self.entropy += self._get_entropy(mo_es[1], mo_occs[1], mu[1])
             self.entropy /= nkpts
 
             fermi = (mol_addons._get_fermi(mo_es[0], nocc[0]),
                      mol_addons._get_fermi(mo_es[1], nocc[1]))
             logger.debug(self, '    Alpha-spin Fermi level %g  Sum mo_occ_kpts = %s  should equal nelec = %s',
@@ -159,14 +164,15 @@
                 nocc = (nelectron + 1) // 2
 
             if self.mu0 is None:
                 mu, mo_occs = mol_addons._smearing_optimize(f_occ, mo_es, nocc, sigma)
             else:
                 # If mu0 is given, fix mu instead of electron number. XXX -Chong Sun
                 mu = self.mu0
+                assert numpy.isscalar(mu)
                 mo_occs = f_occ(mu, mo_es, sigma)
             self.entropy = self._get_entropy(mo_es, mo_occs, mu) / nkpts
             if is_rhf:
                 mo_occs *= 2
                 self.entropy *= 2
 
             fermi = mol_addons._get_fermi(mo_es, nocc)
```

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/chkfile.py` & `pyscf-2.6.0/pyscf/pbc/scf/chkfile.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/cphf.py` & `pyscf-2.6.0/pyscf/pbc/scf/cphf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/ghf.py` & `pyscf-2.6.0/pyscf/pbc/scf/ghf.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,16 @@
         return self._transfer_attrs_(dft.GKS(self.cell, self.kpt, xc=xc))
 
     def convert_from_(self, mf):
         '''Convert given mean-field object to GHF'''
         addons.convert_to_ghf(mf, self)
         return self
 
+    to_gpu = lib.to_gpu
+
 
 if __name__ == '__main__':
     from pyscf.pbc import gto
     from pyscf.pbc import scf
 
     cell = gto.Cell()
     cell.atom = '''
```

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/hf.py` & `pyscf-2.6.0/pyscf/pbc/scf/hf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# Copyright 2014-2019 The PySCF Developers. All Rights Reserved.
+# Copyright 2014-2024 The PySCF Developers. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -49,31 +49,32 @@
     '''
     precision = cell.precision * 1e-5
     rcut = max(cell.rcut, gto.estimate_rcut(cell, precision))
     with lib.temporary_env(cell, rcut=rcut, precision=precision):
         # Avoid pbcopt's prescreening in the lattice sum, for better accuracy
         s = cell.pbc_intor('int1e_ovlp', hermi=0, kpts=kpt,
                            pbcopt=lib.c_null_ptr())
-    s = lib.asarray(s)
+    s = np.asarray(s)
     hermi_error = abs(s - np.rollaxis(s.conj(), -1, -2)).max()
     if hermi_error > cell.precision and hermi_error > 1e-12:
         logger.warn(cell, '%.4g error found in overlap integrals. '
                     'cell.precision  or  cell.rcut  can be adjusted to '
                     'improve accuracy.', hermi_error)
 
-    cond = np.max(lib.cond(s))
-    if cond * precision > 1e2:
-        prec = 1e7 / cond
-        rmin = gto.estimate_rcut(cell, prec*1e-5)
-        logger.warn(cell, 'Singularity detected in overlap matrix.  '
-                    'Integral accuracy may be not enough.\n      '
-                    'You can adjust  cell.precision  or  cell.rcut  to '
-                    'improve accuracy.  Recommended settings are\n      '
-                    'cell.precision < %.2g\n      '
-                    'cell.rcut > %.4g', prec, rmin)
+    if cell.verbose >= logger.DEBUG:
+        cond = np.max(lib.cond(s))
+        if cond * precision > 1e2:
+            prec = 1e7 / cond
+            rmin = gto.estimate_rcut(cell, prec*1e-5)
+            logger.warn(cell, 'Singularity detected in overlap matrix.  '
+                        'Integral accuracy may be not enough.\n      '
+                        'You can adjust  cell.precision  or  cell.rcut  to '
+                        'improve accuracy.  Recommended settings are\n      '
+                        'cell.precision < %.2g\n      '
+                        'cell.rcut > %.4g', prec, rmin)
     return s
 
 
 def get_hcore(cell, kpt=np.zeros(3)):
     '''Get the core Hamiltonian AO matrix.
     '''
     hcore = get_t(cell, kpt)
@@ -611,19 +612,26 @@
         logger.info(self, 'DF object = %s', self.with_df)
         if not getattr(self.with_df, 'build', None):
             # .dump_flags() is called in pbc.df.build function
             self.with_df.dump_flags(verbose)
         return self
 
     def check_sanity(self):
-        mol_hf.SCF.check_sanity(self)
+        lib.StreamObject.check_sanity(self)
         if (isinstance(self.exxdiv, str) and self.exxdiv.lower() != 'ewald' and
             isinstance(self.with_df, df.df.DF)):
             logger.warn(self, 'exxdiv %s is not supported in DF or MDF',
                         self.exxdiv)
+
+        if self.verbose >= logger.DEBUG:
+            s = self.get_ovlp()
+            cond = np.max(lib.cond(s))
+            if cond * 1e-17 > self.conv_tol:
+                logger.warn(self, 'Singularity detected in overlap matrix (condition number = %4.3g). '
+                            'SCF may be inaccurate and hard to converge.', cond)
         return self
 
     def get_hcore(self, cell=None, kpt=None):
         if cell is None: cell = self.cell
         if kpt is None: kpt = self.kpt
         if cell.pseudo:
             nuc = self.with_df.get_pp(kpt)
@@ -734,15 +742,15 @@
         if cell is None: cell = self.cell
         if kpt is None: kpt = self.kpt
         if self._eri is None:
             self._eri = self.with_df.get_ao_eri(kpt, compact=True)
         return self.get_jk(cell, dm, hermi, kpt)
 
     def energy_nuc(self):
-        return self.cell.energy_nuc()
+        return self.cell.enuc
 
     @lib.with_doc(dip_moment.__doc__)
     def dip_moment(self, cell=None, dm=None, unit='Debye', verbose=logger.NOTE,
                    **kwargs):
         if cell is None:
             cell = self.cell
         rho = kwargs.pop('rho', None)
@@ -754,18 +762,18 @@
         '''Hook for dumping results and clearing up the object.'''
         mol_hf.SCF._finalize(self)
 
         if self.cell.charge != 0:
             makov_payne_correction(self)
         return self
 
-    def get_init_guess(self, cell=None, key='minao'):
+    def get_init_guess(self, cell=None, key='minao', s1e=None):
         if cell is None: cell = self.cell
         dm = mol_hf.SCF.get_init_guess(self, cell, key)
-        dm = normalize_dm_(self, dm)
+        dm = normalize_dm_(self, dm, s1e)
         return dm
 
     def init_guess_by_1e(self, cell=None):
         if cell is None: cell = self.cell
         if cell.dimension < 3:
             logger.warn(self, 'Hcore initial guess is not recommended in '
                         'the SCF of low-dimensional systems.')
@@ -885,14 +893,15 @@
 
 
 class RHF(SCF):
 
     analyze = mol_hf.RHF.analyze
     spin_square = mol_hf.RHF.spin_square
     stability = mol_hf.RHF.stability
+    to_gpu = lib.to_gpu
 
     def nuc_grad_method(self):
         raise NotImplementedError
 
     def to_ks(self, xc='HF'):
         '''Convert to RKS object.
         '''
@@ -910,20 +919,22 @@
         vj = vj.reshape(dm.shape)
     elif kpts_band.ndim == 1:  # a single k-point on bands
         vj = vj.reshape(dm.shape)
     elif getattr(dm, "ndim", 0) == 2:
         vj = vj[0]
     return vj
 
-def normalize_dm_(mf, dm):
+def normalize_dm_(mf, dm, s1e=None):
     '''
     Scale density matrix to make it produce the correct number of electrons.
     '''
     cell = mf.cell
-    ne = np.einsum('ij,ji->', dm, mf.get_ovlp(cell)).real
+    if s1e is None:
+        s1e = mf.get_ovlp(cell)
+    ne = lib.einsum('ij,ji->', dm, s1e).real
     if abs(ne - cell.nelectron) > 0.01:
         logger.debug(mf, 'Big error detected in the electron number '
                      'of initial guess density matrix (Ne/cell = %g)!\n'
                      '  This can cause huge error in Fock matrix and '
                      'lead to instability in SCF for low-dimensional '
                      'systems.\n  DM is normalized wrt the number '
                      'of electrons %s', ne, cell.nelectron)
```

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/kghf.py` & `pyscf-2.6.0/pyscf/pbc/scf/kghf.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,14 +196,16 @@
     init_guess_by_atom = _cast_mol_init_guess(mol_hf.init_guess_by_atom)
     init_guess_by_chkfile = mol_ghf.init_guess_by_chkfile
     get_jk = get_jk
     get_occ = get_occ
     analyze = khf.analyze
     convert_from_ = pbcghf.GHF.convert_from_
 
+    to_gpu = lib.to_gpu
+
     def get_hcore(self, cell=None, kpts=None):
         hcore = khf.KSCF.get_hcore(self, cell, kpts)
         hcore = lib.asarray([scipy.linalg.block_diag(h, h) for h in hcore])
         if self.with_soc:
             raise NotImplementedError
         return hcore
```

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/kghf_ksymm.py` & `pyscf-2.6.0/pyscf/pbc/scf/kghf_ksymm.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/khf.py` & `pyscf-2.6.0/pyscf/pbc/scf/khf.py`

 * *Files 1% similar despite different names*

```diff
@@ -492,15 +492,15 @@
             logger.info(self, 'Smearing method = %s', self.smearing_method)
         logger.info(self, 'DF object = %s', self.with_df)
         if not getattr(self.with_df, 'build', None):
             # .dump_flags() is called in pbc.df.build function
             self.with_df.dump_flags(verbose)
         return self
 
-    def get_init_guess(self, cell=None, key='minao'):
+    def get_init_guess(self, cell=None, key='minao', s1e=None):
         raise NotImplementedError
 
     def init_guess_by_1e(self, cell=None):
         if cell is None: cell = self.cell
         if cell.dimension < 3:
             logger.warn(self, 'Hcore initial guess is not recommended in '
                         'the SCF of low-dimensional systems.')
@@ -520,18 +520,18 @@
                with_j=True, with_k=True, omega=None, **kwargs):
         if cell is None: cell = self.cell
         if kpts is None: kpts = self.kpts
         if dm_kpts is None: dm_kpts = self.make_rdm1()
         cpu0 = (logger.process_clock(), logger.perf_counter())
         if self.rsjk:
             vj, vk = self.rsjk.get_jk(dm_kpts, hermi, kpts, kpts_band,
-                                      with_j, with_k, omega, self.exxdiv)
+                                      with_j, with_k, omega=omega, exxdiv=self.exxdiv)
         else:
             vj, vk = self.with_df.get_jk(dm_kpts, hermi, kpts, kpts_band,
-                                         with_j, with_k, omega, self.exxdiv)
+                                         with_j, with_k, omega=omega, exxdiv=self.exxdiv)
         logger.timer(self, 'vj and vk', *cpu0)
         return vj, vk
 
     def get_veff(self, cell=None, dm_kpts=None, dm_last=0, vhf_last=0, hermi=1,
                  kpts=None, kpts_band=None):
         '''Hartree-Fock potential matrix for the given density matrix.
         See :func:`scf.hf.get_veff` and :func:`scf.hf.RHF.get_veff`
@@ -684,35 +684,38 @@
     def convert_from_(self, mf):
         raise NotImplementedError
 
 class KRHF(KSCF):
 
     analyze = analyze
     spin_square = mol_hf.RHF.spin_square
+    to_gpu = lib.to_gpu
 
     def check_sanity(self):
         cell = self.cell
         if isinstance(self.kpts, KPoints):
             nkpts = self.kpts.nkpts
         else:
             nkpts = len(self.kpts)
         if cell.spin != 0 and nkpts % 2 != 0:
             logger.warn(self, 'Problematic nelec %s and number of k-points %d '
                         'found in KRHF method.', cell.nelec, nkpts)
         return KSCF.check_sanity(self)
 
-    def get_init_guess(self, cell=None, key='minao'):
+    def get_init_guess(self, cell=None, key='minao', s1e=None):
+        if s1e is None:
+            s1e = self.get_ovlp(cell)
         dm = mol_hf.SCF.get_init_guess(self, cell, key)
         nkpts = len(self.kpts)
         if dm.ndim == 2:
             # dm[nao,nao] at gamma point -> dm_kpts[nkpts,nao,nao]
             dm = np.repeat(dm[None,:,:], nkpts, axis=0)
         dm_kpts = dm
 
-        ne = np.einsum('kij,kji->', dm_kpts, self.get_ovlp(cell)).real
+        ne = lib.einsum('kij,kji->', dm_kpts, s1e).real
         # FIXME: consider the fractional num_electron or not? This maybe
         # relate to the charged system.
         nelectron = float(self.cell.tot_electrons(nkpts))
         if abs(ne - nelectron) > 0.01*nkpts:
             logger.debug(self, 'Big error detected in the electron number '
                          'of initial guess density matrix (Ne/cell = %g)!\n'
                          '  This can cause huge error in Fock matrix and '
```

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/khf_ksymm.py` & `pyscf-2.6.0/pyscf/pbc/scf/khf_ksymm.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,22 +339,24 @@
 
 
 class KsymAdaptedKRHF(KsymAdaptedKSCF, khf.KRHF):
 
     to_ks = khf.KRHF.to_ks
     convert_from_ = khf.KRHF.convert_from_
 
-    def get_init_guess(self, cell=None, key='minao'):
+    def get_init_guess(self, cell=None, key='minao', s1e=None):
+        if s1e is None:
+            s1e = self.get_ovlp(cell)
         dm_kpts = mol_hf.SCF.get_init_guess(self, cell, key)
         if dm_kpts.ndim == 2:
             dm_kpts = np.asarray([dm_kpts]*self.kpts.nkpts_ibz)
         elif len(dm_kpts) != self.kpts.nkpts_ibz:
             dm_kpts = dm_kpts[self.kpts.ibz2bz]
 
-        ne = np.einsum('k,kij,kji', self.kpts.weights_ibz, dm_kpts, self.get_ovlp(cell)).real
+        ne = lib.einsum('k,kij,kji', self.kpts.weights_ibz, dm_kpts, s1e).real
         nkpts = self.kpts.nkpts
         ne *= nkpts
         nelectron = float(self.cell.tot_electrons(nkpts))
         if abs(ne - nelectron) > 0.01*nkpts:
             logger.debug(self, 'Big error detected in the electron number '
                          'of initial guess density matrix (Ne/cell = %g)!\n'
                          '  This can cause huge error in Fock matrix and '
```

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/krohf.py` & `pyscf-2.6.0/pyscf/pbc/scf/krohf.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,14 +270,15 @@
     get_fock = get_fock
     get_occ = get_occ
     energy_elec = energy_elec
     get_rho = get_rho
     analyze = khf.analyze
     spin_square = pbcrohf.ROHF.spin_square
     canonicalize = canonicalize
+    to_gpu = lib.to_gpu
 
     def __init__(self, cell, kpts=np.zeros((1,3)),
                  exxdiv=getattr(__config__, 'pbc_scf_SCF_exxdiv', 'ewald')):
         khf.KSCF.__init__(self, cell, kpts, exxdiv)
         self.nelec = None
 
     @property
```

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/kuhf.py` & `pyscf-2.6.0/pyscf/pbc/scf/kuhf.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,14 +380,15 @@
     get_fock = get_fock
     get_fermi = get_fermi
     get_occ = get_occ
     energy_elec = energy_elec
     get_rho = get_rho
     analyze = khf.analyze
     canonicalize = canonicalize
+    to_gpu = lib.to_gpu
 
     def __init__(self, cell, kpts=np.zeros((1,3)),
                  exxdiv=getattr(__config__, 'pbc_scf_SCF_exxdiv', 'ewald')):
         khf.KSCF.__init__(self, cell, kpts, exxdiv)
         self.nelec = None
         self.init_guess_breaksym = None
 
@@ -412,23 +413,25 @@
 
     def dump_flags(self, verbose=None):
         khf.KSCF.dump_flags(self, verbose)
         logger.info(self, 'number of electrons per cell  '
                     'alpha = %d beta = %d', *self.nelec)
         return self
 
-    def get_init_guess(self, cell=None, key='minao'):
+    def get_init_guess(self, cell=None, key='minao', s1e=None):
+        if s1e is None:
+            s1e = self.get_ovlp(cell)
         dm_kpts = mol_hf.SCF.get_init_guess(self, cell, key)
         assert dm_kpts.shape[0] == 2
         nkpts = len(self.kpts)
         if dm_kpts.ndim != 4:
             # dm[spin,nao,nao] at gamma point -> dm_kpts[spin,nkpts,nao,nao]
             dm_kpts = np.repeat(dm_kpts[:,None,:,:], nkpts, axis=1)
 
-        ne = np.einsum('xkij,kji->x', dm_kpts, self.get_ovlp(cell)).real
+        ne = lib.einsum('xkij,kji->x', dm_kpts, s1e).real
         nelec = np.asarray(self.nelec)
         if np.any(abs(ne - nelec) > 0.01*nkpts):
             logger.debug(self, 'Big error detected in the electron number '
                          'of initial guess density matrix (Ne/cell = %g)!\n'
                          '  This can cause huge error in Fock matrix and '
                          'lead to instability in SCF for low-dimensional '
                          'systems.\n  DM is normalized wrt the number '
```

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/newton_ah.py` & `pyscf-2.6.0/pyscf/pbc/scf/newton_ah.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/rohf.py` & `pyscf-2.6.0/pyscf/pbc/scf/rohf.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     make_rdm1 = mol_rohf.ROHF.make_rdm1
     energy_elec = mol_rohf.ROHF.energy_elec
     analyze = mol_rohf.ROHF.analyze
     canonicalize = mol_rohf.ROHF.canonicalize
     spin_square = mol_rohf.ROHF.spin_square
     stability = mol_rohf.ROHF.stability
     dip_moment = pbchf.SCF.dip_moment
+    to_gpu = lib.to_gpu
 
     def __init__(self, cell, kpt=np.zeros(3),
                  exxdiv=getattr(__config__, 'pbc_scf_SCF_exxdiv', 'ewald')):
         pbchf.SCF.__init__(self, cell, kpt, exxdiv)
         self.nelec = None
 
     @property
```

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/rsjk.py` & `pyscf-2.6.0/pyscf/pbc/scf/rsjk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1156,14 +1156,16 @@
         if time_reversal_symmetry:
             for k, k_conj in t_rev_pairs:
                 if k != k_conj:
                     vk_kpts[:,k_conj] = vk_kpts[:,k].conj()
         log.timer_debug1('get_lr_k_kpts', *cpu0)
         return vk_kpts
 
+    to_gpu = lib.to_gpu
+
 RangeSeparationJKBuilder = RangeSeparatedJKBuilder
 
 def _purify(mat_kpts, phase):
     if phase is None:
         return mat_kpts
     #:mat_bvk = np.einsum('Rk,nkij,Sk->nRSij', phase, mat_kpts, phase.conj())
     #:return np.einsum('Rk,nRSij,Sk->nkij', phase.conj(), mat_bvk.real, phase)
```

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/scfint.py` & `pyscf-2.6.0/pyscf/pbc/scf/scfint.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/stability.py` & `pyscf-2.6.0/pyscf/pbc/scf/stability.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/scf/uhf.py` & `pyscf-2.6.0/pyscf/pbc/scf/uhf.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,14 +124,15 @@
     get_rho = get_rho
     analyze = mol_uhf.UHF.analyze
     mulliken_pop = mol_uhf.UHF.mulliken_pop
     mulliken_meta = mol_uhf.UHF.mulliken_meta
     canonicalize = mol_uhf.UHF.canonicalize
     spin_square = mol_uhf.UHF.spin_square
     stability = mol_uhf.UHF.stability
+    to_gpu = lib.to_gpu
 
     def __init__(self, cell, kpt=np.zeros(3),
                  exxdiv=getattr(__config__, 'pbc_scf_SCF_exxdiv', 'ewald')):
         pbchf.SCF.__init__(self, cell, kpt, exxdiv)
         self.nelec = None
         self.init_guess_breaksym = None
 
@@ -217,18 +218,21 @@
         if dm is None:
             dm = self.make_rdm1()
         rho = kwargs.pop('rho', None)
         if rho is None:
             rho = self.get_rho(dm)
         return dip_moment(cell, dm, unit, verbose, rho=rho, kpt=self.kpt, **kwargs)
 
-    def get_init_guess(self, cell=None, key='minao'):
-        if cell is None: cell = self.cell
+    def get_init_guess(self, cell=None, key='minao', s1e=None):
+        if cell is None:
+            cell = self.cell
+        if s1e is None:
+            s1e = self.get_ovlp(cell)
         dm = mol_uhf.UHF.get_init_guess(self, cell, key)
-        ne = np.einsum('xij,ji->x', dm, self.get_ovlp(cell)).real
+        ne = np.einsum('xij,ji->x', dm, s1e).real
         nelec = self.nelec
         if np.any(abs(ne - nelec) > 0.01):
             logger.debug(self, 'Big error detected in the electron number '
                          'of initial guess density matrix (Ne/cell = %s)!\n'
                          '  This can cause huge error in Fock matrix and '
                          'lead to instability in SCF for low-dimensional '
                          'systems.\n  DM is normalized wrt the number '
```

### Comparing `pyscf-2.5.0/pyscf/pbc/symm/__init__.py` & `pyscf-2.6.0/pyscf/pbc/symm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/symm/basis.py` & `pyscf-2.6.0/pyscf/pbc/symm/basis.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/symm/geom.py` & `pyscf-2.6.0/pyscf/pbc/symm/geom.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         The current implementation treats the cell with the spins on all
         atoms flipped as the same as the original cell. If this is not desired,
         then one can use different names for the two sets of atoms and set their
         magnetic moment to 0.
     '''
     if rotations is None: rotations = search_point_group_ops(cell, tol=tol)
     a = cell.lattice_vectors()
-    coords = cell.get_scaled_positions()
+    coords = cell.get_scaled_atom_coords()
     atmgrp = mole.atom_types(cell._atom, magmom=cell.magmom)
     atmgrp_spin_inv = {} #spin up and down inverted
     has_spin = False
     for atm in atmgrp.keys():
         if atm[-2:] == '_u':
             has_spin = True
             atmgrp_spin_inv[atm] = atmgrp[atm[:-2]+'_d']
```

### Comparing `pyscf-2.5.0/pyscf/pbc/symm/group.py` & `pyscf-2.6.0/pyscf/pbc/symm/group.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/symm/pyscf_spglib.py` & `pyscf-2.6.0/pyscf/pbc/symm/pyscf_spglib.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     raise ImportError(msg)
 
 def cell_to_spgcell(cell):
     '''
     Convert PySCF Cell object to spglib cell object
     '''
     a = cell.lattice_vectors()
-    atm_pos = cell.get_scaled_positions()
+    atm_pos = cell.get_scaled_atom_coords()
     atm_num = []
     from pyscf.data import elements
     for symbol in cell.elements:
         if 'X-' in symbol or 'GHOST-' in symbol:
             raise NotImplementedError("Ghost atoms are not supported with symmetry.")
         atm_num.append(elements.NUC[symbol])
     for iatm in range(cell.natm):
```

### Comparing `pyscf-2.5.0/pyscf/pbc/symm/space_group.py` & `pyscf-2.6.0/pyscf/pbc/symm/space_group.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/symm/symmetry.py` & `pyscf-2.6.0/pyscf/pbc/symm/symmetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 
     def dump_info(self):
         self.spacegroup.dump_info(ops=self.ops)
 
 
 def _get_phase(cell, op, kpt_scaled, ignore_phase=False, tol=SYMPREC):
     kpt_scaled = op.a2b(cell).dot_rot(kpt_scaled)
-    coords_scaled = cell.get_scaled_positions().reshape(-1,3)
+    coords_scaled = cell.get_scaled_atom_coords().reshape(-1,3)
     natm = coords_scaled.shape[0]
     phase = np.ones((natm,), dtype=np.complex128)
     atm_map = np.arange(natm)
     coords0 = pbctools.round_to_cell0(coords_scaled, tol=tol)
     for iatm in range(natm):
         r = coords_scaled[iatm]
         op_dot_r = op.dot_rot(r) + op.trans
```

### Comparing `pyscf-2.5.0/pyscf/pbc/symm/tables.py` & `pyscf-2.6.0/pyscf/pbc/symm/tables.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tddft/__init__.py` & `pyscf-2.6.0/pyscf/pbc/tddft/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tdscf/__init__.py` & `pyscf-2.6.0/pyscf/pbc/tdscf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tdscf/kproxy.py` & `pyscf-2.6.0/pyscf/pbc/tdscf/kproxy.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tdscf/kproxy_supercell.py` & `pyscf-2.6.0/pyscf/pbc/tdscf/kproxy_supercell.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tdscf/krhf.py` & `pyscf-2.6.0/pyscf/pbc/tdscf/krhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tdscf/krhf_slow.py` & `pyscf-2.6.0/pyscf/pbc/tdscf/krhf_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tdscf/krhf_slow_gamma.py` & `pyscf-2.6.0/pyscf/pbc/tdscf/krhf_slow_gamma.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tdscf/krhf_slow_supercell.py` & `pyscf-2.6.0/pyscf/pbc/tdscf/krhf_slow_supercell.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tdscf/krks.py` & `pyscf-2.6.0/pyscf/pbc/tdscf/krks.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tdscf/kuhf.py` & `pyscf-2.6.0/pyscf/pbc/tdscf/kuhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tdscf/kuks.py` & `pyscf-2.6.0/pyscf/pbc/tdscf/kuks.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tdscf/proxy.py` & `pyscf-2.6.0/pyscf/pbc/tdscf/proxy.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tdscf/rhf.py` & `pyscf-2.6.0/pyscf/pbc/tdscf/rhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tdscf/rhf_slow.py` & `pyscf-2.6.0/pyscf/pbc/tdscf/rhf_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tdscf/rks.py` & `pyscf-2.6.0/pyscf/pbc/tdscf/rks.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tdscf/uhf.py` & `pyscf-2.6.0/pyscf/pbc/tdscf/uhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tdscf/uks.py` & `pyscf-2.6.0/pyscf/pbc/tdscf/uks.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tools/__init__.py` & `pyscf-2.6.0/pyscf/pbc/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tools/k2gamma.py` & `pyscf-2.6.0/pyscf/pbc/tools/k2gamma.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tools/lattice.py` & `pyscf-2.6.0/pyscf/pbc/tools/lattice.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tools/make_test_cell.py` & `pyscf-2.6.0/pyscf/pbc/tools/make_test_cell.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tools/pbc.py` & `pyscf-2.6.0/pyscf/pbc/tools/pbc.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import warnings
+import ctypes
 import numpy as np
 import scipy.linalg
 from pyscf import lib
 from pyscf.lib import logger
 from pyscf.gto import ATM_SLOTS, BAS_SLOTS, ATOM_OF, PTR_COORD
 from pyscf.pbc.lib.kpts_helper import get_kconserv, get_kconserv3  # noqa
 from pyscf import __config__
@@ -53,14 +54,52 @@
         buf[:] = gi.reshape(mesh)
         f = lib.dot(buf.reshape(mesh[0],-1).T, expRGx, 1./mesh[0], c=out[i].reshape(-1,mesh[0]))
         f = lib.dot(f.reshape(mesh[1],-1).T, expRGy, 1./mesh[1], c=buf.reshape(-1,mesh[1]))
         f = lib.dot(f.reshape(mesh[2],-1).T, expRGz, 1./mesh[2], c=out[i].reshape(-1,mesh[2]))
     return out.reshape(-1, *mesh)
 
 if FFT_ENGINE == 'FFTW':
+    try:
+        libfft = lib.load_library('libfft')
+    except OSError:
+        raise RuntimeError("Failed to load libfft")
+
+    def _copy_d2z(a):
+        fn = libfft._copy_d2z
+        out = np.empty(a.shape, dtype=np.complex128)
+        fn(out.ctypes.data_as(ctypes.c_void_p),
+           a.ctypes.data_as(ctypes.c_void_p),
+           ctypes.c_size_t(a.size))
+        return out
+
+    def _complex_fftn_fftw(f, mesh, func):
+        if f.dtype == np.double and f.flags.c_contiguous:
+            # np.asarray or np.astype is too slow
+            f = _copy_d2z(f)
+        else:
+            f = np.asarray(f, order='C', dtype=np.complex128)
+        mesh = np.asarray(mesh, order='C', dtype=np.int32)
+        rank = len(mesh)
+        out = np.empty_like(f)
+        fn = getattr(libfft, func)
+        for i, fi in enumerate(f):
+            fn(fi.ctypes.data_as(ctypes.c_void_p),
+               out[i].ctypes.data_as(ctypes.c_void_p),
+               mesh.ctypes.data_as(ctypes.c_void_p),
+               ctypes.c_int(rank))
+        return out
+
+    def _fftn_wrapper(a):
+        mesh = a.shape[1:]
+        return _complex_fftn_fftw(a, mesh, 'fft')
+    def _ifftn_wrapper(a):
+        mesh = a.shape[1:]
+        return _complex_fftn_fftw(a, mesh, 'ifft')
+
+elif FFT_ENGINE == 'PYFFTW':
     # pyfftw is slower than np.fft in most cases
     try:
         import pyfftw
         pyfftw.interfaces.cache.enable()
         nproc = lib.num_threads()
         def _fftn_wrapper(a):
             return pyfftw.interfaces.numpy_fft.fftn(a, axes=(1,2,3), threads=nproc)
@@ -231,16 +270,17 @@
         Gv = cell.get_Gv(mesh)
 
     if abs(k).sum() > 1e-9:
         kG = k + Gv
     else:
         kG = Gv
 
-    equal2boundary = np.zeros(Gv.shape[0], dtype=bool)
+    equal2boundary = None
     if wrap_around and abs(k).sum() > 1e-9:
+        equal2boundary = np.zeros(Gv.shape[0], dtype=bool)
         # Here we 'wrap around' the high frequency k+G vectors into their lower
         # frequency counterparts.  Important if you want the gamma point and k-point
         # answers to agree
         b = cell.reciprocal_vectors()
         box_edge = np.einsum('i,ij->ij', np.asarray(mesh)//2+0.5, b)
         assert (all(np.linalg.solve(box_edge.T, k).round(9).astype(int)==0))
         reduced_coords = np.linalg.solve(box_edge.T, kG.T).T.round(9)
@@ -353,15 +393,16 @@
         # Coulomb integrals were cancelled out by electron-nucleus
         # interaction. The periodic part of (ii|ii) in exchange cannot be
         # cancelled out by Coulomb integrals. Its leading term is calculated
         # using Ewald probe charge (the function madelung below)
         if cell.dimension > 0 and exxdiv == 'ewald' and len(G0_idx) > 0:
             coulG[G0_idx] += Nk*cell.vol*madelung(cell, kpts)
 
-    coulG[equal2boundary] = 0
+    if equal2boundary is not None:
+        coulG[equal2boundary] = 0
 
     # Scale the coulG kernel for attenuated Coulomb integrals.
     # * omega is used by RangeSeparatedJKBuilder which requires ewald probe charge
     # being evaluated with regular Coulomb interaction (1/r12).
     # * cell.omega, which affects the ewald probe charge, is often set by
     # DFT-RSH functionals to build long-range HF-exchange for erf(omega*r12)/r12
     if omega is not None:
@@ -503,15 +544,15 @@
         rcut = cell.rcut
 
     if dimension == 0 or rcut <= 0 or cell.natm == 0:
         return np.zeros((1, 3))
 
     a = cell.lattice_vectors()
 
-    scaled_atom_coords = np.linalg.solve(a.T, cell.atom_coords().T).T
+    scaled_atom_coords = cell.get_scaled_atom_coords()
     atom_boundary_max = scaled_atom_coords[:,:dimension].max(axis=0)
     atom_boundary_min = scaled_atom_coords[:,:dimension].min(axis=0)
     if (np.any(atom_boundary_max > 1) or np.any(atom_boundary_min < -1)):
         atom_boundary_max[atom_boundary_max > 1] = 1
         atom_boundary_min[atom_boundary_min <-1] = -1
     ovlp_penalty = atom_boundary_max - atom_boundary_min
     dR = ovlp_penalty.dot(a[:dimension])
@@ -538,19 +579,20 @@
         zb = 0
     bounds = np.ceil([xb, yb, zb]).astype(int)
     Ts = lib.cartesian_prod((np.arange(-bounds[0], bounds[0]+1),
                              np.arange(-bounds[1], bounds[1]+1),
                              np.arange(-bounds[2], bounds[2]+1)))
     Ls = np.dot(Ts[:,:dimension], a[:dimension])
 
-    ovlp_penalty += 1e-200  # avoid /0
-    Ts_scaled = (Ts[:,:dimension] + 1e-200) / ovlp_penalty
-    ovlp_penalty_fac = 1. / abs(Ts_scaled).min(axis=1)
-    Ls_mask = np.linalg.norm(Ls, axis=1) * (1-ovlp_penalty_fac) < rcut
-    Ls = Ls[Ls_mask]
+    if discard:
+        ovlp_penalty += 1e-200  # avoid /0
+        Ts_scaled = (Ts[:,:dimension] + 1e-200) / ovlp_penalty
+        ovlp_penalty_fac = 1. / abs(Ts_scaled).min(axis=1)
+        Ls_mask = np.linalg.norm(Ls, axis=1) * (1-ovlp_penalty_fac) < rcut
+        Ls = Ls[Ls_mask]
     return np.asarray(Ls, order='C')
 
 
 def super_cell(cell, ncopy, wrap_around=False):
     '''Create an ncopy[0] x ncopy[1] x ncopy[2] supercell of the input cell
     Note this function differs from :func:`cell_plus_imgs` that cell_plus_imgs
     creates images in both +/- direction.
@@ -630,14 +672,15 @@
     nimgs = len(Ls)
     symbs = [atom[0] for atom in cell._atom] * nimgs
     coords = Ls.reshape(-1,1,3) + cell.atom_coords()
     coords = coords.reshape(-1,3)
     x, y, z = coords.T
     supcell.atom = supcell._atom = list(zip(symbs, zip(x, y, z)))
     supcell.unit = 'B'
+    supcell.enuc = None # reset nuclear energy
 
     # Do not call supcell.build() to initialize supcell since it may normalize
     # the basis contraction coefficients
 
     # preserves environments defined in cell._env (e.g. omega, gauge origin)
     _env = np.append(cell._env, coords.ravel())
     _atm = np.repeat(cell._atm[None,:,:], nimgs, axis=0)
```

### Comparing `pyscf-2.5.0/pyscf/pbc/tools/print_funcs.py` & `pyscf-2.6.0/pyscf/pbc/tools/print_funcs.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tools/pyscf_ase.py` & `pyscf-2.6.0/pyscf/pbc/tools/pyscf_ase.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tools/pywannier90.py` & `pyscf-2.6.0/pyscf/pbc/tools/pywannier90.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/tools/tril.py` & `pyscf-2.6.0/pyscf/pbc/tools/tril.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/x2c/__init__.py` & `pyscf-2.6.0/pyscf/pbc/x2c/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/x2c/sfx2c1e.py` & `pyscf-2.6.0/pyscf/pbc/x2c/sfx2c1e.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/pbc/x2c/x2c1e.py` & `pyscf-2.6.0/pyscf/pbc/x2c/x2c1e.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/qmmm/__init__.py` & `pyscf-2.6.0/pyscf/qmmm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/qmmm/itrf.py` & `pyscf-2.6.0/pyscf/qmmm/itrf.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,14 +184,19 @@
         charges = self.mm_mol.atom_charges()
         for j in range(self.mol.natm):
             q2, r2 = self.mol.atom_charge(j), self.mol.atom_coord(j)
             r = lib.norm(r2-coords, axis=1)
             nuc += q2*(charges/r).sum()
         return nuc
 
+    def to_gpu(self):
+        obj = self.undo_qmmm().to_gpu()
+        obj = qmmm_for_scf(obj, self.mm_mol)
+        return lib.to_gpu(self, obj)
+
     def nuc_grad_method(self):
         scf_grad = super().nuc_grad_method()
         return qmmm_grad_for_scf(scf_grad)
 
     Gradients = nuc_grad_method
 
 class QMMMPostSCF(QMMM):
@@ -203,14 +208,16 @@
         self.mo_energy = mf.mo_energy
 
     def undo_qmmm(self):
         obj = lib.view(self, lib.drop_class(self.__class__, QMMM))
         obj._scf = self._scf.undo_qmmm()
         return obj
 
+    to_gpu = QMMMSCF.to_gpu
+
 
 def add_mm_charges_grad(scf_grad, atoms_or_coords, charges, radii=None, unit=None):
     '''Apply the MM charges in the QM gradients' method.  It affects both the
     electronic and nuclear parts of the QM fragment.
 
     Args:
         scf_grad : a HF or DFT gradient object (grad.HF or grad.RKS etc)
@@ -392,14 +399,19 @@
         for i in range(mol.natm):
             q1 = mol.atom_charge(i)
             r1 = mol.atom_coord(i)
             r = lib.norm(r1-coords, axis=1)
             g_mm += q1 * numpy.einsum('i,ix,i->ix', charges, r1-coords, 1/r**3)
         return g_mm
 
+    def to_gpu(self):
+        obj = self.undo_qmmm().to_gpu()
+        obj = qmmm_grad_for_scf(obj)
+        return lib.to_gpu(self, obj)
+
 _QMMMGrad = QMMMGrad
 
 # Inject QMMM interface wrapper to other modules
 scf.hf.SCF.QMMM = mm_charge
 mcscf.casci.CASBase.QMMM = mm_charge
 grad.rhf.Gradients.QMMM = mm_charge_grad
```

### Comparing `pyscf-2.5.0/pyscf/qmmm/mm_mole.py` & `pyscf-2.6.0/pyscf/qmmm/mm_mole.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/scf/__init__.py` & `pyscf-2.6.0/pyscf/scf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,15 @@
 def X2C(mol, *args):
     '''X2C Hartree-Fock'''
     from pyscf.x2c import x2c
     if dhf.zquatev and mol.spin == 0:
         return x2c.RHF(mol, *args)
     else:
         return x2c.UHF(mol, *args)
+X2C_HF = X2C
 gto.Mole.X2C = gto.Mole.X2C_HF = property(X2C)
 
 def sfx2c1e(mf):
     '''spin-free (the scalar part) X2C with 1-electron X-matrix'''
     return mf.sfx2c1e()
 sfx2c = sfx2c1e
```

### Comparing `pyscf-2.5.0/pyscf/scf/_response_functions.py` & `pyscf-2.6.0/pyscf/scf/_response_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     if mo_coeff is None: mo_coeff = mf.mo_coeff
     if mo_occ is None: mo_occ = mf.mo_occ
     mol = mf.mol
     if isinstance(mf, hf.KohnShamDFT):
         from pyscf.dft import numint
         ni = mf._numint
         ni.libxc.test_deriv_order(mf.xc, 2, raise_error=True)
-        if mf.nlc or ni.libxc.is_nlc(mf.xc):
+        if mf.do_nlc():
             logger.warn(mf, 'NLC functional found in DFT object.  Its second '
                         'deriviative is not available. Its contribution is '
                         'not included in the response function.')
         omega, alpha, hyb = ni.rsh_and_hybrid_coeff(mf.xc, mol.spin)
         hybrid = ni.libxc.is_hybrid_xc(mf.xc)
 
         # mf can be pbc.dft.RKS object with multigrid
@@ -151,15 +151,15 @@
     assert isinstance(mf, (uhf.UHF, rohf.ROHF))
     if mo_coeff is None: mo_coeff = mf.mo_coeff
     if mo_occ is None: mo_occ = mf.mo_occ
     mol = mf.mol
     if isinstance(mf, hf.KohnShamDFT):
         ni = mf._numint
         ni.libxc.test_deriv_order(mf.xc, 2, raise_error=True)
-        if mf.nlc or ni.libxc.is_nlc(mf.xc):
+        if mf.do_nlc():
             logger.warn(mf, 'NLC functional found in DFT object.  Its second '
                         'deriviative is not available. Its contribution is '
                         'not included in the response function.')
         omega, alpha, hyb = ni.rsh_and_hybrid_coeff(mf.xc, mol.spin)
         hybrid = ni.libxc.is_hybrid_xc(mf.xc)
 
         # mf can be pbc.dft.UKS object with multigrid
@@ -224,15 +224,15 @@
     if mo_occ is None: mo_occ = mf.mo_occ
     mol = mf.mol
     if isinstance(mf, hf.KohnShamDFT):
         from pyscf.dft import numint2c, r_numint
         ni = mf._numint
         assert isinstance(ni, (numint2c.NumInt2C, r_numint.RNumInt))
         ni.libxc.test_deriv_order(mf.xc, 2, raise_error=True)
-        if mf.nlc or ni.libxc.is_nlc(mf.xc):
+        if mf.do_nlc():
             raise NotImplementedError('NLC')
         omega, alpha, hyb = ni.rsh_and_hybrid_coeff(mf.xc, mol.spin)
         hybrid = ni.libxc.is_hybrid_xc(mf.xc)
 
         # mf can be pbc.dft.UKS object with multigrid
         if (not hybrid and
             'MultiGridFFTDF' == getattr(mf, 'with_df', None).__class__.__name__):
```

### Comparing `pyscf-2.5.0/pyscf/scf/_vhf.py` & `pyscf-2.6.0/pyscf/scf/_vhf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/scf/addons.py` & `pyscf-2.6.0/pyscf/scf/addons.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,20 +136,25 @@
                 mo_es = (mo_energy, mo_energy)
             else:
                 mo_es = mo_energy
             nocc = self.nelec
             if self.mu0 is None:
                 mu_a, occa = _smearing_optimize(f_occ, mo_es[0], nocc[0], sigma)
                 mu_b, occb = _smearing_optimize(f_occ, mo_es[1], nocc[1], sigma)
-                mu = [mu_a, mu_b]
-                mo_occs = [occa, occb]
             else:
-                mu = self.mu0
-                mo_occs = f_occ(mu[0], mo_es[0], sigma)
-                mo_occs = f_occ(mu[1], mo_es[1], sigma)
+                if numpy.isscalar(self.mu0):
+                    mu_a = mu_b = self.mu0
+                elif len(self.mu0) == 2:
+                    mu_a, mu_b = self.mu0
+                else:
+                    raise TypeError(f'Unsupported mu0: {self.mu0}')
+                occa = f_occ(mu_a, mo_es[0], sigma)
+                occb = f_occ(mu_b, mo_es[1], sigma)
+            mu = [mu_a, mu_b]
+            mo_occs = [occa, occb]
             self.entropy  = self._get_entropy(mo_es[0], mo_occs[0], mu[0])
             self.entropy += self._get_entropy(mo_es[1], mo_occs[1], mu[1])
             fermi = (_get_fermi(mo_es[0], nocc[0]), _get_fermi(mo_es[1], nocc[1]))
 
             logger.debug(self, '    Alpha-spin Fermi level %g  Sum mo_occ = %s  should equal nelec = %s',
                          fermi[0], mo_occs[0].sum(), nocc[0])
             logger.debug(self, '    Beta-spin  Fermi level %g  Sum mo_occ = %s  should equal nelec = %s',
@@ -159,27 +164,28 @@
             logger.info(self, '    sigma = %g  Optimized mu_beta  = %.12g  entropy = %.12g',
                         sigma, mu[1], self.entropy)
             if self.verbose >= logger.DEBUG:
                 print_mo_energy_occ(self, mo_energy, mo_occs, True)
             if is_rohf:
                 mo_occs = mo_occs[0] + mo_occs[1]
         else: # all orbitals treated with the same fermi level
-            nocc = nelectron = self.mol.tot_electrons()
+            nocc = nelectron = self.mol.nelectron
             if is_uhf:
                 mo_es = numpy.hstack(mo_energy)
             else:
                 mo_es = mo_energy
             if is_rhf:
                 nocc = (nelectron + 1) // 2
 
             if self.mu0 is None:
                 mu, mo_occs = _smearing_optimize(f_occ, mo_es, nocc, sigma)
             else:
                 # If mu0 is given, fix mu instead of electron number. XXX -Chong Sun
                 mu = self.mu0
+                assert numpy.isscalar(mu)
                 mo_occs = f_occ(mu, mo_es, sigma)
             self.entropy = self._get_entropy(mo_es, mo_occs, mu)
             if is_rhf:
                 mo_occs *= 2
                 self.entropy *= 2
 
             fermi = _get_fermi(mo_es, nocc)
```

### Comparing `pyscf-2.5.0/pyscf/scf/atom_hf.py` & `pyscf-2.6.0/pyscf/scf/atom_hf.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 def get_atm_nrhf(mol, atomic_configuration=elements.NRSRHF_CONFIGURATION):
     elements = {a[0] for a in mol._atom}
     logger.info(mol, 'Spherically averaged atomic HF for %s', elements)
 
     atm_template = mol.copy(deep=False)
     atm_template.charge = 0
+    atm_template.enuc = 0
     atm_template.symmetry = False  # TODO: enable SO3 symmetry here
     atm_template.atom = atm_template._atom = []
     atm_template.cart = False  # AtomSphAverageRHF does not support cartesian basis
 
     atm_scf_result = {}
     for ia, a in enumerate(mol._atom):
         element = a[0]
@@ -46,23 +47,35 @@
         atm._bas = mol._bas[mol._bas[:,0] == ia].copy()
         atm._ecpbas = mol._ecpbas[mol._ecpbas[:,0] == ia].copy()
         # Point to the only atom
         atm._bas[:,0] = 0
         atm._ecpbas[:,0] = 0
         if element in mol._pseudo:
             atm._pseudo = {element: mol._pseudo.get(element)}
-            raise NotImplementedError
         atm.spin = atm.nelectron % 2
 
         nao = atm.nao
         # nao == 0 for the case that no basis was assigned to an atom
         if nao == 0 or atm.nelectron == 0:  # GHOST
             mo_occ = mo_energy = numpy.zeros(nao)
             mo_coeff = numpy.zeros((nao,nao))
             atm_scf_result[element] = (0, mo_energy, mo_coeff, mo_occ)
+        elif atm._pseudo:
+            from pyscf.scf import atom_hf_pp
+            atm.a = None
+            if atm.nelectron == 1:
+                atm_hf = atom_hf_pp.AtomHF1ePP(atm)
+            else:
+                atm_hf = atom_hf_pp.AtomSCFPP(atm)
+                atm_hf.atomic_configuration = atomic_configuration
+
+            atm_hf.verbose = mol.verbose
+            atm_hf.run()
+            atm_scf_result[element] = (atm_hf.e_tot, atm_hf.mo_energy,
+                                       atm_hf.mo_coeff, atm_hf.mo_occ)
         else:
             if atm.nelectron == 1:
                 atm_hf = AtomHF1e(atm)
             else:
                 atm_hf = AtomSphAverageRHF(atm)
                 atm_hf.atomic_configuration = atomic_configuration
 
@@ -76,15 +89,15 @@
 class AtomSphAverageRHF(hf.RHF):
     def __init__(self, mol):
         self._eri = None
         self.atomic_configuration = elements.NRSRHF_CONFIGURATION
         hf.SCF.__init__(self, mol)
 
         # The default initial guess minao does not have super-heavy elements
-        if mol.atom_charge(0) > 96:
+        if gto.charge(mol.atom_symbol(0)) > 96:
             self.init_guess = '1e'
 
         self = self.apply(addons.remove_linear_dep_)
 
     def check_sanity(self):
         pass
```

### Comparing `pyscf-2.5.0/pyscf/scf/atom_ks.py` & `pyscf-2.6.0/pyscf/scf/atom_ks.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/scf/chkfile.py` & `pyscf-2.6.0/pyscf/scf/chkfile.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/scf/cphf.py` & `pyscf-2.6.0/pyscf/scf/cphf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/scf/dhf.py` & `pyscf-2.6.0/pyscf/scf/dhf.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,22 +281,22 @@
         else: # nr-UHF
             dm = (reduce(numpy.dot, (mo[0]*mo_occ[0], mo[0].T)) +
                   reduce(numpy.dot, (mo[1]*mo_occ[1], mo[1].T)))
         dm = _proj_dmll(chk_mol, dm, mol)
     return dm
 
 
-def get_init_guess(mol, key='minao'):
+def get_init_guess(mol, key='minao', **kwargs):
     '''Generate density matrix for initial guess
 
     Kwargs:
         key : str
             One of 'minao', 'atom', 'huckel', 'mod_huckel', 'hcore', '1e', 'chkfile'.
     '''
-    return UHF(mol).get_init_guess(mol, key)
+    return UHF(mol).get_init_guess(mol, key, **kwargs)
 
 def time_reversal_matrix(mol, mat):
     ''' T(A_ij) = A[T(i),T(j)]^*
     '''
     tao = numpy.asarray(mol.time_reversal_map())
     n2c = tao.size
     # tao(i) = -j  means  T(f_i) = -f_j
@@ -450,20 +450,19 @@
     with_ssss = getattr(__config__, 'scf_dhf_SCF_with_ssss', True)
     with_gaunt = getattr(__config__, 'scf_dhf_SCF_with_gaunt', False)
     with_breit = getattr(__config__, 'scf_dhf_SCF_with_breit', False)
     # corrections for small component when with_ssss is set to False
     ssss_approx = getattr(__config__, 'scf_dhf_SCF_ssss_approx', 'Visscher')
 
     _keys = {'conv_tol', 'with_ssss', 'with_gaunt',
-                 'with_breit', 'ssss_approx', 'opt'}
+                 'with_breit', 'ssss_approx'}
 
     def __init__(self, mol):
         hf.SCF.__init__(self, mol)
         self._coulomb_level = 'SSSS' # 'SSSS' ~ LLLL+LLSS+SSSS
-        self.opt = None # (opt_llll, opt_ssll, opt_ssss, opt_gaunt)
 
     def dump_flags(self, verbose=None):
         hf.SCF.dump_flags(self, verbose)
         log = logger.new_logger(self, verbose)
         log.info('with_ssss %s, with_gaunt %s, with_breit %s',
                  self.with_ssss, self.with_gaunt, self.with_breit)
         if not self.with_ssss:
@@ -514,16 +513,14 @@
     def init_guess_by_chkfile(self, chkfile=None, project=None):
         if chkfile is None: chkfile = self.chkfile
         return init_guess_by_chkfile(self.mol, chkfile, project=project)
 
     def build(self, mol=None):
         if self.verbose >= logger.WARN:
             self.check_sanity()
-        if self.direct_scf:
-            self.opt = self.init_direct_scf(mol)
         return self
 
     def get_occ(self, mo_energy=None, mo_coeff=None):
         if mo_energy is None: mo_energy = self.mo_energy
         mol = self.mol
         c = lib.param.LIGHT_SPEED
         n4c = len(mo_energy)
@@ -682,15 +679,14 @@
 
     def reset(self, mol=None):
         '''Reset mol and clean up relevant attributes for scanner mode'''
         if mol is not None:
             self.mol = mol
         self._coulomb_level = 'SSSS' # 'SSSS' ~ LLLL+LLSS+SSSS
         self._opt = {None: None}
-        self.opt = None # (opt_llll, opt_ssll, opt_ssss, opt_gaunt)
         return self
 
     def stability(self, internal=None, external=None, verbose=None, return_status=False):
         '''
         DHF/DKS stability analysis.
 
         See also pyscf.scf.stability.rhf_stability function.
@@ -745,14 +741,16 @@
         mf = self.view(dks.UDKS)
         mf.xc = xc
         mf.converged = False
         return mf
 
     to_ks = to_dks
 
+    to_gpu = lib.to_gpu
+
 UHF = UDHF = DHF
 
 
 class HF1e(DHF):
     scf = hf._hf1e_scf
 
     def _eigh(self, h, s):
```

### Comparing `pyscf-2.5.0/pyscf/scf/diis.py` & `pyscf-2.6.0/pyscf/scf/diis.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,18 +40,14 @@
 class CDIIS(lib.diis.DIIS):
     def __init__(self, mf=None, filename=None, Corth=None):
         lib.diis.DIIS.__init__(self, mf, filename)
         self.rollback = 0
         self.space = 8
         self.Corth = Corth
         self.damp = 0
-        #?self._scf = mf
-        #?if hasattr(self._scf, 'get_orbsym'): # Symmetry adapted SCF objects
-        #?    self.orbsym = mf.get_orbsym(Corth)
-        #?    sym_forbid = self.orbsym[:,None] != self.orbsym
 
     def update(self, s, d, f, *args, **kwargs):
         errvec = get_err_vec(s, d, f, self.Corth)
         logger.debug1(self, 'diis-norm(errvec)=%g', numpy.linalg.norm(errvec))
         f_prev = kwargs.get('f_prev', None)
         if abs(self.damp) < 1e-6 or f_prev is None:
             xnew = lib.diis.DIIS.update(self, f, xerr=errvec)
@@ -68,21 +64,21 @@
             return len(self._bookkeep)
 
 SCFDIIS = SCF_DIIS = DIIS = CDIIS
 
 def get_err_vec_orig(s, d, f):
     '''error vector = SDF - FDS'''
     if isinstance(f, numpy.ndarray) and f.ndim == 2:
-        sdf = reduce(numpy.dot, (s,d,f))
+        sdf = reduce(lib.dot, (s,d,f))
         errvec = (sdf.conj().T - sdf).ravel()
 
     elif isinstance(f, numpy.ndarray) and f.ndim == 3 and s.ndim == 3:
         errvec = []
         for i in range(f.shape[0]):
-            sdf = reduce(numpy.dot, (s[i], d[i], f[i]))
+            sdf = reduce(lib.dot, (s[i], d[i], f[i]))
             errvec.append((sdf.conj().T - sdf).ravel())
         errvec = numpy.hstack(errvec)
 
     elif f.ndim == s.ndim+1 and f.shape[0] == 2:  # for UHF
         errvec = numpy.hstack([
             get_err_vec_orig(s, d[0], f[0]).ravel(),
             get_err_vec_orig(s, d[1], f[1]).ravel()])
@@ -94,23 +90,23 @@
     '''error vector in orthonormal basis = C.T.conj() (SDF - FDS) C'''
     # Symmetry information to reduce numerical error in DIIS (issue #1524)
     orbsym = getattr(Corth, 'orbsym', None)
     if orbsym is not None:
         sym_forbid = orbsym[:,None] != orbsym
 
     if isinstance(f, numpy.ndarray) and f.ndim == 2:
-        sdf = reduce(numpy.dot, (Corth.conj().T, s, d, f, Corth))
+        sdf = reduce(lib.dot, (Corth.conj().T, s, d, f, Corth))
         if orbsym is not None:
             sdf[sym_forbid] = 0
         errvec = (sdf.conj().T - sdf).ravel()
 
     elif isinstance(f, numpy.ndarray) and f.ndim == 3 and s.ndim == 3:
         errvec = []
         for i in range(f.shape[0]):
-            sdf = reduce(numpy.dot, (Corth[i].conj().T, s[i], d[i], f[i], Corth[i]))
+            sdf = reduce(lib.dot, (Corth[i].conj().T, s[i], d[i], f[i], Corth[i]))
             if orbsym is not None:
                 sdf[sym_forbid] = 0
             errvec.append((sdf.conj().T - sdf).ravel())
         errvec = numpy.hstack(errvec)
 
     elif f.ndim == s.ndim+1 and f.shape[0] == 2:  # for UHF
         errvec = numpy.hstack([
```

### Comparing `pyscf-2.5.0/pyscf/scf/dispersion.py` & `pyscf-2.6.0/pyscf/grad/dispersion.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,68 +13,54 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # Author: Xiaojie Wu <wxj6000@gmail.com>
 #
 
 '''
-dispersion correction for HF and DFT
+gradient of dispersion correction for HF and DFT
 '''
 
+import numpy as np
+from pyscf.lib import logger
+from pyscf.scf.dispersion import check_disp, parse_disp
+
+def get_dispersion(mf_grad, disp=None, with_3body=None, verbose=None):
+    '''gradient of DFTD3/DFTD4 dispersion correction'''
+    mf = mf_grad.base
+    mol = mf.mol
+    disp_version = check_disp(mf, disp)
+    if not disp_version:
+        return np.zeros([mol.natm,3])
+
+    try:
+        from pyscf.dispersion import dftd3, dftd4
+    except ImportError:
+        print('dftd3 and dftd4 not available. Install them with `pip install pyscf-dispersion`')
+        raise
 
-import numpy
-from pyscf.scf.hf import KohnShamDFT
+    method = getattr(mf, 'xc', 'hf')
+    method, _, disp_with_3body = parse_disp(method)
 
-def get_dispersion(mf, disp_version=None):
-    if disp_version is None:
-        disp_version = mf.disp
-    mol = mf.mol
-    if disp_version is None:
-        return 0.0
-    if isinstance(mf, KohnShamDFT):
-        method = mf.xc
-    else:
-        method = 'hf'
+    if with_3body is not None:
+        with_3body = disp_with_3body
 
-    # for dftd3
     if disp_version[:2].upper() == 'D3':
-        try:
-            import dftd3.pyscf as disp
-        except ImportError:
-            raise ImportError("\n \
-cannot find dftd3 in the current environment.\n \
-please install dftd3 via \n \
-**************************************\n\
-        pip3 install dftd3 \n \
-**************************************")
-
-        d3 = disp.DFTD3Dispersion(mol, xc=method, version=disp_version)
-        e_d3, _ = d3.kernel()
-        mf.scf_summary['dispersion'] = e_d3
-        return e_d3
-
-    # for dftd4
+        logger.info(mf, "Calc dispersion correction with DFTD3.")
+        logger.info(mf, f"Parameters: xc={method}, version={disp_version}, atm={with_3body}")
+        d3_model = dftd3.DFTD3Dispersion(mol, xc=method, version=disp_version, atm=with_3body)
+        res = d3_model.get_dispersion(grad=True)
+        g_d3 = res.get('gradient')
+        return g_d3
     elif disp_version[:2].upper() == 'D4':
-        from pyscf.data.elements import charge
-        atoms = numpy.array([ charge(a[0]) for a in mol._atom])
-        coords = mol.atom_coords()
-        try:
-            from dftd4.interface import DampingParam, DispersionModel
-        except ImportError:
-            raise ImportError("\n \
-cannot find dftd4 in the current environment. \n \
-please install dftd4 via \n \
-***************************************\n \
-        pip3 install dftd4 \n \
-***************************************")
-
-        model = DispersionModel(atoms, coords)
-        res = model.get_dispersion(DampingParam(method=method), grad=False)
-        e_d4 = res.get("energy")
-        mf.scf_summary['dispersion'] = e_d4
-        return e_d4
+        logger.info(mf, "Calc dispersion correction with DFTD4.")
+        logger.info(mf, f"Parameters: xc={method}, atm={with_3body}")
+        d4_model = dftd4.DFTD4Dispersion(mol, xc=method, atm=with_3body)
+        res = d4_model.get_dispersion(grad=True)
+        g_d4 = res.get('gradient')
+        return g_d4
     else:
-        raise RuntimeError(f'dipersion correction: {disp_version} is not supported.')
+        raise RuntimeError(f'dispersion correction: {disp_version} is not supported.')
 
-# Inject to SCF class
-from pyscf import scf
-scf.hf.SCF.get_dispersion = get_dispersion
+# Inject to Gradient
+from pyscf import grad
+grad.rhf.GradientsBase.get_dispersion = get_dispersion
```

### Comparing `pyscf-2.5.0/pyscf/scf/ghf.py` & `pyscf-2.6.0/pyscf/scf/ghf.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,24 +378,22 @@
 
     Attributes for GHF method
         GHF orbital coefficients are 2D array.  Let nao be the number of spatial
         AOs, mo_coeff[:nao] are the coefficients of AO with alpha spin;
         mo_coeff[nao:nao*2] are the coefficients of AO with beta spin.
     '''
 
+    with_soc = None
+
     _keys = {'with_soc'}
 
     get_init_guess = hf.RHF.get_init_guess
     get_occ = get_occ
     _finalize = uhf.UHF._finalize
 
-    def __init__(self, mol):
-        hf.SCF.__init__(self, mol)
-        self.with_soc = None
-
     def get_hcore(self, mol=None):
         if mol is None: mol = self.mol
         hcore = hf.get_hcore(mol)
         hcore = scipy.linalg.block_diag(hcore, hcore)
 
         if self.with_soc and mol.has_ecp_soc():
             # The ECP SOC contribution = <|1j * s * U_SOC|>
@@ -537,17 +535,15 @@
 
     def to_ks(self, xc='HF'):
         '''Convert to GKS object.
         '''
         from pyscf import dft
         return self._transfer_attrs_(dft.GKS(self.mol, xc=xc))
 
-    def to_gpu(self):
-        from gpu4pyscf.scf import GHF
-        return lib.to_gpu(hf.SCF.reset(self.view(GHF)))
+    to_gpu = lib.to_gpu
 
 def _from_rhf_init_dm(dm, breaksym=True):
     dma = dm * .5
     dm = scipy.linalg.block_diag(dma, dma)
     if breaksym:
         nao = dma.shape[0]
         idx, idy = numpy.diag_indices(nao)
```

### Comparing `pyscf-2.5.0/pyscf/scf/ghf_symm.py` & `pyscf-2.6.0/pyscf/scf/ghf_symm.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,16 +277,15 @@
         if getattr(mo_coeff, 'orbsym', None) is not None:
             return mo_coeff.orbsym
         if s is None:
             s = self.get_ovlp()
         return numpy.asarray(get_orbsym(self.mol, mo_coeff, s))
     orbsym = property(get_orbsym)
 
-    def to_gpu(self):
-        raise NotImplementedError
+    to_gpu = lib.to_gpu
 
 GHF = SymAdaptedGHF
 
 
 class HF1e(GHF):
     scf = hf._hf1e_scf
```

### Comparing `pyscf-2.5.0/pyscf/scf/hf.py` & `pyscf-2.6.0/pyscf/scf/hf.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,34 +111,29 @@
 Keyword argument "init_dm" is replaced by "dm0"''')
     cput0 = (logger.process_clock(), logger.perf_counter())
     if conv_tol_grad is None:
         conv_tol_grad = numpy.sqrt(conv_tol)
         logger.info(mf, 'Set gradient conv threshold to %g', conv_tol_grad)
 
     mol = mf.mol
+    s1e = mf.get_ovlp(mol)
+
     if dm0 is None:
-        dm = mf.get_init_guess(mol, mf.init_guess)
+        dm = mf.get_init_guess(mol, mf.init_guess, s1e=s1e)
     else:
         dm = dm0
 
     h1e = mf.get_hcore(mol)
     vhf = mf.get_veff(mol, dm)
     e_tot = mf.energy_tot(dm, h1e, vhf)
     logger.info(mf, 'init E= %.15g', e_tot)
 
     scf_conv = False
     mo_energy = mo_coeff = mo_occ = None
 
-    s1e = mf.get_ovlp(mol)
-    cond = lib.cond(s1e)
-    logger.debug(mf, 'cond(S) = %s', cond)
-    if numpy.max(cond)*1e-17 > conv_tol:
-        logger.warn(mf, 'Singularity detected in overlap matrix (condition number = %4.3g). '
-                    'SCF may be inaccurate and hard to converge.', numpy.max(cond))
-
     # Skip SCF iterations. Compute only the total energy of the initial density
     if mf.max_cycle <= 0:
         fock = mf.get_fock(h1e, s1e, vhf, dm)  # = h1e + vhf, no DIIS
         mo_energy, mo_coeff = mf.eig(fock, s1e)
         mo_occ = mf.get_occ(mo_energy, mo_coeff)
         return scf_conv, e_tot, mo_energy, mo_coeff, mo_occ
 
@@ -230,20 +225,14 @@
         elif abs(e_tot-last_hf_e) < conv_tol or norm_gorb < conv_tol_grad:
             scf_conv = True
         logger.info(mf, 'Extra cycle  E= %.15g  delta_E= %4.3g  |g|= %4.3g  |ddm|= %4.3g',
                     e_tot, e_tot-last_hf_e, norm_gorb, norm_ddm)
         if dump_chk:
             mf.dump_chk(locals())
 
-    #FIX DISP!!
-    if mf.disp is not None:
-        e_disp = mf.get_dispersion()
-        mf.scf_summary['dispersion'] = e_disp
-        e_tot += e_disp
-
     logger.timer(mf, 'scf_cycle', *cput0)
     # A post-processing hook before return
     mf.post_kernel(locals())
     return scf_conv, e_tot, mo_energy, mo_coeff, mo_occ
 
 
 def energy_elec(mf, dm=None, h1e=None, vhf=None):
@@ -298,16 +287,25 @@
     r'''Total Hartree-Fock energy, electronic part plus nuclear repulstion
     See :func:`scf.hf.energy_elec` for the electron part
 
     Note this function has side effects which cause mf.scf_summary updated.
 
     '''
     nuc = mf.energy_nuc()
-    e_tot = mf.energy_elec(dm, h1e, vhf)[0] + nuc
     mf.scf_summary['nuc'] = nuc.real
+
+    e_tot = mf.energy_elec(dm, h1e, vhf)[0] + nuc
+    if mf.do_disp():
+        if 'dispersion' in mf.scf_summary:
+            e_tot += mf.scf_summary['dispersion']
+        else:
+            e_disp = mf.get_dispersion()
+            mf.scf_summary['dispersion'] = e_disp
+            e_tot += e_disp
+
     return e_tot
 
 
 def get_hcore(mol):
     '''Core Hamiltonian
 
     Examples:
@@ -718,22 +716,22 @@
         dm = dma + dmb
         s = get_ovlp(mol)
         _, mo_coeff = scipy.linalg.eigh(dm, s, type=2)
         dm = lib.tag_array(dm, mo_coeff=mo_coeff[:,::-1], mo_occ=mo_occ)
     return dm
 
 
-def get_init_guess(mol, key='minao'):
+def get_init_guess(mol, key='minao', **kwargs):
     '''Generate density matrix for initial guess
 
     Kwargs:
         key : str
             One of 'minao', 'atom', 'huckel', 'hcore', '1e', 'chkfile'.
     '''
-    return RHF(mol).get_init_guess(mol, key)
+    return RHF(mol).get_init_guess(mol, key, **kwargs)
 
 
 # eigenvalue of d is 1
 def level_shift(s, d, f, factor):
     r'''Apply level shift :math:`\Delta` to virtual orbitals
 
     .. math::
@@ -748,15 +746,15 @@
             0 & \text{otherwise}
          \end{cases}
        \end{align}
 
     Returns:
         New Fock matrix, 2D ndarray
     '''
-    dm_vir = s - reduce(numpy.dot, (s, d, s))
+    dm_vir = s - reduce(lib.dot, (s, d, s))
     return f + dm_vir * factor
 
 
 def damping(f, f_prev, factor):
     return f*(1-factor) + f_prev*factor
 
 
@@ -1503,16 +1501,18 @@
     >>> mf.verbose = 0
     >>> mf.level_shift = .4
     >>> mf.scf()
     -1.0811707843775884
     '''
     conv_tol = getattr(__config__, 'scf_hf_SCF_conv_tol', 1e-9)
     conv_tol_grad = getattr(__config__, 'scf_hf_SCF_conv_tol_grad', None)
+    conv_tol_cpscf = getattr(__config__, 'scf_hf_SCF_conv_tol_cpscf', 1e-8)
     max_cycle = getattr(__config__, 'scf_hf_SCF_max_cycle', 50)
     init_guess = getattr(__config__, 'scf_hf_SCF_init_guess', 'minao')
+    disp = None  # for DFT-D3 and DFT-D4
 
     # To avoid diis pollution from previous run, self.diis should not be
     # initialized as DIIS instance here
     DIIS = diis.SCF_DIIS
     diis = getattr(__config__, 'scf_hf_SCF_diis', True)
     diis_space = getattr(__config__, 'scf_hf_SCF_diis_space', 8)
     diis_damp = getattr(__config__, 'scf_hf_SCF_diis_damp', 0)
@@ -1526,32 +1526,31 @@
     direct_scf = getattr(__config__, 'scf_hf_SCF_direct_scf', True)
     direct_scf_tol = getattr(__config__, 'scf_hf_SCF_direct_scf_tol', 1e-13)
     conv_check = getattr(__config__, 'scf_hf_SCF_conv_check', True)
 
     callback = None
 
     _keys = {
-        'conv_tol', 'conv_tol_grad', 'max_cycle', 'init_guess',
+        'conv_tol', 'conv_tol_grad', 'conv_tol_cpscf', 'max_cycle', 'init_guess',
         'DIIS', 'diis', 'diis_space', 'diis_damp', 'diis_start_cycle',
         'diis_file', 'diis_space_rollback', 'damp', 'level_shift',
         'direct_scf', 'direct_scf_tol', 'conv_check', 'callback',
         'mol', 'chkfile', 'mo_energy', 'mo_coeff', 'mo_occ',
-        'e_tot', 'converged', 'scf_summary', 'opt', 'disp',
+        'e_tot', 'converged', 'scf_summary', 'opt', 'disp', 'disp_with_3body',
     }
 
     def __init__(self, mol):
         if not mol._built:
             sys.stderr.write('Warning: %s must be initialized before calling SCF.\n'
                              'Initialize %s in %s\n' % (mol, mol, self))
             mol.build()
         self.mol = mol
         self.verbose = mol.verbose
         self.max_memory = mol.max_memory
         self.stdout = mol.stdout
-        self.disp = None
 
         # If chkfile is muted, SCF intermediates will not be dumped anywhere.
         if MUTE_CHKFILE:
             self.chkfile = None
         else:
             # the chkfile will be removed automatically, to save the chkfile, assign a
             # filename to self.chkfile
@@ -1566,14 +1565,23 @@
         self.e_tot = 0
         self.converged = False
         self.scf_summary = {}
 
         self._opt = {None: None}
         self._eri = None # Note: self._eri requires large amount of memory
 
+    def check_sanity(self):
+        s1e = self.get_ovlp()
+        cond = lib.cond(s1e)
+        logger.debug(self, 'cond(S) = %s', cond)
+        if numpy.max(cond)*1e-17 > self.conv_tol:
+            logger.warn(self, 'Singularity detected in overlap matrix (condition number = %4.3g). '
+                        'SCF may be inaccurate and hard to converge.', numpy.max(cond))
+        return super().check_sanity()
+
     def build(self, mol=None):
         if mol is None: mol = self.mol
         if self.verbose >= logger.WARN:
             self.check_sanity()
         return self
 
     @property
@@ -1700,15 +1708,15 @@
     def init_guess_by_chkfile(self, chkfile=None, project=None):
         if chkfile is None: chkfile = self.chkfile
         return init_guess_by_chkfile(self.mol, chkfile, project=project)
     def from_chk(self, chkfile=None, project=None):
         return self.init_guess_by_chkfile(chkfile, project)
     from_chk.__doc__ = init_guess_by_chkfile.__doc__
 
-    def get_init_guess(self, mol=None, key='minao'):
+    def get_init_guess(self, mol=None, key='minao', **kwargs):
         if not isinstance(key, str):
             return key
 
         key = key.lower()
         if mol is None:
             mol = self.mol
         if key == '1e' or key == 'hcore':
@@ -1738,15 +1746,15 @@
 
     make_rdm1 = lib.module_method(make_rdm1, absences=['mo_coeff', 'mo_occ'])
     make_rdm2 = lib.module_method(make_rdm2, absences=['mo_coeff', 'mo_occ'])
     energy_elec = energy_elec
     energy_tot = energy_tot
 
     def energy_nuc(self):
-        return self.mol.energy_nuc()
+        return self.mol.enuc
 
     # A hook for overloading convergence criteria in SCF iterations. Assigning
     # a function
     #   f(envs) => bool
     # to check_convergence can overwrite the default convergence criteria
     check_convergence = None
 
@@ -2054,16 +2062,20 @@
         '''
         raise NotImplementedError
 
     def _transfer_attrs_(self, dst):
         '''This helper function transfers attributes from one SCF object to
         another SCF object. It is invoked by to_ks and to_hf methods.
         '''
+        # Search for all tracked attributes, including those in base classes
+        cls_keys = [getattr(cls, '_keys', ()) for cls in dst.__class__.__mro__[:-1]]
+        dst_keys = set(dst.__dict__).union(*cls_keys)
+
         loc_dic = self.__dict__
-        keys = dst.__dict__.keys() & loc_dic.keys()
+        keys = set(loc_dic).intersection(dst_keys)
         dst.__dict__.update({k: loc_dic[k] for k in keys})
         dst.converged = False
         return dst
 
     def to_gpu(self):
         '''Converts to the object with GPU support.
         '''
@@ -2099,16 +2111,16 @@
     def check_sanity(self):
         mol = self.mol
         if mol.nelectron != 1 and mol.spin != 0:
             logger.warn(self, 'Invalid number of electrons %d for RHF method.',
                         mol.nelectron)
         return SCF.check_sanity(self)
 
-    def get_init_guess(self, mol=None, key='minao'):
-        dm = SCF.get_init_guess(self, mol, key)
+    def get_init_guess(self, mol=None, key='minao', **kwargs):
+        dm = SCF.get_init_guess(self, mol, key, **kwargs)
         if self.verbose >= logger.DEBUG1:
             s = self.get_ovlp()
             nelec = numpy.einsum('ij,ji', dm, s).real
             logger.debug1(self, 'Nelec from initial guess = %s', nelec)
         return dm
 
     @lib.with_doc(get_jk.__doc__)
@@ -2189,19 +2201,16 @@
 
     def to_ks(self, xc='HF'):
         '''Convert to RKS object.
         '''
         from pyscf import dft
         return self._transfer_attrs_(dft.RKS(self.mol, xc=xc))
 
-    def to_gpu(self):
-        # FIXME: consider the density_fit, x2c and soscf decoration
-        from gpu4pyscf.scf import RHF
-        obj = SCF.reset(self.view(RHF))
-        return lib.to_gpu(obj)
+    # FIXME: consider the density_fit, x2c and soscf decoration
+    to_gpu = lib.to_gpu
 
 def _hf1e_scf(mf, *args):
     logger.info(mf, '\n')
     logger.info(mf, '******** 1 electron system ********')
     mf.converged = True
     h1e = mf.get_hcore(mf.mol)
     s1e = mf.get_ovlp(mf.mol)
```

### Comparing `pyscf-2.5.0/pyscf/scf/hf_symm.py` & `pyscf-2.6.0/pyscf/scf/hf_symm.py`

 * *Files 0% similar despite different names*

```diff
@@ -569,16 +569,15 @@
     orbsym = property(get_orbsym)
 
     get_wfnsym = get_wfnsym
     wfnsym = property(get_wfnsym)
 
     canonicalize = canonicalize
 
-    def to_gpu(self):
-        raise NotImplementedError
+    to_gpu = lib.to_gpu
 
 RHF = SymAdaptedRHF
 
 
 class SymAdaptedROHF(rohf.ROHF):
     __doc__ = hf.SCF.__doc__ + '''
     Attributes for symmetry allowed ROHF:
@@ -930,16 +929,15 @@
 
     get_orbsym = SymAdaptedRHF.get_orbsym
     orbsym = property(get_orbsym)
 
     get_wfnsym = get_wfnsym
     wfnsym = property(get_wfnsym)
 
-    def to_gpu(self):
-        raise NotImplementedError
+    to_gpu = lib.to_gpu
 
 ROHF = SymAdaptedROHF
 
 
 def _dump_mo_energy(mol, mo_energy, mo_occ, ehomo, elumo, orbsym, title='',
                     verbose=logger.DEBUG):
     log = logger.new_logger(mol, verbose)
```

### Comparing `pyscf-2.5.0/pyscf/scf/jk.py` & `pyscf-2.6.0/pyscf/scf/jk.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/scf/rohf.py` & `pyscf-2.6.0/pyscf/scf/rohf.py`

 * *Files 1% similar despite different names*

```diff
@@ -516,17 +516,15 @@
 
     def to_ks(self, xc='HF'):
         '''Convert to ROKS object.
         '''
         from pyscf import dft
         return self._transfer_attrs_(dft.ROKS(self.mol, xc=xc))
 
-    def to_gpu(self):
-        from gpu4pyscf.scf import ROHF
-        return lib.to_gpu(hf.SCF.reset(self.view(ROHF)))
+    to_gpu = lib.to_gpu
 
 
 class HF1e(ROHF):
     scf = hf._hf1e_scf
 
 
 del (WITH_META_LOWDIN)
```

### Comparing `pyscf-2.5.0/pyscf/scf/stability.py` & `pyscf-2.6.0/pyscf/scf/stability.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/scf/stability_slow.py` & `pyscf-2.6.0/pyscf/scf/stability_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/scf/ucphf.py` & `pyscf-2.6.0/pyscf/scf/ucphf.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/scf/uhf.py` & `pyscf-2.6.0/pyscf/scf/uhf.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,16 +126,16 @@
     if mol.spin == 0 and abs(dma - dmb).max() < 1e-2:
         #remove off-diagonal part of beta DM
         dmb = numpy.zeros_like(dma)
         for b0, b1, p0, p1 in mol.aoslice_by_atom():
             dmb[...,p0:p1,p0:p1] = dma[...,p0:p1,p0:p1]
     return dma, dmb
 
-def get_init_guess(mol, key='minao'):
-    return UHF(mol).get_init_guess(mol, key)
+def get_init_guess(mol, key='minao', **kwargs):
+    return UHF(mol).get_init_guess(mol, key, **kwargs)
 
 def make_rdm1(mo_coeff, mo_occ, **kwargs):
     '''One-particle density matrix in AO representation
 
     Args:
         mo_coeff : tuple of 2D ndarrays
             Orbital coefficients for alpha and beta spins. Each column is one orbital.
@@ -759,23 +759,24 @@
     >>> mf = scf.UHF(mol)
     >>> mf.kernel()
     -75.623975516256706
     >>> print('S^2 = %.7f, 2S+1 = %.7f' % mf.spin_square())
     S^2 = 0.7570150, 2S+1 = 2.0070027
     '''
 
+    init_guess_breaksym = None
+
     _keys = {"init_guess_breaksym"}
 
     def __init__(self, mol):
         hf.SCF.__init__(self, mol)
         # self.mo_coeff => [mo_a, mo_b]
         # self.mo_occ => [mo_occ_a, mo_occ_b]
         # self.mo_energy => [mo_energy_a, mo_energy_b]
         self.nelec = None
-        self.init_guess_breaksym = None
 
     @property
     def nelec(self):
         if self._nelec is not None:
             return self._nelec
         else:
             return self.mol.nelec
@@ -826,16 +827,16 @@
             mo_coeff = self.mo_coeff
         if mo_occ is None:
             mo_occ = self.mo_occ
         return make_rdm2(mo_coeff, mo_occ, **kwargs)
 
     energy_elec = energy_elec
 
-    def get_init_guess(self, mol=None, key='minao'):
-        dm = hf.SCF.get_init_guess(self, mol, key)
+    def get_init_guess(self, mol=None, key='minao', **kwargs):
+        dm = hf.SCF.get_init_guess(self, mol, key, **kwargs)
         if self.verbose >= logger.DEBUG1:
             s = self.get_ovlp()
             nelec =(numpy.einsum('ij,ji', dm[0], s).real,
                     numpy.einsum('ij,ji', dm[1], s).real)
             logger.debug1(self, 'Nelec from initial guess = %s', nelec)
         return dm
 
@@ -1062,17 +1063,15 @@
 
     def to_ks(self, xc='HF'):
         '''Convert to UKS object.
         '''
         from pyscf import dft
         return self._transfer_attrs_(dft.UKS(self.mol, xc=xc))
 
-    def to_gpu(self):
-        from gpu4pyscf.scf import UHF
-        return lib.to_gpu(hf.SCF.reset(self.view(UHF)))
+    to_gpu = lib.to_gpu
 
 def _hf1e_scf(mf, *args):
     logger.info(mf, '\n')
     logger.info(mf, '******** 1 electron system ********')
     mf.converged = True
     h1e = mf.get_hcore(mf.mol)
     s1e = mf.get_ovlp(mf.mol)
```

### Comparing `pyscf-2.5.0/pyscf/scf/uhf_symm.py` & `pyscf-2.6.0/pyscf/scf/uhf_symm.py`

 * *Files 1% similar despite different names*

```diff
@@ -561,16 +561,15 @@
     orbsym = property(get_orbsym)
 
     get_wfnsym = get_wfnsym
     wfnsym = property(get_wfnsym)
 
     canonicalize = canonicalize
 
-    def to_gpu(self):
-        raise NotImplementedError
+    to_gpu = lib.to_gpu
 
 UHF = SymAdaptedUHF
 
 
 class HF1e(UHF):
     scf = uhf._hf1e_scf
```

### Comparing `pyscf-2.5.0/pyscf/sgx/sgx.py` & `pyscf-2.6.0/pyscf/sgx/sgx.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,17 @@
 
     def post_kernel(self, envs):
         self._in_scf = False
         self._last_dm = 0
         self._last_vj = 0
         self._last_vk = 0
 
+    def to_gpu(self):
+        raise NotImplementedError
+
     def method_not_implemented(self, *args, **kwargs):
         raise NotImplementedError
     nuc_grad_method = Gradients = method_not_implemented
     Hessian = method_not_implemented
     NMR = method_not_implemented
     NSR = method_not_implemented
     Polarizability = method_not_implemented
@@ -370,7 +373,9 @@
             if with_k:
                 vk = sgx_jk.get_jk(self, dm, hermi, False, with_k, direct_scf_tol)[1]
             else:
                 vk = None
         else:
             vj, vk = sgx_jk.get_jk(self, dm, hermi, with_j, with_k, direct_scf_tol)
         return vj, vk
+
+    to_gpu = lib.to_gpu
```

### Comparing `pyscf-2.5.0/pyscf/sgx/sgx_jk.py` & `pyscf-2.6.0/pyscf/sgx/sgx_jk.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/solvent/__init__.py` & `pyscf-2.6.0/pyscf/solvent/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from pyscf.solvent import ddcosmo
+from pyscf.solvent import ddcosmo, pcm
 
 def ddCOSMO(method_or_mol, solvent_obj=None, dm=None):
     '''Initialize ddCOSMO model.
 
     Examples:
 
     >>> mf = ddCOSMO(scf.RHF(mol))
@@ -138,8 +138,32 @@
     elif isinstance(method_or_mol, mcscf.casci.CASCI):
         return pcm.pcm_for_casci(method_or_mol, solvent_obj, dm)
     elif isinstance(method_or_mol, (tdscf.rhf.TDA, tdscf.rhf.TDHF)):
         return pcm.pcm_for_tdscf(method_or_mol, solvent_obj, dm)
     else:
         return pcm.pcm_for_post_scf(method_or_mol, solvent_obj, dm)
 
-PCM = PCM
+PCM = PCM
+
+def SMD(method_or_mol, solvent_obj=None, dm=None):
+    '''Initialize PCM model.
+
+    Examples:
+
+    >>> mf = PCM(scf.RHF(mol))
+    >>> mf.kernel()
+    >>> sol = PCM(mol)
+    >>> mc = PCM(CASCI(mf, 6, 6), sol)
+    >>> mc.kernel()
+    '''
+    from pyscf import gto
+    from pyscf import scf
+    from pyscf.solvent import smd
+
+    if isinstance(method_or_mol, gto.mole.Mole):
+        return smd.SMD(method_or_mol)
+    elif isinstance(method_or_mol, scf.hf.SCF):
+        return smd.smd_for_scf(method_or_mol, solvent_obj, dm)
+    else:
+        raise NotImplementedError
+
+SMD = SMD
```

### Comparing `pyscf-2.5.0/pyscf/solvent/_attach_solvent.py` & `pyscf-2.6.0/pyscf/solvent/_attach_solvent.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,26 +103,46 @@
                                 fock_last)
 
     def energy_elec(self, dm=None, h1e=None, vhf=None):
         if dm is None:
             dm = self.make_rdm1()
         if getattr(vhf, 'e_solvent', None) is None:
             vhf = self.get_veff(self.mol, dm)
+
         e_tot, e_coul = super().energy_elec(dm, h1e, vhf)
-        e_tot += vhf.e_solvent
+        e_solvent = vhf.e_solvent
+        e_tot += e_solvent
         self.scf_summary['e_solvent'] = vhf.e_solvent.real
-        logger.debug(self, 'Solvent Energy = %.15g', vhf.e_solvent)
+
+        if (hasattr(self.with_solvent, 'method') and
+            self.with_solvent.method.upper() == 'SMD'):
+            if self.with_solvent.e_cds is None:
+                e_cds = self.with_solvent.get_cds()
+                self.with_solvent.e_cds = e_cds
+            else:
+                e_cds = self.with_solvent.e_cds
+
+            if isinstance(e_cds, numpy.ndarray):
+                e_cds = e_cds[0]
+            e_tot += e_cds
+            self.scf_summary['e_cds'] = e_cds
+            logger.info(self, f'CDS correction = {e_cds:.15f}')
+        logger.info(self, 'Solvent Energy = %.15g', vhf.e_solvent)
         return e_tot, e_coul
 
     def nuc_grad_method(self):
         grad_method = super().nuc_grad_method()
         return self.with_solvent.nuc_grad_method(grad_method)
 
     Gradients = nuc_grad_method
 
+    def Hessian(self):
+        hess_method = super().Hessian()
+        return self.with_solvent.Hessian(hess_method)
+
     def gen_response(self, *args, **kwargs):
         vind = super().gen_response(*args, **kwargs)
         is_uhf = isinstance(self, scf.uhf.UHF)
         # singlet=None is orbital hessian or CPHF type response function
         singlet = kwargs.get('singlet', True)
         singlet = singlet or singlet is None
         def vind_with_solvent(dm1):
@@ -143,14 +163,20 @@
         # If solvent was frozen, its contribution is treated as the
         # external potential. The response of solvent does not need to
         # be considered in stability analysis.
         with lib.temporary_env(self.with_solvent,
                                equilibrium_solvation=not self.with_solvent.frozen):
             return super().stability(*args, **kwargs)
 
+    def to_gpu(self):
+        from gpu4pyscf.solvent import _attach_solvent # type: ignore
+        solvent_obj = self.with_solvent.to_gpu()
+        obj = _attach_solvent._for_scf(self.undo_solvent().to_gpu(), solvent_obj)
+        return obj
+
 def _for_casscf(mc, solvent_obj, dm=None):
     '''Add solvent model to CASSCF method.
 
     Kwargs:
         dm : if given, solvent does not respond to the change of density
             matrix. A frozen ddCOSMO potential is added to the results.
     '''
@@ -280,14 +306,19 @@
 MCSCF_DM * V_solvent[d/dX MCSCF_DM] + V_solvent[MCSCF_DM] * d/dX MCSCF_DM
 ''')
         grad_method = super().nuc_grad_method()
         return self.with_solvent.nuc_grad_method(grad_method)
 
     Gradients = nuc_grad_method
 
+    def to_gpu(self):
+        obj = self.undo_solvent().to_gpu()
+        obj = _for_casscf(obj, self.with_solvent)
+        return lib.to_gpu(self, obj)
+
 
 def _for_casci(mc, solvent_obj, dm=None):
     '''Add solvent model to CASCI method.
 
     Kwargs:
         dm : if given, solvent does not respond to the change of density
             matrix. A frozen ddCOSMO potential is added to the results.
@@ -417,14 +448,19 @@
 MCSCF_DM * V_solvent[d/dX MCSCF_DM] + V_solvent[MCSCF_DM] * d/dX MCSCF_DM
 ''')
         grad_method = super().nuc_grad_method()
         return self.with_solvent.nuc_grad_method(grad_method)
 
     Gradients = nuc_grad_method
 
+    def to_gpu(self):
+        obj = self.undo_solvent().to_gpu()
+        obj = _for_casci(obj, self.with_solvent)
+        return lib.to_gpu(self, obj)
+
 
 def _for_post_scf(method, solvent_obj, dm=None):
     '''A wrapper of solvent model for post-SCF methods (CC, CI, MP etc.)
 
     NOTE: this implementation often causes (macro iteration) convergence issue
 
     Kwargs:
@@ -548,14 +584,19 @@
 DM * V_solvent[d/dX DM] + V_solvent[DM] * d/dX DM
 ''')
         grad_method = super().nuc_grad_method()
         return self.with_solvent.nuc_grad_method(grad_method)
 
     Gradients = nuc_grad_method
 
+    def to_gpu(self):
+        obj = self.undo_solvent().to_gpu()
+        obj = _for_post_scf(obj, self.with_solvent)
+        return lib.to_gpu(self, obj)
+
 
 def _for_tdscf(method, solvent_obj, dm=None):
     '''Add solvent model in TDDFT calculations.
 
     Kwargs:
         dm : if given, solvent does not respond to the change of density
             matrix. A frozen ddCOSMO potential is added to the results.
@@ -579,15 +620,15 @@
     sol_td = TDSCFWithSolvent(method, scf_with_solvent)
     name = solvent_obj.__class__.__name__ + method.__class__.__name__
     return lib.set_class(sol_td, (TDSCFWithSolvent, method.__class__), name)
 
 class TDSCFWithSolvent(_Solvation):
     _keys = {'with_solvent'}
 
-    def __init__(self, method, scf_with_solvent):
+    def __init__(self, method, scf_with_solvent=None):
         self.__dict__.update(method.__dict__)
         self._scf = scf_with_solvent
         self.with_solvent = self._scf.with_solvent
 
     def undo_solvent(self):
         cls = self.__class__
         name_mixin = self.with_solvent.__class__.__name__
@@ -626,7 +667,12 @@
         #a, b = get_ab(mf)
         if self.equilibrium_solvation:
             raise NotImplementedError
 
     def nuc_grad_method(self):
         grad_method = super().nuc_grad_method()
         return self.with_solvent.nuc_grad_method(grad_method)
+
+    def to_gpu(self):
+        obj = self.undo_solvent().to_gpu()
+        obj = _for_tdscf(obj, self.with_solvent)
+        return lib.to_gpu(self, obj)
```

### Comparing `pyscf-2.5.0/pyscf/solvent/_ddcosmo_tdscf_grad.py` & `pyscf-2.6.0/pyscf/solvent/_ddcosmo_tdscf_grad.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from pyscf.lib import logger
 from pyscf import gto
 from pyscf import scf
 from pyscf import dft
 from pyscf import df
 from pyscf.dft import numint
 from pyscf.solvent import ddcosmo
-from pyscf.solvent import ddcosmo_grad
+from pyscf.solvent.grad import ddcosmo_grad
 from pyscf.solvent._attach_solvent import _Solvation
 from pyscf.grad import rks as rks_grad
 from pyscf.grad import tdrks as tdrks_grad
 from pyscf.grad import tduks as tduks_grad
 from pyscf.scf import cphf, ucphf
```

### Comparing `pyscf-2.5.0/pyscf/solvent/ddcosmo.py` & `pyscf-2.6.0/pyscf/solvent/ddcosmo.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,14 +233,15 @@
 import numpy
 from pyscf import lib
 from pyscf.lib import logger
 from pyscf import gto
 from pyscf import df
 from pyscf.dft import gen_grid, numint
 from pyscf.data import radii
+from pyscf.solvent.grad import ddcosmo_grad
 from pyscf.symm import sph
 
 from pyscf.solvent import _attach_solvent
 
 @lib.with_doc(_attach_solvent._for_scf.__doc__)
 def ddcosmo_for_scf(mf, solvent_obj=None, dm=None):
     if solvent_obj is None:
@@ -336,17 +337,15 @@
                                             + 10*eta**2 - 15*eta + 6)
 # JCP, 139, 054111
 #    xt[on_shell] = 1./eta**4 * (1-ti)**2 * (ti-1+2*eta)**2
     return xt
 
 def make_grids_one_sphere(lebedev_order):
     ngrid_1sph = gen_grid.LEBEDEV_ORDER[lebedev_order]
-    leb_grid = numpy.empty((ngrid_1sph,4))
-    gen_grid.libdft.MakeAngularGrid(leb_grid.ctypes.data_as(ctypes.c_void_p),
-                                    ctypes.c_int(ngrid_1sph))
+    leb_grid = gen_grid.MakeAngularGrid(ngrid_1sph)
     coords_1sph = leb_grid[:,:3]
     # Note the Lebedev angular grids are normalized to 1 in pyscf
     weights_1sph = 4*numpy.pi * leb_grid[:,3]
     return coords_1sph, weights_1sph
 
 def make_L(pcmobj, r_vdw, ylm_1sph, fi):
     # See JCTC, 9, 3637, Eq (18)
@@ -858,23 +857,25 @@
     def regularize_xt(self, t, eta, scale=1):
         return regularize_xt(t, eta)
 
     def nuc_grad_method(self, grad_method):
         '''For grad_method in vacuum, add nuclear gradients of solvent
         '''
         from pyscf import tdscf
-        from pyscf.solvent import ddcosmo_grad, _ddcosmo_tdscf_grad
+        from pyscf.solvent import _ddcosmo_tdscf_grad
         if self.frozen:
             raise RuntimeError('Frozen solvent model is not supported for '
                                'energy gradients')
         if isinstance(grad_method.base, tdscf.rhf.TDBase):
             return _ddcosmo_tdscf_grad.make_grad_object(grad_method)
         else:
             return ddcosmo_grad.make_grad_object(grad_method)
 
+    to_gpu = lib.to_gpu
+
 DDCOSMO = ddCOSMO
 
 class Grids(gen_grid.Grids):
     '''DFT grids without sorting grids'''
 
     alignment = 0
```

### Comparing `pyscf-2.5.0/pyscf/solvent/ddcosmo_grad.py` & `pyscf-2.6.0/pyscf/solvent/grad/ddcosmo_grad.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/solvent/ddpcm.py` & `pyscf-2.6.0/pyscf/solvent/ddpcm.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,15 @@
                 a = numpy.einsum('xn,n,mn->xm', ylm_1sph, weights, pol[l])
                 Amat[ja,:,ka,p0:p1] += -fac * a
     return Amat
 
 class ddPCM(ddcosmo.DDCOSMO):
     def __init__(self, mol):
         ddcosmo.DDCOSMO.__init__(self, mol)
+        self.method = 'ddPCM'
 
     def dump_flags(self, verbose=None):
         logger.info(self, '******** %s (In testing) ********', self.__class__)
         logger.warn(self, 'ddPCM is an experimental feature. It is '
                     'still in testing.\nFeatures and APIs may be changed '
                     'in the future.')
         logger.info(self, 'lebedev_order = %s (%d grids per sphere)',
```

### Comparing `pyscf-2.5.0/pyscf/solvent/pcm.py` & `pyscf-2.6.0/pyscf/solvent/pcm.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 '''
 PCM family solvent models
 '''
 
 import numpy
 import scipy
-import ctypes
 from pyscf import lib
 from pyscf.lib import logger
 from pyscf import gto, df
 from pyscf.dft import gen_grid
 from pyscf.data import radii
 from pyscf.solvent import ddcosmo
 from pyscf.solvent import _attach_solvent
@@ -118,38 +117,36 @@
     3890: 4.90777965981,
     4334: 4.90782469526,
     4802: 4.90749125553,
     5294: 4.90762073452,
     5810: 4.90792902522,
 }
 
-Bondi = radii.VDW
-Bondi[1] = 1.1/radii.BOHR      # modified version
+modified_Bondi = radii.VDW.copy()
+modified_Bondi[1] = 1.1/radii.BOHR      # modified version
 PI = numpy.pi
 
 def switch_h(x):
     '''
     switching function (eq. 3.19)
     J. Chem. Phys. 133, 244111 (2010)
     notice the typo in the paper
     '''
     y = x**3 * (10.0 - 15.0*x + 6.0*x**2)
     y[x<0] = 0.0
     y[x>1] = 1.0
     return y
 
-def gen_surface(mol, ng=302, vdw_scale=1.2):
+def gen_surface(mol, ng=302, rad=modified_Bondi, vdw_scale=1.2):
     '''J. Phys. Chem. A 1999, 103, 11060-11079'''
-    unit_sphere = numpy.empty((ng,4))
-    libdft.MakeAngularGrid(unit_sphere.ctypes.data_as(ctypes.c_void_p), ctypes.c_int(ng))
-
+    unit_sphere = gen_grid.MakeAngularGrid(ng)
     atom_coords = mol.atom_coords(unit='B')
     charges = mol.atom_charges()
     N_J = ng * numpy.ones(mol.natm)
-    R_J = numpy.asarray([vdw_scale*Bondi[chg] for chg in charges])
+    R_J = numpy.asarray([rad[chg] for chg in charges])
     R_sw_J = R_J * (14.0 / N_J)**0.5
     alpha_J = 1.0/2.0 + R_J/R_sw_J - ((R_J/R_sw_J)**2 - 1.0/28)**0.5
     R_in_J = R_J - alpha_J * R_sw_J
 
     grid_coords = []
     weights = []
     charge_exp = []
@@ -158,15 +155,15 @@
     norm_vec = []
     area = []
     gslice_by_atom = []
     p0 = p1 = 0
     for ia in range(mol.natm):
         symb = mol.atom_symbol(ia)
         chg = gto.charge(symb)
-        r_vdw = vdw_scale*Bondi[chg]
+        r_vdw = rad[chg]
 
         atom_grid = r_vdw * unit_sphere[:,:3] + atom_coords[ia,:]
         riJ = scipy.spatial.distance.cdist(atom_grid[:,:3], atom_coords)
         diJ = (riJ - R_in_J) / R_sw_J
         diJ[:,ia] = 1.0
         diJ[diJ < 1e-8] = 0.0
         fiJ = switch_h(diJ)
@@ -247,68 +244,102 @@
 
         D = S*nrij/rij**2 -2.0*xi_r_ij/PI**0.5*numpy.exp(-xi_r_ij**2)*nrij/rij**3
         numpy.fill_diagonal(D, -charge_exp * (2.0 / PI)**0.5 / (2.0 * R_vdw))
 
     return D, S
 
 
-class PCM(ddcosmo.DDCOSMO):
+class PCM(lib.StreamObject):
+    _keys = {
+        'method', 'vdw_scale', 'surface', 'r_probe', 'intopt',
+        'mol', 'radii_table', 'atom_radii', 'lebedev_order', 'lmax', 'eta',
+        'eps', 'max_cycle', 'conv_tol', 'state_id', 'frozen',
+        'equilibrium_solvation', 'e', 'v', 'v_grids_n',
+    }
+
+    kernel = ddcosmo.DDCOSMO.kernel
+
     def __init__(self, mol):
-        ddcosmo.DDCOSMO.__init__(self, mol)
+        self.mol = mol
+        self.stdout = mol.stdout
+        self.verbose = mol.verbose
+        self.max_memory = mol.max_memory
         self.method = 'C-PCM'
+
         self.vdw_scale = 1.2 # default value in qchem
         self.surface = {}
+        self.r_probe = 0.0
+        self.radii_table = None
+        self.atom_radii = None
         self.lebedev_order = 29
         self._intermediates = {}
+        self.eps = 78.3553
+
+        self.max_cycle = 20
+        self.conv_tol = 1e-7
+        self.state_id = 0
+
+        self.frozen = False
+        self.equilibrium_solvation = False
+
+        self.e = None
+        self.v = None
+        self._dm = None
 
     def dump_flags(self, verbose=None):
         logger.info(self, '******** %s (In testing) ********', self.__class__)
         logger.warn(self, 'PCM is an experimental feature. It is '
                     'still in testing.\nFeatures and APIs may be changed '
                     'in the future.')
         logger.info(self, 'lebedev_order = %s (%d grids per sphere)',
                     self.lebedev_order, gen_grid.LEBEDEV_ORDER[self.lebedev_order])
-        logger.info(self, 'lmax = %s'         , self.lmax)
-        logger.info(self, 'eta = %s'          , self.eta)
         logger.info(self, 'eps = %s'          , self.eps)
         logger.info(self, 'frozen = %s'       , self.frozen)
         logger.info(self, 'equilibrium_solvation = %s', self.equilibrium_solvation)
         logger.debug2(self, 'radii_table %s', self.radii_table)
         if self.atom_radii:
             logger.info(self, 'User specified atomic radii %s', str(self.atom_radii))
-        self.grids.dump_flags(verbose)
         return self
 
+    def to_gpu(self):
+        from pyscf.lib import to_gpu
+        obj = to_gpu(self)
+        return obj.reset()
+
     def reset(self, mol=None):
+        if mol is not None:
+            self.mol = mol
+        self._intermediates = None
         self.surface = None
-        super().reset(mol)
+        self.intopt = None
         return self
 
     def build(self, ng=None):
-        vdw_scale = self.vdw_scale
-        self.radii_table = vdw_scale * Bondi
+        if self.radii_table is None:
+            vdw_scale = self.vdw_scale
+            self.radii_table = vdw_scale * modified_Bondi + self.r_probe
         mol = self.mol
         if ng is None:
             ng = gen_grid.LEBEDEV_ORDER[self.lebedev_order]
 
-        self.surface = gen_surface(mol, ng=ng, vdw_scale=vdw_scale)
+        self.surface = gen_surface(mol, rad=self.radii_table, ng=ng)
         self._intermediates = {}
         F, A = get_F_A(self.surface)
         D, S = get_D_S(self.surface, with_S=True, with_D=True)
 
         epsilon = self.eps
-        if self.method.upper() == 'C-PCM':
+        if self.method.upper() in ['C-PCM', 'CPCM']:
             f_epsilon = (epsilon-1.)/epsilon
             K = S
             R = -f_epsilon * numpy.eye(K.shape[0])
         elif self.method.upper() == 'COSMO':
             f_epsilon = (epsilon - 1.0)/(epsilon + 1.0/2.0)
             K = S
             R = -f_epsilon * numpy.eye(K.shape[0])
-        elif self.method.upper() == 'IEF-PCM':
+        elif self.method.upper() in ['IEF-PCM', 'IEFPCM']:
             f_epsilon = (epsilon - 1.0)/(epsilon + 1.0)
             DA = D*A
             DAS = numpy.dot(DA, S)
             K = S - f_epsilon/(2.0*PI) * DAS
             R = -f_epsilon * (numpy.eye(K.shape[0]) - 1.0/(2.0*PI)*DA)
         elif self.method.upper() == 'SS(V)PE':
             f_epsilon = (epsilon - 1.0)/(epsilon + 1.0)
@@ -325,83 +356,133 @@
             'A': A,
             'K': K,
             'R': R,
             'f_epsilon': f_epsilon
         }
         self._intermediates.update(intermediates)
 
+        charge_exp  = self.surface['charge_exp']
+        grid_coords = self.surface['grid_coords']
+        atom_coords = mol.atom_coords(unit='B')
+        atom_charges = mol.atom_charges()
+
+        int2c2e = mol._add_suffix('int2c2e')
+        fakemol = gto.fakemol_for_charges(grid_coords, expnt=charge_exp**2)
+        fakemol_nuc = gto.fakemol_for_charges(atom_coords)
+        v_ng = gto.mole.intor_cross(int2c2e, fakemol_nuc, fakemol)
+        self.v_grids_n = numpy.dot(atom_charges, v_ng)
+
     def _get_vind(self, dms):
-        if not self._intermediates or self.grids.coords is None:
+        if not self._intermediates:
             self.build()
 
         nao = dms.shape[-1]
         dms = dms.reshape(-1,nao,nao)
+        if dms.shape[0] == 2:
+            dms = (dms[0] + dms[1]).reshape(-1,nao,nao)
 
         K = self._intermediates['K']
         R = self._intermediates['R']
-        v_grids = self._get_v(self.surface, dms)
-        b = numpy.dot(R, v_grids)
-        q = numpy.linalg.solve(K, b)
+        v_grids_e = self._get_v(dms)
+        v_grids = self.v_grids_n - v_grids_e
 
-        vK_1 = numpy.linalg.solve(K.T, v_grids)
-        q_sym = (q + numpy.dot(R.T, vK_1))/2.0
+        b = numpy.dot(R, v_grids.T)
+        q = numpy.linalg.solve(K, b).T
 
-        vmat = self._get_vmat(q_sym)
-        epcm = 0.5 * numpy.dot(q_sym, v_grids)
+        vK_1 = numpy.linalg.solve(K.T, v_grids.T)
+        qt = numpy.dot(R.T, vK_1).T
+        q_sym = (q + qt)/2.0
 
-        self._intermediates['K'] = K
-        self._intermediates['R'] = R
-        self._intermediates['q'] = q
-        self._intermediates['q_sym'] = q_sym
-        self._intermediates['v_grids'] = v_grids
+        vmat = self._get_vmat(q_sym)
+        epcm = 0.5 * numpy.dot(q_sym[0], v_grids[0])
 
-        return epcm, vmat
+        self._intermediates['q'] = q[0]
+        self._intermediates['q_sym'] = q_sym[0]
+        self._intermediates['v_grids'] = v_grids[0]
+        self._intermediates['dm'] = dms
+        return epcm, vmat[0]
 
-    def _get_v(self, surface, dms):
+    def _get_v(self, dms):
         '''
         return electrostatic potential on surface
         '''
         mol = self.mol
         nao = dms.shape[-1]
-        atom_coords = mol.atom_coords(unit='B')
-        atom_charges = mol.atom_charges()
-        grid_coords = surface['grid_coords']
-        exponents   = surface['charge_exp']
-
+        grid_coords = self.surface['grid_coords']
+        exponents   = self.surface['charge_exp']
+        ngrids = grid_coords.shape[0]
+        nset = dms.shape[0]
+        v_grids_e = numpy.empty([nset, ngrids])
         max_memory = self.max_memory - lib.current_memory()[0]
         blksize = int(max(max_memory*.9e6/8/nao**2, 400))
-        ngrids = grid_coords.shape[0]
         int3c2e = mol._add_suffix('int3c2e')
         cintopt = gto.moleintor.make_cintopt(mol._atm, mol._bas, mol._env, int3c2e)
-        v_grids_e = numpy.empty(ngrids)
         for p0, p1 in lib.prange(0, ngrids, blksize):
             fakemol = gto.fakemol_for_charges(grid_coords[p0:p1], expnt=exponents[p0:p1]**2)
             v_nj = df.incore.aux_e2(mol, fakemol, intor=int3c2e, aosym='s1', cintopt=cintopt)
-            v_grids_e[p0:p1] = numpy.einsum('ijL,ij->L',v_nj, dms[0])
+            for i in range(nset):
+                v_grids_e[i,p0:p1] = numpy.einsum('ijL,ij->L',v_nj, dms[i])
 
-        int2c2e = mol._add_suffix('int2c2e')
-
-        fakemol_nuc = gto.fakemol_for_charges(atom_coords)
-        v_ng = gto.mole.intor_cross(int2c2e, fakemol_nuc, fakemol)
-        v_grids_n = numpy.dot(atom_charges, v_ng)
-
-        v_grids = v_grids_n - v_grids_e
-        return v_grids
+        return v_grids_e
 
     def _get_vmat(self, q):
         mol = self.mol
         nao = mol.nao
         grid_coords = self.surface['grid_coords']
         exponents   = self.surface['charge_exp']
-
+        ngrids = grid_coords.shape[0]
+        q = q.reshape([-1,ngrids])
+        nset = q.shape[0]
+        vmat = numpy.zeros([nset,nao,nao])
         max_memory = self.max_memory - lib.current_memory()[0]
         blksize = int(max(max_memory*.9e6/8/nao**2, 400))
-        ngrids = grid_coords.shape[0]
+
         int3c2e = mol._add_suffix('int3c2e')
         cintopt = gto.moleintor.make_cintopt(mol._atm, mol._bas, mol._env, int3c2e)
-        vmat = numpy.zeros([nao,nao])
         for p0, p1 in lib.prange(0, ngrids, blksize):
-            fakemol = gto.fakemol_for_charges(grid_coords[p0:p1], expnt=exponents**2)
+            fakemol = gto.fakemol_for_charges(grid_coords[p0:p1], expnt=exponents[p0:p1]**2)
             v_nj = df.incore.aux_e2(mol, fakemol, intor=int3c2e, aosym='s1', cintopt=cintopt)
-            vmat += -numpy.einsum('ijL,L->ij', v_nj, q[p0:p1])
+            for i in range(nset):
+                vmat[i] += -numpy.einsum('ijL,L->ij', v_nj, q[i,p0:p1])
         return vmat
 
+    def nuc_grad_method(self, grad_method):
+        from pyscf.solvent.grad import pcm as pcm_grad
+        if self.frozen:
+            raise RuntimeError('Frozen solvent model is not supported')
+        from pyscf import scf
+        from pyscf.solvent import _ddcosmo_tdscf_grad
+        if isinstance(grad_method.base, tdscf.rhf.TDBase):
+            return _ddcosmo_tdscf_grad.make_grad_object(grad_method)
+        else:
+            return pcm_grad.make_grad_object(grad_method)
+
+    def Hessian(self, hess_method):
+        from pyscf.solvent.hessian import pcm as pcm_hess
+        if self.frozen:
+            raise RuntimeError('Frozen solvent model is not supported')
+        from pyscf import scf
+        if isinstance(hess_method.base, (scf.hf.RHF, scf.uhf.UHF)):
+            return pcm_hess.make_hess_object(hess_method)
+        else:
+            raise RuntimeError('Only SCF gradient is supported')
+
+    def _B_dot_x(self, dms):
+        if not self._intermediates:
+            self.build()
+        out_shape = dms.shape
+        nao = dms.shape[-1]
+        dms = dms.reshape(-1,nao,nao)
+
+        K = self._intermediates['K']
+        R = self._intermediates['R']
+        v_grids = -self._get_v(dms)
+
+        b = numpy.dot(R, v_grids.T)
+        q = numpy.linalg.solve(K, b).T
+
+        vK_1 = numpy.linalg.solve(K.T, v_grids.T)
+        qt = numpy.dot(R.T, vK_1).T
+        q_sym = (q + qt)/2.0
+
+        vmat = self._get_vmat(q_sym)
+        return vmat.reshape(out_shape)
```

### Comparing `pyscf-2.5.0/pyscf/solvent/pol_embed.py` & `pyscf-2.6.0/pyscf/solvent/pol_embed.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/soscf/__init__.py` & `pyscf-2.6.0/pyscf/soscf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/soscf/ciah.py` & `pyscf-2.6.0/pyscf/soscf/ciah.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/soscf/newton_ah.py` & `pyscf-2.6.0/pyscf/soscf/newton_ah.py`

 * *Files 1% similar despite different names*

```diff
@@ -796,14 +796,17 @@
                                    self.mo_coeff[:,idx]))
             log.debug('Overlap to initial guess, SVD = %s',
                       _effective_svd(s, 1e-5))
             log.debug('Overlap to last step, SVD = %s',
                       _effective_svd(u[idx][:,idx], 1e-5))
         return mo
 
+    def to_gpu(self):
+        return self.undo_soscf().to_gpu()
+
 class _SecondOrderROHF(_CIAH_SOSCF):
     gen_g_hop = gen_g_hop_rohf
 
 class _SecondOrderUHF(_CIAH_SOSCF):
     gen_g_hop = gen_g_hop_uhf
 
     def update_rotate_matrix(self, dx, mo_occ, u0=1, mo_coeff=None):
```

### Comparing `pyscf-2.5.0/pyscf/symm/Dmatrix.py` & `pyscf-2.6.0/pyscf/symm/Dmatrix.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/symm/__init__.py` & `pyscf-2.6.0/pyscf/symm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/symm/addons.py` & `pyscf-2.6.0/pyscf/symm/addons.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/symm/basis.py` & `pyscf-2.6.0/pyscf/symm/basis.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/symm/cg.py` & `pyscf-2.6.0/pyscf/symm/cg.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/symm/geom.py` & `pyscf-2.6.0/pyscf/symm/geom.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,18 +45,14 @@
 from pyscf.lib import logger
 from pyscf.lib.exceptions import PointGroupSymmetryError
 from pyscf.symm.param import OPERATOR_TABLE
 from pyscf import __config__
 
 TOLERANCE = getattr(__config__, 'symm_geom_tol', 1e-5)
 
-# For code compatibility in python-2 and python-3
-if sys.version_info >= (3,):
-    unicode = str
-
 
 def parallel_vectors(v1, v2, tol=TOLERANCE):
     if numpy.allclose(v1, 0, atol=tol) or numpy.allclose(v2, 0, atol=tol):
         return True
     else:
         cos = numpy.dot(_normalize(v1), _normalize(v2))
         return (abs(cos-1) < TOLERANCE) | (abs(cos+1) < TOLERANCE)
@@ -398,15 +394,15 @@
 
 def as_subgroup(topgroup, axes, subgroup=None):
     from pyscf.symm import std_symb
     from pyscf.symm.param import SUBGROUP
 
     groupname, axes = get_subgroup(topgroup, axes)
 
-    if isinstance(subgroup, (str, unicode)):
+    if isinstance(subgroup, str):
         subgroup = std_symb(subgroup)
         if groupname == 'C2v' and subgroup == 'Cs':
             axes = numpy.einsum('ij,kj->ki', rotation_mat(axes[1], numpy.pi/2), axes)
 
         elif (groupname == 'D2' and re.search(r'D\d+d', topgroup) and
               subgroup in ('C2v', 'Cs')):
             # Special treatment for D2d, D4d, .... get_subgroup gives D2 by
@@ -463,15 +459,15 @@
         coords0 = coords[idx0]
         opdic = symm_ops(gpname)
         newc = numpy.dot(coords, opdic['sz'])
         idx1 = argsort_coords(newc)
         dup_atom_ids = numpy.sort((idx0,idx1), axis=0).T
         uniq_idx = numpy.unique(dup_atom_ids[:,0], return_index=True)[1]
         eql_atom_ids = dup_atom_ids[uniq_idx]
-        eql_atom_ids = [list(sorted(set(i))) for i in eql_atom_ids]
+        eql_atom_ids = [sorted(set(i)) for i in eql_atom_ids]
         return eql_atom_ids
     elif gpname == 'Coov':
         eql_atom_ids = [[i] for i,a in enumerate(atoms)]
         return eql_atom_ids
 
     coords = numpy.array([a[1] for a in atoms])
 
@@ -492,15 +488,15 @@
         if not numpy.allclose(coords0, newc[idx], atol=TOLERANCE):
             raise PointGroupSymmetryError('Symmetry identical atoms not found')
         dup_atom_ids.append(idx)
 
     dup_atom_ids = numpy.sort(dup_atom_ids, axis=0).T
     uniq_idx = numpy.unique(dup_atom_ids[:,0], return_index=True)[1]
     eql_atom_ids = dup_atom_ids[uniq_idx]
-    eql_atom_ids = [list(sorted(set(i))) for i in eql_atom_ids]
+    eql_atom_ids = [sorted(set(i)) for i in eql_atom_ids]
     return eql_atom_ids
 
 def check_symm(gpname, atoms, basis=None):
     '''
     Check whether the declared symmetry (gpname) exists in the system
 
     If basis is specified, this function checks also the basis functions have
```

### Comparing `pyscf-2.5.0/pyscf/symm/msym.py` & `pyscf-2.6.0/pyscf/symm/msym.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/symm/param.py` & `pyscf-2.6.0/pyscf/symm/param.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/symm/sph.py` & `pyscf-2.6.0/pyscf/symm/sph.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/tddft/__init__.py` & `pyscf-2.6.0/pyscf/tddft/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/tdscf/__init__.py` & `pyscf-2.6.0/pyscf/tdscf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/tdscf/common_slow.py` & `pyscf-2.6.0/pyscf/tdscf/common_slow.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,23 @@
 that, unlike other 'fast' routines with an implicit construction of the eigenvalue problem, these modules construct
 TDHF matrices explicitly. As a result, regular `numpy.linalg.eig` can be used to retrieve TDHF roots in a reliable
 fashion without any issues related to the Davidson procedure.
 
 This is a helper module defining basic interfaces.
 """
 
-import sys
 from pyscf.lib import logger
 
 from pyscf.pbc.tools import get_kconserv
 
 import numpy
 from scipy.linalg import solve
 
 from itertools import count, groupby
 
-if sys.version_info >= (3,):
-    unicode = str
 
 def msize(m):
     """
     Checks whether the matrix is square and returns its size.
 
     Args:
         m (numpy.ndarray): the matrix to measure;
@@ -158,15 +155,15 @@
 
     @staticmethod
     def __check_primary_form__(m):
         if not isinstance(m, tuple):
             raise ValueError("The value returned by `tdhf_primary_form` is not a tuple")
         if len(m) < 1:
             raise ValueError("Empty tuple returned by `tdhf_primary_form`")
-        if not isinstance(m[0], (str, unicode)):
+        if not isinstance(m[0], str):
             raise ValueError("The first item returned by `tdhf_primary_form` must be a string")
         forms = {"ab": 3, "mk": 3, "full": 2}
         if m[0] in forms:
             if len(m) != forms[m[0]]:
                 raise ValueError("The {} form returned by `tdhf_primary_form` must contain {:d} values".format(
                     m[0].upper(), forms[m[0]],
                 ))
```

### Comparing `pyscf-2.5.0/pyscf/tdscf/dhf.py` & `pyscf-2.6.0/pyscf/tdscf/dhf.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         b = b - numpy.einsum('jaib->iajb', eri_mo[:nocc,nocc:,:nocc,nocc:]) * hyb
         return a, b
 
     if isinstance(mf, dft.KohnShamDFT):
         from pyscf.dft import xc_deriv
         ni = mf._numint
         ni.libxc.test_deriv_order(mf.xc, 2, raise_error=True)
-        if mf.nlc or ni.libxc.is_nlc(mf.xc):
+        if mf.do_nlc():
             raise NotImplementedError('DKS-TDDFT for NLC functionals')
 
         omega, alpha, hyb = ni.rsh_and_hybrid_coeff(mf.xc, mol.spin)
 
         a, b = add_hf_(a, b, hyb)
 
         xctype = ni._xc_type(mf.xc)
```

### Comparing `pyscf-2.5.0/pyscf/tdscf/dks.py` & `pyscf-2.6.0/pyscf/tdscf/dks.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/tdscf/ghf.py` & `pyscf-2.6.0/pyscf/tdscf/ghf.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         b -= numpy.einsum('jaib->iajb', eri_mo[:nocc,nocc:,:nocc,nocc:]) * hyb
         return a, b
 
     if isinstance(mf, dft.KohnShamDFT):
         from pyscf.dft import xc_deriv
         ni = mf._numint
         ni.libxc.test_deriv_order(mf.xc, 2, raise_error=True)
-        if mf.nlc or ni.libxc.is_nlc(mf.xc):
+        if mf.do_nlc():
             raise NotImplementedError('DKS-TDDFT NLC functional')
 
         if not mf.collinear:
             raise NotImplementedError
 
         omega, alpha, hyb = ni.rsh_and_hybrid_coeff(mf.xc, mol.spin)
```

### Comparing `pyscf-2.5.0/pyscf/tdscf/gks.py` & `pyscf-2.6.0/pyscf/tdscf/gks.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/tdscf/proxy.py` & `pyscf-2.6.0/pyscf/tdscf/proxy.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/tdscf/rhf.py` & `pyscf-2.6.0/pyscf/tdscf/rhf.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         b += numpy.einsum('iajb->iajb', eri_mo[:nocc,nocc:,:nocc,nocc:]) * 2
         b -= numpy.einsum('jaib->iajb', eri_mo[:nocc,nocc:,:nocc,nocc:]) * hyb
 
     if isinstance(mf, scf.hf.KohnShamDFT):
         from pyscf.dft import xc_deriv
         ni = mf._numint
         ni.libxc.test_deriv_order(mf.xc, 2, raise_error=True)
-        if mf.nlc or ni.libxc.is_nlc(mf.xc):
+        if mf.do_nlc():
             logger.warn(mf, 'NLC functional found in DFT object.  Its second '
                         'deriviative is not available. Its contribution is '
                         'not included in the response function.')
         omega, alpha, hyb = ni.rsh_and_hybrid_coeff(mf.xc, mol.spin)
 
         add_hf_(a, b, hyb)
 
@@ -760,14 +760,17 @@
         '''Hook for dumping results and clearing up the object.'''
         if not all(self.converged):
             logger.note(self, 'TD-SCF states %s not converged.',
                         [i for i, x in enumerate(self.converged) if not x])
         logger.note(self, 'Excited State energies (eV)\n%s', self.e * nist.HARTREE2EV)
         return self
 
+    def to_gpu(self):
+        raise NotImplementedError
+
 class TDA(TDBase):
     '''Tamm-Dancoff approximation
 
     Attributes:
         conv_tol : float
             Diagonalization convergence tolerance.  Default is 1e-9.
         nstates : int
@@ -862,14 +865,16 @@
             lib.chkfile.save(self.chkfile, 'tddft/e', self.e)
             lib.chkfile.save(self.chkfile, 'tddft/xy', self.xy)
 
         log.timer('TDA', *cpu0)
         self._finalize()
         return self.e, self.xy
 
+    to_gpu = lib.to_gpu
+
 CIS = TDA
 
 
 def gen_tdhf_operation(mf, fock_ao=None, singlet=True, wfnsym=None):
     '''Generate function to compute
 
     [ A  B][X]
@@ -1040,14 +1045,16 @@
         self._finalize()
         return self.e, self.xy
 
     def nuc_grad_method(self):
         from pyscf.grad import tdrhf
         return tdrhf.Gradients(self)
 
+    to_gpu = lib.to_gpu
+
 RPA = TDRHF = TDHF
 
 scf.hf.RHF.TDA = lib.class_as_method(TDA)
 scf.hf.RHF.TDHF = lib.class_as_method(TDHF)
 scf.rohf.ROHF.TDA = None
 scf.rohf.ROHF.TDHF = None
 scf.hf_symm.ROHF.TDA = None
```

### Comparing `pyscf-2.5.0/pyscf/tdscf/rhf_slow.py` & `pyscf-2.6.0/pyscf/tdscf/rhf_slow.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/tdscf/rks.py` & `pyscf-2.6.0/pyscf/tdscf/rks.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/tdscf/uhf.py` & `pyscf-2.6.0/pyscf/tdscf/uhf.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         a_ab += numpy.einsum('iabj->iajb', eri_ab[:nocc_a,nocc_a:,nocc_b:,:nocc_b])
         b_ab += numpy.einsum('iajb->iajb', eri_ab[:nocc_a,nocc_a:,:nocc_b,nocc_b:])
 
     if isinstance(mf, scf.hf.KohnShamDFT):
         from pyscf.dft import xc_deriv
         ni = mf._numint
         ni.libxc.test_deriv_order(mf.xc, 2, raise_error=True)
-        if mf.nlc or ni.libxc.is_nlc(mf.xc):
+        if mf.do_nlc():
             logger.warn(mf, 'NLC functional found in DFT object.  Its second '
                         'deriviative is not available. Its contribution is '
                         'not included in the response function.')
         omega, alpha, hyb = ni.rsh_and_hybrid_coeff(mf.xc, mol.spin)
 
         add_hf_(a, b, hyb)
 
@@ -686,14 +686,16 @@
             lib.chkfile.save(self.chkfile, 'tddft/e', self.e)
             lib.chkfile.save(self.chkfile, 'tddft/xy', self.xy)
 
         log.timer('TDA', *cpu0)
         self._finalize()
         return self.e, self.xy
 
+    to_gpu = lib.to_gpu
+
 CIS = TDA
 
 
 def gen_tdhf_operation(mf, fock_ao=None, singlet=True, wfnsym=None):
     '''Generate function to compute
 
     [ A  B][X]
@@ -854,13 +856,15 @@
             lib.chkfile.save(self.chkfile, 'tddft/e', self.e)
             lib.chkfile.save(self.chkfile, 'tddft/xy', self.xy)
 
         log.timer('TDDFT', *cpu0)
         self._finalize()
         return self.e, self.xy
 
+    to_gpu = lib.to_gpu
+
 RPA = TDUHF = TDHF
 
 scf.uhf.UHF.TDA = lib.class_as_method(TDA)
 scf.uhf.UHF.TDHF = lib.class_as_method(TDHF)
 
 del (OUTPUT_THRESHOLD)
```

### Comparing `pyscf-2.5.0/pyscf/tdscf/uks.py` & `pyscf-2.6.0/pyscf/tdscf/uks.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/tools/__init__.py` & `pyscf-2.6.0/pyscf/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/tools/c60struct.py` & `pyscf-2.6.0/pyscf/tools/c60struct.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/tools/chgcar.py` & `pyscf-2.6.0/pyscf/tools/chgcar.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,27 +20,23 @@
 '''
 Vasp CHGCAR file format
 
 See also
 https://cms.mpi.univie.ac.at/vasp/vasp/CHGCAR_file.html
 '''
 
-import sys
 import collections
 import time
 import numpy
 import pyscf
 from pyscf import lib
 from pyscf import gto
 from pyscf.pbc import gto as pbcgto
 from pyscf.tools import cubegen
 
-if sys.version_info >= (3,):
-    unicode = str
-
 RESOLUTION = cubegen.RESOLUTION
 BOX_MARGIN = cubegen.BOX_MARGIN
 
 
 def density(cell, outfile, dm, nx=60, ny=60, nz=60, resolution=RESOLUTION):
     '''Calculates electron density and write out in CHGCAR format.
 
@@ -165,15 +161,15 @@
             self.box = numpy.diag(box)
             lib.logger.warn(cell, 'Molecular system is found. FFT-grid is not '
                             'available for Molecule. Lattice (in Bohr)\n'
                             '%s\nand FFT grids %s are applied.',
                             self.box, (nx,ny,nz))
             self.mol = cell
             cell = cell.view(pbcgto.Cell)
-            if (isinstance(cell.unit, (str, unicode)) and
+            if (isinstance(cell.unit, str) and
                 cell.unit.startswith(('B','b','au','AU'))):
                 cell.a = self.box
             else:
                 cell.a = self.box * lib.param.BOHR
             ptr = cell._atm[:,gto.PTR_COORD]
             cell._env[ptr+0] = coord[:,0] - boxorig[0]
             cell._env[ptr+1] = coord[:,1] - boxorig[1]
```

### Comparing `pyscf-2.5.0/pyscf/tools/chkfile_util.py` & `pyscf-2.6.0/pyscf/tools/chkfile_util.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/tools/cubegen.py` & `pyscf-2.6.0/pyscf/tools/cubegen.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/tools/dump_mat.py` & `pyscf-2.6.0/pyscf/tools/dump_mat.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/tools/fcidump.py` & `pyscf-2.6.0/pyscf/tools/fcidump.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/tools/mo_mapping.py` & `pyscf-2.6.0/pyscf/tools/mo_mapping.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/tools/molden.py` & `pyscf-2.6.0/pyscf/tools/molden.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/tools/ring.py` & `pyscf-2.6.0/pyscf/tools/ring.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/tools/wfn_format.py` & `pyscf-2.6.0/pyscf/tools/wfn_format.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/x2c/__init__.py` & `pyscf-2.6.0/pyscf/x2c/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/x2c/_response_functions.py` & `pyscf-2.6.0/pyscf/x2c/_response_functions.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/x2c/dft.py` & `pyscf-2.6.0/pyscf/x2c/dft.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/x2c/newton_ah.py` & `pyscf-2.6.0/pyscf/x2c/newton_ah.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/x2c/sfx2c1e.py` & `pyscf-2.6.0/pyscf/x2c/sfx2c1e.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,16 +124,17 @@
             nao = mol.nao_nr()
             dm = dm[:nao,:nao] + dm[nao:,nao:]
 
         with mol.with_common_orig((0,0,0)):
             if picture_change:
                 xmol = self.with_x2c.get_xmol()[0]
                 nao = xmol.nao
-                prp = xmol.intor_symmetric('int1e_sprsp').reshape(3,4,nao,nao)[:,0]
-                ao_dip = self.with_x2c.picture_change(('int1e_r', prp))
+                prp = xmol.intor_symmetric('int1e_sprsp').reshape(3,4,nao,nao)[:,3]
+                c1 = 0.5/lib.param.LIGHT_SPEED
+                ao_dip = self.with_x2c.picture_change(('int1e_r', prp*c1**2))
             else:
                 ao_dip = mol.intor_symmetric('int1e_r')
 
         el_dip = numpy.einsum('xij,ji->x', ao_dip, dm).real
 
         charges = mol.atom_charges()
         coords  = mol.atom_coords()
@@ -150,14 +151,18 @@
     def _transfer_attrs_(self, dst):
         if self.with_x2c and not hasattr(dst, 'with_x2c'):
             logger.warn(self, 'Destination object of to_hf/to_ks method is not '
                         'an X2C object. Convert dst to X2C object.')
             dst = dst.sfx2c()
         return hf.SCF._transfer_attrs_(self, dst)
 
+    def to_gpu(self):
+        obj = self.undo_x2c().to_gpu().sfx2c1e()
+        return lib.to_gpu(self, obj)
+
 
 class SpinFreeX2CHelper(x2c.X2CHelperBase):
     '''1-component X2c (spin-free part only)
     '''
     def get_hcore(self, mol=None):
         '''1-component X2c Foldy-Wouthuysen (FW Hamiltonian  (spin-free part only)
         '''
```

### Comparing `pyscf-2.5.0/pyscf/x2c/sfx2c1e_grad.py` & `pyscf-2.6.0/pyscf/x2c/sfx2c1e_grad.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/x2c/sfx2c1e_hess.py` & `pyscf-2.6.0/pyscf/x2c/sfx2c1e_hess.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/x2c/stability.py` & `pyscf-2.6.0/pyscf/x2c/stability.py`

 * *Files identical despite different names*

### Comparing `pyscf-2.5.0/pyscf/x2c/tdscf.py` & `pyscf-2.6.0/pyscf/x2c/tdscf.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         b = b - numpy.einsum('jaib->iajb', eri_mo[:nocc,nocc:,:nocc,nocc:]) * hyb
         return a, b
 
     if isinstance(mf, dft.KohnShamDFT):
         from pyscf.dft import xc_deriv
         ni = mf._numint
         ni.libxc.test_deriv_order(mf.xc, 2, raise_error=True)
-        if mf.nlc or ni.libxc.is_nlc(mf.xc):
+        if mf.do_nlc():
             raise NotImplementedError('X2C-TDDFT for NLC functionals')
 
         if not mf.collinear:
             raise NotImplementedError
 
         omega, alpha, hyb = ni.rsh_and_hybrid_coeff(mf.xc, mol.spin)
```

### Comparing `pyscf-2.5.0/pyscf/x2c/x2c.py` & `pyscf-2.6.0/pyscf/x2c/x2c.py`

 * *Files 1% similar despite different names*

```diff
@@ -655,14 +655,16 @@
         Note this conversion only changes the class of the mean-field object.
         The total energy and wave-function are the same as them in the input
         mean-field object.
         '''
         from pyscf.x2c import dft
         return self._transfer_attrs_(dft.UKS(self.mol, xc=xc))
 
+    to_gpu = lib.to_gpu
+
 X2C_UHF = UHF
 
 class RHF(SCF):
     def __init__(self, mol):
         super().__init__(mol)
         if dhf.zquatev is None:
             raise RuntimeError('zquatev library is required to perform Kramers-restricted X2C-RHF')
@@ -676,14 +678,16 @@
         Note this conversion only changes the class of the mean-field object.
         The total energy and wave-function are the same as them in the input
         mean-field object.
         '''
         from pyscf.x2c import dft
         return self._transfer_attrs_(dft.RKS(self.mol, xc=xc))
 
+    to_gpu = lib.to_gpu
+
 X2C_RHF = RHF
 
 def x2c1e_ghf(mf):
     '''
     For the given *GHF* object, generate X2C-GSCF object in GHF spin-orbital
     basis. Note the orbital basis of X2C_GSCF is different to the X2C_RHF and
     X2C_UHF objects. X2C_RHF and X2C_UHF use spinor basis.
@@ -795,14 +799,18 @@
                         'an X2C object. Convert dst to X2C object.')
             dst = dst.x2c()
         return hf.SCF._transfer_attrs_(self, dst)
 
     def to_ks(self, xc='HF'):
         raise NotImplementedError
 
+    def to_gpu(self):
+        obj = self.undo_x2c().to_gpu().x2c1e()
+        return lib.to_gpu(self, obj)
+
 
 def _uncontract_mol(mol, xuncontract=None, exp_drop=0.2):
     '''mol._basis + uncontracted steep functions'''
     pmol, contr_coeff = mol.decontract_basis(atoms=xuncontract)
     contr_coeff = scipy.linalg.block_diag(*contr_coeff)
     return pmol, contr_coeff
```

### Comparing `pyscf-2.5.0/pyscf.egg-info/SOURCES.txt` & `pyscf-2.6.0/pyscf.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 CHANGELOG
 LICENSE
 MANIFEST.in
 NOTICE
 README.md
-setup.cfg
+pyproject.toml
 setup.py
 pyscf/__all__.py
 pyscf/__config__.py
 pyscf/__init__.py
 pyscf/post_scf.py
 pyscf.egg-info/PKG-INFO
 pyscf.egg-info/SOURCES.txt
@@ -124,15 +124,17 @@
 pyscf/df/grad/uhf.py
 pyscf/df/grad/uks.py
 pyscf/df/hessian/__init__.py
 pyscf/df/hessian/rhf.py
 pyscf/df/hessian/rks.py
 pyscf/df/hessian/uhf.py
 pyscf/df/hessian/uks.py
+pyscf/dft/LebedevGrid.py
 pyscf/dft/__init__.py
+pyscf/dft/dft_parser.py
 pyscf/dft/dks.py
 pyscf/dft/gen_grid.py
 pyscf/dft/gen_libxc_param.py
 pyscf/dft/gen_xcfun_param.py
 pyscf/dft/gks.py
 pyscf/dft/gks_symm.py
 pyscf/dft/libxc.py
@@ -550,19 +552,27 @@
 pyscf/lib/cc/ccsd_pack.c
 pyscf/lib/cc/ccsd_t.c
 pyscf/lib/cc/uccsd_t.c
 pyscf/lib/dft/CMakeLists.txt
 pyscf/lib/dft/CxLebedevGrid.c
 pyscf/lib/dft/grid_basis.c
 pyscf/lib/dft/grid_basis.h
+pyscf/lib/dft/grid_collocate.c
+pyscf/lib/dft/grid_common.c
+pyscf/lib/dft/grid_common.h
+pyscf/lib/dft/grid_integrate.c
 pyscf/lib/dft/libxc_itrf.c
+pyscf/lib/dft/multigrid.c
+pyscf/lib/dft/multigrid.h
 pyscf/lib/dft/nr_numint.c
 pyscf/lib/dft/nr_numint_sparse.c
 pyscf/lib/dft/numint_uniform_grid.c
 pyscf/lib/dft/r_numint.c
+pyscf/lib/dft/utils.c
+pyscf/lib/dft/utils.h
 pyscf/lib/dft/xc_deriv.c
 pyscf/lib/dft/xcfun_itrf.c
 pyscf/lib/gto/CMakeLists.txt
 pyscf/lib/gto/deriv1.c
 pyscf/lib/gto/deriv2.c
 pyscf/lib/gto/fastexp.c
 pyscf/lib/gto/fill_grids_int2c.c
@@ -595,30 +605,41 @@
 pyscf/lib/np_helper/np_helper.c
 pyscf/lib/np_helper/np_helper.h
 pyscf/lib/np_helper/npdot.c
 pyscf/lib/np_helper/omp_reduce.c
 pyscf/lib/np_helper/pack_tril.c
 pyscf/lib/np_helper/transpose.c
 pyscf/lib/pbc/CMakeLists.txt
+pyscf/lib/pbc/cell.c
+pyscf/lib/pbc/cell.h
 pyscf/lib/pbc/cint2e.c
 pyscf/lib/pbc/cint3c2e.c
+pyscf/lib/pbc/fft.c
+pyscf/lib/pbc/fft.h
 pyscf/lib/pbc/fill_ints.c
+pyscf/lib/pbc/fill_ints.h
+pyscf/lib/pbc/fill_ints_screened.c
 pyscf/lib/pbc/fill_ints_sr.c
 pyscf/lib/pbc/ft_ao.c
 pyscf/lib/pbc/grid_ao.c
+pyscf/lib/pbc/hf_grad.c
 pyscf/lib/pbc/inner_dot.c
+pyscf/lib/pbc/neighbor_list.c
+pyscf/lib/pbc/neighbor_list.h
 pyscf/lib/pbc/nr_direct.c
 pyscf/lib/pbc/nr_ecp.c
 pyscf/lib/pbc/optimizer.c
 pyscf/lib/pbc/optimizer.h
 pyscf/lib/pbc/pbc.h
+pyscf/lib/pbc/pp.c
 pyscf/lib/pbc/symmetry.c
 pyscf/lib/pbc/transform_mo.c
 pyscf/lib/ri/CMakeLists.txt
 pyscf/lib/ri/r_df_incore.c
+pyscf/lib/solvent/CMakeLists.txt
 pyscf/lib/vhf/CMakeLists.txt
 pyscf/lib/vhf/cvhf.h
 pyscf/lib/vhf/fblas.h
 pyscf/lib/vhf/fill_nr_s8.c
 pyscf/lib/vhf/hessian_screen.c
 pyscf/lib/vhf/nr_direct.c
 pyscf/lib/vhf/nr_direct.h
@@ -747,34 +768,44 @@
 pyscf/pbc/dft/krkspu.py
 pyscf/pbc/dft/krkspu_ksymm.py
 pyscf/pbc/dft/kroks.py
 pyscf/pbc/dft/kuks.py
 pyscf/pbc/dft/kuks_ksymm.py
 pyscf/pbc/dft/kukspu.py
 pyscf/pbc/dft/kukspu_ksymm.py
-pyscf/pbc/dft/multigrid.py
 pyscf/pbc/dft/numint.py
 pyscf/pbc/dft/numint2c.py
 pyscf/pbc/dft/rks.py
 pyscf/pbc/dft/roks.py
 pyscf/pbc/dft/uks.py
+pyscf/pbc/dft/multigrid/__init__.py
+pyscf/pbc/dft/multigrid/multigrid.py
+pyscf/pbc/dft/multigrid/multigrid_pair.py
+pyscf/pbc/dft/multigrid/pp.py
+pyscf/pbc/dft/multigrid/utils.py
 pyscf/pbc/eph/__init__.py
 pyscf/pbc/eph/eph_fd.py
 pyscf/pbc/geomopt/__init__.py
 pyscf/pbc/geomopt/geometric_solver.py
 pyscf/pbc/grad/__init__.py
 pyscf/pbc/grad/krhf.py
 pyscf/pbc/grad/krks.py
 pyscf/pbc/grad/kuhf.py
 pyscf/pbc/grad/kuks.py
+pyscf/pbc/grad/rhf.py
+pyscf/pbc/grad/rks.py
+pyscf/pbc/grad/uhf.py
+pyscf/pbc/grad/uks.py
 pyscf/pbc/gto/__init__.py
 pyscf/pbc/gto/_pbcintor.py
 pyscf/pbc/gto/cell.py
 pyscf/pbc/gto/ecp.py
 pyscf/pbc/gto/eval_gto.py
+pyscf/pbc/gto/ewald_methods.py
+pyscf/pbc/gto/neighborlist.py
 pyscf/pbc/gto/basis/__init__.py
 pyscf/pbc/gto/basis/gth-aug-dzvp.dat
 pyscf/pbc/gto/basis/gth-aug-qzv2p.dat
 pyscf/pbc/gto/basis/gth-aug-qzv3p.dat
 pyscf/pbc/gto/basis/gth-aug-tzv2p.dat
 pyscf/pbc/gto/basis/gth-aug-tzvp.dat
 pyscf/pbc/gto/basis/gth-cc-dzvp.dat
@@ -905,14 +936,15 @@
 pyscf/qmmm/itrf.py
 pyscf/qmmm/mm_mole.py
 pyscf/scf/__init__.py
 pyscf/scf/_response_functions.py
 pyscf/scf/_vhf.py
 pyscf/scf/addons.py
 pyscf/scf/atom_hf.py
+pyscf/scf/atom_hf_pp.py
 pyscf/scf/atom_ks.py
 pyscf/scf/chkfile.py
 pyscf/scf/cphf.py
 pyscf/scf/dhf.py
 pyscf/scf/diis.py
 pyscf/scf/dispersion.py
 pyscf/scf/ghf.py
@@ -929,18 +961,28 @@
 pyscf/sgx/__init__.py
 pyscf/sgx/sgx.py
 pyscf/sgx/sgx_jk.py
 pyscf/solvent/__init__.py
 pyscf/solvent/_attach_solvent.py
 pyscf/solvent/_ddcosmo_tdscf_grad.py
 pyscf/solvent/ddcosmo.py
-pyscf/solvent/ddcosmo_grad.py
 pyscf/solvent/ddpcm.py
 pyscf/solvent/pcm.py
 pyscf/solvent/pol_embed.py
+pyscf/solvent/smd.py
+pyscf/solvent/smd_experiment.py
+pyscf/solvent/grad/__init__.py
+pyscf/solvent/grad/ddcosmo_grad.py
+pyscf/solvent/grad/pcm.py
+pyscf/solvent/grad/smd.py
+pyscf/solvent/grad/smd_experiment.py
+pyscf/solvent/hessian/__init__.py
+pyscf/solvent/hessian/pcm.py
+pyscf/solvent/hessian/smd.py
+pyscf/solvent/hessian/smd_experiment.py
 pyscf/soscf/__init__.py
 pyscf/soscf/ciah.py
 pyscf/soscf/newton_ah.py
 pyscf/symm/Dmatrix.py
 pyscf/symm/__init__.py
 pyscf/symm/addons.py
 pyscf/symm/basis.py
```

