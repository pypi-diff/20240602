# Comparing `tmp/rocat-0.2.0.tar.gz` & `tmp/rocat-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocat-0.2.0.tar", last modified: Sat Jun  1 23:35:27 2024, max compression
+gzip compressed data, was "rocat-0.2.1.tar", last modified: Sun Jun  2 07:36:04 2024, max compression
```

## Comparing `rocat-0.2.0.tar` & `rocat-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 23:35:27.349848 rocat-0.2.0/
--rw-rw-rw-   0        0        0     1081 2024-05-28 06:15:40.000000 rocat-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     4581 2024-06-01 23:35:27.348851 rocat-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3551 2024-05-28 08:33:31.000000 rocat-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 23:35:27.338883 rocat-0.2.0/rocat/
--rw-rw-rw-   0        0        0      869 2024-05-28 08:57:15.000000 rocat-0.2.0/rocat/__init__.py
--rw-rw-rw-   0        0        0     1162 2024-05-28 08:32:13.000000 rocat-0.2.0/rocat/__main__.py
--rw-rw-rw-   0        0        0     2623 2024-05-28 08:58:20.000000 rocat-0.2.0/rocat/ai_functions.py
--rw-rw-rw-   0        0        0     2116 2024-05-28 08:58:23.000000 rocat-0.2.0/rocat/config.py
--rw-rw-rw-   0        0        0    12217 2024-05-28 08:58:41.000000 rocat-0.2.0/rocat/file_utils.py
--rw-rw-rw-   0        0        0     7451 2024-05-28 08:54:53.000000 rocat-0.2.0/rocat/language_model.py
--rw-rw-rw-   0        0        0      838 2024-05-28 08:56:06.000000 rocat-0.2.0/rocat/language_utils.py
--rw-rw-rw-   0        0        0      480 2024-05-28 08:56:10.000000 rocat-0.2.0/rocat/main.py
--rw-rw-rw-   0        0        0      807 2024-05-28 08:56:11.000000 rocat-0.2.0/rocat/template_utils.py
--rw-rw-rw-   0        0        0     2215 2024-05-28 08:58:58.000000 rocat-0.2.0/rocat/web_utils.py
-drwxrwxrwx   0        0        0        0 2024-06-01 23:35:27.347854 rocat-0.2.0/rocat.egg-info/
--rw-rw-rw-   0        0        0     4581 2024-06-01 23:35:27.000000 rocat-0.2.0/rocat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2024-06-01 23:35:27.000000 rocat-0.2.0/rocat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 23:35:27.000000 rocat-0.2.0/rocat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-06-01 23:35:27.000000 rocat-0.2.0/rocat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      303 2024-06-01 23:35:27.000000 rocat-0.2.0/rocat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-06-01 23:35:27.000000 rocat-0.2.0/rocat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 23:35:27.349848 rocat-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1462 2024-06-01 23:34:42.000000 rocat-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 23:35:27.347854 rocat-0.2.0/tests/
--rw-rw-rw-   0        0        0     2055 2024-05-28 06:15:40.000000 rocat-0.2.0/tests/test.py
--rw-rw-rw-   0        0        0     3341 2024-05-28 09:06:39.000000 rocat-0.2.0/tests/test_file_utils.py
--rw-rw-rw-   0        0        0     1137 2024-05-28 09:03:24.000000 rocat-0.2.0/tests/test_web_utils.py
+drwxrwxrwx   0        0        0        0 2024-06-02 07:36:04.006117 rocat-0.2.1/
+-rw-rw-rw-   0        0        0     1081 2024-05-28 06:15:40.000000 rocat-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4566 2024-06-02 07:36:04.005120 rocat-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3539 2024-06-02 06:45:57.000000 rocat-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 07:36:03.992164 rocat-0.2.1/rocat/
+-rw-rw-rw-   0        0        0      753 2024-06-02 04:55:56.000000 rocat-0.2.1/rocat/__init__.py
+-rw-rw-rw-   0        0        0     1162 2024-05-28 08:32:13.000000 rocat-0.2.1/rocat/__main__.py
+-rw-rw-rw-   0        0        0     2449 2024-06-02 05:16:39.000000 rocat-0.2.1/rocat/ai_functions.py
+-rw-rw-rw-   0        0        0      651 2024-06-02 06:01:19.000000 rocat-0.2.1/rocat/audio_utils.py
+-rw-rw-rw-   0        0        0     2426 2024-06-02 04:57:35.000000 rocat-0.2.1/rocat/config.py
+-rw-rw-rw-   0        0        0    11584 2024-06-02 07:35:00.000000 rocat-0.2.1/rocat/file_utils.py
+-rw-rw-rw-   0        0        0     1482 2024-06-02 05:30:21.000000 rocat-0.2.1/rocat/image_utils.py
+-rw-rw-rw-   0        0        0     5804 2024-06-02 05:14:37.000000 rocat-0.2.1/rocat/language_model.py
+-rw-rw-rw-   0        0        0      838 2024-05-28 08:56:06.000000 rocat-0.2.1/rocat/language_utils.py
+-rw-rw-rw-   0        0        0      480 2024-05-28 08:56:10.000000 rocat-0.2.1/rocat/main.py
+-rw-rw-rw-   0        0        0      807 2024-05-28 08:56:11.000000 rocat-0.2.1/rocat/template_utils.py
+-rw-rw-rw-   0        0        0     2215 2024-06-02 01:42:25.000000 rocat-0.2.1/rocat/web_utils.py
+drwxrwxrwx   0        0        0        0 2024-06-02 07:36:04.004124 rocat-0.2.1/rocat.egg-info/
+-rw-rw-rw-   0        0        0     4566 2024-06-02 07:36:03.000000 rocat-0.2.1/rocat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-06-02 07:36:03.000000 rocat-0.2.1/rocat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 07:36:03.000000 rocat-0.2.1/rocat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-06-02 07:36:03.000000 rocat-0.2.1/rocat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      302 2024-06-02 07:36:03.000000 rocat-0.2.1/rocat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-06-02 07:36:03.000000 rocat-0.2.1/rocat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 07:36:04.006117 rocat-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1461 2024-06-02 07:35:33.000000 rocat-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 07:36:04.003127 rocat-0.2.1/tests/
+-rw-rw-rw-   0        0        0     1988 2024-06-02 05:36:39.000000 rocat-0.2.1/tests/test_ai_functions.py
+-rw-rw-rw-   0        0        0      934 2024-06-02 06:11:22.000000 rocat-0.2.1/tests/test_audio_utils.py
+-rw-rw-rw-   0        0        0     4864 2024-06-02 06:45:29.000000 rocat-0.2.1/tests/test_file_utils.py
+-rw-rw-rw-   0        0        0     1613 2024-06-02 05:38:40.000000 rocat-0.2.1/tests/test_image_utils.py
+-rw-rw-rw-   0        0        0     1392 2024-06-02 05:39:16.000000 rocat-0.2.1/tests/test_language_model.py
+-rw-rw-rw-   0        0        0      640 2024-06-02 05:39:27.000000 rocat-0.2.1/tests/test_template_utils.py
+-rw-rw-rw-   0        0        0     1543 2024-06-02 06:10:32.000000 rocat-0.2.1/tests/test_web_utils.py
```

### Comparing `rocat-0.2.0/LICENSE` & `rocat-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rocat-0.2.0/PKG-INFO` & `rocat-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocat
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple and user-friendly library for AI services
 Home-page: https://github.com/Yumeta-Lab/rocat-dev
 Author: YumetaLab
 Author-email: root@yumeta.kr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: docx2txt==0.8
 Requires-Dist: google_search_results==2.4.2
 Requires-Dist: openai==1.30.3
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: pandas==2.2.2
 Requires-Dist: pillow==10.3.0
-Requires-Dist: PyPDF2==3.0.1
+Requires-Dist: pypdf==4.2.0
 Requires-Dist: python-docx==1.1.2
 Requires-Dist: python-pptx==0.6.23
 Requires-Dist: requests==2.32.2
 Requires-Dist: serpapi==0.1.5
 Requires-Dist: xlrd==2.0.1
 Requires-Dist: XlsxWriter==3.2.0
 Requires-Dist: youtube-transcript-api==0.6.2
@@ -33,146 +33,152 @@
 
 RoCat is a Python library that provides a simple and user-friendly interface for integrating AI services into your projects. It supports various AI functionalities such as text summarization, YouTube transcript retrieval, audio transcription using OpenAI's Whisper, and web search using SerpAPI.
 
 ## Installation
 
 You can install RoCat using pip:
 
-​```bash
+~~~bash
 pip install rocat
-​```
+~~~
 
 ## Quick Start Guide
 
-1. Initialize RoCat: Begin by creating a default configuration and example code to get started.
+1. **Initialize RoCat**: Begin by creating a default configuration and example code to get started.
 
-```bash
-(.venv) > rocat init 
+~~~bash
+rocat init
 
 Default configuration file and example code created.
-- config.ini      
+- config.ini
 - rocat_example.py
-```
+~~~
 
 This command creates a default configuration file (config.ini) and an example script (rocat_example.py).
 
-2. Edit Configuration: Open config.ini to add your API keys.
+2. **Edit Configuration**: Open config.ini to add your API keys.
 
-```bash
+~~~ini
 [API_KEYS]
 openai = 
 anthropic = 
-naver = 
 serpapi =
-```
+naver_clovastudio =
+naver_apigw =
+~~~
 
-3. Now write your code! You can refer to the rocat_example.py file for sample usage of the library.
+3. **Write Your Code**: You can refer to the rocat_example.py file for sample usage of the library.
 
-```python
+~~~python
 # rocat_example.py
 import rocat as rc
 
 def main():
     # Initialize the library
     rc.initialize()
     
     # Write your code here.
 
 if __name__ == "__main__":
     main()
-```
+~~~
 
 ## Example Usage
 
 ### Text Summarization
-```python
+
+~~~python
 def main():
     rc.initialize()
     
-    # Get text from a web page  
-    url = "https://www.example.com/sample-page"  
-    text = rc.get_web(url)  
-
-    # Summarize the text  
+    # Get text from a web page
+    url = "https://www.example.com/sample-page"
+    text = rc.get_web(url)
+    
+    # Summarize the text
     summary = rc.ai_summarize(text, 3)
-
-
-    # Print the summarized text  
-    print("\nAI Summary Test:")  
+    
+    # Print the summarized text
+    print("\nAI Summary Test:")
     print(summary)
 
 if __name__ == "__main__":
     main()
-```
+~~~
 
 ### YouTube Transcript Retrieval
-```python
+
+~~~python
 def main():
     rc.initialize()
     
-    # Get captions from a YouTube video  
-    video_url = "https://www.youtube.com/watch?v=example-video-id"  
-    transcript = rc.get_youtube(video_url)  
-
-    # Print the caption text  
-    print("\nYouTube Caption Test:")  
-    print(transcript)  
+    # Get captions from a YouTube video
+    video_url = "https://www.youtube.com/watch?v=example-video-id"
+    transcript = rc.get_youtube(video_url)
+    
+    # Print the caption text
+    print("\nYouTube Caption Test:")
+    print(transcript)
 
 if __name__ == "__main__":
     main()
-```
+~~~
 
+### Audio Transcription
 
-### Audio Transcription 
-```python
+~~~python
 def main():
     rc.initialize()
     
-    # Convert an audio file to text  
-    audio_file = "path/to/example/audio.mp3"  
-    transcription = rc.get_whisper(audio_file)  
-
-    # Print the converted text  
-    print("\nWhisper Recognition :")  
-    print(transcription)  
+    # Convert an audio file to text
+    audio_file = "path/to/example/audio.mp3"
+    transcription = rc.get_whisper(audio_file)
+    
+    # Print the converted text
+    print("\nWhisper Recognition:")
+    print(transcription)
 
 if __name__ == "__main__":
     main()
-```
+~~~
 
 ### Web Search
-```python
+
+~~~python
 def main():
     rc.initialize()
     
-    # Get google search results  
-    query = "python"  
-    search_results = rc.get_search(query)  
-    for result in search_results:  
-        print(f"Title: {result['title']}")  
-        print(f"Link: {result['link']}")  
+    # Get Google search results
+    query = "python"
+    search_results = rc.get_search(query)
+    for result in search_results:
+        print(f"Title: {result['title']}")
+        print(f"Link: {result['link']}")
         print(f"Snippet: {result['snippet']}")
 
 if __name__ == "__main__":
     main()
-```
+~~~
 
 ## Features
 
 - Text summarization using AI
 - YouTube transcript retrieval
 - Audio transcription using OpenAI's Whisper
 - Web search using SerpAPI
 - File utilities for handling various file formats (txt, xls, xlsx, doc, docx, ppt, pptx, csv, pdf, hwp, hwpx)
 - Language model integration (GPT-3.5, GPT-4, Claude, Opus, Haiku, Sonnet)
 
 ## License
+
 This project is licensed under the MIT License. See the LICENSE file for more information.
 
 ## Contributing
+
 Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the GitHub repository.
 
 ## Contact
+
 If you have any questions or inquiries, please contact the author:
 
 - Name: Faith6
 - Email: root@yumeta.kr
```

### Comparing `rocat-0.2.0/README.md` & `rocat-0.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,146 +2,152 @@
 
 RoCat is a Python library that provides a simple and user-friendly interface for integrating AI services into your projects. It supports various AI functionalities such as text summarization, YouTube transcript retrieval, audio transcription using OpenAI's Whisper, and web search using SerpAPI.
 
 ## Installation
 
 You can install RoCat using pip:
 
-​```bash
+~~~bash
 pip install rocat
-​```
+~~~
 
 ## Quick Start Guide
 
-1. Initialize RoCat: Begin by creating a default configuration and example code to get started.
+1. **Initialize RoCat**: Begin by creating a default configuration and example code to get started.
 
-```bash
-(.venv) > rocat init 
+~~~bash
+rocat init
 
 Default configuration file and example code created.
-- config.ini      
+- config.ini
 - rocat_example.py
-```
+~~~
 
 This command creates a default configuration file (config.ini) and an example script (rocat_example.py).
 
-2. Edit Configuration: Open config.ini to add your API keys.
+2. **Edit Configuration**: Open config.ini to add your API keys.
 
-```bash
+~~~ini
 [API_KEYS]
 openai = 
 anthropic = 
-naver = 
 serpapi =
-```
+naver_clovastudio =
+naver_apigw =
+~~~
 
-3. Now write your code! You can refer to the rocat_example.py file for sample usage of the library.
+3. **Write Your Code**: You can refer to the rocat_example.py file for sample usage of the library.
 
-```python
+~~~python
 # rocat_example.py
 import rocat as rc
 
 def main():
     # Initialize the library
     rc.initialize()
     
     # Write your code here.
 
 if __name__ == "__main__":
     main()
-```
+~~~
 
 ## Example Usage
 
 ### Text Summarization
-```python
+
+~~~python
 def main():
     rc.initialize()
     
-    # Get text from a web page  
-    url = "https://www.example.com/sample-page"  
-    text = rc.get_web(url)  
-
-    # Summarize the text  
+    # Get text from a web page
+    url = "https://www.example.com/sample-page"
+    text = rc.get_web(url)
+    
+    # Summarize the text
     summary = rc.ai_summarize(text, 3)
-
-
-    # Print the summarized text  
-    print("\nAI Summary Test:")  
+    
+    # Print the summarized text
+    print("\nAI Summary Test:")
     print(summary)
 
 if __name__ == "__main__":
     main()
-```
+~~~
 
 ### YouTube Transcript Retrieval
-```python
+
+~~~python
 def main():
     rc.initialize()
     
-    # Get captions from a YouTube video  
-    video_url = "https://www.youtube.com/watch?v=example-video-id"  
-    transcript = rc.get_youtube(video_url)  
-
-    # Print the caption text  
-    print("\nYouTube Caption Test:")  
-    print(transcript)  
+    # Get captions from a YouTube video
+    video_url = "https://www.youtube.com/watch?v=example-video-id"
+    transcript = rc.get_youtube(video_url)
+    
+    # Print the caption text
+    print("\nYouTube Caption Test:")
+    print(transcript)
 
 if __name__ == "__main__":
     main()
-```
+~~~
 
+### Audio Transcription
 
-### Audio Transcription 
-```python
+~~~python
 def main():
     rc.initialize()
     
-    # Convert an audio file to text  
-    audio_file = "path/to/example/audio.mp3"  
-    transcription = rc.get_whisper(audio_file)  
-
-    # Print the converted text  
-    print("\nWhisper Recognition :")  
-    print(transcription)  
+    # Convert an audio file to text
+    audio_file = "path/to/example/audio.mp3"
+    transcription = rc.get_whisper(audio_file)
+    
+    # Print the converted text
+    print("\nWhisper Recognition:")
+    print(transcription)
 
 if __name__ == "__main__":
     main()
-```
+~~~
 
 ### Web Search
-```python
+
+~~~python
 def main():
     rc.initialize()
     
-    # Get google search results  
-    query = "python"  
-    search_results = rc.get_search(query)  
-    for result in search_results:  
-        print(f"Title: {result['title']}")  
-        print(f"Link: {result['link']}")  
+    # Get Google search results
+    query = "python"
+    search_results = rc.get_search(query)
+    for result in search_results:
+        print(f"Title: {result['title']}")
+        print(f"Link: {result['link']}")
         print(f"Snippet: {result['snippet']}")
 
 if __name__ == "__main__":
     main()
-```
+~~~
 
 ## Features
 
 - Text summarization using AI
 - YouTube transcript retrieval
 - Audio transcription using OpenAI's Whisper
 - Web search using SerpAPI
 - File utilities for handling various file formats (txt, xls, xlsx, doc, docx, ppt, pptx, csv, pdf, hwp, hwpx)
 - Language model integration (GPT-3.5, GPT-4, Claude, Opus, Haiku, Sonnet)
 
 ## License
+
 This project is licensed under the MIT License. See the LICENSE file for more information.
 
 ## Contributing
+
 Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the GitHub repository.
 
 ## Contact
+
 If you have any questions or inquiries, please contact the author:
 
 - Name: Faith6
-- Email: root@yumeta.kr
+- Email: root@yumeta.kr
```

### Comparing `rocat-0.2.0/rocat/__main__.py` & `rocat-0.2.1/rocat/__main__.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.0/rocat/ai_functions.py` & `rocat-0.2.1/rocat/ai_functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# rocat/ai_functions.py
 from rocat import language_model
 
 config = None
 
 def set_config(cfg):
     """
     설정을 전역 변수 config에 저장합니다.
@@ -13,62 +12,51 @@
     config = cfg
 
 def _run_model(prompt, model):
     """
     선택한 모델을 사용하여 프롬프트를 처리하고 결과를 반환합니다.
 
     :param prompt: 모델에 입력할 프롬프트 텍스트
-    :param model: 사용할 모델의 이름 ("gpt", "gpt4", "opus", "haiku", "sonnet")
+    :param model: 사용할 모델의 이름 ("gpt3", "gpt4o", "opus", "haiku", "sonnet", "clova")
     :return: 모델이 생성한 텍스트
     :raises ValueError: 지원하지 않는 모델이 선택된 경우
     """
-    if model == "gpt":
-        return language_model.run_gpt(prompt)
-    elif model == "gpt4":
-        return language_model.run_gpt4(prompt)
-    elif model == "opus":
-        return language_model.run_opus(prompt)
-    elif model == "haiku":
-        return language_model.run_haiku(prompt)
-    elif model == "sonnet":
-        return language_model.run_sonnet(prompt)
-    else:
-        raise ValueError(f"지원하지 않는 모델: {model}")
+    return language_model.run_model(model, prompt)
 
-def ai_summarize(text, num_sentences, model="gpt"):
+def ai_summarize(text, num_sentences, model="gpt3"):
     """
     주어진 텍스트를 지정된 개수의 문장으로 요약합니다.
 
     :param text: 요약할 텍스트
     :param num_sentences: 요약본에 포함할 문장의 개수
-    :param model: 사용할 모델의 이름 (기본값: "gpt")
+    :param model: 사용할 모델의 이름 (기본값: "gpt3", 선택 가능한 모델: "gpt3", "gpt4o", "opus", "haiku", "sonnet", "clova")
     :return: 요약된 텍스트
     """
     prompt = f"다음 텍스트를 {num_sentences}개의 문장으로 요약해 주세요:\n\n{text}"
     summary = _run_model(prompt, model)
     return summary
 
-def ai_bullet(text, num, model="gpt"):
+def ai_bullet(text, num, model="gpt3"):
     """
     주어진 텍스트를 지정된 개수의 bullet point로 요약합니다.
 
     :param text: 요약할 텍스트
     :param num: 생성할 bullet point의 개수
-    :param model: 사용할 모델의 이름 (기본값: "gpt")
+    :param model: 사용할 모델의 이름 (기본값: "gpt3", 선택 가능한 모델: "gpt3", "gpt4o", "opus", "haiku", "sonnet", "clova")
     :return: bullet point로 요약된 텍스트
     """
     prompt = f"다음 텍스트를 {num}개의 bullet point로 요약해 주세요:\n\n{text}"
     bullet_points = _run_model(prompt, model)
     return bullet_points
 
-def ai_translate(text, target_lang, model="gpt"):
+def ai_translate(text, target_lang, model="gpt3"):
     """
     주어진 텍스트를 지정된 언어로 번역합니다.
 
     :param text: 번역할 텍스트
     :param target_lang: 번역 대상 언어
-    :param model: 사용할 모델의 이름 (기본값: "gpt")
+    :param model: 사용할 모델의 이름 (기본값: "gpt3", 선택 가능한 모델: "gpt3", "gpt4o", "opus", "haiku", "sonnet", "clova")
     :return: 번역된 텍스트
     """
     prompt = f"다음 텍스트를 {target_lang}로 번역해 주세요:\n\n{text}"
     translation = _run_model(prompt, model)
-    return translation
+    return translation
```

### Comparing `rocat-0.2.0/rocat/config.py` & `rocat-0.2.1/rocat/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # rocat/config.py
 import configparser
+import os
 
 _config_instance = None
 
 def load_config(config_file="config.ini"):
     """ 
     설정 파일을 로드하고, 설정 인스턴스를 반환합니다.
     
@@ -20,27 +21,32 @@
             _config_instance.read(config_file)
         except Exception as e:
             print(f"Error loading config file: {e}")
             _config_instance = None
     return _config_instance
 
 def get_api_key(service_name):
-    """ 
+    """
     지정된 서비스 이름에 대한 API 키를 설정에서 가져옵니다.
     
     Args:
         service_name (str): 서비스 이름.
     
     Returns:
-        str: API 키. 키가 없거나 로드되지 않은 설정의 경우 빈 문자열을 반환합니다.
+        str: API 키. 환경변수에서 가져오며, 설정 파일에도 없을 경우 빈 문자열을 반환합니다.
     """
-    config = load_config()
-    if config and "API_KEYS" in config:
-        return config["API_KEYS"].get(service_name, "")
-    return None
+    env_var_name = f"{service_name.upper()}_API_KEY"
+    api_key = os.getenv(env_var_name)
+    
+    if not api_key:
+        config = load_config()
+        if config and "API_KEYS" in config:
+            if service_name in ["openai", "anthropic", "serpapi", "naver_clovastudio", "naver_apigw"]:
+                return config["API_KEYS"].get(service_name, "")
+    return api_key or ""
 
 def save_config(config, config_file="config.ini"):
     """ 
     주어진 설정 객체를 파일에 저장합니다.
     
     Args:
         config (ConfigParser): 설정 객체.
@@ -59,11 +65,12 @@
     Args:
         config_file (str): 설정 파일의 경로. 기본값은 "config.ini"입니다.
     """
     config = configparser.ConfigParser()
     config["API_KEYS"] = {
         "openai": "",
         "anthropic": "",
-        "naver": "",
-        "serpapi": ""  
+        "serpapi": "",
+        "naver_clovastudio": "",
+        "naver_apigw": ""  
     }
-    save_config(config, config_file)
+    save_config(config, config_file)
```

### Comparing `rocat-0.2.0/rocat/file_utils.py` & `rocat-0.2.1/rocat/file_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # rocat/file_utils.py
 from openpyxl import load_workbook
 import xlrd
 import re
 import csv
-from PyPDF2 import PdfReader
+from pypdf import PdfReader
 import docx2txt
 import pptx
 import docx2txt
 from pptx import Presentation
 from olefile import OleFileIO
 import olefile
 import zlib
 import io
 import zipfile
 import xml.etree.ElementTree as ET
-import os
 import struct
-from openai import OpenAI
-from .config import get_api_key
 
 
 
 def get_txt(location, encoding='utf-8'):
     """ 
     텍스트 파일의 내용을 읽어옵니다.
     
@@ -252,15 +249,15 @@
     try:
         with open(file_path, 'r', encoding=encoding) as file:
             csv_reader = csv.reader(file, delimiter=delimiter)
             rows = [row for row in csv_reader]
             return rows
     except Exception as e:
         return f"ERROR: {str(e)}"
-
+    
 def get_pdf(file_path):
     """ 
     PDF 파일의 텍스트를 추출합니다.
     
     Args:
         file_path (str): 파일 경로.
     
@@ -366,28 +363,8 @@
                         tree = ET.parse(file)
                         root = tree.getroot()
                         for elem in root.iter():
                             if elem.text:
                                 text_parts.append(elem.text.strip())
     
    
-    return '\n'.join(text_parts)
-
-def get_whisper(audio_file):
-    """ 
-    오디오 파일을 Whisper API를 사용하여 텍스트로 변환합니다.
-    
-    Args:
-        audio_file (str): 오디오 파일 경로.
-    
-    Returns:
-        str: 변환된 텍스트.
-    """
-    api_key = get_api_key("openai")
-    client = OpenAI(api_key=api_key)
-    with open(audio_file, "rb") as file:
-        transcription = client.audio.transcriptions.create(
-            model="whisper-1",
-            file=file,
-            response_format="text"
-        )
-    return transcription
+    return '\n'.join(text_parts)
```

### Comparing `rocat-0.2.0/rocat/language_model.py` & `rocat-0.2.1/rocat/language_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,97 +1,78 @@
 # rocat/language_model.py
 from openai import OpenAI
+from rocat.config import get_api_key
+import requests
+import json
+import uuid
 import anthropic
 from .config import get_api_key
 from .language_utils import _convert_language_code
 
-def run_gpt(prompt, system_prompt="", temperature=0.7, top_p=1, max_tokens=1024, key=None):
-    """
-    OpenAI GPT-3.5 모델을 사용하여 주어진 프롬프트에 대한 응답을 생성합니다.
-    
-    Parameters:
-        prompt (str): 모델에 입력할 프롬프트.
-        system_prompt (str): 시스템 프롬프트, 대화의 맥락을 설정하는 데 사용됩니다 (옵션).
-        temperature (float): 생성의 무작위성을 결정하는 값.
-        top_p (float): 토큰 확률의 누적 분포 임곗값.
-        max_tokens (int): 생성할 최대 토큰 수.
-    
-    Returns:
-        str: 생성된 텍스트 응답.
-    """
-    key = get_api_key("openai")
-    client = OpenAI(api_key=key)
-    
-    messages = [{"role": "system", "content": system_prompt}] if system_prompt else []
-    
-    if isinstance(prompt, str):
-        prompt = [prompt]
-    
-    for p in prompt:
-        messages.append({"role": "user", "content": p})
-    
-    response = client.chat.completions.create(
-        model="gpt-3.5-turbo",
-        messages=messages,
-        max_tokens=max_tokens
-    )
-    
-    return response.choices[0].message.content
+MODEL_MAP = {
+    "gpt3": "gpt-3.5-turbo",
+    "gpt4o": "gpt-4o",
+    "opus": "claude-3-opus-20240229",
+    "haiku": "claude-3-haiku-20240307",
+    "sonnet": "claude-3-sonnet-20240229",
+    "clova": "HCX-003"
+}
 
-def run_gpt4( prompt, system_prompt="", key=None, temperature=0.7, top_p=1, max_tokens=1024):
+def run_model(model, prompt, system_prompt="", temperature=0.7, top_p=1, max_tokens=1024, output="default", lang="", tools=[]):
     """
-    OpenAI GPT-4 모델을 사용하여 주어진 프롬프트에 대한 응답을 생성합니다.
+    주어진 모델을 사용하여 프롬프트에 대한 응답을 생성합니다.
     
     Parameters:
+        model (str): 사용할 모델의 이름.
         prompt (str): 모델에 입력할 프롬프트.
         system_prompt (str): 시스템 프롬프트, 대화의 맥락을 설정하는 데 사용됩니다 (옵션).
         temperature (float): 생성의 무작위성을 결정하는 값.
         top_p (float): 토큰 확률의 누적 분포 임곗값.
         max_tokens (int): 생성할 최대 토큰 수.
+        output (str): 응답의 출력 형식 (default, word, sentence, bullet, json).
+        lang (str): 응답 언어 코드 (ISO 639-1).
+        tools (list): 사용할 도구 목록.
     
     Returns:
         str: 생성된 텍스트 응답.
     """
+    full_model_name = MODEL_MAP.get(model.lower())
+    if not full_model_name:
+        raise ValueError(f"Unknown model: {model}")
+    
+    if "gpt" in model.lower():
+        return _run_openai(full_model_name, prompt, system_prompt, temperature, top_p, max_tokens)
+    elif "claude" in full_model_name or "opus" in full_model_name or "haiku" in full_model_name or "sonnet" in full_model_name:
+        return _run_anthropic(full_model_name, prompt, system_prompt, temperature, top_p, max_tokens, output, lang, tools)
+    elif "clova" in model.lower():
+        return _run_clova(full_model_name, prompt, temperature, top_p, max_tokens)
+    else:
+        raise ValueError(f"Unknown model: {model}")
+
+def _run_openai(model, prompt, system_prompt="", temperature=0.7, top_p=1, max_tokens=1024):
     key = get_api_key("openai")
     client = OpenAI(api_key=key)
     
     messages = [{"role": "system", "content": system_prompt}] if system_prompt else []
     
     if isinstance(prompt, str):
         prompt = [prompt]
     
     for p in prompt:
         messages.append({"role": "user", "content": p})
     
     response = client.chat.completions.create(
-        model="gpt-4",
+        model=model,
         messages=messages,
         max_tokens=max_tokens
     )
     
     return response.choices[0].message.content
 
-def run_claude(prompt, model_name="claude-3-sonnet-20240229", system_prompt="", temperature=0.7, top_p=1, max_tokens=1024, output="default", lang="", tools=[]):
-    """
-    Anthropic의 Claude 모델을 사용하여 주어진 프롬프트에 대한 응답을 생성하고 특정 형식으로 출력합니다.
-
-    Parameters:
-        prompt (str or list of str): 모델에 입력할 프롬프트.
-        model_name (str): 사용할 Claude 모델의 이름.
-        system_prompt (str): 대화 컨텍스트를 위한 시스템 프롬프트 (옵션).
-        temperature (float): 생성의 무작위성을 결정하는 값.
-        top_p (float): 토큰 확률의 누적 분포 임곗값.
-        max_tokens (int): 생성할 최대 토큰 수.
-        output (str): 응답의 출력 형식 (default, word, sentence, bullet, json).
-        lang (str): 응답 언어 코드 (ISO 639-1).
-        tools (list): 사용할 도구 목록.
-
-    Returns:
-        str: 생성된 텍스트 응답. 여러 개의 텍스트 블록이 있을 경우 이를 연결하여 반환합니다.
-    """
+def _run_anthropic(model_name, prompt, system_prompt="", temperature=0.7, top_p=1, max_tokens=1024, output="default", lang="", tools=[]):
     key = get_api_key("anthropic")
     anth_client = anthropic.Anthropic(api_key=key)
     output_format = {
         "default": "",
         "word": " Don't explain, keep your output to very short one word.",
         "sentence": " Keep your output to very short one sentence.",
         "bullet": " Don't explain, keep your output in bullet points. Don't say anything else.",
@@ -118,57 +99,51 @@
             max_tokens=max_tokens,
             messages=messages,
             temperature=temperature,
             top_p=top_p
         )
         content = response.content
         return "\n".join([block.text for block in content if hasattr(block, 'text')])
-    else:
-        # Tool 처리 로직 추가
-        tool_format = [{
-            "name": tool[0],
-            "description": tool[1],
-            "input_schema": {
-                "type": "object",
-                "properties": {key: {"type": "string", "description": value} for key, value in tool[2].items()}
-            }
-        } for tool in tools]
 
-        response = anth_client.beta.tools.messages.create(
-            model=model_name,
-            max_tokens=max_tokens,
-            temperature=temperature,
-            tools=tool_format,
-            system=system_prompt,
-            messages=messages
-        )
-        # 도구 사용 결과 처리 로직 추가
-        content = response.content
-        return "\n".join([block.text for block in content if hasattr(block, 'text')])
-
-
-def run_opus(prompt, system_prompt="", temperature=0.7, top_p=1, max_tokens=1024):
-    """
-    Anthropic의 Claude-3-Opus 모델을 사용하여 주어진 프롬프트에 대한 응답을 생성합니다.
-    이 함수는 run_claude 함수의 특정 모델을 사용하는 버전입니다.
+def _run_clova(model, prompt, temperature=0.7, top_p=0.8, max_tokens=256):
+    host = 'https://clovastudio.stream.ntruss.com'
     
-    Parameters와 Returns는 run_claude 함수와 동일합니다.
-    """
-    return run_claude(prompt, model_name="claude-3-opus-20240229", system_prompt=system_prompt, temperature=temperature, top_p=top_p, max_tokens=max_tokens)
-
-def run_haiku(prompt, system_prompt="", temperature=0.7, top_p=1, max_tokens=1024):
-    """
-    Anthropic의 Claude-3-Haiku 모델을 사용하여 주어진 프롬프트에 대한 응답을 생성합니다.
-    이 함수는 run_claude 함수의 특정 모델을 사용하는 버전입니다.
+    api_key = get_api_key("naver_clovastudio")
+    api_key_primary_val = get_api_key("naver_apigw")
     
-    Parameters와 Returns는 run_claude 함수와 동일합니다.
-    """
-    return run_claude(prompt, model_name="claude-3-haiku-20240307", system_prompt=system_prompt, temperature=temperature, top_p=top_p, max_tokens=max_tokens)
+    request_id = str(uuid.uuid4())
 
-def run_sonnet(prompt, system_prompt="", temperature=0.7, top_p=1, max_tokens=1024):
-    """
-    Anthropic의 Claude-3-Sonnet 모델을 사용하여 주어진 프롬프트에 대한 응답을 생성합니다.
-    이 함수는 run_claude 함수의 특정 모델을 사용하는 버전입니다.
-    
-    Parameters와 Returns는 run_claude 함수와 동일합니다.
-    """
-    return run_claude(prompt, model_name="claude-3-sonnet-20240229", system_prompt=system_prompt, temperature=temperature, top_p=top_p, max_tokens=max_tokens)
+    headers = {
+        'X-NCP-CLOVASTUDIO-API-KEY': api_key,
+        'X-NCP-APIGW-API-KEY': api_key_primary_val,
+        'X-NCP-CLOVASTUDIO-REQUEST-ID': request_id,
+        'Content-Type': 'application/json; charset=utf-8',
+        'Accept': 'text/event-stream'
+    }
+
+    request_data = {
+        'messages': [{"role": "user", "content": prompt}],
+        'topP': top_p,
+        'topK': 0,
+        'maxTokens': max_tokens,
+        'temperature': temperature,
+        'repeatPenalty': 5.0,
+        'stopBefore': [],
+        'includeAiFilters': True,
+        'seed': 0
+    }
+
+    with requests.post(host + f'/testapp/v1/chat-completions/{model}',
+                       headers=headers, json=request_data, stream=True) as r:
+        content = ""
+        for line in r.iter_lines():
+            if line:
+                decoded_line = line.decode("utf-8")
+                if "data:" in decoded_line:
+                    _, data = decoded_line.split("data:")
+                    data = data.strip()
+                    if data != "[DONE]":
+                        event_data = json.loads(data)
+                        if "message" in event_data:
+                            content += event_data["message"]["content"]
+        
+        return content.strip()
```

### Comparing `rocat-0.2.0/rocat/language_utils.py` & `rocat-0.2.1/rocat/language_utils.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.0/rocat/template_utils.py` & `rocat-0.2.1/rocat/template_utils.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.0/rocat/web_utils.py` & `rocat-0.2.1/rocat/web_utils.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.0/rocat.egg-info/PKG-INFO` & `rocat-0.2.1/rocat.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocat
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple and user-friendly library for AI services
 Home-page: https://github.com/Yumeta-Lab/rocat-dev
 Author: YumetaLab
 Author-email: root@yumeta.kr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: docx2txt==0.8
 Requires-Dist: google_search_results==2.4.2
 Requires-Dist: openai==1.30.3
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: pandas==2.2.2
 Requires-Dist: pillow==10.3.0
-Requires-Dist: PyPDF2==3.0.1
+Requires-Dist: pypdf==4.2.0
 Requires-Dist: python-docx==1.1.2
 Requires-Dist: python-pptx==0.6.23
 Requires-Dist: requests==2.32.2
 Requires-Dist: serpapi==0.1.5
 Requires-Dist: xlrd==2.0.1
 Requires-Dist: XlsxWriter==3.2.0
 Requires-Dist: youtube-transcript-api==0.6.2
@@ -33,146 +33,152 @@
 
 RoCat is a Python library that provides a simple and user-friendly interface for integrating AI services into your projects. It supports various AI functionalities such as text summarization, YouTube transcript retrieval, audio transcription using OpenAI's Whisper, and web search using SerpAPI.
 
 ## Installation
 
 You can install RoCat using pip:
 
-​```bash
+~~~bash
 pip install rocat
-​```
+~~~
 
 ## Quick Start Guide
 
-1. Initialize RoCat: Begin by creating a default configuration and example code to get started.
+1. **Initialize RoCat**: Begin by creating a default configuration and example code to get started.
 
-```bash
-(.venv) > rocat init 
+~~~bash
+rocat init
 
 Default configuration file and example code created.
-- config.ini      
+- config.ini
 - rocat_example.py
-```
+~~~
 
 This command creates a default configuration file (config.ini) and an example script (rocat_example.py).
 
-2. Edit Configuration: Open config.ini to add your API keys.
+2. **Edit Configuration**: Open config.ini to add your API keys.
 
-```bash
+~~~ini
 [API_KEYS]
 openai = 
 anthropic = 
-naver = 
 serpapi =
-```
+naver_clovastudio =
+naver_apigw =
+~~~
 
-3. Now write your code! You can refer to the rocat_example.py file for sample usage of the library.
+3. **Write Your Code**: You can refer to the rocat_example.py file for sample usage of the library.
 
-```python
+~~~python
 # rocat_example.py
 import rocat as rc
 
 def main():
     # Initialize the library
     rc.initialize()
     
     # Write your code here.
 
 if __name__ == "__main__":
     main()
-```
+~~~
 
 ## Example Usage
 
 ### Text Summarization
-```python
+
+~~~python
 def main():
     rc.initialize()
     
-    # Get text from a web page  
-    url = "https://www.example.com/sample-page"  
-    text = rc.get_web(url)  
-
-    # Summarize the text  
+    # Get text from a web page
+    url = "https://www.example.com/sample-page"
+    text = rc.get_web(url)
+    
+    # Summarize the text
     summary = rc.ai_summarize(text, 3)
-
-
-    # Print the summarized text  
-    print("\nAI Summary Test:")  
+    
+    # Print the summarized text
+    print("\nAI Summary Test:")
     print(summary)
 
 if __name__ == "__main__":
     main()
-```
+~~~
 
 ### YouTube Transcript Retrieval
-```python
+
+~~~python
 def main():
     rc.initialize()
     
-    # Get captions from a YouTube video  
-    video_url = "https://www.youtube.com/watch?v=example-video-id"  
-    transcript = rc.get_youtube(video_url)  
-
-    # Print the caption text  
-    print("\nYouTube Caption Test:")  
-    print(transcript)  
+    # Get captions from a YouTube video
+    video_url = "https://www.youtube.com/watch?v=example-video-id"
+    transcript = rc.get_youtube(video_url)
+    
+    # Print the caption text
+    print("\nYouTube Caption Test:")
+    print(transcript)
 
 if __name__ == "__main__":
     main()
-```
+~~~
 
+### Audio Transcription
 
-### Audio Transcription 
-```python
+~~~python
 def main():
     rc.initialize()
     
-    # Convert an audio file to text  
-    audio_file = "path/to/example/audio.mp3"  
-    transcription = rc.get_whisper(audio_file)  
-
-    # Print the converted text  
-    print("\nWhisper Recognition :")  
-    print(transcription)  
+    # Convert an audio file to text
+    audio_file = "path/to/example/audio.mp3"
+    transcription = rc.get_whisper(audio_file)
+    
+    # Print the converted text
+    print("\nWhisper Recognition:")
+    print(transcription)
 
 if __name__ == "__main__":
     main()
-```
+~~~
 
 ### Web Search
-```python
+
+~~~python
 def main():
     rc.initialize()
     
-    # Get google search results  
-    query = "python"  
-    search_results = rc.get_search(query)  
-    for result in search_results:  
-        print(f"Title: {result['title']}")  
-        print(f"Link: {result['link']}")  
+    # Get Google search results
+    query = "python"
+    search_results = rc.get_search(query)
+    for result in search_results:
+        print(f"Title: {result['title']}")
+        print(f"Link: {result['link']}")
         print(f"Snippet: {result['snippet']}")
 
 if __name__ == "__main__":
     main()
-```
+~~~
 
 ## Features
 
 - Text summarization using AI
 - YouTube transcript retrieval
 - Audio transcription using OpenAI's Whisper
 - Web search using SerpAPI
 - File utilities for handling various file formats (txt, xls, xlsx, doc, docx, ppt, pptx, csv, pdf, hwp, hwpx)
 - Language model integration (GPT-3.5, GPT-4, Claude, Opus, Haiku, Sonnet)
 
 ## License
+
 This project is licensed under the MIT License. See the LICENSE file for more information.
 
 ## Contributing
+
 Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the GitHub repository.
 
 ## Contact
+
 If you have any questions or inquiries, please contact the author:
 
 - Name: Faith6
 - Email: root@yumeta.kr
```

### Comparing `rocat-0.2.0/setup.py` & `rocat-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="rocat",
-    version="0.2.0",
+    version="0.2.1",
     description="A simple and user-friendly library for AI services",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="YumetaLab",
     author_email="root@yumeta.kr",
     url="https://github.com/Yumeta-Lab/rocat-dev",
     packages=find_packages(exclude=["tests"]),
@@ -20,15 +20,15 @@
         "beautifulsoup4==4.12.3",
         "docx2txt==0.8",
         "google_search_results==2.4.2",
         "openai==1.30.3",
         "openpyxl==3.1.2",
         "pandas==2.2.2",
         "pillow==10.3.0",
-        "PyPDF2==3.0.1",
+        "pypdf==4.2.0",
         "python-docx==1.1.2",
         "python-pptx==0.6.23",
         "requests==2.32.2",
         "serpapi==0.1.5",
         "xlrd==2.0.1",
         "XlsxWriter==3.2.0",
         "youtube-transcript-api==0.6.2",
```

### Comparing `rocat-0.2.0/tests/test_web_utils.py` & `rocat-0.2.1/tests/test_web_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 # tests/test_web_utils.py
-import os
 import pytest
+from unittest.mock import patch, mock_open, MagicMock
 from rocat.web_utils import get_web, get_youtube, get_search
-from rocat.file_utils import get_whisper
+from rocat.audio_utils import get_whisper
 
 def test_get_web():
     url = "https://www.naver.com"
     text = get_web(url)
     html = get_web(url, type="html")
     
     assert isinstance(text, str)
     assert len(text) > 0
     
     assert html.find("h1") is not None
     
     with pytest.raises(ValueError):
         get_web(url, type="invalid")
 
-def test_get_youtube():
+@patch('rocat.web_utils.YouTubeTranscriptApi.get_transcript')
+def test_get_youtube(mock_get_transcript):
+    mock_get_transcript.return_value = [{'text': 'This is a test transcript.'}]
     url = "https://www.youtube.com/watch?v=mQG7vN8UYLU"
     transcript = get_youtube(url)
     
     assert isinstance(transcript, str)
-    assert len(transcript) > 0
+    assert "This is a test transcript." in transcript
+    mock_get_transcript.assert_called_once()
 
-def test_get_whisper():
-    audio_file = "tests/test.mp3"
-    transcription = get_whisper(audio_file)
-    
-    assert isinstance(transcription, str)
-    assert len(transcription) > 0
 
-def test_get_search():
+@patch('rocat.web_utils.GoogleSearch.get_dict')
+def test_get_search(mock_get_dict):
+    mock_get_dict.return_value = {
+        "organic_results": [
+            {"title": "Python programming", "link": "http://example.com", "snippet": "Python is a programming language."}
+        ]
+    }
     query = "Python programming language"
     results = get_search(query)
     
     assert isinstance(results, list)
     assert len(results) > 0
     assert "title" in results[0]
     assert "link" in results[0]
     assert "snippet" in results[0]
+
+if __name__ == "__main__":
+    pytest.main()
```

