# Comparing `tmp/csm_ai-0.1.1.tar.gz` & `tmp/csm_ai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csm_ai-0.1.1.tar", last modified: Fri May 24 17:57:58 2024, max compression
+gzip compressed data, was "csm_ai-0.1.2.tar", last modified: Sun Jun  2 21:15:55 2024, max compression
```

## Comparing `csm_ai-0.1.1.tar` & `csm_ai-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rfeinman   (501) staff       (20)        0 2024-05-24 17:57:58.806795 csm_ai-0.1.1/
--rw-r--r--   0 rfeinman   (501) staff       (20)    11357 2024-05-15 14:49:42.000000 csm_ai-0.1.1/LICENSE
--rw-r--r--   0 rfeinman   (501) staff       (20)     1532 2024-05-24 17:57:58.806557 csm_ai-0.1.1/PKG-INFO
--rw-r--r--   0 rfeinman   (501) staff       (20)     1093 2024-05-24 17:40:36.000000 csm_ai-0.1.1/README.md
--rw-r--r--   0 rfeinman   (501) staff       (20)       97 2024-05-13 17:46:38.000000 csm_ai-0.1.1/pyproject.toml
--rw-r--r--   0 rfeinman   (501) staff       (20)       38 2024-05-24 17:57:58.806847 csm_ai-0.1.1/setup.cfg
--rw-r--r--   0 rfeinman   (501) staff       (20)      964 2024-05-21 14:48:20.000000 csm_ai-0.1.1/setup.py
-drwxr-xr-x   0 rfeinman   (501) staff       (20)        0 2024-05-24 17:57:58.804324 csm_ai-0.1.1/src/
-drwxr-xr-x   0 rfeinman   (501) staff       (20)        0 2024-05-24 17:57:58.805452 csm_ai-0.1.1/src/csm/
--rw-r--r--   0 rfeinman   (501) staff       (20)       78 2024-05-20 19:48:44.000000 csm_ai-0.1.1/src/csm/__init__.py
--rw-r--r--   0 rfeinman   (501) staff       (20)    14899 2024-05-24 17:41:13.000000 csm_ai-0.1.1/src/csm/client.py
--rw-r--r--   0 rfeinman   (501) staff       (20)       21 2024-05-24 17:55:04.000000 csm_ai-0.1.1/src/csm/version.py
-drwxr-xr-x   0 rfeinman   (501) staff       (20)        0 2024-05-24 17:57:58.806273 csm_ai-0.1.1/src/csm_ai.egg-info/
--rw-r--r--   0 rfeinman   (501) staff       (20)     1532 2024-05-24 17:57:58.000000 csm_ai-0.1.1/src/csm_ai.egg-info/PKG-INFO
--rw-r--r--   0 rfeinman   (501) staff       (20)      267 2024-05-24 17:57:58.000000 csm_ai-0.1.1/src/csm_ai.egg-info/SOURCES.txt
--rw-r--r--   0 rfeinman   (501) staff       (20)        1 2024-05-24 17:57:58.000000 csm_ai-0.1.1/src/csm_ai.egg-info/dependency_links.txt
--rw-r--r--   0 rfeinman   (501) staff       (20)       16 2024-05-24 17:57:58.000000 csm_ai-0.1.1/src/csm_ai.egg-info/requires.txt
--rw-r--r--   0 rfeinman   (501) staff       (20)        4 2024-05-24 17:57:58.000000 csm_ai-0.1.1/src/csm_ai.egg-info/top_level.txt
+drwxr-xr-x   0 rfeinman   (501) staff       (20)        0 2024-06-02 21:15:55.485953 csm_ai-0.1.2/
+-rw-r--r--   0 rfeinman   (501) staff       (20)    11357 2024-05-15 14:49:42.000000 csm_ai-0.1.2/LICENSE
+-rw-r--r--   0 rfeinman   (501) staff       (20)     1425 2024-06-02 21:15:55.485773 csm_ai-0.1.2/PKG-INFO
+-rw-r--r--   0 rfeinman   (501) staff       (20)      986 2024-06-02 21:11:46.000000 csm_ai-0.1.2/README.md
+-rw-r--r--   0 rfeinman   (501) staff       (20)       97 2024-05-13 17:46:38.000000 csm_ai-0.1.2/pyproject.toml
+-rw-r--r--   0 rfeinman   (501) staff       (20)       38 2024-06-02 21:15:55.485985 csm_ai-0.1.2/setup.cfg
+-rw-r--r--   0 rfeinman   (501) staff       (20)      964 2024-05-21 14:48:20.000000 csm_ai-0.1.2/setup.py
+drwxr-xr-x   0 rfeinman   (501) staff       (20)        0 2024-06-02 21:15:55.483811 csm_ai-0.1.2/src/
+drwxr-xr-x   0 rfeinman   (501) staff       (20)        0 2024-06-02 21:15:55.484864 csm_ai-0.1.2/src/csm/
+-rw-r--r--   0 rfeinman   (501) staff       (20)      111 2024-06-02 21:11:46.000000 csm_ai-0.1.2/src/csm/__init__.py
+-rw-r--r--   0 rfeinman   (501) staff       (20)    16068 2024-06-02 21:11:46.000000 csm_ai-0.1.2/src/csm/client.py
+-rw-r--r--   0 rfeinman   (501) staff       (20)       21 2024-06-02 21:13:32.000000 csm_ai-0.1.2/src/csm/version.py
+drwxr-xr-x   0 rfeinman   (501) staff       (20)        0 2024-06-02 21:15:55.485607 csm_ai-0.1.2/src/csm_ai.egg-info/
+-rw-r--r--   0 rfeinman   (501) staff       (20)     1425 2024-06-02 21:15:55.000000 csm_ai-0.1.2/src/csm_ai.egg-info/PKG-INFO
+-rw-r--r--   0 rfeinman   (501) staff       (20)      267 2024-06-02 21:15:55.000000 csm_ai-0.1.2/src/csm_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 rfeinman   (501) staff       (20)        1 2024-06-02 21:15:55.000000 csm_ai-0.1.2/src/csm_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 rfeinman   (501) staff       (20)       16 2024-06-02 21:15:55.000000 csm_ai-0.1.2/src/csm_ai.egg-info/requires.txt
+-rw-r--r--   0 rfeinman   (501) staff       (20)        4 2024-06-02 21:15:55.000000 csm_ai-0.1.2/src/csm_ai.egg-info/top_level.txt
```

### Comparing `csm_ai-0.1.1/LICENSE` & `csm_ai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `csm_ai-0.1.1/setup.py` & `csm_ai-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `csm_ai-0.1.1/src/csm/client.py` & `csm_ai-0.1.2/src/csm/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import time
 import warnings
 from urllib.request import urlretrieve
+from dataclasses import dataclass
 import requests
 import base64
 from io import BytesIO
 from PIL import Image
 
 
 class BackendClient:
@@ -67,14 +68,15 @@
             diffusion_time_steps=75,
             ## refine args
             pixel_alignment="highest",
             model_resolution="high",
             polygon_count="high_poly",
             topology="tris",
             texture_resolution=2048,
+            scaled_bbox=(1.0, 1.0, 1.0),
         ):
         assert preview_mesh in ["turbo", "hd"]
         assert 16 <= diffusion_time_steps <= 200
         assert pixel_alignment in ["lowest", "highest"]
         assert model_resolution in ["low", "high"]
         assert polygon_count in ["low_poly", "high_poly"]
         assert topology in ["tris", "quads"]
@@ -88,14 +90,15 @@
             "model_resolution": model_resolution,
             "resolution": polygon_count,
             "diffusion_time_steps": diffusion_time_steps,
             "auto_gen_3d": auto_gen_3d,
             "topology": topology,
             "texture_resolution": texture_resolution,
             "manual_segmentation": False,  # TODO: implement this option
+            "scaled_bbox": [float(s) for s in scaled_bbox],
         }
 
         response = requests.post(
             url=f"{self.base_url}/image-to-3d-sessions",
             json=parameters,
             headers=self.headers,
         )
@@ -116,24 +119,25 @@
         response = requests.post(
             url=f"{self.base_url}/image-to-3d-sessions/get-3d/refine/{session_code}",
             headers=self.headers,
         )
 
         return response.json()
     
-    def get_3d_preview(self, session_code, spin_url=None):
+    def get_3d_preview(self, session_code, spin_url=None, scaled_bbox=(1.0, 1.0, 1.0)):
         selected_spin_index = 0
 
         if spin_url is None:
             result = self.get_image_to_3d_session_info(session_code)
             spin_url = result['data']['spins'][selected_spin_index]["image_url"]
 
         parameters = {
             "selected_spin_index": selected_spin_index,
             "selected_spin": spin_url,
+            "scaled_bbox": [float(s) for s in scaled_bbox],
         }
 
         response = requests.post(
             url=f"{self.base_url}/image-to-3d-sessions/get-3d/preview/{session_code}",
             json=parameters,
             headers=self.headers,
             timeout=100,
@@ -172,14 +176,51 @@
             headers=self.headers,
         )
         self._check_http_response(response)
 
         return response.json()
 
 
+@dataclass
+class ImageTo3DResult:
+    r"""
+    Output class for image-to-3d generation.
+
+    Parameters
+    ----------
+    session_code : str
+        The image-to-3d session code.
+    mesh_path : str
+        Local path of the generated mesh file.
+    """
+
+    session_code: str
+    mesh_path: str
+
+
+@dataclass
+class TextTo3DResult:
+    r"""
+    Output class for text-to-3d generation.
+
+    Parameters
+    ----------
+    session_code : str
+        The image-to-3d session code.
+    mesh_path : str
+        Local path of the generated mesh file.
+    image_path : str
+        Local path of the image generated as part of text-to-3d.
+    """
+
+    session_code: str
+    mesh_path: str
+    image_path: str
+
+
 class CSMClient:
     r"""Core client utility for accessing the CSM API.
 
     Parameters
     ----------
     api_key : str, optional
         API key for the CSM account you would like to use. If not provided,
@@ -216,29 +257,30 @@
             *,
             generate_spin_video=False,
             diffusion_time_steps=75,
             mesh_format='obj',
             output='./',
             timeout=200,
             verbose=True,
+            scaled_bbox=(1.0, 1.0, 1.0),
         ):
         r"""Generate a 3D mesh from an image.
 
         The input image can be provided as a URL, a local path, or a :class:`PIL.Image`.
 
         Parameters
         ----------
         image : str or Image
             The input image. May be provided as a url, a local path, or a
             :class:`Image` instance.
 
         Returns
         -------
-        mesh_path : str
-            Local path of the resulting mesh file.
+        ImageTo3DResult
+            Result object. Contains the local path of the generated mesh file.
         """
         if generate_spin_video:
             warnings.warn(
                 "The option `generate_spin_video=True` is deprecated and will be removed "
                 "in a future release", DeprecationWarning)
 
         mesh_format = mesh_format.lower()
@@ -255,14 +297,15 @@
         # initialize session
         result = self.backend.create_image_to_3d_session(
             image_url,
             preview_mesh="turbo",
             generate_preview_mesh=not generate_spin_video,
             diffusion_time_steps=diffusion_time_steps,
             auto_gen_3d=False,
+            scaled_bbox=scaled_bbox,
         )
 
         status = result['data']['status']
         if (generate_spin_video and status != "spin_generate_processing") or (not generate_spin_video and status != "training_preview"):
             raise RuntimeError(f"Image-to-3d session creation failed (status='{status}')")
 
         session_code = result['data']['session_code']
@@ -302,14 +345,15 @@
             spin_path = os.path.join(output, 'spin.mp4')
             urlretrieve(spin_url, spin_path)
 
             # launch preview mesh export
             result = self.backend.get_3d_preview(
                 session_code,
                 spin_url=spin_url,
+                scaled_bbox=scaled_bbox,
             )
             step_label = "mesh export"
 
         if verbose:
             print(f'[INFO] Running preview {step_label}...')
 
         # wait for preview mesh export to complete (20-30s)
@@ -344,15 +388,15 @@
             mesh_file = 'mesh.usdz'
         else:
             raise ValueError(f"Encountered unexpected mesh_format value ('{mesh_format}').")
 
         mesh_path = os.path.join(output, mesh_file)  # TODO: os.path.abspath ?
         urlretrieve(mesh_url, mesh_path)
 
-        return mesh_path
+        return ImageTo3DResult(session_code=session_code, mesh_path=mesh_path)
 
     def text_to_3d(
             self,
             prompt,
             *,
             style_id="",
             guidance=6,
@@ -368,19 +412,17 @@
         Parameters
         ----------
         prompt : str
             The input text prompt.
 
         Returns
         -------
-        mesh_path : str
-            Local path of the resulting mesh file.
-        image_path : str
-            Local path of the image that was generated as part of the
-            text-to-3d pipeline.
+        TextTo3DResult
+            Result object. Contains the local path of the generated mesh file,
+            as well as the image that was generated as part of the pipeline.
         """
         os.makedirs(output, exist_ok=True)
 
         # initialize text-to-image session
         result = self.backend.create_text_to_image_session(
             prompt,
             style_id=style_id,
@@ -419,25 +461,25 @@
         image_url = result['data']['image_url']
 
         # download image
         image_path = os.path.join(output, 'image.png')
         urlretrieve(image_url, image_path)
 
         # launch image-to-3d
-        mesh_path = self.image_to_3d(
+        i23 = self.image_to_3d(
             image_url,
             generate_spin_video=generate_spin_video,
             diffusion_time_steps=diffusion_time_steps,
             mesh_format=mesh_format,
             output=output,
             timeout=timeout,
             verbose=verbose
         )
 
-        return mesh_path, image_path
+        return TextTo3DResult(session_code=i23.session_code, mesh_path=i23.mesh_path, image_path=image_path)
 
 
 def pil_image_to_x64(image: Image.Image) -> str:
     """PIL.Image.Image to base64"""
     buffer = BytesIO()
     image.save(buffer, "PNG")
     x64 = buffer.getvalue()
```

