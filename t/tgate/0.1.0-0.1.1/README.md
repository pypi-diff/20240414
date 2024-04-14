# Comparing `tmp/tgate-0.1.0.tar.gz` & `tmp/tgate-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tgate-0.1.0.tar", last modified: Wed Apr 10 15:15:38 2024, max compression
+gzip compressed data, was "dist/tgate-0.1.1.tar", last modified: Sun Apr 14 10:46:59 2024, max compression
```

## Comparing `tgate-0.1.0.tar` & `tgate-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 liuh0g   (187183) g-liuh0g (1187183)        0 2024-04-10 15:15:38.021873 tgate-0.1.0/
--rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)     1067 2024-04-09 12:18:22.000000 tgate-0.1.0/LICENSE
--rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)     7692 2024-04-10 15:15:38.015873 tgate-0.1.0/PKG-INFO
--rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)     6985 2024-04-10 15:11:38.000000 tgate-0.1.0/README.md
--rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)       38 2024-04-10 15:15:38.018856 tgate-0.1.0/setup.cfg
--rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)      958 2024-04-10 15:10:48.000000 tgate-0.1.0/setup.py
-drwxr-xr-x   0 liuh0g   (187183) g-liuh0g (1187183)        0 2024-04-10 15:15:37.983399 tgate-0.1.0/src/
-drwxr-xr-x   0 liuh0g   (187183) g-liuh0g (1187183)        0 2024-04-10 15:15:38.000090 tgate-0.1.0/src/tgate/
--rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)    16071 2024-04-09 19:19:42.000000 tgate-0.1.0/src/tgate/PixArt_Alpha.py
--rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)    15954 2024-04-09 19:19:42.000000 tgate-0.1.0/src/tgate/SD.py
--rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)    25944 2024-04-09 19:19:42.000000 tgate-0.1.0/src/tgate/SDXL.py
--rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)    26500 2024-04-10 05:20:48.000000 tgate-0.1.0/src/tgate/SDXL_DeepCache.py
--rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)    16470 2024-04-10 05:21:18.000000 tgate-0.1.0/src/tgate/SD_DeepCache.py
--rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)      209 2024-04-09 19:19:42.000000 tgate-0.1.0/src/tgate/__init__.py
--rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)     9402 2024-04-09 19:19:42.000000 tgate-0.1.0/src/tgate/tgate_utils.py
-drwxr-xr-x   0 liuh0g   (187183) g-liuh0g (1187183)        0 2024-04-10 15:15:38.016259 tgate-0.1.0/src/tgate.egg-info/
--rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)     7692 2024-04-10 15:15:37.000000 tgate-0.1.0/src/tgate.egg-info/PKG-INFO
--rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)      351 2024-04-10 15:15:37.000000 tgate-0.1.0/src/tgate.egg-info/SOURCES.txt
--rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)        1 2024-04-10 15:15:37.000000 tgate-0.1.0/src/tgate.egg-info/dependency_links.txt
--rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)       57 2024-04-10 15:15:37.000000 tgate-0.1.0/src/tgate.egg-info/requires.txt
--rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)        6 2024-04-10 15:15:37.000000 tgate-0.1.0/src/tgate.egg-info/top_level.txt
+drwxr-xr-x   0 liuh0g   (187183) g-liuh0g (1187183)        0 2024-04-14 10:46:59.563253 tgate-0.1.1/
+-rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)     1067 2024-04-09 12:18:22.000000 tgate-0.1.1/LICENSE
+-rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)     7621 2024-04-14 10:46:59.560446 tgate-0.1.1/PKG-INFO
+-rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)     6985 2024-04-10 15:11:38.000000 tgate-0.1.1/README.md
+-rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)       38 2024-04-14 10:46:59.563040 tgate-0.1.1/setup.cfg
+-rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)      892 2024-04-14 10:46:40.000000 tgate-0.1.1/setup.py
+drwxr-xr-x   0 liuh0g   (187183) g-liuh0g (1187183)        0 2024-04-14 10:46:59.410759 tgate-0.1.1/src/
+drwxr-xr-x   0 liuh0g   (187183) g-liuh0g (1187183)        0 2024-04-14 10:46:59.442929 tgate-0.1.1/src/tgate/
+-rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)    16071 2024-04-09 19:19:42.000000 tgate-0.1.1/src/tgate/PixArt_Alpha.py
+-rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)    15954 2024-04-09 19:19:42.000000 tgate-0.1.1/src/tgate/SD.py
+-rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)    27167 2024-04-14 09:24:48.000000 tgate-0.1.1/src/tgate/SDXL.py
+-rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)    27723 2024-04-14 09:25:40.000000 tgate-0.1.1/src/tgate/SDXL_DeepCache.py
+-rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)    16470 2024-04-10 05:21:18.000000 tgate-0.1.1/src/tgate/SD_DeepCache.py
+-rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)      209 2024-04-09 19:19:42.000000 tgate-0.1.1/src/tgate/__init__.py
+-rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)     9402 2024-04-09 19:19:42.000000 tgate-0.1.1/src/tgate/tgate_utils.py
+drwxr-xr-x   0 liuh0g   (187183) g-liuh0g (1187183)        0 2024-04-14 10:46:59.558395 tgate-0.1.1/src/tgate.egg-info/
+-rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)     7621 2024-04-14 10:46:59.000000 tgate-0.1.1/src/tgate.egg-info/PKG-INFO
+-rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)      351 2024-04-14 10:46:59.000000 tgate-0.1.1/src/tgate.egg-info/SOURCES.txt
+-rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)        1 2024-04-14 10:46:59.000000 tgate-0.1.1/src/tgate.egg-info/dependency_links.txt
+-rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)       57 2024-04-14 10:46:59.000000 tgate-0.1.1/src/tgate.egg-info/requires.txt
+-rw-r--r--   0 liuh0g   (187183) g-liuh0g (1187183)        6 2024-04-14 10:46:59.000000 tgate-0.1.1/src/tgate.egg-info/top_level.txt
```

### Comparing `tgate-0.1.0/LICENSE` & `tgate-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tgate-0.1.0/PKG-INFO` & `tgate-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tgate
-Version: 0.1.0
+Version: 0.1.1
 Summary: T-GATE: Cross-Attention Makes Inference Cumbersome in Text-to-Image Diffusion Models.
-Home-page: https://github.com/HaozheLiu-ST/T-GATE/tree/release-v.0.1.0/
-Author: ['Wentian Zhang', 'Haozhe Liu', 'Jinheng Xie']
-Author-email: ['zhangwentianml@gmail.com', 'haozhe.liu@kaust.edu.sa']
+Home-page: https://github.com/HaozheLiu-ST/T-GATE/tree/releases/
+Author: Wentian Zhang
+Author-email: zhangwentianml@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: diffusers
```

### Comparing `tgate-0.1.0/README.md` & `tgate-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tgate-0.1.0/setup.py` & `tgate-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 setuptools.setup(
     name="tgate",
-    version="v0.1.0",
-    author=["Wentian Zhang", "Haozhe Liu", "Jinheng Xie"],
-    author_email=["zhangwentianml@gmail.com","haozhe.liu@kaust.edu.sa"],
+    version="v0.1.1",
+    author="Wentian Zhang",
+    author_email="zhangwentianml@gmail.com",
     description="T-GATE: Cross-Attention Makes Inference Cumbersome in Text-to-Image Diffusion Models.",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
-    url="https://github.com/HaozheLiu-ST/T-GATE/tree/release-v.0.1.0/",
+    url="https://github.com/HaozheLiu-ST/T-GATE/tree/releases/",
     package_dir={"": "src"},
     packages=setuptools.find_packages('src'),
     include_package_data=False,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `tgate-0.1.0/src/tgate/PixArt_Alpha.py` & `tgate-0.1.1/src/tgate/PixArt_Alpha.py`

 * *Files identical despite different names*

### Comparing `tgate-0.1.0/src/tgate/SD.py` & `tgate-0.1.1/src/tgate/SD.py`

 * *Files identical despite different names*

### Comparing `tgate-0.1.0/src/tgate/SDXL.py` & `tgate-0.1.1/src/tgate/SDXL.py`

 * *Files 6% similar despite different names*

```diff
@@ -451,29 +451,48 @@
                 if callback is not None and i % callback_steps == 0:
                     step_idx = i // getattr(self.scheduler, "order", 1)
                     callback(step_idx, t, latents)
 
             if XLA_AVAILABLE:
                 xm.mark_step()
 
-    if not output_type == "latent":
-        # make sure the VAE is in float32 mode, as it overflows in float16
-        needs_upcasting = self.vae.dtype == torch.float16 and self.vae.config.force_upcast
-
-        if needs_upcasting:
-            self.upcast_vae()
-            latents = latents.to(next(iter(self.vae.post_quant_conv.parameters())).dtype)
-
-        image = self.vae.decode(latents / self.vae.config.scaling_factor, return_dict=False)[0]
-
-        # cast back to fp16 if needed
-        if needs_upcasting:
-            self.vae.to(dtype=torch.float16)
-    else:
-        image = latents
+        if not output_type == "latent":
+            # make sure the VAE is in float32 mode, as it overflows in float16
+            needs_upcasting = self.vae.dtype == torch.float16 and self.vae.config.force_upcast
+
+            if needs_upcasting:
+                self.upcast_vae()
+                latents = latents.to(next(iter(self.vae.post_quant_conv.parameters())).dtype)
+            elif latents.dtype != self.vae.dtype:
+                if torch.backends.mps.is_available():
+                    # some platforms (eg. apple mps) misbehave due to a pytorch bug: https://github.com/pytorch/pytorch/pull/99272
+                    self.vae = self.vae.to(latents.dtype)
+
+            # unscale/denormalize the latents
+            # denormalize with the mean and std if available and not None
+            has_latents_mean = hasattr(self.vae.config, "latents_mean") and self.vae.config.latents_mean is not None
+            has_latents_std = hasattr(self.vae.config, "latents_std") and self.vae.config.latents_std is not None
+            if has_latents_mean and has_latents_std:
+                latents_mean = (
+                    torch.tensor(self.vae.config.latents_mean).view(1, 4, 1, 1).to(latents.device, latents.dtype)
+                )
+                latents_std = (
+                    torch.tensor(self.vae.config.latents_std).view(1, 4, 1, 1).to(latents.device, latents.dtype)
+                )
+                latents = latents * latents_std / self.vae.config.scaling_factor + latents_mean
+            else:
+                latents = latents / self.vae.config.scaling_factor
+
+            image = self.vae.decode(latents, return_dict=False)[0]
+
+            # cast back to fp16 if needed
+            if needs_upcasting:
+                self.vae.to(dtype=torch.float16)
+        else:
+            image = latents
 
     if not output_type == "latent":
         # apply watermark if available
         if self.watermark is not None:
             image = self.watermark.apply_watermark(image)
 
         image = self.image_processor.postprocess(image, output_type=output_type)
@@ -493,8 +512,8 @@
     register_tgate_forward(pipe.unet, 
         'Attention',
         gate_step=gate_step,
         inference_num_per_image = num_inference_steps, 
         lcm=lcm,
         )
     pipe.tgate = MethodType(tgate,pipe)
-    return pipe
+    return pipe
```

### Comparing `tgate-0.1.0/src/tgate/SDXL_DeepCache.py` & `tgate-0.1.1/src/tgate/SDXL_DeepCache.py`

 * *Files 6% similar despite different names*

```diff
@@ -463,29 +463,49 @@
                     step_idx = i // getattr(self.scheduler, "order", 1)
                     callback(step_idx, t, latents)
 
             if XLA_AVAILABLE:
                 xm.mark_step()
         self.deepcache.disable()
         self.deepcache.enable()
-    if not output_type == "latent":
-        # make sure the VAE is in float32 mode, as it overflows in float16
-        needs_upcasting = self.vae.dtype == torch.float16 and self.vae.config.force_upcast
 
-        if needs_upcasting:
-            self.upcast_vae()
-            latents = latents.to(next(iter(self.vae.post_quant_conv.parameters())).dtype)
-
-        image = self.vae.decode(latents / self.vae.config.scaling_factor, return_dict=False)[0]
-
-        # cast back to fp16 if needed
-        if needs_upcasting:
-            self.vae.to(dtype=torch.float16)
-    else:
-        image = latents
+        if not output_type == "latent":
+            # make sure the VAE is in float32 mode, as it overflows in float16
+            needs_upcasting = self.vae.dtype == torch.float16 and self.vae.config.force_upcast
+
+            if needs_upcasting:
+                self.upcast_vae()
+                latents = latents.to(next(iter(self.vae.post_quant_conv.parameters())).dtype)
+            elif latents.dtype != self.vae.dtype:
+                if torch.backends.mps.is_available():
+                    # some platforms (eg. apple mps) misbehave due to a pytorch bug: https://github.com/pytorch/pytorch/pull/99272
+                    self.vae = self.vae.to(latents.dtype)
+
+            # unscale/denormalize the latents
+            # denormalize with the mean and std if available and not None
+            has_latents_mean = hasattr(self.vae.config, "latents_mean") and self.vae.config.latents_mean is not None
+            has_latents_std = hasattr(self.vae.config, "latents_std") and self.vae.config.latents_std is not None
+            if has_latents_mean and has_latents_std:
+                latents_mean = (
+                    torch.tensor(self.vae.config.latents_mean).view(1, 4, 1, 1).to(latents.device, latents.dtype)
+                )
+                latents_std = (
+                    torch.tensor(self.vae.config.latents_std).view(1, 4, 1, 1).to(latents.device, latents.dtype)
+                )
+                latents = latents * latents_std / self.vae.config.scaling_factor + latents_mean
+            else:
+                latents = latents / self.vae.config.scaling_factor
+
+            image = self.vae.decode(latents, return_dict=False)[0]
+
+            # cast back to fp16 if needed
+            if needs_upcasting:
+                self.vae.to(dtype=torch.float16)
+        else:
+            image = latents
 
     if not output_type == "latent":
         # apply watermark if available
         if self.watermark is not None:
             image = self.watermark.apply_watermark(image)
 
         image = self.image_processor.postprocess(image, output_type=output_type)
```

### Comparing `tgate-0.1.0/src/tgate/SD_DeepCache.py` & `tgate-0.1.1/src/tgate/SD_DeepCache.py`

 * *Files identical despite different names*

### Comparing `tgate-0.1.0/src/tgate/tgate_utils.py` & `tgate-0.1.1/src/tgate/tgate_utils.py`

 * *Files identical despite different names*

### Comparing `tgate-0.1.0/src/tgate.egg-info/PKG-INFO` & `tgate-0.1.1/src/tgate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tgate
-Version: 0.1.0
+Version: 0.1.1
 Summary: T-GATE: Cross-Attention Makes Inference Cumbersome in Text-to-Image Diffusion Models.
-Home-page: https://github.com/HaozheLiu-ST/T-GATE/tree/release-v.0.1.0/
-Author: ['Wentian Zhang', 'Haozhe Liu', 'Jinheng Xie']
-Author-email: ['zhangwentianml@gmail.com', 'haozhe.liu@kaust.edu.sa']
+Home-page: https://github.com/HaozheLiu-ST/T-GATE/tree/releases/
+Author: Wentian Zhang
+Author-email: zhangwentianml@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: diffusers
```

