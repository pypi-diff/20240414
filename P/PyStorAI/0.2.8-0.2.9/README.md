# Comparing `tmp/PyStorAI-0.2.8.tar.gz` & `tmp/PyStorAI-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyStorAI-0.2.8.tar", last modified: Sat Apr 13 10:55:07 2024, max compression
+gzip compressed data, was "PyStorAI-0.2.9.tar", last modified: Sun Apr 14 18:43:26 2024, max compression
```

## Comparing `PyStorAI-0.2.8.tar` & `PyStorAI-0.2.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 10:55:07.531303 PyStorAI-0.2.8/
--rw-r--r--   0 root         (0) root         (0)      815 2024-04-13 10:55:07.531303 PyStorAI-0.2.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 10:55:07.529303 PyStorAI-0.2.8/PyStorAI/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-13 10:48:03.000000 PyStorAI-0.2.8/PyStorAI/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6136 2024-04-13 10:47:47.000000 PyStorAI-0.2.8/PyStorAI/storyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 10:55:07.531303 PyStorAI-0.2.8/PyStorAI.egg-info/
--rw-r--r--   0 root         (0) root         (0)      815 2024-04-13 10:55:07.000000 PyStorAI-0.2.8/PyStorAI.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      180 2024-04-13 10:55:07.000000 PyStorAI-0.2.8/PyStorAI.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 10:55:07.000000 PyStorAI-0.2.8/PyStorAI.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-13 10:55:07.000000 PyStorAI-0.2.8/PyStorAI.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 10:55:07.531303 PyStorAI-0.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1015 2024-04-13 10:54:01.000000 PyStorAI-0.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 18:43:26.257300 PyStorAI-0.2.9/
+-rw-r--r--   0 root         (0) root         (0)      815 2024-04-14 18:43:26.257300 PyStorAI-0.2.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 18:43:26.255300 PyStorAI-0.2.9/PyStorAI/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 18:42:17.000000 PyStorAI-0.2.9/PyStorAI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5444 2024-04-14 18:42:55.000000 PyStorAI-0.2.9/PyStorAI/storyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 18:43:26.256300 PyStorAI-0.2.9/PyStorAI.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      815 2024-04-14 18:43:26.000000 PyStorAI-0.2.9/PyStorAI.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      180 2024-04-14 18:43:26.000000 PyStorAI-0.2.9/PyStorAI.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 18:43:26.000000 PyStorAI-0.2.9/PyStorAI.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-14 18:43:26.000000 PyStorAI-0.2.9/PyStorAI.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-14 18:43:26.257300 PyStorAI-0.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1015 2024-04-14 18:41:31.000000 PyStorAI-0.2.9/setup.py
```

### Comparing `PyStorAI-0.2.8/PKG-INFO` & `PyStorAI-0.2.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyStorAI
-Version: 0.2.8
+Version: 0.2.9
 Summary: Effective Storyboard Visualisations for Artificial Intelligence.
 Home-page: https://github.com/VisualXAI/PyStorAI
 Author: Alexander Brown
 Author-email: ajbrownv@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PyStorAI-0.2.8/PyStorAI/storyboard.py` & `PyStorAI-0.2.9/PyStorAI/storyboard.py`

 * *Files 11% similar despite different names*

```diff
@@ -66,54 +66,38 @@
         num_cols = 5
     else:
         num_cols = 4
 
     num_rows = -(-num_images // num_cols)
 
 
-    with PdfPages('output.pdf') as pdf:
-        # plt.ioff() # Disable interactive mode
-
-        if inline: # Plot inline if inline=True
-            
-            fig, axes = plt.subplots(num_rows, num_cols, figsize=(num_cols*2, num_rows*2))
-
-            # Plot each image and only show necessary axes
-            for i, file_name in enumerate(image_files):
-                img = imread(file_name)
-                ax = axes[i // num_cols, i % num_cols] if num_rows > 1 else axes[i % num_cols]
-                ax.imshow(img)
-                ax.axis('off')
-
-            # Hide any remaining empty axes
-            for i in range(num_images, num_rows * num_cols):
-                axes.flatten()[i].axis('off')
-
-            # Adjust layout and show the plot (blocking)
-            plt.tight_layout()
-            plt.show()
-
-        # Save images to PDF
-        fig, axes = plt.subplots(num_rows, num_cols, figsize=(num_cols*2, num_rows*2))
-
-        for i, file_name in enumerate(image_files):
-            img = imread(file_name)
-            ax = axes[i // num_cols, i % num_cols] if num_rows > 1 else axes[i % num_cols]
-            ax.imshow(img)
-            ax.axis('off')
-
-        # Hide any remaining empty axes
-        for i in range(num_images, num_rows * num_cols):
-            axes.flatten()[i].axis('off')
-
-        # Adjust layout and save to PDF
-        plt.tight_layout()
-        pdf.savefig()
-
-        # plt.ion()  # Re-enable interactive mode
+    with PdfPages('output.pdf') as pdf:
+        # plt.ioff() # Disable interactive mode
+
+        fig, axes = plt.subplots(num_rows, num_cols, figsize=(num_cols*2, num_rows*2))
+
+        # Plot images in correct layout
+        for i, file_name in enumerate(image_files):
+          img = imread(file_name)
+          ax = axes[i // num_cols, i % num_cols] if num_rows > 1 else axes[i % num_cols]
+          ax.imshow(img)
+          ax.axis('off')
+
+        # Hide any remaining empty axes
+        for i in range(num_images, num_rows * num_cols):
+          axes.flatten()[i].axis('off')
+
+        # Adjust layout and save to PDF
+        plt.tight_layout()
+        pdf.savefig()
+
+        if inline: # Plot inline if inline=True
+          plt.show()
+        
+        # plt.ion() # Re-enable interactive mode
         plt.close()
 
 
 
 def show_all():
 
     base_url = "https://github.com/VisualXAI/PyStorAI/blob/main/image"
```

### Comparing `PyStorAI-0.2.8/PyStorAI.egg-info/PKG-INFO` & `PyStorAI-0.2.9/PyStorAI.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyStorAI
-Version: 0.2.8
+Version: 0.2.9
 Summary: Effective Storyboard Visualisations for Artificial Intelligence.
 Home-page: https://github.com/VisualXAI/PyStorAI
 Author: Alexander Brown
 Author-email: ajbrownv@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PyStorAI-0.2.8/setup.py` & `PyStorAI-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PyStorAI',
-    version='0.2.8',
+    version='0.2.9',
     packages=find_packages(),
     install_requires=[],
     include_package_data=True,
     author='Alexander Brown',
     author_email='ajbrownv@gmail.com',
     description='Effective Storyboard Visualisations for Artificial Intelligence.',
     long_description='A longer description of your package',
```

