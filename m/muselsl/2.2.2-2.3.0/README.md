# Comparing `tmp/muselsl-2.2.2.tar.gz` & `tmp/muselsl-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\danomorrison\muse-lsl\dist\.tmp-u9ht3p3i\muselsl-2.2.2.tar", last modified: Tue Jan  3 19:46:02 2023, max compression
+gzip compressed data, was "muselsl-2.3.0.tar", last modified: Sun Jun  2 18:23:16 2024, max compression
```

## Comparing `muselsl-2.2.2.tar` & `muselsl-2.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-01-03 19:46:02.482923 muselsl-2.2.2/
--rw-rw-rw-   0        0        0     1537 2023-01-03 19:39:28.000000 muselsl-2.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0       58 2023-01-03 19:39:28.000000 muselsl-2.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     9036 2023-01-03 19:46:02.482923 muselsl-2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     8214 2023-01-03 19:39:28.000000 muselsl-2.2.2/README.md
--rw-rw-rw-   0        0        0    96935 2023-01-03 19:39:28.000000 muselsl-2.2.2/blinks.png
-drwxrwxrwx   0        0        0        0 2023-01-03 19:46:02.370521 muselsl-2.2.2/muselsl/
--rw-rw-rw-   0        0        0      130 2023-01-03 19:39:28.000000 muselsl-2.2.2/muselsl/__init__.py
--rw-rw-rw-   0        0        0     2793 2023-01-03 19:39:28.000000 muselsl-2.2.2/muselsl/__main__.py
--rw-rw-rw-   0        0        0     2408 2023-01-03 19:41:36.000000 muselsl-2.2.2/muselsl/backends.py
--rw-rw-rw-   0        0        0     7767 2023-01-03 19:39:28.000000 muselsl-2.2.2/muselsl/cli.py
--rw-rw-rw-   0        0        0     2319 2023-01-03 19:39:28.000000 muselsl-2.2.2/muselsl/constants.py
-drwxrwxrwx   0        0        0        0 2023-01-03 19:46:02.480950 muselsl-2.2.2/muselsl/docs/
--rw-rw-rw-   0        0        0     8214 2023-01-03 19:46:02.000000 muselsl-2.2.2/muselsl/docs/README.md
--rw-rw-rw-   0        0        0      906 2023-01-03 19:39:28.000000 muselsl-2.2.2/muselsl/helper.py
--rw-rw-rw-   0        0        0    21212 2023-01-03 19:39:28.000000 muselsl-2.2.2/muselsl/muse.py
--rw-rw-rw-   0        0        0     7439 2023-01-03 19:39:28.000000 muselsl-2.2.2/muselsl/record.py
--rw-rw-rw-   0        0        0    11069 2023-01-03 19:39:28.000000 muselsl-2.2.2/muselsl/stream.py
--rw-rw-rw-   0        0        0      280 2023-01-03 19:39:28.000000 muselsl-2.2.2/muselsl/view.py
--rw-rw-rw-   0        0        0     6709 2023-01-03 19:39:28.000000 muselsl-2.2.2/muselsl/viewer_v1.py
--rw-rw-rw-   0        0        0     9172 2023-01-03 19:39:28.000000 muselsl-2.2.2/muselsl/viewer_v2.py
-drwxrwxrwx   0        0        0        0 2023-01-03 19:46:02.420090 muselsl-2.2.2/muselsl.egg-info/
--rw-rw-rw-   0        0        0     9036 2023-01-03 19:46:02.000000 muselsl-2.2.2/muselsl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-01-03 19:46:02.000000 muselsl-2.2.2/muselsl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-03 19:46:02.000000 muselsl-2.2.2/muselsl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-01-03 19:46:02.000000 muselsl-2.2.2/muselsl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-01-03 19:43:13.000000 muselsl-2.2.2/muselsl.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      102 2023-01-03 19:46:02.000000 muselsl-2.2.2/muselsl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-01-03 19:46:02.000000 muselsl-2.2.2/muselsl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      167 2023-01-03 19:46:02.491900 muselsl-2.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2459 2023-01-03 19:42:12.000000 muselsl-2.2.2/setup.py
+drwxr-xr-x   0 danomorrison   (501) staff       (20)        0 2024-06-02 18:23:16.435654 muselsl-2.3.0/
+-rw-r--r--   0 danomorrison   (501) staff       (20)     1514 2024-06-02 16:15:23.000000 muselsl-2.3.0/LICENSE.txt
+-rw-r--r--   0 danomorrison   (501) staff       (20)       56 2024-06-02 16:15:23.000000 muselsl-2.3.0/MANIFEST.in
+-rw-r--r--   0 danomorrison   (501) staff       (20)     9137 2024-06-02 18:23:16.435353 muselsl-2.3.0/PKG-INFO
+-rw-r--r--   0 danomorrison   (501) staff       (20)     8043 2024-06-02 16:15:23.000000 muselsl-2.3.0/README.md
+-rw-r--r--   0 danomorrison   (501) staff       (20)    96935 2024-06-02 16:15:23.000000 muselsl-2.3.0/blinks.png
+drwxr-xr-x   0 danomorrison   (501) staff       (20)        0 2024-06-02 18:23:16.417539 muselsl-2.3.0/muselsl/
+-rw-r--r--   0 danomorrison   (501) staff       (20)      126 2024-06-02 18:11:44.000000 muselsl-2.3.0/muselsl/__init__.py
+-rw-r--r--   0 danomorrison   (501) staff       (20)     2732 2024-06-02 17:17:34.000000 muselsl-2.3.0/muselsl/__main__.py
+-rw-r--r--   0 danomorrison   (501) staff       (20)     3134 2024-06-02 17:42:25.000000 muselsl-2.3.0/muselsl/backends.py
+-rw-r--r--   0 danomorrison   (501) staff       (20)     8590 2024-06-02 18:04:58.000000 muselsl-2.3.0/muselsl/cli.py
+-rw-r--r--   0 danomorrison   (501) staff       (20)     2649 2024-06-02 17:50:32.000000 muselsl-2.3.0/muselsl/constants.py
+drwxr-xr-x   0 danomorrison   (501) staff       (20)        0 2024-06-02 18:23:16.433645 muselsl-2.3.0/muselsl/docs/
+-rw-r--r--   0 danomorrison   (501) staff       (20)     8043 2024-06-02 18:23:15.000000 muselsl-2.3.0/muselsl/docs/README.md
+-rw-r--r--   0 danomorrison   (501) staff       (20)      881 2024-06-02 16:15:23.000000 muselsl-2.3.0/muselsl/helper.py
+-rw-r--r--   0 danomorrison   (501) staff       (20)    20937 2024-06-02 18:07:37.000000 muselsl-2.3.0/muselsl/muse.py
+-rw-r--r--   0 danomorrison   (501) staff       (20)     8413 2024-06-02 17:17:34.000000 muselsl-2.3.0/muselsl/record.py
+-rw-r--r--   0 danomorrison   (501) staff       (20)    11169 2024-06-02 18:04:38.000000 muselsl-2.3.0/muselsl/stream.py
+-rw-r--r--   0 danomorrison   (501) staff       (20)      272 2024-06-02 16:15:23.000000 muselsl-2.3.0/muselsl/view.py
+-rw-r--r--   0 danomorrison   (501) staff       (20)     6529 2024-06-02 16:15:23.000000 muselsl-2.3.0/muselsl/viewer_v1.py
+-rw-r--r--   0 danomorrison   (501) staff       (20)     8912 2024-06-02 16:15:23.000000 muselsl-2.3.0/muselsl/viewer_v2.py
+drwxr-xr-x   0 danomorrison   (501) staff       (20)        0 2024-06-02 18:23:16.434499 muselsl-2.3.0/muselsl.egg-info/
+-rw-r--r--   0 danomorrison   (501) staff       (20)     9137 2024-06-02 18:23:16.000000 muselsl-2.3.0/muselsl.egg-info/PKG-INFO
+-rw-r--r--   0 danomorrison   (501) staff       (20)      528 2024-06-02 18:23:16.000000 muselsl-2.3.0/muselsl.egg-info/SOURCES.txt
+-rw-r--r--   0 danomorrison   (501) staff       (20)        1 2024-06-02 18:23:16.000000 muselsl-2.3.0/muselsl.egg-info/dependency_links.txt
+-rw-r--r--   0 danomorrison   (501) staff       (20)       50 2024-06-02 18:23:16.000000 muselsl-2.3.0/muselsl.egg-info/entry_points.txt
+-rw-r--r--   0 danomorrison   (501) staff       (20)        1 2024-06-02 16:22:44.000000 muselsl-2.3.0/muselsl.egg-info/not-zip-safe
+-rw-r--r--   0 danomorrison   (501) staff       (20)      102 2024-06-02 18:23:16.000000 muselsl-2.3.0/muselsl.egg-info/requires.txt
+-rw-r--r--   0 danomorrison   (501) staff       (20)        8 2024-06-02 18:23:16.000000 muselsl-2.3.0/muselsl.egg-info/top_level.txt
+-rw-r--r--   0 danomorrison   (501) staff       (20)      155 2024-06-02 18:23:16.437335 muselsl-2.3.0/setup.cfg
+-rw-r--r--   0 danomorrison   (501) staff       (20)     2389 2024-06-02 18:17:53.000000 muselsl-2.3.0/setup.py
```

### Comparing `muselsl-2.2.2/LICENSE.txt` & `muselsl-2.3.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Copyright © 2018, authors of muselsl
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-    * Redistributions of source code must retain the above copyright
-      notice, this list of conditions and the following disclaimer.
-    * Redistributions in binary form must reproduce the above copyright
-      notice, this list of conditions and the following disclaimer in the
-      documentation and/or other materials provided with the distribution.
-    * Neither the names of muselsl authors nor the names of any
-      contributors may be used to endorse or promote products derived from
-      this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR ANY
-DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+Copyright © 2018, authors of muselsl
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+    * Redistributions of source code must retain the above copyright
+      notice, this list of conditions and the following disclaimer.
+    * Redistributions in binary form must reproduce the above copyright
+      notice, this list of conditions and the following disclaimer in the
+      documentation and/or other materials provided with the distribution.
+    * Neither the names of muselsl authors nor the names of any
+      contributors may be used to endorse or promote products derived from
+      this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR ANY
+DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
+ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `muselsl-2.2.2/PKG-INFO` & `muselsl-2.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,193 +1,204 @@
-Metadata-Version: 2.1
-Name: muselsl
-Version: 2.2.2
-Summary: Stream and visualize EEG data from the Muse headset.
-Home-page: https://github.com/alexandrebarachant/muse-lsl/
-Author: Alexandre Barachant
-Author-email: alexandre.barachant@gmail.com
-License: BSD (3-clause)
-Keywords: muse lsl eeg ble neuroscience
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Software Development
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown
-Provides-Extra: Viewer V2
-License-File: LICENSE.txt
-
-
-[![DOI](https://zenodo.org/badge/80209610.svg)](https://zenodo.org/badge/latestdoi/80209610)
-
-# Muse LSL
-
-A Python package for streaming, visualizing, and recording EEG data from the Muse devices developed by InteraXon.
-
-![Blinks](blinks.png)
-
-## Requirements
-
-The code relies on a number of different bluetooth backends for connecting to the muse. We recommend using the `bleak` backend (enabled by default), but you may be interested in [BlueMuse](https://github.com/kowalej/BlueMuse/tree/master/Dist) for a GUI to discover and connect to Muse devices on Windows or [bgapi] if you are on a Mac with a BLED112 dongle. 
-
-**Compatible with Python 2.7 and Python 3.x**
-
-**Compatible with Muse 2, Muse S, and the classic Muse (2016)**
-
-_Note: if you run into any issues, first check out out [Common Issues](#common-issues) and then the [Issues](https://github.com/alexandrebarachant/muse-lsl/issues) section of this repository_
-
-## Getting Started
-
-### Installation
-
-Install Muse LSL with pip
-
-    pip install muselsl
-
-### Setting Up a Stream
-
-On Windows 10, we recommend using the [BlueMuse](https://github.com/kowalej/BlueMuse/tree/master/Dist) GUI to set up an LSL stream. On Mac and Linux, the easiest way to get Muse data is to use Muse LSL directly from the command line. Use the `-h` flag to get a comprehensive list of all commands and options.
-
-To print a list of available muses:
-
-    $ muselsl list
-
-To begin an LSL stream from the first available Muse:
-
-    $ muselsl stream  
-
-To connect to a specific Muse you can pass the name of the device as an argument. Device names can be found on the inside of the left earpiece (e.g. Muse-41D2):
-
-    $ muselsl stream --name YOUR_DEVICE_NAME
-
-You can also directly pass the MAC address of your Muse. This provides the benefit of bypassing the device discovery step and can make connecting to devices quicker and more reliable:
-
-    $ muselsl stream --address YOUR_DEVICE_ADDRESS
-
-### Working with Streaming Data
-
-Once an LSL stream is created, you have access to the following commands.
-
-*Note: the process running the `stream` command must be kept alive in order to maintain the LSL stream. These following commands should be run in another terminal or second process*
-
-To view data:
-
-    $ muselsl view
-
-If the visualization freezes or is laggy, you can also try the alternate version 2 of the viewer. *Note: this will require the additional [vispy](https://github.com/vispy/vispy) and [mne](https://github.com/mne-tools/mne-python) dependencies*
-
-    $ muselsl view --version 2
-
-To record EEG data into a CSV:
-
-    $ muselsl record --duration 60  
-
-*Note: this command will also save data from any LSL stream containing 'Markers' data, such as from the stimulus presentation scripts in [EEG Notebooks](https://github.com/neurotechx/eeg-notebooks)*
-
-Alternatively, you can record data directly without using LSL through the following command:
-
-    $ muselsl record_direct --duration 60
-
-_Note: direct recording does not allow 'Markers' data to be recorded_
-
-## Running Experiments
-
-Muse LSL was designed so that the Muse could be used to run a number of classic EEG experiments, including the [P300 event-related potential](http://alexandre.barachant.org/blog/2017/02/05/P300-with-muse.html) and the SSVEP and SSAEP evoked potentials.
-
-The code to perform these experiments is still available, but is now maintained in the [EEG Notebooks](https://github.com/neurotechx/eeg-notebooks) repository by the [NeuroTechX](https://neurotechx.com) community.
-
-## Usage as a Library
-
-If you want to integrate Muse LSL into your own Python project, you can import and use its functions as you would any Python library. Examples are available in the `examples` folder:
-
-```Python
-from muselsl import stream, list_muses
-
-muses = list_muses()
-stream(muses[0]['address'])
-
-# Note: Streaming is synchronous, so code here will not execute until after the stream has been closed
-print('Stream has ended')
-```
-
-## Alternate Data Types
-
-In addition to EEG, the Muse also provides data from an accelerometer, gyroscope, and, in the case of the Muse 2, a photoplethysmography (PPG) sensor. These data types can be enabled via command line arguments or by passing the correct parameters to the `stream` function. Once enabled, PPG, accelerometer, and gyroscope data will streamed in their own separate LSL streams named "PPG", "ACC", and "GYRO", respectively.
-
-To stream data from all sensors in a Muse 2 from the command line:
-
-    muselsl stream --ppg --acc --gyro
-
-As a library function:
-
-```Python
-from muselsl import stream, list_muses
-
-muses = list_muses()
-stream(muses[0]['address'], ppg_enabled=True, acc_enabled=True, gyro_enabled=True)
-```
-
-To record data from an alternate data source:
-
-    muselsl record --type ACC
-
-*Note: The record process will only record from one data type at a time. However, multiple terminals or processes can be used to record from multiple data types simultaneously*
-
-## What is LSL?
-
-Lab Streaming Layer or LSL is a system designed to unify the collection of time series data for research experiments. It has become standard in the field of EEG-based brain-computer interfaces for its ability to make seperate streams of data available on a network with time synchronization and near real-time access. For more information, check out this [lecture from Modern Brain-Computer Interface Design](https://www.youtube.com/watch?v=Y1at7yrcFW0) or the [LSL repository](https://github.com/sccn/labstreaminglayer)
-
-## Common Issues
-
-### Mac and Windows
-
-1.  Connection issues with BLED112 dongle:
-
-- You may need to use the `--interface` argument to provide the appropriate COM port value for the BLED112 device. The default value is COM9. To setup or view the device's COM port go to your OS's system settings
-
-### Linux
-
-1.  `pygatt.exceptions.BLEError: Unexpected error when scanning: Set scan parameters failed: Operation not permitted` (Linux)
-
-- This is an issue with pygatt requiring root privileges to run a scan. Make sure you [have `libcap` installed](https://askubuntu.com/questions/347788/how-can-i-install-libpcap-header-files-on-ubuntu-12-04) and run `` sudo setcap 'cap_net_raw,cap_net_admin+eip' `which hcitool` ``
-
-2.  `pygatt.exceptions.BLEError: No characteristic found matching 273e0003-4c4d-454d-96be-f03bac821358` (Linux)
-
-- There is a problem with the most recent version of pygatt. Work around this by downgrading to 3.1.1: `pip install pygatt==3.1.1`
-
-3.  `pygatt.exceptions.BLEError: No BLE adapter found` (Linux)
-
-- Make sure your computer's Bluetooth is turned on.
-
-4.  `pygatt.exceptions.BLEError: Unexpected error when scanning: Set scan parameters failed: Connection timed out` (Linux)
-
-- This seems to be due to a OS-level Bluetooth crash. Try turning your computer's bluetooth off and on again
-
-5.  `'RuntimeError: could not create stream outlet'` (Linux)
-
-- This appears to be due to Linux-specific issues with the newest version of pylsl. Ensure that you have pylsl 1.10.5 installed in the environment in which you are trying to run Muse LSL
-- If this is preceded by `Could not instantiate IPv4 stack: getrandom`, it could be [this issue](https://github.com/boostorg/uuid/issues/91) which can be resolved by building `liblsl` with `-DBOOST_UUID_RANDOM_PROVIDER_FORCE_POSIX` (e.g. by editing `standalone_compilation_linux.sh`)
-
-## Citing muse-lsl
-
-```
-@misc{muse-lsl,
-  author       = {Alexandre Barachant and
-                  Dano Morrison and
-                  Hubert Banville and
-                  Jason Kowaleski and
-                  Uri Shaked and
-                  Sylvain Chevallier and
-                  Juan JesÃºs Torre Tresols},
-  title        = {muse-lsl},
-  month        = may,
-  year         = 2019,
-  doi          = {10.5281/zenodo.3228861},
-  url          = {https://doi.org/10.5281/zenodo.3228861}
-}
-```
-
-> Alexandre Barachant, Dano Morrison, Hubert Banville, Jason Kowaleski, Uri Shaked, Sylvain Chevallier, & Juan JesÃºs Torre Tresols. (2019, May 25). muse-lsl (Version v2.0.2). Zenodo. http://doi.org/10.5281/zenodo.3228861
+Metadata-Version: 2.1
+Name: muselsl
+Version: 2.3.0
+Summary: Stream and visualize EEG data from the Muse headset.
+Home-page: https://github.com/alexandrebarachant/muse-lsl/
+Author: Alexandre Barachant
+Author-email: alexandre.barachant@gmail.com
+License: BSD (3-clause)
+Keywords: muse lsl eeg ble neuroscience
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Software Development
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: bitstring
+Requires-Dist: bleak>=0.18.0
+Requires-Dist: pygatt
+Requires-Dist: pandas
+Requires-Dist: scikit-learn
+Requires-Dist: numpy
+Requires-Dist: seaborn
+Requires-Dist: pexpect
+Requires-Dist: pylsl
+Provides-Extra: viewer-v2
+Requires-Dist: mne; extra == "viewer-v2"
+Requires-Dist: vispy; extra == "viewer-v2"
+
+
+[![DOI](https://zenodo.org/badge/80209610.svg)](https://zenodo.org/badge/latestdoi/80209610)
+
+# Muse LSL
+
+A Python package for streaming, visualizing, and recording EEG data from the Muse devices developed by InteraXon.
+
+![Blinks](blinks.png)
+
+## Requirements
+
+The code relies on a number of different bluetooth backends for connecting to the muse. We recommend using the `bleak` backend (enabled by default), but you may be interested in [BlueMuse](https://github.com/kowalej/BlueMuse/tree/master/Dist) for a GUI to discover and connect to Muse devices on Windows or [bgapi] if you are on a Mac with a BLED112 dongle. 
+
+**Compatible with Python 2.7 and Python 3.x**
+
+**Compatible with Muse 2, Muse S, and the classic Muse (2016)**
+
+_Note: if you run into any issues, first check out out [Common Issues](#common-issues) and then the [Issues](https://github.com/alexandrebarachant/muse-lsl/issues) section of this repository_
+
+## Getting Started
+
+### Installation
+
+Install Muse LSL with pip
+
+    pip install muselsl
+
+### Setting Up a Stream
+
+On Windows 10, we recommend using the [BlueMuse](https://github.com/kowalej/BlueMuse/tree/master/Dist) GUI to set up an LSL stream. On Mac and Linux, the easiest way to get Muse data is to use Muse LSL directly from the command line. Use the `-h` flag to get a comprehensive list of all commands and options.
+
+To print a list of available muses:
+
+    $ muselsl list
+
+To begin an LSL stream from the first available Muse:
+
+    $ muselsl stream  
+
+To connect to a specific Muse you can pass the name of the device as an argument. Device names can be found on the inside of the left earpiece (e.g. Muse-41D2):
+
+    $ muselsl stream --name YOUR_DEVICE_NAME
+
+You can also directly pass the MAC address of your Muse. This provides the benefit of bypassing the device discovery step and can make connecting to devices quicker and more reliable:
+
+    $ muselsl stream --address YOUR_DEVICE_ADDRESS
+
+### Working with Streaming Data
+
+Once an LSL stream is created, you have access to the following commands.
+
+*Note: the process running the `stream` command must be kept alive in order to maintain the LSL stream. These following commands should be run in another terminal or second process*
+
+To view data:
+
+    $ muselsl view
+
+If the visualization freezes or is laggy, you can also try the alternate version 2 of the viewer. *Note: this will require the additional [vispy](https://github.com/vispy/vispy) and [mne](https://github.com/mne-tools/mne-python) dependencies*
+
+    $ muselsl view --version 2
+
+To record EEG data into a CSV:
+
+    $ muselsl record --duration 60  
+
+*Note: this command will also save data from any LSL stream containing 'Markers' data, such as from the stimulus presentation scripts in [EEG Notebooks](https://github.com/neurotechx/eeg-notebooks)*
+
+Alternatively, you can record data directly without using LSL through the following command:
+
+    $ muselsl record_direct --duration 60
+
+_Note: direct recording does not allow 'Markers' data to be recorded_
+
+## Running Experiments
+
+Muse LSL was designed so that the Muse could be used to run a number of classic EEG experiments, including the [P300 event-related potential](http://alexandre.barachant.org/blog/2017/02/05/P300-with-muse.html) and the SSVEP and SSAEP evoked potentials.
+
+The code to perform these experiments is still available, but is now maintained in the [EEG Notebooks](https://github.com/neurotechx/eeg-notebooks) repository by the [NeuroTechX](https://neurotechx.com) community.
+
+## Usage as a Library
+
+If you want to integrate Muse LSL into your own Python project, you can import and use its functions as you would any Python library. Examples are available in the `examples` folder:
+
+```Python
+from muselsl import stream, list_muses
+
+muses = list_muses()
+stream(muses[0]['address'])
+
+# Note: Streaming is synchronous, so code here will not execute until after the stream has been closed
+print('Stream has ended')
+```
+
+## Alternate Data Types
+
+In addition to EEG, the Muse also provides data from an accelerometer, gyroscope, and, in the case of the Muse 2, a photoplethysmography (PPG) sensor. These data types can be enabled via command line arguments or by passing the correct parameters to the `stream` function. Once enabled, PPG, accelerometer, and gyroscope data will streamed in their own separate LSL streams named "PPG", "ACC", and "GYRO", respectively.
+
+To stream data from all sensors in a Muse 2 from the command line:
+
+    muselsl stream --ppg --acc --gyro
+
+As a library function:
+
+```Python
+from muselsl import stream, list_muses
+
+muses = list_muses()
+stream(muses[0]['address'], ppg_enabled=True, acc_enabled=True, gyro_enabled=True)
+```
+
+To record data from an alternate data source:
+
+    muselsl record --type ACC
+
+*Note: The record process will only record from one data type at a time. However, multiple terminals or processes can be used to record from multiple data types simultaneously*
+
+## What is LSL?
+
+Lab Streaming Layer or LSL is a system designed to unify the collection of time series data for research experiments. It has become standard in the field of EEG-based brain-computer interfaces for its ability to make seperate streams of data available on a network with time synchronization and near real-time access. For more information, check out this [lecture from Modern Brain-Computer Interface Design](https://www.youtube.com/watch?v=Y1at7yrcFW0) or the [LSL repository](https://github.com/sccn/labstreaminglayer)
+
+## Common Issues
+
+### Mac and Windows
+
+1.  Connection issues with BLED112 dongle:
+
+- You may need to use the `--interface` argument to provide the appropriate COM port value for the BLED112 device. The default value is COM9. To setup or view the device's COM port go to your OS's system settings
+
+### Linux
+
+1.  `pygatt.exceptions.BLEError: Unexpected error when scanning: Set scan parameters failed: Operation not permitted` (Linux)
+
+- This is an issue with pygatt requiring root privileges to run a scan. Make sure you [have `libcap` installed](https://askubuntu.com/questions/347788/how-can-i-install-libpcap-header-files-on-ubuntu-12-04) and run `` sudo setcap 'cap_net_raw,cap_net_admin+eip' `which hcitool` ``
+
+2.  `pygatt.exceptions.BLEError: No characteristic found matching 273e0003-4c4d-454d-96be-f03bac821358` (Linux)
+
+- There is a problem with the most recent version of pygatt. Work around this by downgrading to 3.1.1: `pip install pygatt==3.1.1`
+
+3.  `pygatt.exceptions.BLEError: No BLE adapter found` (Linux)
+
+- Make sure your computer's Bluetooth is turned on.
+
+4.  `pygatt.exceptions.BLEError: Unexpected error when scanning: Set scan parameters failed: Connection timed out` (Linux)
+
+- This seems to be due to a OS-level Bluetooth crash. Try turning your computer's bluetooth off and on again
+
+5.  `'RuntimeError: could not create stream outlet'` (Linux)
+
+- This appears to be due to Linux-specific issues with the newest version of pylsl. Ensure that you have pylsl 1.10.5 installed in the environment in which you are trying to run Muse LSL
+- If this is preceded by `Could not instantiate IPv4 stack: getrandom`, it could be [this issue](https://github.com/boostorg/uuid/issues/91) which can be resolved by building `liblsl` with `-DBOOST_UUID_RANDOM_PROVIDER_FORCE_POSIX` (e.g. by editing `standalone_compilation_linux.sh`)
+
+## Citing muse-lsl
+
+```
+@misc{muse-lsl,
+  author       = {Alexandre Barachant and
+                  Dano Morrison and
+                  Hubert Banville and
+                  Jason Kowaleski and
+                  Uri Shaked and
+                  Sylvain Chevallier and
+                  Juan Jesús Torre Tresols},
+  title        = {muse-lsl},
+  month        = may,
+  year         = 2019,
+  doi          = {10.5281/zenodo.3228861},
+  url          = {https://doi.org/10.5281/zenodo.3228861}
+}
+```
+
+> Alexandre Barachant, Dano Morrison, Hubert Banville, Jason Kowaleski, Uri Shaked, Sylvain Chevallier, & Juan Jesús Torre Tresols. (2019, May 25). muse-lsl (Version v2.0.2). Zenodo. http://doi.org/10.5281/zenodo.3228861
```

### Comparing `muselsl-2.2.2/README.md` & `muselsl-2.3.0/README.md`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-
-[![DOI](https://zenodo.org/badge/80209610.svg)](https://zenodo.org/badge/latestdoi/80209610)
-
-# Muse LSL
-
-A Python package for streaming, visualizing, and recording EEG data from the Muse devices developed by InteraXon.
-
-![Blinks](blinks.png)
-
-## Requirements
-
-The code relies on a number of different bluetooth backends for connecting to the muse. We recommend using the `bleak` backend (enabled by default), but you may be interested in [BlueMuse](https://github.com/kowalej/BlueMuse/tree/master/Dist) for a GUI to discover and connect to Muse devices on Windows or [bgapi] if you are on a Mac with a BLED112 dongle. 
-
-**Compatible with Python 2.7 and Python 3.x**
-
-**Compatible with Muse 2, Muse S, and the classic Muse (2016)**
-
-_Note: if you run into any issues, first check out out [Common Issues](#common-issues) and then the [Issues](https://github.com/alexandrebarachant/muse-lsl/issues) section of this repository_
-
-## Getting Started
-
-### Installation
-
-Install Muse LSL with pip
-
-    pip install muselsl
-
-### Setting Up a Stream
-
-On Windows 10, we recommend using the [BlueMuse](https://github.com/kowalej/BlueMuse/tree/master/Dist) GUI to set up an LSL stream. On Mac and Linux, the easiest way to get Muse data is to use Muse LSL directly from the command line. Use the `-h` flag to get a comprehensive list of all commands and options.
-
-To print a list of available muses:
-
-    $ muselsl list
-
-To begin an LSL stream from the first available Muse:
-
-    $ muselsl stream  
-
-To connect to a specific Muse you can pass the name of the device as an argument. Device names can be found on the inside of the left earpiece (e.g. Muse-41D2):
-
-    $ muselsl stream --name YOUR_DEVICE_NAME
-
-You can also directly pass the MAC address of your Muse. This provides the benefit of bypassing the device discovery step and can make connecting to devices quicker and more reliable:
-
-    $ muselsl stream --address YOUR_DEVICE_ADDRESS
-
-### Working with Streaming Data
-
-Once an LSL stream is created, you have access to the following commands.
-
-*Note: the process running the `stream` command must be kept alive in order to maintain the LSL stream. These following commands should be run in another terminal or second process*
-
-To view data:
-
-    $ muselsl view
-
-If the visualization freezes or is laggy, you can also try the alternate version 2 of the viewer. *Note: this will require the additional [vispy](https://github.com/vispy/vispy) and [mne](https://github.com/mne-tools/mne-python) dependencies*
-
-    $ muselsl view --version 2
-
-To record EEG data into a CSV:
-
-    $ muselsl record --duration 60  
-
-*Note: this command will also save data from any LSL stream containing 'Markers' data, such as from the stimulus presentation scripts in [EEG Notebooks](https://github.com/neurotechx/eeg-notebooks)*
-
-Alternatively, you can record data directly without using LSL through the following command:
-
-    $ muselsl record_direct --duration 60
-
-_Note: direct recording does not allow 'Markers' data to be recorded_
-
-## Running Experiments
-
-Muse LSL was designed so that the Muse could be used to run a number of classic EEG experiments, including the [P300 event-related potential](http://alexandre.barachant.org/blog/2017/02/05/P300-with-muse.html) and the SSVEP and SSAEP evoked potentials.
-
-The code to perform these experiments is still available, but is now maintained in the [EEG Notebooks](https://github.com/neurotechx/eeg-notebooks) repository by the [NeuroTechX](https://neurotechx.com) community.
-
-## Usage as a Library
-
-If you want to integrate Muse LSL into your own Python project, you can import and use its functions as you would any Python library. Examples are available in the `examples` folder:
-
-```Python
-from muselsl import stream, list_muses
-
-muses = list_muses()
-stream(muses[0]['address'])
-
-# Note: Streaming is synchronous, so code here will not execute until after the stream has been closed
-print('Stream has ended')
-```
-
-## Alternate Data Types
-
-In addition to EEG, the Muse also provides data from an accelerometer, gyroscope, and, in the case of the Muse 2, a photoplethysmography (PPG) sensor. These data types can be enabled via command line arguments or by passing the correct parameters to the `stream` function. Once enabled, PPG, accelerometer, and gyroscope data will streamed in their own separate LSL streams named "PPG", "ACC", and "GYRO", respectively.
-
-To stream data from all sensors in a Muse 2 from the command line:
-
-    muselsl stream --ppg --acc --gyro
-
-As a library function:
-
-```Python
-from muselsl import stream, list_muses
-
-muses = list_muses()
-stream(muses[0]['address'], ppg_enabled=True, acc_enabled=True, gyro_enabled=True)
-```
-
-To record data from an alternate data source:
-
-    muselsl record --type ACC
-
-*Note: The record process will only record from one data type at a time. However, multiple terminals or processes can be used to record from multiple data types simultaneously*
-
-## What is LSL?
-
-Lab Streaming Layer or LSL is a system designed to unify the collection of time series data for research experiments. It has become standard in the field of EEG-based brain-computer interfaces for its ability to make seperate streams of data available on a network with time synchronization and near real-time access. For more information, check out this [lecture from Modern Brain-Computer Interface Design](https://www.youtube.com/watch?v=Y1at7yrcFW0) or the [LSL repository](https://github.com/sccn/labstreaminglayer)
-
-## Common Issues
-
-### Mac and Windows
-
-1.  Connection issues with BLED112 dongle:
-
-- You may need to use the `--interface` argument to provide the appropriate COM port value for the BLED112 device. The default value is COM9. To setup or view the device's COM port go to your OS's system settings
-
-### Linux
-
-1.  `pygatt.exceptions.BLEError: Unexpected error when scanning: Set scan parameters failed: Operation not permitted` (Linux)
-
-- This is an issue with pygatt requiring root privileges to run a scan. Make sure you [have `libcap` installed](https://askubuntu.com/questions/347788/how-can-i-install-libpcap-header-files-on-ubuntu-12-04) and run `` sudo setcap 'cap_net_raw,cap_net_admin+eip' `which hcitool` ``
-
-2.  `pygatt.exceptions.BLEError: No characteristic found matching 273e0003-4c4d-454d-96be-f03bac821358` (Linux)
-
-- There is a problem with the most recent version of pygatt. Work around this by downgrading to 3.1.1: `pip install pygatt==3.1.1`
-
-3.  `pygatt.exceptions.BLEError: No BLE adapter found` (Linux)
-
-- Make sure your computer's Bluetooth is turned on.
-
-4.  `pygatt.exceptions.BLEError: Unexpected error when scanning: Set scan parameters failed: Connection timed out` (Linux)
-
-- This seems to be due to a OS-level Bluetooth crash. Try turning your computer's bluetooth off and on again
-
-5.  `'RuntimeError: could not create stream outlet'` (Linux)
-
-- This appears to be due to Linux-specific issues with the newest version of pylsl. Ensure that you have pylsl 1.10.5 installed in the environment in which you are trying to run Muse LSL
-- If this is preceded by `Could not instantiate IPv4 stack: getrandom`, it could be [this issue](https://github.com/boostorg/uuid/issues/91) which can be resolved by building `liblsl` with `-DBOOST_UUID_RANDOM_PROVIDER_FORCE_POSIX` (e.g. by editing `standalone_compilation_linux.sh`)
-
-## Citing muse-lsl
-
-```
-@misc{muse-lsl,
-  author       = {Alexandre Barachant and
-                  Dano Morrison and
-                  Hubert Banville and
-                  Jason Kowaleski and
-                  Uri Shaked and
-                  Sylvain Chevallier and
-                  Juan Jesús Torre Tresols},
-  title        = {muse-lsl},
-  month        = may,
-  year         = 2019,
-  doi          = {10.5281/zenodo.3228861},
-  url          = {https://doi.org/10.5281/zenodo.3228861}
-}
-```
-
-> Alexandre Barachant, Dano Morrison, Hubert Banville, Jason Kowaleski, Uri Shaked, Sylvain Chevallier, & Juan Jesús Torre Tresols. (2019, May 25). muse-lsl (Version v2.0.2). Zenodo. http://doi.org/10.5281/zenodo.3228861
+
+[![DOI](https://zenodo.org/badge/80209610.svg)](https://zenodo.org/badge/latestdoi/80209610)
+
+# Muse LSL
+
+A Python package for streaming, visualizing, and recording EEG data from the Muse devices developed by InteraXon.
+
+![Blinks](blinks.png)
+
+## Requirements
+
+The code relies on a number of different bluetooth backends for connecting to the muse. We recommend using the `bleak` backend (enabled by default), but you may be interested in [BlueMuse](https://github.com/kowalej/BlueMuse/tree/master/Dist) for a GUI to discover and connect to Muse devices on Windows or [bgapi] if you are on a Mac with a BLED112 dongle. 
+
+**Compatible with Python 2.7 and Python 3.x**
+
+**Compatible with Muse 2, Muse S, and the classic Muse (2016)**
+
+_Note: if you run into any issues, first check out out [Common Issues](#common-issues) and then the [Issues](https://github.com/alexandrebarachant/muse-lsl/issues) section of this repository_
+
+## Getting Started
+
+### Installation
+
+Install Muse LSL with pip
+
+    pip install muselsl
+
+### Setting Up a Stream
+
+On Windows 10, we recommend using the [BlueMuse](https://github.com/kowalej/BlueMuse/tree/master/Dist) GUI to set up an LSL stream. On Mac and Linux, the easiest way to get Muse data is to use Muse LSL directly from the command line. Use the `-h` flag to get a comprehensive list of all commands and options.
+
+To print a list of available muses:
+
+    $ muselsl list
+
+To begin an LSL stream from the first available Muse:
+
+    $ muselsl stream  
+
+To connect to a specific Muse you can pass the name of the device as an argument. Device names can be found on the inside of the left earpiece (e.g. Muse-41D2):
+
+    $ muselsl stream --name YOUR_DEVICE_NAME
+
+You can also directly pass the MAC address of your Muse. This provides the benefit of bypassing the device discovery step and can make connecting to devices quicker and more reliable:
+
+    $ muselsl stream --address YOUR_DEVICE_ADDRESS
+
+### Working with Streaming Data
+
+Once an LSL stream is created, you have access to the following commands.
+
+*Note: the process running the `stream` command must be kept alive in order to maintain the LSL stream. These following commands should be run in another terminal or second process*
+
+To view data:
+
+    $ muselsl view
+
+If the visualization freezes or is laggy, you can also try the alternate version 2 of the viewer. *Note: this will require the additional [vispy](https://github.com/vispy/vispy) and [mne](https://github.com/mne-tools/mne-python) dependencies*
+
+    $ muselsl view --version 2
+
+To record EEG data into a CSV:
+
+    $ muselsl record --duration 60  
+
+*Note: this command will also save data from any LSL stream containing 'Markers' data, such as from the stimulus presentation scripts in [EEG Notebooks](https://github.com/neurotechx/eeg-notebooks)*
+
+Alternatively, you can record data directly without using LSL through the following command:
+
+    $ muselsl record_direct --duration 60
+
+_Note: direct recording does not allow 'Markers' data to be recorded_
+
+## Running Experiments
+
+Muse LSL was designed so that the Muse could be used to run a number of classic EEG experiments, including the [P300 event-related potential](http://alexandre.barachant.org/blog/2017/02/05/P300-with-muse.html) and the SSVEP and SSAEP evoked potentials.
+
+The code to perform these experiments is still available, but is now maintained in the [EEG Notebooks](https://github.com/neurotechx/eeg-notebooks) repository by the [NeuroTechX](https://neurotechx.com) community.
+
+## Usage as a Library
+
+If you want to integrate Muse LSL into your own Python project, you can import and use its functions as you would any Python library. Examples are available in the `examples` folder:
+
+```Python
+from muselsl import stream, list_muses
+
+muses = list_muses()
+stream(muses[0]['address'])
+
+# Note: Streaming is synchronous, so code here will not execute until after the stream has been closed
+print('Stream has ended')
+```
+
+## Alternate Data Types
+
+In addition to EEG, the Muse also provides data from an accelerometer, gyroscope, and, in the case of the Muse 2, a photoplethysmography (PPG) sensor. These data types can be enabled via command line arguments or by passing the correct parameters to the `stream` function. Once enabled, PPG, accelerometer, and gyroscope data will streamed in their own separate LSL streams named "PPG", "ACC", and "GYRO", respectively.
+
+To stream data from all sensors in a Muse 2 from the command line:
+
+    muselsl stream --ppg --acc --gyro
+
+As a library function:
+
+```Python
+from muselsl import stream, list_muses
+
+muses = list_muses()
+stream(muses[0]['address'], ppg_enabled=True, acc_enabled=True, gyro_enabled=True)
+```
+
+To record data from an alternate data source:
+
+    muselsl record --type ACC
+
+*Note: The record process will only record from one data type at a time. However, multiple terminals or processes can be used to record from multiple data types simultaneously*
+
+## What is LSL?
+
+Lab Streaming Layer or LSL is a system designed to unify the collection of time series data for research experiments. It has become standard in the field of EEG-based brain-computer interfaces for its ability to make seperate streams of data available on a network with time synchronization and near real-time access. For more information, check out this [lecture from Modern Brain-Computer Interface Design](https://www.youtube.com/watch?v=Y1at7yrcFW0) or the [LSL repository](https://github.com/sccn/labstreaminglayer)
+
+## Common Issues
+
+### Mac and Windows
+
+1.  Connection issues with BLED112 dongle:
+
+- You may need to use the `--interface` argument to provide the appropriate COM port value for the BLED112 device. The default value is COM9. To setup or view the device's COM port go to your OS's system settings
+
+### Linux
+
+1.  `pygatt.exceptions.BLEError: Unexpected error when scanning: Set scan parameters failed: Operation not permitted` (Linux)
+
+- This is an issue with pygatt requiring root privileges to run a scan. Make sure you [have `libcap` installed](https://askubuntu.com/questions/347788/how-can-i-install-libpcap-header-files-on-ubuntu-12-04) and run `` sudo setcap 'cap_net_raw,cap_net_admin+eip' `which hcitool` ``
+
+2.  `pygatt.exceptions.BLEError: No characteristic found matching 273e0003-4c4d-454d-96be-f03bac821358` (Linux)
+
+- There is a problem with the most recent version of pygatt. Work around this by downgrading to 3.1.1: `pip install pygatt==3.1.1`
+
+3.  `pygatt.exceptions.BLEError: No BLE adapter found` (Linux)
+
+- Make sure your computer's Bluetooth is turned on.
+
+4.  `pygatt.exceptions.BLEError: Unexpected error when scanning: Set scan parameters failed: Connection timed out` (Linux)
+
+- This seems to be due to a OS-level Bluetooth crash. Try turning your computer's bluetooth off and on again
+
+5.  `'RuntimeError: could not create stream outlet'` (Linux)
+
+- This appears to be due to Linux-specific issues with the newest version of pylsl. Ensure that you have pylsl 1.10.5 installed in the environment in which you are trying to run Muse LSL
+- If this is preceded by `Could not instantiate IPv4 stack: getrandom`, it could be [this issue](https://github.com/boostorg/uuid/issues/91) which can be resolved by building `liblsl` with `-DBOOST_UUID_RANDOM_PROVIDER_FORCE_POSIX` (e.g. by editing `standalone_compilation_linux.sh`)
+
+## Citing muse-lsl
+
+```
+@misc{muse-lsl,
+  author       = {Alexandre Barachant and
+                  Dano Morrison and
+                  Hubert Banville and
+                  Jason Kowaleski and
+                  Uri Shaked and
+                  Sylvain Chevallier and
+                  Juan Jesús Torre Tresols},
+  title        = {muse-lsl},
+  month        = may,
+  year         = 2019,
+  doi          = {10.5281/zenodo.3228861},
+  url          = {https://doi.org/10.5281/zenodo.3228861}
+}
+```
+
+> Alexandre Barachant, Dano Morrison, Hubert Banville, Jason Kowaleski, Uri Shaked, Sylvain Chevallier, & Juan Jesús Torre Tresols. (2019, May 25). muse-lsl (Version v2.0.2). Zenodo. http://doi.org/10.5281/zenodo.3228861
```

### Comparing `muselsl-2.2.2/blinks.png` & `muselsl-2.3.0/blinks.png`

 * *Files identical despite different names*

### Comparing `muselsl-2.2.2/muselsl/__main__.py` & `muselsl-2.3.0/muselsl/__main__.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-import argparse
-import sys
-from .cli import CLI
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        description='Python package for streaming, recording, and visualizing EEG data from the Muse 2016 headset.',
-        usage='''muselsl <command> [<args>]
-    Available commands:
-    list        List available Muse devices.
-                -b --backend    BLE backend to use. can be auto, bluemuse, gatt or bgapi.
-                -i --interface  The interface to use, 'hci0' for gatt or a com port for bgapi.
-
-    stream      Start an LSL stream from Muse headset.
-                -a --address    Device MAC address.
-                -n --name       Device name (e.g. Muse-41D2).
-                -b --backend    BLE backend to use. can be auto, bluemuse, gatt or bgapi.
-                -i --interface  The interface to use, 'hci0' for gatt or a com port for bgapi.
-                -p --ppg        Include PPG data
-                -c --acc        Include accelerometer data
-                -g --gyro       Include gyroscope data
-                --disable-eeg   Disable EEG data
-
-    view     Visualize EEG data from an LSL stream.
-                -w --window     Window length to display in seconds.
-                -s --scale      Scale in uV.
-                -r --refresh    Refresh rate in seconds.
-                -f --figure     Window size.
-                -v --version    Viewer version (1 or 2) - 1 is the default stable version, 2 is in development (and takes no arguments).
-                -b --backend    Matplotlib backend to use. Default: TkAgg
-
-    record   Record EEG data from an LSL stream.
-                -d --duration   Duration of the recording in seconds.
-                -f --filename   Name of the recording file.
-                -dj --dejitter  Whether to apply dejitter correction to timestamps.
-                -t --type       Data type to record from. Either EEG, PPG, ACC, or GYRO 
-
-    record_direct      Record data directly from Muse headset (no LSL).
-                -a --address    Device MAC address.
-                -n --name       Device name (e.g. Muse-41D2).
-                -b --backend    BLE backend to use. can be auto, bluemuse, gatt or bgapi.
-                -i --interface  The interface to use, 'hci0' for gatt or a com port for bgapi.
-        ''')
-
-    parser.add_argument('command', help='Command to run.')
-
-    # parse_args defaults to [1:] for args, but you need to
-    # exclude the rest of the args too, or validation will fail
-    args = parser.parse_args(sys.argv[1:2])
-
-    if not hasattr(CLI, args.command):
-        print('Incorrect usage. See help below.')
-        parser.print_help()
-        exit(1)
-
-    cli = CLI(args.command)
-
-
-if __name__ == '__main__':
-    main()
+import argparse
+import sys
+from .cli import CLI
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        description='Python package for streaming, recording, and visualizing EEG data from the Muse 2016 headset.',
+        usage='''muselsl <command> [<args>]
+    Available commands:
+    list        List available Muse devices.
+                -b --backend    BLE backend to use. can be auto, bluemuse, gatt or bgapi.
+                -i --interface  The interface to use, 'hci0' for gatt or a com port for bgapi.
+
+    stream      Start an LSL stream from Muse headset.
+                -a --address    Device MAC address.
+                -n --name       Device name (e.g. Muse-41D2).
+                -b --backend    BLE backend to use. can be auto, bluemuse, gatt or bgapi.
+                -i --interface  The interface to use, 'hci0' for gatt or a com port for bgapi.
+                -p --ppg        Include PPG data
+                -c --acc        Include accelerometer data
+                -g --gyro       Include gyroscope data
+                --disable-eeg   Disable EEG data
+
+    view     Visualize EEG data from an LSL stream.
+                -w --window     Window length to display in seconds.
+                -s --scale      Scale in uV.
+                -r --refresh    Refresh rate in seconds.
+                -f --figure     Window size.
+                -v --version    Viewer version (1 or 2) - 1 is the default stable version, 2 is in development (and takes no arguments).
+                -b --backend    Matplotlib backend to use. Default: TkAgg
+
+    record   Record EEG data from an LSL stream.
+                -d --duration   Duration of the recording in seconds.
+                -f --filename   Name of the recording file.
+                -dj --dejitter  Whether to apply dejitter correction to timestamps.
+                -t --type       Data type to record from. Either EEG, PPG, ACC, or GYRO 
+
+    record_direct      Record data directly from Muse headset (no LSL).
+                -a --address    Device MAC address.
+                -n --name       Device name (e.g. Muse-41D2).
+                -b --backend    BLE backend to use. can be auto, bluemuse, gatt or bgapi.
+                -i --interface  The interface to use, 'hci0' for gatt or a com port for bgapi.
+        ''')
+
+    parser.add_argument('command', help='Command to run.')
+
+    # parse_args defaults to [1:] for args, but you need to
+    # exclude the rest of the args too, or validation will fail
+    args = parser.parse_args(sys.argv[1:2])
+
+    if not hasattr(CLI, args.command):
+        print('Incorrect usage. See help below.')
+        parser.print_help()
+        exit(1)
+
+    cli = CLI(args.command)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `muselsl-2.2.2/muselsl/backends.py` & `muselsl-2.3.0/muselsl/backends.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,87 @@
-import asyncio
-import atexit
-import time
-try:
-    import bleak
-except ModuleNotFoundError as error:
-    bleak = error
-
-def _wait(coroutine):
-    loop = asyncio.get_event_loop()
-    return loop.run_until_complete(coroutine)
-
-def sleep(seconds):
-    time.sleep(seconds)
-
-class BleakBackend:
-    def __init__(self):
-        self.connected = set()
-        atexit.register(self.stop)
-        # run the event loop when sleeping
-        global sleep
-        sleep = self.pump
-    def start(self):
-        pass
-    def pump(self, seconds=1):
-        _wait(asyncio.sleep(seconds))
-    def stop(self):
-        for device in [*self.connected]:
-            device.disconnect()
-    def scan(self, timeout=10):
-        if isinstance(bleak, ModuleNotFoundError):
-            raise bleak
-        devices = _wait(bleak.BleakScanner.discover(timeout))
-        return [{'name':device.name, 'address':device.address} for device in devices]
-    def connect(self, address):
-        result = BleakDevice(self, address)
-        result.connect()
-        return result
-
-class BleakDevice:
-    def __init__(self, adapter, address):
-        self._adapter = adapter
-        self._client = bleak.BleakClient(address)
-    def connect(self):
-        _wait(self._client.connect())
-        self._adapter.connected.add(self)
-    def disconnect(self):
-        _wait(self._client.disconnect())
-        self._adapter.connected.remove(self)
-    # Characteristics have two handles: the declaration handle and the value handle.
-    # Pygatt seems to use the value handle, which appears less common.  Bleak uses the
-    # declaration handle used by d-bus.
-    # With the muse, the declaration and value handles happen to be sequential.
-    # So, we subtract 1 to get the declaration handle, and add 1 to get the value handle.
-    def char_write_handle(self, value_handle, value, wait_for_response=True, timeout=30):
-        declaration_handle = value_handle - 1
-        _wait(self._client.write_gatt_char(
-            declaration_handle,
-            bytearray(value),
-            wait_for_response))
-    def subscribe(self, uuid, callback=None, indication=False, wait_for_response=True):
-        def wrap(gatt_characteristic, data):
-            value_handle = gatt_characteristic.handle + 1
-            callback(value_handle, data)
-        _wait(self._client.start_notify(uuid, wrap))
+import asyncio
+import atexit
+import sys
+import time
+try:
+    import bleak
+except ModuleNotFoundError as error:
+    bleak = error
+from .constants import RETRY_SLEEP_TIMEOUT
+
+def _wait(coroutine):
+    loop = asyncio.get_event_loop()
+    return loop.run_until_complete(coroutine)
+
+def sleep(seconds):
+    time.sleep(seconds)
+
+class BleakBackend:
+    def __init__(self):
+        self.connected = set()
+        atexit.register(self.stop)
+        # run the event loop when sleeping
+        global sleep
+        sleep = self.pump
+    def start(self):
+        pass
+    def pump(self, seconds=1):
+        _wait(asyncio.sleep(seconds))
+    def stop(self):
+        for device in [*self.connected]:
+            device.disconnect()
+    def scan(self, timeout=10):
+        if isinstance(bleak, ModuleNotFoundError):
+            raise bleak
+        devices = _wait(bleak.BleakScanner.discover(timeout))
+        return [{'name':device.name, 'address':device.address} for device in devices]
+    def connect(self, address, retries):
+        result = BleakDevice(self, address)
+        if not result.connect(retries):
+            return None
+        return result
+
+class BleakDevice:
+    def __init__(self, adapter, address):
+        self._adapter = adapter
+        self._address = address
+        self._client = None
+    # Use retries=-1 to continue attempting to reconnect forever
+    def connect(self, retries):
+        attempts = 1
+        while True:
+            self._client = bleak.BleakClient(self._address)
+            if attempts > 1:
+                print(f'Connection attempt {attempts}')
+            try:
+                _wait(self._client.connect())
+            except (
+                bleak.exc.BleakDeviceNotFoundError, bleak.exc.BleakError
+            ) as err:
+                print(f'Failed to connect: {err}', file=sys.stderr)
+                if attempts == 1 + retries:
+                    return False
+                sleep(RETRY_SLEEP_TIMEOUT)
+                attempts += 1
+            else:
+                break
+        self._adapter.connected.add(self)
+        return True
+    def disconnect(self):
+        _wait(self._client.disconnect())
+        self._adapter.connected.remove(self)
+    # Characteristics have two handles: the declaration handle and the value handle.
+    # Pygatt seems to use the value handle, which appears less common.  Bleak uses the
+    # declaration handle used by d-bus.
+    # With the muse, the declaration and value handles happen to be sequential.
+    # So, we subtract 1 to get the declaration handle, and add 1 to get the value handle.
+    def char_write_handle(self, value_handle, value, wait_for_response=True, timeout=30):
+        declaration_handle = value_handle - 1
+        _wait(self._client.write_gatt_char(
+            declaration_handle,
+            bytearray(value),
+            wait_for_response))
+    def subscribe(self, uuid, callback=None, indication=False, wait_for_response=True):
+        def wrap(gatt_characteristic, data):
+            value_handle = gatt_characteristic.handle + 1
+            callback(value_handle, data)
+        _wait(self._client.start_notify(uuid, wrap))
```

### Comparing `muselsl-2.2.2/muselsl/cli.py` & `muselsl-2.3.0/muselsl/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,245 +1,275 @@
-#!/usr/bin/python
-import sys
-import argparse
-
-
-class CLI:
-    def __init__(self, command):
-        # use dispatch pattern to invoke method with same name
-        getattr(self, command)()
-
-    def list(self):
-        parser = argparse.ArgumentParser(
-            description='List available Muse devices.')
-        parser.add_argument(
-            "-b",
-            "--backend",
-            dest="backend",
-            type=str,
-            default="auto",
-            help="BLE backend to use. Can be auto, bluemuse, gatt or bgapi.")
-        parser.add_argument(
-            "-i",
-            "--interface",
-            dest="interface",
-            type=str,
-            default=None,
-            help=
-            "The interface to use, 'hci0' for gatt or a com port for bgapi. WIll auto-detect if not specified"
-        )
-        args = parser.parse_args(sys.argv[2:])
-        from . import list_muses
-        list_muses(args.backend, args.interface)
-
-    def stream(self):
-        parser = argparse.ArgumentParser(
-            description='Start an LSL stream from Muse headset.')
-        parser.add_argument(
-            "-a",
-            "--address",
-            dest="address",
-            type=str,
-            default=None,
-            help="Device MAC address.")
-        parser.add_argument(
-            "-n",
-            "--name",
-            dest="name",
-            type=str,
-            default=None,
-            help="Name of the device.")
-        parser.add_argument(
-            "-b",
-            "--backend",
-            dest="backend",
-            type=str,
-            default="auto",
-            help="BLE backend to use. Can be auto, bluemuse, gatt or bgapi.")
-        parser.add_argument(
-            "-i",
-            "--interface",
-            dest="interface",
-            type=str,
-            default=None,
-            help=
-            "The interface to use, 'hci0' for gatt or a com port for bgapi.")
-        parser.add_argument("-P",
-            "--preset",
-            type=int,
-            default=None,
-            help="Select preset which dictates data channels to be streamed")
-        parser.add_argument(
-            "-p",
-            "--ppg",
-            default=False,
-            action="store_true",
-            help="Include PPG data")
-        parser.add_argument(
-            "-c",
-            "--acc",
-            default=False,
-            action="store_true",
-            help="Include accelerometer data")
-        parser.add_argument(
-            "-g",
-            "--gyro",
-            default=False,
-            action="store_true",
-            help="Include gyroscope data")
-        parser.add_argument(
-            '-d',
-            '--disable-eeg',
-            dest='disable_eeg',
-            action='store_true',
-            help="Disable EEG data")
-        parser.add_argument(
-            '-dl',
-            '--disable-light',
-            dest='disable_light',
-            action='store_true',
-            help='Turn off light on the Muse S headband')
-
-
-        args = parser.parse_args(sys.argv[2:])
-        from . import stream
-
-        stream(args.address, args.backend, args.interface, args.name, args.ppg,
-               args.acc, args.gyro, args.disable_eeg, args.preset, args.disable_light)
-
-    def record(self):
-        parser = argparse.ArgumentParser(
-            description='Record data from an LSL stream.')
-        parser.add_argument(
-            "-d",
-            "--duration",
-            dest="duration",
-            type=int,
-            default=60,
-            help="Duration of the recording in seconds.")
-        parser.add_argument(
-            "-f",
-            "--filename",
-            dest="filename",
-            type=str,
-            default=None,
-            help="Name of the recording file.")
-        parser.add_argument(
-            "-dj",
-            "--dejitter",
-            dest="dejitter",
-            type=bool,
-            default=False,
-            help="Whether to apply dejitter correction to timestamps.")
-        parser.add_argument(
-            "-t",
-            "--type",
-            type=str,
-            default="EEG",
-            help="Data type to record from. Either EEG, PPG, ACC, or GYRO.")
-
-        args = parser.parse_args(sys.argv[2:])
-        from . import record
-        record(args.duration, args.filename, args.dejitter, args.type)
-
-    def record_direct(self):
-        parser = argparse.ArgumentParser(
-            description='Record directly from Muse without LSL.')
-        parser.add_argument(
-            "-a",
-            "--address",
-            dest="address",
-            type=str,
-            default=None,
-            help="Device MAC address.")
-        parser.add_argument(
-            "-n",
-            "--name",
-            dest="name",
-            type=str,
-            default=None,
-            help="Name of the device.")
-        parser.add_argument(
-            "-b",
-            "--backend",
-            dest="backend",
-            type=str,
-            default="auto",
-            help="BLE backend to use. Can be auto, bluemuse, gatt or bgapi.")
-        parser.add_argument(
-            "-i",
-            "--interface",
-            dest="interface",
-            type=str,
-            default=None,
-            help=
-            "The interface to use, 'hci0' for gatt or a com port for bgapi.")
-        parser.add_argument(
-            "-d",
-            "--duration",
-            dest="duration",
-            type=int,
-            default=60,
-            help="Duration of the recording in seconds.")
-        parser.add_argument(
-            "-f",
-            "--filename",
-            dest="filename",
-            type=str,
-            default=None,
-            help="Name of the recording file.")
-        args = parser.parse_args(sys.argv[2:])
-        from . import record_direct
-        record_direct(args.duration, args.address, args.filename, args.backend,
-                      args.interface, args.name)
-
-    def view(self):
-        parser = argparse.ArgumentParser(
-            description='View EEG data from an LSL stream.')
-        parser.add_argument(
-            "-w",
-            "--window",
-            dest="window",
-            type=float,
-            default=5.,
-            help="Window length to display in seconds.")
-        parser.add_argument(
-            "-s",
-            "--scale",
-            dest="scale",
-            type=float,
-            default=100,
-            help="Scale in uV.")
-        parser.add_argument(
-            "-r",
-            "--refresh",
-            dest="refresh",
-            type=float,
-            default=0.2,
-            help="Refresh rate in seconds.")
-        parser.add_argument(
-            "-f",
-            "--figure",
-            dest="figure",
-            type=str,
-            default="15x6",
-            help="Window size.")
-        parser.add_argument(
-            "-v",
-            "--version",
-            dest="version",
-            type=int,
-            default=1,
-            help=
-            "Viewer version (1 or 2) - 1 is the default stable version, 2 is in development (and takes no arguments)."
-        )
-        parser.add_argument(
-            "-b",
-            "--backend",
-            dest="backend",
-            type=str,
-            default='TkAgg',
-            help="Matplotlib backend to use. Default: %(default)s")
-        args = parser.parse_args(sys.argv[2:])
-        from . import view
-        view(args.window, args.scale, args.refresh, args.figure, args.version,
-             args.backend)
+#!/usr/bin/python
+import sys
+import argparse
+from .constants import LOG_LEVELS
+
+class CLI:
+    def __init__(self, command):
+        # use dispatch pattern to invoke method with same name
+        getattr(self, command)()
+
+    def list(self):
+        parser = argparse.ArgumentParser(
+            description='List available Muse devices.')
+        parser.add_argument(
+            "-b",
+            "--backend",
+            dest="backend",
+            type=str,
+            default="auto",
+            help="BLE backend to use. Can be auto, bluemuse, gatt or bgapi.")
+        parser.add_argument(
+            "-i",
+            "--interface",
+            dest="interface",
+            type=str,
+            default=None,
+            help=
+            "The interface to use, 'hci0' for gatt or a com port for bgapi. WIll auto-detect if not specified"
+        )
+        parser.add_argument(
+            '-l',
+            "--log", 
+            choices=LOG_LEVELS.keys(),
+            dest="log_level",
+            default='info',
+            help='Set the logging level'
+        )
+        args = parser.parse_args(sys.argv[2:])
+        from . import list_muses
+        list_muses(args.backend, args.interface, LOG_LEVELS[args.log_level])
+
+    def stream(self):
+        parser = argparse.ArgumentParser(
+            description='Start an LSL stream from Muse headset.')
+        parser.add_argument(
+            "-a",
+            "--address",
+            dest="address",
+            type=str,
+            default=None,
+            help="Device MAC address.")
+        parser.add_argument(
+            "-n",
+            "--name",
+            dest="name",
+            type=str,
+            default=None,
+            help="Name of the device.")
+        parser.add_argument(
+            "-b",
+            "--backend",
+            dest="backend",
+            type=str,
+            default="auto",
+            help="BLE backend to use. Can be auto, bluemuse, gatt or bgapi.")
+        parser.add_argument(
+            "-i",
+            "--interface",
+            dest="interface",
+            type=str,
+            default=None,
+            help=
+            "The interface to use, 'hci0' for gatt or a com port for bgapi.")
+        parser.add_argument("-P",
+            "--preset",
+            type=int,
+            default=None,
+            help="Select preset which dictates data channels to be streamed")
+        parser.add_argument(
+            "-p",
+            "--ppg",
+            default=False,
+            action="store_true",
+            help="Include PPG data")
+        parser.add_argument(
+            "-c",
+            "--acc",
+            default=False,
+            action="store_true",
+            help="Include accelerometer data")
+        parser.add_argument(
+            "-g",
+            "--gyro",
+            default=False,
+            action="store_true",
+            help="Include gyroscope data")
+        parser.add_argument(
+            '-d',
+            '--disable-eeg',
+            dest='disable_eeg',
+            action='store_true',
+            help="Disable EEG data")
+        parser.add_argument(
+            '-dl',
+            '--disable-light',
+            dest='disable_light',
+            action='store_true',
+            help='Turn off light on the Muse S headband')
+        parser.add_argument(
+            "-lslt",
+            "--lsltime",
+            default=False,
+            dest='lsl_time',
+            action="store_true",
+            help="Use pylsl's local_clock() for timestamps instead of Python's time.time()")
+        parser.add_argument(
+            "-r",
+            "--retries",
+            default=1,
+            dest='retries',
+            action="store_true",
+            help="How many times to retry connecting to the device on a failed attempt")
+        parser.add_argument(
+            '-l',
+            "--log", 
+            choices=LOG_LEVELS.keys(),
+            dest="log_level",
+            default='info',
+            help='Set the logging level'
+        )
+
+        args = parser.parse_args(sys.argv[2:])
+        from . import stream
+
+        stream(args.address, args.backend, args.interface, args.name, args.ppg,
+               args.acc, args.gyro, args.disable_eeg, args.preset, args.disable_light,
+               args.lsl_time, args.retries, LOG_LEVELS[args.log_level])
+
+    def record(self):
+        parser = argparse.ArgumentParser(
+            description='Record data from an LSL stream.')
+        parser.add_argument(
+            "-d",
+            "--duration",
+            dest="duration",
+            type=int,
+            default=60,
+            help="Duration of the recording in seconds.")
+        parser.add_argument(
+            "-f",
+            "--filename",
+            dest="filename",
+            type=str,
+            default=None,
+            help="Name of the recording file.")
+        parser.add_argument(
+            "-dj",
+            "--dejitter",
+            dest="dejitter",
+            type=bool,
+            default=False,
+            help="Whether to apply dejitter correction to timestamps.")
+        parser.add_argument(
+            "-t",
+            "--type",
+            type=str,
+            default="EEG",
+            help="Data type to record from. Either EEG, PPG, ACC, or GYRO.")
+
+        args = parser.parse_args(sys.argv[2:])
+        from . import record
+        record(args.duration, args.filename, args.dejitter, args.type)
+
+    def record_direct(self):
+        parser = argparse.ArgumentParser(
+            description='Record directly from Muse without LSL.')
+        parser.add_argument(
+            "-a",
+            "--address",
+            dest="address",
+            type=str,
+            default=None,
+            help="Device MAC address.")
+        parser.add_argument(
+            "-n",
+            "--name",
+            dest="name",
+            type=str,
+            default=None,
+            help="Name of the device.")
+        parser.add_argument(
+            "-b",
+            "--backend",
+            dest="backend",
+            type=str,
+            default="auto",
+            help="BLE backend to use. Can be auto, bluemuse, gatt or bgapi.")
+        parser.add_argument(
+            "-i",
+            "--interface",
+            dest="interface",
+            type=str,
+            default=None,
+            help=
+            "The interface to use, 'hci0' for gatt or a com port for bgapi.")
+        parser.add_argument(
+            "-d",
+            "--duration",
+            dest="duration",
+            type=int,
+            default=60,
+            help="Duration of the recording in seconds.")
+        parser.add_argument(
+            "-f",
+            "--filename",
+            dest="filename",
+            type=str,
+            default=None,
+            help="Name of the recording file.")
+        args = parser.parse_args(sys.argv[2:])
+        from . import record_direct
+        record_direct(args.duration, args.address, args.filename, args.backend,
+                      args.interface, args.name)
+
+    def view(self):
+        parser = argparse.ArgumentParser(
+            description='View EEG data from an LSL stream.')
+        parser.add_argument(
+            "-w",
+            "--window",
+            dest="window",
+            type=float,
+            default=5.,
+            help="Window length to display in seconds.")
+        parser.add_argument(
+            "-s",
+            "--scale",
+            dest="scale",
+            type=float,
+            default=100,
+            help="Scale in uV.")
+        parser.add_argument(
+            "-r",
+            "--refresh",
+            dest="refresh",
+            type=float,
+            default=0.2,
+            help="Refresh rate in seconds.")
+        parser.add_argument(
+            "-f",
+            "--figure",
+            dest="figure",
+            type=str,
+            default="15x6",
+            help="Window size.")
+        parser.add_argument(
+            "-v",
+            "--version",
+            dest="version",
+            type=int,
+            default=1,
+            help=
+            "Viewer version (1 or 2) - 1 is the default stable version, 2 is in development (and takes no arguments)."
+        )
+        parser.add_argument(
+            "-b",
+            "--backend",
+            dest="backend",
+            type=str,
+            default='TkAgg',
+            help="Matplotlib backend to use. Default: %(default)s")
+        args = parser.parse_args(sys.argv[2:])
+        from . import view
+        view(args.window, args.scale, args.refresh, args.figure, args.version,
+             args.backend)
```

### Comparing `muselsl-2.2.2/muselsl/constants.py` & `muselsl-2.3.0/muselsl/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,67 @@
-MUSE_NB_EEG_CHANNELS = 5
-MUSE_SAMPLING_EEG_RATE = 256
-LSL_EEG_CHUNK = 12
-
-MUSE_NB_PPG_CHANNELS = 3
-MUSE_SAMPLING_PPG_RATE = 64
-LSL_PPG_CHUNK = 6
-
-MUSE_NB_ACC_CHANNELS = 3
-MUSE_SAMPLING_ACC_RATE = 52
-LSL_ACC_CHUNK = 1
-
-MUSE_NB_GYRO_CHANNELS = 3
-MUSE_SAMPLING_GYRO_RATE = 52
-LSL_GYRO_CHUNK = 1
-
-# 00001800-0000-1000-8000-00805f9b34fb Generic Access 0x05-0x0b
-# 00001801-0000-1000-8000-00805f9b34fb Generic Attribute 0x01-0x04
-MUSE_GATT_ATTR_SERVICECHANGED = '00002a05-0000-1000-8000-00805f9b34fb' # ble std 0x02-0x04
-# 0000fe8d-0000-1000-8000-00805f9b34fb Interaxon Inc. 0x0c-0x42
-MUSE_GATT_ATTR_STREAM_TOGGLE = '273e0001-4c4d-454d-96be-f03bac821358' # serial 0x0d-0x0f
-MUSE_GATT_ATTR_LEFTAUX = '273e0002-4c4d-454d-96be-f03bac821358' # not implemented yet 0x1c-0x1e
-MUSE_GATT_ATTR_TP9 = '273e0003-4c4d-454d-96be-f03bac821358' # 0x1f-0x21
-MUSE_GATT_ATTR_AF7 = '273e0004-4c4d-454d-96be-f03bac821358' # fp1 0x22-0x24
-MUSE_GATT_ATTR_AF8 = '273e0005-4c4d-454d-96be-f03bac821358' # fp2 0x25-0x27
-MUSE_GATT_ATTR_TP10 = '273e0006-4c4d-454d-96be-f03bac821358' # 0x28-0x2a
-MUSE_GATT_ATTR_RIGHTAUX = '273e0007-4c4d-454d-96be-f03bac821358' #0x2b-0x2d
-MUSE_GATT_ATTR_REFDRL = '273e0008-4c4d-454d-96be-f03bac821358' # not implemented yet 0x10-0x12
-MUSE_GATT_ATTR_GYRO = '273e0009-4c4d-454d-96be-f03bac821358' # 0x13-0x15
-MUSE_GATT_ATTR_ACCELEROMETER = '273e000a-4c4d-454d-96be-f03bac821358' # 0x16-0x18
-MUSE_GATT_ATTR_TELEMETRY = '273e000b-4c4d-454d-96be-f03bac821358' # 0x19-0x1b
-#MUSE_GATT_ATTR_MAGNETOMETER = '273e000c-4c4d-454d-96be-f03bac821358' # 0x2e-0x30
-#MUSE_GATT_ATTR_PRESSURE = '273e000d-4c4d-454d-96be-f03bac821358' # 0x31-0x33
-#MUSE_GATT_ATTR_ULTRAVIOLET = '273e000e-4c4d-454d-96be-f03bac821358' # 0x34-0x36
-MUSE_GATT_ATTR_PPG1 = "273e000f-4c4d-454d-96be-f03bac821358" # ambient 0x37-0x39
-MUSE_GATT_ATTR_PPG2 = "273e0010-4c4d-454d-96be-f03bac821358" # infrared 0x3a-0x3c
-MUSE_GATT_ATTR_PPG3 = "273e0011-4c4d-454d-96be-f03bac821358" # red 0x3d-0x3f
-MUSE_GATT_ATTR_THERMISTOR = "273e0012-4c4d-454d-96be-f03bac821358" # muse S only, not implemented yet 0x40-0x42
-
-MUSE_ACCELEROMETER_SCALE_FACTOR = 0.0000610352
-MUSE_GYRO_SCALE_FACTOR = 0.0074768
-
-MUSE_SCAN_TIMEOUT = 10.5
-AUTO_DISCONNECT_DELAY = 3
-
-LSL_SCAN_TIMEOUT = 5
-LSL_BUFFER = 360
-
-VIEW_SUBSAMPLE = 2
-VIEW_BUFFER = 12
+import logging
+
+MUSE_NB_EEG_CHANNELS = 5
+MUSE_SAMPLING_EEG_RATE = 256
+LSL_EEG_CHUNK = 12
+
+MUSE_NB_PPG_CHANNELS = 3
+MUSE_SAMPLING_PPG_RATE = 64
+LSL_PPG_CHUNK = 6
+
+MUSE_NB_ACC_CHANNELS = 3
+MUSE_SAMPLING_ACC_RATE = 52
+LSL_ACC_CHUNK = 1
+
+MUSE_NB_GYRO_CHANNELS = 3
+MUSE_SAMPLING_GYRO_RATE = 52
+LSL_GYRO_CHUNK = 1
+
+# 00001800-0000-1000-8000-00805f9b34fb Generic Access 0x05-0x0b
+# 00001801-0000-1000-8000-00805f9b34fb Generic Attribute 0x01-0x04
+MUSE_GATT_ATTR_SERVICECHANGED = '00002a05-0000-1000-8000-00805f9b34fb' # ble std 0x02-0x04
+# 0000fe8d-0000-1000-8000-00805f9b34fb Interaxon Inc. 0x0c-0x42
+MUSE_GATT_ATTR_STREAM_TOGGLE = '273e0001-4c4d-454d-96be-f03bac821358' # serial 0x0d-0x0f
+MUSE_GATT_ATTR_LEFTAUX = '273e0002-4c4d-454d-96be-f03bac821358' # not implemented yet 0x1c-0x1e
+MUSE_GATT_ATTR_TP9 = '273e0003-4c4d-454d-96be-f03bac821358' # 0x1f-0x21
+MUSE_GATT_ATTR_AF7 = '273e0004-4c4d-454d-96be-f03bac821358' # fp1 0x22-0x24
+MUSE_GATT_ATTR_AF8 = '273e0005-4c4d-454d-96be-f03bac821358' # fp2 0x25-0x27
+MUSE_GATT_ATTR_TP10 = '273e0006-4c4d-454d-96be-f03bac821358' # 0x28-0x2a
+MUSE_GATT_ATTR_RIGHTAUX = '273e0007-4c4d-454d-96be-f03bac821358' #0x2b-0x2d
+MUSE_GATT_ATTR_REFDRL = '273e0008-4c4d-454d-96be-f03bac821358' # not implemented yet 0x10-0x12
+MUSE_GATT_ATTR_GYRO = '273e0009-4c4d-454d-96be-f03bac821358' # 0x13-0x15
+MUSE_GATT_ATTR_ACCELEROMETER = '273e000a-4c4d-454d-96be-f03bac821358' # 0x16-0x18
+MUSE_GATT_ATTR_TELEMETRY = '273e000b-4c4d-454d-96be-f03bac821358' # 0x19-0x1b
+#MUSE_GATT_ATTR_MAGNETOMETER = '273e000c-4c4d-454d-96be-f03bac821358' # 0x2e-0x30
+#MUSE_GATT_ATTR_PRESSURE = '273e000d-4c4d-454d-96be-f03bac821358' # 0x31-0x33
+#MUSE_GATT_ATTR_ULTRAVIOLET = '273e000e-4c4d-454d-96be-f03bac821358' # 0x34-0x36
+MUSE_GATT_ATTR_PPG1 = "273e000f-4c4d-454d-96be-f03bac821358" # ambient 0x37-0x39
+MUSE_GATT_ATTR_PPG2 = "273e0010-4c4d-454d-96be-f03bac821358" # infrared 0x3a-0x3c
+MUSE_GATT_ATTR_PPG3 = "273e0011-4c4d-454d-96be-f03bac821358" # red 0x3d-0x3f
+MUSE_GATT_ATTR_THERMISTOR = "273e0012-4c4d-454d-96be-f03bac821358" # muse S only, not implemented yet 0x40-0x42
+
+MUSE_ACCELEROMETER_SCALE_FACTOR = 0.0000610352
+MUSE_GYRO_SCALE_FACTOR = 0.0074768
+
+# How long to wait while scanning for devices
+LIST_SCAN_TIMEOUT = 10.5
+# How long to wait after device stops sending data before ending the stream
+AUTO_DISCONNECT_DELAY = 3
+# How long to wait in between connection attempts
+RETRY_SLEEP_TIMEOUT = 1
+
+LSL_SCAN_TIMEOUT = 5
+LSL_BUFFER = 360
+
+VIEW_SUBSAMPLE = 2
+VIEW_BUFFER = 12
+
+LOG_LEVELS = {
+    'debug': logging.DEBUG,
+    'info': logging.INFO,
+    'warning': logging.WARNING,
+    'error': logging.ERROR,
+    'critical': logging.CRITICAL
+}
+
+
+
```

### Comparing `muselsl-2.2.2/muselsl/docs/README.md` & `muselsl-2.3.0/muselsl/docs/README.md`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-
-[![DOI](https://zenodo.org/badge/80209610.svg)](https://zenodo.org/badge/latestdoi/80209610)
-
-# Muse LSL
-
-A Python package for streaming, visualizing, and recording EEG data from the Muse devices developed by InteraXon.
-
-![Blinks](blinks.png)
-
-## Requirements
-
-The code relies on a number of different bluetooth backends for connecting to the muse. We recommend using the `bleak` backend (enabled by default), but you may be interested in [BlueMuse](https://github.com/kowalej/BlueMuse/tree/master/Dist) for a GUI to discover and connect to Muse devices on Windows or [bgapi] if you are on a Mac with a BLED112 dongle. 
-
-**Compatible with Python 2.7 and Python 3.x**
-
-**Compatible with Muse 2, Muse S, and the classic Muse (2016)**
-
-_Note: if you run into any issues, first check out out [Common Issues](#common-issues) and then the [Issues](https://github.com/alexandrebarachant/muse-lsl/issues) section of this repository_
-
-## Getting Started
-
-### Installation
-
-Install Muse LSL with pip
-
-    pip install muselsl
-
-### Setting Up a Stream
-
-On Windows 10, we recommend using the [BlueMuse](https://github.com/kowalej/BlueMuse/tree/master/Dist) GUI to set up an LSL stream. On Mac and Linux, the easiest way to get Muse data is to use Muse LSL directly from the command line. Use the `-h` flag to get a comprehensive list of all commands and options.
-
-To print a list of available muses:
-
-    $ muselsl list
-
-To begin an LSL stream from the first available Muse:
-
-    $ muselsl stream  
-
-To connect to a specific Muse you can pass the name of the device as an argument. Device names can be found on the inside of the left earpiece (e.g. Muse-41D2):
-
-    $ muselsl stream --name YOUR_DEVICE_NAME
-
-You can also directly pass the MAC address of your Muse. This provides the benefit of bypassing the device discovery step and can make connecting to devices quicker and more reliable:
-
-    $ muselsl stream --address YOUR_DEVICE_ADDRESS
-
-### Working with Streaming Data
-
-Once an LSL stream is created, you have access to the following commands.
-
-*Note: the process running the `stream` command must be kept alive in order to maintain the LSL stream. These following commands should be run in another terminal or second process*
-
-To view data:
-
-    $ muselsl view
-
-If the visualization freezes or is laggy, you can also try the alternate version 2 of the viewer. *Note: this will require the additional [vispy](https://github.com/vispy/vispy) and [mne](https://github.com/mne-tools/mne-python) dependencies*
-
-    $ muselsl view --version 2
-
-To record EEG data into a CSV:
-
-    $ muselsl record --duration 60  
-
-*Note: this command will also save data from any LSL stream containing 'Markers' data, such as from the stimulus presentation scripts in [EEG Notebooks](https://github.com/neurotechx/eeg-notebooks)*
-
-Alternatively, you can record data directly without using LSL through the following command:
-
-    $ muselsl record_direct --duration 60
-
-_Note: direct recording does not allow 'Markers' data to be recorded_
-
-## Running Experiments
-
-Muse LSL was designed so that the Muse could be used to run a number of classic EEG experiments, including the [P300 event-related potential](http://alexandre.barachant.org/blog/2017/02/05/P300-with-muse.html) and the SSVEP and SSAEP evoked potentials.
-
-The code to perform these experiments is still available, but is now maintained in the [EEG Notebooks](https://github.com/neurotechx/eeg-notebooks) repository by the [NeuroTechX](https://neurotechx.com) community.
-
-## Usage as a Library
-
-If you want to integrate Muse LSL into your own Python project, you can import and use its functions as you would any Python library. Examples are available in the `examples` folder:
-
-```Python
-from muselsl import stream, list_muses
-
-muses = list_muses()
-stream(muses[0]['address'])
-
-# Note: Streaming is synchronous, so code here will not execute until after the stream has been closed
-print('Stream has ended')
-```
-
-## Alternate Data Types
-
-In addition to EEG, the Muse also provides data from an accelerometer, gyroscope, and, in the case of the Muse 2, a photoplethysmography (PPG) sensor. These data types can be enabled via command line arguments or by passing the correct parameters to the `stream` function. Once enabled, PPG, accelerometer, and gyroscope data will streamed in their own separate LSL streams named "PPG", "ACC", and "GYRO", respectively.
-
-To stream data from all sensors in a Muse 2 from the command line:
-
-    muselsl stream --ppg --acc --gyro
-
-As a library function:
-
-```Python
-from muselsl import stream, list_muses
-
-muses = list_muses()
-stream(muses[0]['address'], ppg_enabled=True, acc_enabled=True, gyro_enabled=True)
-```
-
-To record data from an alternate data source:
-
-    muselsl record --type ACC
-
-*Note: The record process will only record from one data type at a time. However, multiple terminals or processes can be used to record from multiple data types simultaneously*
-
-## What is LSL?
-
-Lab Streaming Layer or LSL is a system designed to unify the collection of time series data for research experiments. It has become standard in the field of EEG-based brain-computer interfaces for its ability to make seperate streams of data available on a network with time synchronization and near real-time access. For more information, check out this [lecture from Modern Brain-Computer Interface Design](https://www.youtube.com/watch?v=Y1at7yrcFW0) or the [LSL repository](https://github.com/sccn/labstreaminglayer)
-
-## Common Issues
-
-### Mac and Windows
-
-1.  Connection issues with BLED112 dongle:
-
-- You may need to use the `--interface` argument to provide the appropriate COM port value for the BLED112 device. The default value is COM9. To setup or view the device's COM port go to your OS's system settings
-
-### Linux
-
-1.  `pygatt.exceptions.BLEError: Unexpected error when scanning: Set scan parameters failed: Operation not permitted` (Linux)
-
-- This is an issue with pygatt requiring root privileges to run a scan. Make sure you [have `libcap` installed](https://askubuntu.com/questions/347788/how-can-i-install-libpcap-header-files-on-ubuntu-12-04) and run `` sudo setcap 'cap_net_raw,cap_net_admin+eip' `which hcitool` ``
-
-2.  `pygatt.exceptions.BLEError: No characteristic found matching 273e0003-4c4d-454d-96be-f03bac821358` (Linux)
-
-- There is a problem with the most recent version of pygatt. Work around this by downgrading to 3.1.1: `pip install pygatt==3.1.1`
-
-3.  `pygatt.exceptions.BLEError: No BLE adapter found` (Linux)
-
-- Make sure your computer's Bluetooth is turned on.
-
-4.  `pygatt.exceptions.BLEError: Unexpected error when scanning: Set scan parameters failed: Connection timed out` (Linux)
-
-- This seems to be due to a OS-level Bluetooth crash. Try turning your computer's bluetooth off and on again
-
-5.  `'RuntimeError: could not create stream outlet'` (Linux)
-
-- This appears to be due to Linux-specific issues with the newest version of pylsl. Ensure that you have pylsl 1.10.5 installed in the environment in which you are trying to run Muse LSL
-- If this is preceded by `Could not instantiate IPv4 stack: getrandom`, it could be [this issue](https://github.com/boostorg/uuid/issues/91) which can be resolved by building `liblsl` with `-DBOOST_UUID_RANDOM_PROVIDER_FORCE_POSIX` (e.g. by editing `standalone_compilation_linux.sh`)
-
-## Citing muse-lsl
-
-```
-@misc{muse-lsl,
-  author       = {Alexandre Barachant and
-                  Dano Morrison and
-                  Hubert Banville and
-                  Jason Kowaleski and
-                  Uri Shaked and
-                  Sylvain Chevallier and
-                  Juan Jesús Torre Tresols},
-  title        = {muse-lsl},
-  month        = may,
-  year         = 2019,
-  doi          = {10.5281/zenodo.3228861},
-  url          = {https://doi.org/10.5281/zenodo.3228861}
-}
-```
-
-> Alexandre Barachant, Dano Morrison, Hubert Banville, Jason Kowaleski, Uri Shaked, Sylvain Chevallier, & Juan Jesús Torre Tresols. (2019, May 25). muse-lsl (Version v2.0.2). Zenodo. http://doi.org/10.5281/zenodo.3228861
+
+[![DOI](https://zenodo.org/badge/80209610.svg)](https://zenodo.org/badge/latestdoi/80209610)
+
+# Muse LSL
+
+A Python package for streaming, visualizing, and recording EEG data from the Muse devices developed by InteraXon.
+
+![Blinks](blinks.png)
+
+## Requirements
+
+The code relies on a number of different bluetooth backends for connecting to the muse. We recommend using the `bleak` backend (enabled by default), but you may be interested in [BlueMuse](https://github.com/kowalej/BlueMuse/tree/master/Dist) for a GUI to discover and connect to Muse devices on Windows or [bgapi] if you are on a Mac with a BLED112 dongle. 
+
+**Compatible with Python 2.7 and Python 3.x**
+
+**Compatible with Muse 2, Muse S, and the classic Muse (2016)**
+
+_Note: if you run into any issues, first check out out [Common Issues](#common-issues) and then the [Issues](https://github.com/alexandrebarachant/muse-lsl/issues) section of this repository_
+
+## Getting Started
+
+### Installation
+
+Install Muse LSL with pip
+
+    pip install muselsl
+
+### Setting Up a Stream
+
+On Windows 10, we recommend using the [BlueMuse](https://github.com/kowalej/BlueMuse/tree/master/Dist) GUI to set up an LSL stream. On Mac and Linux, the easiest way to get Muse data is to use Muse LSL directly from the command line. Use the `-h` flag to get a comprehensive list of all commands and options.
+
+To print a list of available muses:
+
+    $ muselsl list
+
+To begin an LSL stream from the first available Muse:
+
+    $ muselsl stream  
+
+To connect to a specific Muse you can pass the name of the device as an argument. Device names can be found on the inside of the left earpiece (e.g. Muse-41D2):
+
+    $ muselsl stream --name YOUR_DEVICE_NAME
+
+You can also directly pass the MAC address of your Muse. This provides the benefit of bypassing the device discovery step and can make connecting to devices quicker and more reliable:
+
+    $ muselsl stream --address YOUR_DEVICE_ADDRESS
+
+### Working with Streaming Data
+
+Once an LSL stream is created, you have access to the following commands.
+
+*Note: the process running the `stream` command must be kept alive in order to maintain the LSL stream. These following commands should be run in another terminal or second process*
+
+To view data:
+
+    $ muselsl view
+
+If the visualization freezes or is laggy, you can also try the alternate version 2 of the viewer. *Note: this will require the additional [vispy](https://github.com/vispy/vispy) and [mne](https://github.com/mne-tools/mne-python) dependencies*
+
+    $ muselsl view --version 2
+
+To record EEG data into a CSV:
+
+    $ muselsl record --duration 60  
+
+*Note: this command will also save data from any LSL stream containing 'Markers' data, such as from the stimulus presentation scripts in [EEG Notebooks](https://github.com/neurotechx/eeg-notebooks)*
+
+Alternatively, you can record data directly without using LSL through the following command:
+
+    $ muselsl record_direct --duration 60
+
+_Note: direct recording does not allow 'Markers' data to be recorded_
+
+## Running Experiments
+
+Muse LSL was designed so that the Muse could be used to run a number of classic EEG experiments, including the [P300 event-related potential](http://alexandre.barachant.org/blog/2017/02/05/P300-with-muse.html) and the SSVEP and SSAEP evoked potentials.
+
+The code to perform these experiments is still available, but is now maintained in the [EEG Notebooks](https://github.com/neurotechx/eeg-notebooks) repository by the [NeuroTechX](https://neurotechx.com) community.
+
+## Usage as a Library
+
+If you want to integrate Muse LSL into your own Python project, you can import and use its functions as you would any Python library. Examples are available in the `examples` folder:
+
+```Python
+from muselsl import stream, list_muses
+
+muses = list_muses()
+stream(muses[0]['address'])
+
+# Note: Streaming is synchronous, so code here will not execute until after the stream has been closed
+print('Stream has ended')
+```
+
+## Alternate Data Types
+
+In addition to EEG, the Muse also provides data from an accelerometer, gyroscope, and, in the case of the Muse 2, a photoplethysmography (PPG) sensor. These data types can be enabled via command line arguments or by passing the correct parameters to the `stream` function. Once enabled, PPG, accelerometer, and gyroscope data will streamed in their own separate LSL streams named "PPG", "ACC", and "GYRO", respectively.
+
+To stream data from all sensors in a Muse 2 from the command line:
+
+    muselsl stream --ppg --acc --gyro
+
+As a library function:
+
+```Python
+from muselsl import stream, list_muses
+
+muses = list_muses()
+stream(muses[0]['address'], ppg_enabled=True, acc_enabled=True, gyro_enabled=True)
+```
+
+To record data from an alternate data source:
+
+    muselsl record --type ACC
+
+*Note: The record process will only record from one data type at a time. However, multiple terminals or processes can be used to record from multiple data types simultaneously*
+
+## What is LSL?
+
+Lab Streaming Layer or LSL is a system designed to unify the collection of time series data for research experiments. It has become standard in the field of EEG-based brain-computer interfaces for its ability to make seperate streams of data available on a network with time synchronization and near real-time access. For more information, check out this [lecture from Modern Brain-Computer Interface Design](https://www.youtube.com/watch?v=Y1at7yrcFW0) or the [LSL repository](https://github.com/sccn/labstreaminglayer)
+
+## Common Issues
+
+### Mac and Windows
+
+1.  Connection issues with BLED112 dongle:
+
+- You may need to use the `--interface` argument to provide the appropriate COM port value for the BLED112 device. The default value is COM9. To setup or view the device's COM port go to your OS's system settings
+
+### Linux
+
+1.  `pygatt.exceptions.BLEError: Unexpected error when scanning: Set scan parameters failed: Operation not permitted` (Linux)
+
+- This is an issue with pygatt requiring root privileges to run a scan. Make sure you [have `libcap` installed](https://askubuntu.com/questions/347788/how-can-i-install-libpcap-header-files-on-ubuntu-12-04) and run `` sudo setcap 'cap_net_raw,cap_net_admin+eip' `which hcitool` ``
+
+2.  `pygatt.exceptions.BLEError: No characteristic found matching 273e0003-4c4d-454d-96be-f03bac821358` (Linux)
+
+- There is a problem with the most recent version of pygatt. Work around this by downgrading to 3.1.1: `pip install pygatt==3.1.1`
+
+3.  `pygatt.exceptions.BLEError: No BLE adapter found` (Linux)
+
+- Make sure your computer's Bluetooth is turned on.
+
+4.  `pygatt.exceptions.BLEError: Unexpected error when scanning: Set scan parameters failed: Connection timed out` (Linux)
+
+- This seems to be due to a OS-level Bluetooth crash. Try turning your computer's bluetooth off and on again
+
+5.  `'RuntimeError: could not create stream outlet'` (Linux)
+
+- This appears to be due to Linux-specific issues with the newest version of pylsl. Ensure that you have pylsl 1.10.5 installed in the environment in which you are trying to run Muse LSL
+- If this is preceded by `Could not instantiate IPv4 stack: getrandom`, it could be [this issue](https://github.com/boostorg/uuid/issues/91) which can be resolved by building `liblsl` with `-DBOOST_UUID_RANDOM_PROVIDER_FORCE_POSIX` (e.g. by editing `standalone_compilation_linux.sh`)
+
+## Citing muse-lsl
+
+```
+@misc{muse-lsl,
+  author       = {Alexandre Barachant and
+                  Dano Morrison and
+                  Hubert Banville and
+                  Jason Kowaleski and
+                  Uri Shaked and
+                  Sylvain Chevallier and
+                  Juan Jesús Torre Tresols},
+  title        = {muse-lsl},
+  month        = may,
+  year         = 2019,
+  doi          = {10.5281/zenodo.3228861},
+  url          = {https://doi.org/10.5281/zenodo.3228861}
+}
+```
+
+> Alexandre Barachant, Dano Morrison, Hubert Banville, Jason Kowaleski, Uri Shaked, Sylvain Chevallier, & Juan Jesús Torre Tresols. (2019, May 25). muse-lsl (Version v2.0.2). Zenodo. http://doi.org/10.5281/zenodo.3228861
```

### Comparing `muselsl-2.2.2/muselsl/helper.py` & `muselsl-2.3.0/muselsl/helper.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import platform
-import warnings
-
-
-def warn_bluemuse_not_supported(extra_text = ''):
-    warnings.warn('Operation not supported by bluemuse backend.' + extra_text,
-                  RuntimeWarning)
-
-
-def resolve_backend(backend):
-    if backend == 'auto':
-        ## if there are any issues with bleak,
-        ## below are the previous defaults
-        # platformName = platform.system().lower()
-        # if platformName == 'linux' or platformName == 'linux2':
-        #     backend = 'gatt'
-        # elif platformName == 'windows' and int(platform.version().replace('.', '')) >= 10015063:
-        #     backend = 'bluemuse'
-        # else:
-        #     backend = 'bgapi'
-        backend = 'bleak'
-    if backend in ['gatt', 'bgapi', 'bluemuse', 'bleak']:
-        return backend
-    else:
-        raise(ValueError('Backend must be one of: auto, gatt, bgapi, bluemuse, bleak.'))
+import platform
+import warnings
+
+
+def warn_bluemuse_not_supported(extra_text = ''):
+    warnings.warn('Operation not supported by bluemuse backend.' + extra_text,
+                  RuntimeWarning)
+
+
+def resolve_backend(backend):
+    if backend == 'auto':
+        ## if there are any issues with bleak,
+        ## below are the previous defaults
+        # platformName = platform.system().lower()
+        # if platformName == 'linux' or platformName == 'linux2':
+        #     backend = 'gatt'
+        # elif platformName == 'windows' and int(platform.version().replace('.', '')) >= 10015063:
+        #     backend = 'bluemuse'
+        # else:
+        #     backend = 'bgapi'
+        backend = 'bleak'
+    if backend in ['gatt', 'bgapi', 'bluemuse', 'bleak']:
+        return backend
+    else:
+        raise(ValueError('Backend must be one of: auto, gatt, bgapi, bluemuse, bleak.'))
```

### Comparing `muselsl-2.2.2/muselsl/muse.py` & `muselsl-2.3.0/muselsl/muse.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,603 +1,613 @@
-import bitstring
-import pygatt
-import numpy as np
-from time import time, sleep
-from sys import platform
-import subprocess
-from . import backends
-from . import helper
-from .constants import *
-
-
-class Muse():
-    """Muse 2016 headband"""
-
-    def __init__(self,
-                 address,
-                 callback_eeg=None,
-                 callback_control=None,
-                 callback_telemetry=None,
-                 callback_acc=None,
-                 callback_gyro=None,
-                 callback_ppg=None,
-                 backend='auto',
-                 interface=None,
-                 time_func=time,
-                 name=None,
-                 preset=None,
-                 disable_light=False):
-        """Initialize
-
-        callback_eeg -- callback for eeg data, function(data, timestamps)
-        callback_control -- function(message)
-        callback_telemetry -- function(timestamp, battery, fuel_gauge,
-                                       adc_volt, temperature)
-
-        callback_acc -- function(timestamp, samples)
-        callback_gyro -- function(timestamp, samples)
-        - samples is a list of 3 samples, where each sample is [x, y, z]
-        """
-
-        self.address = address
-        self.name = name
-        self.callback_eeg = callback_eeg
-        self.callback_telemetry = callback_telemetry
-        self.callback_control = callback_control
-        self.callback_acc = callback_acc
-        self.callback_gyro = callback_gyro
-        self.callback_ppg = callback_ppg
-
-        self.enable_eeg = not callback_eeg is None
-        self.enable_control = not callback_control is None
-        self.enable_telemetry = not callback_telemetry is None
-        self.enable_acc = not callback_acc is None
-        self.enable_gyro = not callback_gyro is None
-        self.enable_ppg = not callback_ppg is None
-
-        self.interface = interface
-        self.time_func = time_func
-        self.backend = helper.resolve_backend(backend)
-        self.preset = preset
-        self.disable_light = disable_light
-
-    def connect(self, interface=None):
-        """Connect to the device"""
-        try:
-            if self.backend == 'bluemuse':
-                print('Starting BlueMuse.')
-                subprocess.call('start bluemuse:', shell=True)
-                self.last_timestamp = self.time_func()
-            else:
-                print('Connecting to %s: %s...' % (self.name
-                                                   if self.name else 'Muse',
-                                                   self.address))
-                if self.backend == 'gatt':
-                    self.interface = self.interface or 'hci0'
-                    self.adapter = pygatt.GATTToolBackend(self.interface)
-                elif self.backend == 'bleak':
-                    self.adapter = backends.BleakBackend()
-                else:
-                    self.adapter = pygatt.BGAPIBackend(
-                        serial_port=self.interface)
-
-                self.adapter.start()
-                self.device = self.adapter.connect(self.address)
-                if(self.preset != None):
-                    self.select_preset(self.preset)
-
-                # subscribes to EEG stream
-                if self.enable_eeg:
-                    self._subscribe_eeg()
-
-                if self.enable_control:
-                    self._subscribe_control()
-
-                if self.enable_telemetry:
-                    self._subscribe_telemetry()
-
-                if self.enable_acc:
-                    self._subscribe_acc()
-
-                if self.enable_gyro:
-                    self._subscribe_gyro()
-
-                if self.enable_ppg:
-                    self._subscribe_ppg()
-                
-                if self.disable_light:
-                    self._disable_light()
-
-                self.last_timestamp = self.time_func()
-
-            return True
-
-        except pygatt.exceptions.BLEError as error:
-            if ("characteristic" in str(error)):
-                self.ask_reset()
-                sleep(2)
-                self.device = self.adapter.connect(self.address)
-                self.select_preset(self.preset)
-
-                # subscribes to EEG stream
-                if self.enable_eeg:
-                    self._subscribe_eeg()
-
-                if self.enable_control:
-                    self._subscribe_control()
-
-                if self.enable_telemetry:
-                    self._subscribe_telemetry()
-
-                if self.enable_acc:
-                    self._subscribe_acc()
-
-                if self.enable_gyro:
-                    self._subscribe_gyro()
-
-                if self.enable_ppg:
-                    self._subscribe_ppg()
-                
-                if self.disable_light:
-                    self._disable_light()
-
-                self.last_timestamp = self.time_func()
-
-                return True
-
-            else:
-                print('Connection to', self.address, 'failed')
-                return False
-
-    def _write_cmd(self, cmd):
-        """Wrapper to write a command to the Muse device.
-        cmd -- list of bytes"""
-        self.device.char_write_handle(0x000e, cmd, False)
-
-    def _write_cmd_str(self, cmd):
-        """Wrapper to encode and write a command string to the Muse device.
-        cmd -- string to send"""
-        self._write_cmd([len(cmd) + 1, *(ord(char) for char in cmd), ord('\n')])
-
-    def ask_control(self):
-        """Send a message to Muse to ask for the control status.
-
-        Only useful if control is enabled (to receive the answer!)
-
-        The message received is a dict with the following keys:
-        "hn": device name
-        "sn": serial number
-        "ma": MAC address
-        "id":
-        "bp": battery percentage
-        "ts":
-        "ps": preset selected
-        "rc": return status, if 0 is OK
-        """
-        if self.backend == 'bluemuse':
-            helper.warn_bluemuse_not_supported('Control information available manually by using the BlueMuse GUI.')
-            return
-        self._write_cmd_str('s')
-
-    def ask_device_info(self):
-        """Send a message to Muse to ask for the device info.
-
-        The message received is a dict with the following keys:
-        "ap":
-        "sp":
-        "tp": firmware type, e.g: "consumer"
-        "hw": hardware version?
-        "bn": build number?
-        "fw": firmware version?
-        "bl":
-        "pv": protocol version?
-        "rc": return status, if 0 is OK
-        """
-        if self.backend == 'bluemuse':
-            helper.warn_bluemuse_not_supported('Device information available manually by using the BlueMuse GUI.')
-            return
-        self._write_cmd_str('v1')
-
-    def ask_reset(self):
-        """Undocumented command reset for '*1'
-        The message received is a singleton with:
-        "rc": return status, if 0 is OK
-        """
-        self._write_cmd_str('*1')
-
-    def start(self):
-        """Start streaming."""
-        if self.backend == 'bluemuse':
-            address = self.address if self.address is not None else self.name
-            if address is None:
-                subprocess.call(
-                    'start bluemuse://start?streamfirst=true', shell=True)
-            else:
-                subprocess.call(
-                    'start bluemuse://start?addresses={0}'.format(address),
-                    shell=True)
-            return
-
-        self.first_sample = True
-        self._init_sample()
-        self._init_ppg_sample()
-        self.last_tm = 0
-        self.last_tm_ppg = 0
-        self._init_control()
-        self.resume()
-
-    def resume(self):
-        """Resume streaming, sending 'd' command"""
-        self._write_cmd_str('d')
-
-    def stop(self):
-        """Stop streaming."""
-        if self.backend == 'bluemuse':
-            address = self.address if self.address is not None else self.name
-            if address is None:
-                subprocess.call('start bluemuse://stopall', shell=True)
-            else:
-                subprocess.call(
-                    'start bluemuse://stop?addresses={0}'.format(address),
-                    shell=True)
-            return
-
-        self._write_cmd_str('h')
-
-    def keep_alive(self):
-        """Keep streaming, sending 'k' command"""
-        self._write_cmd_str('k')
-
-    def select_preset(self, preset=21):
-        """Set preset for headband configuration
-
-        See details here https://articles.jaredcamins.com/figuring-out-bluetooth-low-energy-part-2-750565329a7d
-        For 2016 headband, possible choice are 'p20' and 'p21'.
-        Untested but possible values include 'p22','p23','p31','p32','p50','p51','p52','p53','p60','p61','p63','pAB','pAD'
-        Default is 'p21'."""
-
-        if type(preset) is int:
-            preset = str(preset)
-        if preset[0] == 'p':
-            preset = preset[1:]
-        if str(preset) != '21':
-            print('Sending command for non-default preset: p' + preset)
-        preset = bytes(preset, 'utf-8')
-        self._write_cmd([0x04, 0x70, *preset, 0x0a])
-
-    def disconnect(self):
-        """disconnect."""
-        if self.backend == 'bluemuse':
-            subprocess.call('start bluemuse://shutdown', shell=True)
-            return
-
-        self.device.disconnect()
-        if self.adapter:
-            self.adapter.stop()
-
-    def _subscribe_eeg(self):
-        """subscribe to eeg stream."""
-        self.device.subscribe(MUSE_GATT_ATTR_TP9, callback=self._handle_eeg)
-        self.device.subscribe(MUSE_GATT_ATTR_AF7, callback=self._handle_eeg)
-        self.device.subscribe(MUSE_GATT_ATTR_AF8, callback=self._handle_eeg)
-        self.device.subscribe(MUSE_GATT_ATTR_TP10, callback=self._handle_eeg)
-        self.device.subscribe(
-            MUSE_GATT_ATTR_RIGHTAUX, callback=self._handle_eeg)
-
-    def _unpack_eeg_channel(self, packet):
-        """Decode data packet of one EEG channel.
-
-        Each packet is encoded with a 16bit timestamp followed by 12 time
-        samples with a 12 bit resolution.
-        """
-        aa = bitstring.Bits(bytes=packet)
-        pattern = "uint:16,uint:12,uint:12,uint:12,uint:12,uint:12,uint:12, \
-                   uint:12,uint:12,uint:12,uint:12,uint:12,uint:12"
-
-        res = aa.unpack(pattern)
-        packetIndex = res[0]
-        data = res[1:]
-        # 12 bits on a 2 mVpp range
-        data = 0.48828125 * (np.array(data) - 2048)
-        return packetIndex, data
-
-    def _init_sample(self):
-        """initialize array to store the samples"""
-        self.timestamps = np.full(5, np.nan)
-        self.data = np.zeros((5, 12))
-
-    def _init_ppg_sample(self):
-        """ Initialise array to store PPG samples
-
-            Must be separate from the EEG packets since they occur with a different sampling rate. Ideally the counters
-            would always match, but this is not guaranteed
-        """
-        self.timestamps_ppg = np.full(3, np.nan)
-        self.data_ppg = np.zeros((3, 6))
-
-    def _init_timestamp_correction(self):
-        """Init IRLS params"""
-        # initial params for the timestamp correction
-        # the time it started + the inverse of sampling rate
-        self.sample_index = 0
-        self.sample_index_ppg = 0
-        self._P = 1e-4
-        t0 = self.time_func()
-        self.reg_params = np.array([t0, 1. / MUSE_SAMPLING_EEG_RATE])
-        self.reg_ppg_sample_rate = np.array([t0, 1. / MUSE_SAMPLING_PPG_RATE])
-
-    def _update_timestamp_correction(self, t_source, t_receiver):
-        """Update regression for dejittering
-
-        This is based on Recursive least square.
-        See https://arxiv.org/pdf/1308.3846.pdf.
-        """
-
-        # remove the offset
-        t_receiver = t_receiver - self.reg_params[0]
-
-        # least square estimation
-        P = self._P
-        R = self.reg_params[1]
-        P = P - ((P**2) * (t_source**2)) / (1 - (P * (t_source**2)))
-        R = R + P * t_source * (t_receiver - t_source * R)
-
-        # update parameters
-        self.reg_params[1] = R
-        self._P = P
-
-    def _handle_eeg(self, handle, data):
-        """Callback for receiving a sample.
-
-        samples are received in this order : 44, 41, 38, 32, 35
-        wait until we get 35 and call the data callback
-        """
-        if self.first_sample:
-            self._init_timestamp_correction()
-            self.first_sample = False
-
-        timestamp = self.time_func()
-        index = int((handle - 32) / 3)
-        tm, d = self._unpack_eeg_channel(data)
-
-        if self.last_tm == 0:
-            self.last_tm = tm - 1
-
-        self.data[index] = d
-        self.timestamps[index] = timestamp
-        # last data received
-        if handle == 35:
-            if tm != self.last_tm + 1:
-                if (tm - self.last_tm) != -65535:  # counter reset
-                    print("missing sample %d : %d" % (tm, self.last_tm))
-                    # correct sample index for timestamp estimation
-                    self.sample_index += 12 * (tm - self.last_tm + 1)
-
-            self.last_tm = tm
-
-            # calculate index of time samples
-            idxs = np.arange(0, 12) + self.sample_index
-            self.sample_index += 12
-
-            # update timestamp correction
-            # We received the first packet as soon as the last timestamp got
-            # sampled
-            self._update_timestamp_correction(idxs[-1], np.nanmin(
-                self.timestamps))
-
-            # timestamps are extrapolated backwards based on sampling rate
-            # and current time
-            timestamps = self.reg_params[1] * idxs + self.reg_params[0]
-
-            # push data
-            self.callback_eeg(self.data, timestamps)
-
-            # save last timestamp for disconnection timer
-            self.last_timestamp = timestamps[-1]
-
-            # reset sample
-            self._init_sample()
-
-    def _init_control(self):
-        """Variable to store the current incoming message."""
-        self._current_msg = ""
-
-    def _subscribe_control(self):
-        self.device.subscribe(
-            MUSE_GATT_ATTR_STREAM_TOGGLE, callback=self._handle_control)
-
-        self._init_control()
-
-    def _handle_control(self, handle, packet):
-        """Handle the incoming messages from the 0x000e handle.
-
-        Each message is 20 bytes
-        The first byte, call it n, is the length of the incoming string.
-        The rest of the bytes are in ASCII, and only n chars are useful
-
-        Multiple messages together are a json object (or dictionary in python)
-        If a message has a '}' then the whole dict is finished.
-
-        Example:
-        {'key': 'value',
-        'key2': 'really-long
-        -value',
-        'key3': 'value3'}
-
-        each line is a message, the 4 messages are a json object.
-        """
-        if handle != 14:
-            return
-
-        # Decode data
-        bit_decoder = bitstring.Bits(bytes=packet)
-        pattern = "uint:8,uint:8,uint:8,uint:8,uint:8,uint:8,uint:8,uint:8,uint:8,uint:8, \
-                    uint:8,uint:8,uint:8,uint:8,uint:8,uint:8,uint:8,uint:8,uint:8,uint:8"
-
-        chars = bit_decoder.unpack(pattern)
-
-        # Length of the string
-        n_incoming = chars[0]
-
-        # Parse as chars, only useful bytes
-        incoming_message = "".join(map(chr, chars[1:]))[:n_incoming]
-
-        # Add to current message
-        self._current_msg += incoming_message
-
-        if incoming_message[-1] == '}':  # Message ended completely
-            self.callback_control(self._current_msg)
-
-            self._init_control()
-
-    def _subscribe_telemetry(self):
-        self.device.subscribe(
-            MUSE_GATT_ATTR_TELEMETRY, callback=self._handle_telemetry)
-
-    def _handle_telemetry(self, handle, packet):
-        """Handle the telemetry (battery, temperature and stuff) incoming data
-        """
-
-        if handle != 26:  # handle 0x1a
-            return
-        timestamp = self.time_func()
-
-        bit_decoder = bitstring.Bits(bytes=packet)
-        pattern = "uint:16,uint:16,uint:16,uint:16,uint:16"  # The rest is 0 padding
-        data = bit_decoder.unpack(pattern)
-
-        battery = data[1] / 512
-        fuel_gauge = data[2] * 2.2
-        adc_volt = data[3]
-        temperature = data[4]
-
-        self.callback_telemetry(timestamp, battery, fuel_gauge, adc_volt,
-                                temperature)
-
-    def _unpack_imu_channel(self, packet, scale=1):
-        """Decode data packet of the accelerometer and gyro (imu) channels.
-
-        Each packet is encoded with a 16bit timestamp followed by 9 samples
-        with a 16 bit resolution.
-        """
-        bit_decoder = bitstring.Bits(bytes=packet)
-        pattern = "uint:16,int:16,int:16,int:16,int:16, \
-                   int:16,int:16,int:16,int:16,int:16"
-
-        data = bit_decoder.unpack(pattern)
-
-        packet_index = data[0]
-
-        samples = np.array(data[1:]).reshape((3, 3), order='F') * scale
-
-        return packet_index, samples
-
-    def _subscribe_acc(self):
-        self.device.subscribe(
-            MUSE_GATT_ATTR_ACCELEROMETER, callback=self._handle_acc)
-
-    def _handle_acc(self, handle, packet):
-        """Handle incoming accelerometer data.
-
-        sampling rate: ~17 x second (3 samples in each message, roughly 50Hz)"""
-        if handle != 23:  # handle 0x17
-            return
-        timestamps = [self.time_func()] * 3
-
-        # save last timestamp for disconnection timer
-        self.last_timestamp = timestamps[-1]
-
-        packet_index, samples = self._unpack_imu_channel(
-            packet, scale=MUSE_ACCELEROMETER_SCALE_FACTOR)
-
-        self.callback_acc(samples, timestamps)
-
-    def _subscribe_gyro(self):
-        self.device.subscribe(MUSE_GATT_ATTR_GYRO, callback=self._handle_gyro)
-
-    def _handle_gyro(self, handle, packet):
-        """Handle incoming gyroscope data.
-
-        sampling rate: ~17 x second (3 samples in each message, roughly 50Hz)"""
-        if handle != 20:  # handle 0x14
-            return
-
-        timestamps = [self.time_func()] * 3
-
-        # save last timestamp for disconnection timer
-        self.last_timestamp = timestamps[-1]
-
-        packet_index, samples = self._unpack_imu_channel(
-            packet, scale=MUSE_GYRO_SCALE_FACTOR)
-
-        self.callback_gyro(samples, timestamps)
-
-    def _subscribe_ppg(self):
-        try:
-            """subscribe to ppg stream."""
-            self.device.subscribe(
-                MUSE_GATT_ATTR_PPG1, callback=self._handle_ppg)
-            self.device.subscribe(
-                MUSE_GATT_ATTR_PPG2, callback=self._handle_ppg)
-            self.device.subscribe(
-                MUSE_GATT_ATTR_PPG3, callback=self._handle_ppg)
-
-        except pygatt.exceptions.BLEError as error:
-            raise Exception(
-                'PPG data is not available on this device. PPG is only available on Muse 2'
-            )
-
-    def _handle_ppg(self, handle, data):
-        """Callback for receiving a sample.
-
-        samples are received in this order : 56, 59, 62
-        wait until we get x and call the data callback
-        """
-        timestamp = self.time_func()
-        index = int((handle - 56) / 3)
-        tm, d = self._unpack_ppg_channel(data)
-
-        if self.last_tm_ppg == 0:
-            self.last_tm_ppg = tm - 1
-
-        self.data_ppg[index] = d
-        self.timestamps_ppg[index] = timestamp
-        # last data received
-        if handle == 62:
-            if tm != self.last_tm_ppg + 1:
-                print("missing sample %d : %d" % (tm, self.last_tm_ppg))
-            self.last_tm_ppg = tm
-
-            # calculate index of time samples
-            idxs = np.arange(0, LSL_PPG_CHUNK) + self.sample_index_ppg
-            self.sample_index_ppg += LSL_PPG_CHUNK
-
-            # timestamps are extrapolated backwards based on sampling rate and current time
-            timestamps = self.reg_ppg_sample_rate[1] * \
-                idxs + self.reg_ppg_sample_rate[0]
-
-            # save last timestamp for disconnection timer
-            self.last_timestamp = timestamps[-1]
-
-            # push data
-            if self.callback_ppg:
-                self.callback_ppg(self.data_ppg, timestamps)
-
-            # reset sample
-            self._init_ppg_sample()
-
-    def _unpack_ppg_channel(self, packet):
-        """Decode data packet of one PPG channel.
-        Each packet is encoded with a 16bit timestamp followed by 3
-        samples with an x bit resolution.
-        """
-
-        aa = bitstring.Bits(bytes=packet)
-        pattern = "uint:16,uint:24,uint:24,uint:24,uint:24,uint:24,uint:24"
-        res = aa.unpack(pattern)
-        packetIndex = res[0]
-        data = res[1:]
-
-        return packetIndex, data
-    
-    def _disable_light(self):
-        self._write_cmd_str('L0')
+import logging
+import sys
+
+import bitstring
+import pygatt
+import numpy as np
+from time import time, sleep
+from sys import platform
+import subprocess
+from . import backends
+from . import helper
+from .constants import *
+
+logger = logging.getLogger(__name__)
+
+class Muse():
+    """Muse headband"""
+
+    def __init__(self,
+                 address,
+                 callback_eeg=None,
+                 callback_control=None,
+                 callback_telemetry=None,
+                 callback_acc=None,
+                 callback_gyro=None,
+                 callback_ppg=None,
+                 backend='auto',
+                 interface=None,
+                 time_func=time,
+                 name=None,
+                 preset=None,
+                 disable_light=False,
+                 log_level=logging.ERROR):
+        """Initialize
+
+        callback_eeg -- callback for eeg data, function(data, timestamps)
+        callback_control -- function(message)
+        callback_telemetry -- function(timestamp, battery, fuel_gauge,
+                                       adc_volt, temperature)
+
+        callback_acc -- function(timestamp, samples)
+        callback_gyro -- function(timestamp, samples)
+        - samples is a list of 3 samples, where each sample is [x, y, z]
+        """
+        logging.basicConfig(stream=sys.stdout, level=log_level)
+
+        self.address = address
+        self.name = name
+        self.callback_eeg = callback_eeg
+        self.callback_telemetry = callback_telemetry
+        self.callback_control = callback_control
+        self.callback_acc = callback_acc
+        self.callback_gyro = callback_gyro
+        self.callback_ppg = callback_ppg
+
+        self.enable_eeg = not callback_eeg is None
+        self.enable_control = not callback_control is None
+        self.enable_telemetry = not callback_telemetry is None
+        self.enable_acc = not callback_acc is None
+        self.enable_gyro = not callback_gyro is None
+        self.enable_ppg = not callback_ppg is None
+
+        self.interface = interface
+        self.time_func = time_func
+        self.backend = helper.resolve_backend(backend)
+        self.preset = preset
+        self.disable_light = disable_light
+
+    def connect(self, interface=None, retries=0):
+        """Connect to the device"""
+        try:
+            if self.backend == 'bluemuse':
+                logger.info('Starting BlueMuse.')
+                subprocess.call('start bluemuse:', shell=True)
+                self.last_timestamp = self.time_func()
+            else:
+                logger.info('Connecting to %s: %s...' % (self.name
+                                                   if self.name else 'Muse',
+                                                   self.address))
+                if self.backend == 'gatt':
+                    self.interface = self.interface or 'hci0'
+                    self.adapter = pygatt.GATTToolBackend(self.interface)
+                elif self.backend == 'bleak':
+                    self.adapter = backends.BleakBackend()
+                else:
+                    self.adapter = pygatt.BGAPIBackend(
+                        serial_port=self.interface)
+
+                self.adapter.start()
+                if ((device := self.adapter.connect(self.address, retries))
+                    is None):
+                    return False
+                self.device = device
+
+                if(self.preset != None):
+                    self.select_preset(self.preset)
+
+                # subscribes to EEG stream
+                if self.enable_eeg:
+                    self._subscribe_eeg()
+
+                if self.enable_control:
+                    self._subscribe_control()
+
+                if self.enable_telemetry:
+                    self._subscribe_telemetry()
+
+                if self.enable_acc:
+                    self._subscribe_acc()
+
+                if self.enable_gyro:
+                    self._subscribe_gyro()
+
+                if self.enable_ppg:
+                    self._subscribe_ppg()
+                
+                if self.disable_light:
+                    self._disable_light()
+
+                self.last_timestamp = self.time_func()
+
+            return True
+
+        except pygatt.exceptions.BLEError as error:
+            if ("characteristic" in str(error)):
+                self.ask_reset()
+                sleep(2)
+                self.device = self.adapter.connect(self.address)
+                self.select_preset(self.preset)
+
+                # subscribes to EEG stream
+                if self.enable_eeg:
+                    self._subscribe_eeg()
+
+                if self.enable_control:
+                    self._subscribe_control()
+
+                if self.enable_telemetry:
+                    self._subscribe_telemetry()
+
+                if self.enable_acc:
+                    self._subscribe_acc()
+
+                if self.enable_gyro:
+                    self._subscribe_gyro()
+
+                if self.enable_ppg:
+                    self._subscribe_ppg()
+                
+                if self.disable_light:
+                    self._disable_light()
+
+                self.last_timestamp = self.time_func()
+
+                return True
+
+            else:
+                logger.error('Connection to', self.address, 'failed')
+                return False
+
+    def _write_cmd(self, cmd):
+        """Wrapper to write a command to the Muse device.
+        cmd -- list of bytes"""
+        self.device.char_write_handle(0x000e, cmd, False)
+
+    def _write_cmd_str(self, cmd):
+        """Wrapper to encode and write a command string to the Muse device.
+        cmd -- string to send"""
+        self._write_cmd([len(cmd) + 1, *(ord(char) for char in cmd), ord('\n')])
+
+    def ask_control(self):
+        """Send a message to Muse to ask for the control status.
+
+        Only useful if control is enabled (to receive the answer!)
+
+        The message received is a dict with the following keys:
+        "hn": device name
+        "sn": serial number
+        "ma": MAC address
+        "id":
+        "bp": battery percentage
+        "ts":
+        "ps": preset selected
+        "rc": return status, if 0 is OK
+        """
+        if self.backend == 'bluemuse':
+            helper.warn_bluemuse_not_supported('Control information available manually by using the BlueMuse GUI.')
+            return
+        self._write_cmd_str('s')
+
+    def ask_device_info(self):
+        """Send a message to Muse to ask for the device info.
+
+        The message received is a dict with the following keys:
+        "ap":
+        "sp":
+        "tp": firmware type, e.g: "consumer"
+        "hw": hardware version?
+        "bn": build number?
+        "fw": firmware version?
+        "bl":
+        "pv": protocol version?
+        "rc": return status, if 0 is OK
+        """
+        if self.backend == 'bluemuse':
+            helper.warn_bluemuse_not_supported('Device information available manually by using the BlueMuse GUI.')
+            return
+        self._write_cmd_str('v1')
+
+    def ask_reset(self):
+        """Undocumented command reset for '*1'
+        The message received is a singleton with:
+        "rc": return status, if 0 is OK
+        """
+        self._write_cmd_str('*1')
+
+    def start(self):
+        """Start streaming."""
+        if self.backend == 'bluemuse':
+            address = self.address if self.address is not None else self.name
+            if address is None:
+                subprocess.call(
+                    'start bluemuse://start?streamfirst=true', shell=True)
+            else:
+                subprocess.call(
+                    'start bluemuse://start?addresses={0}'.format(address),
+                    shell=True)
+            return
+
+        self.first_sample = True
+        self._init_sample()
+        self._init_ppg_sample()
+        self.last_tm = 0
+        self.last_tm_ppg = 0
+        self._init_control()
+        self.resume()
+
+    def resume(self):
+        """Resume streaming, sending 'd' command"""
+        self._write_cmd_str('d')
+
+    def stop(self):
+        """Stop streaming."""
+        if self.backend == 'bluemuse':
+            address = self.address if self.address is not None else self.name
+            if address is None:
+                subprocess.call('start bluemuse://stopall', shell=True)
+            else:
+                subprocess.call(
+                    'start bluemuse://stop?addresses={0}'.format(address),
+                    shell=True)
+            return
+
+        self._write_cmd_str('h')
+
+    def keep_alive(self):
+        """Keep streaming, sending 'k' command"""
+        self._write_cmd_str('k')
+
+    def select_preset(self, preset=21):
+        """Set preset for headband configuration
+
+        See details here https://articles.jaredcamins.com/figuring-out-bluetooth-low-energy-part-2-750565329a7d
+        For 2016 headband, possible choice are 'p20' and 'p21'.
+        Untested but possible values include 'p22','p23','p31','p32','p50','p51','p52','p53','p60','p61','p63','pAB','pAD'
+        Default is 'p21'."""
+
+        if type(preset) is int:
+            preset = str(preset)
+        if preset[0] == 'p':
+            preset = preset[1:]
+        if str(preset) != '21':
+            logger.debug('Sending command for non-default preset: p' + preset)
+        preset = bytes(preset, 'utf-8')
+        self._write_cmd([0x04, 0x70, *preset, 0x0a])
+
+    def disconnect(self):
+        """disconnect."""
+        if self.backend == 'bluemuse':
+            subprocess.call('start bluemuse://shutdown', shell=True)
+            return
+
+        self.device.disconnect()
+        if self.adapter:
+            self.adapter.stop()
+
+    def _subscribe_eeg(self):
+        """subscribe to eeg stream."""
+        self.device.subscribe(MUSE_GATT_ATTR_TP9, callback=self._handle_eeg)
+        self.device.subscribe(MUSE_GATT_ATTR_AF7, callback=self._handle_eeg)
+        self.device.subscribe(MUSE_GATT_ATTR_AF8, callback=self._handle_eeg)
+        self.device.subscribe(MUSE_GATT_ATTR_TP10, callback=self._handle_eeg)
+        self.device.subscribe(
+            MUSE_GATT_ATTR_RIGHTAUX, callback=self._handle_eeg)
+
+    def _unpack_eeg_channel(self, packet):
+        """Decode data packet of one EEG channel.
+
+        Each packet is encoded with a 16bit timestamp followed by 12 time
+        samples with a 12 bit resolution.
+        """
+        aa = bitstring.Bits(bytes=packet)
+        pattern = "uint:16,uint:12,uint:12,uint:12,uint:12,uint:12,uint:12, \
+                   uint:12,uint:12,uint:12,uint:12,uint:12,uint:12"
+
+        res = aa.unpack(pattern)
+        packetIndex = res[0]
+        data = res[1:]
+        # 12 bits on a 2 mVpp range
+        data = 0.48828125 * (np.array(data) - 2048)
+        return packetIndex, data
+
+    def _init_sample(self):
+        """initialize array to store the samples"""
+        self.timestamps = np.full(5, np.nan)
+        self.data = np.zeros((5, 12))
+
+    def _init_ppg_sample(self):
+        """ Initialise array to store PPG samples
+
+            Must be separate from the EEG packets since they occur with a different sampling rate. Ideally the counters
+            would always match, but this is not guaranteed
+        """
+        self.timestamps_ppg = np.full(3, np.nan)
+        self.data_ppg = np.zeros((3, 6))
+
+    def _init_timestamp_correction(self):
+        """Init IRLS params"""
+        # initial params for the timestamp correction
+        # the time it started + the inverse of sampling rate
+        self.sample_index = 0
+        self.sample_index_ppg = 0
+        self._P = 1e-4
+        t0 = self.time_func()
+        self.reg_params = np.array([t0, 1. / MUSE_SAMPLING_EEG_RATE])
+        self.reg_ppg_sample_rate = np.array([t0, 1. / MUSE_SAMPLING_PPG_RATE])
+
+    def _update_timestamp_correction(self, t_source, t_receiver):
+        """Update regression for dejittering
+
+        This is based on Recursive least square.
+        See https://arxiv.org/pdf/1308.3846.pdf.
+        """
+
+        # remove the offset
+        t_receiver = t_receiver - self.reg_params[0]
+
+        # least square estimation
+        P = self._P
+        R = self.reg_params[1]
+        P = P - ((P**2) * (t_source**2)) / (1 - (P * (t_source**2)))
+        R = R + P * t_source * (t_receiver - t_source * R)
+
+        # update parameters
+        self.reg_params[1] = R
+        self._P = P
+
+    def _handle_eeg(self, handle, data):
+        """Callback for receiving a sample.
+
+        samples are received in this order : 44, 41, 38, 32, 35
+        wait until we get 35 and call the data callback
+        """
+        if self.first_sample:
+            self._init_timestamp_correction()
+            self.first_sample = False
+
+        timestamp = self.time_func()
+        index = int((handle - 32) / 3)
+        tm, d = self._unpack_eeg_channel(data)
+
+        if self.last_tm == 0:
+            self.last_tm = tm - 1
+
+        self.data[index] = d
+        self.timestamps[index] = timestamp
+        # last data received
+        if handle == 35:
+            if tm != self.last_tm + 1:
+                if (tm - self.last_tm) != -65535:  # counter reset
+                    logger.debug("missing sample %d : %d" % (tm, self.last_tm))
+                    # correct sample index for timestamp estimation
+                    self.sample_index += 12 * (tm - self.last_tm + 1)
+
+            self.last_tm = tm
+
+            # calculate index of time samples
+            idxs = np.arange(0, 12) + self.sample_index
+            self.sample_index += 12
+
+            # update timestamp correction
+            # We received the first packet as soon as the last timestamp got
+            # sampled
+            self._update_timestamp_correction(idxs[-1], np.nanmin(
+                self.timestamps))
+
+            # timestamps are extrapolated backwards based on sampling rate
+            # and current time
+            timestamps = self.reg_params[1] * idxs + self.reg_params[0]
+
+            # push data
+            self.callback_eeg(self.data, timestamps)
+
+            # save last timestamp for disconnection timer
+            self.last_timestamp = timestamps[-1]
+
+            # reset sample
+            self._init_sample()
+
+    def _init_control(self):
+        """Variable to store the current incoming message."""
+        self._current_msg = ""
+
+    def _subscribe_control(self):
+        self.device.subscribe(
+            MUSE_GATT_ATTR_STREAM_TOGGLE, callback=self._handle_control)
+
+        self._init_control()
+
+    def _handle_control(self, handle, packet):
+        """Handle the incoming messages from the 0x000e handle.
+
+        Each message is 20 bytes
+        The first byte, call it n, is the length of the incoming string.
+        The rest of the bytes are in ASCII, and only n chars are useful
+
+        Multiple messages together are a json object (or dictionary in python)
+        If a message has a '}' then the whole dict is finished.
+
+        Example:
+        {'key': 'value',
+        'key2': 'really-long
+        -value',
+        'key3': 'value3'}
+
+        each line is a message, the 4 messages are a json object.
+        """
+        if handle != 14:
+            return
+
+        # Decode data
+        bit_decoder = bitstring.Bits(bytes=packet)
+        pattern = "uint:8,uint:8,uint:8,uint:8,uint:8,uint:8,uint:8,uint:8,uint:8,uint:8, \
+                    uint:8,uint:8,uint:8,uint:8,uint:8,uint:8,uint:8,uint:8,uint:8,uint:8"
+
+        chars = bit_decoder.unpack(pattern)
+
+        # Length of the string
+        n_incoming = chars[0]
+
+        # Parse as chars, only useful bytes
+        incoming_message = "".join(map(chr, chars[1:]))[:n_incoming]
+
+        # Add to current message
+        self._current_msg += incoming_message
+
+        if incoming_message[-1] == '}':  # Message ended completely
+            self.callback_control(self._current_msg)
+
+            self._init_control()
+
+    def _subscribe_telemetry(self):
+        self.device.subscribe(
+            MUSE_GATT_ATTR_TELEMETRY, callback=self._handle_telemetry)
+
+    def _handle_telemetry(self, handle, packet):
+        """Handle the telemetry (battery, temperature and stuff) incoming data
+        """
+
+        if handle != 26:  # handle 0x1a
+            return
+        timestamp = self.time_func()
+
+        bit_decoder = bitstring.Bits(bytes=packet)
+        pattern = "uint:16,uint:16,uint:16,uint:16,uint:16"  # The rest is 0 padding
+        data = bit_decoder.unpack(pattern)
+
+        battery = data[1] / 512
+        fuel_gauge = data[2] * 2.2
+        adc_volt = data[3]
+        temperature = data[4]
+
+        self.callback_telemetry(timestamp, battery, fuel_gauge, adc_volt,
+                                temperature)
+
+    def _unpack_imu_channel(self, packet, scale=1):
+        """Decode data packet of the accelerometer and gyro (imu) channels.
+
+        Each packet is encoded with a 16bit timestamp followed by 9 samples
+        with a 16 bit resolution.
+        """
+        bit_decoder = bitstring.Bits(bytes=packet)
+        pattern = "uint:16,int:16,int:16,int:16,int:16, \
+                   int:16,int:16,int:16,int:16,int:16"
+
+        data = bit_decoder.unpack(pattern)
+
+        packet_index = data[0]
+
+        samples = np.array(data[1:]).reshape((3, 3), order='F') * scale
+
+        return packet_index, samples
+
+    def _subscribe_acc(self):
+        self.device.subscribe(
+            MUSE_GATT_ATTR_ACCELEROMETER, callback=self._handle_acc)
+
+    def _handle_acc(self, handle, packet):
+        """Handle incoming accelerometer data.
+
+        sampling rate: ~17 x second (3 samples in each message, roughly 50Hz)"""
+        if handle != 23:  # handle 0x17
+            return
+        timestamps = [self.time_func()] * 3
+
+        # save last timestamp for disconnection timer
+        self.last_timestamp = timestamps[-1]
+
+        packet_index, samples = self._unpack_imu_channel(
+            packet, scale=MUSE_ACCELEROMETER_SCALE_FACTOR)
+
+        self.callback_acc(samples, timestamps)
+
+    def _subscribe_gyro(self):
+        self.device.subscribe(MUSE_GATT_ATTR_GYRO, callback=self._handle_gyro)
+
+    def _handle_gyro(self, handle, packet):
+        """Handle incoming gyroscope data.
+
+        sampling rate: ~17 x second (3 samples in each message, roughly 50Hz)"""
+        if handle != 20:  # handle 0x14
+            return
+
+        timestamps = [self.time_func()] * 3
+
+        # save last timestamp for disconnection timer
+        self.last_timestamp = timestamps[-1]
+
+        packet_index, samples = self._unpack_imu_channel(
+            packet, scale=MUSE_GYRO_SCALE_FACTOR)
+
+        self.callback_gyro(samples, timestamps)
+
+    def _subscribe_ppg(self):
+        try:
+            """subscribe to ppg stream."""
+            self.device.subscribe(
+                MUSE_GATT_ATTR_PPG1, callback=self._handle_ppg)
+            self.device.subscribe(
+                MUSE_GATT_ATTR_PPG2, callback=self._handle_ppg)
+            self.device.subscribe(
+                MUSE_GATT_ATTR_PPG3, callback=self._handle_ppg)
+
+        except pygatt.exceptions.BLEError as error:
+            raise Exception(
+                'PPG data is not available on this device. PPG is only available on Muse 2'
+            )
+
+    def _handle_ppg(self, handle, data):
+        """Callback for receiving a sample.
+
+        samples are received in this order : 56, 59, 62
+        wait until we get x and call the data callback
+        """
+        timestamp = self.time_func()
+        index = int((handle - 56) / 3)
+        tm, d = self._unpack_ppg_channel(data)
+
+        if self.last_tm_ppg == 0:
+            self.last_tm_ppg = tm - 1
+
+        self.data_ppg[index] = d
+        self.timestamps_ppg[index] = timestamp
+        # last data received
+        if handle == 62:
+            if tm != self.last_tm_ppg + 1:
+                logger.debug("missing sample %d : %d" % (tm, self.last_tm_ppg))
+            self.last_tm_ppg = tm
+
+            # calculate index of time samples
+            idxs = np.arange(0, LSL_PPG_CHUNK) + self.sample_index_ppg
+            self.sample_index_ppg += LSL_PPG_CHUNK
+
+            # timestamps are extrapolated backwards based on sampling rate and current time
+            timestamps = self.reg_ppg_sample_rate[1] * \
+                idxs + self.reg_ppg_sample_rate[0]
+
+            # save last timestamp for disconnection timer
+            self.last_timestamp = timestamps[-1]
+
+            # push data
+            if self.callback_ppg:
+                self.callback_ppg(self.data_ppg, timestamps)
+
+            # reset sample
+            self._init_ppg_sample()
+
+    def _unpack_ppg_channel(self, packet):
+        """Decode data packet of one PPG channel.
+        Each packet is encoded with a 16bit timestamp followed by 3
+        samples with an x bit resolution.
+        """
+
+        aa = bitstring.Bits(bytes=packet)
+        pattern = "uint:16,uint:24,uint:24,uint:24,uint:24,uint:24,uint:24"
+        res = aa.unpack(pattern)
+        packetIndex = res[0]
+        data = res[1:]
+
+        return packetIndex, data
+    
+    def _disable_light(self):
+        self._write_cmd_str('L0')
```

### Comparing `muselsl-2.2.2/muselsl/record.py` & `muselsl-2.3.0/muselsl/record.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,242 +1,270 @@
-import numpy as np
-import pandas as pd
-import os
-from typing import Union, List, Optional
-from pathlib import Path
-from pylsl import StreamInlet, resolve_byprop
-from sklearn.linear_model import LinearRegression
-from time import time, strftime, gmtime
-from .stream import find_muse
-from . import backends
-from .muse import Muse
-from .constants import LSL_SCAN_TIMEOUT, LSL_EEG_CHUNK, LSL_PPG_CHUNK, LSL_ACC_CHUNK, LSL_GYRO_CHUNK
-
-# Records a fixed duration of EEG data from an LSL stream into a CSV file
-
-
-def record(
-    duration: int,
-    filename=None,
-    dejitter=False,
-    data_source="EEG",
-    continuous: bool = True,
-) -> None:
-    chunk_length = LSL_EEG_CHUNK
-    if data_source == "PPG":
-        chunk_length = LSL_PPG_CHUNK
-    if data_source == "ACC":
-        chunk_length = LSL_ACC_CHUNK
-    if data_source == "GYRO":
-        chunk_length = LSL_GYRO_CHUNK
-
-    if not filename:
-        filename = os.path.join(os.getcwd(), "%s_recording_%s.csv" %
-                                (data_source,
-                                 strftime('%Y-%m-%d-%H.%M.%S', gmtime())))
-
-    print("Looking for a %s stream..." % (data_source))
-    streams = resolve_byprop('type', data_source, timeout=LSL_SCAN_TIMEOUT)
-
-    if len(streams) == 0:
-        print("Can't find %s stream." % (data_source))
-        return
-
-    print("Started acquiring data.")
-    inlet = StreamInlet(streams[0], max_chunklen=chunk_length)
-    # eeg_time_correction = inlet.time_correction()
-
-    print("Looking for a Markers stream...")
-    marker_streams = resolve_byprop(
-        'name', 'Markers', timeout=LSL_SCAN_TIMEOUT)
-
-    if marker_streams:
-        inlet_marker = StreamInlet(marker_streams[0])
-    else:
-        inlet_marker = False
-        print("Can't find Markers stream.")
-
-    info = inlet.info()
-    description = info.desc()
-
-    Nchan = info.channel_count()
-
-    ch = description.child('channels').first_child()
-    ch_names = [ch.child_value('label')]
-    for i in range(1, Nchan):
-        ch = ch.next_sibling()
-        ch_names.append(ch.child_value('label'))
-
-    res = []
-    timestamps = []
-    markers = []
-    t_init = time()
-    time_correction = inlet.time_correction()
-    last_written_timestamp = None
-    print('Start recording at time t=%.3f' % t_init)
-    print('Time correction: ', time_correction)
-    while (time() - t_init) < duration:
-        try:
-            data, timestamp = inlet.pull_chunk(
-                timeout=1.0, max_samples=chunk_length)
-
-            if timestamp:
-                res.append(data)
-                timestamps.extend(timestamp)
-                tr = time()
-            if inlet_marker:
-                marker, timestamp = inlet_marker.pull_sample(timeout=0.0)
-                if timestamp:
-                    markers.append([marker, timestamp])
-
-            # Save every 5s
-            if continuous and (last_written_timestamp is None or last_written_timestamp + 5 < timestamps[-1]):
-                _save(
-                    filename,
-                    res,
-                    timestamps,
-                    time_correction,
-                    dejitter,
-                    inlet_marker,
-                    markers,
-                    ch_names,
-                    last_written_timestamp=last_written_timestamp,
-                )
-                last_written_timestamp = timestamps[-1]
-
-        except KeyboardInterrupt:
-            break
-
-    time_correction = inlet.time_correction()
-    print("Time correction: ", time_correction)
-
-    _save(
-        filename,
-        res,
-        timestamps,
-        time_correction,
-        dejitter,
-        inlet_marker,
-        markers,
-        ch_names,
-    )
-
-    print("Done - wrote file: {}".format(filename))
-
-
-def _save(
-    filename: Union[str, Path],
-    res: list,
-    timestamps: list,
-    time_correction,
-    dejitter: bool,
-    inlet_marker,
-    markers,
-    ch_names: List[str],
-    last_written_timestamp: Optional[float] = None,
-):
-    res = np.concatenate(res, axis=0)
-    timestamps = np.array(timestamps) + time_correction
-
-    if dejitter:
-        y = timestamps
-        X = np.atleast_2d(np.arange(0, len(y))).T
-        lr = LinearRegression()
-        lr.fit(X, y)
-        timestamps = lr.predict(X)
-
-    res = np.c_[timestamps, res]
-    data = pd.DataFrame(data=res, columns=["timestamps"] + ch_names)
-
-    directory = os.path.dirname(filename)
-    if not os.path.exists(directory):
-        os.makedirs(directory)
-
-    if inlet_marker and markers:
-        n_markers = len(markers[0][0])
-        for ii in range(n_markers):
-            data['Marker%d' % ii] = 0
-        # process markers:
-        for marker in markers:
-            # find index of markers
-            ix = np.argmin(np.abs(marker[1] - timestamps))
-            for ii in range(n_markers):
-                data.loc[ix, "Marker%d" % ii] = marker[0][ii]
-
-    # If file doesn't exist, create with headers
-    # If it does exist, just append new rows
-    if not Path(filename).exists():
-        # print("Saving whole file")
-        data.to_csv(filename, float_format='%.3f', index=False)
-    else:
-        # print("Appending file")
-        # truncate already written timestamps
-        data = data[data['timestamps'] > last_written_timestamp]
-        data.to_csv(filename, float_format='%.3f', index=False, mode='a', header=False)
-
-
-
-# Rercord directly from a Muse without the use of LSL
-
-
-def record_direct(duration,
-                  address,
-                  filename=None,
-                  backend='auto',
-                  interface=None,
-                  name=None):
-    if backend == 'bluemuse':
-        raise (NotImplementedError(
-            'Direct record not supported with BlueMuse backend. Use record after starting stream instead.'
-        ))
-
-    if not address:
-        found_muse = find_muse(name, backend)
-        if not found_muse:
-            print('Muse could not be found')
-            return
-        else:
-            address = found_muse['address']
-            name = found_muse['name']
-        print('Connecting to %s : %s...' % (name if name else 'Muse', address))
-
-    if not filename:
-        filename = os.path.join(
-            os.getcwd(),
-            ("recording_%s.csv" % strftime("%Y-%m-%d-%H.%M.%S", gmtime())))
-
-    eeg_samples = []
-    timestamps = []
-
-    def save_eeg(new_samples, new_timestamps):
-        eeg_samples.append(new_samples)
-        timestamps.append(new_timestamps)
-
-    muse = Muse(address, save_eeg, backend=backend)
-    muse.connect()
-    muse.start()
-
-    t_init = time()
-    print('Start recording at time t=%.3f' % t_init)
-
-    while (time() - t_init) < duration:
-        try:
-            backends.sleep(1)
-        except KeyboardInterrupt:
-            break
-
-    muse.stop()
-    muse.disconnect()
-
-    timestamps = np.concatenate(timestamps)
-    eeg_samples = np.concatenate(eeg_samples, 1).T
-    recording = pd.DataFrame(
-        data=eeg_samples, columns=['TP9', 'AF7', 'AF8', 'TP10', 'Right AUX'])
-
-    recording['timestamps'] = timestamps
-
-    directory = os.path.dirname(filename)
-    if not os.path.exists(directory):
-        os.makedirs(directory)
-
-    recording.to_csv(filename, float_format='%.3f')
-    print('Done - wrote file: ' + filename + '.')
+import bleak
+import numpy as np
+import pandas as pd
+import os
+import sys
+from typing import Union, List, Optional
+from pathlib import Path
+from pylsl import StreamInlet, resolve_byprop
+from sklearn.linear_model import LinearRegression
+from time import time, strftime, gmtime
+from .stream import find_muse
+from . import backends
+from .muse import Muse
+from .constants import LSL_SCAN_TIMEOUT, LSL_EEG_CHUNK, LSL_PPG_CHUNK, LSL_ACC_CHUNK, LSL_GYRO_CHUNK
+
+# Records a fixed duration of EEG data from an LSL stream into a CSV file
+
+def record(
+    duration: int,
+    filename=None,
+    dejitter=False,
+    data_source="EEG",
+    continuous: bool = True,
+) -> None:
+    chunk_length = LSL_EEG_CHUNK
+    if data_source == "PPG":
+        chunk_length = LSL_PPG_CHUNK
+    if data_source == "ACC":
+        chunk_length = LSL_ACC_CHUNK
+    if data_source == "GYRO":
+        chunk_length = LSL_GYRO_CHUNK
+
+    if not filename:
+        filename = os.path.join(os.getcwd(), "%s_recording_%s.csv" %
+                                (data_source,
+                                 strftime('%Y-%m-%d-%H.%M.%S', gmtime())))
+
+    print("Looking for a %s stream..." % (data_source))
+    streams = resolve_byprop('type', data_source, timeout=LSL_SCAN_TIMEOUT)
+
+    if len(streams) == 0:
+        print("Can't find %s stream." % (data_source))
+        return
+
+    print("Started acquiring data.")
+    inlet = StreamInlet(streams[0], max_chunklen=chunk_length)
+    # eeg_time_correction = inlet.time_correction()
+
+    print("Looking for a Markers stream...")
+    marker_streams = resolve_byprop(
+        'name', 'Markers', timeout=LSL_SCAN_TIMEOUT)
+
+    if marker_streams:
+        inlet_marker = StreamInlet(marker_streams[0])
+    else:
+        inlet_marker = False
+        print("Can't find Markers stream.")
+
+    info = inlet.info()
+    description = info.desc()
+
+    Nchan = info.channel_count()
+
+    ch = description.child('channels').first_child()
+    ch_names = [ch.child_value('label')]
+    for i in range(1, Nchan):
+        ch = ch.next_sibling()
+        ch_names.append(ch.child_value('label'))
+
+    res = []
+    timestamps = []
+    markers = []
+    t_init = time()
+    time_correction = inlet.time_correction()
+    last_written_timestamp = None
+    print('Start recording at time t=%.3f' % t_init)
+    print('Time correction: ', time_correction)
+    while (time() - t_init) < duration:
+        try:
+            data, timestamp = inlet.pull_chunk(
+                timeout=1.0, max_samples=chunk_length)
+
+            if timestamp:
+                res.append(data)
+                timestamps.extend(timestamp)
+                tr = time()
+            if inlet_marker:
+                marker, timestamp = inlet_marker.pull_sample(timeout=0.0)
+                if timestamp:
+                    markers.append([marker, timestamp])
+
+            # Save every 5s
+            if continuous and (last_written_timestamp is None or last_written_timestamp + 5 < timestamps[-1]):
+                _save(
+                    filename,
+                    res,
+                    timestamps,
+                    time_correction,
+                    dejitter,
+                    inlet_marker,
+                    markers,
+                    ch_names,
+                    last_written_timestamp=last_written_timestamp,
+                )
+                last_written_timestamp = timestamps[-1]
+
+        except KeyboardInterrupt:
+            break
+
+    time_correction = inlet.time_correction()
+    print("Time correction: ", time_correction)
+
+    _save(
+        filename,
+        res,
+        timestamps,
+        time_correction,
+        dejitter,
+        inlet_marker,
+        markers,
+        ch_names,
+    )
+
+    print("Done - wrote file: {}".format(filename))
+
+
+def _save(
+    filename: Union[str, Path],
+    res: list,
+    timestamps: list,
+    time_correction,
+    dejitter: bool,
+    inlet_marker,
+    markers,
+    ch_names: List[str],
+    last_written_timestamp: Optional[float] = None,
+):
+    res = np.concatenate(res, axis=0)
+    timestamps = np.array(timestamps) + time_correction
+
+    if dejitter:
+        y = timestamps
+        X = np.atleast_2d(np.arange(0, len(y))).T
+        lr = LinearRegression()
+        lr.fit(X, y)
+        timestamps = lr.predict(X)
+
+    res = np.c_[timestamps, res]
+    data = pd.DataFrame(data=res, columns=["timestamps"] + ch_names)
+
+    directory = os.path.dirname(filename)
+    if not os.path.exists(directory):
+        os.makedirs(directory)
+
+    if inlet_marker and markers:
+        n_markers = len(markers[0][0])
+        for ii in range(n_markers):
+            data['Marker%d' % ii] = 0
+        # process markers:
+        for marker in markers:
+            # find index of markers
+            ix = np.argmin(np.abs(marker[1] - timestamps))
+            for ii in range(n_markers):
+                data.loc[ix, "Marker%d" % ii] = marker[0][ii]
+
+    # If file doesn't exist, create with headers
+    # If it does exist, just append new rows
+    if not Path(filename).exists():
+        # print("Saving whole file")
+        data.to_csv(filename, float_format='%.3f', index=False)
+    else:
+        # print("Appending file")
+        # truncate already written timestamps
+        data = data[data['timestamps'] > last_written_timestamp]
+        data.to_csv(filename, float_format='%.3f', index=False, mode='a', header=False)
+
+
+
+# Rercord directly from a Muse without the use of LSL
+
+
+def record_direct(duration,
+                  address,
+                  filename=None,
+                  backend='auto',
+                  interface=None,
+                  name=None):
+    if backend == 'bluemuse':
+        raise (NotImplementedError(
+            'Direct record not supported with BlueMuse backend. Use record after starting stream instead.'
+        ))
+
+    if not address:
+        found_muse = find_muse(name, backend)
+        if not found_muse:
+            print('Muse could not be found')
+            return
+        else:
+            address = found_muse['address']
+            name = found_muse['name']
+        print('Connecting to %s : %s...' % (name if name else 'Muse', address))
+
+    if not filename:
+        filename = os.path.join(
+            os.getcwd(),
+            ("recording_%s.csv" % strftime("%Y-%m-%d-%H.%M.%S", gmtime())))
+
+    eeg_samples = []
+    timestamps = []
+
+    def save_eeg(new_samples, new_timestamps):
+        eeg_samples.append(new_samples)
+        timestamps.append(new_timestamps)
+
+    muse = Muse(address, save_eeg, backend=backend)
+    if not muse.connect():
+        print(f'Failed to connect to Muse: {address}', file=sys.stderr)
+        return
+    muse.start()
+
+    t_init = time()
+    print('Start recording at time t=%.3f' % t_init)
+
+    last_update = t_init
+    while (time() - t_init) < duration:
+        try:
+            try:
+                backends.sleep(1)
+
+                # Send a keep alive every 10 secs
+                if time() - last_update > 10:
+                    last_update = time()
+                    muse.keep_alive()
+            except bleak.exc.BleakError:
+                print('Disconnected. Attempting to reconnect...')
+                # Do not giveup since we make a best effort to continue
+                # data collection. Assume device is out of range or another
+                # temp error.
+                while True:
+                    muse.connect(retries=-1)
+                    try:
+                        muse.resume()
+                    except bleak.exc.BleakDBusError:
+                        # Something is wrong with this connection
+                        print('DBus error occurred. Reconnecting.')
+                        muse.disconnect()
+                        continue
+                    else:
+                        break
+                print('Connected. Continuing with data collection...')
+        except KeyboardInterrupt:
+            print('Interrupt received. Exiting data collection.')
+            break
+
+    muse.stop()
+    muse.disconnect()
+
+    timestamps = np.concatenate(timestamps)
+    eeg_samples = np.concatenate(eeg_samples, 1).T
+    recording = pd.DataFrame(
+        data=eeg_samples, columns=['TP9', 'AF7', 'AF8', 'TP10', 'Right AUX'])
+
+    recording['timestamps'] = timestamps
+
+    directory = os.path.dirname(filename)
+    if not os.path.exists(directory):
+        os.makedirs(directory)
+
+    recording.to_csv(filename, float_format='%.3f')
+    print('Done - wrote file: ' + filename + '.')
```

### Comparing `muselsl-2.2.2/muselsl/viewer_v1.py` & `muselsl-2.3.0/muselsl/viewer_v1.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-import numpy as np
-import matplotlib
-from scipy.signal import lfilter, lfilter_zi, firwin
-from time import sleep
-from pylsl import StreamInlet, resolve_byprop
-import seaborn as sns
-from threading import Thread
-from .constants import VIEW_BUFFER, VIEW_SUBSAMPLE, LSL_SCAN_TIMEOUT, LSL_EEG_CHUNK
-
-
-def view(window, scale, refresh, figure, backend, version=1):
-    matplotlib.use(backend)
-    sns.set(style="whitegrid")
-
-    figsize = np.int16(figure.split('x'))
-
-    print("Looking for an EEG stream...")
-    streams = resolve_byprop('type', 'EEG', timeout=LSL_SCAN_TIMEOUT)
-
-    if len(streams) == 0:
-        raise(RuntimeError("Can't find EEG stream."))
-    print("Start acquiring data.")
-
-    fig, axes = matplotlib.pyplot.subplots(1, 1, figsize=figsize, sharex=True)
-    lslv = LSLViewer(streams[0], fig, axes, window, scale)
-    fig.canvas.mpl_connect('close_event', lslv.stop)
-
-    help_str = """
-                toggle filter : d
-                toogle full screen : f
-                zoom out : /
-                zoom in : *
-                increase time scale : -
-                decrease time scale : +
-               """
-    print(help_str)
-    lslv.start()
-    matplotlib.pyplot.show()
-
-
-class LSLViewer():
-    def __init__(self, stream, fig, axes, window, scale, dejitter=True):
-        """Init"""
-        self.stream = stream
-        self.window = window
-        self.scale = scale
-        self.dejitter = dejitter
-        self.inlet = StreamInlet(stream, max_chunklen=LSL_EEG_CHUNK)
-        self.filt = True
-        self.subsample = VIEW_SUBSAMPLE
-
-        info = self.inlet.info()
-        description = info.desc()
-
-        self.sfreq = info.nominal_srate()
-        self.n_samples = int(self.sfreq * self.window)
-        self.n_chan = info.channel_count()
-
-        ch = description.child('channels').first_child()
-        ch_names = [ch.child_value('label')]
-
-        for i in range(self.n_chan):
-            ch = ch.next_sibling()
-            ch_names.append(ch.child_value('label'))
-
-        self.ch_names = ch_names
-
-        fig.canvas.mpl_connect('key_press_event', self.OnKeypress)
-        fig.canvas.mpl_connect('button_press_event', self.onclick)
-
-        self.fig = fig
-        self.axes = axes
-
-        sns.despine(left=True)
-
-        self.data = np.zeros((self.n_samples, self.n_chan))
-        self.times = np.arange(-self.window, 0, 1. / self.sfreq)
-        impedances = np.std(self.data, axis=0)
-        lines = []
-
-        for ii in range(self.n_chan):
-            line, = axes.plot(self.times[::self.subsample],
-                              self.data[::self.subsample, ii] - ii, lw=1)
-            lines.append(line)
-        self.lines = lines
-
-        axes.set_ylim(-self.n_chan + 0.5, 0.5)
-        ticks = np.arange(0, -self.n_chan, -1)
-
-        axes.set_xlabel('Time (s)')
-        axes.xaxis.grid(False)
-        axes.set_yticks(ticks)
-
-        ticks_labels = ['%s - %.1f' % (ch_names[ii], impedances[ii])
-                        for ii in range(self.n_chan)]
-        axes.set_yticklabels(ticks_labels)
-
-        self.display_every = int(0.2 / (12 / self.sfreq))
-
-        self.bf = firwin(32, np.array([1, 40]) / (self.sfreq / 2.), width=0.05,
-                         pass_zero=False)
-        self.af = [1.0]
-
-        zi = lfilter_zi(self.bf, self.af)
-        self.filt_state = np.tile(zi, (self.n_chan, 1)).transpose()
-        self.data_f = np.zeros((self.n_samples, self.n_chan))
-
-    def update_plot(self):
-        k = 0
-        try:
-            while self.started:
-                samples, timestamps = self.inlet.pull_chunk(timeout=1.0,
-                                                            max_samples=LSL_EEG_CHUNK)
-
-                if timestamps:
-                    if self.dejitter:
-                        timestamps = np.float64(np.arange(len(timestamps)))
-                        timestamps /= self.sfreq
-                        timestamps += self.times[-1] + 1. / self.sfreq
-                    self.times = np.concatenate([self.times, timestamps])
-                    self.n_samples = int(self.sfreq * self.window)
-                    self.times = self.times[-self.n_samples:]
-                    self.data = np.vstack([self.data, samples])
-                    self.data = self.data[-self.n_samples:]
-                    filt_samples, self.filt_state = lfilter(
-                        self.bf, self.af,
-                        samples,
-                        axis=0, zi=self.filt_state)
-                    self.data_f = np.vstack([self.data_f, filt_samples])
-                    self.data_f = self.data_f[-self.n_samples:]
-                    k += 1
-                    if k == self.display_every:
-
-                        if self.filt:
-                            plot_data = self.data_f
-                        elif not self.filt:
-                            plot_data = self.data - self.data.mean(axis=0)
-                        for ii in range(self.n_chan):
-                            self.lines[ii].set_xdata(self.times[::self.subsample] -
-                                                     self.times[-1])
-                            self.lines[ii].set_ydata(plot_data[::self.subsample, ii] /
-                                                     self.scale - ii)
-                            impedances = np.std(plot_data, axis=0)
-
-                        ticks_labels = ['%s - %.2f' % (self.ch_names[ii],
-                                                       impedances[ii])
-                                        for ii in range(self.n_chan)]
-                        self.axes.set_yticklabels(ticks_labels)
-                        self.axes.set_xlim(-self.window, 0)
-                        self.fig.canvas.draw()
-                        k = 0
-                else:
-                    sleep(0.2)
-        except RuntimeError as e:
-            raise
-
-    def onclick(self, event):
-        print((event.button, event.x, event.y, event.xdata, event.ydata))
-
-    def OnKeypress(self, event):
-        if event.key == '/':
-            self.scale *= 1.2
-        elif event.key == '*':
-            self.scale /= 1.2
-        elif event.key == '+':
-            self.window += 1
-        elif event.key == '-':
-            if self.window > 1:
-                self.window -= 1
-        elif event.key == 'd':
-            self.filt = not(self.filt)
-
-    def start(self):
-        self.started = True
-        self.thread = Thread(target=self.update_plot)
-        self.thread.daemon = True
-        self.thread.start()
-
-    def stop(self, close_event):
-        self.started = False
+import numpy as np
+import matplotlib
+from scipy.signal import lfilter, lfilter_zi, firwin
+from time import sleep
+from pylsl import StreamInlet, resolve_byprop
+import seaborn as sns
+from threading import Thread
+from .constants import VIEW_BUFFER, VIEW_SUBSAMPLE, LSL_SCAN_TIMEOUT, LSL_EEG_CHUNK
+
+
+def view(window, scale, refresh, figure, backend, version=1):
+    matplotlib.use(backend)
+    sns.set(style="whitegrid")
+
+    figsize = np.int16(figure.split('x'))
+
+    print("Looking for an EEG stream...")
+    streams = resolve_byprop('type', 'EEG', timeout=LSL_SCAN_TIMEOUT)
+
+    if len(streams) == 0:
+        raise(RuntimeError("Can't find EEG stream."))
+    print("Start acquiring data.")
+
+    fig, axes = matplotlib.pyplot.subplots(1, 1, figsize=figsize, sharex=True)
+    lslv = LSLViewer(streams[0], fig, axes, window, scale)
+    fig.canvas.mpl_connect('close_event', lslv.stop)
+
+    help_str = """
+                toggle filter : d
+                toogle full screen : f
+                zoom out : /
+                zoom in : *
+                increase time scale : -
+                decrease time scale : +
+               """
+    print(help_str)
+    lslv.start()
+    matplotlib.pyplot.show()
+
+
+class LSLViewer():
+    def __init__(self, stream, fig, axes, window, scale, dejitter=True):
+        """Init"""
+        self.stream = stream
+        self.window = window
+        self.scale = scale
+        self.dejitter = dejitter
+        self.inlet = StreamInlet(stream, max_chunklen=LSL_EEG_CHUNK)
+        self.filt = True
+        self.subsample = VIEW_SUBSAMPLE
+
+        info = self.inlet.info()
+        description = info.desc()
+
+        self.sfreq = info.nominal_srate()
+        self.n_samples = int(self.sfreq * self.window)
+        self.n_chan = info.channel_count()
+
+        ch = description.child('channels').first_child()
+        ch_names = [ch.child_value('label')]
+
+        for i in range(self.n_chan):
+            ch = ch.next_sibling()
+            ch_names.append(ch.child_value('label'))
+
+        self.ch_names = ch_names
+
+        fig.canvas.mpl_connect('key_press_event', self.OnKeypress)
+        fig.canvas.mpl_connect('button_press_event', self.onclick)
+
+        self.fig = fig
+        self.axes = axes
+
+        sns.despine(left=True)
+
+        self.data = np.zeros((self.n_samples, self.n_chan))
+        self.times = np.arange(-self.window, 0, 1. / self.sfreq)
+        impedances = np.std(self.data, axis=0)
+        lines = []
+
+        for ii in range(self.n_chan):
+            line, = axes.plot(self.times[::self.subsample],
+                              self.data[::self.subsample, ii] - ii, lw=1)
+            lines.append(line)
+        self.lines = lines
+
+        axes.set_ylim(-self.n_chan + 0.5, 0.5)
+        ticks = np.arange(0, -self.n_chan, -1)
+
+        axes.set_xlabel('Time (s)')
+        axes.xaxis.grid(False)
+        axes.set_yticks(ticks)
+
+        ticks_labels = ['%s - %.1f' % (ch_names[ii], impedances[ii])
+                        for ii in range(self.n_chan)]
+        axes.set_yticklabels(ticks_labels)
+
+        self.display_every = int(0.2 / (12 / self.sfreq))
+
+        self.bf = firwin(32, np.array([1, 40]) / (self.sfreq / 2.), width=0.05,
+                         pass_zero=False)
+        self.af = [1.0]
+
+        zi = lfilter_zi(self.bf, self.af)
+        self.filt_state = np.tile(zi, (self.n_chan, 1)).transpose()
+        self.data_f = np.zeros((self.n_samples, self.n_chan))
+
+    def update_plot(self):
+        k = 0
+        try:
+            while self.started:
+                samples, timestamps = self.inlet.pull_chunk(timeout=1.0,
+                                                            max_samples=LSL_EEG_CHUNK)
+
+                if timestamps:
+                    if self.dejitter:
+                        timestamps = np.float64(np.arange(len(timestamps)))
+                        timestamps /= self.sfreq
+                        timestamps += self.times[-1] + 1. / self.sfreq
+                    self.times = np.concatenate([self.times, timestamps])
+                    self.n_samples = int(self.sfreq * self.window)
+                    self.times = self.times[-self.n_samples:]
+                    self.data = np.vstack([self.data, samples])
+                    self.data = self.data[-self.n_samples:]
+                    filt_samples, self.filt_state = lfilter(
+                        self.bf, self.af,
+                        samples,
+                        axis=0, zi=self.filt_state)
+                    self.data_f = np.vstack([self.data_f, filt_samples])
+                    self.data_f = self.data_f[-self.n_samples:]
+                    k += 1
+                    if k == self.display_every:
+
+                        if self.filt:
+                            plot_data = self.data_f
+                        elif not self.filt:
+                            plot_data = self.data - self.data.mean(axis=0)
+                        for ii in range(self.n_chan):
+                            self.lines[ii].set_xdata(self.times[::self.subsample] -
+                                                     self.times[-1])
+                            self.lines[ii].set_ydata(plot_data[::self.subsample, ii] /
+                                                     self.scale - ii)
+                            impedances = np.std(plot_data, axis=0)
+
+                        ticks_labels = ['%s - %.2f' % (self.ch_names[ii],
+                                                       impedances[ii])
+                                        for ii in range(self.n_chan)]
+                        self.axes.set_yticklabels(ticks_labels)
+                        self.axes.set_xlim(-self.window, 0)
+                        self.fig.canvas.draw()
+                        k = 0
+                else:
+                    sleep(0.2)
+        except RuntimeError as e:
+            raise
+
+    def onclick(self, event):
+        print((event.button, event.x, event.y, event.xdata, event.ydata))
+
+    def OnKeypress(self, event):
+        if event.key == '/':
+            self.scale *= 1.2
+        elif event.key == '*':
+            self.scale /= 1.2
+        elif event.key == '+':
+            self.window += 1
+        elif event.key == '-':
+            if self.window > 1:
+                self.window -= 1
+        elif event.key == 'd':
+            self.filt = not(self.filt)
+
+    def start(self):
+        self.started = True
+        self.thread = Thread(target=self.update_plot)
+        self.thread.daemon = True
+        self.thread.start()
+
+    def stop(self, close_event):
+        self.started = False
```

### Comparing `muselsl-2.2.2/muselsl/viewer_v2.py` & `muselsl-2.3.0/muselsl/viewer_v2.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,260 +1,260 @@
-# -*- coding: utf-8 -*-
-# vispy: gallery 2
-# Copyright (c) 2015, Vispy Development Team.
-# Distributed under the (new) BSD License. See LICENSE.txt for more info.
-
-"""
-Multiple real-time digital signals with GLSL-based clipping.
-"""
-
-from vispy import gloo, app, visuals
-
-import numpy as np
-import math
-from seaborn import color_palette
-from pylsl import StreamInlet, resolve_byprop
-from scipy.signal import lfilter, lfilter_zi
-from mne.filter import create_filter
-from .constants import LSL_SCAN_TIMEOUT, LSL_EEG_CHUNK
-
-
-VERT_SHADER = """
-#version 120
-// y coordinate of the position.
-attribute float a_position;
-// row, col, and time index.
-attribute vec3 a_index;
-varying vec3 v_index;
-// 2D scaling factor (zooming).
-uniform vec2 u_scale;
-// Size of the table.
-uniform vec2 u_size;
-// Number of samples per signal.
-uniform float u_n;
-// Color.
-attribute vec3 a_color;
-varying vec4 v_color;
-// Varying variables used for clipping in the fragment shader.
-varying vec2 v_position;
-varying vec4 v_ab;
-void main() {
-    float n_rows = u_size.x;
-    float n_cols = u_size.y;
-    // Compute the x coordinate from the time index.
-    float x = -1 + 2*a_index.z / (u_n-1);
-    vec2 position = vec2(x - (1 - 1 / u_scale.x), a_position);
-    // Find the affine transformation for the subplots.
-    vec2 a = vec2(1./n_cols, 1./n_rows)*.9;
-    vec2 b = vec2(-1 + 2*(a_index.x+.5) / n_cols,
-                    -1 + 2*(a_index.y+.5) / n_rows);
-    // Apply the static subplot transformation + scaling.
-    gl_Position = vec4(a*u_scale*position+b, 0.0, 1.0);
-    v_color = vec4(a_color, 1.);
-    v_index = a_index;
-    // For clipping test in the fragment shader.
-    v_position = gl_Position.xy;
-    v_ab = vec4(a, b);
-}
-"""
-
-FRAG_SHADER = """
-#version 120
-varying vec4 v_color;
-varying vec3 v_index;
-varying vec2 v_position;
-varying vec4 v_ab;
-void main() {
-    gl_FragColor = v_color;
-    // Discard the fragments between the signals (emulate glMultiDrawArrays).
-    if ((fract(v_index.x) > 0.) || (fract(v_index.y) > 0.))
-        discard;
-    // Clipping test.
-    vec2 test = abs((v_position.xy-v_ab.zw)/v_ab.xy);
-    if ((test.x > 1))
-        discard;
-}
-"""
-
-
-def view():
-    print("Looking for an EEG stream...")
-    streams = resolve_byprop('type', 'EEG', timeout=LSL_SCAN_TIMEOUT)
-
-    if len(streams) == 0:
-        raise(RuntimeError("Can't find EEG stream."))
-    print("Start acquiring data.")
-
-    inlet = StreamInlet(streams[0], max_chunklen=LSL_EEG_CHUNK)
-    Canvas(inlet)
-    app.run()
-
-
-class Canvas(app.Canvas):
-    def __init__(self, lsl_inlet, scale=500, filt=True):
-        app.Canvas.__init__(self, title='EEG - Use your wheel to zoom!',
-                            keys='interactive')
-
-        self.inlet = lsl_inlet
-        info = self.inlet.info()
-        description = info.desc()
-
-        window = 10
-        self.sfreq = info.nominal_srate()
-        n_samples = int(self.sfreq * window)
-        self.n_chans = info.channel_count()
-
-        ch = description.child('channels').first_child()
-        ch_names = [ch.child_value('label')]
-
-        for i in range(self.n_chans):
-            ch = ch.next_sibling()
-            ch_names.append(ch.child_value('label'))
-
-        # Number of cols and rows in the table.
-        n_rows = self.n_chans
-        n_cols = 1
-
-        # Number of signals.
-        m = n_rows * n_cols
-
-        # Number of samples per signal.
-        n = n_samples
-
-        # Various signal amplitudes.
-        amplitudes = np.zeros((m, n)).astype(np.float32)
-        # gamma = np.ones((m, n)).astype(np.float32)
-        # Generate the signals as a (m, n) array.
-        y = amplitudes
-
-        color = color_palette("RdBu_r", n_rows)
-
-        color = np.repeat(color, n, axis=0).astype(np.float32)
-        # Signal 2D index of each vertex (row and col) and x-index (sample index
-        # within each signal).
-        index = np.c_[np.repeat(np.repeat(np.arange(n_cols), n_rows), n),
-                      np.repeat(np.tile(np.arange(n_rows), n_cols), n),
-                      np.tile(np.arange(n), m)].astype(np.float32)
-
-        self.program = gloo.Program(VERT_SHADER, FRAG_SHADER)
-        self.program['a_position'] = y.reshape(-1, 1)
-        self.program['a_color'] = color
-        self.program['a_index'] = index
-        self.program['u_scale'] = (1., 1.)
-        self.program['u_size'] = (n_rows, n_cols)
-        self.program['u_n'] = n
-
-        # text
-        self.font_size = 48.
-        self.names = []
-        self.quality = []
-        for ii in range(self.n_chans):
-            text = visuals.TextVisual(ch_names[ii], bold=True, color='white')
-            self.names.append(text)
-            text = visuals.TextVisual('', bold=True, color='white')
-            self.quality.append(text)
-
-        self.quality_colors = color_palette("RdYlGn", 11)[::-1]
-
-        self.scale = scale
-        self.n_samples = n_samples
-        self.filt = filt
-        self.af = [1.0]
-
-        self.data_f = np.zeros((n_samples, self.n_chans))
-        self.data = np.zeros((n_samples, self.n_chans))
-
-        self.bf = create_filter(self.data_f.T, self.sfreq, 3, 40.,
-                                method='fir')
-
-        zi = lfilter_zi(self.bf, self.af)
-        self.filt_state = np.tile(zi, (self.n_chans, 1)).transpose()
-
-        self._timer = app.Timer('auto', connect=self.on_timer, start=True)
-        gloo.set_viewport(0, 0, *self.physical_size)
-        gloo.set_state(clear_color='black', blend=True,
-                       blend_func=('src_alpha', 'one_minus_src_alpha'))
-
-        self.show()
-
-    def on_key_press(self, event):
-
-        # toggle filtering
-        if event.key.name == 'D':
-            self.filt = not self.filt
-
-        # increase time scale
-        if event.key.name in ['+', '-']:
-            if event.key.name == '+':
-                dx = -0.05
-            else:
-                dx = 0.05
-            scale_x, scale_y = self.program['u_scale']
-            scale_x_new, scale_y_new = (scale_x * math.exp(1.0 * dx),
-                                        scale_y * math.exp(0.0 * dx))
-            self.program['u_scale'] = (
-                max(1, scale_x_new), max(1, scale_y_new))
-            self.update()
-
-    def on_mouse_wheel(self, event):
-        dx = np.sign(event.delta[1]) * .05
-        scale_x, scale_y = self.program['u_scale']
-        scale_x_new, scale_y_new = (scale_x * math.exp(0.0 * dx),
-                                    scale_y * math.exp(2.0 * dx))
-        self.program['u_scale'] = (max(1, scale_x_new), max(0.01, scale_y_new))
-        self.update()
-
-    def on_timer(self, event):
-        """Add some data at the end of each signal (real-time signals)."""
-
-        samples, timestamps = self.inlet.pull_chunk(timeout=0.0,
-                                                    max_samples=100)
-        if timestamps:
-            samples = np.array(samples)[:, ::-1]
-
-            self.data = np.vstack([self.data, samples])
-            self.data = self.data[-self.n_samples:]
-            filt_samples, self.filt_state = lfilter(self.bf, self.af, samples,
-                                                    axis=0, zi=self.filt_state)
-            self.data_f = np.vstack([self.data_f, filt_samples])
-            self.data_f = self.data_f[-self.n_samples:]
-
-            if self.filt:
-                plot_data = self.data_f / self.scale
-            elif not self.filt:
-                plot_data = (self.data - self.data.mean(axis=0)) / self.scale
-
-            sd = np.std(plot_data[-int(self.sfreq):],
-                        axis=0)[::-1] * self.scale
-            co = np.int32(np.tanh((sd - 30) / 15) * 5 + 5)
-            for ii in range(self.n_chans):
-                self.quality[ii].text = '%.2f' % (sd[ii])
-                self.quality[ii].color = self.quality_colors[co[ii]]
-                self.quality[ii].font_size = 12 + co[ii]
-
-                self.names[ii].font_size = 12 + co[ii]
-                self.names[ii].color = self.quality_colors[co[ii]]
-
-            self.program['a_position'].set_data(
-                plot_data.T.ravel().astype(np.float32))
-            self.update()
-
-    def on_resize(self, event):
-        # Set canvas viewport and reconfigure visual transforms to match.
-        vp = (0, 0, self.physical_size[0], self.physical_size[1])
-        self.context.set_viewport(*vp)
-
-        for ii, t in enumerate(self.names):
-            t.transforms.configure(canvas=self, viewport=vp)
-            t.pos = (self.size[0] * 0.025,
-                     ((ii + 0.5) / self.n_chans) * self.size[1])
-
-        for ii, t in enumerate(self.quality):
-            t.transforms.configure(canvas=self, viewport=vp)
-            t.pos = (self.size[0] * 0.975,
-                     ((ii + 0.5) / self.n_chans) * self.size[1])
-
-    def on_draw(self, event):
-        gloo.clear()
-        gloo.set_viewport(0, 0, *self.physical_size)
-        self.program.draw('line_strip')
-        [t.draw() for t in self.names + self.quality]
+# -*- coding: utf-8 -*-
+# vispy: gallery 2
+# Copyright (c) 2015, Vispy Development Team.
+# Distributed under the (new) BSD License. See LICENSE.txt for more info.
+
+"""
+Multiple real-time digital signals with GLSL-based clipping.
+"""
+
+from vispy import gloo, app, visuals
+
+import numpy as np
+import math
+from seaborn import color_palette
+from pylsl import StreamInlet, resolve_byprop
+from scipy.signal import lfilter, lfilter_zi
+from mne.filter import create_filter
+from .constants import LSL_SCAN_TIMEOUT, LSL_EEG_CHUNK
+
+
+VERT_SHADER = """
+#version 120
+// y coordinate of the position.
+attribute float a_position;
+// row, col, and time index.
+attribute vec3 a_index;
+varying vec3 v_index;
+// 2D scaling factor (zooming).
+uniform vec2 u_scale;
+// Size of the table.
+uniform vec2 u_size;
+// Number of samples per signal.
+uniform float u_n;
+// Color.
+attribute vec3 a_color;
+varying vec4 v_color;
+// Varying variables used for clipping in the fragment shader.
+varying vec2 v_position;
+varying vec4 v_ab;
+void main() {
+    float n_rows = u_size.x;
+    float n_cols = u_size.y;
+    // Compute the x coordinate from the time index.
+    float x = -1 + 2*a_index.z / (u_n-1);
+    vec2 position = vec2(x - (1 - 1 / u_scale.x), a_position);
+    // Find the affine transformation for the subplots.
+    vec2 a = vec2(1./n_cols, 1./n_rows)*.9;
+    vec2 b = vec2(-1 + 2*(a_index.x+.5) / n_cols,
+                    -1 + 2*(a_index.y+.5) / n_rows);
+    // Apply the static subplot transformation + scaling.
+    gl_Position = vec4(a*u_scale*position+b, 0.0, 1.0);
+    v_color = vec4(a_color, 1.);
+    v_index = a_index;
+    // For clipping test in the fragment shader.
+    v_position = gl_Position.xy;
+    v_ab = vec4(a, b);
+}
+"""
+
+FRAG_SHADER = """
+#version 120
+varying vec4 v_color;
+varying vec3 v_index;
+varying vec2 v_position;
+varying vec4 v_ab;
+void main() {
+    gl_FragColor = v_color;
+    // Discard the fragments between the signals (emulate glMultiDrawArrays).
+    if ((fract(v_index.x) > 0.) || (fract(v_index.y) > 0.))
+        discard;
+    // Clipping test.
+    vec2 test = abs((v_position.xy-v_ab.zw)/v_ab.xy);
+    if ((test.x > 1))
+        discard;
+}
+"""
+
+
+def view():
+    print("Looking for an EEG stream...")
+    streams = resolve_byprop('type', 'EEG', timeout=LSL_SCAN_TIMEOUT)
+
+    if len(streams) == 0:
+        raise(RuntimeError("Can't find EEG stream."))
+    print("Start acquiring data.")
+
+    inlet = StreamInlet(streams[0], max_chunklen=LSL_EEG_CHUNK)
+    Canvas(inlet)
+    app.run()
+
+
+class Canvas(app.Canvas):
+    def __init__(self, lsl_inlet, scale=500, filt=True):
+        app.Canvas.__init__(self, title='EEG - Use your wheel to zoom!',
+                            keys='interactive')
+
+        self.inlet = lsl_inlet
+        info = self.inlet.info()
+        description = info.desc()
+
+        window = 10
+        self.sfreq = info.nominal_srate()
+        n_samples = int(self.sfreq * window)
+        self.n_chans = info.channel_count()
+
+        ch = description.child('channels').first_child()
+        ch_names = [ch.child_value('label')]
+
+        for i in range(self.n_chans):
+            ch = ch.next_sibling()
+            ch_names.append(ch.child_value('label'))
+
+        # Number of cols and rows in the table.
+        n_rows = self.n_chans
+        n_cols = 1
+
+        # Number of signals.
+        m = n_rows * n_cols
+
+        # Number of samples per signal.
+        n = n_samples
+
+        # Various signal amplitudes.
+        amplitudes = np.zeros((m, n)).astype(np.float32)
+        # gamma = np.ones((m, n)).astype(np.float32)
+        # Generate the signals as a (m, n) array.
+        y = amplitudes
+
+        color = color_palette("RdBu_r", n_rows)
+
+        color = np.repeat(color, n, axis=0).astype(np.float32)
+        # Signal 2D index of each vertex (row and col) and x-index (sample index
+        # within each signal).
+        index = np.c_[np.repeat(np.repeat(np.arange(n_cols), n_rows), n),
+                      np.repeat(np.tile(np.arange(n_rows), n_cols), n),
+                      np.tile(np.arange(n), m)].astype(np.float32)
+
+        self.program = gloo.Program(VERT_SHADER, FRAG_SHADER)
+        self.program['a_position'] = y.reshape(-1, 1)
+        self.program['a_color'] = color
+        self.program['a_index'] = index
+        self.program['u_scale'] = (1., 1.)
+        self.program['u_size'] = (n_rows, n_cols)
+        self.program['u_n'] = n
+
+        # text
+        self.font_size = 48.
+        self.names = []
+        self.quality = []
+        for ii in range(self.n_chans):
+            text = visuals.TextVisual(ch_names[ii], bold=True, color='white')
+            self.names.append(text)
+            text = visuals.TextVisual('', bold=True, color='white')
+            self.quality.append(text)
+
+        self.quality_colors = color_palette("RdYlGn", 11)[::-1]
+
+        self.scale = scale
+        self.n_samples = n_samples
+        self.filt = filt
+        self.af = [1.0]
+
+        self.data_f = np.zeros((n_samples, self.n_chans))
+        self.data = np.zeros((n_samples, self.n_chans))
+
+        self.bf = create_filter(self.data_f.T, self.sfreq, 3, 40.,
+                                method='fir')
+
+        zi = lfilter_zi(self.bf, self.af)
+        self.filt_state = np.tile(zi, (self.n_chans, 1)).transpose()
+
+        self._timer = app.Timer('auto', connect=self.on_timer, start=True)
+        gloo.set_viewport(0, 0, *self.physical_size)
+        gloo.set_state(clear_color='black', blend=True,
+                       blend_func=('src_alpha', 'one_minus_src_alpha'))
+
+        self.show()
+
+    def on_key_press(self, event):
+
+        # toggle filtering
+        if event.key.name == 'D':
+            self.filt = not self.filt
+
+        # increase time scale
+        if event.key.name in ['+', '-']:
+            if event.key.name == '+':
+                dx = -0.05
+            else:
+                dx = 0.05
+            scale_x, scale_y = self.program['u_scale']
+            scale_x_new, scale_y_new = (scale_x * math.exp(1.0 * dx),
+                                        scale_y * math.exp(0.0 * dx))
+            self.program['u_scale'] = (
+                max(1, scale_x_new), max(1, scale_y_new))
+            self.update()
+
+    def on_mouse_wheel(self, event):
+        dx = np.sign(event.delta[1]) * .05
+        scale_x, scale_y = self.program['u_scale']
+        scale_x_new, scale_y_new = (scale_x * math.exp(0.0 * dx),
+                                    scale_y * math.exp(2.0 * dx))
+        self.program['u_scale'] = (max(1, scale_x_new), max(0.01, scale_y_new))
+        self.update()
+
+    def on_timer(self, event):
+        """Add some data at the end of each signal (real-time signals)."""
+
+        samples, timestamps = self.inlet.pull_chunk(timeout=0.0,
+                                                    max_samples=100)
+        if timestamps:
+            samples = np.array(samples)[:, ::-1]
+
+            self.data = np.vstack([self.data, samples])
+            self.data = self.data[-self.n_samples:]
+            filt_samples, self.filt_state = lfilter(self.bf, self.af, samples,
+                                                    axis=0, zi=self.filt_state)
+            self.data_f = np.vstack([self.data_f, filt_samples])
+            self.data_f = self.data_f[-self.n_samples:]
+
+            if self.filt:
+                plot_data = self.data_f / self.scale
+            elif not self.filt:
+                plot_data = (self.data - self.data.mean(axis=0)) / self.scale
+
+            sd = np.std(plot_data[-int(self.sfreq):],
+                        axis=0)[::-1] * self.scale
+            co = np.int32(np.tanh((sd - 30) / 15) * 5 + 5)
+            for ii in range(self.n_chans):
+                self.quality[ii].text = '%.2f' % (sd[ii])
+                self.quality[ii].color = self.quality_colors[co[ii]]
+                self.quality[ii].font_size = 12 + co[ii]
+
+                self.names[ii].font_size = 12 + co[ii]
+                self.names[ii].color = self.quality_colors[co[ii]]
+
+            self.program['a_position'].set_data(
+                plot_data.T.ravel().astype(np.float32))
+            self.update()
+
+    def on_resize(self, event):
+        # Set canvas viewport and reconfigure visual transforms to match.
+        vp = (0, 0, self.physical_size[0], self.physical_size[1])
+        self.context.set_viewport(*vp)
+
+        for ii, t in enumerate(self.names):
+            t.transforms.configure(canvas=self, viewport=vp)
+            t.pos = (self.size[0] * 0.025,
+                     ((ii + 0.5) / self.n_chans) * self.size[1])
+
+        for ii, t in enumerate(self.quality):
+            t.transforms.configure(canvas=self, viewport=vp)
+            t.pos = (self.size[0] * 0.975,
+                     ((ii + 0.5) / self.n_chans) * self.size[1])
+
+    def on_draw(self, event):
+        gloo.clear()
+        gloo.set_viewport(0, 0, *self.physical_size)
+        self.program.draw('line_strip')
+        [t.draw() for t in self.names + self.quality]
```

### Comparing `muselsl-2.2.2/muselsl.egg-info/PKG-INFO` & `muselsl-2.3.0/muselsl.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,193 +1,204 @@
-Metadata-Version: 2.1
-Name: muselsl
-Version: 2.2.2
-Summary: Stream and visualize EEG data from the Muse headset.
-Home-page: https://github.com/alexandrebarachant/muse-lsl/
-Author: Alexandre Barachant
-Author-email: alexandre.barachant@gmail.com
-License: BSD (3-clause)
-Keywords: muse lsl eeg ble neuroscience
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Software Development
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown
-Provides-Extra: Viewer V2
-License-File: LICENSE.txt
-
-
-[![DOI](https://zenodo.org/badge/80209610.svg)](https://zenodo.org/badge/latestdoi/80209610)
-
-# Muse LSL
-
-A Python package for streaming, visualizing, and recording EEG data from the Muse devices developed by InteraXon.
-
-![Blinks](blinks.png)
-
-## Requirements
-
-The code relies on a number of different bluetooth backends for connecting to the muse. We recommend using the `bleak` backend (enabled by default), but you may be interested in [BlueMuse](https://github.com/kowalej/BlueMuse/tree/master/Dist) for a GUI to discover and connect to Muse devices on Windows or [bgapi] if you are on a Mac with a BLED112 dongle. 
-
-**Compatible with Python 2.7 and Python 3.x**
-
-**Compatible with Muse 2, Muse S, and the classic Muse (2016)**
-
-_Note: if you run into any issues, first check out out [Common Issues](#common-issues) and then the [Issues](https://github.com/alexandrebarachant/muse-lsl/issues) section of this repository_
-
-## Getting Started
-
-### Installation
-
-Install Muse LSL with pip
-
-    pip install muselsl
-
-### Setting Up a Stream
-
-On Windows 10, we recommend using the [BlueMuse](https://github.com/kowalej/BlueMuse/tree/master/Dist) GUI to set up an LSL stream. On Mac and Linux, the easiest way to get Muse data is to use Muse LSL directly from the command line. Use the `-h` flag to get a comprehensive list of all commands and options.
-
-To print a list of available muses:
-
-    $ muselsl list
-
-To begin an LSL stream from the first available Muse:
-
-    $ muselsl stream  
-
-To connect to a specific Muse you can pass the name of the device as an argument. Device names can be found on the inside of the left earpiece (e.g. Muse-41D2):
-
-    $ muselsl stream --name YOUR_DEVICE_NAME
-
-You can also directly pass the MAC address of your Muse. This provides the benefit of bypassing the device discovery step and can make connecting to devices quicker and more reliable:
-
-    $ muselsl stream --address YOUR_DEVICE_ADDRESS
-
-### Working with Streaming Data
-
-Once an LSL stream is created, you have access to the following commands.
-
-*Note: the process running the `stream` command must be kept alive in order to maintain the LSL stream. These following commands should be run in another terminal or second process*
-
-To view data:
-
-    $ muselsl view
-
-If the visualization freezes or is laggy, you can also try the alternate version 2 of the viewer. *Note: this will require the additional [vispy](https://github.com/vispy/vispy) and [mne](https://github.com/mne-tools/mne-python) dependencies*
-
-    $ muselsl view --version 2
-
-To record EEG data into a CSV:
-
-    $ muselsl record --duration 60  
-
-*Note: this command will also save data from any LSL stream containing 'Markers' data, such as from the stimulus presentation scripts in [EEG Notebooks](https://github.com/neurotechx/eeg-notebooks)*
-
-Alternatively, you can record data directly without using LSL through the following command:
-
-    $ muselsl record_direct --duration 60
-
-_Note: direct recording does not allow 'Markers' data to be recorded_
-
-## Running Experiments
-
-Muse LSL was designed so that the Muse could be used to run a number of classic EEG experiments, including the [P300 event-related potential](http://alexandre.barachant.org/blog/2017/02/05/P300-with-muse.html) and the SSVEP and SSAEP evoked potentials.
-
-The code to perform these experiments is still available, but is now maintained in the [EEG Notebooks](https://github.com/neurotechx/eeg-notebooks) repository by the [NeuroTechX](https://neurotechx.com) community.
-
-## Usage as a Library
-
-If you want to integrate Muse LSL into your own Python project, you can import and use its functions as you would any Python library. Examples are available in the `examples` folder:
-
-```Python
-from muselsl import stream, list_muses
-
-muses = list_muses()
-stream(muses[0]['address'])
-
-# Note: Streaming is synchronous, so code here will not execute until after the stream has been closed
-print('Stream has ended')
-```
-
-## Alternate Data Types
-
-In addition to EEG, the Muse also provides data from an accelerometer, gyroscope, and, in the case of the Muse 2, a photoplethysmography (PPG) sensor. These data types can be enabled via command line arguments or by passing the correct parameters to the `stream` function. Once enabled, PPG, accelerometer, and gyroscope data will streamed in their own separate LSL streams named "PPG", "ACC", and "GYRO", respectively.
-
-To stream data from all sensors in a Muse 2 from the command line:
-
-    muselsl stream --ppg --acc --gyro
-
-As a library function:
-
-```Python
-from muselsl import stream, list_muses
-
-muses = list_muses()
-stream(muses[0]['address'], ppg_enabled=True, acc_enabled=True, gyro_enabled=True)
-```
-
-To record data from an alternate data source:
-
-    muselsl record --type ACC
-
-*Note: The record process will only record from one data type at a time. However, multiple terminals or processes can be used to record from multiple data types simultaneously*
-
-## What is LSL?
-
-Lab Streaming Layer or LSL is a system designed to unify the collection of time series data for research experiments. It has become standard in the field of EEG-based brain-computer interfaces for its ability to make seperate streams of data available on a network with time synchronization and near real-time access. For more information, check out this [lecture from Modern Brain-Computer Interface Design](https://www.youtube.com/watch?v=Y1at7yrcFW0) or the [LSL repository](https://github.com/sccn/labstreaminglayer)
-
-## Common Issues
-
-### Mac and Windows
-
-1.  Connection issues with BLED112 dongle:
-
-- You may need to use the `--interface` argument to provide the appropriate COM port value for the BLED112 device. The default value is COM9. To setup or view the device's COM port go to your OS's system settings
-
-### Linux
-
-1.  `pygatt.exceptions.BLEError: Unexpected error when scanning: Set scan parameters failed: Operation not permitted` (Linux)
-
-- This is an issue with pygatt requiring root privileges to run a scan. Make sure you [have `libcap` installed](https://askubuntu.com/questions/347788/how-can-i-install-libpcap-header-files-on-ubuntu-12-04) and run `` sudo setcap 'cap_net_raw,cap_net_admin+eip' `which hcitool` ``
-
-2.  `pygatt.exceptions.BLEError: No characteristic found matching 273e0003-4c4d-454d-96be-f03bac821358` (Linux)
-
-- There is a problem with the most recent version of pygatt. Work around this by downgrading to 3.1.1: `pip install pygatt==3.1.1`
-
-3.  `pygatt.exceptions.BLEError: No BLE adapter found` (Linux)
-
-- Make sure your computer's Bluetooth is turned on.
-
-4.  `pygatt.exceptions.BLEError: Unexpected error when scanning: Set scan parameters failed: Connection timed out` (Linux)
-
-- This seems to be due to a OS-level Bluetooth crash. Try turning your computer's bluetooth off and on again
-
-5.  `'RuntimeError: could not create stream outlet'` (Linux)
-
-- This appears to be due to Linux-specific issues with the newest version of pylsl. Ensure that you have pylsl 1.10.5 installed in the environment in which you are trying to run Muse LSL
-- If this is preceded by `Could not instantiate IPv4 stack: getrandom`, it could be [this issue](https://github.com/boostorg/uuid/issues/91) which can be resolved by building `liblsl` with `-DBOOST_UUID_RANDOM_PROVIDER_FORCE_POSIX` (e.g. by editing `standalone_compilation_linux.sh`)
-
-## Citing muse-lsl
-
-```
-@misc{muse-lsl,
-  author       = {Alexandre Barachant and
-                  Dano Morrison and
-                  Hubert Banville and
-                  Jason Kowaleski and
-                  Uri Shaked and
-                  Sylvain Chevallier and
-                  Juan JesÃºs Torre Tresols},
-  title        = {muse-lsl},
-  month        = may,
-  year         = 2019,
-  doi          = {10.5281/zenodo.3228861},
-  url          = {https://doi.org/10.5281/zenodo.3228861}
-}
-```
-
-> Alexandre Barachant, Dano Morrison, Hubert Banville, Jason Kowaleski, Uri Shaked, Sylvain Chevallier, & Juan JesÃºs Torre Tresols. (2019, May 25). muse-lsl (Version v2.0.2). Zenodo. http://doi.org/10.5281/zenodo.3228861
+Metadata-Version: 2.1
+Name: muselsl
+Version: 2.3.0
+Summary: Stream and visualize EEG data from the Muse headset.
+Home-page: https://github.com/alexandrebarachant/muse-lsl/
+Author: Alexandre Barachant
+Author-email: alexandre.barachant@gmail.com
+License: BSD (3-clause)
+Keywords: muse lsl eeg ble neuroscience
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Software Development
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: bitstring
+Requires-Dist: bleak>=0.18.0
+Requires-Dist: pygatt
+Requires-Dist: pandas
+Requires-Dist: scikit-learn
+Requires-Dist: numpy
+Requires-Dist: seaborn
+Requires-Dist: pexpect
+Requires-Dist: pylsl
+Provides-Extra: viewer-v2
+Requires-Dist: mne; extra == "viewer-v2"
+Requires-Dist: vispy; extra == "viewer-v2"
+
+
+[![DOI](https://zenodo.org/badge/80209610.svg)](https://zenodo.org/badge/latestdoi/80209610)
+
+# Muse LSL
+
+A Python package for streaming, visualizing, and recording EEG data from the Muse devices developed by InteraXon.
+
+![Blinks](blinks.png)
+
+## Requirements
+
+The code relies on a number of different bluetooth backends for connecting to the muse. We recommend using the `bleak` backend (enabled by default), but you may be interested in [BlueMuse](https://github.com/kowalej/BlueMuse/tree/master/Dist) for a GUI to discover and connect to Muse devices on Windows or [bgapi] if you are on a Mac with a BLED112 dongle. 
+
+**Compatible with Python 2.7 and Python 3.x**
+
+**Compatible with Muse 2, Muse S, and the classic Muse (2016)**
+
+_Note: if you run into any issues, first check out out [Common Issues](#common-issues) and then the [Issues](https://github.com/alexandrebarachant/muse-lsl/issues) section of this repository_
+
+## Getting Started
+
+### Installation
+
+Install Muse LSL with pip
+
+    pip install muselsl
+
+### Setting Up a Stream
+
+On Windows 10, we recommend using the [BlueMuse](https://github.com/kowalej/BlueMuse/tree/master/Dist) GUI to set up an LSL stream. On Mac and Linux, the easiest way to get Muse data is to use Muse LSL directly from the command line. Use the `-h` flag to get a comprehensive list of all commands and options.
+
+To print a list of available muses:
+
+    $ muselsl list
+
+To begin an LSL stream from the first available Muse:
+
+    $ muselsl stream  
+
+To connect to a specific Muse you can pass the name of the device as an argument. Device names can be found on the inside of the left earpiece (e.g. Muse-41D2):
+
+    $ muselsl stream --name YOUR_DEVICE_NAME
+
+You can also directly pass the MAC address of your Muse. This provides the benefit of bypassing the device discovery step and can make connecting to devices quicker and more reliable:
+
+    $ muselsl stream --address YOUR_DEVICE_ADDRESS
+
+### Working with Streaming Data
+
+Once an LSL stream is created, you have access to the following commands.
+
+*Note: the process running the `stream` command must be kept alive in order to maintain the LSL stream. These following commands should be run in another terminal or second process*
+
+To view data:
+
+    $ muselsl view
+
+If the visualization freezes or is laggy, you can also try the alternate version 2 of the viewer. *Note: this will require the additional [vispy](https://github.com/vispy/vispy) and [mne](https://github.com/mne-tools/mne-python) dependencies*
+
+    $ muselsl view --version 2
+
+To record EEG data into a CSV:
+
+    $ muselsl record --duration 60  
+
+*Note: this command will also save data from any LSL stream containing 'Markers' data, such as from the stimulus presentation scripts in [EEG Notebooks](https://github.com/neurotechx/eeg-notebooks)*
+
+Alternatively, you can record data directly without using LSL through the following command:
+
+    $ muselsl record_direct --duration 60
+
+_Note: direct recording does not allow 'Markers' data to be recorded_
+
+## Running Experiments
+
+Muse LSL was designed so that the Muse could be used to run a number of classic EEG experiments, including the [P300 event-related potential](http://alexandre.barachant.org/blog/2017/02/05/P300-with-muse.html) and the SSVEP and SSAEP evoked potentials.
+
+The code to perform these experiments is still available, but is now maintained in the [EEG Notebooks](https://github.com/neurotechx/eeg-notebooks) repository by the [NeuroTechX](https://neurotechx.com) community.
+
+## Usage as a Library
+
+If you want to integrate Muse LSL into your own Python project, you can import and use its functions as you would any Python library. Examples are available in the `examples` folder:
+
+```Python
+from muselsl import stream, list_muses
+
+muses = list_muses()
+stream(muses[0]['address'])
+
+# Note: Streaming is synchronous, so code here will not execute until after the stream has been closed
+print('Stream has ended')
+```
+
+## Alternate Data Types
+
+In addition to EEG, the Muse also provides data from an accelerometer, gyroscope, and, in the case of the Muse 2, a photoplethysmography (PPG) sensor. These data types can be enabled via command line arguments or by passing the correct parameters to the `stream` function. Once enabled, PPG, accelerometer, and gyroscope data will streamed in their own separate LSL streams named "PPG", "ACC", and "GYRO", respectively.
+
+To stream data from all sensors in a Muse 2 from the command line:
+
+    muselsl stream --ppg --acc --gyro
+
+As a library function:
+
+```Python
+from muselsl import stream, list_muses
+
+muses = list_muses()
+stream(muses[0]['address'], ppg_enabled=True, acc_enabled=True, gyro_enabled=True)
+```
+
+To record data from an alternate data source:
+
+    muselsl record --type ACC
+
+*Note: The record process will only record from one data type at a time. However, multiple terminals or processes can be used to record from multiple data types simultaneously*
+
+## What is LSL?
+
+Lab Streaming Layer or LSL is a system designed to unify the collection of time series data for research experiments. It has become standard in the field of EEG-based brain-computer interfaces for its ability to make seperate streams of data available on a network with time synchronization and near real-time access. For more information, check out this [lecture from Modern Brain-Computer Interface Design](https://www.youtube.com/watch?v=Y1at7yrcFW0) or the [LSL repository](https://github.com/sccn/labstreaminglayer)
+
+## Common Issues
+
+### Mac and Windows
+
+1.  Connection issues with BLED112 dongle:
+
+- You may need to use the `--interface` argument to provide the appropriate COM port value for the BLED112 device. The default value is COM9. To setup or view the device's COM port go to your OS's system settings
+
+### Linux
+
+1.  `pygatt.exceptions.BLEError: Unexpected error when scanning: Set scan parameters failed: Operation not permitted` (Linux)
+
+- This is an issue with pygatt requiring root privileges to run a scan. Make sure you [have `libcap` installed](https://askubuntu.com/questions/347788/how-can-i-install-libpcap-header-files-on-ubuntu-12-04) and run `` sudo setcap 'cap_net_raw,cap_net_admin+eip' `which hcitool` ``
+
+2.  `pygatt.exceptions.BLEError: No characteristic found matching 273e0003-4c4d-454d-96be-f03bac821358` (Linux)
+
+- There is a problem with the most recent version of pygatt. Work around this by downgrading to 3.1.1: `pip install pygatt==3.1.1`
+
+3.  `pygatt.exceptions.BLEError: No BLE adapter found` (Linux)
+
+- Make sure your computer's Bluetooth is turned on.
+
+4.  `pygatt.exceptions.BLEError: Unexpected error when scanning: Set scan parameters failed: Connection timed out` (Linux)
+
+- This seems to be due to a OS-level Bluetooth crash. Try turning your computer's bluetooth off and on again
+
+5.  `'RuntimeError: could not create stream outlet'` (Linux)
+
+- This appears to be due to Linux-specific issues with the newest version of pylsl. Ensure that you have pylsl 1.10.5 installed in the environment in which you are trying to run Muse LSL
+- If this is preceded by `Could not instantiate IPv4 stack: getrandom`, it could be [this issue](https://github.com/boostorg/uuid/issues/91) which can be resolved by building `liblsl` with `-DBOOST_UUID_RANDOM_PROVIDER_FORCE_POSIX` (e.g. by editing `standalone_compilation_linux.sh`)
+
+## Citing muse-lsl
+
+```
+@misc{muse-lsl,
+  author       = {Alexandre Barachant and
+                  Dano Morrison and
+                  Hubert Banville and
+                  Jason Kowaleski and
+                  Uri Shaked and
+                  Sylvain Chevallier and
+                  Juan Jesús Torre Tresols},
+  title        = {muse-lsl},
+  month        = may,
+  year         = 2019,
+  doi          = {10.5281/zenodo.3228861},
+  url          = {https://doi.org/10.5281/zenodo.3228861}
+}
+```
+
+> Alexandre Barachant, Dano Morrison, Hubert Banville, Jason Kowaleski, Uri Shaked, Sylvain Chevallier, & Juan Jesús Torre Tresols. (2019, May 25). muse-lsl (Version v2.0.2). Zenodo. http://doi.org/10.5281/zenodo.3228861
```

### Comparing `muselsl-2.2.2/muselsl.egg-info/SOURCES.txt` & `muselsl-2.3.0/muselsl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

