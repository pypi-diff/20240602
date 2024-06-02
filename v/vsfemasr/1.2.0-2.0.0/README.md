# Comparing `tmp/vsfemasr-1.2.0-py3-none-any.whl.zip` & `tmp/vsfemasr-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 22391 bytes, number of entries: 12
--rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsfemasr/FeMaSR_SRX2_model_g.pth
--rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsfemasr/FeMaSR_SRX4_model_g.pth
--rw-r--r--  2.0 fat     9185 b- defN 20-Feb-02 00:00 vsfemasr/__init__.py
--rw-r--r--  2.0 fat      876 b- defN 20-Feb-02 00:00 vsfemasr/__main__.py
+Zip file size: 22614 bytes, number of entries: 13
+-rw-r--r--  2.0 fat     8154 b- defN 20-Feb-02 00:00 vsfemasr/__init__.py
+-rw-r--r--  2.0 fat      886 b- defN 20-Feb-02 00:00 vsfemasr/__main__.py
 -rw-r--r--  2.0 fat     3362 b- defN 20-Feb-02 00:00 vsfemasr/fema_utils.py
--rw-r--r--  2.0 fat    13300 b- defN 20-Feb-02 00:00 vsfemasr/femasr_arch.py
--rw-r--r--  2.0 fat    20109 b- defN 20-Feb-02 00:00 vsfemasr/network_swinir.py
+-rw-r--r--  2.0 fat    13215 b- defN 20-Feb-02 00:00 vsfemasr/femasr_arch.py
+-rw-r--r--  2.0 fat    17189 b- defN 20-Feb-02 00:00 vsfemasr/interpolate.py
+-rw-r--r--  2.0 fat    19854 b- defN 20-Feb-02 00:00 vsfemasr/network_swinir.py
 -rw-r--r--  2.0 fat     6213 b- defN 20-Feb-02 00:00 vsfemasr/vgg_arch.py
-?rw-r--r--  2.0 fat     9924 b- defN 20-Feb-02 00:00 vsfemasr-1.2.0.dist-info/METADATA
-?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 vsfemasr-1.2.0.dist-info/WHEEL
-?rw-r--r--  2.0 fat     7169 b- defN 20-Feb-02 00:00 vsfemasr-1.2.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 fat      953 b- defN 20-Feb-02 00:00 vsfemasr-1.2.0.dist-info/RECORD
-12 files, 71178 bytes uncompressed, 20797 bytes compressed:  70.8%
+-rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsfemasr/models/FeMaSR_SRX2_model_g.pth
+-rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsfemasr/models/FeMaSR_SRX4_model_g.pth
+?rw-r--r--  2.0 fat     1885 b- defN 20-Feb-02 00:00 vsfemasr-2.0.0.dist-info/METADATA
+?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 vsfemasr-2.0.0.dist-info/WHEEL
+?rw-r--r--  2.0 fat     7169 b- defN 20-Feb-02 00:00 vsfemasr-2.0.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 fat     1048 b- defN 20-Feb-02 00:00 vsfemasr-2.0.0.dist-info/RECORD
+13 files, 79062 bytes uncompressed, 20870 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -1,37 +1,40 @@
-Filename: vsfemasr/FeMaSR_SRX2_model_g.pth
-Comment: 
-
-Filename: vsfemasr/FeMaSR_SRX4_model_g.pth
-Comment: 
-
 Filename: vsfemasr/__init__.py
 Comment: 
 
 Filename: vsfemasr/__main__.py
 Comment: 
 
 Filename: vsfemasr/fema_utils.py
 Comment: 
 
 Filename: vsfemasr/femasr_arch.py
 Comment: 
 
+Filename: vsfemasr/interpolate.py
+Comment: 
+
 Filename: vsfemasr/network_swinir.py
 Comment: 
 
 Filename: vsfemasr/vgg_arch.py
 Comment: 
 
-Filename: vsfemasr-1.2.0.dist-info/METADATA
+Filename: vsfemasr/models/FeMaSR_SRX2_model_g.pth
+Comment: 
+
+Filename: vsfemasr/models/FeMaSR_SRX4_model_g.pth
+Comment: 
+
+Filename: vsfemasr-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: vsfemasr-1.2.0.dist-info/WHEEL
+Filename: vsfemasr-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: vsfemasr-1.2.0.dist-info/licenses/LICENSE
+Filename: vsfemasr-2.0.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: vsfemasr-1.2.0.dist-info/RECORD
+Filename: vsfemasr-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vsfemasr/__init__.py

```diff
@@ -1,225 +1,204 @@
 from __future__ import annotations
 
 import math
 import os
+import warnings
+from enum import IntEnum
 from threading import Lock
 
 import numpy as np
-import tensorrt
 import torch
 import torch.nn.functional as F
 import vapoursynth as vs
-from functorch.compile import memory_efficient_fusion
-from torch_tensorrt.fx import LowerSetting
-from torch_tensorrt.fx.lower import Lowerer
-from torch_tensorrt.fx.utils import LowerPrecision
 
-from .femasr_arch import FeMaSRNet, VectorQuantizer
+from .femasr_arch import FeMaSRNet
 
-__version__ = "1.2.0"
+__version__ = "2.0.0"
 
 os.environ["CUDA_MODULE_LOADING"] = "LAZY"
 
-package_dir = os.path.dirname(os.path.realpath(__file__))
+warnings.filterwarnings("ignore", "At pre-dispatch tracing")
+warnings.filterwarnings("ignore", "Attempted to insert a get_attr Node with no underlying reference")
+warnings.filterwarnings("ignore", "Node _run_on_acc_0_engine target _run_on_acc_0_engine _run_on_acc_0_engine of")
+warnings.filterwarnings("ignore", "The given NumPy array is not writable")
+
+model_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "models")
+
+
+class FeMaSRModel(IntEnum):
+    FeMaSR_SRX2_model_g = 0
+    FeMaSR_SRX4_model_g = 1
 
 
 @torch.inference_mode()
 def femasr(
     clip: vs.VideoNode,
-    device_index: int | None = None,
+    device_index: int = 0,
     num_streams: int = 1,
-    nvfuser: bool = False,
-    cuda_graphs: bool = False,
+    model: FeMaSRModel = FeMaSRModel.FeMaSR_SRX2_model_g,
     trt: bool = False,
-    trt_min_subgraph_size: int = 1,
-    trt_max_workspace_size: int = 1 << 25,
-    trt_cache_path: str = package_dir,
-    model: int = 0,
+    trt_debug: bool = False,
+    trt_workspace_size: int = 0,
+    trt_max_aux_streams: int | None = None,
+    trt_optimization_level: int | None = None,
+    trt_cache_dir: str = model_dir,
 ) -> vs.VideoNode:
     """Real-World Blind Super-Resolution via Feature Matching with Implicit High-Resolution Priors
 
     :param clip:                    Clip to process. Only RGBH and RGBS formats are supported.
                                     RGBH performs inference in FP16 mode while RGBS performs inference in FP32 mode.
     :param device_index:            Device ordinal of the GPU.
     :param num_streams:             Number of CUDA streams to enqueue the kernels.
-    :param nvfuser:                 Enable fusion through nvFuser. Not allowed in TensorRT. (experimental)
-    :param cuda_graphs:             Use CUDA Graphs to remove CPU overhead associated with launching CUDA kernels
-                                    sequentially. Not allowed in TensorRT.
-    :param trt:                     Use TensorRT for high-performance inference.
-    :param trt_min_subgraph_size:   Minimum node size in a subgraph after splitting. Subgraphs with smaller size will
-                                    fall back to CUDA. Try trt_min_subgraph_size=5 if TensorRT engine cannot be built
-                                    due to insufficient VRAM, but the performance will degrade.
-    :param trt_max_workspace_size:  Maximum workspace size for TensorRT engine.
-    :param trt_cache_path:          Path for TensorRT engine file. Engine will be cached when it's built for the first
-                                    time. Note each engine is created for specific settings such as model path/name,
-                                    precision, workspace etc, and specific GPUs and it's not portable.
     :param model:                   Model to use.
-                                    0 = FeMaSR_SRX2_model_g
-                                    1 = FeMaSR_SRX4_model_g
+    :param trt:                     Use TensorRT for high-performance inference.
+    :param trt_debug:               Print out verbose debugging information.
+    :param trt_workspace_size:      Size constraints of workspace memory pool.
+    :param trt_max_aux_streams:     Maximum number of auxiliary streams per inference stream that TRT is allowed to use
+                                    to run kernels in parallel if the network contains ops that can run in parallel,
+                                    with the cost of more memory usage. Set this to 0 for optimal memory usage.
+                                    (default = using heuristics)
+    :param trt_optimization_level:  Builder optimization level. Higher level allows TensorRT to spend more building time
+                                    for more optimization options. Valid values include integers from 0 to the maximum
+                                    optimization level, which is currently 5. (default is 3)
+    :param trt_cache_dir:           Directory for TensorRT engine file. Engine will be cached when it's built for the
+                                    first time. Note each engine is created for specific settings such as model
+                                    path/name, precision, workspace etc, and specific GPUs and it's not portable.
     """
     if not isinstance(clip, vs.VideoNode):
         raise vs.Error("femasr: this is not a clip")
 
-    if clip.format.id not in (vs.RGBH, vs.RGBS):
+    if clip.format.id not in [vs.RGBH, vs.RGBS]:
         raise vs.Error("femasr: only RGBH and RGBS formats are supported")
 
     if not torch.cuda.is_available():
         raise vs.Error("femasr: CUDA is not available")
 
     if num_streams < 1:
         raise vs.Error("femasr: num_streams must be at least 1")
 
-    if num_streams > vs.core.num_threads:
-        raise vs.Error("femasr: setting num_streams greater than `core.num_threads` is useless")
+    if model not in FeMaSRModel:
+        raise vs.Error("femasr: model must be one of the members in FeMaSRModel")
 
-    if trt:
-        if nvfuser:
-            raise vs.Error("femasr: nvfuser and trt are mutually exclusive")
-
-        if cuda_graphs:
-            raise vs.Error("femasr: cuda_graphs and trt are mutually exclusive")
-
-    if model not in range(2):
-        raise vs.Error("femasr: model must be 0 or 1")
-
-    if os.path.getsize(os.path.join(package_dir, "FeMaSR_SRX2_model_g.pth")) == 0:
+    if os.path.getsize(os.path.join(model_dir, "FeMaSR_SRX2_model_g.pth")) == 0:
         raise vs.Error("femasr: model files have not been downloaded. run 'python -m vsfemasr' first")
 
     torch.set_float32_matmul_precision("high")
 
     fp16 = clip.format.bits_per_sample == 16
     dtype = torch.half if fp16 else torch.float
 
     device = torch.device("cuda", device_index)
 
     stream = [torch.cuda.Stream(device=device) for _ in range(num_streams)]
     stream_lock = [Lock() for _ in range(num_streams)]
 
     match model:
-        case 0:
-            model_name = "FeMaSR_SRX2_model_g.pth"
+        case FeMaSRModel.FeMaSR_SRX2_model_g:
             scale = 2
             modulo = 32
-        case 1:
-            model_name = "FeMaSR_SRX4_model_g.pth"
+            downscale = 4
+        case FeMaSRModel.FeMaSR_SRX4_model_g:
             scale = 4
             modulo = 16
+            downscale = 2
 
-    model_path = os.path.join(package_dir, model_name)
-
-    module = FeMaSRNet(codebook_params=[[32, 1024, 512]], LQ_stage=True, scale_factor=scale)
-    module.load_state_dict(torch.load(model_path, map_location="cpu")["params"], strict=False)
-    module.eval().to(device, memory_format=torch.channels_last)
+    w = clip.width
+    h = clip.height
+    pad_w = math.ceil(w / modulo) * modulo
+    pad_h = math.ceil(h / modulo) * modulo
+    padding = (0, pad_w - w, 0, pad_h - h)
+
+    model_name = f"{FeMaSRModel(model).name}.pth"
+    state_dict = torch.load(os.path.join(model_dir, model_name), map_location=device, mmap=True)["params"]
+
+    module = FeMaSRNet(
+        input_resolution=(pad_h // downscale, pad_w // downscale),
+        codebook_params=[[32, 1024, 512]],
+        LQ_stage=True,
+        scale_factor=scale,
+    )
+    module.load_state_dict(state_dict, strict=False)
+    module.eval().to(device)
     if fp16:
         module.half()
 
-    pad_w = math.ceil(clip.width / modulo) * modulo
-    pad_h = math.ceil(clip.height / modulo) * modulo
-
-    if nvfuser:
-        module = memory_efficient_fusion(module)
-
-    if cuda_graphs:
-        graph: list[torch.cuda.CUDAGraph] = []
-        static_input: list[torch.Tensor] = []
-        static_output: list[torch.Tensor] = []
-
-        for i in range(num_streams):
-            static_input.append(
-                torch.zeros((1, 3, pad_h, pad_w), dtype=dtype, device=device).to(memory_format=torch.channels_last)
-            )
+    if trt:
+        import tensorrt
+        import torch_tensorrt
 
-            torch.cuda.synchronize(device=device)
-            stream[i].wait_stream(torch.cuda.current_stream(device=device))
-            with torch.cuda.stream(stream[i]):
-                module(static_input[i])
-            torch.cuda.current_stream(device=device).wait_stream(stream[i])
-            torch.cuda.synchronize(device=device)
-
-            graph.append(torch.cuda.CUDAGraph())
-            with torch.cuda.graph(graph[i], stream=stream[i]):
-                static_output.append(module(static_input[i]))
-    elif trt:
-        device_name = torch.cuda.get_device_name(device)
-        trt_version = tensorrt.__version__
-        dimensions = f"{pad_w}x{pad_h}"
-        precision = "fp16" if fp16 else "fp32"
         trt_engine_path = os.path.join(
-            os.path.realpath(trt_cache_path),
+            os.path.realpath(trt_cache_dir),
             (
                 f"{model_name}"
-                + f"_{device_name}"
-                + f"_trt-{trt_version}"
-                + f"_{dimensions}"
-                + f"_{precision}"
-                + f"_workspace-{trt_max_workspace_size}"
-                + ".pt"
+                + f"_{pad_w}x{pad_h}"
+                + f"_{'fp16' if fp16 else 'fp32'}"
+                + f"_{torch.cuda.get_device_name(device)}"
+                + f"_trt-{tensorrt.__version__}"
+                + (f"_workspace-{trt_workspace_size}" if trt_workspace_size > 0 else "")
+                + (f"_aux-{trt_max_aux_streams}" if trt_max_aux_streams is not None else "")
+                + (f"_level-{trt_optimization_level}" if trt_optimization_level is not None else "")
+                + ".ep"
             ),
         )
 
         if not os.path.isfile(trt_engine_path):
-            lower_setting = LowerSetting(
-                lower_precision=LowerPrecision.FP16 if fp16 else LowerPrecision.FP32,
-                min_acc_module_size=trt_min_subgraph_size,
-                leaf_module_list={VectorQuantizer},
-                max_workspace_size=trt_max_workspace_size,
-                dynamic_batch=False,
-                tactic_sources=1 << int(tensorrt.TacticSource.EDGE_MASK_CONVOLUTIONS)
-                | 1 << int(tensorrt.TacticSource.JIT_CONVOLUTIONS),
-            )
-            lowerer = Lowerer.create(lower_setting=lower_setting)
-            module = lowerer(
+            inputs = [torch.zeros((1, 3, pad_h, pad_w), dtype=dtype, device=device)]
+
+            module = torch_tensorrt.compile(
                 module,
-                [torch.zeros((1, 3, pad_h, pad_w), dtype=dtype, device=device).to(memory_format=torch.channels_last)],
+                ir="dynamo",
+                inputs=inputs,
+                enabled_precisions={dtype},
+                debug=trt_debug,
+                workspace_size=trt_workspace_size,
+                min_block_size=1,
+                max_aux_streams=trt_max_aux_streams,
+                optimization_level=trt_optimization_level,
+                truncate_double=True,
+                device=device,
             )
-            torch.save(module, trt_engine_path)
 
-        del module
-        torch.cuda.empty_cache()
-        module = [torch.load(trt_engine_path) for _ in range(num_streams)]
+            torch_tensorrt.save(module, trt_engine_path, inputs=inputs)
+
+        module = [torch.export.load(trt_engine_path).module() for _ in range(num_streams)]
 
     index = -1
     index_lock = Lock()
 
     @torch.inference_mode()
     def inference(n: int, f: list[vs.VideoFrame]) -> vs.VideoFrame:
         nonlocal index
         with index_lock:
             index = (index + 1) % num_streams
             local_index = index
 
         with stream_lock[local_index], torch.cuda.stream(stream[local_index]):
             img = frame_to_tensor(f[0], device)
+            img = F.pad(img, padding, "replicate")
 
-            h, w = img.shape[2:]
-            img = F.pad(img, (0, pad_w - w, 0, pad_h - h), "reflect")
-
-            if cuda_graphs:
-                static_input[local_index].copy_(img)
-                graph[local_index].replay()
-                output = static_output[local_index]
-            elif trt:
+            if trt:
                 output = module[local_index](img)
             else:
                 output = module(img)
 
-            output = output[:, :, : h * scale, : w * scale]
-
-            return tensor_to_frame(output, f[1].copy())
+            return tensor_to_frame(output[:, :, : h * scale, : w * scale], f[1].copy())
 
     new_clip = clip.std.BlankClip(width=clip.width * scale, height=clip.height * scale, keep=True)
     return new_clip.std.FrameEval(
         lambda n: new_clip.std.ModifyFrame([clip, new_clip], inference), clip_src=[clip, new_clip]
     )
 
 
 def frame_to_tensor(frame: vs.VideoFrame, device: torch.device) -> torch.Tensor:
-    array = np.stack([np.asarray(frame[plane]) for plane in range(frame.format.num_planes)])
-    return torch.from_numpy(array).unsqueeze(0).to(device, memory_format=torch.channels_last).clamp(0.0, 1.0)
+    return (
+        torch.stack([torch.from_numpy(np.asarray(frame[plane])).to(device) for plane in range(frame.format.num_planes)])
+        .unsqueeze(0)
+        .clamp(0.0, 1.0)
+    )
 
 
 def tensor_to_frame(tensor: torch.Tensor, frame: vs.VideoFrame) -> vs.VideoFrame:
     array = tensor.squeeze(0).detach().cpu().numpy()
     for plane in range(frame.format.num_planes):
-        np.copyto(np.asarray(frame[plane]), array[plane, :, :])
+        np.copyto(np.asarray(frame[plane]), array[plane])
     return frame
```

## vsfemasr/__main__.py

```diff
@@ -3,15 +3,15 @@
 import requests
 from tqdm import tqdm
 
 
 def download_model(url: str) -> None:
     filename = url.split("/")[-1]
     r = requests.get(url, stream=True)
-    with open(os.path.join(os.path.dirname(os.path.realpath(__file__)), filename), "wb") as f:
+    with open(os.path.join(os.path.dirname(os.path.realpath(__file__)), "models", filename), "wb") as f:
         with tqdm(
             unit="B",
             unit_scale=True,
             unit_divisor=1024,
             miniters=1,
             desc=filename,
             total=int(r.headers.get("content-length", 0)),
```

## vsfemasr/fema_utils.py

```diff
@@ -1,10 +1,11 @@
 import torch
 from torch import nn
-from torch.nn import functional as F
+
+from .interpolate import interpolate
 
 
 class NormLayer(nn.Module):
     """Normalization Layers.
     ------------
     # Arguments
         - channels: input channels, for batch norm and instance norm.
@@ -88,13 +89,13 @@
 class CombineQuantBlock(nn.Module):
     def __init__(self, in_ch1, in_ch2, out_channel):
         super().__init__()
         self.conv = nn.Conv2d(in_ch1 + in_ch2, out_channel, 3, 1, 1)
 
     def forward(self, input1, input2=None):
         if input2 is not None:
-            input2 = F.interpolate(input2, input1.shape[2:])
+            input2 = interpolate(input2, input1.shape[2:])
             input = torch.cat((input1, input2), dim=1)
         else:
             input = input1
         out = self.conv(input)
         return out
```

## vsfemasr/femasr_arch.py

```diff
@@ -1,17 +1,34 @@
 import numpy as np
 import torch
 import torch.nn.functional as F
 from torch import nn
 
 from .fema_utils import CombineQuantBlock, ResBlock
+from .interpolate import interpolate
 from .network_swinir import RSTB
 from .vgg_arch import VGGFeatureExtractor
 
 
+class Upsample(nn.Module):
+    def __init__(self, size=None, scale_factor=None, mode='nearest', align_corners=None, recompute_scale_factor=None):
+        super().__init__()
+        self.size = size
+        if isinstance(scale_factor, tuple):
+            self.scale_factor = tuple(float(factor) for factor in scale_factor)
+        else:
+            self.scale_factor = float(scale_factor) if scale_factor else None
+        self.mode = mode
+        self.align_corners = align_corners
+        self.recompute_scale_factor = recompute_scale_factor
+
+    def forward(self, input):
+        return interpolate(input, self.size, self.scale_factor, self.mode, self.align_corners, self.recompute_scale_factor)
+
+
 class VectorQuantizer(nn.Module):
     """
     see https://github.com/MishaLaskin/vqvae/blob/d761a999e2267766400dc646d82d3ac3657771d4/models/quantizer.py
     ____________________________________________
     Discretization bottleneck part of the VQ-VAE.
     Inputs:
     - n_e : number of embeddings
@@ -74,31 +91,21 @@
             z_q_gt = torch.matmul(gt_min_onehot, codebook)
             z_q_gt = z_q_gt.view(z.shape)
 
         # get quantized latent vectors
         z_q = torch.matmul(min_encodings, codebook)
         z_q = z_q.view(z.shape)
 
-        e_latent_loss = torch.mean((z_q.detach() - z)**2)
-        q_latent_loss = torch.mean((z_q - z.detach())**2)
-
-        if self.LQ_stage and gt_indices is not None:
-            codebook_loss = self.beta * ((z_q_gt.detach() - z) ** 2).mean()
-            texture_loss = self.gram_loss(z, z_q_gt.detach())
-            codebook_loss = codebook_loss + texture_loss
-        else:
-            codebook_loss = q_latent_loss + e_latent_loss * self.beta
-
         # preserve gradients
         z_q = z + (z_q - z).detach()
 
         # reshape back to match original input shape
         z_q = z_q.permute(0, 3, 1, 2).contiguous()
 
-        return z_q, codebook_loss, min_encoding_indices.reshape(z_q.shape[0], 1, z_q.shape[2], z_q.shape[3])
+        return z_q
 
 class SwinLayers(nn.Module):
     def __init__(self, input_resolution=(32, 32), embed_dim=256,
                 blk_depth=6,
                 num_heads=8,
                 window_size=8,
                 **kwargs):
@@ -150,15 +157,15 @@
 
         if LQ_stage:
             self.blocks.append(SwinLayers(**swin_opts))
             upsampler = nn.ModuleList()
             for i in range(2):
                 in_channel, out_channel = channel_query_dict[res], channel_query_dict[res * 2]
                 upsampler.append(nn.Sequential(
-                    nn.Upsample(scale_factor=2),
+                    Upsample(scale_factor=2),
                     nn.Conv2d(in_channel, out_channel, 3, stride=1, padding=1),
                     ResBlock(out_channel, out_channel, norm_type, act_type),
                     ResBlock(out_channel, out_channel, norm_type, act_type),
                     )
                 )
                 res = res * 2
 
@@ -179,29 +186,30 @@
 
 class DecoderBlock(nn.Module):
     def __init__(self, in_channel, out_channel, norm_type='gn', act_type='leakyrelu'):
         super().__init__()
 
         self.block = []
         self.block += [
-            nn.Upsample(scale_factor=2),
+            Upsample(scale_factor=2),
             nn.Conv2d(in_channel, out_channel, 3, stride=1, padding=1),
             ResBlock(out_channel, out_channel, norm_type, act_type),
             ResBlock(out_channel, out_channel, norm_type, act_type),
         ]
 
         self.block = nn.Sequential(*self.block)
 
     def forward(self, input):
         return self.block(input)
 
 
 class FeMaSRNet(nn.Module):
     def __init__(self,
                  *,
+                 input_resolution,
                  in_channel=3,
                  codebook_params=None,
                  gt_resolution=256,
                  LQ_stage=False,
                  norm_type='gn',
                  act_type='silu',
                  use_quantize=True,
@@ -238,15 +246,16 @@
         self.max_depth = int(np.log2(gt_resolution // self.codebook_scale[0]))
         encode_depth = int(np.log2(gt_resolution // self.scale_factor // self.codebook_scale[0]))
         self.multiscale_encoder = MultiScaleEncoder(
                                 in_channel,
                                 encode_depth,
                                 self.gt_res // self.scale_factor,
                                 channel_query_dict,
-                                norm_type, act_type, LQ_stage
+                                norm_type, act_type, LQ_stage,
+                                input_resolution=input_resolution,
                             )
 
 
         # build decoder
         self.decoder_group = nn.ModuleList()
         for i in range(self.max_depth):
             res = gt_resolution // 2**self.max_depth * 2**i
@@ -287,74 +296,65 @@
             self.conv_semantic = nn.Sequential(
                 nn.Conv2d(512, 512, 1, 1, 0),
                 nn.ReLU(),
                 )
             self.vgg_feat_layer = 'relu4_4'
             self.vgg_feat_extractor = VGGFeatureExtractor([self.vgg_feat_layer])
 
+        self.cur_res_in_codebook_scale = (True, False, False)
+
     def encode_and_decode(self, input, gt_indices=None, current_iter=None):
         enc_feats = self.multiscale_encoder(input.detach())
         if self.LQ_stage:
             enc_feats = enc_feats[-3:]
         else:
             enc_feats = enc_feats[::-1]
 
         if self.use_semantic_loss:
             with torch.no_grad():
                 vgg_feat = self.vgg_feat_extractor(input)[self.vgg_feat_layer]
 
-        codebook_loss_list = []
-        indices_list = []
         semantic_loss_list = []
 
         quant_idx = 0
         prev_dec_feat = None
         prev_quant_feat = None
         x = enc_feats[0]
         for i in range(self.max_depth):
-            cur_res = self.gt_res // 2**self.max_depth * 2**i
-            if cur_res in self.codebook_scale:  # needs to perform quantize
+            if self.cur_res_in_codebook_scale[i]:  # needs to perform quantize
                 if prev_dec_feat is not None:
                     before_quant_feat = torch.cat((enc_feats[i], prev_dec_feat), dim=1)
                 else:
                     before_quant_feat = enc_feats[i]
                 feat_to_quant = self.before_quant_group[quant_idx](before_quant_feat)
 
                 if gt_indices is not None:
-                    z_quant, codebook_loss, indices = self.quantize_group[quant_idx](feat_to_quant, gt_indices[quant_idx])
+                    z_quant = self.quantize_group[quant_idx](feat_to_quant, gt_indices[quant_idx])
                 else:
-                    z_quant, codebook_loss, indices = self.quantize_group[quant_idx](feat_to_quant)
+                    z_quant = self.quantize_group[quant_idx](feat_to_quant)
 
                 if self.use_semantic_loss:
                     semantic_z_quant = self.conv_semantic(z_quant)
                     semantic_loss = F.mse_loss(semantic_z_quant, vgg_feat)
                     semantic_loss_list.append(semantic_loss)
 
                 if not self.use_quantize:
                     z_quant = feat_to_quant
 
                 after_quant_feat = self.after_quant_group[quant_idx](z_quant, prev_quant_feat)
 
-                codebook_loss_list.append(codebook_loss)
-                indices_list.append(indices)
-
                 quant_idx += 1
                 prev_quant_feat = z_quant
                 x = after_quant_feat
             else:
                 if self.LQ_stage and self.use_residual:
                     x = x + enc_feats[i]
                 else:
                     x = x
 
             x = self.decoder_group[i](x)
             prev_dec_feat = x
 
-        out_img = self.out_conv(x)
-
-        codebook_loss = sum(codebook_loss_list)
-        semantic_loss = sum(semantic_loss_list) if len(semantic_loss_list) else codebook_loss * 0
-
-        return out_img
+        return self.out_conv(x)
 
     def forward(self, input):
         return self.encode_and_decode(input)
```

## vsfemasr/network_swinir.py

```diff
@@ -5,20 +5,14 @@
 
 import torch
 import torch.nn as nn
 import torch.utils.checkpoint as checkpoint
 from timm.models.layers import DropPath, to_2tuple, trunc_normal_
 
 
-@torch.fx.wrap
-def img_mask_assign(img_mask, h, w, cnt):
-    img_mask[:, h, w, :] = cnt
-    return img_mask
-
-
 class Mlp(nn.Module):
     def __init__(self, in_features, hidden_features=None, out_features=None, act_layer=nn.GELU, drop=0.):
         super().__init__()
         out_features = out_features or in_features
         hidden_features = hidden_features or in_features
         self.fc1 = nn.Linear(in_features, hidden_features)
         self.act = act_layer()
@@ -45,15 +39,14 @@
     """
     B, H, W, C = x.shape
     x = x.view(B, H // window_size, window_size, W // window_size, window_size, C)
     windows = x.permute(0, 1, 3, 2, 4, 5).contiguous().view(-1, window_size, window_size, C)
     return windows
 
 
-@torch.fx.wrap
 def window_reverse(windows, window_size, H, W):
     """
     Args:
         windows: (num_windows*B, window_size, window_size, C)
         window_size (int): Window size
         H (int): Height of image
         W (int): Width of image
@@ -78,15 +71,14 @@
         qkv_bias (bool, optional):  If True, add a learnable bias to query, key, value. Default: True
         qk_scale (float | None, optional): Override default qk scale of head_dim ** -0.5 if set
         attn_drop (float, optional): Dropout ratio of attention weight. Default: 0.0
         proj_drop (float, optional): Dropout ratio of output. Default: 0.0
     """
 
     def __init__(self, dim, window_size, num_heads, qkv_bias=True, qk_scale=None, attn_drop=0., proj_drop=0.):
-
         super().__init__()
         self.dim = dim
         self.window_size = window_size  # Wh, Ww
         self.num_heads = num_heads
         head_dim = dim // num_heads
         self.scale = qk_scale or head_dim ** -0.5
 
@@ -191,35 +183,31 @@
             qkv_bias=qkv_bias, qk_scale=qk_scale, attn_drop=attn_drop, proj_drop=drop)
 
         self.drop_path = DropPath(drop_path) if drop_path > 0. else nn.Identity()
         self.norm2 = norm_layer(dim)
         mlp_hidden_dim = int(dim * mlp_ratio)
         self.mlp = Mlp(in_features=dim, hidden_features=mlp_hidden_dim, act_layer=act_layer, drop=drop)
 
-        if self.shift_size > 0:
-            attn_mask = self.calculate_mask(self.input_resolution)
-        else:
-            attn_mask = None
-
-        self.register_buffer("attn_mask", attn_mask)
+        attn_mask = self.calculate_mask(self.input_resolution)
+        self.register_buffer("attn_mask", attn_mask, persistent=False)
 
-    def calculate_mask(self, x_size, x=None):
+    def calculate_mask(self, x_size):
         # calculate attention mask for SW-MSA
         H, W = x_size
-        img_mask = torch.zeros((1, H, W, 1)) if x is None else x.new_zeros((1, H, W, 1))  # 1 H W 1
+        img_mask = torch.zeros((1, H, W, 1))  # 1 H W 1
         h_slices = (slice(0, -self.window_size),
                     slice(-self.window_size, -self.shift_size),
                     slice(-self.shift_size, None))
         w_slices = (slice(0, -self.window_size),
                     slice(-self.window_size, -self.shift_size),
                     slice(-self.shift_size, None))
         cnt = 0
         for h in h_slices:
             for w in w_slices:
-                img_mask = img_mask_assign(img_mask, h, w, cnt)
+                img_mask[:, h, w, :] = cnt
                 cnt += 1
 
         mask_windows = window_partition(img_mask, self.window_size)  # nW, window_size, window_size, 1
         mask_windows = mask_windows.view(-1, self.window_size * self.window_size)
         attn_mask = mask_windows.unsqueeze(1) - mask_windows.unsqueeze(2)
         attn_mask = attn_mask.masked_fill(attn_mask != 0, float(-100.0)).masked_fill(attn_mask == 0, float(0.0))
 
@@ -241,15 +229,15 @@
             shifted_x = x
 
         # partition windows
         x_windows = window_partition(shifted_x, self.window_size)  # nW*B, window_size, window_size, C
         x_windows = x_windows.view(-1, self.window_size * self.window_size, C)  # nW*B, window_size*window_size, C
 
         # W-MSA/SW-MSA (to be compatible for testing on images whose shapes are the multiple of window size
-        attn_windows = self.attn(x_windows, mask=self.calculate_mask(x_size, x))
+        attn_windows = self.attn(x_windows, mask=self.attn_mask)  # nW*B, window_size*window_size, C
 
         # merge windows
         attn_windows = attn_windows.view(-1, self.window_size, self.window_size, C)
         shifted_x = window_reverse(attn_windows, self.window_size, H, W)  # B H' W' C
 
         # reverse cyclic shift
         if self.shift_size > 0:
@@ -284,15 +272,14 @@
         downsample (nn.Module | None, optional): Downsample layer at the end of the layer. Default: None
         use_checkpoint (bool): Whether to use checkpointing to save memory. Default: False.
     """
 
     def __init__(self, dim, input_resolution, depth, num_heads, window_size,
                  mlp_ratio=4., qkv_bias=True, qk_scale=None, drop=0., attn_drop=0.,
                  drop_path=0., norm_layer=nn.LayerNorm, downsample=None, use_checkpoint=False):
-
         super().__init__()
         self.dim = dim
         self.input_resolution = input_resolution
         self.depth = depth
         self.use_checkpoint = use_checkpoint
 
         # build blocks
```

## Comparing `vsfemasr-1.2.0.dist-info/METADATA` & `vsfemasr-2.0.0.dist-info/licenses/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,177 +1,121 @@
-Metadata-Version: 2.1
-Name: vsfemasr
-Version: 1.2.0
-Summary: FeMaSR function for VapourSynth
-Project-URL: Homepage, https://github.com/HolyWu/vs-femasr
-Project-URL: Bug Tracker, https://github.com/HolyWu/vs-femasr/issues
-Author-email: HolyWu <holywu@gmail.com>
-License: Creative Commons Legal Code
-        
-        CC0 1.0 Universal
-        
-            CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
-            LEGAL SERVICES. DISTRIBUTION OF THIS DOCUMENT DOES NOT CREATE AN
-            ATTORNEY-CLIENT RELATIONSHIP. CREATIVE COMMONS PROVIDES THIS
-            INFORMATION ON AN "AS-IS" BASIS. CREATIVE COMMONS MAKES NO WARRANTIES
-            REGARDING THE USE OF THIS DOCUMENT OR THE INFORMATION OR WORKS
-            PROVIDED HEREUNDER, AND DISCLAIMS LIABILITY FOR DAMAGES RESULTING FROM
-            THE USE OF THIS DOCUMENT OR THE INFORMATION OR WORKS PROVIDED
-            HEREUNDER.
-        
-        Statement of Purpose
-        
-        The laws of most jurisdictions throughout the world automatically confer
-        exclusive Copyright and Related Rights (defined below) upon the creator
-        and subsequent owner(s) (each and all, an "owner") of an original work of
-        authorship and/or a database (each, a "Work").
-        
-        Certain owners wish to permanently relinquish those rights to a Work for
-        the purpose of contributing to a commons of creative, cultural and
-        scientific works ("Commons") that the public can reliably and without fear
-        of later claims of infringement build upon, modify, incorporate in other
-        works, reuse and redistribute as freely as possible in any form whatsoever
-        and for any purposes, including without limitation commercial purposes.
-        These owners may contribute to the Commons to promote the ideal of a free
-        culture and the further production of creative, cultural and scientific
-        works, or to gain reputation or greater distribution for their Work in
-        part through the use and efforts of others.
-        
-        For these and/or other purposes and motivations, and without any
-        expectation of additional consideration or compensation, the person
-        associating CC0 with a Work (the "Affirmer"), to the extent that he or she
-        is an owner of Copyright and Related Rights in the Work, voluntarily
-        elects to apply CC0 to the Work and publicly distribute the Work under its
-        terms, with knowledge of his or her Copyright and Related Rights in the
-        Work and the meaning and intended legal effect of CC0 on those rights.
-        
-        1. Copyright and Related Rights. A Work made available under CC0 may be
-        protected by copyright and related or neighboring rights ("Copyright and
-        Related Rights"). Copyright and Related Rights include, but are not
-        limited to, the following:
-        
-          i. the right to reproduce, adapt, distribute, perform, display,
-             communicate, and translate a Work;
-         ii. moral rights retained by the original author(s) and/or performer(s);
-        iii. publicity and privacy rights pertaining to a person's image or
-             likeness depicted in a Work;
-         iv. rights protecting against unfair competition in regards to a Work,
-             subject to the limitations in paragraph 4(a), below;
-          v. rights protecting the extraction, dissemination, use and reuse of data
-             in a Work;
-         vi. database rights (such as those arising under Directive 96/9/EC of the
-             European Parliament and of the Council of 11 March 1996 on the legal
-             protection of databases, and under any national implementation
-             thereof, including any amended or successor version of such
-             directive); and
-        vii. other similar, equivalent or corresponding rights throughout the
-             world based on applicable law or treaty, and any national
-             implementations thereof.
-        
-        2. Waiver. To the greatest extent permitted by, but not in contravention
-        of, applicable law, Affirmer hereby overtly, fully, permanently,
-        irrevocably and unconditionally waives, abandons, and surrenders all of
-        Affirmer's Copyright and Related Rights and associated claims and causes
-        of action, whether now known or unknown (including existing as well as
-        future claims and causes of action), in the Work (i) in all territories
-        worldwide, (ii) for the maximum duration provided by applicable law or
-        treaty (including future time extensions), (iii) in any current or future
-        medium and for any number of copies, and (iv) for any purpose whatsoever,
-        including without limitation commercial, advertising or promotional
-        purposes (the "Waiver"). Affirmer makes the Waiver for the benefit of each
-        member of the public at large and to the detriment of Affirmer's heirs and
-        successors, fully intending that such Waiver shall not be subject to
-        revocation, rescission, cancellation, termination, or any other legal or
-        equitable action to disrupt the quiet enjoyment of the Work by the public
-        as contemplated by Affirmer's express Statement of Purpose.
-        
-        3. Public License Fallback. Should any part of the Waiver for any reason
-        be judged legally invalid or ineffective under applicable law, then the
-        Waiver shall be preserved to the maximum extent permitted taking into
-        account Affirmer's express Statement of Purpose. In addition, to the
-        extent the Waiver is so judged Affirmer hereby grants to each affected
-        person a royalty-free, non transferable, non sublicensable, non exclusive,
-        irrevocable and unconditional license to exercise Affirmer's Copyright and
-        Related Rights in the Work (i) in all territories worldwide, (ii) for the
-        maximum duration provided by applicable law or treaty (including future
-        time extensions), (iii) in any current or future medium and for any number
-        of copies, and (iv) for any purpose whatsoever, including without
-        limitation commercial, advertising or promotional purposes (the
-        "License"). The License shall be deemed effective as of the date CC0 was
-        applied by Affirmer to the Work. Should any part of the License for any
-        reason be judged legally invalid or ineffective under applicable law, such
-        partial invalidity or ineffectiveness shall not invalidate the remainder
-        of the License, and in such case Affirmer hereby affirms that he or she
-        will not (i) exercise any of his or her remaining Copyright and Related
-        Rights in the Work or (ii) assert any associated claims and causes of
-        action with respect to the Work, in either case contrary to Affirmer's
-        express Statement of Purpose.
-        
-        4. Limitations and Disclaimers.
-        
-         a. No trademark or patent rights held by Affirmer are waived, abandoned,
-            surrendered, licensed or otherwise affected by this document.
-         b. Affirmer offers the Work as-is and makes no representations or
-            warranties of any kind concerning the Work, express, implied,
-            statutory or otherwise, including without limitation warranties of
-            title, merchantability, fitness for a particular purpose, non
-            infringement, or the absence of latent or other defects, accuracy, or
-            the present or absence of errors, whether or not discoverable, all to
-            the greatest extent permissible under applicable law.
-         c. Affirmer disclaims responsibility for clearing rights of other persons
-            that may apply to the Work or any use thereof, including without
-            limitation any person's Copyright and Related Rights in the Work.
-            Further, Affirmer disclaims responsibility for obtaining any necessary
-            consents, permissions or other rights required for any use of the
-            Work.
-         d. Affirmer understands and acknowledges that Creative Commons is not a
-            party to this document and has no duty or obligation with respect to
-            this CC0 or use of the Work.
-License-File: LICENSE
-Keywords: FeMaSR,VapourSynth
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Multimedia :: Video
-Requires-Python: >=3.10
-Requires-Dist: numpy
-Requires-Dist: requests
-Requires-Dist: tensorrt>=8.5.3.1
-Requires-Dist: timm
-Requires-Dist: torch-tensorrt-fx-only>=1.3.0
-Requires-Dist: torch>=1.13.0
-Requires-Dist: tqdm
-Requires-Dist: vapoursynth>=55
-Description-Content-Type: text/markdown
-
-# FeMaSR
-Real-World Blind Super-Resolution via Feature Matching with Implicit High-Resolution Priors, based on https://github.com/chaofengc/FeMaSR.
-
-
-## Dependencies
-- [NumPy](https://numpy.org/install)
-- [PyTorch](https://pytorch.org/get-started) 1.13
-- [VapourSynth](http://www.vapoursynth.com/) R55+
-
-`trt` requires additional runtime libraries:
-- [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) 11.7
-- [cuDNN](https://developer.nvidia.com/cudnn) 8.6
-- [TensorRT](https://developer.nvidia.com/tensorrt) 8.5.3.1
-
-For ease of installation on Windows, you can download the 7z file on [Releases](https://github.com/HolyWu/vs-femasr/releases) which contains required runtime libraries and Python wheel file. Either add the unzipped directory to your system `PATH` or copy the DLL files to a directory which is already in your system `PATH`. Finally pip install the Python wheel file.
-
-
-## Installation
-```
-pip install -U vsfemasr
-python -m vsfemasr
-```
-
-
-## Usage
-```python
-from vsfemasr import femasr
-
-ret = femasr(clip)
-```
-
-See `__init__.py` for the description of the parameters.
+Creative Commons Legal Code
+
+CC0 1.0 Universal
+
+    CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
+    LEGAL SERVICES. DISTRIBUTION OF THIS DOCUMENT DOES NOT CREATE AN
+    ATTORNEY-CLIENT RELATIONSHIP. CREATIVE COMMONS PROVIDES THIS
+    INFORMATION ON AN "AS-IS" BASIS. CREATIVE COMMONS MAKES NO WARRANTIES
+    REGARDING THE USE OF THIS DOCUMENT OR THE INFORMATION OR WORKS
+    PROVIDED HEREUNDER, AND DISCLAIMS LIABILITY FOR DAMAGES RESULTING FROM
+    THE USE OF THIS DOCUMENT OR THE INFORMATION OR WORKS PROVIDED
+    HEREUNDER.
+
+Statement of Purpose
+
+The laws of most jurisdictions throughout the world automatically confer
+exclusive Copyright and Related Rights (defined below) upon the creator
+and subsequent owner(s) (each and all, an "owner") of an original work of
+authorship and/or a database (each, a "Work").
+
+Certain owners wish to permanently relinquish those rights to a Work for
+the purpose of contributing to a commons of creative, cultural and
+scientific works ("Commons") that the public can reliably and without fear
+of later claims of infringement build upon, modify, incorporate in other
+works, reuse and redistribute as freely as possible in any form whatsoever
+and for any purposes, including without limitation commercial purposes.
+These owners may contribute to the Commons to promote the ideal of a free
+culture and the further production of creative, cultural and scientific
+works, or to gain reputation or greater distribution for their Work in
+part through the use and efforts of others.
+
+For these and/or other purposes and motivations, and without any
+expectation of additional consideration or compensation, the person
+associating CC0 with a Work (the "Affirmer"), to the extent that he or she
+is an owner of Copyright and Related Rights in the Work, voluntarily
+elects to apply CC0 to the Work and publicly distribute the Work under its
+terms, with knowledge of his or her Copyright and Related Rights in the
+Work and the meaning and intended legal effect of CC0 on those rights.
+
+1. Copyright and Related Rights. A Work made available under CC0 may be
+protected by copyright and related or neighboring rights ("Copyright and
+Related Rights"). Copyright and Related Rights include, but are not
+limited to, the following:
+
+  i. the right to reproduce, adapt, distribute, perform, display,
+     communicate, and translate a Work;
+ ii. moral rights retained by the original author(s) and/or performer(s);
+iii. publicity and privacy rights pertaining to a person's image or
+     likeness depicted in a Work;
+ iv. rights protecting against unfair competition in regards to a Work,
+     subject to the limitations in paragraph 4(a), below;
+  v. rights protecting the extraction, dissemination, use and reuse of data
+     in a Work;
+ vi. database rights (such as those arising under Directive 96/9/EC of the
+     European Parliament and of the Council of 11 March 1996 on the legal
+     protection of databases, and under any national implementation
+     thereof, including any amended or successor version of such
+     directive); and
+vii. other similar, equivalent or corresponding rights throughout the
+     world based on applicable law or treaty, and any national
+     implementations thereof.
+
+2. Waiver. To the greatest extent permitted by, but not in contravention
+of, applicable law, Affirmer hereby overtly, fully, permanently,
+irrevocably and unconditionally waives, abandons, and surrenders all of
+Affirmer's Copyright and Related Rights and associated claims and causes
+of action, whether now known or unknown (including existing as well as
+future claims and causes of action), in the Work (i) in all territories
+worldwide, (ii) for the maximum duration provided by applicable law or
+treaty (including future time extensions), (iii) in any current or future
+medium and for any number of copies, and (iv) for any purpose whatsoever,
+including without limitation commercial, advertising or promotional
+purposes (the "Waiver"). Affirmer makes the Waiver for the benefit of each
+member of the public at large and to the detriment of Affirmer's heirs and
+successors, fully intending that such Waiver shall not be subject to
+revocation, rescission, cancellation, termination, or any other legal or
+equitable action to disrupt the quiet enjoyment of the Work by the public
+as contemplated by Affirmer's express Statement of Purpose.
+
+3. Public License Fallback. Should any part of the Waiver for any reason
+be judged legally invalid or ineffective under applicable law, then the
+Waiver shall be preserved to the maximum extent permitted taking into
+account Affirmer's express Statement of Purpose. In addition, to the
+extent the Waiver is so judged Affirmer hereby grants to each affected
+person a royalty-free, non transferable, non sublicensable, non exclusive,
+irrevocable and unconditional license to exercise Affirmer's Copyright and
+Related Rights in the Work (i) in all territories worldwide, (ii) for the
+maximum duration provided by applicable law or treaty (including future
+time extensions), (iii) in any current or future medium and for any number
+of copies, and (iv) for any purpose whatsoever, including without
+limitation commercial, advertising or promotional purposes (the
+"License"). The License shall be deemed effective as of the date CC0 was
+applied by Affirmer to the Work. Should any part of the License for any
+reason be judged legally invalid or ineffective under applicable law, such
+partial invalidity or ineffectiveness shall not invalidate the remainder
+of the License, and in such case Affirmer hereby affirms that he or she
+will not (i) exercise any of his or her remaining Copyright and Related
+Rights in the Work or (ii) assert any associated claims and causes of
+action with respect to the Work, in either case contrary to Affirmer's
+express Statement of Purpose.
+
+4. Limitations and Disclaimers.
+
+ a. No trademark or patent rights held by Affirmer are waived, abandoned,
+    surrendered, licensed or otherwise affected by this document.
+ b. Affirmer offers the Work as-is and makes no representations or
+    warranties of any kind concerning the Work, express, implied,
+    statutory or otherwise, including without limitation warranties of
+    title, merchantability, fitness for a particular purpose, non
+    infringement, or the absence of latent or other defects, accuracy, or
+    the present or absence of errors, whether or not discoverable, all to
+    the greatest extent permissible under applicable law.
+ c. Affirmer disclaims responsibility for clearing rights of other persons
+    that may apply to the Work or any use thereof, including without
+    limitation any person's Copyright and Related Rights in the Work.
+    Further, Affirmer disclaims responsibility for obtaining any necessary
+    consents, permissions or other rights required for any use of the
+    Work.
+ d. Affirmer understands and acknowledges that Creative Commons is not a
+    party to this document and has no duty or obligation with respect to
+    this CC0 or use of the Work.
```

