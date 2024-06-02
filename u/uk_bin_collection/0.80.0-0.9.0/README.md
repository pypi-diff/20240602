# Comparing `tmp/uk_bin_collection-0.80.0.tar.gz` & `tmp/uk_bin_collection-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uk_bin_collection-0.80.0.tar", max compression
+gzip compressed data, was "uk_bin_collection-0.9.0.tar", max compression
```

## Comparing `uk_bin_collection-0.80.0.tar` & `uk_bin_collection-0.9.0.tar`

### file list

```diff
@@ -1,186 +1,256 @@
--rw-r--r--   0        0        0     1071 2024-06-02 12:37:08.503945 uk_bin_collection-0.80.0/LICENSE
--rw-r--r--   0        0        0    11861 2024-06-02 12:37:08.503945 uk_bin_collection-0.80.0/README.md
--rw-r--r--   0        0        0     1644 2024-06-02 12:37:08.503945 uk_bin_collection-0.80.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-06-02 12:37:08.503945 uk_bin_collection-0.80.0/uk_bin_collection/README.rst
--rw-r--r--   0        0        0     3843 2024-06-02 12:37:08.503945 uk_bin_collection-0.80.0/uk_bin_collection/tests/council_feature_input_parity.py
--rw-r--r--   0        0        0      127 2024-06-02 12:37:08.503945 uk_bin_collection-0.80.0/uk_bin_collection/tests/features/environment.py
--rw-r--r--   0        0        0      251 2024-06-02 12:37:08.503945 uk_bin_collection-0.80.0/uk_bin_collection/tests/features/validate_council_outputs.feature
--rw-r--r--   0        0        0    58920 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/tests/input.json
--rw-r--r--   0        0        0     1086 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/tests/output.schema
--rw-r--r--   0        0        0     1474 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/tests/step_defs/step_helpers/file_handler.py
--rw-r--r--   0        0        0     3424 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/tests/step_defs/test_validate_council.py
--rw-r--r--   0        0        0     3316 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/tests/test_collect_data.py
--rw-r--r--   0        0        0    11190 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/tests/test_common_functions.py
--rwxr-xr-x   0        0        0     4383 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/collect_data.py
--rw-r--r--   0        0        0     9837 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/common.py
--rw-r--r--   0        0        0     1511 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/AdurAndWorthingCouncils.py
--rw-r--r--   0        0        0     4012 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ArunCouncil.py
--rw-r--r--   0        0        0     2401 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/AylesburyValeCouncil.py
--rw-r--r--   0        0        0     1707 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BCPCouncil.py
--rw-r--r--   0        0        0     8174 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BarnetCouncil.py
--rw-r--r--   0        0        0     4244 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BarnsleyMBCouncil.py
--rw-r--r--   0        0        0     2632 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BasingstokeCouncil.py
--rw-r--r--   0        0        0     3709 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BathAndNorthEastSomersetCouncil.py
--rw-r--r--   0        0        0     1669 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BedfordBoroughCouncil.py
--rw-r--r--   0        0        0     2549 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BedfordshireCouncil.py
--rw-r--r--   0        0        0     5399 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BexleyCouncil.py
--rw-r--r--   0        0        0     4131 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BirminghamCityCouncil.py
--rw-r--r--   0        0        0     4090 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BlackburnCouncil.py
--rw-r--r--   0        0        0     4023 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BoltonCouncil.py
--rw-r--r--   0        0        0     9015 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BracknellForestCouncil.py
--rw-r--r--   0        0        0     4308 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BradfordMDC.py
--rw-r--r--   0        0        0     5823 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BrightonandHoveCityCouncil.py
--rw-r--r--   0        0        0     5576 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BristolCityCouncil.py
--rw-r--r--   0        0        0     4758 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BromleyBoroughCouncil.py
--rw-r--r--   0        0        0     4473 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BroxtoweBoroughCouncil.py
--rw-r--r--   0        0        0     3184 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BuckinghamshireCouncil.py
--rw-r--r--   0        0        0     2632 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BuryCouncil.py
--rw-r--r--   0        0        0     4971 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/CalderdaleCouncil.py
--rw-r--r--   0        0        0     2276 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/CannockChaseDistrictCouncil.py
--rw-r--r--   0        0        0     7208 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/CardiffCouncil.py
--rw-r--r--   0        0        0     3858 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/CastlepointDistrictCouncil.py
--rw-r--r--   0        0        0     2172 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/CharnwoodBoroughCouncil.py
--rw-r--r--   0        0        0     5090 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ChelmsfordCityCouncil.py
--rw-r--r--   0        0        0     1132 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/CheshireEastCouncil.py
--rw-r--r--   0        0        0     4780 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/CheshireWestAndChesterCouncil.py
--rw-r--r--   0        0        0     4118 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ChichesterDistrictCouncil.py
--rw-r--r--   0        0        0     5194 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ChorleyCouncil.py
--rw-r--r--   0        0        0     1034 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ConwyCountyBorough.py
--rw-r--r--   0        0        0     2367 2024-06-02 12:37:08.507945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/CrawleyBoroughCouncil.py
--rw-r--r--   0        0        0    11594 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/CroydonCouncil.py
--rw-r--r--   0        0        0     1550 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/DartfordBoroughCouncil.py
--rw-r--r--   0        0        0     4007 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/DerbyshireDalesDistrictCouncil.py
--rw-r--r--   0        0        0     3118 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/DoncasterCouncil.py
--rw-r--r--   0        0        0     2304 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/DorsetCouncil.py
--rw-r--r--   0        0        0     1891 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/DoverDistrictCouncil.py
--rw-r--r--   0        0        0     1695 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/DurhamCouncil.py
--rw-r--r--   0        0        0     1501 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/EastCambridgeshireCouncil.py
--rw-r--r--   0        0        0     3261 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/EastDevonDC.py
--rw-r--r--   0        0        0     4356 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/EastLindseyDistrictCouncil.py
--rw-r--r--   0        0        0     5218 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/EastRidingCouncil.py
--rw-r--r--   0        0        0     4353 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/EastSuffolkCouncil.py
--rw-r--r--   0        0        0     2310 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/EastleighBoroughCouncil.py
--rw-r--r--   0        0        0     1695 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/EnvironmentFirst.py
--rw-r--r--   0        0        0     2085 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/EppingForestDistrictCouncil.py
--rw-r--r--   0        0        0     2501 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ErewashBoroughCouncil.py
--rw-r--r--   0        0        0     2352 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/FarehamBoroughCouncil.py
--rw-r--r--   0        0        0     2513 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/FenlandDistrictCouncil.py
--rw-r--r--   0        0        0     4504 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ForestOfDeanDistrictCouncil.py
--rw-r--r--   0        0        0     4601 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/GatesheadCouncil.py
--rw-r--r--   0        0        0    58880 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/GedlingBoroughCouncil.py
--rw-r--r--   0        0        0     2528 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/GlasgowCityCouncil.py
--rw-r--r--   0        0        0     5695 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/GuildfordCouncil.py
--rw-r--r--   0        0        0     5837 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/HaltonBoroughCouncil.py
--rw-r--r--   0        0        0     2362 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/HaringeyCouncil.py
--rw-r--r--   0        0        0     2050 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/HarrogateBoroughCouncil.py
--rw-r--r--   0        0        0     4815 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/HighPeakCouncil.py
--rw-r--r--   0        0        0     4564 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/HounslowCouncil.py
--rw-r--r--   0        0        0     1851 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/HullCityCouncil.py
--rw-r--r--   0        0        0     1587 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/HuntingdonDistrictCouncil.py
--rw-r--r--   0        0        0     3543 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/KingstonUponThamesCouncil.py
--rw-r--r--   0        0        0     4499 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/KirkleesCouncil.py
--rw-r--r--   0        0        0     5605 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/KnowsleyMBCouncil.py
--rw-r--r--   0        0        0     2537 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/LancasterCityCouncil.py
--rw-r--r--   0        0        0     5144 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/LeedsCityCouncil.py
--rw-r--r--   0        0        0     3309 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/LisburnCastlereaghCityCouncil.py
--rw-r--r--   0        0        0     2587 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/LiverpoolCityCouncil.py
--rw-r--r--   0        0        0     3021 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/LondonBoroughHounslow.py
--rw-r--r--   0        0        0     6604 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/LondonBoroughRedbridge.py
--rw-r--r--   0        0        0     1997 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/MaldonDistrictCouncil.py
--rw-r--r--   0        0        0     2100 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/MalvernHillsDC.py
--rw-r--r--   0        0        0     4920 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ManchesterCityCouncil.py
--rw-r--r--   0        0        0     1386 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/MansfieldDistrictCouncil.py
--rw-r--r--   0        0        0     1997 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/MertonCouncil.py
--rw-r--r--   0        0        0     5238 2024-06-02 12:37:08.511945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/MidAndEastAntrimBoroughCouncil.py
--rw-r--r--   0        0        0     2705 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/MidSussexDistrictCouncil.py
--rw-r--r--   0        0        0     2005 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/MiltonKeynesCityCouncil.py
--rw-r--r--   0        0        0     3994 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/MoleValleyDistrictCouncil.py
--rw-r--r--   0        0        0     5506 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NeathPortTalbotCouncil.py
--rw-r--r--   0        0        0     5391 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NewForestCouncil.py
--rw-r--r--   0        0        0     2140 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NewarkAndSherwoodDC.py
--rw-r--r--   0        0        0     2085 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NewcastleCityCouncil.py
--rw-r--r--   0        0        0     2086 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NewhamCouncil.py
--rw-r--r--   0        0        0     8480 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NewportCityCouncil.py
--rw-r--r--   0        0        0     4651 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NorthEastDerbyshireDistrictCouncil.py
--rw-r--r--   0        0        0     1817 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NorthEastLincs.py
--rw-r--r--   0        0        0     1681 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NorthKestevenDistrictCouncil.py
--rw-r--r--   0        0        0     1763 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NorthLanarkshireCouncil.py
--rw-r--r--   0        0        0     2467 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NorthLincolnshireCouncil.py
--rw-r--r--   0        0        0     4315 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NorthNorfolkDistrictCouncil.py
--rw-r--r--   0        0        0     2337 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NorthNorthamptonshireCouncil.py
--rw-r--r--   0        0        0     2754 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NorthSomersetCouncil.py
--rw-r--r--   0        0        0    11353 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NorthTynesideCouncil.py
--rw-r--r--   0        0        0     4584 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NorthWestLeicestershire.py
--rw-r--r--   0        0        0     1933 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NorthYorkshire.py
--rw-r--r--   0        0        0     4990 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NorthumberlandCouncil.py
--rw-r--r--   0        0        0     1323 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NottinghamCityCouncil.py
--rw-r--r--   0        0        0     1771 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/OldhamCouncil.py
--rw-r--r--   0        0        0     5588 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/PortsmouthCityCouncil.py
--rw-r--r--   0        0        0     3838 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/PrestonCityCouncil.py
--rw-r--r--   0        0        0     1009 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ReadingBoroughCouncil.py
--rw-r--r--   0        0        0     3251 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ReigateAndBansteadBoroughCouncil.py
--rw-r--r--   0        0        0     5109 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/RenfrewshireCouncil.py
--rw-r--r--   0        0        0     3233 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/RhonddaCynonTaffCouncil.py
--rw-r--r--   0        0        0     2379 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/RochdaleCouncil.py
--rw-r--r--   0        0        0     2613 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/RochfordCouncil.py
--rw-r--r--   0        0        0     4306 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/RugbyBoroughCouncil.py
--rw-r--r--   0        0        0     4005 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/RushcliffeBoroughCouncil.py
--rw-r--r--   0        0        0     3375 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/RushmoorCouncil.py
--rw-r--r--   0        0        0     2506 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SalfordCityCouncil.py
--rw-r--r--   0        0        0     4260 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SevenoaksDistrictCouncil.py
--rw-r--r--   0        0        0     2016 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SheffieldCityCouncil.py
--rw-r--r--   0        0        0     1477 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ShropshireCouncil.py
--rw-r--r--   0        0        0     1609 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SolihullCouncil.py
--rw-r--r--   0        0        0     8480 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SomersetCouncil.py
--rw-r--r--   0        0        0     2722 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SouthAyrshireCouncil.py
--rw-r--r--   0        0        0     2308 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SouthCambridgeshireCouncil.py
--rw-r--r--   0        0        0     2412 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SouthGloucestershireCouncil.py
--rw-r--r--   0        0        0     5587 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SouthKestevenDistrictCouncil.py
--rw-r--r--   0        0        0     3126 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SouthLanarkshireCouncil.py
--rw-r--r--   0        0        0     3971 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SouthNorfolkCouncil.py
--rw-r--r--   0        0        0     3879 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SouthOxfordshireCouncil.py
--rw-r--r--   0        0        0     3426 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SouthTynesideCouncil.py
--rw-r--r--   0        0        0     1451 2024-06-02 12:37:08.515945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/StAlbansCityAndDistrictCouncil.py
--rw-r--r--   0        0        0     2069 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/StHelensBC.py
--rw-r--r--   0        0        0     2292 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/StaffordBoroughCouncil.py
--rw-r--r--   0        0        0     4361 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/StaffordshireMoorlandsDistrictCouncil.py
--rw-r--r--   0        0        0     1429 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/StockportBoroughCouncil.py
--rw-r--r--   0        0        0     2884 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/StokeOnTrentCityCouncil.py
--rw-r--r--   0        0        0     3936 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/StratfordUponAvonCouncil.py
--rw-r--r--   0        0        0     3561 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/StroudDistrictCouncil.py
--rw-r--r--   0        0        0     3825 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SunderlandCityCouncil.py
--rw-r--r--   0        0        0     2048 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SwaleBoroughCouncil.py
--rw-r--r--   0        0        0     2303 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SwanseaCouncil.py
--rw-r--r--   0        0        0     1995 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/TamesideMBCouncil.py
--rw-r--r--   0        0        0     2324 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/TandridgeDistrictCouncil.py
--rw-r--r--   0        0        0     1844 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/TelfordAndWrekinCouncil.py
--rw-r--r--   0        0        0     4274 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/TendringDistrictCouncil.py
--rw-r--r--   0        0        0     8480 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/TestValleyBoroughCouncil.py
--rw-r--r--   0        0        0     5527 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ThreeRiversDistrictCouncil.py
--rw-r--r--   0        0        0     4859 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/TonbridgeAndMallingBC.py
--rw-r--r--   0        0        0     2029 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/TorbayCouncil.py
--rw-r--r--   0        0        0     6386 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/TorridgeDistrictCouncil.py
--rw-r--r--   0        0        0     4129 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/UttlesfordDistrictCouncil.py
--rw-r--r--   0        0        0     5044 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ValeofGlamorganCouncil.py
--rw-r--r--   0        0        0     4292 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ValeofWhiteHorseCouncil.py
--rw-r--r--   0        0        0     4466 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/WakefieldCityCouncil.py
--rw-r--r--   0        0        0     4997 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/WalthamForest.py
--rw-r--r--   0        0        0     1146 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/WarwickDistrictCouncil.py
--rw-r--r--   0        0        0     4662 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/WaverleyBoroughCouncil.py
--rw-r--r--   0        0        0     3368 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/WealdenDistrictCouncil.py
--rw-r--r--   0        0        0     2316 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/WelhatCouncil.py
--rw-r--r--   0        0        0     5110 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/WestBerkshireCouncil.py
--rw-r--r--   0        0        0     4606 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/WestLindseyDistrictCouncil.py
--rw-r--r--   0        0        0     4114 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/WestLothianCouncil.py
--rw-r--r--   0        0        0     1079 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/WestNorthamptonshireCouncil.py
--rw-r--r--   0        0        0     2633 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/WestSuffolkCouncil.py
--rw-r--r--   0        0        0     3746 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/WiganBoroughCouncil.py
--rw-r--r--   0        0        0     5653 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/WiltshireCouncil.py
--rw-r--r--   0        0        0     5554 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/WindsorAndMaidenheadCouncil.py
--rw-r--r--   0        0        0     5204 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/WokingBoroughCouncil.py
--rw-r--r--   0        0        0     3511 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/WyreCouncil.py
--rw-r--r--   0        0        0     1490 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/YorkCouncil.py
--rw-r--r--   0        0        0     1162 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/council_class_template/councilclasstemplate.py
--rw-r--r--   0        0        0     1536 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/create_new_council.py
--rw-r--r--   0        0        0     5414 2024-06-02 12:37:08.519945 uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/get_bin_data.py
--rw-r--r--   0        0        0    12594 1970-01-01 00:00:00.000000 uk_bin_collection-0.80.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-28 16:58:25.674787 uk_bin_collection-0.9.0/LICENSE
+-rw-r--r--   0        0        0     7296 2023-07-28 16:58:25.674787 uk_bin_collection-0.9.0/README.md
+-rw-r--r--   0        0        0     1189 2023-07-28 16:59:00.294518 uk_bin_collection-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/README.rst
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/BCPCouncil.schema
+-rw-r--r--   0        0        0     1291 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/BasingstokeCouncil.schema
+-rw-r--r--   0        0        0     1357 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/BexleyCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/BlackburnCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/BoltonCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/BristolCityCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/BromleyBoroughCouncil.schema
+-rw-r--r--   0        0        0     1002 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/BroxtoweBoroughCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/CardiffCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/CastlepointDistrictCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/CharnwoodBoroughCouncil.schema
+-rw-r--r--   0        0        0     1275 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/ChelmsfordCityCouncil.schema
+-rw-r--r--   0        0        0     1279 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/CheshireEastCouncil.schema
+-rw-r--r--   0        0        0      998 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/Chilterns.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/CrawleyBoroughCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/CroydonCouncil.schema
+-rw-r--r--   0        0        0     1002 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/DerbyshireDalesDistrictCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/DoncasterCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/DurhamCouncil.schema
+-rw-r--r--   0        0        0     1229 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/EastCambridgeshireCouncil.schema
+-rw-r--r--   0        0        0     1276 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/EastDevonDC.schema
+-rw-r--r--   0        0        0     1190 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/EastNorthamptonshireCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/EastRidingCouncil.schema
+-rw-r--r--   0        0        0     1306 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/EastleighBoroughCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/ErewashBoroughCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/FenlandDistrictCouncil.schema
+-rw-r--r--   0        0        0     1317 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/GlasgowCityCouncil.schema
+-rw-r--r--   0        0        0     1211 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/HighPeakCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/HuntingdonDistrictCouncil.schema
+-rw-r--r--   0        0        0      998 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/KingstonUponThamesCouncil.schema
+-rw-r--r--   0        0        0     1209 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/LeedsCityCouncil.schema
+-rw-r--r--   0        0        0     1223 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/LisburnCastlereaghCityCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/LondonBoroughHounslow.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/MaldonDistrictCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/MalvernHillsDC.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/ManchesterCityCouncil.schema
+-rw-r--r--   0        0        0     1007 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/MertonCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/MidSussexDistrictCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/MiltonKeynesCityCouncil.schema
+-rw-r--r--   0        0        0     1244 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/NewarkAndSherwoodDC.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/NewcastleCityCouncil.schema
+-rw-r--r--   0        0        0     1319 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/NorthEastLincs.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/NorthKestevenDistrictCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/NorthLanarkshireCouncil.schema
+-rw-r--r--   0        0        0     1398 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/NorthLincolnshireCouncil.schema
+-rw-r--r--   0        0        0     1002 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/NorthNorfolkDistrictCouncil.schema
+-rw-r--r--   0        0        0     1002 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/NorthSomersetCouncil.schema
+-rw-r--r--   0        0        0     1262 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/NorthTynesideCouncil.schema
+-rw-r--r--   0        0        0     1310 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/NorthumberlandCouncil.schema
+-rw-r--r--   0        0        0     1337 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/PrestonCityCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/RochdaleCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/RushcliffeBoroughCouncil.schema
+-rw-r--r--   0        0        0     1209 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/RushmoorCouncil.schema
+-rw-r--r--   0        0        0     1313 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/SalfordCityCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/SheffieldCityCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/SomersetCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/SouthAyrshireCouncil.schema
+-rw-r--r--   0        0        0     1219 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/SouthCambridgeshireCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/SouthLanarkshireCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/SouthNorfolkCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/SouthOxfordshireCouncil.schema
+-rw-r--r--   0        0        0     1236 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/SouthTynesideCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/StHelensBC.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/StockportBoroughCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/SwaleBoroughCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/TamesideMBCouncil.schema
+-rw-r--r--   0        0        0     1002 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/TonbridgeAndMallingBC.schema
+-rw-r--r--   0        0        0     1002 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/TorbayCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/TorridgeDistrictCouncil.schema
+-rw-r--r--   0        0        0     1202 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/ValeofGlamorganCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/WakefieldCityCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/WarwickDistrictCouncil.schema
+-rw-r--r--   0        0        0     1283 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/WaverleyBoroughCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/WealdenDistrictCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/WelhatCouncil.schema
+-rw-r--r--   0        0        0      382 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/WiganBoroughCouncil.schema
+-rw-r--r--   0        0        0     1273 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/WiltshireCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/WindsorAndMaidenheadCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/WokingBoroughCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/YorkCouncil.schema
+-rw-r--r--   0        0        0      127 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/features/environment.py
+-rw-r--r--   0        0        0     3281 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/features/validate_council_outputs.feature
+-rw-r--r--   0        0        0    24132 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/input.json
+-rw-r--r--   0        0        0      606 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/BCPCouncil.json
+-rw-r--r--   0        0        0     2284 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/BasingstokeCouncil.json
+-rw-r--r--   0        0        0     3473 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/BexleyCouncil.json
+-rw-r--r--   0        0        0      501 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/BlackburnCouncil.json
+-rw-r--r--   0        0        0     1192 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/BoltonCouncil.json
+-rw-r--r--   0        0        0      557 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/BristolCityCouncil.json
+-rw-r--r--   0        0        0      462 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/BromleyBoroughCouncil.json
+-rw-r--r--   0        0        0      315 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/BroxtoweBoroughCouncil.json
+-rw-r--r--   0        0        0     1156 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/CardiffCouncil.json
+-rw-r--r--   0        0        0      958 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/CastlepointDistrictCouncil.json
+-rw-r--r--   0        0        0      213 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/CharnwoodBoroughCouncil.json
+-rw-r--r--   0        0        0     1830 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/ChelmsfordCityCouncil.json
+-rw-r--r--   0        0        0     1187 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/CheshireEastCouncil.json
+-rw-r--r--   0        0        0      493 2023-07-28 16:58:25.678787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/Chilterns.json
+-rw-r--r--   0        0        0      271 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/CrawleyBoroughCouncil.json
+-rw-r--r--   0        0        0      466 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/CroydonCouncil.json
+-rw-r--r--   0        0        0      562 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/DerbyshireDalesDistrictCouncil.json
+-rw-r--r--   0        0        0      775 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/DoncasterCouncil.json
+-rw-r--r--   0        0        0      214 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/DurhamCouncil.json
+-rw-r--r--   0        0        0     1606 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/EastCambridgeshireCouncil.json
+-rw-r--r--   0        0        0     2635 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/EastDevonDC.json
+-rw-r--r--   0        0        0      982 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/EastNorthamptonshireCouncil.json
+-rw-r--r--   0        0        0      312 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/EastRidingCouncil.json
+-rw-r--r--   0        0        0      547 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/EastleighBoroughCouncil.json
+-rw-r--r--   0        0        0      325 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/ErewashBoroughCouncil.json
+-rw-r--r--   0        0        0     1362 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/FenlandDistrictCouncil.json
+-rw-r--r--   0        0        0     4251 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/GlasgowCityCouncil.json
+-rw-r--r--   0        0        0     1726 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/HighPeakCouncil.json
+-rw-r--r--   0        0        0      335 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/HuntingdonDistrictCouncil.json
+-rw-r--r--   0        0        0      534 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/KingstonUponThamesCouncil.json
+-rw-r--r--   0        0        0     1789 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/LeedsCityCouncil.json
+-rw-r--r--   0        0        0      608 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/LisburnCastlereaghCityCouncil.json
+-rw-r--r--   0        0        0     1445 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/LondonBoroughHounslow.json
+-rw-r--r--   0        0        0      409 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/MaldonDistrictCouncil.json
+-rw-r--r--   0        0        0      227 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/MalvernHillsDC.json
+-rw-r--r--   0        0        0      416 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/ManchesterCityCouncil.json
+-rw-r--r--   0        0        0      665 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/MertonCouncil.json
+-rw-r--r--   0        0        0      148 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/MidSussexDistrictCouncil.json
+-rw-r--r--   0        0        0      862 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/MiltonKeynesCityCouncil.json
+-rw-r--r--   0        0        0     1278 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/NewarkAndSherwoodDC.json
+-rw-r--r--   0        0        0      221 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/NewcastleCityCouncil.json
+-rw-r--r--   0        0        0     4096 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/NorthEastLincs.json
+-rw-r--r--   0        0        0      446 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/NorthKestevenDistrictCouncil.json
+-rw-r--r--   0        0        0      902 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/NorthLanarkshireCouncil.json
+-rw-r--r--   0        0        0     3042 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/NorthLincolnshireCouncil.json
+-rw-r--r--   0        0        0      300 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/NorthNorfolkDistrictCouncil.json
+-rw-r--r--   0        0        0      590 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/NorthSomersetCouncil.json
+-rw-r--r--   0        0        0     4935 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/NorthTynesideCouncil.json
+-rw-r--r--   0        0        0     3956 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/NorthumberlandCouncil.json
+-rw-r--r--   0        0        0    15934 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/PrestonCityCouncil.json
+-rw-r--r--   0        0        0      903 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/RochdaleCouncil.json
+-rw-r--r--   0        0        0      306 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/RushcliffeBoroughCouncil.json
+-rw-r--r--   0        0        0     1602 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/RushmoorCouncil.json
+-rw-r--r--   0        0        0     2734 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/SalfordCityCouncil.json
+-rw-r--r--   0        0        0      892 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/SheffieldCityCouncil.json
+-rw-r--r--   0        0        0      307 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/SomersetCouncil.json
+-rw-r--r--   0        0        0     1871 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/SouthAyrshireCouncil.json
+-rw-r--r--   0        0        0     2214 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/SouthCambridgeshireCouncil.json
+-rw-r--r--   0        0        0      258 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/SouthLanarkshireCouncil.json
+-rw-r--r--   0        0        0      217 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/SouthNorfolkCouncil.json
+-rw-r--r--   0        0        0      293 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/SouthOxfordshireCouncil.json
+-rw-r--r--   0        0        0     3283 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/SouthTynesideCouncil.json
+-rw-r--r--   0        0        0      358 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/StHelensBC.json
+-rw-r--r--   0        0        0      409 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/StockportBoroughCouncil.json
+-rw-r--r--   0        0        0      922 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/SwaleBoroughCouncil.json
+-rw-r--r--   0        0        0     1765 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/TamesideMBCouncil.json
+-rw-r--r--   0        0        0     1037 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/TonbridgeAndMallingBC.json
+-rw-r--r--   0        0        0     1406 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/TorbayCouncil.json
+-rw-r--r--   0        0        0      116 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/TorridgeDistrictCouncil.json
+-rw-r--r--   0        0        0     5934 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/ValeofGlamorganCouncil.json
+-rw-r--r--   0        0        0      225 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/WakefieldCityCouncil.json
+-rw-r--r--   0        0        0      318 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/WarwickDistrictCouncil.json
+-rw-r--r--   0        0        0      964 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/WaverleyBoroughCouncil.json
+-rw-r--r--   0        0        0      222 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/WealdenDistrictCouncil.json
+-rw-r--r--   0        0        0      495 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/WelhatCouncil.json
+-rw-r--r--   0        0        0      161 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/WiganBoroughCouncil.json
+-rw-r--r--   0        0        0     1737 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/WiltshireCouncil.json
+-rw-r--r--   0        0        0      367 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/WindsorAndMaidenheadCouncil.json
+-rw-r--r--   0        0        0     1482 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/WokingBoroughCouncil.json
+-rw-r--r--   0        0        0      307 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/outputs/YorkCouncil.json
+-rw-r--r--   0        0        0     1147 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/step_defs/step_helpers/file_handler.py
+-rw-r--r--   0        0        0     2631 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/step_defs/test_validate_council.py
+-rw-r--r--   0        0        0     2576 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/test_collect_data.py
+-rw-r--r--   0        0        0     3977 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/tests/test_common_functions.py
+-rw-r--r--   0        0        0     3083 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/collect_data.py
+-rw-r--r--   0        0        0     6643 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/common.py
+-rw-r--r--   0        0        0     1579 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/BCPCouncil.py
+-rw-r--r--   0        0        0     1936 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/BasingstokeCouncil.py
+-rw-r--r--   0        0        0     2237 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/BexleyCouncil.py
+-rw-r--r--   0        0        0     3156 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/BlackburnCouncil.py
+-rw-r--r--   0        0        0     3028 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/BoltonCouncil.py
+-rw-r--r--   0        0        0     5581 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/BristolCityCouncil.py
+-rw-r--r--   0        0        0     1676 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/BromleyBoroughCouncil.py
+-rw-r--r--   0        0        0     3733 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/BroxtoweBoroughCouncil.py
+-rw-r--r--   0        0        0     7214 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/CardiffCouncil.py
+-rw-r--r--   0        0        0     3946 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/CastlepointDistrictCouncil.py
+-rw-r--r--   0        0        0     1572 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/CharnwoodBoroughCouncil.py
+-rw-r--r--   0        0        0     2170 2023-07-28 16:58:25.682787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/ChelmsfordCityCouncil.py
+-rw-r--r--   0        0        0     1541 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/CheshireEastCouncil.py
+-rw-r--r--   0        0        0     2938 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/Chilterns.py
+-rw-r--r--   0        0        0     1983 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/CrawleyBoroughCouncil.py
+-rw-r--r--   0        0        0    11599 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/CroydonCouncil.py
+-rw-r--r--   0        0        0     3499 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/DerbyshireDalesDistrictCouncil.py
+-rw-r--r--   0        0        0     3124 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/DoncasterCouncil.py
+-rw-r--r--   0        0        0     1626 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/DurhamCouncil.py
+-rw-r--r--   0        0        0     1506 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/EastCambridgeshireCouncil.py
+-rw-r--r--   0        0        0     3267 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/EastDevonDC.py
+-rw-r--r--   0        0        0     3756 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/EastNorthamptonshireCouncil.py
+-rw-r--r--   0        0        0     2170 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/EastRidingCouncil.py
+-rw-r--r--   0        0        0     2203 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/EastleighBoroughCouncil.py
+-rw-r--r--   0        0        0     2507 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/ErewashBoroughCouncil.py
+-rw-r--r--   0        0        0     2519 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/FenlandDistrictCouncil.py
+-rw-r--r--   0        0        0     2534 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/GlasgowCityCouncil.py
+-rw-r--r--   0        0        0     4416 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/HighPeakCouncil.py
+-rw-r--r--   0        0        0     1114 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/HuntingdonDistrictCouncil.py
+-rw-r--r--   0        0        0     1735 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/KingstonUponThamesCouncil.py
+-rw-r--r--   0        0        0     3712 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/LeedsCityCouncil.py
+-rw-r--r--   0        0        0     3313 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/LisburnCastlereaghCityCouncil.py
+-rw-r--r--   0        0        0     2081 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/LondonBoroughHounslow.py
+-rw-r--r--   0        0        0     2003 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/MaldonDistrictCouncil.py
+-rw-r--r--   0        0        0     2092 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/MalvernHillsDC.py
+-rw-r--r--   0        0        0     4949 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/ManchesterCityCouncil.py
+-rw-r--r--   0        0        0     1895 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/MertonCouncil.py
+-rw-r--r--   0        0        0     2711 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/MidSussexDistrictCouncil.py
+-rw-r--r--   0        0        0     2011 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/MiltonKeynesCityCouncil.py
+-rw-r--r--   0        0        0     2146 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NewarkAndSherwoodDC.py
+-rw-r--r--   0        0        0     1997 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NewcastleCityCouncil.py
+-rw-r--r--   0        0        0     1831 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NorthEastLincs.py
+-rw-r--r--   0        0        0     1522 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NorthKestevenDistrictCouncil.py
+-rw-r--r--   0        0        0     1675 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NorthLanarkshireCouncil.py
+-rw-r--r--   0        0        0     2407 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NorthLincolnshireCouncil.py
+-rw-r--r--   0        0        0     3723 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NorthNorfolkDistrictCouncil.py
+-rw-r--r--   0        0        0     2679 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NorthSomersetCouncil.py
+-rw-r--r--   0        0        0    10889 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NorthTynesideCouncil.py
+-rw-r--r--   0        0        0     4695 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NorthumberlandCouncil.py
+-rw-r--r--   0        0        0     3900 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/PrestonCityCouncil.py
+-rw-r--r--   0        0        0     2347 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/RochdaleCouncil.py
+-rw-r--r--   0        0        0     3514 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/RushcliffeBoroughCouncil.py
+-rw-r--r--   0        0        0     2043 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/RushmoorCouncil.py
+-rw-r--r--   0        0        0     2512 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SalfordCityCouncil.py
+-rw-r--r--   0        0        0     1997 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SheffieldCityCouncil.py
+-rw-r--r--   0        0        0     8499 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SomersetCouncil.py
+-rw-r--r--   0        0        0     2728 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SouthAyrshireCouncil.py
+-rw-r--r--   0        0        0     2313 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SouthCambridgeshireCouncil.py
+-rw-r--r--   0        0        0     3132 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SouthLanarkshireCouncil.py
+-rw-r--r--   0        0        0     3966 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SouthNorfolkCouncil.py
+-rw-r--r--   0        0        0     3208 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SouthOxfordshireCouncil.py
+-rw-r--r--   0        0        0     3432 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SouthTynesideCouncil.py
+-rw-r--r--   0        0        0     1960 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/StHelensBC.py
+-rw-r--r--   0        0        0     1404 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/StockportBoroughCouncil.py
+-rw-r--r--   0        0        0     2040 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SwaleBoroughCouncil.py
+-rw-r--r--   0        0        0     2001 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/TamesideMBCouncil.py
+-rw-r--r--   0        0        0     4865 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/TonbridgeAndMallingBC.py
+-rw-r--r--   0        0        0     2035 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/TorbayCouncil.py
+-rw-r--r--   0        0        0     6074 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/TorridgeDistrictCouncil.py
+-rw-r--r--   0        0        0     4863 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/ValeofGlamorganCouncil.py
+-rw-r--r--   0        0        0     3916 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/WakefieldCityCouncil.py
+-rw-r--r--   0        0        0     1153 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/WarwickDistrictCouncil.py
+-rw-r--r--   0        0        0     4667 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/WaverleyBoroughCouncil.py
+-rw-r--r--   0        0        0     3374 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/WealdenDistrictCouncil.py
+-rw-r--r--   0        0        0     2284 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/WelhatCouncil.py
+-rw-r--r--   0        0        0     3612 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/WiganBoroughCouncil.py
+-rw-r--r--   0        0        0     5207 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/WiltshireCouncil.py
+-rw-r--r--   0        0        0     5536 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/WindsorAndMaidenheadCouncil.py
+-rw-r--r--   0        0        0     5027 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/WokingBoroughCouncil.py
+-rw-r--r--   0        0        0     1496 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/YorkCouncil.py
+-rw-r--r--   0        0        0     1121 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/council_class_template/councilclasstemplate.py
+-rw-r--r--   0        0        0     4549 2023-07-28 16:58:25.686787 uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/get_bin_data.py
+-rw-r--r--   0        0        0     7775 1970-01-01 00:00:00.000000 uk_bin_collection-0.9.0/PKG-INFO
```

### Comparing `uk_bin_collection-0.80.0/LICENSE` & `uk_bin_collection-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.80.0/README.md` & `uk_bin_collection-0.9.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,51 @@
-[![Made with Python](https://img.shields.io/badge/Made%20With%20Python-red?style=for-the-badge&logo=python&logoColor=white&labelColor=red)](https://www.python.org)
+Metadata-Version: 2.1
+Name: uk-bin-collection
+Version: 0.9.0
+Summary: Python Lib to collect UK Bin Data
+Author: Robert Bradley
+Author-email: robbrad182@gmail.com
+Requires-Python: >=3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: bs4
+Requires-Dist: holidays
+Requires-Dist: lxml
+Requires-Dist: pandas
+Requires-Dist: requests
+Requires-Dist: selenium
+Project-URL: issues, https://github.com/robbrad/UKBinCollectionData/issues
+Description-Content-Type: text/markdown
 
-[![HACS Badge](https://img.shields.io/badge/HACS-Custom-41BDF5.svg?style=for-the-badge)](https://github.com/robbrad/UKBinCollectionData)
-[![Current Release](https://img.shields.io/github/v/release/robbrad/UKBinCollectionData?style=for-the-badge&filter=*)](https://github.com/robbrad/UKBinCollectionData/releases)
-[![PyPi](https://img.shields.io/pypi/v/uk_bin_collection?label=PyPI&logo=pypi&style=for-the-badge&color=blue)](https://pypi.org/project/uk-bin-collection/)
-
-[![GitHub license](https://img.shields.io/github/license/robbrad/UKBinCollectionData?style=for-the-badge)](https://github.com/robbrad/UKBinCollectionData/blob/master/LICENSE)
-[![GitHub issues](https://img.shields.io/github/issues-raw/robbrad/UKBinCollectionData?style=for-the-badge)](https://github.com/robbrad/UKBinCollectionData/issues?q=is%3Aopen+is%3Aissue)
-[![GitHub closed issues](https://img.shields.io/github/issues-closed-raw/robbrad/UKBinCollectionData?style=for-the-badge)](https://github.com/robbrad/UKBinCollectionData/issues?q=is%3Aissue+is%3Aclosed)
-[![GitHub contributors](https://img.shields.io/github/contributors/robbrad/UKBinCollectionData?style=for-the-badge)](https://github.com/robbrad/UKBinCollectionData/graphs/contributors)
+[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 
-[![Test Councils](https://img.shields.io/github/actions/workflow/status/robbrad/UKBinCollectionData/behave.yml?style=for-the-badge&label=Test+Councils)](https://github.com/robbrad/UKBinCollectionData/actions/workflows/behave.yml)
+![GitHub](https://img.shields.io/github/license/robbrad/UKBinCollectionData?style=for-the-badge) ![GitHub issues](https://img.shields.io/github/issues-raw/robbrad/UKBinCollectionData?style=for-the-badge) ![GitHub closed issues](https://img.shields.io/github/issues-closed-raw/robbrad/UKBinCollectionData?style=for-the-badge)
+![GitHub contributors](https://img.shields.io/github/contributors/robbrad/UKBinCollectionData?style=for-the-badge)
+
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/robbrad/UKBinCollectionData/behave.yml?style=for-the-badge)
 ![Codecov](https://img.shields.io/codecov/c/gh/robbrad/UKBinCollectionData?style=for-the-badge)
-[![CodeQL Analysis](https://img.shields.io/github/actions/workflow/status/robbrad/UKBinCollectionData/codeql-analysis.yml?style=for-the-badge&label=CodeQL+Analysis)](https://github.com/robbrad/UKBinCollectionData/actions/workflows/codeql-analysis.yml)
-[![Publish Release](https://img.shields.io/github/actions/workflow/status/robbrad/UKBinCollectionData/release.yml?style=for-the-badge&label=Publish+Release)](https://github.com/robbrad/UKBinCollectionData/actions/workflows/release.yml)
-[![Test Report Deployment](https://img.shields.io/github/actions/workflow/status/robbrad/UKBinCollectionData/pages%2Fpages-build-deployment?style=for-the-badge&label=Test+Report+Deployment)](https://github.com/robbrad/UKBinCollectionData/actions/workflows/pages/pages-build-deployment)
+
+[![pages-build-deployment](https://github.com/robbrad/UKBinCollectionData/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/robbrad/UKBinCollectionData/actions/workflows/pages/pages-build-deployment) [![Test Councils](https://github.com/robbrad/UKBinCollectionData/actions/workflows/behave.yml/badge.svg)](https://github.com/robbrad/UKBinCollectionData/actions/workflows/behave.yml)
 
 # UK Bin Collection Data (UKBCD)
 This project aims to provide a neat and standard way of providing bin collection data in JSON format from UK councils that have no API to do so.
 
 Why do this?
 You might want to use this in a Home Automation - for example say you had an LED bar that lit up on the day of bin collection to the colour of the bin you want to take out, then this repo provides the data for that. 
 
-**PLEASE respect a councils infrastructure / usage policy and only collect data for your own personal use on a suitable frequency to your collection schedule.**
+**PLEASE respect a councils infrastructure / usage policy and only collect data for your own personal use on a sutable frequency to your collection schedule.**
 
 Most scripts make use of [Beautiful Soup 4](https://pypi.org/project/beautifulsoup4/) to scrape data, although others use different approaches, such as emulating web browser behaviour, or reading data from CSV files.
 
-[![](https://img.shields.io/badge/-41BDF5?style=for-the-badge&logo=homeassistant&logoColor=white&label=HomeAssistant+Thread)](https://community.home-assistant.io/t/bin-waste-collection/55451)
-[![](https://img.shields.io/badge/Request%20a%20council-gray?style=for-the-badge&logo=github&logoColor=white)](https://github.com/robbrad/UKBinCollectionData/issues/new/choose)
-
----
-
-## Home Assistant Usage
-
-### Install with HACS (recommended)
-
-1. Ensure you have [HACS](https://hacs.xyz/) installed
-1. In the Home Assistant UI go to `HACS` > `Integrations` > `⋮` > `Custom repositories`.
-1. Enter `https://github.com/robbrad/UKBinCollectionData` in the `Repository` field.
-1. Select `Integration` as the category then click `ADD`.
-1. Click `+ Add Integration` and search for and select `UK Bin Collection Data` then click `Download`.
-1. Restart your Home Assistant.
-1. In the Home Assistant UI go to `Settings` > `Devices & Services` click `+ Add Integration` and search for `UK Bin Collection Data`.
-1. If your see a "URL of the remote Selenium web driver to use" field when setting up your council, you'll need to provide the URL to a web driver you've set up seperately such as [standalone-chrome](https://hub.docker.com/r/selenium/standalone-chrome).
-
-### Install manually
-
-1. Open the folder for your Home Assistant configuration (where you find `configuration.yaml`).
-1. If you do not have a `custom_components` folder there, you need to create it.
-1. [Download](https://github.com/robbrad/UKBinCollectionData/archive/refs/heads/master.zip) this repository then copy the folder `custom_components/uk_bin_collection` into the `custom_components` folder you found/created in the previous step.
-1. Restart your Home Assistant.
-1. In the Home Assistant UI go to `Settings` > `Devices & Services` click `+ Add Integration` and search for `UK Bin Collection Data`.
+[![](https://img.shields.io/badge/--41BDF5?logo=homeassistant&logoColor=white&label=HomeAssistant+Thread)](https://community.home-assistant.io/t/bin-waste-collection/55451) [![](https://img.shields.io/badge/--181717?logo=github&logoColor=white&label=Request+a+council)](https://github.com/robbrad/UKBinCollectionData/issues/new/choose)
 
 ---
 
-## Standalone Usage
+## Usage
 ```commandline
 PS G:\Projects\Python\UKBinCollectionData\uk_bin_collection\collect_data.py
 usage: collect_data.py [-h] [-p POSTCODE] [-n NUMBER] [-u UPRN] module URL
 
 positional arguments:
   module                Name of council module to use                           (required)
   URL                   URL to parse                                            (required)
@@ -67,14 +55,15 @@
   -p POSTCODE, --postcode POSTCODE      Postcode to parse - should include      (optional)
                                         a space and be wrapped in double
                                         quotes                                  
   -n NUMBER, --number NUMBER            House number to parse                   (optional)
   -u UPRN, --uprn UPRN                  UPRN to parse                           (optional)
 ```
 
+
 ### Quickstart
 The basic command to execute a script is:
 ```commandline
 python collect_data.py <council_name> "<collection_url>"
 ```
 where ```council_name``` is the name of the council's .py script (without the .py) and ```collection_url``` is the URL to scrape.
 The help documentation refers to these as "module" and "URL", respectively. Supported council scripts can be found in the `uk_bin_collection/uk_bin_collection/councils` folder.
@@ -94,119 +83,33 @@
 
 
 ### Project dependencies
 Some scripts rely on external packages to function. A list of required scripts for both development and execution can be found in the project's [PROJECT_TOML](https://github.com/robbrad/UKBinCollectionData/blob/feature/%2353_integration_tests/pyproject.toml) 
 Install can be done via 
 `poetry install` from within the root of the repo.
 
----
 
-## UPRN Finder
+### UPRN Finder
 Some councils make use of the UPRN (Unique property reference number) to identify your property. You can find yours [here](https://www.findmyaddress.co.uk/search) or [here](https://uprn.uk/).
 
----
-
 ## Requesting your council
 To make a request for your council, first check the [Issues](https://github.com/robbrad/UKBinCollectionData/issues) page to make sure it has not already been requested. If not, please fill in a new [Council Request](https://github.com/robbrad/UKBinCollectionData/issues/new/choose) form, including as much information as possible, including:
 - Name of the council
 - URL to bin collections
 - An example postcode and/or UPRN (whichever is relevant)
 - Any further information
 
 Please be aware that this project is run by volunteer contributors and completion depends on numerous factors - even with a request, we cannot guarantee if/when your council will get a script.
 
 ---
 
 ## Reports
 
+- [3.10](https://robbrad.github.io/UKBinCollectionData/3.10/)
 - [3.11](https://robbrad.github.io/UKBinCollectionData/3.11/)
-- [3.12](https://robbrad.github.io/UKBinCollectionData/3.12/)
-
----
-## Docker API Server
-We have created an API for this located under [uk_bin_collection_api_server](https://github.com/robbrad/UKBinCollectionData/uk_bin_collection_api_server)
-
-### Prerequisites
-
-- Docker installed on your machine
-- Python (if you plan to run the API locally without Docker)
-
-### Running the API with Docker
-
-1. Clone this repository.
-2. Navigate to the uk_bin_collection_api_server directory of the project.
-
-#### Build the Docker Container
-
-```bash
-docker build -t ukbc_api_server .
-```
-
-```
-docker run -p 8080:8080 ukbc_api_server
-```
-
-#### Accessing the API
-
-Once the Docker container is running, you can access the API endpoints:
-
-    API Base URL: http://localhost:8080/api
-    Swagger UI: http://localhost:8080/api/ui/
-
-#### API Documentation
-
-The API documentation can be accessed via the Swagger UI. Use the Swagger UI to explore available endpoints, test different requests, and understand the API functionalities.
-
-![Swagger UI](SwaggerUI.png)
-
-#### API Endpoints
-`GET /bin_collection/{council}`
-
-Description: Retrieves information about bin collection for the specified council.
-
-Parameters:
-
-    council (required): Name of the council.
-    Other optional parameters: [Specify optional parameters if any]
-
-Example Request:
-
-```bash
-curl -X GET "http://localhost:8080/api/bin_collection/{council}" -H "accept: application/json"
-```
-
-## Docker Compose
-This includes the Selenium standalone-chrome for Selenium based councils
-
-```
-version: '3'
-
-services:
-  ukbc_api_server:
-    build:
-      context: .
-      dockerfile: Dockerfile 
-    ports:
-      - "8080:8080"  # Adjust the ports as needed
-    depends_on:
-      - selenium
-
-  selenium:
-    image: selenium/standalone-chrome:latest
-    ports:
-      - "4444:4444"
-
-```
-### Run with
-```bash
-sudo apt-get update
-sudo apt-get install docker-compose
-
-docker-compose up
-```
 
 ---
 
 ## FAQ
 #### I've got an issue/support question - what do I do?
 Please post in the [HomeAssistant thread](https://community.home-assistant.io/t/bin-waste-collection/55451) or raise a new (non council request) [issue](https://github.com/robbrad/UKBinCollectionData/issues/new).
 
@@ -217,7 +120,8 @@
 - If you would like to try writing your own scraper, feel free to fork this project and use existing scrapers as a base for your approach (or `councilclasstemplate.py`).
 
 ## Contributors
 <a href="https://github.com/robbrad/UKBinCollectionData/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=robbrad/UKBinCollectionData"  alt="Image of contributors"/>
 </a>
 
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `uk_bin_collection-0.80.0/pyproject.toml` & `uk_bin_collection-0.9.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uk_bin_collection"
-version = "0.80.0"
+version = "0.9.0"
 description = "Python Lib to collect UK Bin Data"
 readme = "README.md"
 authors = ["Robert Bradley <robbrad182@gmail.com>"]
 packages = [
     { include = "uk_bin_collection", from = "." },
 ]
 include = ["uk_bin_collection"]
@@ -31,42 +31,27 @@
 jsonschema = "*"
 pylint = "*"
 pytest = "*"
 setuptools = "*"
 pytest-bdd = "*"
 allure-pytest-bdd = "*"
 pytest-xdist = {extras = ["psutil"], version = "*"}
-pyhamcrest = "*"
-tabulate = "^0.9.0"
+
 
 [tool.poetry.scripts]
-uk_bin_collection = "uk_bin_collection.uk_bin_collection.collect_data:run"
+uk_bin_collection = "uk_bin_collection.uk_bin_collection:collect_data"
 
 [tool.dephell.main]
 versioning = "semver"
 from = {format = "poetrylock", path = "poetry.lock"}
 envs = ["main"]
 to = {format = "poetry", path = "pyproject.toml"}
 
 [tool.poetry.dependencies]
 bs4 = "*"
-python-dateutil = "*"
 holidays = "*"
 pandas = "*"
-python = ">=3.11"
+python = ">=3.10"
 requests = "*"
 selenium = "*"
 lxml = "*"
-urllib3 = "*"
-webdriver-manager = "^4.0.1"
-tabulate = "^0.9.0"
-
-[tool.commitizen]
-major_version_zero = true
-version_provider = "poetry"
-version_scheme = "semver"
-version_files = [
-    "custom_components/uk_bin_collection/manifest.json:version",
-    "custom_components/uk_bin_collection/manifest.json:requirements",
-    "custom_components/uk_bin_collection/config_flow.py:githubusercontent"
-]
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/tests/output.schema` & `uk_bin_collection-0.9.0/uk_bin_collection/tests/council_schemas/LeedsCityCouncil.schema`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7075520833333333%*

 * *Differences: {"'$ref'": "'#/definitions/Welcome2'",*

 * * "'definitions'": "{'Bin': {'properties': {'type': {replace: OrderedDict([('$ref', "*

 * *                  "'#/definitions/Type')])}, 'collectionDate': {delete: ['pattern']}}}, "*

 * *                  "'Welcome2': OrderedDict([('type', 'object'), ('additionalProperties', False), "*

 * *                  "('properties', OrderedDict([('bins', OrderedDict([('type', 'array'), ('items', "*

 * *                  "OrderedDict([('$ref', '#/definitions/Bin')]))]))])), ('required', ['bins']), "*

 * *  […]*

```diff
@@ -1,41 +1,48 @@
 {
-    "$ref": "#/definitions/BinData",
+    "$ref": "#/definitions/Welcome2",
     "$schema": "http://json-schema.org/draft-06/schema#",
     "definitions": {
         "Bin": {
             "additionalProperties": false,
             "properties": {
                 "collectionDate": {
-                    "pattern": "\\d{2}/\\d{2}/\\d{4}",
                     "type": "string"
                 },
                 "type": {
-                    "type": "string"
+                    "$ref": "#/definitions/Type"
                 }
             },
             "required": [
                 "collectionDate",
                 "type"
             ],
             "title": "Bin",
             "type": "object"
         },
-        "BinData": {
+        "Type": {
+            "enum": [
+                "GREEN",
+                "BROWN",
+                "BLACK"
+            ],
+            "title": "Type",
+            "type": "string"
+        },
+        "Welcome2": {
             "additionalProperties": false,
             "properties": {
                 "bins": {
                     "items": {
                         "$ref": "#/definitions/Bin"
                     },
-                    "minItems": 1,
                     "type": "array"
                 }
             },
             "required": [
                 "bins"
             ],
-            "title": "BinData",
+            "title": "Welcome2",
             "type": "object"
         }
     }
 }
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/tests/test_collect_data.py` & `uk_bin_collection-0.9.0/uk_bin_collection/tests/test_collect_data.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from unittest import mock
 
 import pytest
 from requests import exceptions as req_exp
 from requests.models import Response
 from uk_bin_collection.get_bin_data import AbstractGetBinDataClass as agbdc
 from uk_bin_collection.get_bin_data import setup_logging
-import logging
 
 
 def mocked_requests_get(*args, **kwargs):
     class MockResponse:
         def __init__(self, json_data, status_code, raise_error_type):
             self.text = json_data
             self.status_code = status_code
@@ -51,40 +50,14 @@
 def test_logging_exception():
     logging_dict = "SW1A 1AA"
     with pytest.raises(ValueError) as exc_info:
         result = setup_logging(logging_dict, "ROOT")
     assert exc_info.typename == "ValueError"
 
 
-def test_setup_logging_valid_config():
-    # Example of a minimal valid logging configuration dictionary
-    logging_config = {
-        "version": 1,
-        "handlers": {
-            "console": {
-                "class": "logging.StreamHandler",
-                "level": "DEBUG",
-            },
-        },
-        "loggers": {
-            "ROOT": {
-                "handlers": ["console"],
-                "level": "DEBUG",
-            },
-        },
-    }
-    logger_name = "ROOT"
-    # Run the function with valid logging configuration
-    logger = setup_logging(logging_config, logger_name)
-
-    # Assert that logger is correctly configured
-    assert logger.name == logger_name
-    assert logger.level == logging.DEBUG
-
-
 @mock.patch("requests.get", side_effect=mocked_requests_get)
 def test_get_data(mock_get):
     page_data = agbdc.get_data("aurl")
     assert page_data.text == {"test_data": "test"}
 
 
 @pytest.mark.parametrize(
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/AdurAndWorthingCouncils.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/council_class_template/councilclasstemplate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import bs4.element
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
@@ -14,30 +14,19 @@
 
     def parse_data(self, page: str, **kwargs) -> dict:
         # Make a BS4 object
         soup = BeautifulSoup(page.text, features="html.parser")
         soup.prettify()
 
         data = {"bins": []}
-        collections = []
 
-        for bin in (
-            soup.find("table", {"class": "no-style bin-days"})
-            .find("tbody")
-            .find_all("tr")
-        ):
-            bin_type = bin.find("th").get_text().strip() + " bin"
-            bin_dates = bin.find_all("td")[1].contents
-            for date in bin_dates:
-                if type(date) == bs4.element.NavigableString:
-                    bin_date = datetime.strptime(date, "%A %d %b %Y")
-                    collections.append((bin_type, bin_date))
-
-        ordered_data = sorted(collections, key=lambda x: x[1])
-        for item in ordered_data:
-            dict_data = {
-                "type": item[0].capitalize(),
-                "collectionDate": item[1].strftime(date_format),
-            }
-            data["bins"].append(dict_data)
+        for bins in soup.select('div[class*="service-item"]'):
+            bin_type = bins.div.h3.text.strip()
+            bin_collection = bins.select("div > p")[1]
+            if bin_collection:
+                dict_data = {
+                    "type": bin_type,
+                    "collectionDate": datetime.strptime(bin_collection.get_text(strip=True), "%A, %d %B %Y")
+                }
+                data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ArunCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/PrestonCityCouncil.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,103 @@
-import time
+from datetime import datetime
 
 from bs4 import BeautifulSoup
 from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
+from selenium.webdriver.common.keys import Keys
+from selenium.webdriver.support.ui import Select
+from selenium.webdriver.support.wait import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import Select, WebDriverWait
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
+
+
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        try:
-            # Make a BS4 object
-            data = {"bins": []}
-
-            user_paon = kwargs.get("paon")
-            user_postcode = kwargs.get("postcode")
-            headless = kwargs.get("headless")
-            web_driver = kwargs.get("web_driver")
-            driver = create_webdriver(web_driver, headless, None, __name__)
-            page = "https://www1.arun.gov.uk/when-are-my-bins-collected/"
-            check_paon(user_paon)
-            check_postcode(user_postcode)
-            driver.get(page)
-
-            start_now_button = WebDriverWait(driver, timeout=15).until(
-                EC.presence_of_element_located((By.LINK_TEXT, "Start now"))
-            )
-            start_now_button.click()
+        page = "https://selfservice.preston.gov.uk/service/Forms/FindMyNearest.aspx?Service=bins"
 
-            # Wait for the postcode field to appear then populate it
-            input_element_postcode = WebDriverWait(driver, 30).until(
-                EC.presence_of_element_located((By.ID, "postcode"))
-            )
-            input_element_postcode.send_keys(user_postcode)
-
-            continue_button = WebDriverWait(driver, timeout=15).until(
-                EC.presence_of_element_located((By.CLASS_NAME, "govuk-button"))
-            )
-            continue_button.click()
+        data = {"bins": []}
 
-            address_selection_menu = Select(driver.find_element(By.ID, "address"))
-            for idx, addr_option in enumerate(address_selection_menu.options):
-                option_name = addr_option.text[0 : len(user_paon)]
-                if option_name == user_paon:
-                    selected_address = addr_option
-                    break
-            address_selection_menu.select_by_visible_text(selected_address.text)
-
-            continue_button = WebDriverWait(driver, timeout=15).until(
-                EC.presence_of_element_located((By.CLASS_NAME, "govuk-button"))
-            )
-            continue_button.click()
-            # Check for text saying "Next collection dates"
-            WebDriverWait(driver, 30).until(
-                EC.presence_of_element_located(
-                    (By.XPATH, "//*[contains(text(), 'Next collection dates')]")
-                )
+        user_paon = kwargs.get("paon")
+        user_postcode = kwargs.get("postcode")
+        check_paon(user_paon)
+        check_postcode(user_postcode)
+
+        # Set up Selenium to run 'headless'
+        options = webdriver.ChromeOptions()
+        options.add_argument("--headless")
+        options.add_argument("--no-sandbox")
+        options.add_argument("--disable-gpu")
+        options.add_argument("--disable-dev-shm-usage")
+        options.add_experimental_option("excludeSwitches", ["enable-logging"])
+
+        # Create Selenium webdriver
+        driver = webdriver.Chrome(options=options)
+        driver.get(page)
+
+        # If you bang in the house number (or property name) and postcode in the box it should find your property
+        inputElement_address = driver.find_element(
+            By.ID,
+            "MainContent_txtAddress",
+        )
+
+        inputElement_address.send_keys(user_paon)
+        inputElement_address.send_keys(" ")
+        inputElement_address.send_keys(user_postcode)
+
+        driver.find_element(
+            By.ID,
+            "btnSearch",
+        ).click()
+
+        # Wait for the 'Select your property' dropdown to appear and select the first result
+        dropdown = WebDriverWait(driver, 10).until(
+            EC.presence_of_element_located((By.ID, "MainContent_ddlSearchResults"))
+        )
+        # Create a 'Select' for it, then select the first address in the list
+        # (Index 0 is "Make a selection from the list")
+        dropdownSelect = Select(dropdown)
+        dropdownSelect.select_by_index(1)
+
+        # Wait for the 'View more' link to appear, then click it to get the full set of dates
+        viewMoreLink = WebDriverWait(driver, 10).until(
+            EC.presence_of_element_located((By.LINK_TEXT, "View more collection dates"))
+        )
+        viewMoreLink.click()
+
+        soup = BeautifulSoup(driver.page_source, features="html.parser")
+
+        topLevelSpan = soup.find(
+            "span",
+            id="lblCollectionDates"
+        )
+
+        collectionDivs = topLevelSpan.findChildren(recursive=False)
+        for collectionDiv in collectionDivs:
+            # Each date has two child divs - the date and the bin type
+            # However both strings are in <b> tags so there are 4 children, the text is at:
+            # Index 1 - date string i.e. 'Monday 01/01/2023'
+            # Index 3 - bin type i.e. 'General waste'
+            typeAndDateDivs = collectionDiv.findChildren()
+
+            # Strip the day (i.e. Monday) out of the collection date string for parsing
+            dateString = typeAndDateDivs[1].text.split(' ')[1]
+
+            data["bins"].append(
+                {
+                    "type": typeAndDateDivs[3].text,
+                    "collectionDate": datetime.strptime(dateString, "%d/%m/%Y").strftime(date_format)
+                }
             )
 
-            soup = BeautifulSoup(driver.page_source, "html.parser")
-            soup.prettify()
-            table = soup.find("table", class_="govuk-table")
-
-            for row in table.find("tbody").find_all("tr"):
-                # Extract the type of collection and the date of next collection
-                collection_type = (
-                    row.find("th", class_="govuk-table__header").text.strip().split(" ")
-                )[0]
-                collection_date = row.find(
-                    "td", class_="govuk-table__cell"
-                ).text.strip()
-
-                # Append the information to the data structure
-                data["bins"].append(
-                    {"type": collection_type, "collectionDate": collection_date}
-                )
-
-        except Exception as e:
-            # Here you can log the exception if needed
-            print(f"An error occurred: {e}")
-            # Optionally, re-raise the exception if you want it to propagate
-            raise
-        finally:
-            # This block ensures that the driver is closed regardless of an exception.
-            if driver:
-                driver.quit()
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/AylesburyValeCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/WelhatCouncil.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,69 +1,72 @@
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
+
+
+def get_token(page) -> str:
+    """
+    Get a __token to include in the form data
+        :param page: Page html
+        :return: Form __token
+    """
+    soup = BeautifulSoup(page.text, features="html.parser")
+    soup.prettify()
+    token = soup.find("input", {"name": "__token"}).get("value")
+    return token
 
 
-# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
         uprn = kwargs.get("uprn")
+        postcode = kwargs.get("postcode")
         check_uprn(uprn)
+        check_postcode(postcode)
 
-        # Make SOAP Request
-        headers = {
-            "Content-Type": "text/xml; charset=UTF-8",
-            "SOAPAction": '"http://tempuri.org/GetCollections"',
+        values = {
+            "__token": get_token(page),
+            "page": "492",
+            "locale": "en_GB",
+            "q9f451fe0ca70775687eeedd1e54b359e55f7c10c_0_0": postcode,
+            "q9f451fe0ca70775687eeedd1e54b359e55f7c10c_1_0": uprn,
+            "next": "Next",
         }
-
-        post_data = (
-            '<?xml version="1.0" encoding="utf-8"?><soap:Envelope '
-            'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
-            'xmlns:xsd="http://www.w3.org/2001/XMLSchema" '
-            'xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"><soap:Body><GetCollections '
-            'xmlns="http://tempuri.org/"><uprn>'
-            + uprn
-            + "</uprn></GetCollections></soap:Body></soap:Envelope>"
-        )
-
-        response = requests.post(
-            "http://avdcbins.web-labs.co.uk/RefuseApi.asmx",
-            data=post_data,
+        headers = {"User-Agent": "Mozilla/5.0 (Windows NT 6.1; Win64; x64)"}
+        requests.packages.urllib3.disable_warnings()
+        response = requests.request(
+            "POST",
+            "https://www.welhat.gov.uk/xfp/form/214",
             headers=headers,
+            data=values,
         )
 
-        if response.status_code != 200:
-            raise ValueError("No collection data found for provided UPRN.")
+        soup = BeautifulSoup(response.text, features="html.parser")
 
-        # Make a BS4 object
-        soup = BeautifulSoup(response.text, "xml")
-        soup.prettify()
+        rows = soup.find("table").find_all("tr")
 
+        # Form a JSON wrapper
         data = {"bins": []}
 
-        all_collections = soup.find_all("BinCollection")
-
-        for i in range(len(all_collections)):
-            collection_date = datetime.strptime(
-                all_collections[i].Date.get_text(), "%Y-%m-%dT%H:%M:%S"
-            )
-            children = all_collections[i].find_all(
-                ["Refuse", "Recycling", "Garden", "Food"], string="true"
-            )
+        # Loops the Rows
+        for row in rows:
+            cells = row.find_all("td")
+            if cells:
+                binType = cells[0].get_text(strip=True)
+                collectionDate = datetime.strptime(cells[1].get_text(strip=True), "%A %d %B  %Y").strftime(date_format)
 
-            for collection in children:
+                # Make each Bin element in the JSON
                 dict_data = {
-                    "type": collection.name,
-                    "collectionDate": collection_date.strftime(date_format),
+                    "type": binType,
+                    "collectionDate": collectionDate,
                 }
+
+                # Add data to the main JSON Wrapper
                 data["bins"].append(dict_data)
 
-        data["bins"].sort(
-            key=lambda x: datetime.strptime(x.get("collectionDate"), date_format)
-        )
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BCPCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/BCPCouncil.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,40 @@
 import json
-from datetime import timedelta
 
 import requests
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-
         user_uprn = kwargs.get("uprn")
         check_uprn(user_uprn)
 
         api_url = f"https://online.bcpcouncil.gov.uk/bcp-apis/?api=BinDayLookup&uprn={user_uprn}"
 
         requests.packages.urllib3.disable_warnings()
         response = requests.get(api_url)
         json_data = json.loads(response.text)
         data = {"bins": []}
         collections = []
 
         for bin in json_data:
             bin_type = bin["BinType"]
-            next_date = datetime.strptime(
-                bin["Next"], "%m/%d/%Y %I:%M:%S %p"
-            ) + timedelta(hours=1)
-            subseq_date = datetime.strptime(
-                bin["Subsequent"], "%m/%d/%Y %I:%M:%S %p"
-            ) + timedelta(hours=1)
+            next_date = datetime.strptime(bin["Next"], "%m/%d/%Y %H:%M:%S %p")
+            subseq_date = datetime.strptime(bin["Subsequent"], "%m/%d/%Y %H:%M:%S %p")
             collections.append((bin_type, next_date))
             collections.append((bin_type, subseq_date))
 
         ordered_data = sorted(collections, key=lambda x: x[1])
         data = {"bins": []}
         for item in ordered_data:
             dict_data = {
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BarnsleyMBCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SouthNorfolkCouncil.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,109 +1,89 @@
-from typing import Dict, Any
+from xml.etree import ElementTree
+
 from bs4 import BeautifulSoup
-from dateutil.relativedelta import relativedelta
-import requests
-from datetime import datetime
-from uk_bin_collection.uk_bin_collection.common import (
-    check_postcode,
-    check_uprn,
-    date_format,
-)
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.common import *
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
-    base class. They can also override some operations with a default
-    implementation.
+    baseclass. They can also override some
+    operations with a default implementation.
     """
 
-    def parse_data(self, page: str, **kwargs: Any) -> Dict[str, Any]:
-        data: Dict[str, Any] = {"bins": []}
-
-        # Get UPRN and postcode from kwargs
-        user_uprn = str(kwargs.get("uprn"))
-        user_postcode = str(kwargs.get("postcode"))
-        check_postcode(user_postcode)
-        check_uprn(user_uprn)
+    def parse_data(self, page: str, **kwargs) -> dict:
+        uprn = kwargs.get("uprn")
+        check_uprn(uprn)
+        council = "SNO"
 
-        # Pass in form data and make the POST request
+        # Make SOAP request
         headers = {
-            "authority": "waste.barnsley.gov.uk",
-            "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
-            "accept-language": "en-GB,en;q=0.9",
-            "cache-control": "no-cache",
-            "content-type": "application/x-www-form-urlencoded",
-            "origin": "https://waste.barnsley.gov.uk",
-            "pragma": "no-cache",
-            "referer": "https://waste.barnsley.gov.uk/ViewCollection/SelectAddress",
-            "sec-ch-ua": '"Chromium";v="118", "Opera GX";v="104", "Not=A?Brand";v="99"',
+            "Accept": "*/*",
+            "Accept-Encoding": "gzip, deflate, br",
+            "Accept-Language": "en-GB,en-US;q=0.9,en;q=0.8",
+            "Connection": "keep-alive",
+            "Content-Type": "text/xml; charset=UTF-8",
+            "Host": "collections-southnorfolk.azurewebsites.net",
+            "Origin": "https://collections-southnorfolk.azurewebsites.net",
+            "Referer": "https://collections-southnorfolk.azurewebsites.net/calendar.html",
+            "sec-ch-ua": '"Chromium";v="110", "Not A(Brand";v="24", "Google Chrome";v="110"',
             "sec-ch-ua-mobile": "?0",
             "sec-ch-ua-platform": '"Windows"',
-            "sec-fetch-dest": "document",
-            "sec-fetch-mode": "navigate",
-            "sec-fetch-site": "same-origin",
-            "sec-fetch-user": "?1",
-            "upgrade-insecure-requests": "1",
-            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/118.0.5993.118 Safari/537.36",
-        }
-        form_data = {
-            "personInfo.person1.HouseNumberOrName": "",
-            "personInfo.person1.Postcode": f"{user_postcode}",
-            "personInfo.person1.UPRN": f"{user_uprn}",
-            "person1_SelectAddress": "Select address",
+            "Sec-Fetch-Dest": "empty",
+            "Sec-Fetch-Mode": "cors",
+            "Sec-Fetch-Site": "same-origin",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36",
         }
+        requests.packages.urllib3.disable_warnings()
+        post_data = (
+                '<?xml version="1.0" encoding="utf-8"?>'
+                '<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">'
+                '<soap:Body><getRoundCalendarForUPRN xmlns="http://webaspx-collections.azurewebsites.net/">'
+                "<council>" + council + "</council><UPRN>" + uprn + "</UPRN>"
+                                                                    "<from>Chtml</from></getRoundCalendarForUPRN></soap:Body></soap:Envelope>"
+        )
         response = requests.post(
-            "https://waste.barnsley.gov.uk/ViewCollection/SelectAddress",
+            "https://collections-southnorfolk.azurewebsites.net/WSCollExternal.asmx",
             headers=headers,
-            data=form_data,
+            data=post_data,
         )
-
         if response.status_code != 200:
-            raise ConnectionRefusedError(
-                "Error getting results from website! Please open an issue on GitHub!"
-            )
-
-        soup = BeautifulSoup(response.text, features="html.parser")
-
-        results = soup.find_all("fieldset")
-
-        # Next collection details
-        highlight_content = results[0].find("div", {"class": "highlight-content"})
-        bin_date_str = highlight_content.find(
-            "em", {"class": "ui-bin-next-date"}
-        ).text.strip()
-        bin_type = (
-            highlight_content.find("p", {"class": "ui-bin-next-type"}).text.strip()
-            + " bin"
-        )
-
-        if bin_date_str == "Today":
-            bin_date = datetime.today()
-        elif bin_date_str == "Tomorrow":
-            bin_date = datetime.today() + relativedelta(days=1)
-        else:
-            bin_date = datetime.strptime(bin_date_str, "%A, %B %d, %Y")
-
-        dict_data = {
-            "type": bin_type,
-            "collectionDate": bin_date.strftime(date_format),
-        }
-        data["bins"].append(dict_data)
+            raise ValueError("No bin data found for provided UPRN.")
 
-        # Upcoming collections
-        upcoming_collections = results[1].find("tbody").find_all("tr")
-        for row in upcoming_collections:
-            columns = row.find_all("td")
-            bin_date_str = columns[0].text.strip()
-            bin_types = columns[1].text.strip().split(", ")
-
-            for bin_type in bin_types:
-                bin_date = datetime.strptime(bin_date_str, "%A, %B %d, %Y")
-                dict_data = {
-                    "type": bin_type.strip() + " bin",
-                    "collectionDate": bin_date.strftime(date_format),
-                }
-                data["bins"].append(dict_data)
+        # Get HTML from SOAP response
+        xmltree = ElementTree.fromstring(response.text)
+        html = xmltree.find(
+            ".//{http://webaspx-collections.azurewebsites.net/}getRoundCalendarForUPRNResult"
+        ).text
+        # Parse with BS4
+        soup = BeautifulSoup(html, features="html.parser")
+        soup.prettify()
+
+        data = {"bins": []}
+        for bin_type in ["RefuseBin", "RecycleBin", "GardenBin"]:
+            bin_el = soup.find("b", string=bin_type)
+            if bin_el:
+                bin_info = bin_el.next_sibling.split(": ")[1]
+                collection_date = ""
+                results = re.search("([A-Za-z]+ \\d\\d? [A-Za-z]+) then", bin_info)
+                if results:
+                    date = get_next_occurrence_from_day_month(datetime.strptime(
+                        results[1] + " " + datetime.now().strftime("%Y"), "%a %d %b %Y"
+                    ))
+                    if date:
+                        collection_date = date.strftime(date_format)
+                else:
+                    results2 = re.search("([A-Za-z]+) then", bin_info)
+                    if results2:
+                        collection_date = results2[1]
+
+                if collection_date != "":
+                    dict_data = {
+                        "type": bin_type,
+                        "collectionDate": collection_date,
+                    }
+                    data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BasingstokeCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/LondonBoroughHounslow.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,59 @@
 from bs4 import BeautifulSoup
-from datetime import datetime
-import requests
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
-
-COLLECTION_KINDS = {
-    "waste": "rteelem_ctl03_pnlCollections_Refuse",
-    "recycling": "rteelem_ctl03_pnlCollections_Recycling",
-    "glass": "rteelem_ctl03_pnlCollections_Glass",
-    # Garden waste data is only returned if the property is subscribed to the Garden Waste service
-    "garden": "rteelem_ctl03_pnlCollections_GardenWaste",
-}
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
+# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
-    def parse_data(self, page: str, **kwargs) -> dict:
-        requests.packages.urllib3.disable_warnings()
+    """
+    Concrete classes have to implement all abstract operations of the
+    base class. They can also override some operations with a default
+    implementation.
+    """
 
+    def parse_data(self, page: str, **kwargs) -> dict:
+        api_url = "https://www.hounslow.gov.uk/homepage/86/recycling_and_waste_collection_day_finder"
         user_uprn = kwargs.get("uprn")
-        check_uprn(user_uprn)
 
-        cookies = {
-            "cookie_control_popup": "A",
-            "WhenAreMyBinsCollected": f"{user_uprn}",
-        }
+        # Check the UPRN is valid
+        check_uprn(user_uprn)
 
-        headers = {
-            "Accept": "*/*",
-            "Accept-Language": "en-GB,en;q=0.9",
-            "Referer": "https://www.basingstoke.gov.uk/",
-            "Sec-Fetch-Dest": "document",
-            "Sec-Fetch-Mode": "navigate",
-            "Sec-Fetch-Site": "cross-site",
-            "Sec-Fetch-User": "?1",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.5845.188 Safari/537.36",
+        # Create the form data
+        form_data = {
+            "UPRN": user_uprn,
         }
 
-        response = requests.get(
-            "https://www.basingstoke.gov.uk/bincollections",
-            cookies=cookies,
-            headers=headers,
-            verify=False,
-        )
-
-        if response.status_code != 200 or response.text == "0|error|500||":
-            raise SystemError(
-                "Error retrieving data! Please try again or raise an issue on GitHub!"
-            )
+        # Make a request to the API
+        requests.packages.urllib3.disable_warnings()
+        response = requests.post(api_url, data=form_data)
 
         # Make a BS4 object
         soup = BeautifulSoup(response.text, features="html.parser")
         soup.prettify()
 
-        bins = []
+        data = {"bins": []}
 
-        for collection_type, collection_class in COLLECTION_KINDS.items():
-            for date in soup.select(f"div#{collection_class} li"):
-                date_pattern = r"\d{1,2}\s\w+\s\d{4}"  # Regex pattern to extract date
-                match = re.search(date_pattern, date.get_text(strip=True))
-
-                if match:
-                    extracted_date = match.group()
-                    formatted_date = datetime.strptime(
-                        extracted_date, "%d %B %Y"
-                    ).strftime(date_format)
-
-                    bins.append(
-                        {"type": collection_type, "collectionDate": formatted_date}
-                    )
+        # Get the div element
+        div_element = soup.find("div", {"class": "bin_day_main_wrapper"})
+
+        # Get all bins with their corresponding dates using list comprehension
+        # This creates a list of tuples, where each tuple contains the bin type and collection date
+        bins_with_dates = [
+            (
+                bin.get_text().strip(),
+                h4.get_text().replace("This ", "").replace("Next ", ""),
+            )
+            # This first for loop iterates over each h4 element
+            for h4 in div_element.find_all("h4")
+            # This nested for loop iterates over each li element within the corresponding ul element
+            for bin in h4.find_next_sibling("ul").find_all("li")
+        ]
+
+        # Add the bins to the data dict
+        data["bins"] = [
+            {"type": bin_type, "collectionDate": collection_date}
+            for bin_type, collection_date in bins_with_dates
+        ]
 
-        return {"bins": bins}
+        return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BathAndNorthEastSomersetCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/DerbyshireDalesDistrictCouncil.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,100 +1,88 @@
-import json
-import requests
 from bs4 import BeautifulSoup
+from selenium import webdriver
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support.ui import Select
+from selenium.webdriver.support.wait import WebDriverWait
+from selenium.webdriver.support import expected_conditions as EC
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
-import ssl
-import urllib3
-
-
-class CustomHttpAdapter(requests.adapters.HTTPAdapter):
-    """Transport adapter" that allows us to use custom ssl_context."""
-
-    def __init__(self, ssl_context=None, **kwargs):
-        self.ssl_context = ssl_context
-        super().__init__(**kwargs)
-
-    def init_poolmanager(self, connections, maxsize, block=False):
-        self.poolmanager = urllib3.poolmanager.PoolManager(
-            num_pools=connections,
-            maxsize=maxsize,
-            block=block,
-            ssl_context=self.ssl_context,
-        )
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
+# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
+        page = "https://selfserve.derbyshiredales.gov.uk/renderform.aspx?t=103&k=9644C066D2168A4C21BCDA351DA2642526359DFF"
+
+        data = {"bins": []}
+
         user_uprn = kwargs.get("uprn")
+        user_postcode = kwargs.get("postcode")
         check_uprn(user_uprn)
+        check_postcode(user_postcode)
 
-        headers = {
-            "Accept": "application/json, text/javascript, */*; q=0.01",
-            "Accept-Language": "en-GB,en;q=0.9",
-            "Cache-Control": "no-cache",
-            "Connection": "keep-alive",
-            "Content-Type": "application/json; charset=utf-8",
-            "Pragma": "no-cache",
-            "Referer": "https://www.bathnes.gov.uk/webforms/waste/collectionday/",
-            "Sec-Fetch-Dest": "empty",
-            "Sec-Fetch-Mode": "cors",
-            "Sec-Fetch-Site": "same-origin",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.5845.188 Safari/537.36",
-            "X-Requested-With": "XMLHttpRequest",
-        }
-
-        session = requests.Session()
-        ctx = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
-        ctx.options |= 0x4
-        session.mount("https://", CustomHttpAdapter(ctx))
-
-        requests.packages.urllib3.disable_warnings()
-        response = session.get(
-            f"https://www.bathnes.gov.uk/webapi/api/BinsAPI/v2/getbartecroute/{user_uprn}/true",
-            headers=headers,
+        # Set up Selenium to run 'headless'
+        options = webdriver.ChromeOptions()
+        options.add_argument("--headless")
+        options.add_argument("--no-sandbox")
+        options.add_argument("--disable-gpu")
+        options.add_argument("--disable-dev-shm-usage")
+        options.add_experimental_option("excludeSwitches", ["enable-logging"])
+
+        # Create Selenium webdriver
+        driver = webdriver.Chrome(options=options)
+        driver.get(page)
+
+        # Populate postcode field
+        inputElement_postcode = driver.find_element(
+            By.ID,
+            "ctl00_ContentPlaceHolder1_FF2924TB",
         )
-        if response.text == "":
-            raise ValueError(
-                "Error parsing data. Please check the provided UPRN. "
-                "If this error continues please open an issue on GitHub."
-            )
-        json_data = json.loads(response.text)
+        inputElement_postcode.send_keys(user_postcode)
 
-        data = {"bins": []}
+        # Click search button
+        driver.find_element(
+            By.ID,
+            "ctl00_ContentPlaceHolder1_FF2924BTN",
+        ).click()
+
+        # Wait for the 'Select address' dropdown to appear and select option matching UPRN
+        dropdown = WebDriverWait(driver, 10).until(
+            EC.presence_of_element_located((By.ID, "ctl00_ContentPlaceHolder1_FF2924DDL"))
+        )
+        # Create a 'Select' for it, then select the matching URPN option
+        dropdownSelect = Select(dropdown)
+        dropdownSelect.select_by_value("U" + user_uprn)
+
+        # Wait for the submit button to appear, then click it to get the collection dates
+        submit = WebDriverWait(driver, 10).until(
+            EC.presence_of_element_located((By.ID, "ctl00_ContentPlaceHolder1_btnSubmit"))
+        )
+        submit.click()
+
+        soup = BeautifulSoup(driver.page_source, features="html.parser")
 
-        if len(json_data["residualNextDate"]) > 0:
-            dict_data = {
-                "type": "Black Rubbish Bin",
-                "collectionDate": datetime.strptime(
-                    json_data["residualNextDate"], "%Y-%m-%dT%H:%M:%S"
-                ).strftime(date_format),
-            }
-            data["bins"].append(dict_data)
-        if len(json_data["recyclingNextDate"]) > 0:
-            dict_data = {
-                "type": "Recycling Containers",
-                "collectionDate": datetime.strptime(
-                    json_data["recyclingNextDate"], "%Y-%m-%dT%H:%M:%S"
-                ).strftime(date_format),
-            }
-            data["bins"].append(dict_data)
-        if len(json_data["organicNextDate"]) > 0:
-            dict_data = {
-                "type": "Garden Waste",
-                "collectionDate": datetime.strptime(
-                    json_data["organicNextDate"], "%Y-%m-%dT%H:%M:%S"
-                ).strftime(date_format),
-            }
-            data["bins"].append(dict_data)
+        bin_rows = soup.find("div", id="ctl00_ContentPlaceHolder1_pnlConfirmation") \
+            .find("div", {"class": "row"}).find_all("div", {"class": "row"})
+        if bin_rows:
+            for bin_row in bin_rows:
+                bin_data = bin_row.find_all("div")
+                if bin_data and bin_data[0] and bin_data[1]:
+                    collection_date = datetime.strptime(bin_data[0].get_text(strip=True), "%A%d %B, %Y")
+                    dict_data = {
+                        "type": bin_data[1].get_text(strip=True),
+                        "collectionDate": collection_date.strftime(date_format),
+                    }
+                    data["bins"].append(dict_data)
 
         data["bins"].sort(
             key=lambda x: datetime.strptime(x.get("collectionDate"), date_format)
         )
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BedfordBoroughCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/StHelensBC.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-import json
-import requests
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
-    base class. They can also override some operations with a default
-    implementation.
+    baseclass. They can also override some
+    operations with a default implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        user_uprn = kwargs.get("uprn")
-        check_uprn(user_uprn)
+        uprn = kwargs.get("uprn")
+        # Check the UPRN is valid
+        check_uprn(uprn)
 
-        api_url = f"https://bbaz-as-prod-bartecapi.azurewebsites.net/api/bincollections/residential/getbyuprn/{user_uprn}/35"
+        # Request URL
+        url = f"https://secure.sthelens.net/website/CollectionDates.nsf/servlet.xsp/NextCollections?source=1&refid={uprn}"
 
+        # Make Request
         requests.packages.urllib3.disable_warnings()
-        response = requests.get(api_url)
+        s = requests.session()
+        page = s.get(url)
 
-        if response.status_code != 200:
-            raise ConnectionError("Could not get latest data!")
+        # Make a BS4 object
+        soup = BeautifulSoup(re.sub("<div([^>]+)>", "", page.text).replace("</div>", ""), features="html.parser")
+        soup.prettify()
 
-        json_data = json.loads(response.text)["BinCollections"]
         data = {"bins": []}
-        collections = []
+        collection_rows = soup.find("table", {"class": "multitable"}).find("tbody").find_all("tr")
 
-        for day in json_data:
-            for bin in day:
-                bin_type = bin["BinType"]
-                next_date = datetime.strptime(
-                    bin["JobScheduledStart"], "%Y-%m-%dT%H:%M:%S"
-                )
-                collections.append((bin_type, next_date))
-
-        ordered_data = sorted(collections, key=lambda x: x[1])
-        data = {"bins": []}
-        for item in ordered_data:
-            dict_data = {
-                "type": item[0],
-                "collectionDate": item[1].strftime(date_format),
-            }
-            data["bins"].append(dict_data)
+        for collection_row in collection_rows:
+            # Get bin collection type
+            bin_type = collection_row.find("th")
+            if bin_type:
+                bin_type = bin_type.get_text(strip=True)
+                # Get bin collection dates
+                for bin_date in collection_row.find_all("td"):
+                    if bin_date.get_text(strip=True) != "Dates not allocated":
+                        collection_date = datetime.strptime(bin_date.get_text(strip=True), "%a %d %b %Y")
+                        dict_data = {
+                            "type": bin_type,
+                            "collectionDate": collection_date.strftime(date_format)
+                        }
+                        data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BedfordshireCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/BexleyCouncil.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,60 @@
-from datetime import datetime
+import json
 
 import requests
-from bs4 import BeautifulSoup
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        user_uprn = kwargs.get("uprn")
-        user_postcode = kwargs.get("postcode")
-
-        check_uprn(user_uprn)
-        check_postcode(user_postcode)
-
-        # Start a new session to walk through the form
-        requests.packages.urllib3.disable_warnings()
-        s = requests.Session()
-
+        # User email from @Home app as UPRN
+        user_email = kwargs.get("uprn")
         headers = {
-            "Origin": "https://www.centralbedfordshire.gov.uk",
-            "Referer": "https://www.centralbedfordshire.gov.uk/info/163/bins_and_waste_collections_-_check_bin_collection_day",
+            "X-country": "gb",
+            "X-email": user_email,
+            "Connection": "Keep-Alive",
         }
 
-        files = {
-            "postcode": (None, user_postcode),
-            "address": (None, user_uprn),
-        }
-
-        response = requests.post(
-            "https://www.centralbedfordshire.gov.uk/info/163/bins_and_waste_collections_-_check_bin_collection_day#my_bin_collections",
+        # Sniffed from the app
+        requests.packages.urllib3.disable_warnings()
+        response = requests.get(
+            "https://services.athomeapp.net/ServiceData/GetUserRoundJson",
             headers=headers,
-            files=files,
         )
 
-        # Make that BS4 object and use it to prettify the response
-        soup = BeautifulSoup(response.content, features="html.parser")
-        soup.prettify()
+        # 200 is OK. Sometimes it times out and gives this, but I'm not parsing HTTP codes
+        if response.status_code != 200:
+            raise ValueError(
+                "Error parsing API. Please check your email is correct and registered on the @Home app."
+            )
 
-        collections_div = soup.find(id="collections")
-
-        # Get the collection items on the page and strip the bits of text that we don't care for
+        # Load in the json and only get the bins
+        json_data = json.loads(response.text)["userrounds"]
+        data = {"bins": []}
         collections = []
-        for bin in collections_div.find_all("h3"):
-            next_bin = bin.next_sibling
 
-            while next_bin.name != "h3" and next_bin.name != "p":
-                if next_bin.name != "br":
-                    collection_date = datetime.strptime(bin.text, "%A, %d %B %Y")
-                    collections.append((next_bin, collection_date))
-                next_bin = next_bin.next_sibling
+        # For each bin, run through the list of dates and add them to a collection
+        for item in json_data:
+            bin_type = item["containername"]
+            for sched in item["nextcollectiondates"]:
+                bin_collection = datetime.strptime(
+                    sched["datestring"], "%d %m %Y %H:%M"
+                )
+                if bin_collection.date() >= datetime.now().date():
+                    collections.append((bin_type, bin_collection))
 
-        # Sort the collections by date order rather than bin type, then return as a dictionary (with str date)
+        # Order the collection of bins and dates by date order, then add to dict
         ordered_data = sorted(collections, key=lambda x: x[1])
         data = {"bins": []}
         for item in ordered_data:
             dict_data = {
                 "type": item[0],
                 "collectionDate": item[1].strftime(date_format),
             }
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BirminghamCityCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/BroxtoweBoroughCouncil.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,120 +1,93 @@
 from bs4 import BeautifulSoup
-from dateutil.relativedelta import relativedelta
-
+from selenium import webdriver
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support.ui import Select
+from selenium.webdriver.support.wait import WebDriverWait
+from selenium.webdriver.support import expected_conditions as EC
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
-
-
-def get_token(page) -> str:
-    """
-    Get a __token to include in the form data
-        :param page: Page html
-        :return: Form __token
-    """
-    soup = BeautifulSoup(page.text, features="html.parser")
-    soup.prettify()
-    token = soup.find("input", {"name": "__token"}).get("value")
-    return token
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
+# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
-    def get_data(self, url) -> str:
-        """This method makes the request to the council
-
-        Keyword arguments:
-        url -- the url to get the data from
-        """
-        # Set a user agent so we look like a browser ;-)
-        user_agent = (
-            "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) "
-            "Chrome/108.0.0.0 Safari/537.36"
-        )
-        headers = {"User-Agent": user_agent}
-        requests.packages.urllib3.disable_warnings()
-
-        # Make the Request - change the URL - find out your property number
-        try:
-            session = requests.Session()
-            session.headers.update(headers)
-            full_page = session.get(url)
-            return full_page
-        except requests.exceptions.HTTPError as errh:
-            _LOGGER.error(f"Http Error: {errh}")
-            raise
-        except requests.exceptions.ConnectionError as errc:
-            _LOGGER.error(f"Error Connecting: {errc}")
-            raise
-        except requests.exceptions.Timeout as errt:
-            _LOGGER.error(f"Timeout Error: {errt}")
-            raise
-        except requests.exceptions.RequestException as err:
-            _LOGGER.error(f"Oops: Something Else {err}")
-            raise
-
     def parse_data(self, page: str, **kwargs) -> dict:
-        uprn = kwargs.get("uprn")
-        postcode = kwargs.get("postcode")
-        check_uprn(uprn)
-        check_postcode(postcode)
-
-        values = {
-            "__token": get_token(page),
-            "page": "491",
-            "locale": "en_GB",
-            "q1f8ccce1d1e2f58649b4069712be6879a839233f_0_0": postcode,
-            "q1f8ccce1d1e2f58649b4069712be6879a839233f_1_0": uprn,
-            "next": "Next",
-        }
-        headers = {"User-Agent": "Mozilla/5.0 (Windows NT 6.1; Win64; x64)"}
-        requests.packages.urllib3.disable_warnings()
-        response = requests.request(
-            "POST",
-            "https://www.birmingham.gov.uk/xfp/form/619",
-            headers=headers,
-            data=values,
-        )
+        page = "https://selfservice.broxtowe.gov.uk/renderform.aspx?t=217&k=9D2EF214E144EE796430597FB475C3892C43C528"
 
-        soup = BeautifulSoup(response.text, features="html.parser")
+        data = {"bins": []}
 
-        rows = soup.find("table").find_all("tr")
+        user_uprn = kwargs.get("uprn")
+        user_postcode = kwargs.get("postcode")
+        check_uprn(user_uprn)
+        check_postcode(user_postcode)
+
+        # Set up Selenium to run 'headless'
+        options = webdriver.ChromeOptions()
+        options.add_argument("--headless")
+        options.add_argument("--no-sandbox")
+        options.add_argument("--disable-gpu")
+        options.add_argument("--disable-dev-shm-usage")
+        options.add_experimental_option("excludeSwitches", ["enable-logging"])
+
+        # Create Selenium webdriver
+        driver = webdriver.Chrome(options=options)
+        driver.get(page)
+
+        # Populate postcode field
+        inputElement_postcode = driver.find_element(
+            By.ID,
+            "ctl00_ContentPlaceHolder1_FF5683TB",
+        )
+        inputElement_postcode.send_keys(user_postcode)
 
-        # Form a JSON wrapper
-        data = {"bins": []}
+        # Click search button
+        driver.find_element(
+            By.ID,
+            "ctl00_ContentPlaceHolder1_FF5683BTN",
+        ).click()
+
+        # Wait for the 'Select address' dropdown to appear and select option matching UPRN
+        dropdown = WebDriverWait(driver, 10).until(
+            EC.presence_of_element_located((By.ID, "ctl00_ContentPlaceHolder1_FF5683DDL"))
+        )
+        # Create a 'Select' for it, then select the matching URPN option
+        dropdownSelect = Select(dropdown)
+        dropdownSelect.select_by_value("U" + user_uprn)
+
+        # Wait for the submit button to appear, then click it to get the collection dates
+        submit = WebDriverWait(driver, 10).until(
+            EC.presence_of_element_located((By.ID, "ctl00_ContentPlaceHolder1_btnSubmit"))
+        )
+        submit.click()
 
-        # Loops the Rows
-        for row in rows:
-            cells = row.find_all("td")
-            if cells:
-                bin_type = cells[0].get_text(strip=True)
-                collection_next = cells[1].get_text(strip=True)
-
-                collection_date = re.findall("\(.*?\)", collection_next)
-
-                if len(collection_date) != 1:
-                    continue
-
-                collection_date_obj = parse(
-                    re.sub("[()]", "", collection_date[0])
-                ).date()
-
-                # since we only have the next collection day, if the parsed date is in the past,
-                # assume the day is instead next month
-                if collection_date_obj < datetime.now().date():
-                    collection_date_obj += relativedelta(months=1)
-
-                # Make each Bin element in the JSON
-                dict_data = {
-                    "type": bin_type,
-                    "collectionDate": collection_date_obj.strftime(date_format),
-                }
+        soup = BeautifulSoup(driver.page_source, features="html.parser")
 
-                # Add data to the main JSON Wrapper
-                data["bins"].append(dict_data)
+        bins_div = soup.find("div", id="ctl00_ContentPlaceHolder1_FF5686FormGroup")
+        if bins_div:
+            bins_table = bins_div.find("table")
+            if bins_table:
+                # Get table rows
+                for row in bins_table.find_all("tr"):
+                    # Get the rows cells
+                    cells = row.find_all("td")
+                    bin_type = cells[0].get_text(strip=True)
+                    # Skip header row
+                    if bin_type and cells[3] and bin_type != "Bin Type":
+                        collection_date = datetime.strptime(cells[3].get_text(strip=True), "%A, %d %B %Y")
+                        dict_data = {
+                            "type": bin_type,
+                            "collectionDate": collection_date.strftime(date_format),
+                        }
+                        data["bins"].append(dict_data)
+
+                        data["bins"].sort(
+                            key=lambda x: datetime.strptime(x.get("collectionDate"), "%d/%m/%Y")
+                        )
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BlackburnCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/EastNorthamptonshireCouncil.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,107 +1,118 @@
-import json
-import logging
-import ssl
-from collections import OrderedDict
-from datetime import datetime
-
-import requests
-import urllib3
-from bs4 import BeautifulSoup
+import hashlib
+import math
+import time
+from datetime import timedelta
 
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
-class CustomHttpAdapter(requests.adapters.HTTPAdapter):
-    """Transport adapter" that allows us to use custom ssl_context."""
+def ct(e: str) -> int:
+    """
+    Mimic ct() function in main.cbc0dd8a.js
+        :rtype: int
+        :param e: Day name
+        :return: Day index
+    """
+    if e == "MON":
+        return 0
+    elif e == "TUE":
+        return 1
+    elif e == "WED":
+        return 2
+    elif e == "THU":
+        return 3
+    elif e == "FRI":
+        return 4
+    return -1
+
+
+def ft() -> dict:
+    """
+    Mimic ft() function in main.cbc0dd8a.js
+        :rtype: dict
+        :return: Weeks and days
+    """
+    e = datetime.now()
+    t = datetime(2022, 4, 20)
+    return {
+        "weeks": math.floor(((e - t).total_seconds() * 10) / 1e3 / 86400 / 7 % 2),
+        "days": math.floor(((e - t).total_seconds() * 10) / 1e3 / 86400 % 7),
+    }
 
-    def __init__(self, ssl_context=None, **kwargs):
-        self.ssl_context = ssl_context
-        super().__init__(**kwargs)
-
-    def init_poolmanager(self, connections, maxsize, block=False):
-        self.poolmanager = urllib3.poolmanager.PoolManager(
-            num_pools=connections,
-            maxsize=maxsize,
-            block=block,
-            ssl_context=self.ssl_context,
-        )
+
+def st(e: int, t: int, n: str) -> str:
+    """
+    Mimic st() function in main.cbc0dd8a.js
+        :rtype: str
+        :return: Date
+    """
+    d = datetime.now() + timedelta(days=(7 * t + (e - n)))
+    return d.strftime(date_format)
 
 
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        # Make a BS4 object
-
-        driver = None
-        try:
-            data = {"bins": []}
-            uprn = kwargs.get("uprn")
-            web_driver = kwargs.get("web_driver")
-            headless = kwargs.get("headless")
-            current_month = datetime.today().strftime("%m")
-            current_year = datetime.today().strftime("%Y")
-            url = (
-                f"https://mybins.blackburn.gov.uk/api/mybins/getbincollectiondays?uprn={uprn}&month={current_month}"
-                f"&year={current_year}"
+        data = {"bins": []}
+        uprn = kwargs.get("uprn")
+        check_uprn(uprn)
+
+        headers = {
+            "User-Agent": "Mozilla/5.0 (Windows NT 6.1; Win64; x64)",
+            "origin": "https://kbccollectiveapi-coll-api.e4ff.pro-eu-west-1.openshiftapps.com",
+            "referer": "https://kbccollectiveapi-coll-api.e4ff.pro-eu-west-1.openshiftapps.com/",
+        }
+        requests.packages.urllib3.disable_warnings()
+        # Check council website workings haven't changed
+        response = requests.get(
+            f"https://kbccollectiveapi-coll-api.e4ff.pro-eu-west-1.openshiftapps.com/wc-info/static/js/main.cbc0dd8a.js",
+            headers=headers,
+        )
+        if (
+                response.status_code != 200
+                or hashlib.sha256(response.text.encode("utf-8")).hexdigest()
+                != "2f357c24b043c31c0157c234323c401238842c1d00f00f16c7ca3e569a0ab3cd"
+        ):
+            raise ValueError(
+                "Council website has changed, parser needs updating. Please open issue on GitHub."
             )
-            driver = create_webdriver(web_driver, headless, None, __name__)
-            driver.get(url)
-
-            soup = BeautifulSoup(driver.page_source, "html.parser")
+        # Get variables for workings
+        response = requests.get(
+            f"https://api.northnorthants.gov.uk/test/wc-info/{uprn}?r={time.time() * 1000}",
+            headers=headers,
+        )
+        if response.status_code != 200:
+            raise ValueError("No bin data found for provided UPRN.")
 
-            # Find the <pre> tag that contains the JSON data
-            pre_tag = soup.find("pre")
+        json_response = json.loads(response.text)
+        sov = json_response["sov"]
+        day = json_response["day"]
+        schedule = json_response["schedule"]
+        # Mimic workings in main.cbc0dd8a.js
+        if sov == "ENC" or sov == "BCW":
+            n = ft()
+            r = 1
+            if ct(day) > n["days"]:
+                r = 0
+            for o in range(0, 10):
+                week = (n["weeks"] + o + r) % 2
+                if (week == 0 and "B" == schedule) or (week != 0 and "B" != schedule):
+                    bin_type = "General"
+                else:
+                    bin_type = "Recycling"
+                collection_data = {
+                    "type": bin_type,
+                    "collectionDate": st(ct(day), o + r, n["days"]).replace(
+                        ",", ""
+                    ),
+                }
+                data["bins"].append(collection_data)
 
-            if pre_tag:
-                # Extract the text content within the <pre> tag
-
-                # Return JSON from response and loop through collections
-                json_result = json.loads(pre_tag.contents[0])
-                bin_collections = json_result["BinCollectionDays"]
-                for collection in bin_collections:
-                    if collection is not None:
-                        bin_type = collection[0].get("BinType")
-                        current_collection_date = datetime.strptime(
-                            collection[0].get("CollectionDate"), "%Y-%m-%d"
-                        )
-                        next_collection_date = datetime.strptime(
-                            collection[0].get("NextScheduledCollectionDate"), "%Y-%m-%d"
-                        )
-
-                        # Work out the most recent collection date to display
-                        if (
-                            datetime.today().date()
-                            <= current_collection_date.date()
-                            < next_collection_date.date()
-                        ):
-                            collection_date = current_collection_date
-                        else:
-                            collection_date = next_collection_date
-
-                        dict_data = {
-                            "type": bin_type,
-                            "collectionDate": collection_date.strftime(date_format),
-                        }
-                        data["bins"].append(dict_data)
-
-                        data["bins"].sort(
-                            key=lambda x: datetime.strptime(
-                                x.get("collectionDate"), date_format
-                            )
-                        )
-        except Exception as e:
-            # Here you can log the exception if needed
-            print(f"An error occurred: {e}")
-            # Optionally, re-raise the exception if you want it to propagate
-            raise
-        finally:
-            # This block ensures that the driver is closed regardless of an exception
-            if driver:
-                driver.quit()
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BoltonCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/LeedsCityCouncil.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,105 +1,94 @@
-import time
 from datetime import datetime
-
-from bs4 import BeautifulSoup
-from selenium.webdriver.common.by import By
-from selenium.webdriver.common.keys import Keys
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import Select
-from selenium.webdriver.support.wait import WebDriverWait
-
 from uk_bin_collection.uk_bin_collection.common import *
 from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
 
+import pandas as pd
+import urllib.request
+
 
 class CouncilClass(AbstractGetBinDataClass):
     """
-    Concrete classes have to implement all abstract operations of the
-    base class. They can also override some operations with a default
+    Concrete classes have to implement all abstract operations of the base
+    class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        driver = None
-        try:
-            user_uprn = kwargs.get("uprn")
-            check_uprn(user_uprn)
-
-            user_postcode = kwargs.get("postcode")
-            check_postcode(user_postcode)
-            web_driver = kwargs.get("web_driver")
-            headless = kwargs.get("headless")
-
-            data = {"bins": []}
-
-            # Get our initial session running
-            page = "https://carehomes.bolton.gov.uk/bins.aspx"
-
-            driver = create_webdriver(web_driver, headless, None, __name__)
-            driver.get(page)
-
-            # If you bang in the house number (or property name) and postcode in the box it should find your property
-            wait = WebDriverWait(driver, 30)
-
-            pc_search_box = wait.until(
-                EC.presence_of_element_located((By.ID, "txtPostcode"))
+        """
+        Parse council provided CSVs to get the latest bin collections for address
+        """
+        # URLs to data sources
+        address_csv_url = "https://opendata.leeds.gov.uk/downloads/bins/dm_premises.csv"
+        collections_csv_url = "https://opendata.leeds.gov.uk/downloads/bins/dm_jobs.csv"
+
+        user_postcode = kwargs.get("postcode")
+        user_paon = kwargs.get("paon")
+
+        check_postcode(user_postcode)
+        check_paon(user_paon)
+
+        data = {"bins": []}  # dictionary for data
+        prop_id = 0  # LCC use city wide URPNs in this dataset
+        result_row = None  # store the property as a row
+
+        # Get address csv and give it headers (pandas bypasses downloading the file)
+        # print("Getting address data...")
+        with urllib.request.urlopen(address_csv_url) as response:
+            addr = pd.read_csv(
+                response,
+                names=[
+                    "PropertyId",
+                    "PropertyName",
+                    "PropertyNo",
+                    "Street",
+                    "Town",
+                    "City",
+                    "Postcode",
+                ],
+                sep=",",
             )
 
-            pc_search_box.send_keys(user_postcode)
-
-            pcsearch_btn = wait.until(EC.element_to_be_clickable((By.ID, "btnSubmit")))
-
-            pcsearch_btn.click()
-
-            # Wait for the 'Select your property' dropdown to appear and select the first result
-            dropdown = wait.until(EC.element_to_be_clickable((By.ID, "ddlAddresses")))
-
-            dropdown_options = wait.until(
-                EC.presence_of_element_located((By.XPATH, "//select/option[1]"))
-            )
-            time.sleep(1)
-            # Create a 'Select' for it, then select the first address in the list
-            # (Index 0 is "Make a selection from the list")
-            dropdownSelect = Select(dropdown)
-            dropdownSelect.select_by_value(str(user_uprn))
-            dropdown_options = wait.until(
-                EC.presence_of_element_located((By.ID, "pnlStep3"))
+        # Get collections csv and give it headers
+        # print("Getting collection data...")
+        with urllib.request.urlopen(collections_csv_url) as response:
+            coll = pd.read_csv(
+                response, names=["PropertyId", "BinType", "CollectionDate"], sep=","
             )
 
-            soup = BeautifulSoup(driver.page_source, features="html.parser")
-            soup.prettify()
-
-            collections = []
-
-            # Find section with bins in
-            sections = soup.find_all("div", {"class": "bin-info"})
+        # Find the property id from the address data
+        # ("Finding property reference...")
+        for row in addr.itertuples():
+            if (
+                    str(row.Postcode).replace(" ", "").lower()
+                    == user_postcode.replace(" ", "").lower()
+            ):
+                if row.PropertyNo == user_paon:
+                    prop_id = row.PropertyId
+                    # print(f"Reference: {str(prop_id)}")
+                    continue
+
+        # For every match on the property id in the collections data, add the bin type and date to list
+        # Note: time is 7am as that's when LCC ask bins to be out by
+        job_list = []
+        # print(f"Finding collections for property reference: {user_paon} {result_row.Street} "
+        #      f"{result_row.Postcode}...")
+        for row in coll.itertuples():
+            if row.PropertyId == prop_id:
+                job_list.append([row.BinType, datetime.strptime(row.CollectionDate, "%d/%m/%y").strftime(date_format)])
+
+        # If jobs exist, sort list by date order. Load list into dictionary to return
+        # print("Processing collections...")
+        if len(job_list) > 0:
+            job_list.sort(key=lambda x: datetime.strptime(x[1], date_format))
+            for i in range(len(job_list)):
+                job_date = datetime.strptime(job_list[i][1], date_format)
+                if datetime.now() < job_date:
+                    dict_data = {
+                        "type": job_list[i][0],
+                        "collectionDate": job_list[i][1],
+                    }
+                    data["bins"].append(dict_data)
+        else:
+            print("No bin collections found for property!")
 
-            # For each bin section, get the text and the list elements
-            for item in sections:
-                words = item.find_next("strong").text.split()[2:4]
-                bin_type = " ".join(words).capitalize()
-                date_list = item.find_all("p")
-                for d in date_list:
-                    next_collection = datetime.strptime(d.text.strip(), "%A %d %B %Y")
-                    collections.append((bin_type, next_collection))
-
-            # Sort the text and list elements by date
-            ordered_data = sorted(collections, key=lambda x: x[1])
-
-            # Put the elements into the dictionary
-            for item in ordered_data:
-                dict_data = {
-                    "type": item[0],
-                    "collectionDate": item[1].strftime(date_format),
-                }
-                data["bins"].append(dict_data)
-        except Exception as e:
-            # Here you can log the exception if needed
-            print(f"An error occurred: {e}")
-            # Optionally, re-raise the exception if you want it to propagate
-            raise
-        finally:
-            # This block ensures that the driver is closed regardless of an exception
-            if driver:
-                driver.quit()
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BracknellForestCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/CroydonCouncil.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 
 from bs4 import BeautifulSoup
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 def get_headers(base_url: str, method: str) -> dict[str, str]:
     """
     Gets request headers
         :rtype: dict[str, str]
         :param base_url: Base URL to use
@@ -15,15 +15,15 @@
         :return: Request headers
     """
     headers = {
         "Accept-Encoding": "gzip, deflate, br",
         "Accept-Language": "en-GB,en-US;q=0.9,en;q=0.8",
         "Cache-Control": "max-age=0",
         "Connection": "keep-alive",
-        "Host": "selfservice.mybfc.bracknell-forest.gov.uk",
+        "Host": "service.croydon.gov.uk",
         "Origin": base_url,
         "sec-ch-ua": '"Not_A Brand";v="99", "Google Chrome";v="109", "Chromium";v="109"',
         "sec-ch-ua-mobile": "?0",
         "sec-ch-ua-platform": "Windows",
         "Sec-Fetch-Dest": "document",
         "Sec-Fetch-User": "?1",
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko)"
@@ -50,31 +50,43 @@
     """
     Gets session storage global object
         :rtype: object
         :return: Session storage global object
     """
     return {
         "destination_stack": [
-            "w/webpage/waste-collection-days",
+            "w/webpage/bin-day-enter-address",
+            "w/webpage/your-bin-collection-details?context_record_id=86086077"
+            "&webpage_token=5c047b2c10b4aad66bef2054aac6bea52ad7a5e185ffdf7090b01f8ddc96728f",
+            "w/webpage/bin-day-enter-address",
+            "w/webpage/your-bin-collection-details?context_record_id=86085229"
+            "&webpage_token=cf1b8fd6213f4823277d98c1dd8a992e6ebef1fabc7d892714e5d9dade448c37",
+            "w/webpage/bin-day-enter-address",
+            "w/webpage/your-bin-collection-details?context_record_id=86084221"
+            "&webpage_token=7f52fb51019bf0e6bfe9647b1b31000124bd92a9d95781f1557f58b3ed40da52",
+            "w/webpage/bin-day-enter-address",
+            "w/webpage/your-bin-collection-details?context_record_id=86083209"
+            "&webpage_token=de50c265da927336f526d9d9a44947595c3aa38965aa8c495ac2fb73d272ece8",
+            "w/webpage/bin-day-enter-address",
         ],
         "last_context_record_id": "86086077",
     }
 
 
 def get_csrf_token(s: requests.session, base_url: str) -> str:
     """
     Gets a CSRF token
         :rtype: str
-        :param s: requests.Session() to use
+        :param s: requests.session() to use
         :param base_url: Base URL to use
         :return: CSRF token
     """
     csrf_token = ""
     response = s.get(
-        base_url + "/w/webpage/waste-collection-days",
+        base_url + "/wasteservices/w/webpage/bin-day-enter-address",
         headers=get_headers(base_url, "GET"),
     )
     if response.status_code == 200:
         soup = BeautifulSoup(response.text, features="html.parser")
         soup.prettify()
         app_body = soup.find("div", {"class": "app-body"})
         script = app_body.find("script", {"type": "text/javascript"}).string
@@ -91,58 +103,62 @@
 
 def get_address_id(
     s: requests.session, base_url: str, csrf_token: str, postcode: str, paon: str
 ) -> str:
     """
     Gets the address ID
         :rtype: str
-        :param s: requests.Session() to use
+        :param s: requests.session() to use
         :param base_url: Base URL to use
         :param csrf_token: CSRF token to use
         :param postcode: Postcode to use
         :param paon: House number/address to find
         :return: address ID
     """
     address_id = "0"
     # Get the addresses for the postcode
     form_data = {
-        "code_action": "find_addresses",
-        "code_params": '{"search":"' + postcode + '"}',
+        "code_action": "search",
+        "code_params": '{"search_item":"' + postcode + '","is_ss":true}',
+        "fragment_action": "handle_event",
+        "fragment_id": "PCF0020408EECEC1",
+        "fragment_collection_class": "formtable",
+        "fragment_collection_editable_values": '{"PCF0021449EECEC1":"1"}',
         "_session_storage": json.dumps(
             {
-                "/w/webpage/waste-collection-days": {},
+                "/wasteservices/w/webpage/bin-day-enter-address": {},
                 "_global": get_session_storage_global(),
             }
         ),
-        "action_cell_id": "PCL0003988FEFFB1",
-        "action_page_id": "PAG0000570FEFFB1",
+        "action_cell_id": "PCL0005629EECEC1",
+        "action_page_id": "PAG0000898EECEC1",
         "form_check_ajax": csrf_token,
     }
     response = s.post(
         base_url
-        + "/w/webpage/waste-collection-days?webpage_subpage_id=PAG0000570FEFFB1"
-        "&webpage_token=390170046582b0e3d7ca68ef1d6b4829ccff0b1ae9c531047219c6f9b5295738"
-        "&widget_action=handle_event",
+        + "/wasteservices/w/webpage/bin-day-enter-address?webpage_subpage_id=PAG0000898EECEC1"
+        "&webpage_token=faab02e1f62a58f7bad4c2ae5b8622e19846b97dde2a76f546c4bb1230cee044"
+        "&widget_action=fragment_action",
         headers=get_headers(base_url, "POST"),
         data=form_data,
     )
     if response.status_code == 200:
         json_response = json.loads(response.text)
-        addresses = json_response["response"]["addresses"]["items"]
+        addresses = json_response["response"]["items"]
         # Find the matching address id for the paon
         for address in addresses:
             # Check for full matches first
-            if address.get("Description") == paon:
-                address_id = address.get("Id")
+            if address.get("dropdown_display_field") == paon:
+                address_id = address.get("id")
                 break
         # Check for matching start if no full match found
         if address_id == "0":
             for address in addresses:
-                if address.get("Description").split()[0] == paon.strip():
-                    address_id = address.get("Id")
+                if address.get("dropdown_display_field").split()[0] == paon.strip():
+                    address_id = address.get("id")
                     break
         # Check match was found
         if address_id == "0":
             raise ValueError(
                 "Code 2: No matching address for house number/full address found."
             )
     else:
@@ -152,95 +168,125 @@
 
 def get_collection_data(
     s: requests.session, base_url: str, csrf_token: str, address_id: str
 ) -> str:
     """
     Gets the collection data
         :rtype: str
-        :param s: requests.Session() to use
+        :param s: requests.session() to use
         :param base_url: Base URL to use
         :param csrf_token: CSRF token to use
         :param address_id: Address id to use
         :param retries: Retries count
         :return: Collection data
     """
     collection_data = ""
     if address_id != "0":
         form_data = {
-            "code_action": "find_rounds",
-            "code_params": '{"addressId":"' + address_id + '"}',
-            "_session_storage": json.dumps(
-                {
-                    "/w/webpage/waste-collection-days": {},
-                    "_global": get_session_storage_global(),
-                }
-            ),
-            "action_cell_id": "PCL0003988FEFFB1",
-            "action_page_id": "PAG0000570FEFFB1",
+            "form_check": csrf_token,
+            "submitted_page_id": "PAG0000898EECEC1",
+            "submitted_widget_group_id": "PWG0002644EECEC1",
+            "submitted_widget_group_type": "modify",
+            "submission_token": "63e9126bacd815.12997577",
+            "payload[PAG0000898EECEC1][PWG0002644EECEC1][PCL0005629EECEC1][formtable]"
+            "[C_63e9126bacfb3][PCF0020408EECEC1]": address_id,
+            "payload[PAG0000898EECEC1][PWG0002644EECEC1][PCL0005629EECEC1][formtable]"
+            "[C_63e9126bacfb3][PCF0021449EECEC1]": "1",
+            "payload[PAG0000898EECEC1][PWG0002644EECEC1][PCL0005629EECEC1][formtable]"
+            "[C_63e9126bacfb3][PCF0020072EECEC1]": "Next",
+            "submit_fragment_id": "PCF0020072EECEC1",
+            "_session_storage": json.dumps({"_global": get_session_storage_global()}),
+            "_update_page_content_request": 1,
             "form_check_ajax": csrf_token,
         }
         response = s.post(
             base_url
-            + "/w/webpage/waste-collection-days?webpage_subpage_id=PAG0000570FEFFB1"
-            "&webpage_token=390170046582b0e3d7ca68ef1d6b4829ccff0b1ae9c531047219c6f9b5295738"
-            "&widget_action=handle_event",
+            + "/wasteservices/w/webpage/bin-day-enter-address?webpage_subpage_id=PAG0000898EECEC1"
+            "&webpage_token=faab02e1f62a58f7bad4c2ae5b8622e19846b97dde2a76f546c4bb1230cee044",
             headers=get_headers(base_url, "POST"),
             data=form_data,
         )
         if response.status_code == 200 and len(response.text) > 0:
             json_response = json.loads(response.text)
-            collection_data = json_response["response"]["collections"]
+            form_data = {
+                "_dummy": 1,
+                "_session_storage": json.dumps(
+                    {"_global": get_session_storage_global()}
+                ),
+                "_update_page_content_request": 1,
+                "form_check_ajax": csrf_token,
+            }
+            response = s.post(
+                base_url + json_response["redirect_url"],
+                headers=get_headers(base_url, "POST"),
+                data=form_data,
+            )
+            if response.status_code == 200 and len(response.text) > 0:
+                json_response = json.loads(response.text)
+                collection_data = json_response["data"]
+            else:
+                raise ValueError("Code 4: Failed to get bin data.")
         else:
-            raise ValueError("Code 4: Failed to get bin data.")
+            raise ValueError(
+                "Code 5: Failed to get bin data. Too many requests. Please wait a few minutes before trying again."
+            )
     return collection_data
 
 
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
         requests.packages.urllib3.disable_warnings()
-        s = requests.Session()
-        base_url = "https://selfservice.mybfc.bracknell-forest.gov.uk"
+        s = requests.session()
+        base_url = "https://service.croydon.gov.uk"
         paon = kwargs.get("paon")
         postcode = kwargs.get("postcode")
         check_paon(paon)
         check_postcode(postcode)
 
         # Firstly, get a CSRF (cross-site request forgery) token
         csrf_token = get_csrf_token(s, base_url)
         # Next, get the address_id
         address_id = get_address_id(s, base_url, csrf_token, postcode, paon)
         # Finally, use the address_id to get the collection data
         collection_data = get_collection_data(s, base_url, csrf_token, address_id)
         if collection_data != "":
+            soup = BeautifulSoup(collection_data, features="html.parser")
+            soup.prettify()
+
+            # Find the list elements
+            collection_record_elements = soup.find_all(
+                "div", {"class": "listing_template_record"}
+            )
+
             # Form a JSON wrapper
             data = {"bins": []}
 
-            for c in collection_data:
-                collection_type = c["round"]
-                for c_date in c["upcomingCollections"]:
-                    collection_date = (
-                        re.search(r"Your (.*) is(.*)", c_date).group(2).strip()
-                    )
-                    dict_data = {
-                        "type": collection_type,
-                        "collectionDate": datetime.strptime(
-                            collection_date, "%A %d %B %Y"
-                        ).strftime(date_format),
-                    }
-                    data["bins"].append(dict_data)
+            for e in collection_record_elements:
+                collection_type = e.find_all(
+                    "div", {"class": "fragment_presenter_template_show"}
+                )[0].text.strip()
+                collection_date = (
+                    e.find("div", {"class": "bin-collection-next"})
+                    .attrs["data-current_value"]
+                    .strip()
+                )
+                dict_data = {
+                    "type": collection_type,
+                    "collectionDate": datetime.strptime(
+                        collection_date, "%d/%m/%Y %H:%M"
+                    ).strftime(date_format),
+                }
+                data["bins"].append(dict_data)
 
             if len(data["bins"]) == 0:
                 raise ValueError(
                     "Code 5: No bin data found. Please ensure the council website is showing data first,"
                     " then open an issue on GitHub."
                 )
 
-            data["bins"].sort(
-                key=lambda x: datetime.strptime(x.get("collectionDate"), date_format)
-            )
             return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BradfordMDC.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/WaverleyBoroughCouncil.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,103 +1,120 @@
+from datetime import date, datetime
+
 import requests
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        user_uprn = kwargs.get("uprn")
-        check_uprn(user_uprn)
-
-        # UPRN is passed in via a cookie. Set cookies/params and GET the page
-        cookies = {
-            "COLLECTIONDATES": f"{user_uprn}",
-        }
-        headers = {
-            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8",
-            "Accept-Language": "en-GB,en;q=0.7",
+        # pindex isn't actually paon, it's a url parameter that I'm guessing the council use as a property id
+        data = {"bins": []}
+        pindex = kwargs.get("paon")
+        user_postcode = kwargs.get("postcode")
+        check_postcode(user_postcode)
+
+        # WBC use a url parameter called "Track" that's generated when you start a form session.
+        # So first off, open the page, find the page link and copy it with the Track
+        start_url = "https://wav-wrp.whitespacews.com/"
+        s = requests.session()
+        response = s.get(start_url)
+        soup = BeautifulSoup(response.content, features="html.parser")
+        soup.prettify()
+        collection_page_link = soup.find_all(
+            "p", {"class": "govuk-body govuk-!-margin-bottom-0 colorblue lineheight15"}
+        )[0].find("a")["href"]
+        track_id = collection_page_link[33:60]
+
+        # Next we need to search using the postcode, but this is actually an important POST request
+        pc_headers = {
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,"
+            "image/webp,image/apng,*/*;q=0.8",
+            "Accept-Language": "en-GB,en;q=0.9",
             "Cache-Control": "max-age=0",
             "Connection": "keep-alive",
-            "Referer": "https://onlineforms.bradford.gov.uk/ufs/collectiondates.eb",
+            "Origin": "https://wav-wrp.whitespacews.com",
+            "Referer": "https://wav-wrp.whitespacews.com/"
+            + track_id
+            + "&serviceID=A&seq=2",
             "Sec-Fetch-Dest": "document",
             "Sec-Fetch-Mode": "navigate",
             "Sec-Fetch-Site": "same-origin",
             "Sec-Fetch-User": "?1",
             "Sec-GPC": "1",
             "Upgrade-Insecure-Requests": "1",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/107.0.0.0 Safari/537.36",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, "
+            "like Gecko) Chrome/106.0.0.0 Safari/537.36",
         }
-        params = {
-            "ebp": "30",
-            "ebd": "0",
-            "ebz": "1_1713270660323",
+        form_data = {
+            "address_name_number": "",
+            "address_street": "",
+            "street_town": "",
+            "address_postcode": user_postcode,
         }
-        requests.packages.urllib3.disable_warnings()
-        response = requests.get(
-            "https://onlineforms.bradford.gov.uk/ufs/collectiondates.eb",
-            params=params,
-            headers=headers,
-            cookies=cookies,
+        response = s.post(
+            "https://wav-wrp.whitespacews.com/mop.php?serviceID=A&"
+            + track_id
+            + "&seq=2",
+            headers=pc_headers,
+            data=form_data,
         )
 
-        # Parse response text for super speedy finding
-        soup = BeautifulSoup(response.text, features="html.parser")
-        soup.prettify()
-
-        data = {"bins": []}
-
-        # BradfordMDC site has lots of embedded tables, find the table titled 'Your next general/recycling collections are:'
-        for bin in soup.find_all(attrs={"class": "CTID-FHGh1Q77-_"}):
-            if bin.find_all(attrs={"class": "CTID-62bNngCB-_"}):
-                bin_type = "General Waste"
-                bin_colour = "Green"
-                bin_date_text = bin.find(attrs={"class": "CTID-62bNngCB-_"}).get_text()
-            elif bin.find_all(attrs={"class": "CTID-LHo9iO0y-_"}):
-                bin_type = "Recycling Waste"
-                bin_colour = "Grey"
-                bin_date_text = bin.find(attrs={"class": "CTID-LHo9iO0y-_"}).get_text()
-            else:
-                raise ValueError(f"No bin info found in {bin_type_info[0]}")
-
-            # Collection Date info is alongside the bin type, we got the whole line in the if/elif above
-            # below strips the text off at the beginning, to get a date, though recycling is a character shorter hence the lstrip
-            bin_date_info = bin_date_text[29:50].lstrip(" ")
-
-            if contains_date(bin_date_info):
-                bin_date = get_next_occurrence_from_day_month(
-                    datetime.strptime(
-                        bin_date_info,  # + " " + datetime.today().strftime("%Y"),
-                        "%a %b %d %Y",
-                    )
-                ).strftime(date_format)
-                # print(bin_date_info)
-                # print(bin_date)
-            # On exceptional collection schedule (e.g. around English Bank Holidays), date will be contained in the second stripped string
-            else:
-                bin_date = get_next_occurrence_from_day_month(
-                    datetime.strptime(
-                        bin_date_info[1] + " " + datetime.today().strftime("%Y"),
-                        "%a %b %d %Y",
-                    )
-                ).strftime(date_format)
-
-        # Build data dict for each entry
-        dict_data = {
-            "type": bin_type,
-            "collectionDate": bin_date,
-            "colour": bin_colour,
+        # Finally, we can use pindex to find the address and get some data
+        request_url = (
+            "https://wav-wrp.whitespacews.com/mop.php?"
+            + track_id
+            + "&serviceID=A&seq=3&pIndex="
+            + pindex
+        )
+        headers = {
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,"
+            "image/webp,image/apng,*/*;q=0.8",
+            "Accept-Language": "en-GB,en;q=0.9",
+            "Connection": "keep-alive",
+            "Referer": "https://wav-wrp.whitespacews.com/mop.php?serviceID=A&"
+            + track_id
+            + "&seq=2",
+            "Sec-Fetch-Dest": "document",
+            "Sec-Fetch-Mode": "navigate",
+            "Sec-Fetch-Site": "same-origin",
+            "Sec-Fetch-User": "?1",
+            "Sec-GPC": "1",
+            "Upgrade-Insecure-Requests": "1",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, "
+            "like Gecko) Chrome/106.0.0.0 Safari/537.36",
         }
-        data["bins"].append(dict_data)
 
-        data["bins"].sort(
-            key=lambda x: datetime.strptime(x.get("collectionDate"), date_format)
+        response = s.get(request_url, headers=headers)
+        soup = BeautifulSoup(response.content, features="html.parser")
+        soup.prettify()
+
+        # Find the list elements
+        u1_block = soup.find_all(
+            "u1",
+            {
+                "class": "displayinlineblock justifycontentleft alignitemscenter margin0 padding0"
+            },
         )
 
+        for element in u1_block:
+            x = element.find_all_next(
+                "li", {"class": "displayinlineblock padding0px20px5px0px"}
+            )
+            dict_data = {
+                "type": x[2].text.strip(),
+                "collectionDate": datetime.strptime(
+                    x[1].text.strip(), date_format
+                ).strftime(date_format),
+            }
+            data["bins"].append(dict_data)
+
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BristolCityCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/BristolCityCouncil.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ast
 
 import requests
 from bs4 import BeautifulSoup
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
@@ -16,15 +16,15 @@
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
         user_uprn = kwargs.get("uprn")
         check_uprn(user_uprn)
 
         requests.packages.urllib3.disable_warnings()
-        s = requests.Session()
+        s = requests.session()
 
         service_type_headers = {
             "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,"
             "image/webp,image/apng,*/*;q=0.8",
             "Accept-Language": "en-GB,en;q=0.9",
             "Cache-Control": "max-age=0",
             "Connection": "keep-alive",
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BromleyBoroughCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/HighPeakCouncil.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,115 +1,128 @@
-# This script pulls (in one hit) the data from Bromley Council Bins Data
-import datetime
 import time
-from datetime import datetime
 
 from bs4 import BeautifulSoup
-from dateutil.relativedelta import relativedelta
+from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.support.wait import WebDriverWait
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
-# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
-    def parse_data(self, page: str, **kwargs) -> dict:
+    def get_data(self, page) -> dict:
         # Make a BS4 object
-        driver = None
-        try:
-            bin_data_dict = {"bins": []}
-            collections = []
-            web_driver = kwargs.get("web_driver")
-            headless = kwargs.get("headless")
-
-            data = {"bins": []}
-
-            # Get our initial session running
-            driver = create_webdriver(web_driver, headless, None, __name__)
-            driver.get(kwargs.get("url"))
-
-            wait = WebDriverWait(driver, 30)
-            results = wait.until(
-                EC.presence_of_element_located((By.CLASS_NAME, "waste-service-image"))
+        soup = BeautifulSoup(page, features="html.parser")
+        soup.prettify()
+
+        data = {"bins": []}
+
+        for month in soup.select('div[class*="bin-collection__month"]'):
+            monthName = month.select('h3[class*="bin-collection__title"]')[
+                0
+            ].text.strip()
+            for collectionDay in month.select('li[class*="bin-collection__item"]'):
+                bin_type = collectionDay.select('span[class*="bin-collection__type"]')[
+                    0
+                ].text.strip()
+                binCollection = (
+                        collectionDay.select('span[class*="bin-collection__day"]')[
+                            0
+                        ].text.strip()
+                        + ", "
+                        + collectionDay.select('span[class*="bin-collection__number"]')[
+                            0
+                        ].text.strip()
+                        + " "
+                        + monthName
+                )
+
+                dict_data = {
+                    "type": bin_type,
+                    "collectionDate": datetime.strptime(binCollection, "%A, %d %B %Y").strftime(date_format),
+                }
+
+                data["bins"].append(dict_data)
+
+        return data
+
+    def parse_data(self, page: str, **kwargs) -> dict:
+        page = "https://www.highpeak.gov.uk/findyourbinday"
+
+        # Assign user info
+        user_postcode = kwargs.get("postcode")
+        user_paon = kwargs.get("paon")
+
+        # Set up Selenium to run 'headless'
+        options = webdriver.ChromeOptions()
+        options.add_argument("--headless")
+        options.add_argument("--no-sandbox")
+        options.add_argument("--disable-gpu")
+        options.add_argument("--disable-dev-shm-usage")
+        options.add_experimental_option("excludeSwitches", ["enable-logging"])
+
+        # Create Selenium webdriver
+        driver = webdriver.Chrome(options=options)
+        driver.get(page)
+
+        # Hide Cookies
+        inputElement_hc = driver.find_element(
+            By.CLASS_NAME, "cookiemessage__link--close"
+        )
+        inputElement_hc.click()
+
+        # Enter postcode in text box and wait
+        inputElement_pc = driver.find_element(
+            By.ID, "FINDBINDAYSHIGHPEAK_POSTCODESELECT_POSTCODE"
+        )
+        inputElement_pc.send_keys(user_postcode)
+        inputElement_pc.send_keys(Keys.ENTER)
+
+        WebDriverWait(driver, 10).until(
+            EC.presence_of_element_located(
+                (By.ID, "FINDBINDAYSHIGHPEAK_ADDRESSSELECT_ADDRESS")
+            )
+        )
+
+        # Select address from dropdown and wait
+        inputElement_ad = Select(
+            driver.find_element(By.ID, "FINDBINDAYSHIGHPEAK_ADDRESSSELECT_ADDRESS")
+        )
+
+        inputElement_ad.select_by_visible_text(user_paon)
+
+        WebDriverWait(driver, 10).until(
+            EC.presence_of_element_located(
+                (By.ID, "FINDBINDAYSHIGHPEAK_ADDRESSSELECT_ADDRESSSELECTNEXTBTN_NEXT")
             )
-            # Search for the specific bins in the table using BS
-            # Parse the HTML content
-            # Find all elements with the class 'container-name' to extract bin types
-            # Parse the HTML content
-            soup = BeautifulSoup(driver.page_source, "html.parser")
-            soup.prettify
-
-            # Find all elements with class 'govuk-summary-list'
-            bin_info = []
-            waste_services = soup.find_all(
-                "h3", class_="govuk-heading-m waste-service-name"
+        )
+
+        # Submit address information and wait
+        driver.find_element(
+            By.ID, "FINDBINDAYSHIGHPEAK_ADDRESSSELECT_ADDRESSSELECTNEXTBTN_NEXT"
+        ).click()
+
+        WebDriverWait(driver, 10).until(
+            EC.presence_of_element_located(
+                (By.ID, "FINDBINDAYSHIGHPEAK_CALENDAR_MAINCALENDAR")
             )
+        )
 
-            for service in waste_services:
-                service_title = service.get_text(strip=True)
-                next_collection = service.find_next_sibling().find(
-                    "dt", text="Next collection"
-                )
+        # Read next collection information into Pandas
+        table = driver.find_element(
+            By.ID, "FINDBINDAYSHIGHPEAK_CALENDAR_MAINCALENDAR"
+        ).get_attribute("outerHTML")
+
+        # Parse data into dict
+        data = self.get_data(table)
 
-                if next_collection:
-                    next_collection_date = next_collection.find_next_sibling().get_text(
-                        strip=True
-                    )
-                    # Extract date part and remove the suffix
-                    next_collection_date_parse = next_collection_date.split(",")[
-                        1
-                    ].strip()
-                    day = next_collection_date_parse.split()[0]
-                    month = next_collection_date_parse.split()[1]
-
-                    # Remove the suffix (e.g., 'th', 'nd', 'rd', 'st') from the day
-                    if day.endswith(("th", "nd", "rd", "st")):
-                        day = day[:-2]  # Remove the last two characters
-
-                    # Reconstruct the date string without the suffix
-                    date_without_suffix = f"{day} {month}"
-
-                    # Parse the date string to a datetime object
-                    date_object = datetime.strptime(date_without_suffix, "%d %B")
-
-                    # Get the current year
-                    current_year = datetime.now().year
-
-                    # Check if the parsed date is in the past compared to the current date
-                    if date_object < datetime.now():
-                        # If the parsed date is in the past, assume it's for the next year
-                        current_year += 1
-                    # Append the year to the date
-                    date_with_year = date_object.replace(year=current_year)
-
-                    # Format the date with the year
-                    date_with_year_formatted = date_with_year.strftime(
-                        "%d/%m/%Y"
-                    )  # Format the date as '%d/%m/%Y'
-
-                    # Create the dictionary with the formatted data
-                    dict_data = {
-                        "type": service_title,
-                        "collectionDate": date_with_year_formatted,
-                    }
-                    data["bins"].append(dict_data)
-        except Exception as e:
-            # Here you can log the exception if needed
-            print(f"An error occurred: {e}")
-            # Optionally, re-raise the exception if you want it to propagate
-            raise
-        finally:
-            # This block ensures that the driver is closed regardless of an exception
-            if driver:
-                driver.quit()
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BroxtoweBoroughCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/RushcliffeBoroughCouncil.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,107 +1,89 @@
 from bs4 import BeautifulSoup
+from selenium import webdriver
 from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.support.wait import WebDriverWait
-
+from selenium.webdriver.support import expected_conditions as EC
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        driver = None
-        try:
-            page = "https://selfservice.broxtowe.gov.uk/renderform.aspx?t=217&k=9D2EF214E144EE796430597FB475C3892C43C528"
-
-            data = {"bins": []}
-
-            user_uprn = kwargs.get("uprn")
-            user_postcode = kwargs.get("postcode")
-            web_driver = kwargs.get("web_driver")
-            headless = kwargs.get("headless")
-            check_uprn(user_uprn)
-            check_postcode(user_postcode)
-
-            # Create Selenium webdriver
-            driver = create_webdriver(web_driver, headless, None, __name__)
-            driver.get(page)
-
-            # Populate postcode field
-            inputElement_postcode = driver.find_element(
-                By.ID,
-                "ctl00_ContentPlaceHolder1_FF5683TB",
-            )
-            inputElement_postcode.send_keys(user_postcode)
-
-            # Click search button
-            driver.find_element(
-                By.ID,
-                "ctl00_ContentPlaceHolder1_FF5683BTN",
-            ).click()
-
-            # Wait for the 'Select address' dropdown to appear and select option matching UPRN
-            dropdown = WebDriverWait(driver, 10).until(
-                EC.presence_of_element_located(
-                    (By.ID, "ctl00_ContentPlaceHolder1_FF5683DDL")
-                )
-            )
-            # Create a 'Select' for it, then select the matching URPN option
-            dropdownSelect = Select(dropdown)
-            dropdownSelect.select_by_value("U" + user_uprn)
-
-            # Wait for the submit button to appear, then click it to get the collection dates
-            submit = WebDriverWait(driver, 10).until(
-                EC.presence_of_element_located(
-                    (By.ID, "ctl00_ContentPlaceHolder1_btnSubmit")
-                )
-            )
-            submit.click()
-
-            soup = BeautifulSoup(driver.page_source, features="html.parser")
-
-            bins_div = soup.find("div", id="ctl00_ContentPlaceHolder1_FF5686FormGroup")
-            if bins_div:
-                bins_table = bins_div.find("table")
-                if bins_table:
-                    # Get table rows
-                    for row in bins_table.find_all("tr"):
-                        # Get the rows cells
-                        cells = row.find_all("td")
-                        bin_type = cells[0].get_text(strip=True)
-                        # Skip header row
-                        if bin_type and cells[3] and bin_type != "Bin Type":
-                            if len(cells[3].get_text(strip=True)) > 0:
-                                collection_date = datetime.strptime(
-                                    cells[3].get_text(strip=True), "%A, %d %B %Y"
-                                )
-                                dict_data = {
-                                    "type": bin_type,
-                                    "collectionDate": collection_date.strftime(
-                                        date_format
-                                    ),
-                                }
-                                data["bins"].append(dict_data)
-
-                            data["bins"].sort(
-                                key=lambda x: datetime.strptime(
-                                    x.get("collectionDate"), "%d/%m/%Y"
-                                )
-                            )
-        except Exception as e:
-            # Here you can log the exception if needed
-            print(f"An error occurred: {e}")
-            # Optionally, re-raise the exception if you want it to propagate
-            raise
-        finally:
-            # This block ensures that the driver is closed regardless of an exception
-            if driver:
-                driver.quit()
+        page = "https://selfservice.rushcliffe.gov.uk/renderform.aspx?t=1242&k=86BDCD8DE8D868B9E23D10842A7A4FE0F1023CCA"
+
+        data = {"bins": []}
+
+        user_uprn = kwargs.get("uprn")
+        user_postcode = kwargs.get("postcode")
+        check_uprn(user_uprn)
+        check_postcode(user_postcode)
+
+        # Set up Selenium to run 'headless'
+        options = webdriver.ChromeOptions()
+        options.add_argument("--headless")
+        options.add_argument("--no-sandbox")
+        options.add_argument("--disable-gpu")
+        options.add_argument("--disable-dev-shm-usage")
+        options.add_experimental_option("excludeSwitches", ["enable-logging"])
+
+        # Create Selenium webdriver
+        driver = webdriver.Chrome(options=options)
+        driver.get(page)
+
+        # Populate postcode field
+        inputElement_postcode = driver.find_element(
+            By.ID,
+            "ctl00_ContentPlaceHolder1_FF3518TB",
+        )
+        inputElement_postcode.send_keys(user_postcode)
+
+        # Click search button
+        driver.find_element(
+            By.ID,
+            "ctl00_ContentPlaceHolder1_FF3518BTN",
+        ).click()
+
+        # Wait for the 'Select address' dropdown to appear and select option matching UPRN
+        dropdown = WebDriverWait(driver, 10).until(
+            EC.presence_of_element_located((By.ID, "ctl00_ContentPlaceHolder1_FF3518DDL"))
+        )
+        # Create a 'Select' for it, then select the matching URPN option
+        dropdownSelect = Select(dropdown)
+        dropdownSelect.select_by_value("U" + user_uprn)
+
+        # Wait for the submit button to appear, then click it to get the collection dates
+        submit = WebDriverWait(driver, 10).until(
+            EC.presence_of_element_located((By.ID, "ctl00_ContentPlaceHolder1_btnSubmit"))
+        )
+        submit.click()
+
+        soup = BeautifulSoup(driver.page_source, features="html.parser")
+
+        bins_text = soup.find("div", id="ctl00_ContentPlaceHolder1_pnlConfirmation")
+
+        if bins_text:
+            results = re.findall("Your (.*?) bin will next be collected on (\d\d?\/\d\d?\/\d{4})",
+                                 bins_text.find("div", {"class": "ss_confPanel"}).get_text())
+            if results:
+                for result in results:
+                    collection_date = datetime.strptime(result[1], "%d/%m/%Y")
+                    dict_data = {
+                        "type": result[0],
+                        "collectionDate": collection_date.strftime(date_format),
+                    }
+                    data["bins"].append(dict_data)
+
+                    data["bins"].sort(
+                        key=lambda x: datetime.strptime(x.get("collectionDate"), "%d/%m/%Y")
+                    )
+
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BuckinghamshireCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/Chilterns.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import time
 
 import pandas as pd
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support.ui import Select
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
@@ -28,69 +30,64 @@
             }
 
             data["bins"].append(dict_data)
 
         return data
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        driver = None
-        try:
-            page = "https://chiltern.gov.uk/collection-dates"
-
-            # Assign user info
-            user_postcode = kwargs.get("postcode")
-            user_paon = kwargs.get("paon")
-            web_driver = kwargs.get("web_driver")
-            headless = kwargs.get("headless")
-
-            # Create Selenium webdriver
-            driver = create_webdriver(web_driver, headless, None, __name__)
-            driver.get(page)
+        page = "https://chiltern.gov.uk/collection-dates"
 
-            # Enter postcode in text box and wait
-            inputElement_pc = driver.find_element(
+        # Assign user info
+        user_postcode = kwargs.get("postcode")
+        user_paon = kwargs.get("paon")
+
+        # Set up Selenium to run 'headless'
+        options = webdriver.ChromeOptions()
+        options.add_argument("--headless")
+        options.add_argument("--no-sandbox")
+        options.add_argument("--disable-gpu")
+        options.add_argument("--disable-dev-shm-usage")
+        options.add_experimental_option("excludeSwitches", ["enable-logging"])
+
+        # Create Selenium webdriver
+        driver = webdriver.Chrome(options=options)
+        driver.get(page)
+
+        # Enter postcode in text box and wait
+        inputElement_pc = driver.find_element(
+            By.ID, "COPYOFECHOCOLLECTIONDATES_ADDRESSSELECTION_ADDRESSSELECTIONPOSTCODE"
+        )
+        inputElement_pc.send_keys(user_postcode)
+        inputElement_pc.send_keys(Keys.ENTER)
+
+        time.sleep(4)
+
+        # Select address from dropdown and wait
+        inputElement_ad = Select(
+            driver.find_element(
                 By.ID,
-                "COPYOFECHOCOLLECTIONDATES_ADDRESSSELECTION_ADDRESSSELECTIONPOSTCODE",
+                "COPYOFECHOCOLLECTIONDATES_ADDRESSSELECTION_ADDRESSSELECTIONADDRESS",
             )
-            inputElement_pc.send_keys(user_postcode)
-            inputElement_pc.send_keys(Keys.ENTER)
+        )
 
-            time.sleep(4)
+        inputElement_ad.select_by_visible_text(user_paon)
 
-            # Select address from dropdown and wait
-            inputElement_ad = Select(
-                driver.find_element(
-                    By.ID,
-                    "COPYOFECHOCOLLECTIONDATES_ADDRESSSELECTION_ADDRESSSELECTIONADDRESS",
-                )
-            )
+        time.sleep(4)
+
+        # Submit address information and wait
+        inputElement_bn = driver.find_element(
+            By.ID, "COPYOFECHOCOLLECTIONDATES_ADDRESSSELECTION_NAV1_NEXT"
+        ).click()
+
+        time.sleep(4)
 
-            inputElement_ad.select_by_visible_text(user_paon)
+        # Read next collection information into Pandas
+        table = driver.find_element(
+            By.ID, "COPYOFECHOCOLLECTIONDATES_PAGE1_DATES2"
+        ).get_attribute("outerHTML")
+        df = pd.read_html(table, header=[1])
+        df = df[0]
 
-            time.sleep(4)
+        # Parse data into dict
+        data = self.get_data(df)
 
-            # Submit address information and wait
-            inputElement_bn = driver.find_element(
-                By.ID, "COPYOFECHOCOLLECTIONDATES_ADDRESSSELECTION_NAV1_NEXT"
-            ).click()
-
-            time.sleep(4)
-
-            # Read next collection information into Pandas
-            table = driver.find_element(
-                By.ID, "COPYOFECHOCOLLECTIONDATES_PAGE1_DATES2"
-            ).get_attribute("outerHTML")
-            df = pd.read_html(table, header=[1])
-            df = df[0]
-
-            # Parse data into dict
-            data = self.get_data(df)
-        except Exception as e:
-            # Here you can log the exception if needed
-            print(f"An error occurred: {e}")
-            # Optionally, re-raise the exception if you want it to propagate
-            raise
-        finally:
-            # This block ensures that the driver is closed regardless of an exception
-            if driver:
-                driver.quit()
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/BuryCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/MalvernHillsDC.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,58 @@
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
+        api_url = "https://swict.malvernhills.gov.uk/mhdcroundlookup/HandleSearchScreen"
+
+        user_uprn = kwargs.get("uprn")
+        # Check the UPRN is valid
+        check_uprn(user_uprn)
+
+        # Create the form data
+        form_data = {"nmalAddrtxt": "", "alAddrsel": user_uprn}
+        # expects postcode to be looked up and then uprn used.
+        # we can just provide uprn
+
+        # Make a request to the API
+        requests.packages.urllib3.disable_warnings()
+        response = requests.post(api_url, data=form_data)
+
         # Make a BS4 object
-        collections = []
+        soup = BeautifulSoup(response.text, features="html.parser")
+        soup.prettify()
+
+        # Find results table
+        table_element = soup.find("table")
+        table_body = table_element.find("tbody")
+        rows = table_body.find_all("tr")
+
         data = {"bins": []}
 
-        # Get and check postcode and PAON
-        postcode = kwargs.get("postcode")
-        paon = kwargs.get("paon")
-        check_postcode(postcode)
-        check_paon(paon)
-
-        # Make API call to get property info using postcode
-        addr_response = requests.get(
-            f'https://www.bury.gov.uk/app-services/getProperties?postcode={postcode.replace(" ", "")}'
-        )
-        if addr_response.status_code != 200:
-            raise ConnectionAbortedError("Issue encountered getting addresses.")
-        address_json = json.loads(addr_response.text)["response"]
-
-        # This makes addr the next item that has the house number. Since these are ordered by house number, a single
-        # number like 3 wouldn't return 33
-        addr = next(item for item in address_json if paon in item["addressLine1"])
-
-        # Make API call to get bin data using property ID
-        response = requests.get(
-            f'https://www.bury.gov.uk/app-services/getPropertyById?id={addr.get("id")}'
-        )
-        if response.status_code != 200:
-            raise ConnectionAbortedError("Issue encountered getting bin data.")
-        bin_list = json.loads(response.text)["response"]["bins"]
-
-        # The JSON actually returns the next collections and a large calendar. But I opted just for the next dates.
-        for bin_colour, collection_data in bin_list.items():
-            bin_type = bin_colour
-            bin_date = datetime.strptime(
-                remove_ordinal_indicator_from_date_string(
-                    collection_data.get("nextCollection")
-                ),
-                "%A %d %B %Y",
-            )
-            collections.append((bin_type, bin_date))
-
-        # Dates are ordered correctly - soonest first
-        ordered_data = sorted(collections, key=lambda x: x[1])
-        for item in ordered_data:
-            dict_data = {
-                "type": item[0],
-                "collectionDate": item[1].strftime(date_format),
-            }
-            data["bins"].append(dict_data)
+        for row in rows:
+            columns = row.find_all("td")
+            columns = [ele.text.strip() for ele in columns]
+
+            thisCollection = [ele for ele in columns if ele]  # Get rid of empty values
+
+            # if not signed up for garden waste, this appears as Not applicable
+            if "Not applicable" not in thisCollection[1]:
+                bin_type = thisCollection[0].replace("collection", "").strip()
+                date = datetime.strptime(thisCollection[1], "%A %d/%m/%Y")
+                dict_data = {
+                    "type": bin_type,
+                    "collectionDate": date.strftime(date_format),
+                }
+                data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/CalderdaleCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/ValeofGlamorganCouncil.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,122 +1,113 @@
-# This script pulls (in one hit) the data from Bromley Council Bins Data
-import datetime
-import time
-from datetime import datetime
-
-import requests
 from bs4 import BeautifulSoup
-from selenium.webdriver.common.by import By
-from selenium.webdriver.common.keys import Keys
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import Select
-from selenium.webdriver.support.wait import WebDriverWait
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        driver = None
-        try:
-            user_uprn = kwargs.get("uprn")
-            user_postcode = kwargs.get("postcode")
-            check_uprn(user_uprn)
-            check_postcode(user_postcode)
-
-            bin_data_dict = {"bins": []}
-            collections = []
-            web_driver = kwargs.get("web_driver")
-            headless = kwargs.get("headless")
-
-            data = {"bins": []}
-
-            # Get our initial session running
-            driver = create_webdriver(web_driver, headless, None, __name__)
-            driver.get(kwargs.get("url"))
-
-            wait = WebDriverWait(driver, 30)
-            postcode = wait.until(
-                EC.presence_of_element_located((By.XPATH, '//*[@id="pPostcode"]'))
-            )
+        requests.packages.urllib3.disable_warnings()
+        user_uprn = kwargs.get("uprn")
+        check_uprn(user_uprn)
+        headers = {
+            "Accept": "*/*",
+            "Accept-Language": "en-GB,en;q=0.6",
+            "Connection": "keep-alive",
+            "Referer": "https://www.valeofglamorgan.gov.uk/",
+            "Sec-Fetch-Dest": "script",
+            "Sec-Fetch-Mode": "no-cors",
+            "Sec-Fetch-Site": "same-site",
+            "Sec-GPC": "1",
+            "sec-ch-ua": '"Not?A_Brand";v="8", "Chromium";v="108", "Brave";v="108"',
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": '"Windows"',
+        }
+        params = {
+            "RequestType": "LocalInfo",
+            "ms": "ValeOfGlamorgan/AllMaps",
+            "group": "Community and Living|Refuse HIDE2",
+            "type": "json",
+            "callback": "AddressInfoCallback",
+            "uid": user_uprn,
+            "import": "jQuery35108514154283927682_1673022974838",
+            "_": "1673022974840",
+        }
+
+        # Get a response from the council
+        response = requests.get(
+            "https://myvale.valeofglamorgan.gov.uk/getdata.aspx",
+            params=params,
+            headers=headers,
+        ).text
+
+        # Load the JSON and seek out the bin week text, then add it to the calendar URL. Also take the weekly
+        # collection type and generate dates for it. Then make a GET request for the calendar
+        bin_week = str(
+            json.loads(response)["Results"]["Refuse_HIDE2"]["Your_Refuse_round_is"]
+        ).replace(" ", "-")
+        weekly_collection = str(
+            json.loads(response)["Results"]["Refuse_HIDE2"]["Recycling__type"]
+        ).capitalize()
+        weekly_dates = get_weekday_dates_in_period(
+            datetime.now(), days_of_week.get(bin_week.split("-")[0].strip()), amount=48
+        )
+        schedule_url = f"https://www.valeofglamorgan.gov.uk/en/living/Recycling-and-Waste/collections/Black-Bag-Collections/{bin_week}.aspx"
+        response = requests.get(schedule_url, verify=False)
+
+        # BS4 parses the calendar
+        soup = BeautifulSoup(response.text, features="html.parser")
+        soup.prettify()
+
+        # Some scraper variables
+        collections = []
+
+        # Get the calendar table and find the headers
+        table = soup.find("table", {"class": "TableStyle_Activities"}).find("tbody")
+        table_headers = table.find("tr").find_all("th")
+        # For all rows below the header, find all details in th next row
+        for tr in soup.find_all("tr")[1:]:
+            row = tr.find_all("td")
+            # Parse month and year - month needs converting from text to number
+            month_and_year = row[0].text.split()
+            if month_and_year[0] in list(calendar.month_abbr):
+                collection_month = datetime.strptime(month_and_year[0], "%b").month
+            elif month_and_year[0] == "Sept":
+                collection_month = int(9)
+            else:
+                collection_month = datetime.strptime(month_and_year[0], "%B").month
+            collection_year = datetime.strptime(month_and_year[1], "%Y").year
+
+            # Get the collection dates column, remove anything that's not a number or space and then convert to dates
+            for day in remove_alpha_characters(row[1].text.strip()).split():
+                try:
+                    bin_date = datetime(collection_year, collection_month, int(day))
+                    collections.append((table_headers[1].text.strip().replace(" collection date", ""), bin_date))
+                except Exception as ex:
+                    continue
 
-            postcode.send_keys(user_postcode)
-            postcode_search_btn = wait.until(
-                EC.element_to_be_clickable((By.CLASS_NAME, "searchbox_submit"))
+        # Add in weekly dates to the tuple
+        for date in weekly_dates:
+            collections.append(
+                (weekly_collection, datetime.strptime(date, date_format))
             )
-            postcode_search_btn.send_keys(Keys.ENTER)
-            # Wait for the 'Select your property' dropdown to appear and select the first result
-            dropdown = wait.until(EC.element_to_be_clickable((By.ID, "uprn")))
-
-            # Create a 'Select' for it, then select the first address in the list
-            # (Index 0 is "Make a selection from the list")
-            dropdownSelect = Select(dropdown)
-            dropdownSelect.select_by_value(str(user_uprn))
-            checkbox = wait.until(EC.presence_of_element_located((By.ID, "gdprTerms")))
-            checkbox.send_keys(Keys.SPACE)
-            get_bin_data_btn = wait.until(
-                EC.element_to_be_clickable((By.CLASS_NAME, "searchbox_submit"))
-            )
-            get_bin_data_btn.send_keys(Keys.ENTER)
-            # Make a BS4 object
-            results = wait.until(EC.presence_of_element_located((By.ID, "collection")))
-            soup = BeautifulSoup(driver.page_source, features="html.parser")
-            soup.prettify()
-
-            data = {"bins": []}
-
-            # Get collections
-            row_index = 0
-            for row in soup.find("table", {"id": "collection"}).find_all("tr"):
-                # Skip headers row
-                if row_index < 1:
-                    row_index += 1
-                    continue
-                else:
-                    # Get bin info
-                    bin_info = row.find_all("td")
-                    # Get the bin type
-                    bin_type = bin_info[0].find("strong").get_text(strip=True)
-                    # Get the collection date
-                    collection_date = ""
-                    for p in bin_info[2].find_all("p"):
-                        if "your next collection" in p.get_text(strip=True):
-                            collection_date = datetime.strptime(
-                                " ".join(
-                                    p.get_text(strip=True)
-                                    .replace("will be your next collection.", "")
-                                    .split()
-                                ),
-                                "%A %d %B %Y",
-                            )
-
-                    if collection_date != "":
-                        # Append the bin type and date to the data dict
-                        dict_data = {
-                            "type": bin_type,
-                            "collectionDate": collection_date.strftime(date_format),
-                        }
-                        data["bins"].append(dict_data)
 
-                    row_index += 1
+        # Order all the data, only including future dates
+        ordered_data = sorted(collections, key=lambda x: x[1])
+        data = {"bins": []}
+        for item in ordered_data:
+            collection_date = item[1]
+            if collection_date.date() >= datetime.now().date():
+                dict_data = {
+                    "type": item[0],
+                    "collectionDate": collection_date.strftime(date_format),
+                }
+                data["bins"].append(dict_data)
 
-            data["bins"].sort(
-                key=lambda x: datetime.strptime(x.get("collectionDate"), date_format)
-            )
-        except Exception as e:
-            # Here you can log the exception if needed
-            print(f"An error occurred: {e}")
-            # Optionally, re-raise the exception if you want it to propagate
-            raise
-        finally:
-            # This block ensures that the driver is closed regardless of an exception
-            if driver:
-                driver.quit()
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/CannockChaseDistrictCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NorthSomersetCouncil.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,73 @@
 from bs4 import BeautifulSoup
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
-# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        user_uprn = kwargs.get("uprn")
-        user_postcode = kwargs.get("postcode")
-        check_uprn(user_uprn)
-        check_postcode(user_postcode)
-
-        # Make SOAP Request
-        response = requests.post(
-            "https://ccdc.opendata.onl/DynamicCall.dll",
-            data="Method=CollectionDates&Postcode="
-            + user_postcode
-            + "&UPRN="
-            + user_uprn,
-            headers={
-                "Content-Type": "application/x-www-form-urlencoded",
-                "Referer": "https://ccdc.opendata.onl/CCDC_WasteCollection",
-                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/118.0.0.0 Safari/537.36",
-            },
-        )
+        api_url = "https://forms.n-somerset.gov.uk/Waste/CollectionSchedule"
+        uprn = kwargs.get("uprn")
+        postcode = kwargs.get("postcode")
+        check_uprn(uprn)
+        check_postcode(postcode)
+
+        # Get schedule from API
+        values = {
+            "PreviousHouse": "",
+            "PreviousPostcode": postcode,
+            "Postcode": postcode,
+            "SelectedUprn": uprn,
+        }
+        headers = {"User-Agent": "Mozilla/5.0 (Windows NT 6.1; Win64; x64)"}
+        requests.packages.urllib3.disable_warnings()
+        response = requests.request("POST", api_url, headers=headers, data=values)
 
-        # Make a BS4 object
-        soup = BeautifulSoup(response.text, "xml")
-        soup.prettify()
-
-        if (
-            soup.find("ErrorDescription")
-            and soup.find("ErrorDescription").get_text(strip=True)
-            == "No results returned"
-        ):
-            raise ValueError("No collection data found for provided Postcode & UPRN.")
+        soup = BeautifulSoup(response.text, features="html.parser")
 
+        rows = soup.find("table", {"class": re.compile("table")}).find_all("tr")
+
+        # Form a JSON wrapper
         data = {"bins": []}
 
-        collections = soup.find_all("Collection")
+        # Loops the Rows
+        for row in rows:
+            cells = row.find_all("td")
+            if cells:
+                binType = cells[0].get_text(strip=True)
+                collectionDate = cells[1].get_text(strip=True) + " " + datetime.now().strftime("%Y")
+                nextCollectionDate = cells[2].get_text(strip=True) + " " + datetime.now().strftime("%Y")
+
+                # Make each Bin element in the JSON
+                dict_data = {
+                    "type": binType,
+                    "collectionDate": get_next_occurrence_from_day_month(
+                        datetime.strptime(collectionDate, "%A %d %B %Y")
+                    ).strftime(date_format)
+                }
+
+                # Add data to the main JSON Wrapper
+                data["bins"].append(dict_data)
+
+                # Make each next Bin element in the JSON
+                dict_data = {
+                    "type": binType,
+                    "collectionDate": get_next_occurrence_from_day_month(
+                        datetime.strptime(nextCollectionDate, "%A %d %B %Y")
+                    ).strftime(date_format),
+                }
 
-        for i in range(len(collections)):
-            dict_data = {
-                "type": collections[i]
-                .Service.get_text()
-                .replace("Collection Service", "")
-                .strip(),
-                "collectionDate": datetime.strptime(
-                    collections[i].Date.get_text(), "%d/%m/%Y %H:%M:%S"
-                ).strftime(date_format),
-            }
-            data["bins"].append(dict_data)
+                # Add data to the main JSON Wrapper
+                data["bins"].append(dict_data)
 
         data["bins"].sort(
             key=lambda x: datetime.strptime(x.get("collectionDate"), date_format)
         )
+
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/CardiffCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/CardiffCouncil.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import datetime
 import json
 from datetime import datetime
 
 import requests
 from requests import auth
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # Taken from
 # https://stackoverflow.com/questions/29931671/making-an-api-call-in-python-with-an-api-that-requires-a-bearer-token
 class BearerAuth(requests.auth.AuthBase):
     def __init__(self, token):
         self.token = token
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/CastlepointDistrictCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/CastlepointDistrictCouncil.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
         # Disable the SSL warnings that otherwise break everything
         requests.packages.urllib3.disable_warnings()
+        requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS += ":HIGH:!DH:!aNULL"
         try:
             requests.packages.urllib3.contrib.pyopenssl.util.ssl_.DEFAULT_CIPHERS += (
                 ":HIGH:!DH:!aNULL"
             )
         except AttributeError:
             pass
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/CharnwoodBoroughCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/CharnwoodBoroughCouncil.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
-
-from datetime import timedelta
-from dateutil.relativedelta import relativedelta
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
@@ -16,39 +14,29 @@
 
     def parse_data(self, page: str, **kwargs) -> dict:
         # Make a BS4 object
         soup = BeautifulSoup(page.text, features="html.parser")
         soup.prettify()
 
         data = {"bins": []}
-        curr_date = datetime.today()
 
         for bins in soup.find_all("ul", {"class": "refuse"}):
             binCollection = bins.find_all("li")
 
             if binCollection:
                 for bin in binCollection:
-                    collection_date = (
-                        bin.find("strong", {"class": "date"}).contents[0].strip()
-                    )
+                    collection_date = bin.find("strong", {"class": "date"}).contents[0].strip()
                     if collection_date.lower() == "today":
                         collection_date = datetime.now()
-                    elif collection_date.lower() == "tomorrow":
-                        collection_date = datetime.now() + timedelta(days=1)
                     else:
-                        collection_date += f" {curr_date.year}"
                         collection_date = datetime.strptime(
-                            remove_ordinal_indicator_from_date_string(
-                                collection_date
-                            ).strip(),
-                            "%a %d %b %Y",
+                            remove_ordinal_indicator_from_date_string(collection_date).strip(),
+                            "%a %d %b"
                         )
-                        if curr_date.month == 12 and collection_date.month == 1:
-                            collection_date = collection_date + relativedelta(years=1)
                     dict_data = {
                         "type": bin.find("a").contents[0],
-                        "collectionDate": collection_date.strftime(date_format),
+                        "collectionDate": collection_date.strftime(date_format)
                     }
 
                     data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/CheshireEastCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NorthEastLincs.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,54 @@
+import pandas as pd
 from bs4 import BeautifulSoup
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.common import date_format
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 class CouncilClass(AbstractGetBinDataClass):
+    """
+    Concrete classes have to implement all abstract operations of the
+    baseclass. They can also override some
+    operations with a default implementation.
+    """
+
     def parse_data(self, page: str, **kwargs) -> dict:
+        # Make a BS4 object
         soup = BeautifulSoup(page.text, features="html.parser")
+        soup.prettify()
 
-        bin_data_dict = {"bins": []}
+        data = {"bins": []}
 
-        table = soup.find("table", {"class": "job-details"})
-        if table:
-            rows = table.find_all("tr", {"class": "data-row"})
-
-            for row in rows:
-                cells = row.find_all(
-                    "td", {"class": lambda L: L and L.startswith("visible-cell")}
-                )
-                labels = cells[0].find_all("label") if cells else []
-
-                if len(labels) >= 3:
-                    bin_type = labels[2].get_text(strip=True)
-                    collection_date = labels[1].get_text(strip=True)
-
-                    bin_data_dict["bins"].append(
-                        {
-                            "type": bin_type,
-                            "collectionDate": collection_date,
-                        }
-                    )
+        # Get list items that can be seen on page
+        for element in soup.find_all(
+                "li", {"class": "list-group-item p-0 p-3 bin-collection-item"}
+        ):
+            element_text = element.text.strip().split("\n\n")
+            element_text = [x.strip() for x in element_text]
+
+            bin_type = element_text[1]
+            collection_date = pd.Timestamp(element_text[0]).strftime(date_format)
+
+            dict_data = {
+                "type": bin_type,
+                "collectionDate": collection_date,
+            }
+            data["bins"].append(dict_data)
+
+        # Get hidden list items too
+        for element in soup.find_all(
+                "li", {"class": "list-group-item p-0 p-3 bin-collection-item d-none"}
+        ):
+            element_text = element.text.strip().split("\n\n")
+            element_text = [x.strip() for x in element_text]
+
+            bin_type = element_text[1]
+            collection_date = pd.Timestamp(element_text[0]).strftime(date_format)
+
+            dict_data = {
+                "type": bin_type,
+                "collectionDate": collection_date,
+            }
+            data["bins"].append(dict_data)
 
-        return bin_data_dict
+        return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ChichesterDistrictCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NorthNorfolkDistrictCouncil.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,110 +1,93 @@
-import time
-from datetime import datetime
-
-from selenium.webdriver.support.ui import Select
 from bs4 import BeautifulSoup
+from selenium import webdriver
 from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.support.wait import WebDriverWait
-from selenium.webdriver.common.keys import Keys
-
+from selenium.webdriver.support import expected_conditions as EC
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        driver = None
-        try:
-            # Make a BS4 object
-
-            page = "https://www.chichester.gov.uk/checkyourbinday"
-
-            user_postcode = kwargs.get("postcode")
-            user_uprn = kwargs.get("uprn")
-            web_driver = kwargs.get("web_driver")
-            headless = kwargs.get("headless")
-            house_number = kwargs.get("paon")
-
-            driver = create_webdriver(web_driver, headless, None, __name__)
-            driver.get(page)
-
-            wait = WebDriverWait(driver, 60)
-
-            inputElement_postcodesearch = wait.until(
-                EC.visibility_of_element_located(
-                    (By.ID, "WASTECOLLECTIONCALENDARV5_CALENDAR_ADDRESSLOOKUPPOSTCODE")
-                )
-            )
+        page = "https://forms.north-norfolk.gov.uk/outreach/BinCollectionDays.ofml"
 
-            inputElement_postcodesearch.send_keys(user_postcode)
+        data = {"bins": []}
 
-            inputElement_postcodesearch_btn = wait.until(
-                EC.visibility_of_element_located(
-                    (By.ID, "WASTECOLLECTIONCALENDARV5_CALENDAR_ADDRESSLOOKUPSEARCH")
-                )
+        user_paon = kwargs.get("paon")
+        user_postcode = kwargs.get("postcode")
+        check_paon(user_paon)
+        check_postcode(user_postcode)
+
+        # Set up Selenium to run 'headless'
+        options = webdriver.ChromeOptions()
+        options.add_argument("--headless")
+        options.add_argument("--no-sandbox")
+        options.add_argument("--disable-gpu")
+        options.add_argument("--disable-dev-shm-usage")
+        options.add_experimental_option("excludeSwitches", ["enable-logging"])
+
+        # Create Selenium webdriver
+        driver = webdriver.Chrome(options=options)
+        driver.get(page)
+
+        # Populate postcode field
+        inputElement_postcode = driver.find_element(
+            By.ID,
+            "F_Address_subform:Postcode",
+        )
+        inputElement_postcode.send_keys(user_postcode)
+
+        # Click search button
+        driver.find_element(
+            By.ID,
+            "BA_Address_subform:Search_button",
+        ).click()
+
+        # Wait for the 'Select address' dropdown to appear
+        dropdown = WebDriverWait(driver, 10).until(
+            EC.presence_of_element_located((By.XPATH, "//select[@id='F_Address_subform:Id']"))
+        )
+        # Create a 'Select' for it, then select the matching house number/name option
+        dropdownSelect = Select(dropdown)
+        matchingOptions = [o for o in dropdownSelect.options if user_paon.lower() in o.text.lower()]
+        if matchingOptions:
+            matchingOptions[0].click()
+
+            # Wait for the results to appear
+            WebDriverWait(driver, 10).until(
+                EC.presence_of_element_located((By.XPATH, "//div[contains(@class, 'fieldmergedcolumn')]/ul"))
             )
-            inputElement_postcodesearch_btn.send_keys(Keys.ENTER)
 
-            inputElement_select_address = wait.until(
-                EC.element_to_be_clickable(
-                    (By.ID, "WASTECOLLECTIONCALENDARV5_CALENDAR_ADDRESSLOOKUPADDRESS")
-                )
-            )
-            dropdown_element = driver.find_element(
-                By.ID, "WASTECOLLECTIONCALENDARV5_CALENDAR_ADDRESSLOOKUPADDRESS"
-            )
-
-            # Now create a Select object based on the found element
-            dropdown = Select(dropdown_element)
-
-            # Select the option by visible text
-            dropdown.select_by_visible_text(house_number)
+            soup = BeautifulSoup(driver.page_source, features="html.parser")
 
-            results = wait.until(
-                EC.element_to_be_clickable(
-                    (By.CLASS_NAME, "bin-collection-dates-container")
-                )
-            )
+            bins_text = soup.find("div", id="Search_result_details_cps_hd")
 
-            soup = BeautifulSoup(driver.page_source, features="html.parser")
-            soup.prettify()
+            if bins_text:
+                results = re.findall("Your next (.*?) Bin collection is ([A-Za-z]+ \\d\\d? [A-Za-z]+)",
+                                     bins_text.get_text())
+                if results:
+                    for result in results:
+                        collection_date = datetime.strptime(result[1] + " " + datetime.now().strftime("%Y"),
+                                                            "%A %d %B %Y")
+                        dict_data = {
+                            "type": result[0],
+                            "collectionDate": collection_date.strftime(date_format),
+                        }
+                        data["bins"].append(dict_data)
+
+                        data["bins"].sort(
+                            key=lambda x: datetime.strptime(x.get("collectionDate"), date_format)
+                        )
+        else:
+            raise ValueError("No matching address for house number/name found.")
 
-            # Extract data from the table
-            bin_collection_data = []
-            rows = soup.find(
-                "table", class_="defaultgeneral bin-collection-dates"
-            ).find_all("tr")
-            for row in rows:
-                cells = row.find_all("td")
-                if cells:
-                    date_str = cells[0].text.strip()
-                    bin_type = cells[1].text.strip()
-                    # Convert date string to the required format DD/MM/YYYY
-                    date_obj = datetime.strptime(date_str, "%d %B %Y")
-                    date_formatted = date_obj.strftime(date_format)
-                    bin_collection_data.append(
-                        {"collectionDate": date_formatted, "type": bin_type}
-                    )
-
-            # Convert to JSON
-            json_data = {"bins": bin_collection_data}
-
-        except Exception as e:
-            # Here you can log the exception if needed
-            print(f"An error occurred: {e}")
-            # Optionally, re-raise the exception if you want it to propagate
-            raise
-        finally:
-            # This block ensures that the driver is closed regardless of an exception
-            if driver:
-                driver.quit()
-        return json_data
+        return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ConwyCountyBorough.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NorthLanarkshireCouncil.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,43 @@
 from bs4 import BeautifulSoup
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
 from uk_bin_collection.uk_bin_collection.common import *
-from datetime import datetime
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
+# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
+    """
+    Concrete classes have to implement all abstract operations of the
+    base class. They can also override some operations with a default
+    implementation.
+    """
+
     def parse_data(self, page: str, **kwargs) -> dict:
+        # Make a BS4 object
         soup = BeautifulSoup(page.text, features="html.parser")
-        data = {"bins": []}
+        soup.prettify()
 
-        for bin_section in soup.select('div[class*="containererf"]'):
-            date_text = bin_section.find(id="content").text.strip()
-            collection_date = datetime.strptime(date_text, "%A, %d/%m/%Y")
-
-            bin_types = bin_section.find(id="main1").findAll("li")
-            for bin_type in bin_types:
-                bin_type_name = bin_type.text.split("(")[0].strip()
-
-                data["bins"].append(
-                    {
-                        "type": bin_type_name,
-                        "collectionDate": collection_date.strftime(date_format),
-                    }
-                )
+        data = {"bins": []}
+        for bins in soup.select("div[class^=waste-type-container]"):
+            bin_type = bins.div.h3.text.strip()
+            collection_date = bins.select("div > p")[0].get_text(strip=True)
+            next_collection_date = bins.select("div > p")[1].get_text(strip=True)
+            if collection_date:
+                # Add collection date
+                dict_data = {
+                    "type": bin_type,
+                    "collectionDate": datetime.strptime(collection_date, "%d %B %Y").strftime(date_format)
+                }
+                data["bins"].append(dict_data)
+                # Add next collection date
+                dict_data = {
+                    "type": bin_type,
+                    "collectionDate": datetime.strptime(next_collection_date, "%d %B %Y").strftime(date_format)
+                }
+                data["bins"].append(dict_data)
+
+        data["bins"].sort(
+            key=lambda x: datetime.strptime(x.get("collectionDate"), date_format)
+        )
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/CrawleyBoroughCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/CrawleyBoroughCouncil.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from bs4 import BeautifulSoup
-from dateutil.relativedelta import relativedelta
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
         # Make a BS4 object
         uprn = kwargs.get("uprn")
-        usrn = kwargs.get("paon")
+        usrn = kwargs.get("usrn")
         check_uprn(uprn)
         check_usrn(usrn)
 
         day = datetime.now().date().strftime("%d")
         month = datetime.now().date().strftime("%m")
         year = datetime.now().date().strftime("%Y")
 
@@ -31,31 +30,24 @@
         response = requests.get(api_url)
 
         soup = BeautifulSoup(response.text, features="html.parser")
         soup.prettify()
 
         data = {"bins": []}
 
-        titles = [title.text for title in soup.select(".block-title")]
+        titles = [title.text for title in soup.select(".title")]
         collection_tag = soup.body.find_all(
             "div", {"class": "col-md-6 col-sm-6 col-xs-6"}, string="Next collection"
         )
         bin_index = 0
         for tag in collection_tag:
             for item in tag.next_elements:
-                if (
-                    str(item).startswith('<div class="date text-right text-grey">')
-                    and str(item) != ""
-                ):
-                    collection_date = datetime.strptime(item.text, "%A %d %B")
-                    next_collection = collection_date.replace(year=datetime.now().year)
-                    if datetime.now().month == 12 and next_collection.month == 1:
-                        next_collection = next_collection + relativedelta(years=1)
-
+                if str(item).startswith('<div class="date text-right text-grey">'):
+                    collection_date = datetime.strptime(item.text, "%A %d %B").strftime(date_format)
                     dict_data = {
                         "type": titles[bin_index].strip(),
-                        "collectionDate": next_collection.strftime(date_format),
+                        "collectionDate": collection_date,
                     }
                     data["bins"].append(dict_data)
                     bin_index += 1
                     break
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/DartfordBoroughCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/WarwickDistrictCouncil.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,36 @@
+# This script pulls (in one hit) the data
+# from Warick District Council Bins Data
+
 from bs4 import BeautifulSoup
-from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
+
     """
     Concrete classes have to implement all abstract operations of the
-    base class. They can also override some operations with a default
-    implementation.
+    baseclass. They can also override some
+    operations with a default implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
         # Make a BS4 object
         soup = BeautifulSoup(page.text, features="html.parser")
         soup.prettify()
 
-        # Extract data
-        bin_data = {"bins": []}
-
-        # Find the table containing the bin collection data
-        table = soup.find("table", {"class": "eb-EVDNdR1G-tableContent"})
-
-        if table:
-            rows = table.find_all("tr", class_="eb-EVDNdR1G-tableRow")
+        data = {"bins": []}
 
-            for row in rows:
-                columns = row.find_all("td")
-                if len(columns) >= 4:
-                    collection_type = columns[1].get_text(strip=True)
-                    collection_date = columns[3].get_text(strip=True)
-
-                    # Validate collection_date format
-                    if re.match(r"\d{2}/\d{2}/\d{4}", collection_date):
-                        bin_entry = {
-                            "type": collection_type,
-                            "collectionDate": collection_date,
-                        }
-                        bin_data["bins"].append(bin_entry)
+        for element in soup.find_all("strong"):
+            bin_type = element.next_element
+            bin_type = bin_type.lstrip()
+            collectionDateElement = element.next_sibling.next_element.next_element
+            collectionDate = collectionDateElement.getText()
+            dict_data = {
+                "type": bin_type,
+                "collectionDate": collectionDate,
+            }
+            data["bins"].append(dict_data)
 
-        return bin_data
+        return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/DoncasterCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/DoncasterCouncil.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import math
 from datetime import timedelta
 
 import requests
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/DorsetCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/DurhamCouncil.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,48 @@
-from bs4 import BeautifulSoup, element
+import re
+from datetime import datetime
+
+import requests
+from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        data = {"bins": []}
-        collections = []
+        url = "https://www.durham.gov.uk/bincollections?uprn="
+        uprn = kwargs.get("uprn")
+        check_uprn(uprn)
+        url += uprn
+        requests.packages.urllib3.disable_warnings()
+        page = requests.get(url)
 
-        # Parse the page and find all the result boxes
+        # Make a BS4 object
         soup = BeautifulSoup(page.text, features="html.parser")
-        soup.prettify()
-        results = soup.find_all("li", {"class": "resultListItem"})
 
-        # If the result box has a wanted string in, we can use it. Check the contents of each box and find the
-        # desired text and dates
-        for r in results:
-            if "Your next" in r.text:
-                if type(r.contents[10]) is element.NavigableString:
-                    bin_text = r.contents[10].text.split(" ")[2].title() + " bin"
-                    bin_date = datetime.strptime(
-                        remove_ordinal_indicator_from_date_string(
-                            r.contents[11].text.strip()
-                        ),
-                        "%A %d %B %Y",
-                    )
-                else:
-                    bin_text = r.contents[11].text.split(" ")[2].title() + " bin"
-                    bin_date = datetime.strptime(
-                        remove_ordinal_indicator_from_date_string(
-                            r.contents[12].text.strip()
-                        ),
-                        "%A %d %B %Y",
-                    )
-
-                if bin_date.date() >= datetime.now().date():
-                    collections.append((bin_text, bin_date))
-
-                # Sort the text and date elements by date
-                ordered_data = sorted(collections, key=lambda x: x[1])
-
-        # Put the elements into the dictionary
-        for item in ordered_data:
-            dict_data = {
-                "type": item[0],
-                "collectionDate": item[1].strftime(date_format),
-            }
-            data["bins"].append(dict_data)
+        data = {"bins": []}
+
+        for bin_type in ["rubbish", "recycling", "gardenwaste"]:
+            bin_info = soup.find(class_=f"bins{bin_type}")
+
+            if bin_info:
+                collection_text = bin_info.get_text(strip=True)
+
+                if collection_text:
+                    results = re.search("\\d\\d? [A-Za-z]+ \\d{4}", collection_text)
+                    if results:
+                        date = datetime.strptime(results[0], "%d %B %Y")
+                        if date:
+                            data["bins"].append({
+                                "type": bin_type,
+                                "collectionDate": date.strftime(date_format)
+                            })
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/DoverDistrictCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SheffieldCityCouncil.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 from bs4 import BeautifulSoup
-from datetime import datetime
-import re
-from uk_bin_collection.uk_bin_collection.common import *  # Consider specific imports
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.common import *
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
+# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
+    """
+    Concrete classes have to implement all abstract operations of the
+    base class. They can also override some operations with a default
+    implementation.
+    """
+
     def parse_data(self, page: str, **kwargs) -> dict:
-        soup = BeautifulSoup(page.text, "html.parser")
+        # Make a BS4 object
+        soup = BeautifulSoup(page.text, features="html.parser")
+        soup.prettify()
+
+        # Form a JSON wrapper
+        data = {"bins": []}
+
+        # Search for the specific table using BS4
+        rows = soup.find("table", {"class": re.compile("table")}).find_all("tr")
+
+        # Loops the Rows
+        for row in rows:
+            cells = row.find_all(
+                "td", {"class": lambda L: L and L.startswith("service-name")}
+            )
 
-        bins_data = {"bins": []}
-        bin_collections = []
+            if len(cells) > 0:
+                collectionDatesRawData = row.find_all(
+                    "td", {"class": lambda L: L and L.startswith("next-service")}
+                )[0].get_text(strip=True)
+                collectionDate = collectionDatesRawData[
+                                 16: len(collectionDatesRawData)
+                                 ].split(",")
+                bin_type = row.find_all(
+                    "td", {"class": lambda L: L and L.startswith("service-name")}
+                )[0].h4.get_text(strip=True)
+
+                for collectDate in collectionDate:
+                    # Make each Bin element in the JSON
+                    dict_data = {
+                        "type": bin_type,
+                        "collectionDate": datetime.strptime(collectDate.strip(), "%d %b %Y").strftime(date_format),
+                    }
 
-        results_wrapper = soup.find("div", {"class": "results-table-wrapper"})
-        if not results_wrapper:
-            return bins_data  # Return empty if the results wrapper is not found
-
-        bins = results_wrapper.find_all("div", {"class": "service-wrapper"})
-        for bin_item in bins:
-            service_name = bin_item.find("h3", {"class": "service-name"})
-            next_service = bin_item.find("td", {"class": "next-service"})
-
-            if service_name and next_service:
-                bin_type = service_name.get_text().replace("Collection", "bin").strip()
-                date_span = next_service.find("span", {"class": "table-label"})
-                date_text = (
-                    date_span.next_sibling.get_text().strip() if date_span else None
-                )
-
-                if date_text and re.match(r"\d{2}/\d{2}/\d{4}", date_text):
-                    try:
-                        bin_date = datetime.strptime(date_text, "%d/%m/%Y")
-                        bin_collections.append((bin_type, bin_date))
-                    except ValueError:
-                        continue
-
-        for bin_type, bin_date in sorted(bin_collections, key=lambda x: x[1]):
-            bins_data["bins"].append(
-                {
-                    "type": bin_type.capitalize(),
-                    "collectionDate": bin_date.strftime("%d/%m/%Y"),
-                }
-            )
+                    # Add data to the main JSON Wrapper
+                    data["bins"].append(dict_data)
 
-        return bins_data
+        return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/DurhamCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NorthKestevenDistrictCouncil.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,39 @@
-import re
-from datetime import datetime
-
-import requests
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        url = "https://www.durham.gov.uk/bincollections?uprn="
-        uprn = kwargs.get("uprn")
-        check_uprn(uprn)
-        url += uprn
-        requests.packages.urllib3.disable_warnings()
-        page = requests.get(url)
-
         # Make a BS4 object
         soup = BeautifulSoup(page.text, features="html.parser")
+        soup.prettify()
 
         data = {"bins": []}
 
-        for bin_type in ["rubbish", "recycling", "gardenwaste"]:
-            bin_info = soup.find(class_=f"bins{bin_type}")
-
-            if bin_info:
-                collection_text = bin_info.get_text(strip=True)
-
-                if collection_text:
-                    results = re.search("\\d\\d? [A-Za-z]+ \\d{4}", collection_text)
+        for bins in soup.find_all("div", {"class": lambda L: L and L.startswith("bg-")}):
+            for bin in bins.find_all("p"):
+                if bin.find("strong"):
+                    results = re.search(
+                        "Next Collection:(.*?) on ([A-Za-z]+, \\d\\d? [A-Za-z]+ \\d{4})",
+                        bin.find("strong").get_text(strip=True))
                     if results:
-                        date = datetime.strptime(results[0], "%d %B %Y")
-                        if date:
-                            data["bins"].append(
-                                {
-                                    "type": bin_type,
-                                    "collectionDate": date.strftime(date_format),
-                                }
-                            )
+                        collection_date = datetime.strptime(results.groups()[1], "%A, %d %B %Y")
+                        data["bins"].append({
+                            "type": bins.h3.get_text(strip=True),
+                            "collectionDate": collection_date.strftime(date_format)
+                        })
+
+        data["bins"].sort(
+            key=lambda x: datetime.strptime(x.get("collectionDate"), date_format)
+        )
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/EastCambridgeshireCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/EastCambridgeshireCouncil.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from bs4 import BeautifulSoup
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
@@ -18,15 +18,15 @@
         check_uprn(uprn)
 
         # Request URL
         url = f"https://eastcambs-self.achieveservice.com/appshost/firmstep/self/apps/custompage/bincollections?language=en&uprn={uprn}"
 
         # Make Request
         requests.packages.urllib3.disable_warnings()
-        s = requests.Session()
+        s = requests.session()
         page = s.get(url)
 
         # Make a BS4 object
         soup = BeautifulSoup(page.text, features="html.parser")
         soup.prettify()
 
         # Form a JSON wrapper
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/EastDevonDC.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/EastDevonDC.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 from datetime import datetime
 
 import pandas as pd
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import date_format
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     baseclass. They can also override some
     operations with a default implementation.
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/EastleighBoroughCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/EastleighBoroughCouncil.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
@@ -51,20 +52,19 @@
 
         # Create dict for bin name and string dates
         binDict = dict(zip(keys, values))
 
         # Process dict for valid bin types
         for bin in list(binDict):
             if bin in binTypes:
-                if not binDict[bin].startswith("You haven't yet signed up for"):
-                    # Convert date
-                    date = datetime.strptime(binDict[bin], "%a, %d %b %Y")
-
-                    # Set bin data
-                    dict_data = {
-                        "type": bin,
-                        "collectionDate": date.strftime(date_format),
-                    }
-                    data["bins"].append(dict_data)
+                # Convert date
+                date = datetime.strptime(binDict[bin], "%a, %d %b %Y")
+
+                # Set bin data
+                dict_data = {
+                    "type": bin,
+                    "collectionDate": date.strftime(date_format),
+                }
+                data["bins"].append(dict_data)
 
         # Return bin data
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/EnvironmentFirst.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/BromleyBoroughCouncil.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+# This script pulls (in one hit) the data from Bromley Council Bins Data
+import dateutil.parser
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
@@ -12,37 +15,32 @@
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
         # Make a BS4 object
         soup = BeautifulSoup(page.text, features="html.parser")
         soup.prettify()
 
-        # Get the paragraph lines from the page
-        data = {"bins": []}
-        page_text = soup.find("div", {"class": "collect"}).find_all("p")
-
-        # Parse the correct lines (find them, remove the ordinal indicator and make them the correct format date) and
-        # then add them to the dictionary
-        rubbish_day = datetime.strptime(
-            remove_ordinal_indicator_from_date_string(
-                page_text[2].find_next("strong").text
-            ),
-            "%d %B %Y",
-        ).strftime(date_format)
-        dict_data = {
-            "type": "Rubbish",
-            "collectionDate": rubbish_day,
-        }
-        data["bins"].append(dict_data)
-        recycling_day = datetime.strptime(
-            remove_ordinal_indicator_from_date_string(
-                page_text[4].find_next("strong").text
-            ),
-            "%d %B %Y",
-        ).strftime(date_format)
-        dict_data = {
-            "type": "Recycling",
-            "collectionDate": recycling_day,
-        }
-        data["bins"].append(dict_data)
+        bin_data_dict = {"bins": []}
 
-        return data
+        # Search for the specific bin in the table using BS4
+        rows = soup.find("div", class_=("waste__collections")).find_all(
+            "h3",
+            class_=("waste-service-name",),
+        )
+
+        # Loops the Rows
+        for row in rows:
+            bin_type = row.get_text().strip()
+            collectionDate = row.find_all_next(
+                "dd", {"class": "govuk-summary-list__value"}
+            )
+            # Make each Bin element in the JSON, but only if we have a date available
+            if collectionDate:
+                date = dateutil.parser.parse(collectionDate[1].text.strip())
+                dict_data = {
+                    "type": bin_type,
+                    "collectionDate": date.strftime(date_format),
+                }
+                # Add data to the main JSON Wrapper
+                bin_data_dict["bins"].append(dict_data)
+
+        return bin_data_dict
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ErewashBoroughCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/ErewashBoroughCouncil.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/FarehamBoroughCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/YorkCouncil.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,46 @@
 import json
+from datetime import datetime
 
 import requests
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
+# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        user_postcode = kwargs.get("postcode")
-        check_postcode(user_postcode)
-
-        headers = {
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/107.0.0.0 Safari/537.36",
-        }
-        params = {
-            "type": "JSON",
-            "list": "DomesticBinCollections",
-            "Road": "",
-            "Postcode": user_postcode,
-        }
-
-        response = requests.get(
-            "https://www.fareham.gov.uk/internetlookups/search_data.aspx",
-            params=params,
-            headers=headers,
+        api_url = (
+            "https://waste-api.york.gov.uk/api/Collections/GetBinCollectionDataForUprn/"
         )
+        uprn = kwargs.get("uprn")
+        check_uprn(uprn)
 
-        bin_data = response.json()["data"]
+        requests.packages.urllib3.disable_warnings()
+        response = requests.get(f"{api_url}{uprn}")
+        json_response = json.loads(response.content)["services"]
         data = {"bins": []}
+        collection_tuple = []
 
-        if "rows" in bin_data:
-            collection_str = bin_data["rows"][0]["DomesticBinDay"]
-
-            results = re.findall(r"(\d\d?\/\d\d?\/\d{4}) \((\w*)\)", collection_str)
-
-            if results:
-                for result in results:
-                    collection_date = datetime.strptime(result[0], "%d/%m/%Y")
-                    dict_data = {
-                        "type": result[1],
-                        "collectionDate": collection_date.strftime(date_format),
-                    }
-                    data["bins"].append(dict_data)
-
-                    # Garden waste is also collected on recycling day
-                    if dict_data["type"] == "Recycling":
-                        garden_data = {
-                            "type": "Garden",
-                            "collectionDate": dict_data["collectionDate"],
-                        }
-                        data["bins"].append(garden_data)
-            else:
-                raise RuntimeError("Dates not parsed correctly.")
-        else:
-            raise ValueError("Postcode not found on website.")
-
-        data["bins"].sort(
-            key=lambda x: datetime.strptime(x.get("collectionDate"), "%d/%m/%Y")
-        )
+        for item in json_response:
+            collection_date = datetime.strptime(
+                item.get("nextCollection"), "%Y-%m-%dT%H:%M:%S"
+            ).strftime(date_format)
+            collection_tuple.append((item.get("service"), collection_date))
+
+        ordered_data = sorted(collection_tuple, key=lambda x: x[1])
+
+        for item in ordered_data:
+            dict_data = {
+                "type": item[0],
+                "collectionDate": item[1],
+            }
+            data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/FenlandDistrictCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/FenlandDistrictCouncil.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 
 import requests
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/GlasgowCityCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/GlasgowCityCouncil.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/GuildfordCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/WiltshireCouncil.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,150 +1,119 @@
-# This script pulls (in one hit) the data from Bromley Council Bins Data
-import datetime
-import re
-import time
-from datetime import datetime
-
-import requests
 from bs4 import BeautifulSoup
-from selenium.webdriver.common.by import By
-from selenium.webdriver.common.keys import Keys
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import Select
-from selenium.webdriver.support.wait import WebDriverWait
 
 from uk_bin_collection.uk_bin_collection.common import *
 from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
 
 
-# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        driver = None
-        try:
-            uprn = kwargs.get("uprn")
-            postcode = kwargs.get("postcode")
-            full_address = kwargs.get("paon")
-
-            url = "https://my.guildford.gov.uk/customers/s/view-bin-collections"
-
-            web_driver = kwargs.get("web_driver")
-            headless = kwargs.get("headless")
-
-            driver = create_webdriver(web_driver, headless, None, __name__)
-            driver.get(kwargs.get("url"))
-
-            wait = WebDriverWait(driver, 120)
-            post_code_search = wait.until(
-                EC.presence_of_element_located(
-                    (By.XPATH, "//input[contains(@class, 'slds-input')]")
-                )
-            )
-
-            post_code_search.send_keys(postcode)
-
-            post_code_submit_btn = wait.until(
-                EC.presence_of_element_located(
-                    (By.XPATH, "//button[contains(@class,'slds-button')]")
-                )
-            )
-            post_code_submit_btn.send_keys(Keys.ENTER)
-
-            # Locate the element containing the specified address text
-            address_element = WebDriverWait(driver, 10).until(
-                EC.presence_of_element_located(
-                    (
-                        By.XPATH,
-                        f"//lightning-base-formatted-text[contains(text(), '{full_address}')]",
-                    )
-                )
-            )
+        requests.packages.urllib3.disable_warnings()
+        # Define some months to get from the calendar
+        this_month = datetime.now().month
+        this_year = datetime.now().year
+        one_month = this_month + 1
+        two_month = this_month + 2
+        months = [this_month, one_month, two_month]
+
+        # Get and check the postcode and UPRN values
+        user_postcode = kwargs.get("postcode")
+        check_postcode(user_postcode)
+        user_uprn = kwargs.get("uprn")
+        check_uprn(user_uprn)
+
+        # Some data for the request
+        cookies = {
+            'ARRAffinity': 'c5a9db7fe43cef907f06528c3d34a997365656f757206fbdf34193e2c3b6f737',
+            'ARRAffinitySameSite': 'c5a9db7fe43cef907f06528c3d34a997365656f757206fbdf34193e2c3b6f737',
+        }
+        headers = {
+            'Accept': '*/*',
+            'Accept-Language': 'en-GB,en;q=0.9',
+            'Cache-Control': 'no-cache',
+            'Connection': 'keep-alive',
+            'Content-Type': 'application/x-www-form-urlencoded; charset=UTF-8',
+            # 'Cookie': 'ARRAffinity=c5a9db7fe43cef907f06528c3d34a997365656f757206fbdf34193e2c3b6f737; ARRAffinitySameSite=c5a9db7fe43cef907f06528c3d34a997365656f757206fbdf34193e2c3b6f737',
+            'Origin': 'https://ilambassadorformsprod.azurewebsites.net',
+            'Pragma': 'no-cache',
+            'Referer': 'https://ilambassadorformsprod.azurewebsites.net/wastecollectiondays/index',
+            'Sec-Fetch-Dest': 'empty',
+            'Sec-Fetch-Mode': 'cors',
+            'Sec-Fetch-Site': 'same-origin',
+            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36 OPR/98.0.0.0',
+            'X-Requested-With': 'XMLHttpRequest',
+            'sec-ch-ua': '"Chromium";v="112", "Not_A Brand";v="24", "Opera GX";v="98"',
+            'sec-ch-ua-mobile': '?0',
+            'sec-ch-ua-platform': '"Windows"',
+        }
+
+        collections = []
+
+        # For each of the months we defined
+        for cal_month in months:
+            # If we're in Nov/Dec, the calculations won't work since its just adding one, so roll it
+            # to next year correctly
+            if cal_month == 13:
+                cal_month = 1
+                cal_year = this_year + 1
+            elif cal_month == 14:
+                cal_month = 2
+                cal_year = this_year + 1
+            else:
+                cal_year = this_year
+
+            # Data for the calendar
+            data = {
+                'Month': cal_month,
+                'Year': cal_year,
+                'Postcode': user_postcode,
+                'Uprn': user_uprn,
+            }
+
+            # Send it all as a POST
+            response = requests.post(
+                'https://ilambassadorformsprod.azurewebsites.net/wastecollectiondays/collectionlist',
+                cookies=cookies,
+                headers=headers,
+                data=data,
+            )
+
+            # If we don't get a HTTP200, throw an error
+            if response.status_code != 200:
+                raise SystemError("Error retrieving data! Please try again or raise an issue on GitHub!")
+
+            soup = BeautifulSoup(response.text, features="html.parser")
+            soup.prettify()
+
+            # Find all the bits of the current calendar that contain an event
+            events = soup.find_all("div", {"class": "rc-event-container"})
+
+            for event in events:
+                # Get the date and type of each bin collection
+                bin_date = datetime.strptime(event.find_next("a").attrs.get("data-original-datetext"), "%A %d %B, %Y")
+                bin_type = event.find_next("a").attrs.get("data-original-title")
+                # Only process it if it's today or in the future
+                if bin_date.date() >= datetime.now().date():
+                    # Split the really long type up into two separate bins
+                    if bin_type == 'Mixed dry recycling (blue lidded bin) and glass (black box or basket)':
+                        collections.append(
+                            ('Mixed dry recycling (blue lidded bin)', datetime.strftime(bin_date, date_format)))
+                        collections.append(('Glass (black box or basket)', datetime.strftime(bin_date, date_format)))
+                    else:
+                        collections.append((bin_type, datetime.strftime(bin_date, date_format)))
+
+        data = {"bins": []}
+
+        # Now there's a list of collections, yeet them into the dictionary for nice JSON
+        for item in collections:
+            dict_data = {
+                "type": item[0],
+                "collectionDate": item[1]
+            }
+            data["bins"].append(dict_data)
 
-            # Find the associated radio button in the same row (preceding sibling)
-            radio_button = address_element.find_element(
-                By.XPATH, "../../../../preceding-sibling::td//input[@type='radio']"
-            )
-
-            radio_button.send_keys(Keys.SPACE)
-            address_submit_btn = wait.until(
-                EC.presence_of_element_located(
-                    (By.XPATH, "//button[contains(@name,'NEXT')]")
-                )
-            )
-            address_submit_btn.send_keys(Keys.ENTER)
-
-            results = wait.until(
-                EC.presence_of_element_located((By.CLASS_NAME, "cBinScheduleDisplay"))
-            )
-
-            results2 = wait.until(
-                EC.presence_of_element_located(
-                    (By.XPATH, f'//div[contains(@title,"Bin Job")]')
-                )
-            )
-            soup = BeautifulSoup(driver.page_source, features="html.parser")
-            # Find all table rows containing bin information
-            rows = soup.find_all("tr", class_="slds-hint-parent")
-
-            data = {"bins": []}
-
-            # Extract bin type and next collection date for each row
-            for row in rows:
-                bin_type = (
-                    row.find("td", {"data-label": "Bin Job"})
-                    .find("strong")
-                    .text.strip()
-                    if row.find("td", {"data-label": "Bin Job"})
-                    else None
-                )
-
-                next_collection_date = (
-                    row.find("td", {"data-label": "Next Collection"}).text.strip()
-                    if row.find("td", {"data-label": "Next Collection"})
-                    else None
-                )
-
-                if bin_type and next_collection_date:
-                    # Convert date string to datetime object
-                    date_format = (
-                        "%A, %d %B"  # Adjust the format according to your date string
-                    )
-                    try:
-                        next_collection_date = datetime.strptime(
-                            next_collection_date, date_format
-                        )
-
-                        # Logic to determine year
-                        current_date = datetime.now()
-                        if next_collection_date.month < current_date.month:
-                            year = current_date.year + 1
-                        else:
-                            year = current_date.year
-
-                        # Format the date
-                        next_collection_date = next_collection_date.replace(
-                            year=year
-                        ).strftime("%d/%m/%Y")
-                    except ValueError:
-                        pass
-
-                    dict_data = {
-                        "type": bin_type,
-                        "collectionDate": next_collection_date,
-                    }
-                    data["bins"].append(dict_data)
-        except Exception as e:
-            # Here you can log the exception if needed
-            print(f"An error occurred: {e}")
-            # Optionally, re-raise the exception if you want it to propagate
-            raise
-        finally:
-            # This block ensures that the driver is closed regardless of an exception
-            if driver:
-                driver.quit()
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/HaringeyCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/MertonCouncil.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,54 @@
+# This script pulls (in one hit) the data from Merton Council Bins Data
 from bs4 import BeautifulSoup
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
+# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        data = {"bins": []}
-
-        uprn = kwargs.get("uprn")
-        check_uprn(uprn)  # Assuming check_uprn() raises an exception if UPRN is invalid
-
-        try:
-            response = requests.post(
-                f"https://wastecollections.haringey.gov.uk/property/{uprn}",
-                timeout=10,  # Set a timeout for the request
-            )
-            response.raise_for_status()  # This will raise an exception for HTTP errors
-        except requests.RequestException as e:
-            logging.error(f"Network or HTTP error occurred: {e}")
-            raise ConnectionError("Failed to retrieve data.") from e
-
-        try:
-            soup = BeautifulSoup(response.text, features="html.parser")
-            soup.prettify()
-
-            sections = soup.find_all("div", {"class": "property-service-wrapper"})
-
-            date_regex = re.compile(r"\d{2}/\d{2}/\d{4}")
-            for section in sections:
-                service_name_element = section.find("h3", {"class": "service-name"})
-                next_service_element = section.find("tbody").find(
-                    "td", {"class": "next-service"}
-                )
-
-                if service_name_element and next_service_element:
-                    service = service_name_element.text
-                    next_collection = next_service_element.find(text=date_regex)
-
-                    if next_collection:
-                        dict_data = {
-                            "type": service.replace("Collect ", "")
-                            .replace("Paid ", "")
-                            .strip(),
-                            "collectionDate": next_collection.strip(),
-                        }
-                        data["bins"].append(dict_data)
-        except Exception as e:
-            logging.error(f"Error parsing data: {e}")
-            raise ValueError("Error processing the HTML data.") from e
+        # Make a BS4 object
+        soup = BeautifulSoup(page.text, features="html.parser")
+        soup.prettify()
+
+        bin_data_dict = {"bins": []}
+
+        # Search for the specific bin in the table using BS4
+        rows = soup.find("table", class_=("collectiondays")).find_all(
+            "tr",
+            class_=(
+                "food-caddy",
+                "papercard-wheelie",
+                "plastics-boxes",
+                "rubbish-wheelie",
+                "textiles",
+                "batteries",
+            ),
+        )
+
+        # Loops the Rows
+        for row in rows:
+            # Get all the cells
+            cells = row.find_all("td")
+            # First cell is the bin_type
+            bin_type = cells[0].get_text().strip()
+            # Date is on the second cell, second paragraph, wrapped in p
+            collectionDate = cells[1].select("p > b")[2].get_text(strip=True)
+            # Make each Bin element in the JSON
+            dict_data = {
+                "bin_type": bin_type,
+                "collectionDate": datetime.strptime(
+                    collectionDate, "%d %B %Y"
+                ).strftime(date_format),
+            }
+            # # Add data to the main JSON Wrapper
+            bin_data_dict["bins"].append(dict_data)
 
-        return data
+        return bin_data_dict
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/HarrogateBoroughCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/MaldonDistrictCouncil.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,53 @@
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        user_uprn = kwargs.get("uprn")
-        check_uprn(user_uprn)
-
         data = {"bins": []}
-
-        headers = {
-            "accept-language": "en-GB,en;q=0.9",
-            "cache-control": "no-cache",
-        }
-
-        req_data = {
-            "uprn": user_uprn,
-        }
-
-        url = f"https://secure.harrogate.gov.uk/inmyarea/Property/?uprn={user_uprn}"
+        uprn = kwargs.get("uprn")
+        check_uprn(uprn)
 
         requests.packages.urllib3.disable_warnings()
-        response = requests.post(url, headers=headers)
+        response = requests.get(
+            f"https://maldon.suez.co.uk/maldon/ServiceSummary?uprn={uprn}",
+            headers={"User-Agent": "Mozilla/5.0 (Windows NT 6.1; Win64; x64)"},
+        )
+        if response.status_code != 200:
+            raise ValueError("No bin data found for provided UPRN.")
 
         soup = BeautifulSoup(response.text, features="html.parser")
-        soup.prettify()
-
-        collections = []
-
-        # Find section with bins in
-        table = soup.find_all("table", {"class": "hbcRounds"})[1]
-
-        # For each bin section, get the text and the list elements
-        for row in table.find_all("tr"):
-            bin_type = row.find("th").text
-            td = row.find("td")
-            for span in td.find_all("span"):
-                span.extract()
-            collectionDate = td.text.strip()
-            next_collection = datetime.strptime(collectionDate, "%a %d %b %Y")
-            collections.append((bin_type, next_collection))
-
-        # Sort the text and list elements by date
-        ordered_data = sorted(collections, key=lambda x: x[1])
-
-        # Put the elements into the dictionary
-        for item in ordered_data:
-            dict_data = {
-                "type": item[0],
-                "collectionDate": item[1].strftime(date_format),
-            }
-            data["bins"].append(dict_data)
+        collections = soup.find_all("div", {"class": "panel"})
+        for c in collections:
+            binType = c.find("div", {"class": "panel-heading"}).get_text(strip=True)
+            collectionDate = ""
+            rows = c.find("div", {"class": "panel-body"}).find_all(
+                "div", {"class": "row"}
+            )
+            for row in rows:
+                if row.find("strong").get_text(strip=True).lower() == "next collection":
+                    collectionDate = row.find(
+                        "div", {"class": "col-sm-9"}
+                    ).get_text(strip=True)
+
+            if collectionDate != "":
+                collection_data = {
+                    "type": binType,
+                    "collectionDate": collectionDate,
+                }
+                data["bins"].append(collection_data)
+
+        data["bins"].sort(
+            key=lambda x: datetime.strptime(x.get("collectionDate"), date_format)
+        )
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/HounslowCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NorthumberlandCouncil.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-import time
-from datetime import datetime
-
-from bs4 import BeautifulSoup
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import Select
-from selenium.webdriver.support.wait import WebDriverWait
-from selenium.webdriver.common.keys import Keys
-
-from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
-
-
-# import the wonderful Beautiful Soup and the URL grabber
-class CouncilClass(AbstractGetBinDataClass):
-    """
-    Concrete classes have to implement all abstract operations of the
-    base class. They can also override some operations with a default
-    implementation.
-    """
-
-    def parse_date(self, date_str):
-        date_formats = [
-            "This %A - %d %b %Y",  # Changed %B to %b to accommodate abbreviated month names
-            "Next %A - %d %b %Y",  # Same change here
-            "%A %d %b %Y",  # And here
-        ]
-        for format in date_formats:
-            try:
-                return datetime.strptime(date_str, format).strftime("%d/%m/%Y")
-            except ValueError:
-                continue
-        raise ValueError(f"Date format not recognized: {date_str}")
-
-    def parse_data(self, page: str, **kwargs) -> dict:
-        driver = None
-        try:
-            # Make a BS4 object
-
-            page = "https://www.hounslow.gov.uk/info/20272/recycling_and_waste_collection_day_finder"
-
-            user_postcode = kwargs.get("postcode")
-            user_uprn = kwargs.get("uprn")
-            user_paon = kwargs.get("paon")
-            web_driver = kwargs.get("web_driver")
-            headless = kwargs.get("headless")
-
-            driver = create_webdriver(web_driver, headless, None, __name__)
-            driver.get(page)
-
-            wait = WebDriverWait(driver, 60)
-
-            inputElement_postcodesearch = wait.until(
-                EC.element_to_be_clickable((By.ID, "Postcode"))
-            )
-
-            inputElement_postcodesearch.send_keys(user_postcode)
-
-            inputElement_postcodesearch_btn = wait.until(
-                EC.element_to_be_clickable((By.ID, "findAddress"))
-            )
-            inputElement_postcodesearch_btn.click()
-
-            inputElement_select_address = wait.until(
-                EC.element_to_be_clickable((By.ID, "UPRN"))
-            )
-
-            select_element = wait.until(
-                EC.visibility_of_element_located((By.ID, "UPRN"))
-            )  # Adjust this ID to your element's ID
-
-            # Create a Select object
-            select = Select(select_element)
-
-            # Fetch all options
-            options = select.options
-
-            # Loop through options to find the one that starts with the UPRN
-            for option in options:
-                if option.get_attribute("value").startswith(f"{user_uprn}|"):
-                    option.click()  # Select the matching option
-                    break
-
-            results = wait.until(
-                EC.element_to_be_clickable((By.CLASS_NAME, "bin_day_main_wrapper"))
-            )
-
-            soup = BeautifulSoup(driver.page_source, features="html.parser")
-            soup.prettify()
-
-            # Find all headers which include collection dates
-            collection_headers = soup.find_all("h4")
-            bins_data = []
-
-            # Process each collection date and corresponding bins
-            for header in collection_headers:
-                date_text = header.get_text(strip=True)
-                collection_date = self.parse_date(date_text)
-
-                # Get next sibling which should be the list of bins
-                bin_list = header.find_next_sibling("ul")
-                if bin_list:
-                    for item in bin_list.find_all("li", class_="list-group-item"):
-                        bin_type = item.get_text(strip=True)
-                        bins_data.append(
-                            {"type": bin_type, "collectionDate": collection_date}
-                        )
-
-            # Construct the final JSON object
-            json_data = {"bins": bins_data}
-
-        except Exception as e:
-            # Here you can log the exception if needed
-            print(f"An error occurred: {e}")
-            # Optionally, re-raise the exception if you want it to propagate
-            raise
-        finally:
-            # This block ensures that the driver is closed regardless of an exception
-            if driver:
-                driver.quit()
-        return json_data
+import time
+
+import requests
+from bs4 import BeautifulSoup
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from selenium.webdriver.common.keys import Keys
+from selenium.webdriver.support.ui import Select
+from uk_bin_collection.uk_bin_collection.common import *
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
+
+# import the wonderful Beautiful Soup and the URL grabber
+
+
+class CouncilClass(AbstractGetBinDataClass):
+    """
+    Concrete classes have to implement all abstract operations of the
+    base class. They can also override some operations with a default
+    implementation.
+    """
+
+    def extract_styles(self, style_str: str) -> dict:
+        return dict(
+            (a.strip(), b.strip())
+            for a, b in (
+                element.split(":") for element in style_str.split(";") if element
+            )
+        )
+
+    def parse_data(self, page: str, **kwargs) -> dict:
+        page = "https://www.northumberland.gov.uk/Waste/Bins/Bin-Calendars.aspx"
+
+        data = {"bins": []}
+
+        user_paon = kwargs.get("paon")
+        user_postcode = kwargs.get("postcode")
+        check_paon(user_paon)
+        check_postcode(user_postcode)
+
+        # Set up Selenium to run 'headless'
+        options = webdriver.ChromeOptions()
+        options.add_argument("--headless")
+        options.add_argument("--no-sandbox")
+        options.add_argument("--disable-gpu")
+        options.add_argument("--disable-dev-shm-usage")
+        options.add_experimental_option("excludeSwitches", ["enable-logging"])
+
+        # Create Selenium webdriver
+        driver = webdriver.Chrome(options=options)
+        driver.get(page)
+
+        time.sleep(1)
+
+        # Press the cookie accept - wait is to let the JS load it up
+        driver.find_element(By.ID, "ccc-notify-accept").click()
+
+        inputElement_hn = driver.find_element(
+            By.ID,
+            "p_lt_ctl04_pageplaceholder_p_lt_ctl02_WasteCollectionCalendars_NCCAddressLookup_txtHouse",
+        )
+        inputElement_pc = driver.find_element(
+            By.ID,
+            "p_lt_ctl04_pageplaceholder_p_lt_ctl02_WasteCollectionCalendars_NCCAddressLookup_txtPostcode",
+        )
+
+        inputElement_pc.send_keys(user_postcode)
+        inputElement_hn.send_keys(user_paon)
+
+        driver.find_element(
+            By.ID,
+            "p_lt_ctl04_pageplaceholder_p_lt_ctl02_WasteCollectionCalendars_NCCAddressLookup_butLookup",
+        ).click()
+
+        soup = BeautifulSoup(driver.page_source, features="html.parser")
+
+        # Work out which bins can be collected for this address. Glass bins are only on some houses due to pilot programme.
+        bins_collected = list(
+            map(
+                str.strip,
+                soup.find(
+                    "span",
+                    id="p_lt_ctl04_pageplaceholder_p_lt_ctl02_WasteCollectionCalendars_spanRouteSummary",
+                )
+                .string.replace("Routes found: ", "")
+                .split(","),
+            )
+        )
+
+        # Get the background colour for each of them...
+        bins_by_colours = dict()
+        for bin in bins_collected:
+            style_str = soup.find("span", string=bin)["style"]
+            bin_colour = self.extract_styles(style_str)["background-color"].upper()
+            bins_by_colours[bin_colour] = bin
+
+        # Work through the tables gathering the dates, if the cell has a background colour - match it to the bin type.
+        calander_tables = soup.find_all("table", title="Calendar")
+        for table in calander_tables:
+            # Get month and year
+            # First row in table is the header
+            rows = table.find_all("tr")
+            month_and_year = (
+                rows[0].find("table", class_="calCtrlTitle").find("td").string
+            )
+            bin_days = table.find_all("td", class_="calCtrlDay")
+            for day in bin_days:
+                day_styles = self.extract_styles(day["style"])
+                if "background-color" in day_styles:
+                    colour = day_styles["background-color"].upper()
+                    date = time.strptime(f"{day.string} {month_and_year}", "%d %B %Y")
+
+                    # Add it to the data
+                    data["bins"].append(
+                        {
+                            "type": bins_by_colours[colour],
+                            "collectionDate": time.strftime(date_format, date),
+                        }
+                    )
+
+        return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/HullCityCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/RushmoorCouncil.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,41 +8,42 @@
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
+        # Make a BS4 object
+        soup = BeautifulSoup(page.text, features="html.parser")
+        soup.prettify()
 
-        user_uprn = kwargs.get("uprn")
-        check_uprn(user_uprn)
         data = {"bins": []}
 
-        headers = {
-            "authority": "www.hull.gov.uk",
-            "accept": "*/*",
-            "accept-language": "en-GB,en;q=0.9",
-            "cache-control": "no-cache",
-            "pragma": "no-cache",
-            "referer": "https://www.hull.gov.uk/bins-and-recycling/bin-collections/bin-collection-day-checker",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/121.0.6167.186 Safari/537.36",
-        }
-        api_url = f"https://www.hull.gov.uk/ajax/bin-collection?bindate={user_uprn}"
-
-        res = requests.get(api_url, headers=headers)
-        if res.status_code != 200:
-            raise ConnectionRefusedError("Cannot connect to API!")
+        collections = []
+        for month in soup.find_all("div", {"class": "calendar__print"}):
+            current_month_name = month.find_next("h2").text
+            general_bins = month.find_all("li", {"class": "active-refuse day"})
+            recycling_bins = month.find_all("li", {"class": "active-recycling day"})
+            bin_list = general_bins + recycling_bins
+            for bin in bin_list:
+                if bin.attrs.get("class")[0] == "active-recycling":
+                    bin_type = "Recycling/Glass"
+                elif bin.attrs.get("class")[0] == "active-refuse":
+                    bin_type = "General waste/Garden"
+                bin_date = datetime.strptime(bin.text.strip().capitalize() + " " + current_month_name + " " +
+                                             str(datetime.now().year), '%A %d %B %Y')
+                collections.append((bin_type, bin_date))
+
+            # It'd be really hard to deal with next year, so just get December then end
+            if current_month_name == "December":
+                break
 
-        json_data = res.json()[0]
-        for item in json_data:
+        ordered_data = sorted(collections, key=lambda x: x[1])
+        data = {"bins": []}
+        for item in ordered_data:
             dict_data = {
-                "type": item.get("collection_type").capitalize(),
-                "collectionDate": datetime.strptime(
-                    item.get("next_collection_date"), "%Y-%m-%d"
-                ).strftime(date_format),
+                "type": item[0],
+                "collectionDate": item[1].strftime(date_format),
             }
             data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/HuntingdonDistrictCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/CheshireEastCouncil.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,48 @@
-#!/usr/bin/env python3
+# This script pulls (in one hit) the data from Cheshire East Council Bins Data
+import re
 
-# This script pulls (in one hit) the data from
-# Huntingdon District Council District Council Bins Data
 from bs4 import BeautifulSoup
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
-from uk_bin_collection.uk_bin_collection.common import date_format
-from datetime import datetime
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
-    def parse_data(self, page, **kwargs) -> None:
+    def parse_data(self, page: str, **kwargs) -> dict:
         # Make a BS4 object
         soup = BeautifulSoup(page.text, features="html.parser")
         soup.prettify()
 
-        data = {"bins": []}
+        bin_data_dict = {"bins": []}
 
-        no_garden_message = "Your property does not receive a garden waste collection"
-        results = soup.find("ul", class_="d-print-none").find_all("li")
+        # Search for the specific table using BS4
+        rows = soup.find("table", {"class": re.compile("job-details")}).find_all(
+            "tr", {"class": re.compile("data-row")}
+        )
+
+        # Loops the Rows
+        for row in rows:
+            cells = row.find_all(
+                "td", {"class": lambda L: L and L.startswith("visible-cell")}
+            )
+
+            labels = cells[0].find_all("label")
+            bin_type = labels[2].get_text(strip=True)
+            collectionDate = labels[1].get_text(strip=True)
+
+            # Make each Bin element in the JSON
+            dict_data = {
+                "type": bin_type,
+                "collectionDate": collectionDate,
+            }
 
-        for result in results:
-            if no_garden_message in result.get_text(strip=True):
-                continue
-            else:
-                data["bins"].append(
-                    {
-                        "type": " ".join(
-                            result.get_text(strip=True).split(" ")[5:7]
-                        ).capitalize(),
-                        "collectionDate": datetime.strptime(
-                            result.find("strong").get_text(strip=True), "%A %d %B %Y"
-                        ).strftime(date_format),
-                    }
-                )
+            # Add data to the main JSON Wrapper
+            bin_data_dict["bins"].append(dict_data)
 
-        return data
+        return bin_data_dict
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/KingstonUponThamesCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/WakefieldCityCouncil.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,104 @@
-# alternative implementation for retrieving bin data from Kingston Upon Thames Council
-# principal URL is https://waste-services.kingston.gov.uk/waste/[uprn]
-# https://www.kingston.gov.uk/info/200287/bins_and_recycling/1113/check_your_bin_collection_day
-
-# switched to using Selenium as the htmx elements are not rendered reliably with requests
-
-import re
-
+# This script pulls (in one hit) the data
+# from Warick District Council Bins Data
+import requests
 from bs4 import BeautifulSoup
-from selenium import webdriver
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import WebDriverWait
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
-    Concrete classes have to implement all abstract operations of the
-    base class. They can also override some operations with a default
+    Concrete classes have to implement all abstract operations of the base
+    class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-
-        driver = None
-        try:
-
-            headless = kwargs.get("headless")
-            web_driver = kwargs.get("web_driver")
-            driver = create_webdriver(web_driver, headless, None, __name__)
-            driver.get(kwargs.get("url"))
-            wait = WebDriverWait(driver, 15, 2)
-
-            wait.until(
-                EC.presence_of_element_located((By.CLASS_NAME, "waste-service-name"))
+        # UPRN passed in as an argument
+        user_uprn = kwargs.get("uprn")
+        check_uprn(user_uprn)
+
+        # cookies = {
+        #    'visid_incap_2049675':    'xZCc/tFgSzaFmZD7XkN3koJGuGMAAAAAQUIPAAAAAAB7QGC8d+Jmlk0i3y06Zer6',
+        #    'WSS_FullScreenMode':     'false',
+        #    'incap_ses_1184_2049675': 'a2ZQQ9lCM3wa4+23mWpuEHnAuGMAAAAAfl4ebLXAvItl6dCfbMEWoQ==',
+        # }
+        headers = {
+            "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36"
+        }
+
+        params = {
+            "uprn": user_uprn,
+        }
+
+        requests.packages.urllib3.disable_warnings()
+        s = requests.Session()  # gets cookies and keeps them
+
+        wakefield_session = s.get("https://www.wakefield.gov.uk/", headers=headers)
+        # Make a GET for the data with correct params and cookies
+        response = s.get(
+            "https://www.wakefield.gov.uk/site/Where-I-Live-Results",
+            params=params,
+            headers=headers,
+            verify=False,
+        )
+
+        # Have BS4 process the page
+        soup = BeautifulSoup(response.text, features="html.parser")
+        soup.prettify()
+        data = {"bins": []}
+
+        # Start a tuple for collections with (TYPE:DATE). Add the first for the bin types since they're separate
+        # elements on the page. All dates are parsed from text to datetime
+        collections = [
+            (
+                "Household waste",
+                datetime.strptime(
+                    soup.select(
+                        "#ctl00_PlaceHolderMain_Waste_output > div:nth-child(4) > "
+                        "div:nth-child(3) > div:nth-child(2)"
+                    )[0].text,
+                    "%d/%m/%Y",
+                ),
+            ),
+            (
+                "Mixed recycling",
+                datetime.strptime(
+                    soup.select(
+                        "#ctl00_PlaceHolderMain_Waste_output > div:nth-child(6) > "
+                        "div:nth-child(3) > div:nth-child(2)"
+                    )[0].text,
+                    "%d/%m/%Y",
+                ),
+            ),
+        ]
+
+        # Process the hidden future collection dates by adding them to the tuple
+        household_future_table = soup.find(
+            "table", {"class": "mb10 wilWasteContent RESIDUAL (D)FutureData"}
+        ).find_all("td")
+        for x in household_future_table:
+            collections.append(
+                ("Household waste", datetime.strptime(x.text, "%d/%m/%Y"))
             )
-
-            data = {"bins": []}
-
-            soup = BeautifulSoup(driver.page_source, "html.parser")
-            collections = soup.find_all("h3", {"class": "waste-service-name"})
-            for c in collections:
-                rows = c.find_next_sibling("div", {"class": "govuk-grid-row"}).find_all(
-                    "div", {"class": "govuk-summary-list__row"}
-                )
-                for row in rows:
-                    if row.find("dt").get_text().strip().lower() == "next collection":
-                        collection_date = remove_ordinal_indicator_from_date_string(
-                            row.find("dd").get_text()
-                        ).strip()
-                        # strip out any text inside of the date string
-                        collection_date = re.sub(
-                            r"\n\s*\(this.*?\)", "", collection_date
-                        )
-                        dict_data = {
-                            "type": c.get_text().strip().capitalize(),
-                            "collectionDate": get_next_occurrence_from_day_month(
-                                datetime.strptime(
-                                    collection_date
-                                    + " "
-                                    + datetime.now().strftime("%Y"),
-                                    "%A, %d %B %Y",
-                                )
-                            ).strftime(date_format),
-                        }
-                        data["bins"].append(dict_data)
-
-            data["bins"].sort(
-                key=lambda x: datetime.strptime(x.get("collectionDate"), date_format)
+        recycling_future_table = soup.find(
+            "table", {"class": "mb10 wilWasteContent RECYCLING (D)FutureData"}
+        ).find_all("td")
+        for x in recycling_future_table:
+            collections.append(
+                ("Mixed recycling", datetime.strptime(x.text, "%d/%m/%Y"))
             )
 
-        except Exception as e:
-            # Here you can log the exception if needed
-            print(f"An error occurred: {e}")
-            # Optionally, re-raise the exception if you want it to propagate
-            raise
-        finally:
-            # This block ensures that the driver is closed regardless of an exception
-            if driver:
-                driver.quit()
+        # Order the data by datetime, then add to and return it as a dictionary
+        ordered_data = sorted(collections, key=lambda x: x[1])
+        data = {"bins": []}
+        for item in ordered_data:
+            dict_data = {
+                "type": item[0],
+                "collectionDate": item[1].strftime(date_format),
+            }
+            data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/LancasterCityCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/ChelmsfordCityCouncil.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,52 @@
-from datetime import datetime
-
-import requests
 from bs4 import BeautifulSoup
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
+# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        # data to return
         data = {"bins": []}
+        headers = {"User-Agent": "Mozilla/5.0 (Windows NT 6.1; Win64; x64)"}
 
-        # start session
-        # note: this ignores the given url
-        base_url = "https://lcc-wrp.whitespacews.com"
-        session = requests.Session()
-        response = session.get(base_url + "/#!")
-        links = [
-            a["href"]
-            for a in BeautifulSoup(response.text, features="html.parser").select("a")
-        ]
-        portal_link = ""
-        for l in links:
-            if "seq=1" in l:
-                portal_link = l
-
-        # fill address form
-        response = session.get(portal_link)
-        form = BeautifulSoup(response.text, features="html.parser").find("form")
-        form_url = dict(form.attrs).get("action")
-        payload = {
-            "address_name_number": kwargs.get("number"),
-            "address_street": "",
-            "address_postcode": kwargs.get("postcode"),
-        }
-
-        # get (first) found address
-        response = session.post(form_url, data=payload)
-        links = [
-            a["href"]
-            for a in BeautifulSoup(response.text, features="html.parser").select("a")
-        ]
-        addr_link = ""
-        for l in links:
-            if "seq=3" in l:
-                addr_link = base_url + "/" + l
-
-        # get json formatted bin data for addr
-        response = session.get(addr_link)
-        new_soup = BeautifulSoup(response.text, features="html.parser")
-        services = new_soup.find("section", {"id": "scheduled-collections"})
-        services_sub = services.find_all("li")
-        for i in range(0, len(services_sub), 3):
-            dt = datetime.strptime(services_sub[i + 1].text.strip(), "%d/%m/%Y").date()
-            bin_type = BeautifulSoup(services_sub[i + 2].text, features="lxml").find(
-                "p"
-            )
-            data["bins"].append(
-                {
-                    "type": bin_type.text.strip().removesuffix(" Collection Service"),
-                    "collectionDate": dt.strftime(date_format),
-                }
-            )
+        # Make a BS4 object
+        soup = BeautifulSoup(page.text, features="html.parser")
+        soup.prettify()
+
+        # Get collection calendar
+        calendar_urls = soup.find_all("a", string=re.compile(r"view or download the collection calendar"))
+        if len(calendar_urls) > 0:
+            requests.packages.urllib3.disable_warnings()
+            response = requests.get(calendar_urls[0].get("href"), headers=headers)
+
+            # Make a BS4 object
+            soup = BeautifulSoup(response.text, features="html.parser")
+            soup.prettify()
+
+            # Loop the months
+            for month in soup.find_all("div", {"class": "usercontent"}):
+                if month.find("h2"):
+                    year = datetime.strptime(
+                        month.find("h2").get_text(strip=True), "%B %Y"
+                    ).strftime("%Y")
+                    for row in month.find_all("li"):
+                        results = re.search(
+                            "([A-Za-z]+ \\d\\d? [A-Za-z]+): (.+)", row.get_text(strip=True)
+                        )
+                        if results:
+                            dict_data = {
+                                "type": results.groups()[1].capitalize(),
+                                "collectionDate": datetime.strptime(
+                                    results.groups()[0] + " " + year, "%A %d %B %Y"
+                                ).strftime(date_format),
+                            }
+                            data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/LisburnCastlereaghCityCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/LisburnCastlereaghCityCouncil.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import difflib
 from datetime import date, datetime
 
 import requests
 from bs4 import BeautifulSoup
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
@@ -58,15 +58,15 @@
             address_by_id[address_id] = address
 
         addresses = list(address_by_id.values())
 
         common = difflib.SequenceMatcher(
             a=addresses[0], b=addresses[1]
         ).find_longest_match()
-        extra_bit = addresses[0][common.a : common.a + common.size]
+        extra_bit = addresses[0][common.a: common.a + common.size]
 
         ids_by_paon = {
             a.replace(extra_bit, ""): a_id.replace("/view/", "").replace("/", "")
             for a_id, a in address_by_id.items()
         }
 
         property_id = ids_by_paon.get(paon)
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/LiverpoolCityCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/EastRidingCouncil.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,55 @@
+import json
+from datetime import datetime
+
+import requests
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
-from dateutil.relativedelta import relativedelta
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        # Add in some variables we need
+        api_url = "https://wasterecyclingapi.eastriding.gov.uk/api/RecyclingData/CollectionsData?"
+        api_key = "APIKey=ekBWR8tSiv6qwMo31REEeTZ5FAiMNB"
+        api_license = "&Licensee=BinCollectionWebTeam"
+        postcode = kwargs.get("postcode")
+
+        # Url is built from multiple parameters
+        requests.packages.urllib3.disable_warnings()
+        response = requests.get(f"{api_url}{api_key}{api_license}&Postcode={postcode}")
+        json_response = json.loads(response.content)["dataReturned"]
         data = {"bins": []}
-        collections = []
-        curr_date = datetime.today()
-
-        # Parse the page
-        soup = BeautifulSoup(page.text, features="html.parser")
-        soup.prettify()
-
-        # Get all table rows on the page - enumerate gives us an index, which is handy for to keep a row count.
-        # In this case, the first (0th) row is headings, so we can skip it, then parse the other data.
-        for idx, row in enumerate(soup.find_all("tr")):
-            if idx == 0:
-                continue
-
-            row_type = row.find("th").text.strip()
-            row_data = row.find_all("td")
-
-            # When we get the row data, we can loop through it all and parse it to datetime. Because there are no
-            # years, we must add it in, then check if we need to overflow it to the following year.
-            for item in row_data:
-                item_text = item.text.strip()
-
-                if item_text == "Today":
-                    collections.append((row_type, curr_date))
-                elif item_text == "Tomorrow":
-                    collections.append((row_type, curr_date + relativedelta(days=1)))
-                else:
-                    bin_date = datetime.strptime(
-                        remove_ordinal_indicator_from_date_string(item_text),
-                        "%A, %d %B",
-                    ).replace(year=curr_date.year)
-
-                    if curr_date.month == 12 and bin_date.month == 1:
-                        bin_date = bin_date + relativedelta(years=1)
+        collection_tuple = []
 
-                    collections.append((row_type, bin_date))
+        # East riding seems to return the information per postcode, so we only need the first entry for the bin dates
+        collection_date = datetime.strptime(
+            json_response[0].get("BlueDate"), "%Y-%m-%dT%H:%M:%S"
+        ).strftime(date_format)
+        collection_tuple.append(("Blue Bin", collection_date))
+        collection_date = datetime.strptime(
+            json_response[0].get("GreenDate"), "%Y-%m-%dT%H:%M:%S"
+        ).strftime(date_format)
+        collection_tuple.append(("Green Bin", collection_date))
+        collection_date = datetime.strptime(
+            json_response[0].get("BrownDate"), "%Y-%m-%dT%H:%M:%S"
+        ).strftime(date_format)
+        collection_tuple.append(("Brown Bin", collection_date))
 
-        # Sort the text and list elements by date
-        ordered_data = sorted(collections, key=lambda x: x[1])
+        ordered_data = sorted(collection_tuple, key=lambda x: x[1])
 
-        # Put the elements into the dictionary
         for item in ordered_data:
             dict_data = {
                 "type": item[0],
-                "collectionDate": item[1].strftime(date_format),
+                "collectionDate": item[1],
             }
             data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/LondonBoroughHounslow.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NewarkAndSherwoodDC.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,53 @@
+from datetime import timedelta
+
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        api_url = "https://www.hounslow.gov.uk/homepage/86/recycling_and_waste_collection_day_finder"
-        user_uprn = kwargs.get("uprn")
-
-        # Check the UPRN is valid
-        check_uprn(user_uprn)
-
-        # Create the form data
-        form_data = {
-            "UPRN": user_uprn,
-        }
-
-        # Make a request to the API
-        requests.packages.urllib3.disable_warnings()
-        response = requests.post(api_url, data=form_data)
-
-        # Make a BS4 object
-        soup = BeautifulSoup(response.text, features="html.parser")
+        # Get page with BS4
+        soup = BeautifulSoup(page.text, features="html.parser")
         soup.prettify()
 
+        # Work out some date bounds
+        today = datetime.today()
+        eight_weeks = datetime.today() + timedelta(days=8 * 7)
         data = {"bins": []}
 
-        # Get the div element
-        div_element = soup.find("div", {"class": "bin_day_main_wrapper"})
-
-        # Get all bins with their corresponding dates using list comprehension
-        # This creates a list of tuples, where each tuple contains the bin type and collection date
-        bins_with_dates = [
-            (
-                bin.get_text().strip(),
-                h4.get_text().replace("This ", "").replace("Next ", ""),
-            )
-            # This first for loop iterates over each h4 element
-            for h4 in div_element.find_all("h4")
-            # This nested for loop iterates over each li element within the corresponding ul element
-            for bin in h4.find_next_sibling("ul").find_all("li")
-        ]
-
-        for bin_type, collection_date in bins_with_dates:
-            if "-" in collection_date:
-                date_part = collection_date.split(" - ")[1]
-                data["bins"].append(
-                    {
-                        "type": bin_type,
-                        "collectionDate": datetime.strptime(
-                            date_part, "%d %b %Y"
-                        ).strftime(date_format),
-                    }
+        # Each month calendar is a table, so get the object then find all rows in that object.
+        # Month and year is also a row and not included in the date, so save it then remove the row
+        for month in soup.select('table[class*="table table-condensed"]'):
+            info = month.find_all("tr")
+            month_year = info[0].text.strip()
+            info.pop(0)
+            # Each remaining item is a bin collection, so get the type and tidy up the date.
+            for item in info:
+                bin_type = item.text.split(",")[0].strip()
+                bin_date = datetime.strptime(
+                    remove_ordinal_indicator_from_date_string(
+                        item.text.split(",")[1].strip() + " " + month_year
+                    ),
+                    "%A %d %B %Y",
                 )
-            elif len(collection_date.split(" ")) == 4:
-                data["bins"].append(
-                    {
+                # Only include dates on or after today, but also only within eight weeks
+                if (
+                    today.date() <= bin_date.date() <= eight_weeks.date()
+                    and "cancelled" not in bin_type
+                ):
+                    dict_data = {
                         "type": bin_type,
-                        "collectionDate": datetime.strptime(
-                            collection_date, "%A %d %b %Y"
-                        ).strftime(date_format),
+                        "collectionDate": bin_date.strftime(date_format),
                     }
-                )
-            else:
-                data["bins"].append(
-                    {
-                        "type": bin_type,
-                        "collectionDate": datetime.strptime(
-                            collection_date, "%d %b %Y"
-                        ).strftime(date_format),
-                    }
-                )
+                    data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/MaldonDistrictCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/KingstonUponThamesCouncil.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,42 @@
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
         data = {"bins": []}
-        uprn = kwargs.get("uprn")
-        check_uprn(uprn)
 
-        requests.packages.urllib3.disable_warnings()
-        response = requests.get(
-            f"https://maldon.suez.co.uk/maldon/ServiceSummary?uprn={uprn}",
-            headers={"User-Agent": "Mozilla/5.0 (Windows NT 6.1; Win64; x64)"},
-        )
-        if response.status_code != 200:
-            raise ValueError("No bin data found for provided UPRN.")
-
-        soup = BeautifulSoup(response.text, features="html.parser")
-        collections = soup.find_all("div", {"class": "panel"})
+        soup = BeautifulSoup(page.text, features="html.parser")
+        collections = soup.find_all("h3", {"class": "waste-service-name"})
         for c in collections:
-            binType = c.find("div", {"class": "panel-heading"}).get_text(strip=True)
-            collectionDate = ""
-            rows = c.find("div", {"class": "panel-body"}).find_all(
-                "div", {"class": "row"}
+            rows = c.find_next_sibling("div", {"class": "govuk-grid-row"}).find_all(
+                "div", {"class": "govuk-summary-list__row"}
             )
             for row in rows:
-                if row.find("strong").get_text(strip=True).lower() == "next collection":
-                    collectionDate = row.find("div", {"class": "col-sm-9"}).get_text(
-                        strip=True
+                if row.find("dt").get_text().strip().lower() == "next collection":
+                    collection_date = (
+                        remove_ordinal_indicator_from_date_string(row.find("dd").get_text()).strip()
                     )
-
-            if collectionDate != "":
-                collection_data = {
-                    "type": binType,
-                    "collectionDate": collectionDate,
-                }
-                data["bins"].append(collection_data)
+                    dict_data = {
+                        "type": c.get_text().strip().capitalize(),
+                        "collectionDate": get_next_occurrence_from_day_month(datetime.strptime(
+                            collection_date + " " + datetime.now().strftime("%Y"),
+                            "%A, %d %B %Y",
+                        )).strftime(date_format),
+                    }
+                    data["bins"].append(dict_data)
 
         data["bins"].sort(
             key=lambda x: datetime.strptime(x.get("collectionDate"), date_format)
         )
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/MalvernHillsDC.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SwaleBoroughCouncil.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,53 @@
+import requests
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
+
+
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        api_url = "https://swict.malvernhills.gov.uk/mhdcroundlookup/HandleSearchScreen"
-
+        # Get postcode and UPRN from kwargs
+        user_postcode = kwargs.get("postcode")
         user_uprn = kwargs.get("uprn")
-        # Check the UPRN is valid
+        check_postcode(user_postcode)
         check_uprn(user_uprn)
 
-        # Create the form data
-        form_data = {"nmalAddrtxt": "", "alAddrsel": user_uprn}
-        # expects postcode to be looked up and then uprn used.
-        # we can just provide uprn
+        # Build URL to parse
+        council_url = f"https://swale.gov.uk/bins-littering-and-the-environment/bins/collection-days?postcode={user_postcode.replace(' ', '+')}&addresses={user_uprn}&address-submit="
 
-        # Make a request to the API
+        # Parse URL and read if connection successful
         requests.packages.urllib3.disable_warnings()
-        response = requests.post(api_url, data=form_data, verify=False)
-
-        # Make a BS4 object
-        soup = BeautifulSoup(response.text, features="html.parser")
-        soup.prettify()
-
-        # Find results table
-        table_element = soup.find("table")
-        table_body = table_element.find("tbody")
-        rows = table_body.find_all("tr")
+        response = requests.get(council_url)
+        if response.status_code == 200:
+            soup = BeautifulSoup(response.text, features="html.parser")
+            soup.prettify()
+        else:
+            raise ConnectionAbortedError("Could not parse council website.")
 
         data = {"bins": []}
 
-        for row in rows:
-            columns = row.find_all("td")
-            columns = [ele.text.strip() for ele in columns]
-
-            thisCollection = [ele for ele in columns if ele]  # Get rid of empty values
-
-            # if not signed up for garden waste, this appears as Not applicable
-            if "Not applicable" not in thisCollection[1]:
-                bin_type = thisCollection[0].replace("collection", "").strip()
-                date = datetime.strptime(thisCollection[1], "%A %d/%m/%Y")
-                dict_data = {
-                    "type": bin_type,
-                    "collectionDate": date.strftime(date_format),
-                }
-                data["bins"].append(dict_data)
+        # Get the collection bullet points on the page and parse them
+        form_area = soup.find("form", {"class": "integration bin-lookup"})
+        collections = [
+            item.text.strip().split(",") for item in form_area.find_all("li")
+        ]
+        for c in collections:
+            bin_type = c[0].strip()
+            # temp_date = c[2].strip() + " " + str(datetime.now().year)
+            bin_date = datetime.strptime(
+                c[2].strip() + " " + str(datetime.now().year), "%d %B %Y"
+            ).strftime(date_format)
+            dict_data = {"type": bin_type, "collectionDate": bin_date}
+            data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ManchesterCityCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/ManchesterCityCouncil.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 
 import requests
 from bs4 import BeautifulSoup
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
@@ -17,36 +17,36 @@
     def parse_data(self, page: str, **kwargs) -> dict:
         # Get and check UPRN
         user_uprn = kwargs.get("uprn")
         check_uprn(user_uprn)
 
         # Start a new session to walk through the form
         requests.packages.urllib3.disable_warnings()
-        s = requests.Session()
+        s = requests.session()
 
         # There's a cookie that makes the whole thing valid when you search for a postcode,
         # but postcode and UPRN is a hassle imo, so this makes a request for the session to get a cookie
         # using a Manchester City Council postcode I hardcoded in the data payload
         postcode_request_header = {
             "authority": "www.manchester.gov.uk",
             "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,"
-            "image/webp,image/apng,*/*;q=0.8",
+                      "image/webp,image/apng,*/*;q=0.8",
             "accept-language": "en-GB,en;q=0.6",
             "cache-control": "max-age=0",
             # Requests sorts cookies= alphabetically
             "origin": "https://www.manchester.gov.uk",
             "referer": "https://www.manchester.gov.uk/bincollections",
             "sec-fetch-dest": "document",
             "sec-fetch-mode": "navigate",
             "sec-fetch-site": "same-origin",
             "sec-fetch-user": "?1",
             "sec-gpc": "1",
             "upgrade-insecure-requests": "1",
             "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, "
-            "like Gecko) Chrome/104.0.5112.102 Safari/537.36",
+                          "like Gecko) Chrome/104.0.5112.102 Safari/537.36",
         }
         postcode_request_data = {
             "mcc_bin_dates_search_term": "M2 5DB",
             "mcc_bin_dates_submit": "Go",
         }
         response = s.post(
             "https://www.manchester.gov.uk/bincollections",
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/MansfieldDistrictCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/HuntingdonDistrictCouncil.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-import requests
+#!/usr/bin/env python3
 
+# This script pulls (in one hit) the data from
+# Huntingdon District Council District Council Bins Data
 from bs4 import BeautifulSoup
-from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
-    def parse_data(self, page: str, **kwargs) -> dict:
-        user_uprn = kwargs.get("uprn")
-        check_uprn(user_uprn)
+    def parse_data(self, page, **kwargs) -> None:
+        # Make a BS4 object
+        soup = BeautifulSoup(page.text, features="html.parser")
+        soup.prettify()
 
         data = {"bins": []}
-        api_url = f'https://portal.mansfield.gov.uk/MDCWhiteSpaceWebService/WhiteSpaceWS.asmx/GetCollectionByUPRNAndDate?apiKey=mDc-wN3-B0f-f4P&UPRN={user_uprn}&coldate={datetime.now().strftime("%d/%m/%Y")}'
 
-        response = requests.get(api_url)
-        if response.status_code != 200:
-            raise ConnectionError("Could not get latest data!")
-
-        json_data = response.json()["Collections"]
-        for item in json_data:
-
-            dict_data = {
-                "type": item.get("Service").split(" ")[0] + " bin",
-                "collectionDate": datetime.strptime(
-                    item.get("Date"), "%d/%m/%Y %H:%M:%S"
-                ).strftime(date_format),
-            }
-            data["bins"].append(dict_data)
+        bin_types = ["Domestic", "Recycle", "Organic"]
+
+        for i, date in enumerate(soup.find("ul", class_="d-print-none").find_all("li")):
+            data["bins"].append(
+                {
+                    "type": bin_types[i],
+                    "collectionDate": date.find("strong").get_text(strip=True),
+                }
+            )
+            ++i
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/MertonCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/BasingstokeCouncil.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-# This script pulls (in one hit) the data from Merton Council Bins Data
 from bs4 import BeautifulSoup
+from datetime import datetime
+import requests
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
+
+COLLECTION_KINDS = {
+    "waste": "rteelem_ctl03_pnlCollections_Refuse",
+    "recycling": "rteelem_ctl03_pnlCollections_Recycling",
+    "glass": "rteelem_ctl03_pnlCollections_Glass",
+    # Garden waste data is only returned if the property is subscribed to the Garden Waste service
+    "garden": "rteelem_ctl03_pnlCollections_GardenWaste"
+}
 
 
-# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
-    """
-    Concrete classes have to implement all abstract operations of the
-    base class. They can also override some operations with a default
-    implementation.
-    """
 
-    def parse_data(self, page: str, **kwargs) -> dict:
-        # Make a BS4 object
-        soup = BeautifulSoup(page.text, features="html.parser")
-        soup.prettify()
+    def get_data(self, address_url):
+        # Unused, we need the uprn!
+        return None
 
-        data = {"bins": []}
-        collections = []
+    def parse_data(self, page: str, **kwargs) -> dict:
+        user_uprn = kwargs.get("uprn")
+        check_uprn(user_uprn)
 
-        # Search for the specific bin in the table using BS4
-        rows = soup.find("table", class_=("collectiondays")).find_all(
-            "tr",
-            class_=(
-                "food-caddy",
-                "papercard-wheelie",
-                "plastics-boxes",
-                "rubbish-wheelie",
-                "textiles",
-                "batteries",
-            ),
+        request_headers = {
+            "cookie": f"WhenAreMyBinsCollected={user_uprn}"
+        }
+        requests.packages.urllib3.disable_warnings()
+        response = requests.get(
+            "https://www.basingstoke.gov.uk/bincollections",
+            headers=request_headers,
         )
 
-        # Loops the Rows
-        for row in rows:
-            # Get all the cells
-            cells = row.find_all("td")
-            # First cell is the bin_type
-            bin_type = cells[0].get_text().strip()
-            # Date is on the second cell, second paragraph, wrapped in p
-            collectionDate = datetime.strptime(
-                cells[1].select("p > b")[2].get_text(strip=True), "%d %B %Y"
-            )
-
-            # Add each collection to the list as a tuple
-            collections.append((bin_type, collectionDate))
-
-        ordered_data = sorted(collections, key=lambda x: x[1])
-        for item in ordered_data:
-            dict_data = {
-                "type": item[0].capitalize(),
-                "collectionDate": item[1].strftime(date_format),
-            }
-            data["bins"].append(dict_data)
+        if response.status_code != 200:
+            raise SystemError("Error retrieving data! Please try again or raise an issue on GitHub!")
+
+        # Make a BS4 object
+        soup = BeautifulSoup(response.text, features="html.parser")
+        soup.prettify()
+
+        bins = []
 
-        return data
+        for collection_type, collection_class in COLLECTION_KINDS.items():
+            for date in soup.select(f"div#{collection_class} li"):
+                bins.append({
+                    "type": collection_type,
+                    "collectionDate": datetime.strptime(
+                        # Friday, 21 July 2023
+                        date.get_text(strip=True),
+                        '%A, %d %B %Y'
+                    ).strftime(date_format)
+                })
+
+        return {
+            "bins": bins
+        }
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/MidSussexDistrictCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/MidSussexDistrictCouncil.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 from datetime import datetime
 
 import requests
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 def get_token(res) -> str:
     """
     Get a UFPRT code for the form data to be processed
         :param res:
         :return:
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/MiltonKeynesCityCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/MiltonKeynesCityCouncil.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NewarkAndSherwoodDC.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/RochdaleCouncil.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,68 @@
-from datetime import timedelta
-
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        # Get page with BS4
-        soup = BeautifulSoup(page.text, features="html.parser")
+        api_url = "https://webforms.rochdale.gov.uk/BinCalendar"
+        user_postcode = kwargs.get("postcode")
+        user_uprn = kwargs.get("uprn")
+
+        # Check the postcode and UPRN are valid
+        check_postcode(user_postcode)
+        check_uprn(user_uprn)
+
+        # Create the form data
+        form_data = {
+            "PostCode": user_postcode,
+            "SelectedUprn": user_uprn,
+            "Step": 2,
+        }
+
+        # Make a request to the API
+        requests.packages.urllib3.disable_warnings()
+        response = requests.post(api_url, data=form_data)
+
+        # Make a BS4 object
+        soup = BeautifulSoup(response.text, features="html.parser")
         soup.prettify()
 
-        # Work out some date bounds
-        today = datetime.today()
-        eight_weeks = datetime.today() + timedelta(days=8 * 7)
         data = {"bins": []}
 
-        # Each month calendar is a table, so get the object then find all rows in that object.
-        # Month and year is also a row and not included in the date, so save it then remove the row
-        for month in soup.select('table[class*="table table-condensed"]'):
-            info = month.find_all("tr")
-            month_year = info[0].text.strip()
-            info.pop(0)
-            # Each remaining item is a bin collection, so get the type and tidy up the date.
-            for item in info:
-                bin_type = item.text.split(",")[0].strip()
-                bin_date = datetime.strptime(
-                    remove_ordinal_indicator_from_date_string(
-                        item.text.split(",")[1].strip() + " " + month_year
-                    ),
-                    "%A %d %B %Y",
-                )
-                # Only include dates on or after today, but also only within eight weeks
-                if (
-                    today.date() <= bin_date.date() <= eight_weeks.date()
-                    and "cancelled" not in bin_type
-                ):
-                    dict_data = {
-                        "type": bin_type,
-                        "collectionDate": bin_date.strftime(date_format),
-                    }
-                    data["bins"].append(dict_data)
+        # Get the table element and rows
+        table_element = soup.find("table", {"id": "tblCollectionDetails"})
+        table_rows = table_element.find_all_next("tr")
+
+        row_index = 0
+        for row in table_rows:
+            if row_index < 1:
+                row_index += 1
+                continue
+            else:
+                # Get the date from the th element
+                date = datetime.strptime(row.find("th").get_text().strip(), "%A %d %B %Y").strftime(date_format)
+
+                # Get the bin types from the td elements and filter out the empty ones
+                bin_types = filter(lambda td: td.find("img"), row.find_all("td"))
+
+                # Convert the bin types to a list
+                bin_types_list = list(bin_types)
+
+                # Append the bin type and date to the data dict
+                for td in bin_types_list:
+                    img = td.find("img")
+                    bin_type_text = img["alt"]
+                    data["bins"].append({"type": bin_type_text, "collectionDate": date})
+
+                row_index += 1
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NewcastleCityCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NewcastleCityCouncil.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 # This script pulls (in one hit) the data from
 # Newcastle City Council Bins Data
 from datetime import datetime
 
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import date_format
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
@@ -26,29 +27,24 @@
 
         for element in soup.find_all("strong"):
             collectionInfo = ""
             # Domestic Waste is formatted differently to other bins
             if "Green Bin (Domestic Waste) details:" in str(element):
                 if element.next_sibling.find("br"):
                     collectionInfo = element.next_sibling.find("br").next_element
-            elif "Next collection" in str(
-                element.next_sibling.next_sibling.next_sibling.next_sibling
-            ):
+            elif "Next collection" in str(element.next_sibling.next_sibling.next_sibling.next_sibling):
                 collectionInfo = (
                     element.next_sibling.next_sibling.next_sibling.next_sibling
                 )
 
             if collectionInfo != "" and collectionInfo != "Next collection : n/a":
-                bin_type = str(element)[
-                    str(element).find("(") + 1 : str(element).find(")")
-                ]
+                bin_type = str(element)[str(element).find("(") + 1: str(element).find(")")]
                 collectionDate = str(
                     datetime.strptime(
-                        str(collectionInfo).replace("Next collection : ", ""),
-                        "%d-%b-%Y",
+                        str(collectionInfo).replace("Next collection : ", ""), "%d-%b-%Y"
                     )
                     .date()
                     .strftime(date_format)
                 )
 
                 dict_data = {"type": bin_type, "collectionDate": collectionDate}
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NewhamCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/WealdenDistrictCouncil.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,87 @@
-import urllib3
-from bs4 import BeautifulSoup
+import json
 
+import requests
+from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
+# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        # get the page data
-        request = urllib3.request(method="get", url=kwargs["url"])
-        page_data = request.data
-
-        # Make a BS4 object
-        soup = BeautifulSoup(page_data, features="html.parser")
-        soup.prettify()
+        user_uprn = kwargs.get("uprn")
+        check_uprn(user_uprn)
 
-        # Form a JSON wrapper
-        data = {"bins": []}
+        headers = {
+            "authority": "www.wealden.gov.uk",
+            "accept": "*/*",
+            "accept-language": "en-GB,en;q=0.7",
+            "content-type": "application/x-www-form-urlencoded; charset=UTF-8",
+            # Requests sorts cookies= alphabetically
+            # 'cookie': 'ARRAffinity=e45c20b343b490e3866d5d35c3dbda687e4a1357c2163c32922209862abb5872; ARRAffinitySameSite=e45c20b343b490e3866d5d35c3dbda687e4a1357c2163c32922209862abb5872',
+            "origin": "https://www.wealden.gov.uk",
+            "referer": "https://www.wealden.gov.uk/recycling-and-waste/bin-search/?uprn=10033413624",
+            "sec-fetch-dest": "empty",
+            "sec-fetch-mode": "cors",
+            "sec-fetch-site": "same-origin",
+            "sec-gpc": "1",
+            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/107.0.0.0 Safari/537.36",
+            "x-requested-with": "XMLHttpRequest",
+        }
+
+        data = {
+            "action": "wealden_get_collections_for_uprn",
+            "uprn": user_uprn,
+        }
+
+        requests.packages.urllib3.disable_warnings()
+        response = requests.post(
+            "https://www.wealden.gov.uk/wp-admin/admin-ajax.php",
+            headers=headers,
+            data=data,
+        )
+        json_data = json.loads(response.text)
 
-        # Find section with bins in
-        sections = soup.find_all("div", {"class": "card h-100"})
+        if json_data["status"] != "success":
+            raise ValueError("Error parsing data. Please open an issue on GitHub.")
 
-        # there may also be a recycling one too
-        sections_recycling = soup.find_all(
-            "div", {"class": "card h-100 card-recycling"}
-        )
-        if len(sections_recycling) > 0:
-            sections.append(sections_recycling[0])
+        property_data = json_data["collection"]
+        data = {"bins": []}
+        collections = []
 
-        # For each bin section, get the text and the list elements
-        for item in sections:
-            header = item.find("div", {"class": "card-header"})
-            bin_type_element = header.find_next("b")
-            if bin_type_element is not None:
-                bin_type = bin_type_element.text
-                array_expected_types = ["Domestic", "Recycling"]
-                if bin_type in array_expected_types:
-                    date = (
-                        item.find_next("p", {"class": "card-text"})
-                        .find_next("mark")
-                        .next_sibling.strip()
-                    )
-                    next_collection = datetime.strptime(date, "%d/%m/%Y")
-
-                    dict_data = {
-                        "type": bin_type,
-                        "collectionDate": next_collection.strftime(date_format),
-                    }
-                    data["bins"].append(dict_data)
+        if len(property_data["refuseCollectionDate"]) > 0:
+            bin_type = "Rubbish Bin"
+            bin_date = datetime.strptime(
+                property_data["refuseCollectionDate"], "%Y-%m-%dT%H:%M:%S"
+            )
+            collections.append((bin_type, bin_date))
+        if len(property_data["recyclingCollectionDate"]) > 0:
+            bin_type = "Recycling Bin"
+            bin_date = datetime.strptime(
+                property_data["recyclingCollectionDate"], "%Y-%m-%dT%H:%M:%S"
+            )
+            collections.append((bin_type, bin_date))
+        if len(property_data["gardenCollectionDate"]) > 0:
+            bin_type = "Garden Bin"
+            bin_date = datetime.strptime(
+                property_data["gardenCollectionDate"], "%Y-%m-%dT%H:%M:%S"
+            )
+            collections.append((bin_type, bin_date))
+
+        ordered_data = sorted(collections, key=lambda x: x[1])
+        data = {"bins": []}
+        for item in ordered_data:
+            dict_data = {
+                "type": item[0],
+                "collectionDate": item[1].strftime(date_format),
+            }
+            data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NewportCityCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SomersetCouncil.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from bs4 import BeautifulSoup
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
@@ -16,25 +16,25 @@
         user_postcode = kwargs.get("postcode")
         check_postcode(user_postcode)
         user_uprn = kwargs.get("uprn")
         check_uprn(user_uprn)
 
         headers = {
             "User-Agent": "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) "
-            "Chrome/87.0.4280.141 Safari/537.36"
+                          "Chrome/87.0.4280.141 Safari/537.36"
         }
 
         requests.packages.urllib3.disable_warnings()
         with requests.Session() as s:
             # Set Headers
             s.headers = headers
 
             # Get the first page - This is the Search for property by Post Code page
             resource = s.get(
-                "https://iweb.itouchvision.com/portal/f?p=customer:BIN_DAYS:::NO:RP:UID:6CDD2A34C912312074D8E2410531401A8C00EFF7"
+                "https://iweb.itouchvision.com/portal/f?p=customer:BIN_DAYS:::NO:RP:UID:625C791B4D9301137723E9095361401AE8C03934"
             )
             # Create a BeautifulSoup object from the page's HTML
             soup = BeautifulSoup(resource.text, "html.parser")
 
             # The page contains a number of values that must be passed into subsequent requests - extract them here
             payload = {
                 i["name"]: i.get("value", "") for i in soup.select("input[name]")
@@ -92,15 +92,15 @@
             }
             json_object = json.dumps(json_builder, separators=(",", ":"))
             other_list["p_json"] = json_object
 
             # Set Referrer header
             s.headers.update(
                 {
-                    "referer": "https://iweb.itouchvision.com/portal/f?p=customer:BIN_DAYS:::NO:RP:UID:6CDD2A34C912312074D8E2410531401A8C00EFF7"
+                    "referer": "https://iweb.itouchvision.com/portal/f?p=customer:BIN_DAYS:::NO:RP:UID:625C791B4D9301137723E9095361401AE8C03934"
                 }
             )
 
             # Generate POST including all the JSON we just built
             s.post(
                 "https://iweb.itouchvision.com/portal/wwv_flow.accept", data=other_list
             )
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NorthEastLincs.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/StockportBoroughCouncil.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,38 @@
-import pandas as pd
+# This script pulls (in one hit) the
+# data from Warick District Council Bins Data
 from bs4 import BeautifulSoup
-from uk_bin_collection.uk_bin_collection.common import date_format
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.common import *
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
+# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
-    baseclass. They can also override some
-    operations with a default implementation.
+    base class. They can also override some operations with a default
+    implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
         # Make a BS4 object
         soup = BeautifulSoup(page.text, features="html.parser")
         soup.prettify()
 
         data = {"bins": []}
 
-        # Get list items that can be seen on page
-        for element in soup.find_all(
-            "li", {"class": "list-group-item p-0 p-3 bin-collection-item"}
-        ):
-            element_text = element.text.strip().split("\n\n")
-            element_text = [x.strip() for x in element_text]
-
-            bin_type = element_text[1]
-            collection_date = pd.Timestamp(element_text[0]).strftime(date_format)
-
-            dict_data = {
-                "type": bin_type,
-                "collectionDate": collection_date,
-            }
-            data["bins"].append(dict_data)
-
-        # Get hidden list items too
-        for element in soup.find_all(
-            "li", {"class": "list-group-item p-0 p-3 bin-collection-item d-none"}
-        ):
-            element_text = element.text.strip().split("\n\n")
-            element_text = [x.strip() for x in element_text]
-
-            bin_type = element_text[1]
-            collection_date = pd.Timestamp(element_text[0]).strftime(date_format)
-
-            dict_data = {
-                "type": bin_type,
-                "collectionDate": collection_date,
-            }
-            data["bins"].append(dict_data)
+        for bins in soup.select('div[class*="service-item"]'):
+            bin_type = bins.div.h3.text.strip()
+            binCollection = datetime.strptime(bins.select("div > p")[1].get_text(strip=True), "%A, %d %B %Y")
+            # binImage = "https://myaccount.stockport.gov.uk" + bins.img['src']
+
+            # batteries don't have a service date or other
+            # info associated with them.
+            if binCollection:
+                dict_data = {
+                    "type": bin_type,
+                    "collectionDate": binCollection.strftime(date_format)
+                }
+                data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NorthKestevenDistrictCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SouthLanarkshireCouncil.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,79 @@
+import time
+from datetime import timedelta
+
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
+        data = {"bins": []}
+        collection_types = [
+            "non recyclable waste",
+            "food and garden",
+            "paper and card",
+            "glass, cans and plastics",
+        ]
+
         # Make a BS4 object
         soup = BeautifulSoup(page.text, features="html.parser")
         soup.prettify()
 
-        data = {"bins": []}
-
-        for bins in soup.find_all(
-            "div", {"class": lambda L: L and L.startswith("bg-")}
-        ):
-            for bin in bins.find_all("p"):
-                if bin.find("strong"):
-                    results = re.search(
-                        "Next Collection:(.*?) on ([A-Za-z]+, \\d\\d? [A-Za-z]+ \\d{4})",
-                        bin.find("strong").get_text(strip=True),
-                    )
-                    if results:
-                        collection_date = datetime.strptime(
-                            results.groups()[1], "%A, %d %B %Y"
-                        )
-                        data["bins"].append(
-                            {
-                                "type": bins.h3.get_text(strip=True),
-                                "collectionDate": collection_date.strftime(date_format),
-                            }
-                        )
+        week_details = soup.find("div", {"class": "bin-dir-snip"})
+        week_dates = week_details.find("div", {"class": "clearfix"}).find("p")
+        week_collections = week_details.find_all_next("h4")
 
-        data["bins"].sort(
-            key=lambda x: datetime.strptime(x.get("collectionDate"), date_format)
+        results = re.search(
+            "([A-Za-z0-9 ]+) to ([A-Za-z0-9 ]+)", week_dates.get_text().strip()
         )
+        if results:
+            week_start = datetime.strptime(results.groups()[0], "%A %d %B %Y")
+            week_end = datetime.strptime(results.groups()[1], "%A %d %B %Y")
+            week_days = (
+                week_start + timedelta(days=i)
+                for i in range((week_end - week_start).days + 1)
+            )
+
+            week_collection_types = []
+            for week_collection in week_collections:
+                week_collection = (
+                    week_collection.get_text().strip().lower().replace("-", " ")
+                )
+                for collection_type in collection_types:
+                    if collection_type in week_collection:
+                        week_collection_types.append(collection_type)
+
+            collection_schedule = (
+                soup.find("div", {"class": "serviceDetails"})
+                .find("table")
+                .find_all_next("tr")
+            )
+
+            for day in week_days:
+                for row in collection_schedule:
+                    schedule_type = row.find("th").get_text().strip()
+                    results2 = re.search("([^(]+)", row.find("td").get_text().strip())
+                    if results2:
+                        schedule_day = results2[1].strip()
+                        for collection_type in week_collection_types:
+                            if collection_type in schedule_type.lower():
+                                if (
+                                    day.weekday()
+                                    == time.strptime(schedule_day, "%A").tm_wday
+                                ):
+                                    dict_data = {
+                                        "type": schedule_type,
+                                        "collectionDate": day.strftime(date_format),
+                                    }
+                                    data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NorthLincolnshireCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NorthLincolnshireCouncil.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
@@ -32,27 +33,25 @@
         requests.packages.urllib3.disable_warnings()
         response = requests.get(
             f"https://m.northlincs.gov.uk/bin_collections?no_collections=20&uprn={uprn}",
             headers=headers,
         )
         if response.status_code != 200:
             raise ValueError("No bin data found for provided UPRN.")
-        json_data = json.loads(response.text.encode().decode("utf-8-sig"))
+        json_data = json.loads(response.text.encode().decode('utf-8-sig'))
 
         data = {"bins": []}
         for c in json_data["Collections"]:
             bin_type = c["BinCodeDescription"].strip()
             if bin_type.lower() != "textiles bag":
                 dict_data = {
                     "type": bin_type,
-                    "collectionDate": get_next_occurrence_from_day_month(
-                        datetime.strptime(
-                            c["BinCollectionDate"].replace(" (*)", "").strip()
-                            + " "
-                            + datetime.now().strftime("%Y"),
-                            "%A %d %B %Y",
-                        )
-                    ).strftime(date_format),
+                    "collectionDate": get_next_occurrence_from_day_month(datetime.strptime(
+                        c["BinCollectionDate"].replace(" (*)", "").strip()
+                        + " "
+                        + datetime.now().strftime("%Y"),
+                        "%A %d %B %Y",
+                    )).strftime(date_format),
                 }
                 data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NorthSomersetCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SalfordCityCouncil.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,71 @@
+from datetime import datetime
+
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
+# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        api_url = "https://forms.n-somerset.gov.uk/Waste/CollectionSchedule"
-        uprn = kwargs.get("uprn")
-        postcode = kwargs.get("postcode")
-        check_uprn(uprn)
-        check_postcode(postcode)
-
-        # Get schedule from API
-        values = {
-            "PreviousHouse": "",
-            "PreviousPostcode": postcode,
-            "Postcode": postcode,
-            "SelectedUprn": uprn,
+        api_url = "https://www.salford.gov.uk/bins-and-recycling/bin-collection-days/your-bin-collections"
+        user_uprn = kwargs.get("uprn")
+
+        # Check the UPRN is valid
+        check_uprn(user_uprn)
+
+        # Create the form data
+        params = {
+            "UPRN": user_uprn,
         }
-        headers = {"User-Agent": "Mozilla/5.0 (Windows NT 6.1; Win64; x64)"}
+
+        # Make a request to the API
         requests.packages.urllib3.disable_warnings()
-        response = requests.request("POST", api_url, headers=headers, data=values)
+        response = requests.get(api_url, params=params)
 
+        # Make a BS4 object
         soup = BeautifulSoup(response.text, features="html.parser")
+        soup.prettify()
 
-        rows = soup.find("table", {"class": re.compile("table")}).find_all("tr")
-
-        # Form a JSON wrapper
         data = {"bins": []}
 
-        # Loops the Rows
-        for row in rows:
-            cells = row.find_all("td")
-            if cells:
-                binType = cells[0].get_text(strip=True)
-                collectionDate = (
-                    cells[1].get_text(strip=True) + " " + datetime.now().strftime("%Y")
-                )
-                nextCollectionDate = (
-                    cells[2].get_text(strip=True) + " " + datetime.now().strftime("%Y")
+        # Get the div element
+        div_element = soup.find("div", {"class": "wastefurther"})
+
+        # Get the bins
+        bin_lists = div_element.find_all("ul")
+
+        # Loop through each <ul> tag to extract the bin information
+        for i, bin_list in enumerate(bin_lists):
+            # Find the <p> tag containing the bin type string
+            bin_type = bin_list.find_previous_sibling("p").find("strong").text.strip()
+
+            # Loop through each <li> tag in the <ul> tag to extract the collection date
+            for li in bin_list.find_all("li"):
+                # Convert the collection time to a datetime object
+                collection_time = datetime.strptime(li.text, "%A %d %B %Y")
+
+                # Add the bin to the data dict
+                data["bins"].append(
+                    {
+                        # remove the ":" from the end of the bin type
+                        "type": bin_type[:-1],
+                        "collectionTime": collection_time,
+                    }
                 )
 
-                # Make each Bin element in the JSON
-                dict_data = {
-                    "type": binType,
-                    "collectionDate": get_next_occurrence_from_day_month(
-                        datetime.strptime(collectionDate, "%A %d %B %Y")
-                    ).strftime(date_format),
-                }
-
-                # Add data to the main JSON Wrapper
-                data["bins"].append(dict_data)
-
-                # Make each next Bin element in the JSON
-                dict_data = {
-                    "type": binType,
-                    "collectionDate": get_next_occurrence_from_day_month(
-                        datetime.strptime(nextCollectionDate, "%A %d %B %Y")
-                    ).strftime(date_format),
-                }
-
-                # Add data to the main JSON Wrapper
-                data["bins"].append(dict_data)
-
-        data["bins"].sort(
-            key=lambda x: datetime.strptime(x.get("collectionDate"), date_format)
-        )
+        # Sort the bins by collection time
+        data["bins"] = sorted(data["bins"], key=lambda x: x["collectionTime"])
+
+        # Convert the datetime objects to strings in the desired format
+        for bin in data["bins"]:
+            bin["collectionTime"] = bin["collectionTime"].strftime(date_format)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NorthTynesideCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/NorthTynesideCouncil.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 from datetime import *
 
 import requests
 from bs4 import BeautifulSoup
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
@@ -21,19 +21,19 @@
         data = {"bins": []}
         user_uprn = kwargs.get("uprn")
         user_postcode = kwargs.get("postcode")
         check_uprn(user_uprn)
         check_postcode(user_postcode)
 
         # Get form data
-        s = requests.Session()
+        s = requests.session()
         cookies = {
-            "ntc-cookie-policy": "1",
-            "SSESS6ec6d5d2d471c0357053d5993a839bce": "qBdR7XhmSMd5_PDBIqG0It2R0Fq67igrejRY-WOcskE",
             "has_js": "1",
+            "SSESS6ec6d5d2d471c0357053d5993a839bce": "nDJusnUyqrl2rk8LaiyDv3VaLUwSadRLGLPUpG2e2PY",
+            "ntc-cookie-policy": "1",
         }
         headers = {
             "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8",
             "Accept-Language": "en-GB,en;q=0.7",
             "Cache-Control": "max-age=0",
             "Connection": "keep-alive",
             "Origin": "https://my.northtyneside.gov.uk",
@@ -47,15 +47,15 @@
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36",
             "sec-ch-ua": '"Not?A_Brand";v="8", "Chromium";v="108", "Brave";v="108"',
             "sec-ch-ua-mobile": "?0",
             "sec-ch-ua-platform": '"Windows"',
         }
         ajax_data = {
             "postcode": user_postcode,
-            "form_build_id": "form-BQ47tM0NKADE0s8toYkdSef3QBn6lDM-yBseqIOho80",
+            "form_build_id": "form-O65oY-ly-CYJlnQrhohK2uS1OP-4vXsS3CqYXD7-BeM",
             "form_id": "ntc_address_wizard",
             "_triggering_element_name": "op",
             "_triggering_element_value": "Find",
             "ajax_html_ids[]": [
                 "ntc-web-my",
                 "skip-link",
                 "navbar",
@@ -74,15 +74,15 @@
                 "wizard-form-wrapper",
                 "ntc-address-wizard",
                 "edit-postcode",
                 "edit-find",
                 "backtotop",
             ],
             "ajax_page_state[theme]": "ntc_bootstrap",
-            "ajax_page_state[theme_token]": "LN05JIzI6rocWDiBpDyVeywYveuS4jlxD_N0_hhp2Ko",
+            "ajax_page_state[theme_token]": "sAhZZMhTYHnHhQ1H7ruHKsid2GUGRRHlLQKP0RFrotA",
             "ajax_page_state[css][0]": "1",
             "ajax_page_state[css][modules/system/system.base.css]": "1",
             "ajax_page_state[css][misc/ui/jquery.ui.core.css]": "1",
             "ajax_page_state[css][misc/ui/jquery.ui.theme.css]": "1",
             "ajax_page_state[css][misc/ui/jquery.ui.menu.css]": "1",
             "ajax_page_state[css][misc/ui/jquery.ui.autocomplete.css]": "1",
             "ajax_page_state[css][sites/all/modules/calendar/css/calendar_multiday.css]": "1",
@@ -131,53 +131,42 @@
             "ajax_page_state[js][sites/all/themes/ntc_bootstrap/scripts/cookieconsent.js]": "1",
             "ajax_page_state[js][sites/all/themes/ntc_bootstrap/scripts/google-analytics.js]": "1",
             "ajax_page_state[js][sites/all/themes/ntc_bootstrap/scripts/ios-orientationchange-fix.js]": "1",
             "ajax_page_state[js][sites/all/themes/bootstrap/js/misc/ajax.js]": "1",
             "ajax_page_state[jquery_version]": "1.10",
         }
         uprn_data = {
-            "house_number": "0000" + f"{user_uprn}",
+            "house_number": user_uprn,
             "op": "Use",
-            "form_build_id": "form-BQ47tM0NKADE0s8toYkdSef3QBn6lDM-yBseqIOho80",
+            "form_build_id": "form-O65oY-ly-CYJlnQrhohK2uS1OP-4vXsS3CqYXD7-BeM",
             "form_id": "ntc_address_wizard",
         }
         collections = []
 
         response = s.post(
             "https://my.northtyneside.gov.uk/system/ajax",
-            # cookies=cookies,
+            cookies=cookies,
             headers=headers,
             data=ajax_data,
             verify=False,
         )
         response = s.post(
             "https://my.northtyneside.gov.uk/category/81/bin-collection-dates",
-            # cookies=cookies,
-            headers=headers,
-            data=uprn_data,
-            verify=False,
-        )
-        response = s.get(
-            "https://my.northtyneside.gov.uk/category/81/bin-collection-dates",
-            # cookies=cookies,
+            cookies=cookies,
             headers=headers,
             data=uprn_data,
             verify=False,
         )
 
         # Parse form page and get the day of week text
         soup = BeautifulSoup(response.text, features="html.parser")
         soup.prettify()
         bin_text = soup.find("section", {"class": "block block-ntc-bins clearfix"})
         regular_text = bin_text.select("p:nth-child(2) > strong")[0].text.strip()
-        x = bin_text.select("p:nth-child(4) > strong")
-        if len(bin_text.select("p:nth-child(4) > strong")) == 1:
-            special_text = bin_text.select("p:nth-child(4) > strong")[0].text.strip()
-        else:
-            special_text = bin_text.select("p:nth-child(5) > strong")[0].text.strip()
+        special_text = bin_text.select("p:nth-child(4) > strong")[0].text.strip()
 
         # Since calendar only shows until end of March 2024, work out how many weeks that is
         weeks_total = math.floor((datetime(2024, 4, 1) - datetime.now()).days / 7)
 
         # Convert day text to series of dates using previous calculation
         regular_collections = get_weekday_dates_in_period(
             datetime.today(),
@@ -188,23 +177,22 @@
             datetime.today(), days_of_week.get(special_text.capitalize())
         )
 
         # Differentiate between regular and recycling bins
         for item in regular_collections:
             item_as_date = datetime.strptime(item, date_format)
             # Check if holiday (calendar only has one day that's a holiday, and it's moved to the next day)
-            if is_holiday(item_as_date, Region.ENG):
+            if is_holiday(item_as_date, Region.England):
                 item_as_date += timedelta(days=1)
             # Use the isoweek number to separate collections - at the time of writing 11th Jan is week 2, which
             # is for the grey bin
             if (item_as_date.date().isocalendar()[1] % 2) == 0:
-                collections.append(("Regular bin (green)", item_as_date))
-
-            else:
                 collections.append(("Recycling bin (grey)", item_as_date))
+            else:
+                collections.append(("Regular bin (green)", item_as_date))
 
         # Add the special collection dates to the collection tuple
         collections += [
             ("Special collection (bookable)", datetime.strptime(item, date_format))
             for item in special_collections
         ]
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/NorthYorkshire.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SouthAyrshireCouncil.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,74 @@
-from bs4 import BeautifulSoup
+import json
+from datetime import timedelta
+
+import requests
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
+# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        uprn = kwargs.get("uprn")
-        check_uprn(uprn)
-
-        # Figure bin data URL from UPRN
-        url = "https://www.northyorks.gov.uk/bin-calendar/lookup"
-
-        payload = {
-            "selected_address": uprn,
-            "submit": "Continue",
-            "form_id": "bin_calendar_lookup_form",
+        # Get and check both the passed UPRN and postcode
+        user_uprn = kwargs.get("uprn")
+        check_uprn(user_uprn)
+        user_postcode = kwargs.get("postcode")
+        check_postcode(user_postcode)
+
+        # Build the headers, specify the parameters and then make a GET for the calendar
+        headers = {
+            "Connection": "Keep-Alive",
+            "User-Agent": "okhttp/3.14.9",
         }
-        headers = {"Content-Type": "application/x-www-form-urlencoded"}
-
-        # This endpoint redirects to the data url.
-        response = requests.request("POST", url, headers=headers, data=payload)
-        bin_data_url = f"{response.url}/ajax"
-
-        # Get bin data
-        response = requests.request("GET", bin_data_url)
-        bin_data = response.json()
-
-        # Parse bin data
-        soup = BeautifulSoup(bin_data[1]["data"], "html.parser")
-
-        # All collection info is in the table
-        table = (
-            soup.find("div", {"id": "upcoming-collection"}).find("table").find("tbody")
+        params = {
+            "end_date": "2024-01-01",
+            "rn": user_uprn,
+            "device": "undefined",
+            "postcode": user_postcode,
+            "OS": "android",
+            "OS_ver": "31",
+            "app_ver": "35",
+        }
+        requests.packages.urllib3.disable_warnings()
+        response = requests.get(
+            "http://www.sac-bins.co.uk/get_calendar.php", params=params, headers=headers
         )
-        rows = table.find_all("tr")
 
+        # Load the response as JSON
+        json_data = json.loads(response.text)
+
+        # The response loads well over a year's worth of data, so figure out some dates to limit output
+        today = datetime.today()
+        eight_weeks = datetime.today() + timedelta(days=8 * 7)
         data = {"bins": []}
-        for row in rows:
-            cols = row.find_all("td")
-            # First column is date
-            bin_date = datetime.strptime(cols[0].text.strip(), "%d %B %Y")
-            # Third column is type
-            bin_type = cols[2].text.strip()
-            # This bin
-            this_bin = {
-                "type": bin_type,
-                "collectionDate": bin_date.strftime(date_format),
-            }
-            data["bins"].append(this_bin)
+
+        # The bin titles are pretty weird and colours are too basic, so make the names match the app
+        bin_friendly_names = {
+            "blue": "Blue Bin",
+            "red": "Food Caddy",
+            "green": "Green Bin",
+            "grey": "Grey Bin",
+            "purple": "Purple Bin",
+            "brown": "Brown Bin",
+        }
+
+        # Loop through the results. When a date is found that's on or greater than today's date AND less than
+        # eight weeks away, we want it in the output. So look up the friendly name and add it in.
+        for item in json_data:
+            bin_date = datetime.strptime(item["start"], "%Y-%m-%d").date()
+            if today.date() <= bin_date <= eight_weeks.date():
+                bin_type = bin_friendly_names.get(item["className"])
+                dict_data = {
+                    "type": bin_type,
+                    "collectionDate": bin_date.strftime(date_format),
+                }
+                data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/RhonddaCynonTaffCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SouthOxfordshireCouncil.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,81 @@
+import requests
 from bs4 import BeautifulSoup
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
+# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        data = {"bins": []}
-
-        # Get UPRN from kwargs
         user_uprn = kwargs.get("uprn")
         check_uprn(user_uprn)
 
-        # Construct headers and set passed UPRN as a param for request
+        # UPRN is passed in via a cookie. Set cookies/params and GET the page
+        cookies = {
+            # 'JSESSIONID': '96F2A15C14569B2ED2BBEB140FE86532',
+            "SVBINZONE": f"SOUTH%3AUPRN%40{user_uprn}",
+        }
         headers = {
-            "authority": "www.rctcbc.gov.uk",
-            "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
-            "accept-language": "en-GB,en;q=0.9",
-            "cache-control": "no-cache",
-            # 'cookie': 'ASP.NET_SessionId=2b4gaaydt1rlu5pccgrpzamm',
-            "pragma": "no-cache",
-            "referer": "https://www.rctcbc.gov.uk/EN/Resident/RecyclingandWaste/RecyclingandWasteCollectionDays.aspx?PropertyNumber=&Postcode=CF72%209JD",
-            "sec-ch-ua": '"Chromium";v="116", "Not)A;Brand";v="24", "Opera GX";v="102"',
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": '"Windows"',
-            "sec-fetch-dest": "document",
-            "sec-fetch-mode": "navigate",
-            "sec-fetch-site": "same-origin",
-            "sec-fetch-user": "?1",
-            "upgrade-insecure-requests": "1",
-            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.5845.188 Safari/537.36",
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8",
+            "Accept-Language": "en-GB,en;q=0.7",
+            "Cache-Control": "max-age=0",
+            "Connection": "keep-alive",
+            "Referer": "https://eform.southoxon.gov.uk/ebase/BINZONE_DESKTOP.eb?SOVA_TAG=SOUTH&ebd=0&ebz=1_1668467255368",
+            "Sec-Fetch-Dest": "document",
+            "Sec-Fetch-Mode": "navigate",
+            "Sec-Fetch-Site": "same-origin",
+            "Sec-Fetch-User": "?1",
+            "Sec-GPC": "1",
+            "Upgrade-Insecure-Requests": "1",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/107.0.0.0 Safari/537.36",
         }
         params = {
-            "uprn": user_uprn,
+            "SOVA_TAG": "SOUTH",
+            "ebd": "0",
+            # 'ebz':      '1_1668467255368',
         }
-
+        requests.packages.urllib3.disable_warnings()
         response = requests.get(
-            "https://www.rctcbc.gov.uk/EN/Resident/RecyclingandWaste/RecyclingandWasteCollectionDays.aspx",
+            "https://eform.southoxon.gov.uk/ebase/BINZONE_DESKTOP.eb",
             params=params,
             headers=headers,
+            cookies=cookies,
         )
 
-        # Throw an error if response is not HTTP200
-        if response.status_code != 200:
-            raise SystemError(
-                "Response status was not 200: Please raise an issue on GitHub!"
-            )
-
-        # Parse response page and get all table rows
+        # Parse response text for super speedy finding
         soup = BeautifulSoup(response.text, features="html.parser")
         soup.prettify()
-        table_rows = soup.find("table", class_=("waste-table")).find_all("tr")
 
-        # Find the bin type and parse the date for each row, then add to dict. First row will be just headings,
-        # so skip it
-        for row in table_rows:
-            if len(row.contents) > 3:
-                continue
-            bin_type = row.contents[1].text.strip()
-            bin_date_text = (
-                row.contents[2].text.split(",")[1].strip().replace(" of ", "")
-            )
-            bin_date = datetime.strptime(
-                remove_ordinal_indicator_from_date_string(bin_date_text), "%A %d %B %Y"
-            ).strftime(date_format)
+        data = {"bins": []}
+
+        # Page has slider info side by side, which are two instances of this class
+        for bin in soup.find_all("div", {"class": "binextra"}):
+            bin_info = bin.text.split("-")
+            try:
+                # No date validation since year isn't included on webpage
+                bin_date = get_next_occurrence_from_day_month(
+                    datetime.strptime(bin_info[0].strip() + " " + datetime.today().strftime("%Y"),
+                                      "%A %d %B %Y")).strftime(date_format)
+                bin_type = str.capitalize(bin_info[1].strip())
+            except Exception as ex:
+                raise ValueError(f"Error parsing bin data: {ex}")
 
+            # Build data dict for each entry
             dict_data = {
                 "type": bin_type,
                 "collectionDate": bin_date,
             }
             data["bins"].append(dict_data)
 
+        data["bins"].sort(
+            key=lambda x: datetime.strptime(x.get("collectionDate"), date_format)
+        )
+
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/RochdaleCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/TorbayCouncil.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,52 @@
-from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
-# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        api_url = "https://webforms.rochdale.gov.uk/BinCalendar"
-        user_postcode = kwargs.get("postcode")
-        user_uprn = kwargs.get("uprn")
-
-        # Check the postcode and UPRN are valid
-        check_postcode(user_postcode)
-        check_uprn(user_uprn)
-
-        # Create the form data
-        form_data = {
-            "PostCode": user_postcode,
-            "SelectedUprn": user_uprn,
-            "Step": 2,
-        }
+        uprn = kwargs.get("uprn")
+        check_uprn(uprn)
 
-        # Make a request to the API
+        headers = {
+            "Accept": "*/*",
+            "Accept-Encoding": "gzip, deflate, br",
+            "Accept-Language": "en-GB,en-US;q=0.9,en;q=0.8",
+            "Connection": "keep-alive",
+            "Host": "online.torbay.gov.uk",
+            "Origin": "https://www.torbay.gov.uk",
+            "Referer": "https://www.torbay.gov.uk/",
+            "sec-ch-ua": '"Chromium";v="110", "Not A(Brand";v="24", "Google Chrome";v="110"',
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": '"Windows"',
+            "Sec-Fetch-Dest": "empty",
+            "Sec-Fetch-Mode": "cors",
+            "Sec-Fetch-Site": "same-site",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36",
+        }
         requests.packages.urllib3.disable_warnings()
-        response = requests.post(api_url, data=form_data)
-
-        # Make a BS4 object
-        soup = BeautifulSoup(response.text, features="html.parser")
-        soup.prettify()
+        response = requests.get(
+            f"https://online.torbay.gov.uk/services.bartec/collections?uprn={uprn}",
+            headers=headers,
+        )
+        if response.status_code != 200:
+            raise ValueError("No bin data found for provided UPRN.")
+        json_data = json.loads(response.text)
 
         data = {"bins": []}
-
-        # Get the table element and rows
-        table_element = soup.find("table", {"id": "tblCollectionDetails"})
-        table_rows = table_element.find_all_next("tr")
-
-        row_index = 0
-        for row in table_rows:
-            if row_index < 1:
-                row_index += 1
-                continue
-            else:
-                # Get the date from the th element
-                date = datetime.strptime(
-                    row.find("th").get_text().strip(), "%A %d %B %Y"
-                ).strftime(date_format)
-
-                # Get the bin types from the td elements and filter out the empty ones
-                bin_types = filter(lambda td: td.find("img"), row.find_all("td"))
-
-                # Convert the bin types to a list
-                bin_types_list = list(bin_types)
-
-                # Append the bin type and date to the data dict
-                for td in bin_types_list:
-                    img = td.find("img")
-                    bin_type_text = img["alt"]
-                    data["bins"].append({"type": bin_type_text, "collectionDate": date})
-
-                row_index += 1
+        for c in json_data:
+            dict_data = {
+                "type": c["Service"].replace("Empty ", "").strip(),
+                "collectionDate": datetime.strptime(
+                    c["NextCollection"].strip(), "%d %B %Y"
+                ).strftime(date_format),
+            }
+            data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/RugbyBoroughCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/TonbridgeAndMallingBC.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,93 +1,102 @@
+from datetime import *
+
+import requests
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        data = {"bins": []}
-        bin_types = {
-            "240L RUBBISH BIN": "Black bin",
-            "240L GARDEN BIN": "Green bin",
-            "180L RECYCLING BIN": "Blue lid bin",
-        }
-        collections = []
-
-        user_postcode = kwargs.get("postcode")
+        # Get UPRN and postcode from the parsed args
         user_uprn = kwargs.get("uprn")
-
+        user_postcode = kwargs.get("postcode")
         check_uprn(user_uprn)
         check_postcode(user_postcode)
 
+        requests.packages.urllib3.disable_warnings()
+
+        # Set up some form data, then POST for the form and scrape the result
         headers = {
-            "authority": "www.rugby.gov.uk",
-            "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
-            "accept-language": "en-GB,en;q=0.9",
-            "cache-control": "no-cache",
-            "content-type": "application/x-www-form-urlencoded",
-            # 'cookie': 'JSESSIONID=7E90CAB54B649C3DCC7F6B5DA0897C63; COOKIE_SUPPORT=true; GUEST_LANGUAGE_ID=en_GB; AWSELB=D941E98916B5759862ED6C39DA9FB3FD9880491851D200C98112ABEC3223D52B19A2A2C6B37A89D3650D44FA5728FCAFEDE7BB2592D948FFF9C7B18D76C41AF02C308B0F3A2DE17F1585E9959BCE68CC83BC3AC753; CookieControl={"necessaryCookies":[],"optionalCookies":{},"statement":{},"consentDate":1701710876715,"consentExpiry":90,"interactedWith":true,"user":"8FED8810-3C3E-4D50-A9DC-42655030B3B1"}',
-            "origin": "https://www.rugby.gov.uk",
-            "pragma": "no-cache",
-            "referer": "https://www.rugby.gov.uk/check-your-next-bin-day",
-            "sec-ch-ua": '"Chromium";v="118", "Opera GX";v="104", "Not=A?Brand";v="99"',
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8",
+            "Accept-Language": "en-GB,en;q=0.6",
+            "Cache-Control": "no-cache",
+            "Connection": "keep-alive",
+            "Content-Type": "multipart/form-data; boundary=----WebKitFormBoundaryI1XYcX9fNeKxm4LB",
+            # 'Cookie': 'PHPSESSID=-3mn6j-vkWcY4xPPXbT3Ggk1gSQJLId%2CztSoQV5-f8Pi7Cju1wwE151qtwdUyE1c',
+            "Origin": "https://www.tmbc.gov.uk",
+            "Pragma": "no-cache",
+            "Referer": "https://www.tmbc.gov.uk/xfp/form/167",
+            "Sec-Fetch-Dest": "document",
+            "Sec-Fetch-Mode": "navigate",
+            "Sec-Fetch-Site": "same-origin",
+            "Sec-Fetch-User": "?1",
+            "Sec-GPC": "1",
+            "Upgrade-Insecure-Requests": "1",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36",
+            "sec-ch-ua": '"Not?A_Brand";v="8", "Chromium";v="108", "Brave";v="108"',
             "sec-ch-ua-mobile": "?0",
             "sec-ch-ua-platform": '"Windows"',
-            "sec-fetch-dest": "document",
-            "sec-fetch-mode": "navigate",
-            "sec-fetch-site": "same-origin",
-            "sec-fetch-user": "?1",
-            "upgrade-insecure-requests": "1",
-            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/118.0.5993.118 Safari/537.36",
-        }
-        params = {
-            "p_p_id": "com_placecube_digitalplace_local_waste_portlet_CollectionDayFinderPortlet",
-            "p_p_lifecycle": "0",
-            "p_p_state": "normal",
-            "p_p_mode": "view",
-            "_com_placecube_digitalplace_local_waste_portlet_CollectionDayFinderPortlet_mvcRenderCommandName": "/collection_day_finder/get_days",
-        }
-        data = {
-            "_com_placecube_digitalplace_local_waste_portlet_CollectionDayFinderPortlet_formDate": f"{datetime.now().timestamp().__floor__()}",
-            "_com_placecube_digitalplace_local_waste_portlet_CollectionDayFinderPortlet_postcode": f"{user_postcode}",
-            "_com_placecube_digitalplace_local_waste_portlet_CollectionDayFinderPortlet_uprn": f"{user_uprn}",
         }
+        data = (
+            f"------WebKitFormBoundaryI1XYcX9fNeKxm4LB\r\nContent-Disposition: form-data; "
+            f'name="__token"\r\n\r\ns_flSv1eIvJDeCwbFaYxclM3UTomdpWgg2cMWzZckaU\r\n'
+            f"------WebKitFormBoundaryI1XYcX9fNeKxm4LB\r\nContent-Disposition: form-data; "
+            f'name="page"\r\n\r\n128\r\n------WebKitFormBoundaryI1XYcX9fNeKxm4LB\r\nContent-Disposition: '
+            f'form-data; name="locale"\r\n\r\nen_GB\r\n------WebKitFormBoundaryI1XYcX9fNeKxm4LB\r\nContent'
+            f'-Disposition: form-data; name="q752eec300b2ffef2757e4536b77b07061842041a_0_0"\r\n\r\n'
+            f"{user_postcode}\r\n------WebKitFormBoundaryI1XYcX9fNeKxm4LB\r\nContent-Disposition: form-data; "
+            f'name="q752eec300b2ffef2757e4536b77b07061842041a_1_0"\r\n\r\n'
+            f"{user_uprn}\r\n------WebKitFormBoundaryI1XYcX9fNeKxm4LB\r\nContent-Disposition: form-data; "
+            f'name="next"\r\n\r\nNext\r\n------WebKitFormBoundaryI1XYcX9fNeKxm4LB--\r\n '
+        )
 
         response = requests.post(
-            "https://www.rugby.gov.uk/check-your-next-bin-day",
-            params=params,
-            headers=headers,
-            data=data,
+            "https://www.tmbc.gov.uk/xfp/form/167", headers=headers, data=data
         )
-
         soup = BeautifulSoup(response.text, features="html.parser")
         soup.prettify()
 
-        table_rows = soup.find("table", {"class": "table"}).find("tbody").find_all("tr")
-
-        for row in table_rows:
-            row_text = row.text.strip().split("\n")
-            bin_type = bin_types.get(row_text[0])
-            collections.append(
-                (bin_type, datetime.strptime(row_text[1], "%A %d %b %Y"))
-            )
-            collections.append(
-                (bin_type, datetime.strptime(row_text[3], "%A %d %b %Y"))
-            )
-
-        ordered_data = sorted(collections, key=lambda x: x[1])
         data = {"bins": []}
-        for item in ordered_data:
-            dict_data = {
-                "type": item[0],
-                "collectionDate": item[1].strftime(date_format),
-            }
-            data["bins"].append(dict_data)
+        last_date = datetime.now()
+
+        # Find the table on the page and get data from each row (we don't care about the headings)
+        table = soup.find(
+            "table", {"class": "data-table waste-collections-table"}
+        ).find("tbody")
+        for row in table.find_all("tr"):
+            bin_date = row.find_next("td").text.strip()
+            collection_types = row.find("div", {"class": "collections"}).find_all("p")
+
+            # For each collection type in the list, parse the time
+            for item in collection_types:
+                curr_bin_date = datetime.strptime(bin_date, "%a %d %B")
+
+                # The calendar doesn't include the year, so using this to try to mitigate year change (note: it's
+                # currently January, so no idea if it will work until the end of the year lol)
+                if last_date.date().isocalendar()[1] < 52:
+                    curr_bin_date = datetime(
+                        last_date.year, curr_bin_date.month, curr_bin_date.day
+                    )
+                else:
+                    curr_bin_date = datetime(
+                        last_date.year + 1, curr_bin_date.month, curr_bin_date.day
+                    )
+
+                # Add each collection to the dictionary
+                dict_data = {
+                    "type": item.text.strip(),
+                    "collectionDate": curr_bin_date.strftime(date_format),
+                }
+                data["bins"].append(dict_data)
+                last_date = curr_bin_date
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SouthCambridgeshireCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SouthCambridgeshireCouncil.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 from bs4 import BeautifulSoup
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SouthOxfordshireCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/WiganBoroughCouncil.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,94 @@
+from datetime import datetime
+
 import requests
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
+        # Get and check UPRN
         user_uprn = kwargs.get("uprn")
         check_uprn(user_uprn)
+        user_uprn = user_uprn.zfill(
+            12
+        )  # Wigan is expecting 12 character UPRN or else it falls over, expects 0 padded UPRNS at the start for any that aren't 12 chars
 
-        # UPRN is passed in via a cookie. Set cookies/params and GET the page
-        cookies = {
-            # 'JSESSIONID': '96F2A15C14569B2ED2BBEB140FE86532',
-            "SVBINZONE": f"SOUTH%3AUPRN%40{user_uprn}",
-        }
-        headers = {
-            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8",
-            "Accept-Language": "en-GB,en;q=0.7",
-            "Cache-Control": "max-age=0",
-            "Connection": "keep-alive",
-            "Referer": "https://eform.southoxon.gov.uk/ebase/BINZONE_DESKTOP.eb?SOVA_TAG=SOUTH&ebd=0&ebz=1_1668467255368",
-            "Sec-Fetch-Dest": "document",
-            "Sec-Fetch-Mode": "navigate",
-            "Sec-Fetch-Site": "same-origin",
-            "Sec-Fetch-User": "?1",
-            "Sec-GPC": "1",
-            "Upgrade-Insecure-Requests": "1",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/107.0.0.0 Safari/537.36",
+        user_postcode = kwargs.get("postcode")
+        check_postcode(user_postcode)
+
+        # Start a new session to walk through the form
+        requests.packages.urllib3.disable_warnings()
+        s = requests.session()
+
+        # Get our initial session running
+        response = s.get("https://apps.wigan.gov.uk/MyNeighbourhood/")
+
+        soup = BeautifulSoup(response.text, features="html.parser")
+        soup.prettify()
+
+        # Grab the ASP variables needed to continue
+        payload = {
+            "__VIEWSTATE": (soup.find("input", {"id": "__VIEWSTATE"}).get("value")),
+            "__VIEWSTATEGENERATOR": (
+                soup.find("input", {"id": "__VIEWSTATEGENERATOR"}).get("value")
+            ),
+            "__EVENTVALIDATION": (
+                soup.find("input", {"id": "__EVENTVALIDATION"}).get("value")
+            ),
+            "ctl00$ContentPlaceHolder1$txtPostcode": (user_postcode),
+            "ctl00$ContentPlaceHolder1$btnPostcodeSearch": ("Search"),
         }
-        params = {
-            "SOVA_TAG": "SOUTH",
-            "ebd": "0",
-            # 'ebz':      '1_1668467255368',
+
+        # Use the above to get to the next page with address selection
+        response = s.post("https://apps.wigan.gov.uk/MyNeighbourhood/", payload)
+
+        soup = BeautifulSoup(response.text, features="html.parser")
+        soup.prettify()
+
+        # Load the new variables that are constant and can't be gotten from the page
+        payload = {
+            "__EVENTTARGET": ("ctl00$ContentPlaceHolder1$lstAddresses"),
+            "__EVENTARGUMENT": (""),
+            "__LASTFOCUS": (""),
+            "__VIEWSTATE": (soup.find("input", {"id": "__VIEWSTATE"}).get("value")),
+            "__VIEWSTATEGENERATOR": (
+                soup.find("input", {"id": "__VIEWSTATEGENERATOR"}).get("value")
+            ),
+            "__EVENTVALIDATION": (
+                soup.find("input", {"id": "__EVENTVALIDATION"}).get("value")
+            ),
+            "ctl00$ContentPlaceHolder1$txtPostcode": (user_postcode),
+            "ctl00$ContentPlaceHolder1$lstAddresses": ("UPRN" + user_uprn),
         }
-        requests.packages.urllib3.disable_warnings()
-        response = requests.get(
-            "https://eform.southoxon.gov.uk/ebase/BINZONE_DESKTOP.eb",
-            params=params,
-            headers=headers,
-            cookies=cookies,
-        )
 
-        # Parse response text for super speedy finding
+        # Get the final page with the actual dates
+        response = s.post("https://apps.wigan.gov.uk/MyNeighbourhood/", payload)
+
         soup = BeautifulSoup(response.text, features="html.parser")
         soup.prettify()
 
         data = {"bins": []}
 
-        # Page has slider info side by side, which are two instances of this class
-        for bin in soup.find_all("div", {"class": "binextra"}):
-            bin_info = list(bin.stripped_strings)
-            try:
-                # On standard collection schedule, date will be contained in the first stripped string
-                if contains_date(bin_info[0]):
-                    bin_date = get_next_occurrence_from_day_month(
-                        datetime.strptime(
-                            bin_info[0] + " " + datetime.today().strftime("%Y"),
-                            "%A %d %B - %Y",
-                        )
-                    ).strftime(date_format)
-                    bin_type = str.capitalize(bin_info[1])
-                # On exceptional collection schedule (e.g. around English Bank Holidays), date will be contained in the second stripped string
-                else:
-                    bin_date = get_next_occurrence_from_day_month(
-                        datetime.strptime(
-                            bin_info[1] + " " + datetime.today().strftime("%Y"),
-                            "%A %d %B - %Y",
-                        )
-                    ).strftime(date_format)
-                    bin_type = str.capitalize(bin_info[2])
-            except Exception as ex:
-                raise ValueError(f"Error parsing bin data: {ex}")
-
-            # Build data dict for each entry
-            dict_data = {
-                "type": bin_type,
-                "collectionDate": bin_date,
-            }
-            data["bins"].append(dict_data)
-
-        data["bins"].sort(
-            key=lambda x: datetime.strptime(x.get("collectionDate"), date_format)
-        )
+        # Get the dates.
+        for bins in soup.find_all("div", {"class": "BinsRecycling"}):
+            bin_type = bins.find("h2").text
+            binCollection = bins.find("div", {"class": "dateWrapper-next"}).get_text(
+                strip=True
+            )
+            binData = datetime.strptime(
+                re.sub(r"(\d)(st|nd|rd|th)", r"\1", binCollection), "%A%d%b%Y"
+            )
+            if binData:
+                data[bin_type] = binData.strftime(date_format)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/SouthTynesideCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/SouthTynesideCouncil.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from datetime import datetime
 
 import requests
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 def get_address_uprn(postcode: str, paon: str, api_url: str) -> str:
     """
     Gets the UPRN and address in desired format
         :rtype: str
         :param postcode: Postcode to use
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/StAlbansCityAndDistrictCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/TamesideMBCouncil.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,63 @@
+import json
+from datetime import datetime, timedelta
+
+import requests
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
-from dateutil import parser
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 class CouncilClass(AbstractGetBinDataClass):
     def parse_data(self, page: str, **kwargs) -> dict:
-        user_uprn = kwargs.get("uprn")
-        check_uprn(user_uprn)
-
-        data = {"bins": []}
-
-        headers = {
-            "Content-Type": "application/json; charset=UTF-8",
+        api_url = "http://lite.tameside.gov.uk/BinCollections/CollectionService.svc/GetBinCollection"
+        uprn = kwargs.get("uprn")
+        check_uprn(uprn)
+
+        params = {
+            "version": "3.1.4",
+            "uprn": uprn,
+            "token": "",
+            "notification": "1",
+            "operatingsystemid": "2",
+            "testmode": "true",
         }
 
-        req_data = {"uprn": user_uprn, "noticeBoard": "default"}
+        headers = {"content-type": "text/plain"}
 
-        url = "https://gis.stalbans.gov.uk/NoticeBoard9/VeoliaProxy.NoticeBoard.asmx/GetServicesByUprnAndNoticeBoard"
+        requests.packages.urllib3.disable_warnings()
+        response = requests.post(api_url, json=params, headers=headers)
 
-        response = requests.post(url, json=req_data, headers=headers)
+        json_response = json.loads(response.content)["GetBinCollectionResult"]["Data"]
 
-        collections_response = response.json()
+        today = datetime.today()
+        eight_weeks = datetime.today() + timedelta(days=8 * 7)
+        data = {"bins": []}
+        collection_tuple = []
 
-        collections = []
+        bin_friendly_names = {
+            "2": "Blue Bin",
+            "6": "Green Bin",
+            "5": "Black Bin",
+            "3": "Brown Bin",
+        }
 
-        for collection in collections_response["d"]:
-            collection_data = collection["ServiceHeaders"][0]
-            bin_type = collection_data["TaskType"]
-            collection_date = collection_data["Next"]
-            next_collection = parser.isoparser().isoparse(collection_date)
-            collections.append((bin_type, next_collection))
+        for item in json_response:
+            collection_date = datetime.strptime(
+                item.get("CollectionDate"), "%d/%m/%Y %H:%M:%S"
+            )
+            if today.date() <= collection_date.date() <= eight_weeks.date():
+                bin_type = bin_friendly_names.get(item.get("BinType"))
+                collection_tuple.append(
+                    (bin_type, collection_date.strftime(date_format))
+                )
 
-        ordered_data = sorted(collections, key=lambda x: x[1])
+        ordered_data = sorted(collection_tuple, key=lambda x: x[1])
 
         for item in ordered_data:
             dict_data = {
                 "type": item[0],
-                "collectionDate": item[1].strftime(date_format),
+                "collectionDate": item[1],
             }
             data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/TorbayCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/BoltonCouncil.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,78 @@
+from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
 from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
 
 
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        uprn = kwargs.get("uprn")
-        check_uprn(uprn)
+
+        user_uprn = kwargs.get("uprn")
+        check_uprn(user_uprn)
+
+        soup = BeautifulSoup(page.text, features="html.parser")
+        soup.prettify()
+
+        data = {"bins": []}
 
         headers = {
-            "Accept": "*/*",
-            "Accept-Encoding": "gzip, deflate, br",
-            "Accept-Language": "en-GB,en-US;q=0.9,en;q=0.8",
-            "Connection": "keep-alive",
-            "Host": "online.torbay.gov.uk",
-            "Origin": "https://www.torbay.gov.uk",
-            "Referer": "https://www.torbay.gov.uk/",
-            "sec-ch-ua": '"Chromium";v="110", "Not A(Brand";v="24", "Google Chrome";v="110"',
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": '"Windows"',
-            "Sec-Fetch-Dest": "empty",
-            "Sec-Fetch-Mode": "cors",
-            "Sec-Fetch-Site": "same-site",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36",
+            'authority': 'www.bolton.gov.uk',
+            'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
+            'accept-language': 'en-GB,en;q=0.9',
+            'cache-control': 'no-cache',
+            'content-type': 'application/x-www-form-urlencoded',
+            'origin': 'https://www.bolton.gov.uk',
+            'pragma': 'no-cache',
+            'referer': 'https://www.bolton.gov.uk/next-bin-collection',
+            'sec-ch-ua': '"Not?A_Brand";v="99", "Opera GX";v="97", "Chromium";v="111"',
+            'sec-ch-ua-mobile': '?0',
+            'sec-ch-ua-platform': '"Windows"',
+            'sec-fetch-dest': 'document',
+            'sec-fetch-mode': 'navigate',
+            'sec-fetch-site': 'same-origin',
+            'sec-fetch-user': '?1',
+            'upgrade-insecure-requests': '1',
+            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.5563.147 Safari/537.36',
+        }
+
+        req_data = {
+            'uprn': user_uprn,
         }
+
         requests.packages.urllib3.disable_warnings()
-        response = requests.get(
-            f"https://online.torbay.gov.uk/services.bartec/collections?uprn={uprn}",
-            headers=headers,
-        )
-        if response.status_code != 200:
-            raise ValueError("No bin data found for provided UPRN.")
-        json_data = json.loads(response.text)
+        response = requests.post('https://www.bolton.gov.uk/next-bin-collection', headers=headers, data=req_data)
 
-        data = {"bins": []}
-        for c in json_data:
+        soup = BeautifulSoup(response.text, features="html.parser")
+        soup.prettify()
+
+        collections = []
+
+        # Find section with bins in
+        sections = soup.find_all("div", {"class": "media-body"})
+
+        # For each bin section, get the text and the list elements
+        for item in sections:
+            words = item.find_next("p", {"class": "media-heading"}).text.split()[2:4]
+            bin_type = ' '.join(words).capitalize()
+            date_list = item.find_all("li")
+            for d in date_list:
+                next_collection = datetime.strptime(d.text.strip(), "%A %d %B %Y")
+                collections.append((bin_type, next_collection))
+
+        # Sort the text and list elements by date
+        ordered_data = sorted(collections, key=lambda x: x[1])
+
+        # Put the elements into the dictionary
+        for item in ordered_data:
             dict_data = {
-                "type": c["Service"].replace("Empty ", "").strip(),
-                "collectionDate": datetime.strptime(
-                    c["NextCollection"].strip(), "%d %B %Y"
-                ).strftime(date_format),
+                "type": item[0],
+                "collectionDate": item[1].strftime(date_format),
             }
             data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/TorridgeDistrictCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/TorridgeDistrictCouncil.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from xml.etree import ElementTree
 
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     baseclass. They can also override some
@@ -35,17 +36,17 @@
             )
 
         # Make the Request - change the URL - find out your property number
         # URL
         url = "https://collections-torridge.azurewebsites.net/WebService2.asmx"
         # Post data
         post_data = (
-            '<?xml version="1.0" encoding="utf-8"?><soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"><soap:Body><getRoundCalendarForUPRN xmlns="http://tempuri2.org/"><council>TOR</council><UPRN>'
-            + uprn
-            + "</UPRN><PW>wax01653</PW></getRoundCalendarForUPRN></soap:Body></soap:Envelope>"
+                '<?xml version="1.0" encoding="utf-8"?><soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"><soap:Body><getRoundCalendarForUPRN xmlns="http://tempuri2.org/"><council>TOR</council><UPRN>'
+                + uprn
+                + "</UPRN><PW>wax01653</PW></getRoundCalendarForUPRN></soap:Body></soap:Envelope>"
         )
         requests.packages.urllib3.disable_warnings()
         full_page = requests.post(url, headers=headers, data=post_data)
 
         return full_page
 
     def parse_data(self, page, **kwargs) -> dict:
@@ -70,17 +71,17 @@
             )
 
         # Make the Request - change the URL - find out your property number
         # URL
         url = "https://collections-torridge.azurewebsites.net/WebService2.asmx"
         # Post data
         post_data = (
-            '<?xml version="1.0" encoding="utf-8"?><soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"><soap:Body><getRoundCalendarForUPRN xmlns="http://tempuri2.org/"><council>TOR</council><UPRN>'
-            + uprn
-            + "</UPRN><PW>wax01653</PW></getRoundCalendarForUPRN></soap:Body></soap:Envelope>"
+                '<?xml version="1.0" encoding="utf-8"?><soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"><soap:Body><getRoundCalendarForUPRN xmlns="http://tempuri2.org/"><council>TOR</council><UPRN>'
+                + uprn
+                + "</UPRN><PW>wax01653</PW></getRoundCalendarForUPRN></soap:Body></soap:Envelope>"
         )
         requests.packages.urllib3.disable_warnings()
         page = requests.post(url, headers=headers, data=post_data)
 
         # Remove the soap wrapper
         namespaces = {
             "soap": "http://schemas.xmlsoap.org/soap/envelope/",
@@ -97,58 +98,43 @@
         soup = BeautifulSoup(page.text, features="html.parser")
         soup.prettify()
 
         data = {"bins": []}
 
         b_el = soup.find("b", string="GardenBin")
         if b_el:
-            results = re.search(
-                "([A-Za-z]+ \\d\\d? [A-Za-z]+) (.*?)", b_el.next_sibling.split(": ")[1]
-            )
+            results = re.search("([A-Za-z]+ \\d\\d? [A-Za-z]+) (.*?)", b_el.next_sibling.split(": ")[1])
             if results and results.groups()[0]:
                 date = results.groups()[0] + " " + datetime.today().strftime("%Y")
-                data["bins"].append(
-                    {
-                        "type": "GardenBin",
-                        "collectionDate": get_next_occurrence_from_day_month(
-                            datetime.strptime(date, "%a %d %b %Y")
-                        ).strftime(date_format),
-                    }
-                )
+                data["bins"].append({
+                    "type": "GardenBin",
+                    "collectionDate": get_next_occurrence_from_day_month(datetime.strptime(date, "%a %d %b %Y"))
+                    .strftime(date_format)
+                })
 
         b_el = soup.find("b", string="Refuse")
         if b_el:
-            results = re.search(
-                "([A-Za-z]+ \\d\\d? [A-Za-z]+) (.*?)", b_el.next_sibling.split(": ")[1]
-            )
+            results = re.search("([A-Za-z]+ \\d\\d? [A-Za-z]+) (.*?)", b_el.next_sibling.split(": ")[1])
             if results and results.groups()[0]:
                 date = results.groups()[0] + " " + datetime.today().strftime("%Y")
-                data["bins"].append(
-                    {
-                        "type": "Refuse",
-                        "collectionDate": get_next_occurrence_from_day_month(
-                            datetime.strptime(date, "%a %d %b %Y")
-                        ).strftime(date_format),
-                    }
-                )
+                data["bins"].append({
+                    "type": "Refuse",
+                    "collectionDate": get_next_occurrence_from_day_month(datetime.strptime(date, "%a %d %b %Y"))
+                    .strftime(date_format)
+                })
 
         b_el = soup.find("b", string="Recycling")
         if b_el:
-            results = re.search(
-                "([A-Za-z]+ \\d\\d? [A-Za-z]+) (.*?)", b_el.next_sibling.split(": ")[1]
-            )
+            results = re.search("([A-Za-z]+ \\d\\d? [A-Za-z]+) (.*?)", b_el.next_sibling.split(": ")[1])
             if results and results.groups()[0]:
                 date = results.groups()[0] + " " + datetime.today().strftime("%Y")
-                data["bins"].append(
-                    {
-                        "type": "Recycling",
-                        "collectionDate": get_next_occurrence_from_day_month(
-                            datetime.strptime(date, "%a %d %b %Y")
-                        ).strftime(date_format),
-                    }
-                )
+                data["bins"].append({
+                    "type": "Recycling",
+                    "collectionDate": get_next_occurrence_from_day_month(datetime.strptime(date, "%a %d %b %Y"))
+                    .strftime(date_format)
+                })
 
         data["bins"].sort(
             key=lambda x: datetime.strptime(x.get("collectionDate"), date_format)
         )
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/ValeofWhiteHorseCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/WokingBoroughCouncil.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,103 +1,101 @@
-import requests
 from bs4 import BeautifulSoup
+import urllib
 from uk_bin_collection.uk_bin_collection.common import *
 from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
 
 
-# import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        user_uprn = kwargs.get("uprn")
-        check_uprn(user_uprn)
+        requests.packages.urllib3.disable_warnings()
+        root_url = "https://asjwsw-wrpwokingmunicipal-live.whitespacews.com/"
+        # Get the house number and postcode from the commandline
+        user_paon = kwargs.get("paon")
+        user_postcode = kwargs.get("postcode")
+        check_postcode(user_postcode)
+
+        # Start a new session for the form, and get the chosen URL from the commandline
+        session = requests.Session()
+        req = session.get(root_url)
+
+        # Parse the requested URL to get a link to the "View My Collections" portal with a unique service ID
+        start = BeautifulSoup(req.text, features="html.parser")
+        start.prettify()
+        base_link = start.select(
+            "#menu-content > div > div:nth-child(1) > p.govuk-body.govuk-\!-margin-bottom-0.colorblue.lineheight15 > a")[
+            0].attrs.get("href")
+
+        # We need to reorder the query parts from the unique URL, so split them up to make it easier
+        query_parts = urllib.parse.urlparse(base_link).query.split("&")
+        parts = base_link.split("?")
+        addr_link = parts[0] + "/mop.php?" + query_parts[1] + "&" + query_parts[0] + "&seq=2"
 
-        # UPRN is passed in via a cookie. Set cookies/params and GET the page
-        cookies = {
-            "SVBINZONE": f"VALE%3AUPRN%40{user_uprn}",
-        }
+        # Bring in some headers to emulate a browser, and put the UPRN and postcode into the form data.
+        # This is sent in a POST request, emulating browser behaviour.
         headers = {
-            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8",
-            "Accept-Language": "en-GB,en;q=0.7",
-            "Cache-Control": "max-age=0",
-            "Connection": "keep-alive",
-            "Referer": "https://eform.whitehorsedc.gov.uk/ebase/BINZONE_DESKTOP.eb?SOVA_TAG=VALE&ebd=0&ebz=1_1704201201813",
-            "Sec-Fetch-Dest": "document",
-            "Sec-Fetch-Mode": "navigate",
-            "Sec-Fetch-Site": "same-origin",
-            "Sec-Fetch-User": "?1",
-            "Sec-GPC": "1",
-            "Upgrade-Insecure-Requests": "1",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/107.0.0.0 Safari/537.36",
+            'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
+            'Accept-Language': 'en-GB,en;q=0.9',
+            'Cache-Control': 'no-cache',
+            'Connection': 'keep-alive',
+            'Content-Type': 'application/x-www-form-urlencoded',
+            'Origin': 'https://asjwsw-wrpwokingmunicipal-live.whitespacews.com',
+            'Pragma': 'no-cache',
+            'Referer': 'https://asjwsw-wrpwokingmunicipal-live.whitespacews.com/',
+            'Sec-Fetch-Dest': 'document',
+            'Sec-Fetch-Mode': 'navigate',
+            'Sec-Fetch-Site': 'same-origin',
+            'Sec-Fetch-User': '?1',
+            'Upgrade-Insecure-Requests': '1',
+            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36 OPR/98.0.0.0',
+            'sec-ch-ua': '"Chromium";v="112", "Not_A Brand";v="24", "Opera GX";v="98"',
+            'sec-ch-ua-mobile': '?0',
+            'sec-ch-ua-platform': '"Windows"',
         }
-        params = {
-            "SOVA_TAG": "VALE",
-            "ebd": "0",
+        data = {
+            'address_name_number': user_paon,
+            'address_street': '',
+            'street_town': '',
+            'address_postcode': user_postcode,
         }
-        requests.packages.urllib3.disable_warnings()
-        response = requests.get(
-            "https://eform.whitehorsedc.gov.uk/ebase/BINZONE_DESKTOP.eb",
-            params=params,
-            headers=headers,
-            cookies=cookies,
-        )
+        addr_page = session.post(addr_link, headers=headers, data=data)
+        addr = BeautifulSoup(addr_page.text, features="html.parser")
+        addr.prettify()
+
+        # This page should only have one address, but regardless, select the first one and make a request to load the
+        # calendar page.
+        cal_link = root_url + addr.select("#property_list > ul > li > a")[0].attrs.get("href")
+        cal_page = session.get(cal_link)
 
-        # Parse response text for super speedy finding
-        soup = BeautifulSoup(response.text, features="html.parser")
+        # Parse the calendar page
+        soup = BeautifulSoup(cal_page.text, features="html.parser")
         soup.prettify()
-
         data = {"bins": []}
 
-        # Page has slider info side by side, which are two instances of this class
-        for bin in soup.find_all("div", {"class": "bintxt"}):
-            try:
-                # Check bin type heading and make that bin type and colour
-                bin_type_info = list(bin.stripped_strings)
-                if "rubbish" in bin_type_info[0]:
-                    bin_type = "Rubbish"
-                    bin_colour = "Black"
-                elif "recycling" in bin_type_info[0]:
-                    bin_type = "Recycling"
-                    bin_colour = "Green"
-                else:
-                    raise ValueError(f"No bin info found in {bin_type_info[0]}")
-
-                bin_date_info = list(
-                    bin.find_next("div", {"class": "binextra"}).stripped_strings
-                )
-                # On standard collection schedule, date will be contained in the first string
-                if contains_date(bin_date_info[0]):
-                    bin_date = get_next_occurrence_from_day_month(
-                        datetime.strptime(
-                            bin_date_info[0] + " " + datetime.today().strftime("%Y"),
-                            "%A %d %B - %Y",
-                        )
-                    ).strftime(date_format)
-                # On exceptional collection schedule (e.g. around English Bank Holidays), date will be contained in the second stripped string
-                else:
-                    bin_date = get_next_occurrence_from_day_month(
-                        datetime.strptime(
-                            bin_date_info[1] + " " + datetime.today().strftime("%Y"),
-                            "%A %d %B - %Y",
-                        )
-                    ).strftime(date_format)
-            except Exception as ex:
-                raise ValueError(f"Error parsing bin data: {ex}")
-
-            # Build data dict for each entry
-            dict_data = {
-                "type": bin_type,
-                "collectionDate": bin_date,
-                "colour": bin_colour,
-            }
-            data["bins"].append(dict_data)
-
-        data["bins"].sort(
-            key=lambda x: datetime.strptime(x.get("collectionDate"), date_format)
-        )
+        # For whatever reason, each row contains all the information for that row, and each one after it. This code
+        # essentially gets all items from each row, but ignores the whitespace that you get when splitting using \n.
+        # This produces a big list of dates then bin types, so we split them up into a list of lists - each pair is
+        # a date and the bin type.
+        items = [i for i in soup.find("u1", {
+            "class": "displayinlineblock justifycontentleft alignitemscenter margin0 padding0"}).text.split("\n") if
+                 i != ""]
+        pairs = [items[i:i + 2] for i in range(0, len(items), 2)]
+
+        # Loop through the paired bin dates and types
+        for pair in pairs:
+            # This isn't necessary, but better safe than sorry
+            collection_date = datetime.strptime(pair[0], date_format).strftime(date_format)
+            # Change the formatting of the purple bins to replace the hyphens with slashes
+            if pair[1] == "Batteries-small electricals-textiles":
+                bin_type = pair[1].replace("-", "/").strip()
+            else:
+                bin_type = pair[1]
+
+            # Add the data into the dictionary
+            data["bins"].append({"type": bin_type, "collectionDate": collection_date})
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/councils/WaverleyBoroughCouncil.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/councils/WindsorAndMaidenheadCouncil.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,120 +1,133 @@
-from datetime import date, datetime
+from datetime import datetime
+from urllib.parse import urlparse
 
 import requests
 from bs4 import BeautifulSoup
-
 from uk_bin_collection.uk_bin_collection.common import *
-from uk_bin_collection.uk_bin_collection.get_bin_data import AbstractGetBinDataClass
+from uk_bin_collection.uk_bin_collection.get_bin_data import \
+    AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
 class CouncilClass(AbstractGetBinDataClass):
     """
     Concrete classes have to implement all abstract operations of the
     base class. They can also override some operations with a default
     implementation.
     """
 
     def parse_data(self, page: str, **kwargs) -> dict:
-        # pindex isn't actually paon, it's a url parameter that I'm guessing the council use as a property id
-        data = {"bins": []}
-        pindex = kwargs.get("paon")
+        root_url = "https://my.rbwm.gov.uk"
+        href_url = ""
+        api_url = "https://my.rbwm.gov.uk/block_refresh/block/47/node/136968?"
         user_postcode = kwargs.get("postcode")
-        check_postcode(user_postcode)
+        user_paon = kwargs.get("paon")
 
-        # WBC use a url parameter called "Track" that's generated when you start a form session.
-        # So first off, open the page, find the page link and copy it with the Track
-        start_url = "https://wav-wrp.whitespacews.com/"
-        s = requests.Session()
-        response = s.get(start_url)
-        soup = BeautifulSoup(response.content, features="html.parser")
-        soup.prettify()
-        collection_page_link = soup.find_all(
-            "p", {"class": "govuk-body govuk-!-margin-bottom-0 colorblue lineheight15"}
-        )[0].find("a")["href"]
-        track_id = collection_page_link[33:60]
-
-        # Next we need to search using the postcode, but this is actually an important POST request
-        pc_headers = {
-            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,"
-            "image/webp,image/apng,*/*;q=0.8",
-            "Accept-Language": "en-GB,en;q=0.9",
-            "Cache-Control": "max-age=0",
-            "Connection": "keep-alive",
-            "Origin": "https://wav-wrp.whitespacews.com",
-            "Referer": "https://wav-wrp.whitespacews.com/"
-            + track_id
-            + "&serviceID=A&seq=2",
-            "Sec-Fetch-Dest": "document",
-            "Sec-Fetch-Mode": "navigate",
-            "Sec-Fetch-Site": "same-origin",
-            "Sec-Fetch-User": "?1",
-            "Sec-GPC": "1",
-            "Upgrade-Insecure-Requests": "1",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, "
-            "like Gecko) Chrome/106.0.0.0 Safari/537.36",
-        }
-        form_data = {
-            "address_name_number": "",
-            "address_street": "",
-            "street_town": "",
-            "address_postcode": user_postcode,
+        data = {"bins": []}
+
+        requests.packages.urllib3.disable_warnings()
+        s = requests.session()
+        # Form start
+        headers = {
+            "authority": "my.rbwm.gov.uk",
+            "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8",
+            "accept-language": "en-GB,en;q=0.8",
+            "cache-control": "max-age=0",
+            "referer": "https://my.rbwm.gov.uk/special/your-collection-dates?uprn=100080371082&subdate=2022-08-19&addr=11%20Douglas%20Lane%20Wraysbury%20Staines%20TW19%205NF",
+            "sec-fetch-dest": "document",
+            "sec-fetch-mode": "navigate",
+            "sec-fetch-site": "same-origin",
+            "sec-fetch-user": "?1",
+            "sec-gpc": "1",
+            "upgrade-insecure-requests": "1",
+            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.36",
         }
-        response = s.post(
-            "https://wav-wrp.whitespacews.com/mop.php?serviceID=A&"
-            + track_id
-            + "&seq=2",
-            headers=pc_headers,
-            data=form_data,
-        )
+        s.get("https://my.rbwm.gov.uk/special/find-your-collection-dates", headers=headers)
 
-        # Finally, we can use pindex to find the address and get some data
-        request_url = (
-            "https://wav-wrp.whitespacews.com/mop.php?"
-            + track_id
-            + "&serviceID=A&seq=3&pIndex="
-            + pindex
-        )
+        # Select address
         headers = {
-            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,"
-            "image/webp,image/apng,*/*;q=0.8",
-            "Accept-Language": "en-GB,en;q=0.9",
-            "Connection": "keep-alive",
-            "Referer": "https://wav-wrp.whitespacews.com/mop.php?serviceID=A&"
-            + track_id
-            + "&seq=2",
-            "Sec-Fetch-Dest": "document",
-            "Sec-Fetch-Mode": "navigate",
-            "Sec-Fetch-Site": "same-origin",
-            "Sec-Fetch-User": "?1",
-            "Sec-GPC": "1",
-            "Upgrade-Insecure-Requests": "1",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, "
-            "like Gecko) Chrome/106.0.0.0 Safari/537.36",
+            "authority": "my.rbwm.gov.uk",
+            "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8",
+            "accept-language": "en-GB,en;q=0.8",
+            "cache-control": "max-age=0",
+            "origin": "https://my.rbwm.gov.uk",
+            "referer": "https://my.rbwm.gov.uk/special/find-your-collection-dates",
+            "sec-fetch-dest": "document",
+            "sec-fetch-mode": "navigate",
+            "sec-fetch-site": "same-origin",
+            "sec-fetch-user": "?1",
+            "sec-gpc": "1",
+            "upgrade-insecure-requests": "1",
+            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.36",
+        }
+        request_data = {
+            "atTxtStreet": user_postcode,
+            "nodeid": "x",
+            "formname": "x",
+            "pg": "20",
+            "start": "1",
+            "selectaddress": "Select this address",
+            "selectheading": "The following addresses match the address you entered - choose your address",
+            "arg": "",
         }
+        response = s.post(
+            "https://my.rbwm.gov.uk/special/address-selector-collection-dates",
+            headers=headers,
+            data=request_data
+        )
 
-        response = s.get(request_url, headers=headers)
         soup = BeautifulSoup(response.content, features="html.parser")
         soup.prettify()
 
-        # Find the list elements
-        u1_block = soup.find_all(
-            "u1",
-            {
-                "class": "displayinlineblock justifycontentleft alignitemscenter margin0 padding0"
-            },
-        )
-
-        for element in u1_block:
-            x = element.find_all_next(
-                "li", {"class": "displayinlineblock padding0px20px5px0px"}
-            )
-            dict_data = {
-                "type": x[2].text.strip(),
-                "collectionDate": datetime.strptime(
-                    x[1].text.strip(), date_format
-                ).strftime(date_format),
+        table = soup.find("table")
+        if table:
+            table_rows = table.find_all("tr")
+            for tr in table_rows:
+                td = tr.find_all("td")
+                # row = [i.text for i in td]
+                for item in td:
+                    if user_paon in item.text and user_postcode in item.text:
+                        href_url = td[1].find("a").get("href")
+                        continue
+
+            # Getting to bin data
+            headers = {
+                "authority": "my.rbwm.gov.uk",
+                "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8",
+                "accept-language": "en-GB,en;q=0.8",
+                "referer": "https://my.rbwm.gov.uk/special/address-selector-collection-dates",
+                "sec-fetch-dest": "document",
+                "sec-fetch-mode": "navigate",
+                "sec-fetch-site": "same-origin",
+                "sec-fetch-user": "?1",
+                "sec-gpc": "1",
+                "upgrade-insecure-requests": "1",
+                "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.36",
             }
-            data["bins"].append(dict_data)
+            params = {}
+            parsed_params = urlparse(href_url).query.split("&")
+            for item in parsed_params:
+                values = item.split("=")
+                params.update({values[0]: values[1]})
+
+            s.get(root_url + href_url, params=params, headers=headers)
+            response = s.get(
+                api_url + href_url.split("?")[1], params=params, headers=headers
+            )
+
+            soup = BeautifulSoup(response.content, features="html.parser")
+            soup.prettify()
+
+            table_rows = soup.find_all("tr")
+            for tr in table_rows:
+                td = tr.find_all("td")
+                row = [i.text for i in td]
+
+                if len(row) > 0:
+                    dict_data = {
+                        "type": row[0],
+                        "collectionDate": row[1],
+                    }
+                    data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.80.0/uk_bin_collection/uk_bin_collection/get_bin_data.py` & `uk_bin_collection-0.9.0/uk_bin_collection/uk_bin_collection/get_bin_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 """Module that contains an abstract class that can be imported to
 handle the data recieved from the provided council class.
 
 Keyword arguments: None
 """
-
 import json
 import logging
 from abc import ABC, abstractmethod
 from logging.config import dictConfig
-import os
 
 import requests
 
-from uk_bin_collection.uk_bin_collection.common import update_input_json
-
-_LOGGER = logging.getLogger(__name__)
+from uk_bin_collection.uk_bin_collection.common import write_output_json
 
 LOGGING_CONFIG = dict(
     version=1,
     formatters={"f": {"format": "%(asctime)s %(name)-12s %(levelname)-8s %(message)s"}},
     handlers={
         "h": {"class": "logging.StreamHandler", "formatter": "f", "level": logging.INFO}
     },
@@ -31,14 +27,17 @@
         logging.config.dictConfig(logging_config)
         logger = logging.getLogger(logger_name)
         return logger
     except Exception as exp:
         raise exp
 
 
+LOGGER = setup_logging(LOGGING_CONFIG, None)
+
+
 # import the wonderful Beautiful Soup and the URL grabber
 
 
 class AbstractGetBinDataClass(ABC):
     """An abstract class that can be imported to handle the data recieved from the provided
     council class.
 
@@ -52,64 +51,34 @@
         address_url -- the url to get the data from
         """
         this_url = address_url
         this_postcode = kwargs.get("postcode", None)
         this_paon = kwargs.get("paon", None)
         this_uprn = kwargs.get("uprn", None)
         this_usrn = kwargs.get("usrn", None)
-        this_web_driver = kwargs.get("web_driver", None)
-        this_headless = kwargs.get("headless", None)
         skip_get_url = kwargs.get("skip_get_url", None)
         dev_mode = kwargs.get("dev_mode", False)
         council_module_str = kwargs.get("council_module_str", None)
         if (
-            not skip_get_url or skip_get_url is False
+                not skip_get_url or skip_get_url is False
         ):  # we will not use the generic way to get data - needs a get data in the council class itself
             page = self.get_data(address_url)
             bin_data_dict = self.parse_data(
-                page,
-                postcode=this_postcode,
-                paon=this_paon,
-                uprn=this_uprn,
-                usrn=this_usrn,
-                web_driver=this_web_driver,
-                headless=this_headless,
-                url=this_url,
+                page, postcode=this_postcode, paon=this_paon, uprn=this_uprn, usrn=this_usrn, url=this_url
             )
             json_output = self.output_json(bin_data_dict)
         else:
             bin_data_dict = self.parse_data(
-                "",
-                postcode=this_postcode,
-                paon=this_paon,
-                uprn=this_uprn,
-                usrn=this_usrn,
-                web_driver=this_web_driver,
-                headless=this_headless,
-                url=this_url,
+                "", postcode=this_postcode, paon=this_paon, uprn=this_uprn, usrn=this_usrn
             )
             json_output = self.output_json(bin_data_dict)
 
-        # if dev mode create/update council's entry in the input.json
-        if dev_mode is not None and dev_mode is True:
-            cwd = os.getcwd()
-            input_file_path = os.path.join(
-                cwd, "uk_bin_collection", "tests", "input.json"
-            )
-            update_input_json(
-                council_module_str,
-                this_url,
-                input_file_path,
-                postcode=this_postcode,
-                paon=this_paon,
-                uprn=this_uprn,
-                usrn=this_usrn,
-                web_driver=this_web_driver,
-                skip_get_url=skip_get_url,
-            )
+        # if dev mode create/update council's output JSON if bin_data_dict is not empty
+        if dev_mode is not None and dev_mode is True and bin_data_dict["bins"]:
+            write_output_json(council_module_str, json_output)
 
         return json_output
 
     @classmethod
     def get_data(cls, url) -> str:
         """This method makes the request to the council
 
@@ -125,24 +94,24 @@
         requests.packages.urllib3.disable_warnings()
 
         # Make the Request - change the URL - find out your property number
         try:
             full_page = requests.get(url, headers, verify=False)
             return full_page
         except requests.exceptions.HTTPError as errh:
-            _LOGGER.error(f"Http Error: {errh}")
+            LOGGER.error(f"Http Error: {errh}")
             raise
         except requests.exceptions.ConnectionError as errc:
-            _LOGGER.error(f"Error Connecting: {errc}")
+            LOGGER.error(f"Error Connecting: {errc}")
             raise
         except requests.exceptions.Timeout as errt:
-            _LOGGER.error(f"Timeout Error: {errt}")
+            LOGGER.error(f"Timeout Error: {errt}")
             raise
         except requests.exceptions.RequestException as err:
-            _LOGGER.error(f"Oops: Something Else {err}")
+            LOGGER.error(f"Oops: Something Else {err}")
             raise
 
     @abstractmethod
     def parse_data(self, page: str, **kwargs) -> dict:
         """Abstract method that takes a page as a string
 
         Keyword arguments:
```

