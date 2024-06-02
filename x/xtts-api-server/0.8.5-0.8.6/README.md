# Comparing `tmp/xtts_api_server-0.8.5.tar.gz` & `tmp/xtts_api_server-0.8.6.tar.gz`

## Comparing `xtts_api_server-0.8.5.tar` & `xtts_api_server-0.8.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/XTTS-api-server.ipynb
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/requirements.txt
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/.github/workflows/build-image.yml
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/docker/.dockerignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/docker/.env
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/docker/Dockerfile
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/docker/docker-compose.yml
--rw-r--r--   0        0        0   404742 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/example/calm_female.wav
--rw-r--r--   0        0        0  1002030 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/example/female.wav
--rw-r--r--   0        0        0   762126 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/example/male.wav
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/xtts_api_server/__init__.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/xtts_api_server/__main__.py
--rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/xtts_api_server/modeldownloader.py
--rw-r--r--   0        0        0    12594 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/xtts_api_server/server.py
--rw-r--r--   0        0        0    23940 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/xtts_api_server/tts_funcs.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/README.MD
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/__init__.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/coqui_test.py
--rw-r--r--   0        0        0   371026 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/silence.wav
--rw-r--r--   0        0        0     9293 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/stream_player.py
--rw-r--r--   0        0        0    26015 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/text_to_stream.py
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/threadsafe_generators.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/engines/__init__.py
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/engines/base_engine.py
--rw-r--r--   0        0        0   505425 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/engines/coqui_default_voice.json
--rw-r--r--   0        0        0    29386 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/engines/coqui_engine.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/LICENSE
--rw-r--r--   0        0        0    10049 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/README.md
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/pyproject.toml
--rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 xtts_api_server-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/XTTS-api-server.ipynb
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/requirements.txt
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/.github/workflows/build-image.yml
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/docker/.dockerignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/docker/.env
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/docker/Dockerfile
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/docker/docker-compose.yml
+-rw-r--r--   0        0        0   404742 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/example/calm_female.wav
+-rw-r--r--   0        0        0  1002030 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/example/female.wav
+-rw-r--r--   0        0        0   762126 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/example/male.wav
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/xtts_api_server/__init__.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/xtts_api_server/__main__.py
+-rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/xtts_api_server/modeldownloader.py
+-rw-r--r--   0        0        0    12849 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/xtts_api_server/server.py
+-rw-r--r--   0        0        0    23940 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/xtts_api_server/tts_funcs.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/README.MD
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/__init__.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/coqui_test.py
+-rw-r--r--   0        0        0   371026 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/silence.wav
+-rw-r--r--   0        0        0     9293 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/stream_player.py
+-rw-r--r--   0        0        0    26015 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/text_to_stream.py
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/threadsafe_generators.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/engines/__init__.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/engines/base_engine.py
+-rw-r--r--   0        0        0   505425 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/engines/coqui_default_voice.json
+-rw-r--r--   0        0        0    29386 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/engines/coqui_engine.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/LICENSE
+-rw-r--r--   0        0        0    10049 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/README.md
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0    10853 2020-02-02 00:00:00.000000 xtts_api_server-0.8.6/PKG-INFO
```

### Comparing `xtts_api_server-0.8.5/XTTS-api-server.ipynb` & `xtts_api_server-0.8.6/XTTS-api-server.ipynb`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/.github/workflows/build-image.yml` & `xtts_api_server-0.8.6/.github/workflows/build-image.yml`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/docker/Dockerfile` & `xtts_api_server-0.8.6/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/example/calm_female.wav` & `xtts_api_server-0.8.6/example/calm_female.wav`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/example/female.wav` & `xtts_api_server-0.8.6/example/female.wav`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/example/male.wav` & `xtts_api_server-0.8.6/example/male.wav`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/xtts_api_server/__main__.py` & `xtts_api_server-0.8.6/xtts_api_server/__main__.py`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/xtts_api_server/modeldownloader.py` & `xtts_api_server-0.8.6/xtts_api_server/modeldownloader.py`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/xtts_api_server/server.py` & `xtts_api_server-0.8.6/xtts_api_server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from TTS.api import TTS
-from fastapi import FastAPI, HTTPException, Request, Query
+from fastapi import BackgroundTasks, FastAPI, HTTPException, Request, Query
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import FileResponse,StreamingResponse
 
 from pydantic import BaseModel
 import uvicorn
 
 import os
 import time
 from pathlib import Path
 import shutil
 from loguru import logger
 from argparse import ArgumentParser
 from pathlib import Path
+from uuid import uuid4
 
 from xtts_api_server.tts_funcs import TTSWrapper,supported_languages,InvalidSettingsError
 from xtts_api_server.RealtimeTTS import TextToAudioStream, CoquiEngine
 from xtts_api_server.modeldownloader import check_stream2sentence_version,install_deepspeed_based_on_python_version
 
 # Default Folders , you can change them via API
 DEVICE = os.getenv('DEVICE',"cuda")
@@ -246,15 +247,15 @@
             if disconnected:
                 break
             yield chunk
 
     return StreamingResponse(generator(), media_type='audio/x-wav')
 
 @app.post("/tts_to_audio/")
-async def tts_to_audio(request: SynthesisRequest):
+async def tts_to_audio(request: SynthesisRequest, background_tasks: BackgroundTasks):
     if STREAM_MODE or STREAM_MODE_IMPROVE:
         try:
             global stream
             # Validate language code against supported languages.
             if request.language.lower() not in supported_languages:
                 raise HTTPException(status_code=400,
                                     detail="Language code sent is either unsupported or misspelled.")
@@ -294,17 +295,21 @@
                 raise HTTPException(status_code=400,
                                     detail="Language code sent is either unsupported or misspelled.")
 
             # Generate an audio file using process_tts_to_file.
             output_file_path = XTTS.process_tts_to_file(
                 text=request.text,
                 speaker_name_or_path=request.speaker_wav,
-                language=request.language.lower()
+                language=request.language.lower(),
+                file_name_or_path=f'{str(uuid4())}.wav'
             )
 
+            if not XTTS.enable_cache_results:
+                background_tasks.add_task(os.unlink, output_file_path)
+
             # Return the file in the response
             return FileResponse(
                 path=output_file_path,
                 media_type='audio/wav',
                 filename="output.wav",
                 )
```

### Comparing `xtts_api_server-0.8.5/xtts_api_server/tts_funcs.py` & `xtts_api_server-0.8.6/xtts_api_server/tts_funcs.py`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/coqui_test.py` & `xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/coqui_test.py`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/silence.wav` & `xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/silence.wav`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/stream_player.py` & `xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/stream_player.py`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/text_to_stream.py` & `xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/text_to_stream.py`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/threadsafe_generators.py` & `xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/threadsafe_generators.py`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/engines/base_engine.py` & `xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/engines/base_engine.py`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/engines/coqui_default_voice.json` & `xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/engines/coqui_default_voice.json`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/xtts_api_server/RealtimeTTS/engines/coqui_engine.py` & `xtts_api_server-0.8.6/xtts_api_server/RealtimeTTS/engines/coqui_engine.py`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/LICENSE` & `xtts_api_server-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/README.md` & `xtts_api_server-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `xtts_api_server-0.8.5/pyproject.toml` & `xtts_api_server-0.8.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling","hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xtts-api-server"
-version = "0.8.5"
+version = "0.8.6"
 authors = [
   { name="daswer123", email="daswerq123@gmail.com" },
 ]
 description = "A simple FastAPI server to host XTTSv2"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -29,15 +29,16 @@
   "python-dotenv",
   "torch",
   "torchaudio",
   "uvicorn",
   "cutlet",
   'fugashi[unidic-lite]',
   'tts==0.21.3',
-  'transformers==4.36.2'
+  'transformers==4.36.2',
+  "uuid"
 ]
 
 [project.urls]
 Homepage = "https://github.com/daswer123/xtts-api-server"
 "Bug Tracker" = "https://github.com/daswer123/xtts-api-server/issues"
 
 [tool.hatch.build.targets.wheel]
```

### Comparing `xtts_api_server-0.8.5/PKG-INFO` & `xtts_api_server-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtts-api-server
-Version: 0.8.5
+Version: 0.8.6
 Summary: A simple FastAPI server to host XTTSv2
 Project-URL: Homepage, https://github.com/daswer123/xtts-api-server
 Project-URL: Bug Tracker, https://github.com/daswer123/xtts-api-server/issues
 Author-email: daswer123 <daswerq123@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,14 +21,15 @@
 Requires-Dist: pyttsx3==2.90
 Requires-Dist: requests==2.31.0
 Requires-Dist: stream2sentence==0.2.2
 Requires-Dist: torch
 Requires-Dist: torchaudio
 Requires-Dist: transformers==4.36.2
 Requires-Dist: tts==0.21.3
+Requires-Dist: uuid
 Requires-Dist: uvicorn
 Description-Content-Type: text/markdown
 
 # A simple FastAPI Server to run XTTSv2
 
 This project is inspired by [silero-api-server](https://github.com/ouoertheo/silero-api-server) and utilizes [XTTSv2](https://github.com/coqui-ai/TTS).
```

