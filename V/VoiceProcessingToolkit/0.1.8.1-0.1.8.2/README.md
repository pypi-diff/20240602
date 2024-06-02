# Comparing `tmp/VoiceProcessingToolkit-0.1.8.1.tar.gz` & `tmp/voiceprocessingtoolkit-0.1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VoiceProcessingToolkit-0.1.8.1.tar", last modified: Mon Feb 12 17:58:30 2024, max compression
+gzip compressed data, was "voiceprocessingtoolkit-0.1.8.2.tar", last modified: Sun Jun  2 18:24:04 2024, max compression
```

## Comparing `VoiceProcessingToolkit-0.1.8.1.tar` & `voiceprocessingtoolkit-0.1.8.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 kristoffervatnehol   (501) staff       (20)        0 2024-02-12 17:58:30.521682 VoiceProcessingToolkit-0.1.8.1/
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)       72 2024-01-12 05:35:19.000000 VoiceProcessingToolkit-0.1.8.1/CONTRIBUTORS.md
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)     1611 2024-01-13 17:35:18.000000 VoiceProcessingToolkit-0.1.8.1/LICENSE.txt
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)      396 2024-01-13 21:08:56.000000 VoiceProcessingToolkit-0.1.8.1/MANIFEST.in
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)     7815 2024-02-12 17:58:30.521473 VoiceProcessingToolkit-0.1.8.1/PKG-INFO
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)     6923 2024-01-14 23:52:30.000000 VoiceProcessingToolkit-0.1.8.1/README.md
-drwxr-xr-x   0 kristoffervatnehol   (501) staff       (20)        0 2024-02-12 17:58:30.513889 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)    22352 2024-02-07 23:19:54.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/VoiceProcessingManager.py
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)       77 2024-01-13 18:35:07.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/__init__.py
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)     1714 2024-02-07 23:08:29.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/shared_resources.py
-drwxr-xr-x   0 kristoffervatnehol   (501) staff       (20)        0 2024-02-12 17:58:30.514670 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/text_to_speech/
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)       85 2024-01-12 05:35:20.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/text_to_speech/__init__.py
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)     6160 2024-02-12 17:52:35.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/text_to_speech/elevenlabs_tts.py
-drwxr-xr-x   0 kristoffervatnehol   (501) staff       (20)        0 2024-02-12 17:58:30.515037 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/transcription/
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)       84 2024-01-12 05:35:20.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/transcription/__init__.py
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)     2290 2024-02-07 23:19:54.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/transcription/whisper.py
-drwxr-xr-x   0 kristoffervatnehol   (501) staff       (20)        0 2024-02-12 17:58:30.515817 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/voice_detection/
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)    13837 2024-02-07 23:55:42.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/voice_detection/Voicerecorder.py
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)       86 2024-01-12 05:35:20.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/voice_detection/__init__.py
-drwxr-xr-x   0 kristoffervatnehol   (501) staff       (20)        0 2024-02-12 17:58:30.517517 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/wake_word_detector/
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)     1725 2024-01-14 00:35:16.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/wake_word_detector/ActionManager.py
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)     4315 2024-01-15 01:20:38.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/wake_word_detector/AudioStreamManager.py
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)     1602 2024-01-12 05:35:20.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/wake_word_detector/NotificationSoundManager.py
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)    11706 2024-01-15 01:19:09.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/wake_word_detector/WakeWordDetector.py
-drwxr-xr-x   0 kristoffervatnehol   (501) staff       (20)        0 2024-02-12 17:58:30.517815 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/wake_word_detector/Wav_MP3/
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)        0 2024-01-13 20:44:07.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/wake_word_detector/Wav_MP3/__init__.py
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)   313422 2024-01-12 05:35:20.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/wake_word_detector/Wav_MP3/notification.wav
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)       89 2024-01-12 05:35:20.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/wake_word_detector/__init__.py
-drwxr-xr-x   0 kristoffervatnehol   (501) staff       (20)        0 2024-02-12 17:58:30.520857 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit.egg-info/
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)     7815 2024-02-12 17:58:30.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit.egg-info/PKG-INFO
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)     2114 2024-02-12 17:58:30.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit.egg-info/SOURCES.txt
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)        1 2024-02-12 17:58:30.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit.egg-info/dependency_links.txt
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)        1 2024-02-12 17:58:30.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit.egg-info/not-zip-safe
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)      110 2024-02-12 17:58:30.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit.egg-info/requires.txt
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)       23 2024-02-12 17:58:30.000000 VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit.egg-info/top_level.txt
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)       38 2024-02-12 17:58:30.521722 VoiceProcessingToolkit-0.1.8.1/setup.cfg
--rw-r--r--   0 kristoffervatnehol   (501) staff       (20)     1358 2024-02-12 17:53:08.000000 VoiceProcessingToolkit-0.1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:24:04.130745 voiceprocessingtoolkit-0.1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-06-02 18:24:04.130745 voiceprocessingtoolkit-0.1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:24:04.126745 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)    22267 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/VoiceProcessingManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/shared_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:24:04.126745 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/text_to_speech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/text_to_speech/elevenlabs_tts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:24:04.126745 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/transcription/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/transcription/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/transcription/whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:24:04.126745 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/voice_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/voice_detection/Voicerecorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/voice_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:24:04.126745 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/wake_word_detector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/wake_word_detector/ActionManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/wake_word_detector/AudioStreamManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/wake_word_detector/NotificationSoundManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11724 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/wake_word_detector/WakeWordDetector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:24:04.126745 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/wake_word_detector/Wav_MP3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/wake_word_detector/Wav_MP3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   313422 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/wake_word_detector/Wav_MP3/notification.wav
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/wake_word_detector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:24:04.130745 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-06-02 18:24:04.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-06-02 18:24:04.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 18:24:04.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 18:24:03.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-06-02 18:24:04.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 18:24:04.000000 voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 18:24:04.130745 voiceprocessingtoolkit-0.1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-06-02 18:23:55.000000 voiceprocessingtoolkit-0.1.8.2/setup.py
```

### Comparing `VoiceProcessingToolkit-0.1.8.1/LICENSE.txt` & `voiceprocessingtoolkit-0.1.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `VoiceProcessingToolkit-0.1.8.1/PKG-INFO` & `voiceprocessingtoolkit-0.1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: VoiceProcessingToolkit
-Version: 0.1.8.1
+Version: 0.1.8.2
 Summary: A comprehensive library for voice processing tasks such as wake word detection, speech recognition, translation, and text-to-speech.
 Home-page: https://github.com/kristofferv98/VoiceProcessingToolkit.git
 Author: Kristoffer Vatnehol
 Author-email: kristoffer.vatnehol@appacia.com
 Project-URL: Bug Tracker, https://github.com/kristofferv98/VoiceProcessingToolkit.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: PyAudio~=0.2.14
+Requires-Dist: openai~=1.6.1
+Requires-Dist: python-dotenv~=1.0.0
 Requires-Dist: requests~=2.31.0
+Requires-Dist: elevenlabs==0.2.27
 Requires-Dist: numpy~=1.26.2
 Requires-Dist: pvcobra~=2.0.1
 Requires-Dist: pvkoala~=2.0.0
 Requires-Dist: pvporcupine~=3.0.1
 Requires-Dist: pygame~=2.5.2
 
  # VoiceProcessingToolkit
```

### Comparing `VoiceProcessingToolkit-0.1.8.1/README.md` & `voiceprocessingtoolkit-0.1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/VoiceProcessingManager.py` & `voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/VoiceProcessingManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from VoiceProcessingToolkit.wake_word_detector.ActionManager import ActionManager
 from VoiceProcessingToolkit.voice_detection.Voicerecorder import AudioRecorder
 from VoiceProcessingToolkit.text_to_speech.elevenlabs_tts import ElevenLabsTextToSpeech, ElevenLabsConfig
 from VoiceProcessingToolkit.shared_resources import thread_manager
 
 logger = logging.getLogger(__name__)
 
-
 def tts(text, voice_id=None, api_key=None):
     """
     Converts text to speech using the ElevenLabs API.
 
     This function synthesizes speech from the given text using ElevenLabs' text-to-speech technology. It handles
     the creation of an ElevenLabsTextToSpeech object and manages the API key retrieval from the environment
     variable or the provided parameter.
@@ -33,15 +32,14 @@
     Returns:
         str or None: File path to the saved audio file, or None if synthesis fails.
     """
     config = ElevenLabsConfig(voice_id=voice_id, api_key=api_key or None)
     tts = ElevenLabsTextToSpeech(config=config, voice_id=voice_id)
     return tts.synthesize_speech(text)
 
-
 def text_to_speech(text, config=None, output_dir=None, voice_id=None, api_key=None):
     """
     Converts text to speech using the ElevenLabs API.
 
     This function synthesizes speech from the given text using ElevenLabs' text-to-speech technology. It handles
     the creation of an ElevenLabsTextToSpeech object and manages the API key retrieval from the environment
     variable or the provided parameter.
@@ -82,15 +80,15 @@
         config = ElevenLabsConfig(api_key=api_key or None)
     if not text:
         logging.info("No text provided for synthesis.")
         return
 
     # Ensure text-to-speech is enabled
     if not config.enable_text_to_speech:
-        logging.debug("Text-to-speech is disabled in settings.")
+        logging.info("Text-to-speech is disabled in settings.")
         return
 
     try:
         # Generate the audio stream
         audio_stream = generate(
             text=text,
             voice=voice_id or config.voice_id,
@@ -102,20 +100,20 @@
         # Stream the audio if playback is enabled
         if config.playback_enabled:
             stream(audio_stream)
     except Exception as e:
         logging.exception(f"An error occurred during streaming text-to-speech: {e}")
 
 
+
 class VoiceProcessingManager:
     def __init__(self, transcriber, action_manager, audio_stream_manager, wake_word='computer', sensitivity=0.75,
                  output_directory='Wav_MP3', wake_word_output='wake_word_output',
                  audio_format=pyaudio.paInt16, channels=1, rate=16000, frames_per_buffer=512,
-                 voice_threshold=0.8, silence_limit=2.0, inactivity_limit=2.0, min_recording_length=2.0,
-                 buffer_length=2.0,
+                 voice_threshold=0.8, silence_limit=2.0, inactivity_limit=2.0, min_recording_length=2.0, buffer_length=2.0,
                  use_wake_word=True, save_wake_word_recordings=False, play_notification_sound=True):
         """
         Manages the voice processing pipeline, including optional wake word detection, voice recording, transcription,
         and text-to-speech synthesis. It can be configured to handle different use cases:
         - Wake Word Detection: When enabled, the manager listens for a specific wake word before activating recording.
         - Text-to-Speech: Converts transcribed text back into speech, which can be played back or streamed.
         - Transcription Only: Records and transcribes speech without wake word detection.
@@ -277,15 +275,15 @@
         self.voice_recorder.perform_recording()
         # Wait for the recording to complete
         if self.voice_recorder.recording_thread:
             self.voice_recorder.recording_thread.join()
         # If a recording was made, transcribe it
         if self.voice_recorder.last_saved_file is not None:
             transcription = self.transcriber.transcribe_audio(self.voice_recorder.last_saved_file)
-            logger.debug(f"Transcription: {transcription}")
+            logger.info(f"Transcription: {transcription}")
             if transcription and tts:
                 if streaming:
                     text_to_speech_stream(transcription, api_key=api_key, voice_id=voice_id)
                 else:
                     text_to_speech(transcription, api_key=api_key, voice_id=voice_id)
             return transcription
         logger.debug("Voice command processing completed.")
@@ -294,20 +292,20 @@
     def monitor_active_threads(self):
         """
         Monitors and logs the status of active threads every second.
         """
         try:
             while True:
                 active_threads = threading.enumerate()
-                logger.debug(f"Active threads: {len(active_threads)}")
+                logger.info(f"Active threads: {len(active_threads)}")
                 for thread in active_threads:
-                    logger.debug(f"Thread {thread.name} is {'alive' if thread.is_alive() else 'not alive'}.")
+                    logger.info(f"Thread {thread.name} is {'alive' if thread.is_alive() else 'not alive'}.")
                 time.sleep(1)
         except KeyboardInterrupt:
-            logger.debug("Thread monitoring interrupted by user.")
+            logger.info("Thread monitoring interrupted by user.")
 
     def is_stream_closed(self):
         """
         Checks if the audio stream is closed.
 
         Returns:
             bool: True if the stream is closed, False otherwise.
@@ -315,16 +313,15 @@
         return self.audio_stream_manager.is_stream_closed()
 
     def reinitialize_stream(self):
         """
         Reinitializes the audio stream if it has been closed.
         """
         if self.is_stream_closed():
-            self.audio_stream_manager.initialize_stream(self.rate, self.channels, self.audio_format,
-                                                        self.frames_per_buffer)
+            self.audio_stream_manager.initialize_stream(self.rate, self.channels, self.audio_format, self.frames_per_buffer)
 
     def run(self, tts=False, streaming=True, api_key=None, voice_id=None, transcription=None):
         """
         Main method to start the voice processing workflow. It can be configured to perform different tasks based on
         the provided arguments:
         - tts (bool): If True, performs text-to-speech on the transcribed text.
         - streaming (bool): If True, streams the synthesized speech instead of saving it to a file.
@@ -341,15 +338,15 @@
             streaming (bool): If True, use streaming text-to-speech. Defaults to False. Only relevant if tts is True.
             api_key (str, optional): API key for ElevenLabs, if not provided in config.
             voice_id (str, optional): Specific voice ID for speech synthesis.
 
         Returns:
             str or None: The transcribed text of the voice command, or None if no valid recording was made.
         """
-        logger.debug("VoiceProcessingManager run method called.")
+        logger.info("VoiceProcessingManager run method called.")
         if transcription is False and self.use_wake_word:
             self.wake_word_detector.run_blocking()
 
             return None
         try:
             transcription = None
             self.reinitialize_stream()
@@ -364,45 +361,46 @@
             if self.voice_recorder.recording_thread:
                 self.voice_recorder.recording_thread.join()
 
             # Check if a recording was made
             if self.voice_recorder.last_saved_file:
                 # Transcribe the recording
                 transcription = self.transcriber.transcribe_audio(self.voice_recorder.last_saved_file)
-                logger.debug(f"Transcription: {transcription}")
+                logger.info(f"Transcription: {transcription}")
 
                 # If transcription is successful and text-to-speech is enabled, synthesize speech
                 if transcription and tts:
                     if streaming:
                         text_to_speech_stream(transcription, api_key=api_key, voice_id=voice_id)
                     else:
                         text_to_speech(transcription, api_key=api_key, voice_id=voice_id)
             else:
                 # If no recording was made or it was too short, log the information
-                logger.debug("Recording was not made or was too short.")
+                logger.info("Recording was not made or was too short.")
 
             # Return the transcription or None if no valid recording was made
             return transcription
 
         except Exception as e:
             logger.exception("An error occurred during voice processing.", exc_info=e)
             raise
 
         except KeyboardInterrupt:
-            logger.debug("KeyboardInterrupt received, performing cleanup.")
+            logger.info("KeyboardInterrupt received, performing cleanup.")
+
 
         finally:
             thread_manager.shutdown()
-            logger.debug("VoiceProcessingManager run method completed.")
+            logger.info("VoiceProcessingManager run method completed.")
 
     def setup(self):
         """
         Initializes the wake word detector and voice recorder components of the voice processing manager.
         """
-        logger.debug("Setting up VoiceProcessingManager components.")
+        logger.info("Setting up VoiceProcessingManager components.")
 
         if self.use_wake_word:
             # Initialize WakeWordDetector
             self.wake_word_detector = WakeWordDetector(
                 access_key=os.environ.get('PICOVOICE_APIKEY') or os.getenv('PICOVOICE_APIKEY'),
                 wake_word=self.wake_word,
                 sensitivity=self.sensitivity,
@@ -435,11 +433,11 @@
         if self.voice_recorder.recording_thread:
             self.voice_recorder.recording_thread.join()
 
         # If a recording was made, transcribe it
         if self.voice_recorder.last_saved_file is not None:
             # where the transcrition file recorded is stored
             transcription = self.transcriber.transcribe_audio(self.voice_recorder.last_saved_file)
-            logger.debug(f"Transcription: {transcription}")
+            logger.info(f"Transcription: {transcription}")
             return transcription
 
         return None
```

### Comparing `VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/shared_resources.py` & `voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/shared_resources.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,33 +8,33 @@
 class ThreadManager:
     def __init__(self):
         self.threads = []
         self.shutdown_requested = False
 
     def add_thread(self, thread):
         if thread and isinstance(thread, threading.Thread):
-            logger.debug("Adding thread %s to thread manager", thread.name)
+            logger.info("Adding thread %s to thread manager", thread.name)
             self.threads.append(thread)
 
     def join_all(self):
         for thread in self.threads:
-            logger.debug("Joining thread %s", thread.name)
+            logger.info("Joining thread %s", thread.name)
             if thread.is_alive():
-                logger.debug("Thread %s is alive, joining...", thread.name)
+                logger.info("Thread %s is alive, joining...", thread.name)
                 try:
                     thread.join()
                 except KeyboardInterrupt:
                     # If a KeyboardInterrupt occurs while joining, we set the shutdown flag
                     shutdown_flag.set()
                     # And re-raise the exception to handle it in the outer scope
                     raise
 
     def shutdown(self):
         # Ensure that shutdown is only performed once
-        logger.debug("Shutdown requested")
+        logger.info("Shutdown requested")
         if self.shutdown_requested:
             return
         shutdown_flag.set()
         # Signal all threads to shutdown
         shutdown_flag.set()
         self.join_all()
         self.shutdown_requested = True
```

### Comparing `VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/text_to_speech/elevenlabs_tts.py` & `voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/text_to_speech/elevenlabs_tts.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 import time
 
 import pygame
 import requests
 
 # Constants
 ELEVENLABS_API_URL = 'https://api.elevenlabs.io/v1/text-to-speech/'
-ELEVENLABS_MODEL_ID = 'eleven_multilingual_v2'
+ELEVENLABS_MODEL_ID = 'eleven_monolingual_v1'
 
 
 # Configuration class
 class ElevenLabsConfig:
     # The API key forElevenLabs can be provided as an argument or set as an environment variable 'ELEVENLABS_API_KEY'.
     def __init__(self, api_key=None, voice_id=None, model_id=None, playback_enabled=True):
         self.elevenlabs_api_key = os.getenv('ELEVENLABS_API_KEY', api_key) or api_key
-        self.voice_id = voice_id or "ThT5KcBeYPX3keUQqHPh"
+        self.voice_id = voice_id or "eqI1AF0IrvwU3tgfmt0B"
         self.model_id = model_id or ELEVENLABS_MODEL_ID
         self.enable_text_to_speech = True
         self.playback_enabled = playback_enabled
 
         if not self.elevenlabs_api_key:
             raise ValueError("API key is required for ElevenLabsTextToSpeech.")
 
@@ -51,15 +51,15 @@
             output_dir (str, optional): The directory to save the audio file. Defaults to None.
 
         Returns:
             str: Path to the audio file if successful, None otherwise.
         """
         config = self.config
         if not config.enable_text_to_speech:
-            logging.debug("Text-to-speech is disabled in settings.")
+            logging.info("Text-to-speech is disabled in settings.")
             return None
         if text is None or text == 'NO_VOICE_EXIT' or text == '':
             return None
 
         # Remove asterisks and hashes from the text
         text = text.replace('*', '').replace('#', '')
 
@@ -94,15 +94,15 @@
             logging.debug("Received response from ElevenLabs API with status code: %s", response.status_code)
             if response.status_code == 200:
                 # Define the output file path
                 output_file = os.path.join(output_dir, 'output.mp3')
                 with open(output_file, 'wb') as f:
                     f.write(response.content)
 
-                logging.debug(f"Audio file created at: {output_file}")
+                logging.info(f"Audio file created at: {output_file}")
 
                 # Initialize pygame mixer and play audio file if playback is enabled
                 if config.playback_enabled:
                     pygame.mixer.init()
                     self.mixer_initialized = True
                     pygame.mixer.music.load(output_file)
                     try:
@@ -147,11 +147,8 @@
                 self.temp_dir.cleanup()
                 self.temp_dir = None
 
 
 if __name__ == '__main__':
     logging.basicConfig(level=logging.DEBUG)
     load_dotenv()
-    elevenlabs_api_key = os.getenv('ELEVENLABS_API_KEY')
-    tts = ElevenLabsTextToSpeech()
-    tts.synthesize_speech("Hello world!")
```

### Comparing `VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/transcription/whisper.py` & `voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/transcription/whisper.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,17 +47,17 @@
             logging.exception("An error occurred during the transcription process: %s", e)
             raise
         else:
             # Access the translated and transcribed text
             transcription_text = getattr(transcript, "text", None)
             if transcription_text is not None:
                 transcription_text = transcription_text.strip()
-            logging.debug(f"Transcription: {transcription_text}")
+            logging.info(f"Transcription: {transcription_text}")
             return transcription_text
 
 
 if __name__ == '__main__':
     audio_path = "path_to_audio.mp3"
     transcriber = WhisperTranscriber()
     transcription = transcriber.transcribe_audio(audio_path)
     if transcription:
-        logging.debug(f"Transcription: {transcription}")
+        logging.info(f"Transcription: {transcription}")
```

### Comparing `VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/voice_detection/Voicerecorder.py` & `voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/voice_detection/Voicerecorder.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         self._audio_data_provider = AudioDataProvider()
         self.recording_thread = threading.Thread(target=self.start_recording, args=(self._audio_data_provider,))
         self.recording_thread.start()
         try:
             while self._is_recording:
                 time.sleep(0.1)
         except KeyboardInterrupt:
-            self._logger.debug("Recording interrupted by user.")
+            self._logger.info("Recording interrupted by user.")
         finally:
             self.stop_recording()
             return self.last_saved_file if self.last_saved_file else None
 
     def start_recording(self, audio_data_provider: AudioDataProvider) -> None:
         """
         Starts the audio recording process using the provided audio data provider.
@@ -113,15 +113,15 @@
             audio_data_provider (AudioDataProvider): The provider of audio data frames.
         """
         self._audio_data_provider = audio_data_provider
         self._audio_data_provider.start_stream()
         self._is_recording = True
         self.recording_thread = threading.Thread(target=self.record_loop, args=(audio_data_provider,))
         self.recording_thread.start()
-        self._logger.debug("Recording started.")
+        self._logger.info("Recording started.")
 
     def record_loop(self, audio_data_provider: AudioDataProvider) -> None:
         """
         The main loop for recording audio, processing frames, and managing recording state.
         Args:
             audio_data_provider (AudioDataProvider): The provider of audio data frames.
         """
@@ -138,15 +138,15 @@
                         self._inactivity_frames = 0  # Inactivity frames counter is now private
                         self._frames_to_save.append(frame)
                     else:
                         self._inactivity_frames += 1
                         silent_frames += 1
 
                         if self.should_finalize_recording(silent_frames):
-                            self._logger.debug("Inactivity limit exceeded. Finalizing recording...")
+                            self._logger.info("Inactivity limit exceeded. Finalizing recording...")
                             return
             except Exception as e:
                 self._logger.error(f"An error occurred during recording: {e}")
                 break
 
     def should_finalize_recording(self, silent_frames: int) -> bool:
         """
@@ -154,15 +154,15 @@
         Args:
             silent_frames (int): The number of consecutive silent frames.
         Returns:
             bool: True if the recording should be finalized, False otherwise.
         """
         if (self._inactivity_frames * self._cobra_handle.frame_length / self._cobra_handle.sample_rate > self.
                 INACTIVITY_LIMIT):
-            self._logger.debug("No voice detected for a while. Finalizing recording...")
+            self._logger.info("No voice detected for a while. Finalizing recording...")
             self.finalize_recording()
             return True
         if (silent_frames * self._cobra_handle.frame_length / self._cobra_handle.sample_rate > self.
                 SILENCE_LIMIT):
             self._logger.info("Exceeded silence limit. Finalizing recording...")
             self.finalize_recording()
             return True
@@ -248,17 +248,17 @@
         """
         saved_file_path = None
         if self._frames_to_save:
             recording_length = len(
                 self._frames_to_save) * self._cobra_handle.frame_length / self._cobra_handle.sample_rate
             if recording_length >= self.MIN_RECORDING_LENGTH:
                 saved_file_path = self.save_to_wav_file(self._frames_to_save)
-                self._logger.debug(f"Recording of {recording_length:.2f} seconds saved.")
+                self._logger.info(f"Recording of {recording_length:.2f} seconds saved.")
             else:
-                self._logger.debug(
+                self._logger.info(
                     f"Recording of {recording_length:.2f} seconds is under the minimum length. Discarded.")
             self._recording = False  # Ensure recording state is reset
             self._frames_to_save = []  # Clear the frames to save
             self._is_recording = False  # Ensure is_recording state is reset
             if self.recording_thread:
                 self.recording_thread = None  # Reset the recording thread
         self._recording = False  # Recording state is now private
@@ -288,26 +288,26 @@
         filename = os.path.join(recordings_dir, "recording.wav")
 
         with wave.open(filename, 'wb') as wf:
             wf.setnchannels(1)
             wf.setsampwidth(self._py_audio.get_sample_size(pyaudio.paInt16))
             wf.setframerate(self._cobra_handle.sample_rate)
             wf.writeframes(b''.join(frames))
-        logger.debug(f"Saved to {filename}")
+        logger.info(f"Saved to {filename}")
         return os.path.abspath(filename)
 
     def stop_recording(self) -> None:
         """
         Stops the recording process and joins the recording thread.
         """
         self._is_recording = False  # Recording state is now private
         if self.recording_thread:
             self.recording_thread.join()
             self._py_audio.terminate()
-        self._logger.debug("Recording stopped.")
+        self._logger.info("Recording stopped.")
 
 
 if __name__ == '__main__':
     # Set up logging
     logging.basicConfig(level=logging.INFO)
     load_dotenv()
```

### Comparing `VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/wake_word_detector/ActionManager.py` & `voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/wake_word_detector/ActionManager.py`

 * *Files identical despite different names*

### Comparing `VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/wake_word_detector/AudioStreamManager.py` & `voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/wake_word_detector/AudioStreamManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         Initializes the audio stream with the given parameters.
         """
         if self._py_audio is None:
             self._py_audio = pyaudio.PyAudio()
         try:
             return self._py_audio.open(rate=rate, channels=channels, format=_audio_format,
                                        input=True, frames_per_buffer=frames_per_buffer)
-        except (pyaudio.PyAudio, IOError) as e:
+        except (pyaudio.PyAudioError, IOError) as e:
             logger.exception("Failed to initialize audio stream: %s", e)
             raise
         except Exception as e:
             logger.exception("An unexpected error occurred while initializing the audio stream.", exc_info=e)
             raise
 
     def get_stream(self):
```

### Comparing `VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/wake_word_detector/NotificationSoundManager.py` & `voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/wake_word_detector/NotificationSoundManager.py`

 * *Files identical despite different names*

### Comparing `VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/wake_word_detector/WakeWordDetector.py` & `voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/wake_word_detector/WakeWordDetector.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,14 +230,15 @@
         self._porcupine.delete()
 
 
 def main():
     logging.basicConfig(level=logging.DEBUG)
 
     load_dotenv()
+    load_dotenv()
     # Set up the access key for Porcupine
     access_key = os.getenv('PICOVOICE_APIKEY')
 
     # Set up the audio stream parameters
     rate = 16000
     channels = 1
     audio_format = pyaudio.paInt16
```

### Comparing `VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit/wake_word_detector/Wav_MP3/notification.wav` & `voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit/wake_word_detector/Wav_MP3/notification.wav`

 * *Files identical despite different names*

### Comparing `VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit.egg-info/PKG-INFO` & `voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: VoiceProcessingToolkit
-Version: 0.1.8.1
+Version: 0.1.8.2
 Summary: A comprehensive library for voice processing tasks such as wake word detection, speech recognition, translation, and text-to-speech.
 Home-page: https://github.com/kristofferv98/VoiceProcessingToolkit.git
 Author: Kristoffer Vatnehol
 Author-email: kristoffer.vatnehol@appacia.com
 Project-URL: Bug Tracker, https://github.com/kristofferv98/VoiceProcessingToolkit.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: PyAudio~=0.2.14
+Requires-Dist: openai~=1.6.1
+Requires-Dist: python-dotenv~=1.0.0
 Requires-Dist: requests~=2.31.0
+Requires-Dist: elevenlabs==0.2.27
 Requires-Dist: numpy~=1.26.2
 Requires-Dist: pvcobra~=2.0.1
 Requires-Dist: pvkoala~=2.0.0
 Requires-Dist: pvporcupine~=3.0.1
 Requires-Dist: pygame~=2.5.2
 
  # VoiceProcessingToolkit
```

### Comparing `VoiceProcessingToolkit-0.1.8.1/VoiceProcessingToolkit.egg-info/SOURCES.txt` & `voiceprocessingtoolkit-0.1.8.2/VoiceProcessingToolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VoiceProcessingToolkit-0.1.8.1/setup.py` & `voiceprocessingtoolkit-0.1.8.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="VoiceProcessingToolkit",
-    version="0.1.8.1",
+    version="0.1.8.2",
     author="Kristoffer Vatnehol",
     author_email="kristoffer.vatnehol@appacia.com",
     description="A comprehensive library for voice processing tasks such as wake word detection, speech recognition, "
                 "translation, and text-to-speech.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kristofferv98/VoiceProcessingToolkit.git",
@@ -23,15 +23,18 @@
     ],
     package_dir={"": "."},
     packages=find_packages(where="."),
     include_package_data=True,
     python_requires=">=3.6",
     install_requires=[
         "PyAudio~=0.2.14",
+        "openai~=1.6.1",
+        "python-dotenv~=1.0.0",
         "requests~=2.31.0",
+        "elevenlabs==0.2.27",
         "numpy~=1.26.2",
         "pvcobra~=2.0.1",
         "pvkoala~=2.0.0",
         "pvporcupine~=3.0.1",
         "pygame~=2.5.2",
     ],
     package_data={
```

