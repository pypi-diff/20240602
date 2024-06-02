# Comparing `tmp/crewcal-0.8.1.tar.gz` & `tmp/crewcal-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crewcal-0.8.1.tar", max compression
+gzip compressed data, was "crewcal-0.8.2.tar", max compression
```

## Comparing `crewcal-0.8.1.tar` & `crewcal-0.8.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     1072 2023-11-15 18:40:52.098605 crewcal-0.8.1/LICENSE.txt
--rwxr-xr-x   0        0        0     7452 2023-11-21 02:30:03.671316 crewcal-0.8.1/README.md
--rwxr-xr-x   0        0        0     3697 2023-11-21 02:49:07.099357 crewcal-0.8.1/pyproject.toml
--rwxr-xr-x   0        0        0       85 2023-11-15 18:40:51.747749 crewcal-0.8.1/src/crewcal/__init__.py
--rw-r--r--   0        0        0     4445 2023-11-21 02:41:08.084443 crewcal-0.8.1/src/crewcal/cli.py
--rw-r--r--   0        0        0     6484 2023-11-21 02:45:17.743610 crewcal-0.8.1/src/crewcal/llm_extract.py
--rw-r--r--   0        0        0      988 2023-11-21 01:13:38.599942 crewcal-0.8.1/src/crewcal/llm_prompts.py
--rw-r--r--   0        0        0     4816 2023-11-21 02:00:00.523000 crewcal-0.8.1/src/crewcal/schedule.py
--rwxr-xr-x   0        0        0      456 2023-11-21 02:02:27.847994 crewcal-0.8.1/src/crewcal/wip.py
--rw-r--r--   0        0        0     8419 1970-01-01 00:00:00.000000 crewcal-0.8.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-11-15 18:40:52.000000 crewcal-0.8.2/LICENSE.txt
+-rwxr-xr-x   0        0        0     7855 2023-11-21 16:08:57.000000 crewcal-0.8.2/README.md
+-rwxr-xr-x   0        0        0     3697 2024-06-02 00:22:18.757462 crewcal-0.8.2/pyproject.toml
+-rwxr-xr-x   0        0        0       85 2023-11-15 18:40:51.000000 crewcal-0.8.2/src/crewcal/__init__.py
+-rwxr-xr-x   0        0        0     4438 2023-11-22 03:23:40.000000 crewcal-0.8.2/src/crewcal/cli.py
+-rwxr-xr-x   0        0        0     6484 2023-11-21 02:45:17.000000 crewcal-0.8.2/src/crewcal/llm_extract.py
+-rwxr-xr-x   0        0        0     1111 2024-06-02 00:12:35.589206 crewcal-0.8.2/src/crewcal/llm_prompts.py
+-rwxr-xr-x   0        0        0     4818 2024-06-02 00:20:14.218983 crewcal-0.8.2/src/crewcal/schedule.py
+-rwxr-xr-x   0        0        0      451 2024-06-02 00:18:17.862998 crewcal-0.8.2/src/crewcal/wip.py
+-rw-r--r--   0        0        0     8873 1970-01-01 00:00:00.000000 crewcal-0.8.2/PKG-INFO
```

### Comparing `crewcal-0.8.1/LICENSE.txt` & `crewcal-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crewcal-0.8.1/README.md` & `crewcal-0.8.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -97,23 +97,24 @@
 <!-- ABOUT THE PROJECT -->
 ## About the Project
 
 <div  align="center">
   <a href="https://github.com/EJOOSTEROP/crewcal">
     <img src="https://github.com/EJOOSTEROP/crewcal/blob/main/etc/intro_image.jpg?raw=true" alt="intro_image" width="75%" height="75%">
   </a>
+  <br>
 </div>
 
 <div>
-
+  <br>
   Convert an airline crew schedule pdf into iCalendar format using a machine learning Large Language Model. An LLM (Large Language Model, specifically OpenAI's gpt-3.5-turbo) is used to extract the schedule information. iCalender files are recognized by most calendar systems (iOS, Android, Google, ++) and will create the flights on your phone/device calendar.
 
   The PDF schedule does not need to follow a very prescribed structured format.
 
-  Development performed mostly using AIMS eCrew pdf schedules.
+  Development performed mostly using AIMS eCrew <a href="https://github.com/EJOOSTEROP/crewcal/blob/main/etc/schedule_sample.png?raw=true">pdf schedules</a>. It may work on other systems' schedules. Feel free to <a href="#roadmap">suggest</a> other systems.
 
 </div>
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- BUILT WITH -->
@@ -172,15 +173,15 @@
 The resulting .ics file can be read by most calendar software.
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- ROADMAP -->
 ## Roadmap
 
-- [ ] None (feel free to suggest)
+- [ ] Add support schedules for systems in addition to AIMS. I would be happy to look at suggestions, especially if you can provide sample schedules. Create a new <a href="https://github.com/EJOOSTEROP/crewcal/issues">issue</a>.
 
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- CONTRIBUTING -->
 ## Contributing
```

#### html2text {}

```diff
@@ -38,21 +38,23 @@
    3. _U_s_a_g_e
    4. _R_o_a_d_m_a_p
    5. _C_o_n_t_r_i_b_u_t_i_n_g
    6. _C_o_n_t_a_c_t
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## About the Project
                                  _[_i_n_t_r_o___i_m_a_g_e_]
+
 Convert an airline crew schedule pdf into iCalendar format using a machine
 learning Large Language Model. An LLM (Large Language Model, specifically
 OpenAI's gpt-3.5-turbo) is used to extract the schedule information. iCalender
 files are recognized by most calendar systems (iOS, Android, Google, ++) and
 will create the flights on your phone/device calendar. The PDF schedule does
 not need to follow a very prescribed structured format. Development performed
-mostly using AIMS eCrew pdf schedules.
+mostly using AIMS eCrew _p_d_f_ _s_c_h_e_d_u_l_e_s. It may work on other systems' schedules.
+Feel free to _s_u_g_g_e_s_t other systems.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Getting Started ### Prerequisites Obtain an OpenAI API key. Make this
 available as an environment variable: ```shell export OPENAI_API_KEY=YOUR_KEY
 ``` Alternatively specify the API Key in a .env file.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Installation Strongly consider using pipx or a virtual environment
 depending on your needs. ```shell pip install crewcal ```
@@ -62,15 +64,17 @@
 `crewcal --help` shows a brief manual page. ### Python Package The following
 sript extracts the schedule from `schedule.pdf` and stores the icalendar file
 in `schedule.ics` file. ```python from crewcal.llm_extract import
 OpenAISchedule sched = OpenAISchedule(schedule_path='schedule.pdf',
 to_icalendar_file='schedule.ics') ``` The resulting .ics file can be read by
 most calendar software.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Roadmap - [ ] None (feel free to suggest)
+## Roadmap - [ ] Add support schedules for systems in addition to AIMS. I would
+be happy to look at suggestions, especially if you can provide sample
+schedules. Create a new _i_s_s_u_e.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contributing Any contributions you make are **greatly appreciated**. If you
 have a suggestion that would make this better, please fork the repo and create
 a pull request. You can also [open](https://github.com/EJOOSTEROP/crewcal/
 issues/new/choose) a feature request or bug report. Don't forget to give the
 project a star! Thanks again! 1. Fork the Project 2. Create your Feature Branch
 (`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git commit
```

### Comparing `crewcal-0.8.1/pyproject.toml` & `crewcal-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 skip = [".gitignore", ".dockerignore"]
 
 [tool.mypy]
 disallow_incomplete_defs = true
 
 [tool.poetry]
 name = "crewcal"
-version = "0.8.1"
+version = "0.8.2"
 description = "Convert an airline crew schedule pdf into iCalendar format."
 authors = ["Erik Oosterop <ni7h4txi@duck.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/EJOOSTEROP/crewcal"
 repository = "https://github.com/EJOOSTEROP/crewcal"
 documentation = "https://github.com/EJOOSTEROP/crewcal"
```

### Comparing `crewcal-0.8.1/src/crewcal/cli.py` & `crewcal-0.8.2/src/crewcal/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,28 +119,25 @@
         )
         source_path = source_path_modified
 
     with Halo(
         text="Extracting schedule, saving to iCalendar format.", spinner="dots"
     ) if not to_json else Halo(
         text="Extracting schedule, saving to crewcal json format.", spinner="dots"
-    ):
-        sched = (
+    ) as spinner:
+        (
             OpenAISchedule(
                 schedule_path=str(source_path), to_icalendar_file=str(out_path)
             )
             if not to_json
             else OpenAISchedule(
                 schedule_path=str(source_path), to_json_file=str(out_path)
             )
         )
-
-    click.echo(f"Extracted schedule saved to {out_path}.")
-
-    del sched
+        spinner.info(f"Extracted schedule saved to {out_path}.")
 
     return 0
 
 
 cli.add_command(convert)
 cli.add_command(extract)
```

### Comparing `crewcal-0.8.1/src/crewcal/llm_extract.py` & `crewcal-0.8.2/src/crewcal/llm_extract.py`

 * *Files identical despite different names*

### Comparing `crewcal-0.8.1/src/crewcal/llm_prompts.py` & `crewcal-0.8.2/src/crewcal/llm_prompts.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,13 +14,15 @@
 - Summary which contains the origin and departure airports
 - Origin airport code. Sometimes multiple flights exist. Capture all origin airports.
 - Origin airport name
 - Origin timezone in ISO 8601 format (for example 'America/Toronto')
 - Destination airport code
 - Destination airport name
 - Destination timezone
-- Arrival date
-- Arrival time, the last occurrence of a time for each day
+- Arrival date. A '+1' means the next day.
+- Arrival time, the last occurrence of a time for each day. A '+1' means the next day.
 - List of crew members
-- A list of all times found
-- List of all airport codes
+- A list of all times found.
+- List of all airport codes.
+
+Always include all items in your output even if they are empty.
 """
```

### Comparing `crewcal-0.8.1/src/crewcal/schedule.py` & `crewcal-0.8.2/src/crewcal/schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Classes defining a flight schedule for an airline crew member.
 
 The schedule is a list of events, each of which contains the details of a set of flight.
 
 """
+
 import json
 import logging
 from pathlib import Path
 from typing import List
 
 import ics
 import pendulum
@@ -100,14 +101,15 @@
                 name=flight.summary,
                 description=flight.get_description(),
                 begin=flight.get_begin(),
                 end=flight.get_end(),
             )
             for flight in self.events
         ]
+
         calendar.events.update(events)
 
         return calendar
 
     def to_icalendar_file(self, filename: str) -> None:
         """Write the iCalendar representation of the schedule to a file.
```

### Comparing `crewcal-0.8.1/PKG-INFO` & `crewcal-0.8.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: crewcal
-Version: 0.8.1
+Version: 0.8.2
 Summary: Convert an airline crew schedule pdf into iCalendar format.
 Home-page: https://github.com/EJOOSTEROP/crewcal
 License: MIT
 Keywords: x,y,z
 Author: Erik Oosterop
 Author-email: ni7h4txi@duck.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: ics (>=0.7.2,<0.8.0)
 Requires-Dist: langchain (>=0.0.337,<0.0.338)
 Requires-Dist: openai (>=1.3.3,<2.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: pydantic (>=2.5.1,<3.0.0)
@@ -123,23 +124,24 @@
 <!-- ABOUT THE PROJECT -->
 ## About the Project
 
 <div  align="center">
   <a href="https://github.com/EJOOSTEROP/crewcal">
     <img src="https://github.com/EJOOSTEROP/crewcal/blob/main/etc/intro_image.jpg?raw=true" alt="intro_image" width="75%" height="75%">
   </a>
+  <br>
 </div>
 
 <div>
-
+  <br>
   Convert an airline crew schedule pdf into iCalendar format using a machine learning Large Language Model. An LLM (Large Language Model, specifically OpenAI's gpt-3.5-turbo) is used to extract the schedule information. iCalender files are recognized by most calendar systems (iOS, Android, Google, ++) and will create the flights on your phone/device calendar.
 
   The PDF schedule does not need to follow a very prescribed structured format.
 
-  Development performed mostly using AIMS eCrew pdf schedules.
+  Development performed mostly using AIMS eCrew <a href="https://github.com/EJOOSTEROP/crewcal/blob/main/etc/schedule_sample.png?raw=true">pdf schedules</a>. It may work on other systems' schedules. Feel free to <a href="#roadmap">suggest</a> other systems.
 
 </div>
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- BUILT WITH -->
@@ -198,15 +200,15 @@
 The resulting .ics file can be read by most calendar software.
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- ROADMAP -->
 ## Roadmap
 
-- [ ] None (feel free to suggest)
+- [ ] Add support schedules for systems in addition to AIMS. I would be happy to look at suggestions, especially if you can provide sample schedules. Create a new <a href="https://github.com/EJOOSTEROP/crewcal/issues">issue</a>.
 
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- CONTRIBUTING -->
 ## Contributing
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: crewcal Version: 0.8.1 Summary: Convert an airline
+Metadata-Version: 2.1 Name: crewcal Version: 0.8.2 Summary: Convert an airline
 crew schedule pdf into iCalendar format. Home-page: https://github.com/
 EJOOSTEROP/crewcal License: MIT Keywords: x,y,z Author: Erik Oosterop Author-
 email: ni7h4txi@duck.com Requires-Python: >=3.11,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: click
-(>=8.1.7,<9.0.0) Requires-Dist: halo (>=0.0.31,<0.0.32) Requires-Dist: ics
-(>=0.7.2,<0.8.0) Requires-Dist: langchain (>=0.0.337,<0.0.338) Requires-Dist:
-openai (>=1.3.3,<2.0.0) Requires-Dist: pendulum (>=2.1.2,<3.0.0) Requires-Dist:
-pydantic (>=2.5.1,<3.0.0) Requires-Dist: pypdf (>=3.17.1,<4.0.0) Requires-Dist:
-python-dotenv (>=1.0.0,<2.0.0) Project-URL: Documentation, https://github.com/
-EJOOSTEROP/crewcal Project-URL: Repository, https://github.com/EJOOSTEROP/
-crewcal Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Requires-Dist: click (>=8.1.7,<9.0.0) Requires-Dist:
+halo (>=0.0.31,<0.0.32) Requires-Dist: ics (>=0.7.2,<0.8.0) Requires-Dist:
+langchain (>=0.0.337,<0.0.338) Requires-Dist: openai (>=1.3.3,<2.0.0) Requires-
+Dist: pendulum (>=2.1.2,<3.0.0) Requires-Dist: pydantic (>=2.5.1,<3.0.0)
+Requires-Dist: pypdf (>=3.17.1,<4.0.0) Requires-Dist: python-dotenv
+(>=1.0.0,<2.0.0) Project-URL: Documentation, https://github.com/EJOOSTEROP/
+crewcal Project-URL: Repository, https://github.com/EJOOSTEROP/crewcal
+Description-Content-Type: text/markdown
       [![Current Release][release-shield]][release-url] [![Contributors]
 [contributors-shield]][contributors-url] [![Forks][forks-shield]][forks-url] [!
 [Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]][issues-url]
  [![MIT License][license-shield]][license-url] [![LinkedIn][linkedin-shield]]
  [linkedin-url] ![PyPI - Python Version][pypi-python-shield] ![PyPi - Package
 Version][pypi-version-shield] [![PyPi - License][pypi-license-shield]][license-
     url] [release-shield]:https://img.shields.io/github/release/EJOOSTEROP/
@@ -51,21 +52,23 @@
    3. _U_s_a_g_e
    4. _R_o_a_d_m_a_p
    5. _C_o_n_t_r_i_b_u_t_i_n_g
    6. _C_o_n_t_a_c_t
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## About the Project
                                  _[_i_n_t_r_o___i_m_a_g_e_]
+
 Convert an airline crew schedule pdf into iCalendar format using a machine
 learning Large Language Model. An LLM (Large Language Model, specifically
 OpenAI's gpt-3.5-turbo) is used to extract the schedule information. iCalender
 files are recognized by most calendar systems (iOS, Android, Google, ++) and
 will create the flights on your phone/device calendar. The PDF schedule does
 not need to follow a very prescribed structured format. Development performed
-mostly using AIMS eCrew pdf schedules.
+mostly using AIMS eCrew _p_d_f_ _s_c_h_e_d_u_l_e_s. It may work on other systems' schedules.
+Feel free to _s_u_g_g_e_s_t other systems.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Getting Started ### Prerequisites Obtain an OpenAI API key. Make this
 available as an environment variable: ```shell export OPENAI_API_KEY=YOUR_KEY
 ``` Alternatively specify the API Key in a .env file.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Installation Strongly consider using pipx or a virtual environment
 depending on your needs. ```shell pip install crewcal ```
@@ -75,15 +78,17 @@
 `crewcal --help` shows a brief manual page. ### Python Package The following
 sript extracts the schedule from `schedule.pdf` and stores the icalendar file
 in `schedule.ics` file. ```python from crewcal.llm_extract import
 OpenAISchedule sched = OpenAISchedule(schedule_path='schedule.pdf',
 to_icalendar_file='schedule.ics') ``` The resulting .ics file can be read by
 most calendar software.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Roadmap - [ ] None (feel free to suggest)
+## Roadmap - [ ] Add support schedules for systems in addition to AIMS. I would
+be happy to look at suggestions, especially if you can provide sample
+schedules. Create a new _i_s_s_u_e.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contributing Any contributions you make are **greatly appreciated**. If you
 have a suggestion that would make this better, please fork the repo and create
 a pull request. You can also [open](https://github.com/EJOOSTEROP/crewcal/
 issues/new/choose) a feature request or bug report. Don't forget to give the
 project a star! Thanks again! 1. Fork the Project 2. Create your Feature Branch
 (`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git commit
```

