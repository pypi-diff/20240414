# Comparing `tmp/ngclearn-1.0b2.tar.gz` & `tmp/ngclearn-1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngclearn-1.0b2.tar", last modified: Sat Mar 30 23:09:45 2024, max compression
+gzip compressed data, was "ngclearn-1.0b3.tar", last modified: Sun Apr 14 20:41:22 2024, max compression
```

## Comparing `ngclearn-1.0b2.tar` & `ngclearn-1.0b3.tar`

### file list

```diff
@@ -1,69 +1,77 @@
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 23:09:45.119901 ngclearn-1.0b2/
--rw-rw-r--   0 ago       (1001) ago       (1001)      368 2024-03-27 21:42:18.000000 ngclearn-1.0b2/AUTHORS
--rw-rw-r--   0 ago       (1001) ago       (1001)     1548 2024-03-27 21:42:18.000000 ngclearn-1.0b2/LICENSE
--rw-r--r--   0 ago       (1001) ago       (1001)     8102 2024-03-30 23:09:45.119901 ngclearn-1.0b2/PKG-INFO
--rw-rw-r--   0 ago       (1001) ago       (1001)     6378 2024-03-30 23:05:02.000000 ngclearn-1.0b2/README.md
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 23:09:45.111901 ngclearn-1.0b2/ngclearn/
--rw-rw-r--   0 ago       (1001) ago       (1001)      706 2024-03-29 23:12:24.000000 ngclearn-1.0b2/ngclearn/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 23:09:45.115901 ngclearn-1.0b2/ngclearn/commands/
--rw-rw-r--   0 ago       (1001) ago       (1001)       33 2024-03-28 23:58:59.000000 ngclearn-1.0b2/ngclearn/commands/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 23:09:45.115901 ngclearn-1.0b2/ngclearn/components/
--rw-rw-r--   0 ago       (1001) ago       (1001)     1020 2024-03-30 04:48:51.000000 ngclearn-1.0b2/ngclearn/components/__init__.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     1081 2024-03-28 22:29:48.000000 ngclearn-1.0b2/ngclearn/components/baseComponentTemplate.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 23:09:45.115901 ngclearn-1.0b2/ngclearn/components/input_encoders/
--rw-rw-r--   0 ago       (1001) ago       (1001)      118 2024-03-30 04:48:51.000000 ngclearn-1.0b2/ngclearn/components/input_encoders/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     3576 2024-03-30 04:48:51.000000 ngclearn-1.0b2/ngclearn/components/input_encoders/bernoulliCell.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     8130 2024-03-30 23:00:42.000000 ngclearn-1.0b2/ngclearn/components/input_encoders/latencyCell.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     3933 2024-03-30 20:38:16.000000 ngclearn-1.0b2/ngclearn/components/input_encoders/poissonCell.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 23:09:45.115901 ngclearn-1.0b2/ngclearn/components/neurons/
--rw-rw-r--   0 ago       (1001) ago       (1001)      426 2024-03-27 21:42:18.000000 ngclearn-1.0b2/ngclearn/components/neurons/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 23:09:45.115901 ngclearn-1.0b2/ngclearn/components/neurons/graded/
--rw-rw-r--   0 ago       (1001) ago       (1001)      178 2024-03-27 21:42:18.000000 ngclearn-1.0b2/ngclearn/components/neurons/graded/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     5224 2024-03-28 22:30:33.000000 ngclearn-1.0b2/ngclearn/components/neurons/graded/gaussianErrorCell.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     5221 2024-03-28 22:30:42.000000 ngclearn-1.0b2/ngclearn/components/neurons/graded/laplacianErrorCell.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     6376 2024-03-30 21:58:57.000000 ngclearn-1.0b2/ngclearn/components/neurons/graded/rateCell.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 23:09:45.115901 ngclearn-1.0b2/ngclearn/components/neurons/spiking/
--rw-rw-r--   0 ago       (1001) ago       (1001)    11036 2024-03-28 22:31:05.000000 ngclearn-1.0b2/ngclearn/components/neurons/spiking/LIFCell.py
--rw-rw-r--   0 ago       (1001) ago       (1001)      195 2024-03-27 21:42:18.000000 ngclearn-1.0b2/ngclearn/components/neurons/spiking/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     4465 2024-03-28 22:31:00.000000 ngclearn-1.0b2/ngclearn/components/neurons/spiking/izhikevichCell.py
--rw-rw-r--   0 ago       (1001) ago       (1001)    11707 2024-03-28 22:31:11.000000 ngclearn-1.0b2/ngclearn/components/neurons/spiking/quadLIFCell.py
--rw-rw-r--   0 ago       (1001) ago       (1001)    14285 2024-03-29 04:07:05.000000 ngclearn-1.0b2/ngclearn/components/neurons/spiking/sLIFCell.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 23:09:45.115901 ngclearn-1.0b2/ngclearn/components/other/
--rw-rw-r--   0 ago       (1001) ago       (1001)       64 2024-03-27 21:42:18.000000 ngclearn-1.0b2/ngclearn/components/other/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     4518 2024-03-28 22:31:30.000000 ngclearn-1.0b2/ngclearn/components/other/expKernel.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     5217 2024-03-28 22:31:38.000000 ngclearn-1.0b2/ngclearn/components/other/varTrace.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 23:09:45.115901 ngclearn-1.0b2/ngclearn/components/synapses/
--rw-rw-r--   0 ago       (1001) ago       (1001)      160 2024-03-27 21:42:18.000000 ngclearn-1.0b2/ngclearn/components/synapses/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 23:09:45.115901 ngclearn-1.0b2/ngclearn/components/synapses/hebbian/
--rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-03-27 21:42:18.000000 ngclearn-1.0b2/ngclearn/components/synapses/hebbian/__init__.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     8378 2024-03-28 22:31:56.000000 ngclearn-1.0b2/ngclearn/components/synapses/hebbian/expSTDPSynapse.py
--rw-rw-r--   0 ago       (1001) ago       (1001)    11061 2024-03-29 04:07:05.000000 ngclearn-1.0b2/ngclearn/components/synapses/hebbian/hebbianSynapse.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     9789 2024-03-28 22:32:06.000000 ngclearn-1.0b2/ngclearn/components/synapses/hebbian/traceSTDPSynapse.py
--rw-rw-r--   0 ago       (1001) ago       (1001)      263 2024-03-29 00:03:17.000000 ngclearn-1.0b2/ngclearn/components/wrappers.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 23:09:45.115901 ngclearn-1.0b2/ngclearn/utils/
--rwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-27 21:42:18.000000 ngclearn-1.0b2/ngclearn/utils/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 23:09:45.115901 ngclearn-1.0b2/ngclearn/utils/density/
--rw-r--r--   0 ago       (1001) ago       (1001)        0 2024-03-28 00:06:24.000000 ngclearn-1.0b2/ngclearn/utils/density/__init__.py
--rw-r--r--   0 ago       (1001) ago       (1001)     2816 2024-03-28 02:06:50.000000 ngclearn-1.0b2/ngclearn/utils/density/gmm.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     1629 2024-03-27 21:42:18.000000 ngclearn-1.0b2/ngclearn/utils/io_utils.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     7896 2024-03-30 21:58:57.000000 ngclearn-1.0b2/ngclearn/utils/model_utils.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 23:09:45.115901 ngclearn-1.0b2/ngclearn/utils/optim/
--rw-rw-r--   0 ago       (1001) ago       (1001)       46 2024-03-27 21:42:18.000000 ngclearn-1.0b2/ngclearn/utils/optim/__init__.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     3090 2024-03-27 21:42:18.000000 ngclearn-1.0b2/ngclearn/utils/optim/adam.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)      783 2024-03-27 21:42:18.000000 ngclearn-1.0b2/ngclearn/utils/optim/opt.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     1122 2024-03-27 21:42:18.000000 ngclearn-1.0b2/ngclearn/utils/optim/sgd.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     3164 2024-03-27 21:42:18.000000 ngclearn-1.0b2/ngclearn/utils/patch_utils.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 23:09:45.119901 ngclearn-1.0b2/ngclearn/utils/viz/
--rw-rw-r--   0 ago       (1001) ago       (1001)        0 2024-03-27 21:42:18.000000 ngclearn-1.0b2/ngclearn/utils/viz/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     3414 2024-03-27 21:42:18.000000 ngclearn-1.0b2/ngclearn/utils/viz/dim_reduce.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     6723 2024-03-27 21:42:18.000000 ngclearn-1.0b2/ngclearn/utils/viz/raster.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     4922 2024-03-30 16:17:15.000000 ngclearn-1.0b2/ngclearn/utils/viz/synapse_plot.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 23:09:45.119901 ngclearn-1.0b2/ngclearn.egg-info/
--rw-r--r--   0 ago       (1001) ago       (1001)     8102 2024-03-30 23:09:45.000000 ngclearn-1.0b2/ngclearn.egg-info/PKG-INFO
--rw-rw-r--   0 ago       (1001) ago       (1001)     1867 2024-03-30 23:09:45.000000 ngclearn-1.0b2/ngclearn.egg-info/SOURCES.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)        1 2024-03-30 23:09:45.000000 ngclearn-1.0b2/ngclearn.egg-info/dependency_links.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-03-30 23:09:45.000000 ngclearn-1.0b2/ngclearn.egg-info/requires.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)       19 2024-03-30 23:09:45.000000 ngclearn-1.0b2/ngclearn.egg-info/top_level.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)     1838 2024-03-30 23:03:46.000000 ngclearn-1.0b2/pyproject.toml
--rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-03-30 18:06:06.000000 ngclearn-1.0b2/requirements.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)       38 2024-03-30 23:09:45.119901 ngclearn-1.0b2/setup.cfg
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.783771 ngclearn-1.0b3/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      368 2024-03-27 21:42:18.000000 ngclearn-1.0b3/AUTHORS
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1548 2024-03-27 21:42:18.000000 ngclearn-1.0b3/LICENSE
+-rw-r--r--   0 ago       (1001) ago       (1001)     8238 2024-04-14 20:41:22.783771 ngclearn-1.0b3/PKG-INFO
+-rw-rw-r--   0 ago       (1001) ago       (1001)     6514 2024-04-14 20:41:04.000000 ngclearn-1.0b3/README.md
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.775771 ngclearn-1.0b3/ngclearn/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      706 2024-03-29 23:12:24.000000 ngclearn-1.0b3/ngclearn/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.775771 ngclearn-1.0b3/ngclearn/commands/
+-rw-rw-r--   0 ago       (1001) ago       (1001)       33 2024-03-28 23:58:59.000000 ngclearn-1.0b3/ngclearn/commands/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.775771 ngclearn-1.0b3/ngclearn/components/
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1087 2024-04-04 05:00:32.000000 ngclearn-1.0b3/ngclearn/components/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1081 2024-03-28 22:29:48.000000 ngclearn-1.0b3/ngclearn/components/baseComponentTemplate.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/components/input_encoders/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      118 2024-03-30 04:48:51.000000 ngclearn-1.0b3/ngclearn/components/input_encoders/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     3576 2024-03-30 04:48:51.000000 ngclearn-1.0b3/ngclearn/components/input_encoders/bernoulliCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     8904 2024-04-01 16:58:48.000000 ngclearn-1.0b3/ngclearn/components/input_encoders/latencyCell.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     3933 2024-03-30 20:38:16.000000 ngclearn-1.0b3/ngclearn/components/input_encoders/poissonCell.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/components/neurons/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      486 2024-04-01 02:25:22.000000 ngclearn-1.0b3/ngclearn/components/neurons/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/components/neurons/graded/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      178 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/components/neurons/graded/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     5403 2024-04-09 02:58:27.000000 ngclearn-1.0b3/ngclearn/components/neurons/graded/gaussianErrorCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     5439 2024-04-09 02:58:27.000000 ngclearn-1.0b3/ngclearn/components/neurons/graded/laplacianErrorCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     9968 2024-04-09 02:58:27.000000 ngclearn-1.0b3/ngclearn/components/neurons/graded/rateCell.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/components/neurons/spiking/
+-rw-rw-r--   0 ago       (1001) ago       (1001)    11036 2024-03-28 22:31:05.000000 ngclearn-1.0b3/ngclearn/components/neurons/spiking/LIFCell.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)      247 2024-04-01 02:25:22.000000 ngclearn-1.0b3/ngclearn/components/neurons/spiking/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     8887 2024-04-07 17:56:32.000000 ngclearn-1.0b3/ngclearn/components/neurons/spiking/fitzhughNagumoCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)    11228 2024-04-06 18:49:10.000000 ngclearn-1.0b3/ngclearn/components/neurons/spiking/izhikevichCell.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)    11707 2024-03-28 22:31:11.000000 ngclearn-1.0b3/ngclearn/components/neurons/spiking/quadLIFCell.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)    14148 2024-04-13 21:17:29.000000 ngclearn-1.0b3/ngclearn/components/neurons/spiking/sLIFCell.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/components/other/
+-rw-rw-r--   0 ago       (1001) ago       (1001)       64 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/components/other/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     4379 2024-04-09 02:58:27.000000 ngclearn-1.0b3/ngclearn/components/other/expKernel.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     5084 2024-04-09 02:58:27.000000 ngclearn-1.0b3/ngclearn/components/other/varTrace.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/components/synapses/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      160 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/components/synapses/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/components/synapses/hebbian/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/components/synapses/hebbian/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     8378 2024-03-28 22:31:56.000000 ngclearn-1.0b3/ngclearn/components/synapses/hebbian/expSTDPSynapse.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)    10875 2024-04-13 20:58:40.000000 ngclearn-1.0b3/ngclearn/components/synapses/hebbian/hebbianSynapse.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     9793 2024-04-09 23:34:39.000000 ngclearn-1.0b3/ngclearn/components/synapses/hebbian/traceSTDPSynapse.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)      263 2024-03-29 00:03:17.000000 ngclearn-1.0b3/ngclearn/components/wrappers.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/utils/
+-rwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/utils/__init__.py
+-rw-r--r--   0 ago       (1001) ago       (1001)     3232 2024-04-05 17:47:38.000000 ngclearn-1.0b3/ngclearn/utils/data_loader.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/utils/density/
+-rw-r--r--   0 ago       (1001) ago       (1001)        0 2024-03-28 00:06:24.000000 ngclearn-1.0b3/ngclearn/utils/density/__init__.py
+-rw-r--r--   0 ago       (1001) ago       (1001)     2816 2024-03-28 02:06:50.000000 ngclearn-1.0b3/ngclearn/utils/density/gmm.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/utils/diffeq/
+-rw-rw-r--   0 ago       (1001) ago       (1001)        0 2024-04-06 17:34:24.000000 ngclearn-1.0b3/ngclearn/utils/diffeq/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     5253 2024-04-06 22:55:59.000000 ngclearn-1.0b3/ngclearn/utils/diffeq/ode_utils.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     1629 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/utils/io_utils.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     5470 2024-04-12 02:40:59.000000 ngclearn-1.0b3/ngclearn/utils/metric_utils.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)    18320 2024-04-12 15:57:53.000000 ngclearn-1.0b3/ngclearn/utils/model_utils.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/utils/optim/
+-rw-rw-r--   0 ago       (1001) ago       (1001)       46 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/utils/optim/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     3090 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/utils/optim/adam.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)      783 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/utils/optim/opt.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     1122 2024-04-05 17:34:57.000000 ngclearn-1.0b3/ngclearn/utils/optim/sgd.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     3164 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/utils/patch_utils.py
+-rw-r--r--   0 ago       (1001) ago       (1001)     3809 2024-04-12 16:30:37.000000 ngclearn-1.0b3/ngclearn/utils/surrogate_fx.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/utils/viz/
+-rw-rw-r--   0 ago       (1001) ago       (1001)        0 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/utils/viz/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     3382 2024-04-08 02:28:58.000000 ngclearn-1.0b3/ngclearn/utils/viz/dim_reduce.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     6699 2024-04-03 17:27:35.000000 ngclearn-1.0b3/ngclearn/utils/viz/raster.py
+-rw-r--r--   0 ago       (1001) ago       (1001)     2513 2024-04-03 17:26:57.000000 ngclearn-1.0b3/ngclearn/utils/viz/spike_plot.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     4922 2024-03-30 16:17:15.000000 ngclearn-1.0b3/ngclearn/utils/viz/synapse_plot.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn.egg-info/
+-rw-r--r--   0 ago       (1001) ago       (1001)     8238 2024-04-14 20:41:22.000000 ngclearn-1.0b3/ngclearn.egg-info/PKG-INFO
+-rw-rw-r--   0 ago       (1001) ago       (1001)     2119 2024-04-14 20:41:22.000000 ngclearn-1.0b3/ngclearn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)        1 2024-04-14 20:41:22.000000 ngclearn-1.0b3/ngclearn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-04-14 20:41:22.000000 ngclearn-1.0b3/ngclearn.egg-info/requires.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)       28 2024-04-14 20:41:22.000000 ngclearn-1.0b3/ngclearn.egg-info/top_level.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1838 2024-04-14 20:40:42.000000 ngclearn-1.0b3/pyproject.toml
+-rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-03-30 18:06:06.000000 ngclearn-1.0b3/requirements.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)       38 2024-04-14 20:41:22.783771 ngclearn-1.0b3/setup.cfg
```

### Comparing `ngclearn-1.0b2/LICENSE` & `ngclearn-1.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b2/PKG-INFO` & `ngclearn-1.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngclearn
-Version: 1.0b2
+Version: 1.0b3
 Summary: Simulation software for building and analyzing arbitrary predictive coding, spiking network, and biomimetic neural systems.
 Author-email: Alexander Ororbia <ago@cs.rit.edu>, William Gebhardt <wdg1351@rit.edu>
 License: BSD-3-Clause License
 Project-URL: Homepage, https://github.com/NACLab/ngc-learn
 Project-URL: Documentation, https://ngc-learn.readthedocs.io/
 Project-URL: Lab Page, https://www.cs.rit.edu/~ago/nac_lab.html
 Project-URL: Changelog, https://github.com/NACLab/ngc-learn/blob/main/history.txt
@@ -48,15 +48,17 @@
 
 It is currently maintained by the
 <a href="https://www.cs.rit.edu/~ago/nac_lab.html">Neural Adaptive Computing (NAC) laboratory</a>.
 
 ## <b>Documentation</b>
 
 Official documentation, including tutorials, can be found
-<a href="https://ngc-learn.readthedocs.io/en/latest/#">here</a>.
+<a href="https://ngc-learn.readthedocs.io/en/latest/#">here</a>. The model museum repo, 
+which implements several historical models, can be found 
+<a href="https://github.com/NACLab/ngc-museum">here</a>.
 
 The official blog-post related to the source paper behind this software library
 can be found
 <a href="https://go.nature.com/3rgl1K8">here</a>.<br>
 You can find the related paper <a href="https://www.nature.com/articles/s41467-022-29632-7">right here</a>, which
 was selected to appear in the Nature <i>Neuromorphic Hardware and Computing Collection</i> in 2023 and was
 chosen as one of the <i>Editors' Highlights for Applied Physics and Mathematics</i> in 2022.
@@ -90,15 +92,15 @@
 <!-- (Note: if using the `_generate_patch_set()` within the
 image patching utilities, then Patchify will be needed).-->
 
 ### User Installation
 
 <i>Setup</i>: The easiest way to install ngc-learn (CPU version) is through <code>pip</code>:
 <pre>
-$ python install ngclearn
+$ pip install ngclearn
 </pre>
 
 The documentation includes more detailed
 <a href="https://ngc-learn.readthedocs.io/en/latest/installation.html">installation instructions</a>.
 Note that this library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and 20.04.
 
 <!--
@@ -166,15 +168,15 @@
 If you are working on and developing with ngc-learn pulled from the github
 repo, then run the following command to set up an editable install:
 <pre>
 $ python install -e .
 </pre>
 
 **Version:**<br>
-1.0.2-Beta <!-- -Alpha -->
+1.0.3-Beta <!-- -Alpha -->
 
 Author:
 Alexander G. Ororbia II<br>
 Director, Neural Adaptive Computing (NAC) Laboratory<br>
 Rochester Institute of Technology, Department of Computer Science
 
 ## <b>Copyright:</b>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ngclearn Version: 1.0b2 Summary: Simulation
+Metadata-Version: 2.1 Name: ngclearn Version: 1.0b3 Summary: Simulation
 software for building and analyzing arbitrary predictive coding, spiking
 network, and biomimetic neural systems. Author-email: Alexander Ororbia
 cs.rit.edu>, William Gebhardt
 rit.edu> License: BSD-3-Clause License Project-URL: Homepage, https://
 github.com/NACLab/ngc-learn Project-URL: Documentation, https://ngc-
 learn.readthedocs.io/ Project-URL: Lab Page, https://www.cs.rit.edu/~ago/
 nac_lab.html Project-URL: Changelog, https://github.com/NACLab/ngc-learn/blob/
@@ -33,31 +33,32 @@
 [docs/images/ngc-learn-logo.png]nnggcc--lleeaarrnn is a Python library for building,
 simulating, and analyzing biomimetic systems, neurobiological agents, spiking
 neuronal networks, predictive coding circuitry, and models that learn via
 biologically-plausible forms of credit assignment. This simulation toolkit is
 built on top of JAX and is distributed under the 3-Clause BSD license. It is
 currently maintained by the _N_e_u_r_a_l_ _A_d_a_p_t_i_v_e_ _C_o_m_p_u_t_i_n_g_ _(_N_A_C_)_ _l_a_b_o_r_a_t_o_r_y. ##
 DDooccuummeennttaattiioonn Official documentation, including tutorials, can be found _h_e_r_e.
-The official blog-post related to the source paper behind this software library
-can be found _h_e_r_e.
+The model museum repo, which implements several historical models, can be found
+_h_e_r_e. The official blog-post related to the source paper behind this software
+library can be found _h_e_r_e.
 You can find the related paper _r_i_g_h_t_ _h_e_r_e, which was selected to appear in the
 Nature Neuromorphic Hardware and Computing Collection in 2023 and was chosen as
 one of the Editors' Highlights for Applied Physics and Mathematics in 2022. ##
 Installation ### Dependencies ngc-learn requires: 1) Python (>=3.10) 2) NumPy
 (>=1.26.0) 3) SciPy (>=1.7.0) 4) ngcsimlib (>=0.2.b1), (visit official page
 _h_e_r_e) 5) JAX (>= 0.4.18) (to enable GPU use, make sure to install one of the
 CUDA variants) --- ngc-learn 1.0.beta0 and later require Python 3.10 or newer
 as well as ngcsimlib >=0.2.b2. ngc-learn's plotting capabilities (routines
 within `ngclearn.utils.viz`) require Matplotlib (>=3.8.0) and imageio
 (>=2.31.5) and both plotting and density estimation tools (routines within
 ``ngclearn.utils.density``) will require Scikit-learn (>=0.24.2). Many of the
 tutorials will require Matplotlib (>=3.8.0), imageio (>=2.31.5), and Scikit-
 learn (>=0.24.2). ### User Installation Setup: The easiest way to install ngc-
 learn (CPU version) is through pip:
-$ python install ngclearn
+$ pip install ngclearn
 The documentation includes more detailed _i_n_s_t_a_l_l_a_t_i_o_n_ _i_n_s_t_r_u_c_t_i_o_n_s. Note that
 this library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and
 20.04. If the installation was successful, you should see the following if you
 test it against your Python interpreter, i.e., run the $ python command and
 complete the following sequence of steps as depicted in the screenshot below:
 [docs/images/test_ngclearn_install.png]Note: For access to the previous
 Tensorflow-2 version of ngc-learn (of which we no longer support), please visit
@@ -83,15 +84,15 @@
 [contributing guidelines](CONTRIBUTING.md). SSoouurrccee CCooddee You can check/pull the
 latest source code for this library via:
 $ git clone https://github.com/NACLab/ngc-learn.git
 If you are working on and developing with ngc-learn pulled from the github
 repo, then run the following command to set up an editable install:
 $ python install -e .
 **Version:**
-1.0.2-Beta Author: Alexander G. Ororbia II
+1.0.3-Beta Author: Alexander G. Ororbia II
 Director, Neural Adaptive Computing (NAC) Laboratory
 Rochester Institute of Technology, Department of Computer Science ## CCooppyyrriigghhtt::
 Copyright (C) 2021 The Neural Adaptive Computing Laboratory - All Rights
 Reserved
 You may use, distribute and modify this code under the terms of the BSD 3-
 clause license. You should have received a copy of the BSD 3-clause license
 with this software.
```

### Comparing `ngclearn-1.0b2/README.md` & `ngclearn-1.0b3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 
 It is currently maintained by the
 <a href="https://www.cs.rit.edu/~ago/nac_lab.html">Neural Adaptive Computing (NAC) laboratory</a>.
 
 ## <b>Documentation</b>
 
 Official documentation, including tutorials, can be found
-<a href="https://ngc-learn.readthedocs.io/en/latest/#">here</a>.
+<a href="https://ngc-learn.readthedocs.io/en/latest/#">here</a>. The model museum repo, 
+which implements several historical models, can be found 
+<a href="https://github.com/NACLab/ngc-museum">here</a>.
 
 The official blog-post related to the source paper behind this software library
 can be found
 <a href="https://go.nature.com/3rgl1K8">here</a>.<br>
 You can find the related paper <a href="https://www.nature.com/articles/s41467-022-29632-7">right here</a>, which
 was selected to appear in the Nature <i>Neuromorphic Hardware and Computing Collection</i> in 2023 and was
 chosen as one of the <i>Editors' Highlights for Applied Physics and Mathematics</i> in 2022.
@@ -52,15 +54,15 @@
 <!-- (Note: if using the `_generate_patch_set()` within the
 image patching utilities, then Patchify will be needed).-->
 
 ### User Installation
 
 <i>Setup</i>: The easiest way to install ngc-learn (CPU version) is through <code>pip</code>:
 <pre>
-$ python install ngclearn
+$ pip install ngclearn
 </pre>
 
 The documentation includes more detailed
 <a href="https://ngc-learn.readthedocs.io/en/latest/installation.html">installation instructions</a>.
 Note that this library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and 20.04.
 
 <!--
@@ -128,15 +130,15 @@
 If you are working on and developing with ngc-learn pulled from the github
 repo, then run the following command to set up an editable install:
 <pre>
 $ python install -e .
 </pre>
 
 **Version:**<br>
-1.0.2-Beta <!-- -Alpha -->
+1.0.3-Beta <!-- -Alpha -->
 
 Author:
 Alexander G. Ororbia II<br>
 Director, Neural Adaptive Computing (NAC) Laboratory<br>
 Rochester Institute of Technology, Department of Computer Science
 
 ## <b>Copyright:</b>
```

#### html2text {}

```diff
@@ -9,31 +9,32 @@
 latestdoi/483413212) [docs/images/ngc-learn-logo.png]nnggcc--lleeaarrnn is a Python
 library for building, simulating, and analyzing biomimetic systems,
 neurobiological agents, spiking neuronal networks, predictive coding circuitry,
 and models that learn via biologically-plausible forms of credit assignment.
 This simulation toolkit is built on top of JAX and is distributed under the 3-
 Clause BSD license. It is currently maintained by the _N_e_u_r_a_l_ _A_d_a_p_t_i_v_e_ _C_o_m_p_u_t_i_n_g
 _(_N_A_C_)_ _l_a_b_o_r_a_t_o_r_y. ## DDooccuummeennttaattiioonn Official documentation, including tutorials,
-can be found _h_e_r_e. The official blog-post related to the source paper behind
-this software library can be found _h_e_r_e.
+can be found _h_e_r_e. The model museum repo, which implements several historical
+models, can be found _h_e_r_e. The official blog-post related to the source paper
+behind this software library can be found _h_e_r_e.
 You can find the related paper _r_i_g_h_t_ _h_e_r_e, which was selected to appear in the
 Nature Neuromorphic Hardware and Computing Collection in 2023 and was chosen as
 one of the Editors' Highlights for Applied Physics and Mathematics in 2022. ##
 Installation ### Dependencies ngc-learn requires: 1) Python (>=3.10) 2) NumPy
 (>=1.26.0) 3) SciPy (>=1.7.0) 4) ngcsimlib (>=0.2.b1), (visit official page
 _h_e_r_e) 5) JAX (>= 0.4.18) (to enable GPU use, make sure to install one of the
 CUDA variants) --- ngc-learn 1.0.beta0 and later require Python 3.10 or newer
 as well as ngcsimlib >=0.2.b2. ngc-learn's plotting capabilities (routines
 within `ngclearn.utils.viz`) require Matplotlib (>=3.8.0) and imageio
 (>=2.31.5) and both plotting and density estimation tools (routines within
 ``ngclearn.utils.density``) will require Scikit-learn (>=0.24.2). Many of the
 tutorials will require Matplotlib (>=3.8.0), imageio (>=2.31.5), and Scikit-
 learn (>=0.24.2). ### User Installation Setup: The easiest way to install ngc-
 learn (CPU version) is through pip:
-$ python install ngclearn
+$ pip install ngclearn
 The documentation includes more detailed _i_n_s_t_a_l_l_a_t_i_o_n_ _i_n_s_t_r_u_c_t_i_o_n_s. Note that
 this library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and
 20.04. If the installation was successful, you should see the following if you
 test it against your Python interpreter, i.e., run the $ python command and
 complete the following sequence of steps as depicted in the screenshot below:
 [docs/images/test_ngclearn_install.png]Note: For access to the previous
 Tensorflow-2 version of ngc-learn (of which we no longer support), please visit
@@ -59,15 +60,15 @@
 [contributing guidelines](CONTRIBUTING.md). SSoouurrccee CCooddee You can check/pull the
 latest source code for this library via:
 $ git clone https://github.com/NACLab/ngc-learn.git
 If you are working on and developing with ngc-learn pulled from the github
 repo, then run the following command to set up an editable install:
 $ python install -e .
 **Version:**
-1.0.2-Beta Author: Alexander G. Ororbia II
+1.0.3-Beta Author: Alexander G. Ororbia II
 Director, Neural Adaptive Computing (NAC) Laboratory
 Rochester Institute of Technology, Department of Computer Science ## CCooppyyrriigghhtt::
 Copyright (C) 2021 The Neural Adaptive Computing Laboratory - All Rights
 Reserved
 You may use, distribute and modify this code under the terms of the BSD 3-
 clause license. You should have received a copy of the BSD 3-clause license
 with this software.
```

### Comparing `ngclearn-1.0b2/ngclearn/__init__.py` & `ngclearn-1.0b3/ngclearn/__init__.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b2/ngclearn/components/__init__.py` & `ngclearn-1.0b3/ngclearn/components/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .neurons.graded.rateCell import RateCell
 from .neurons.graded.gaussianErrorCell import GaussianErrorCell
 from .neurons.graded.laplacianErrorCell import LaplacianErrorCell
 ## point to standard spiking cell component types
 from .neurons.spiking.sLIFCell import SLIFCell
 from .neurons.spiking.LIFCell import LIFCell
 from .neurons.spiking.quadLIFCell import QuadLIFCell
+from .neurons.spiking.fitzhughNagumoCell import FitzhughNagumoCell
 from .neurons.spiking.izhikevichCell import IzhikevichCell
 ## point to transformer/operater component types
 from .other.varTrace import VarTrace
 from .other.expKernel import ExpKernel
 ## point to input encoder component types
 from .input_encoders.bernoulliCell import BernoulliCell
 from .input_encoders.poissonCell import PoissonCell
```

### Comparing `ngclearn-1.0b2/ngclearn/components/baseComponentTemplate.py` & `ngclearn-1.0b3/ngclearn/components/baseComponentTemplate.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b2/ngclearn/components/input_encoders/bernoulliCell.py` & `ngclearn-1.0b3/ngclearn/components/input_encoders/bernoulliCell.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b2/ngclearn/components/input_encoders/latencyCell.py` & `ngclearn-1.0b3/ngclearn/components/input_encoders/latencyCell.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     _tols = (1. - s) * tols + (s * t)
     return _tols
 
 @partial(jit, static_argnums=[5])
 def calc_spike_times_linear(data, tau, thr, first_spk_t, num_steps=1.,
                             normalize=False):
     """
-    Computes spike times from data according to a
+    Computes spike times from data according to a linear latency encoding scheme.
 
     Args:
         data: pattern data to convert to spikes/times
 
         tau: latency coding time constant
 
         thr: latency coding threshold value
@@ -54,15 +54,15 @@
     stimes = clamp_max(stimes, max_bound) ## apply upper bound
     return stimes + first_spk_t
 
 @partial(jit, static_argnums=[6])
 def calc_spike_times_nonlinear(data, tau, thr, first_spk_t, eps=1e-7,
                                num_steps=1., normalize=False):
     """
-    Extracts a spike from a latency-coding spike train.
+    Computes spike times from data according to a logarithmic encoding scheme.
 
     Args:
         data: pattern data to convert to spikes/times
 
         tau: latency coding time constant
 
         thr: latency coding threshold value
@@ -124,14 +124,26 @@
         tau: time constant for model used to calculate firing time (Default: 1 ms)
 
         threshold: sensory input features below this threhold value will fire at
             final step in time of this latency coded spike train
 
         first_spike_time: time of first allowable spike (ms) (Default: 0 ms)
 
+        linearize: should the linear latency encoding scheme be used? (otherwise,
+            defaults to logarithmic latency encoding)
+
+        normalize: normalize the latency code such that final spike(s) occur
+            a pre-specified number of simulation steps "num_steps"? (Default: False)
+
+            :Note: if this set to True, you will need to choose a useful value
+                for the "num_steps" argument (>1), depending on how many steps simulated
+
+        num_steps: number of discrete time steps to consider for normalized latency
+            code (only useful if "normalize" is set to True) (Default: 1)
+
         key: PRNG key to control determinism of any underlying synapses
             associated with this cell
 
         useVerboseDict: triggers slower, verbose dictionary mode (Default: False)
     """
 
     ## Class Methods for Compartment Names
@@ -170,29 +182,30 @@
 
     @timeOfLastSpike.setter
     def timeOfLastSpike(self, t):
         self.compartments[self.timeOfLastSpikeCompartmentName()] = t
 
     # Define Functions
     def __init__(self, name, n_units, tau=1., threshold=0.01, first_spike_time=0.,
-                 key=None, useVerboseDict=False, **kwargs):
+                 linearize=False, normalize=False, num_steps=1., key=None,
+                 useVerboseDict=False, **kwargs):
         super().__init__(name, useVerboseDict, **kwargs)
 
         ##Random Number Set up
         self.key = key
         if self.key is None:
             self.key = random.PRNGKey(time.time_ns())
 
         self.first_spike_time = first_spike_time
         self.tau = tau
         self.threshold = threshold
-        self.linearize = False
+        self.linearize = linearize
         ## normalize latency code s.t. final spike(s) occur w/in num_steps
-        self.normalize = False
-        self.num_steps = 100.
+        self.normalize = normalize
+        self.num_steps = num_steps
 
         self.target_spike_times = None
         self._mask = None
 
         ##Layer Size Setup
         self.batch_size = 1
         self.n_units = n_units
```

### Comparing `ngclearn-1.0b2/ngclearn/components/input_encoders/poissonCell.py` & `ngclearn-1.0b3/ngclearn/components/input_encoders/poissonCell.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b2/ngclearn/components/neurons/graded/gaussianErrorCell.py` & `ngclearn-1.0b3/ngclearn/components/neurons/graded/gaussianErrorCell.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,40 +12,41 @@
         dt: integration time constant
 
         targ: target pattern value
 
         mu: prediction value
 
     Returns:
-        derivative w.r.t. mean "dmu", derivative w.r.t. target dtarg
+        derivative w.r.t. mean "dmu", derivative w.r.t. target dtarg, local loss
     """
     return run_gaussian_cell(dt, targ, mu)
 
 @jit
 def run_gaussian_cell(dt, targ, mu):
     """
     Moves Gaussian cell dynamics one step forward. Specifically, this
     routine emulates the error unit behavior of the local cost functional:
 
-    | L(targ, mu) = (1/2) * ||targ - mu||^2_2
+    | L(targ, mu) = -(1/2) * ||targ - mu||^2_2
     | or log likelihood of the multivariate Gaussian with identity covariance
 
     Args:
         dt: integration time constant
 
         targ: target pattern value
 
         mu: prediction value
 
     Returns:
-        derivative w.r.t. mean "dmu", derivative w.r.t. target dtarg
+        derivative w.r.t. mean "dmu", derivative w.r.t. target dtarg, loss
     """
     dmu = (targ - mu) # e (error unit)
     dtarg = -dmu # reverse of e
-    return dmu, dtarg
+    L = -jnp.sum(jnp.square(dmu)) * 0.5
+    return dmu, dtarg, L
 
 class GaussianErrorCell(Component): ## Rate-coded/real-valued error unit/cell
     """
     A simple (non-spiking) Gaussian error cell - this is a fixed-point solution
     of a mismatch signal.
 
     Args:
@@ -61,14 +62,18 @@
             associated with this cell
 
         useVerboseDict: triggers slower, verbose dictionary mode (Default: False)
     """
 
     ## Class Methods for Compartment Names
     @classmethod
+    def lossName(cls):
+        return "L"
+
+    @classmethod
     def inputCompartmentName(cls):
         return 'j' ## electrical current
 
     @classmethod
     def outputCompartmentName(cls):
         return 'e' ## rate-coded output
 
@@ -90,14 +95,22 @@
 
     @classmethod
     def modulatorName(cls):
         return 'modulator'
 
     ## Bind Properties to Compartments for ease of use
     @property
+    def loss(self):
+        return self.compartments.get(self.lossName(), None)
+
+    @loss.setter
+    def loss(self, inp):
+        self.compartments[self.lossName()] = inp
+
+    @property
     def mean(self):
         return self.compartments.get(self.meanName(), None)
 
     @mean.setter
     def mean(self, inp):
         self.compartments[self.meanName()] = inp
 
@@ -142,26 +155,24 @@
         self.key = key
         if self.key is None:
             self.key = random.PRNGKey(time.time_ns())
 
         ##Layer Size Setup
         self.n_units = n_units
         self.batch_size = 1
-
-        ## Set up bundle for multiple inputs of current
         self.reset()
 
     def verify_connections(self):
-        #self.metadata.check_incoming_connections(self.inputCompartmentName(), min_connections=1)
         self.metadata.check_incoming_connections(self.meanName(), min_connections=1)
         self.metadata.check_incoming_connections(self.targetName(), min_connections=1)
 
     def advance_state(self, t, dt, **kwargs):
-        ## currently only Gaussian error cells supported
-        self.derivMean, self.derivTarget = run_cell(dt, self.target, self.mean)
+        ## compute Gaussian error cell output
+        self.derivMean, self.derivTarget, self.loss = \
+            run_cell(dt, self.target, self.mean)
         if self.modulator is not None:
             self.derivMean = self.derivMean * self.modulator
             self.derivTarget = self.derivTarget * self.modulator
             self.modulator = None ## use and consume modulator
 
     def reset(self, **kwargs):
         self.derivMean = jnp.zeros((self.batch_size, self.n_units))
```

### Comparing `ngclearn-1.0b2/ngclearn/components/neurons/graded/laplacianErrorCell.py` & `ngclearn-1.0b3/ngclearn/components/neurons/graded/laplacianErrorCell.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,40 +12,41 @@
         dt: integration time constant
 
         targ: target pattern value
 
         mu: prediction value
 
     Returns:
-        derivative w.r.t. mean "dmu", derivative w.r.t. target dtarg
+        derivative w.r.t. mean "dmu", derivative w.r.t. target dtarg, local loss
     """
     return run_laplacian_cell(dt, targ, mu)
 
 @jit
 def run_laplacian_cell(dt, targ, mu):
     """
     Moves Laplacian cell dynamics one step forward. Specifically, this
     routine emulates the error unit behavior of the local cost functional:
 
-    | L(targ, mu) = ||targ - mu||_1
+    | L(targ, mu) = -||targ - mu||_1
     | or log likelihood of the Laplace distribution with identity scale
 
     Args:
         dt: integration time constant
 
         targ: target pattern value
 
         mu: prediction value
 
     Returns:
-        derivative w.r.t. mean "dmu", derivative w.r.t. target dtarg
+        derivative w.r.t. mean "dmu", derivative w.r.t. target dtarg, loss
     """
     dmu = jnp.sign(targ - mu) # e (error unit)
     dtarg = -dmu # reverse of e
-    return dmu, dtarg
+    L = -jnp.sum(jnp.abs(dmu)) # technically, this is mean absolute error
+    return dmu, dtarg, L
 
 class LaplacianErrorCell(Component): ## Rate-coded/real-valued error unit/cell
     """
     A simple (non-spiking) Laplacian error cell - this is a fixed-point solution
     of a mismatch signal.
 
     Args:
@@ -61,14 +62,18 @@
             associated with this cell
 
         useVerboseDict: triggers slower, verbose dictionary mode (Default: False)
     """
 
     ## Class Methods for Compartment Names
     @classmethod
+    def lossName(cls):
+        return "L"
+
+    @classmethod
     def inputCompartmentName(cls):
         return 'j' ## electrical current
 
     @classmethod
     def outputCompartmentName(cls):
         return 'e' ## rate-coded output
 
@@ -90,14 +95,22 @@
 
     @classmethod
     def modulatorName(cls):
         return 'modulator'
 
     ## Bind Properties to Compartments for ease of use
     @property
+    def loss(self):
+        return self.compartments.get(self.lossName(), None)
+
+    @loss.setter
+    def loss(self, inp):
+        self.compartments[self.lossName()] = inp
+
+    @property
     def mean(self):
         return self.compartments.get(self.meanName(), None)
 
     @mean.setter
     def mean(self, inp):
         self.compartments[self.meanName()] = inp
 
@@ -142,26 +155,24 @@
         self.key = key
         if self.key is None:
             self.key = random.PRNGKey(time.time_ns())
 
         ##Layer Size Setup
         self.n_units = n_units
         self.batch_size = 1
-
-        ## Set up bundle for multiple inputs of current
         self.reset()
 
     def verify_connections(self):
-        #self.metadata.check_incoming_connections(self.inputCompartmentName(), min_connections=1)
         self.metadata.check_incoming_connections(self.meanName(), min_connections=1)
         self.metadata.check_incoming_connections(self.targetName(), min_connections=1)
 
     def advance_state(self, t, dt, **kwargs):
-        ## currently only Gaussian error cells supported
-        self.derivMean, self.derivTarget = run_cell(dt, self.target, self.mean)
+        ## compute Laplacian/MAE error cell output
+        self.derivMean, self.derivTarget, self.loss = \
+            run_cell(dt, self.target, self.mean)
         if self.modulator is not None:
             self.derivMean = self.derivMean * self.modulator
             self.derivTarget = self.derivTarget * self.modulator
             self.modulator = None ## use and consume modulator
 
     def reset(self, **kwargs):
         self.derivMean = jnp.zeros((self.batch_size, self.n_units))
```

### Comparing `ngclearn-1.0b2/ngclearn/components/neurons/graded/rateCell.py` & `ngclearn-1.0b3/ngclearn/components/neurons/spiking/fitzhughNagumoCell.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,201 +1,276 @@
 from ngcsimlib.component import Component
-from jax import numpy as jnp, random, jit, nn
+from jax import numpy as jnp, random, jit
 from functools import partial
-from ngclearn.utils.model_utils import create_function
-import time, sys
+import time
+from ngclearn.utils.diffeq.ode_utils import get_integrator_code, \
+                                            step_euler, step_rk2
 
 @jit
-def modulate(j, dfx_val):
+def update_times(t, s, tols):
     """
-    Apply a signal modulator to j (typically of the form of a derivative/dampening function)
+    Updates time-of-last-spike (tols) variable.
 
     Args:
-        j: current/stimulus value to modulate
+        t: current time (a scalar/int value)
 
-        dfx_val: modulator signal
+        s: binary spike vector
+
+        tols: current time-of-last-spike variable
 
     Returns:
-        modulated j value
+        updated tols variable
     """
-    return j * dfx_val
+    _tols = (1. - s) * tols + (s * t)
+    return _tols
+
+@jit
+def _dfv_internal(j, v, w, a, b, g, tau_m): ## raw voltage dynamics
+    dv_dt = v - jnp.power(v, 3)/g - w + j ## dv/dt
+    dv_dt = dv_dt * (1./tau_m)
+    return dv_dt
+
+def _dfv(v, params): ## voltage dynamics wrapper
+    j, w, a, b, g, tau_m = params
+    dv_dt = _dfv_internal(j, v, w, a, b, g, tau_m)
+    return dv_dt
+
+@jit
+def _dfw_internal(j, v, w, a, b, g, tau_w): ## raw recovery dynamics
+    dw_dt = v + a - b * w ## dw/dt
+    dw_dt = dw_dt * (1./tau_w)
+    return dw_dt
+
+def _dfw(w, params): ## recovery dynamics wrapper
+    j, v, a, b, g, tau_m = params
+    dv_dt = _dfw_internal(j, v, w, a, b, g, tau_m)
+    return dv_dt
 
-@partial(jit, static_argnums=[4,5,6])
-def run_cell(dt, j, j_td, z, tau_m, leak_gamma=0., beta=1.):
+@jit
+def _emit_spike(v, v_thr):
+    s = (v > v_thr).astype(jnp.float32)
+    return s
+
+#@partial(jit, static_argnums=[10])
+def run_cell(dt, j, v, w, v_thr, tau_m, tau_w, a, b, g=3., integType=0):
     """
-    Runs leaky rate-coded state dynamics one step in time.
 
     Args:
         dt: integration time constant
 
-        j: input (bottom-up) electrical/stimulus current
+        j: electrical current
 
-        j_td: modulatory (top-down) electrical/stimulus pressure
+        v: membrane potential / voltage
 
-        z: current value of membrane/state
+        w: recovery variable value(s)
 
-        tau_m: membrane/state time constant
+        v_thr: voltage/membrane threshold (to obtain action potentials in terms
+            of binary spikes)
 
-        leak_gamma: strength of leak to apply to membrane/state
+        tau_m: membrane time constant
 
-        beta: dampening coefficient (Default: 1.)
+        tau_w: recover variable time constant (Default: 12.5 ms)
 
-    Returns:
-        New value of membrane/state for next time step
-    """
-    dz_dt = (-z * leak_gamma + (j + j_td))
-    _z = z * beta + dz_dt * (dt/tau_m)
-    return _z
+        a: dimensionless recovery variable shift factor "alpha" (Default: 0.7)
 
-@jit
-def run_cell_stateless(j):
-    """
-    A simplification of running a stateless set of dynamics over j (an identity
-    functional form of dynamics).
+        b: dimensionless recovery variable scale factor "beta" (Default: 0.8)
 
-    Args:
-        j: stimulus to do nothing to
+        g: power-term divisor 'gamma' (Default: 3.)
+
+        integType: integration type to use (0 --> Euler/RK1, 1 --> Midpoint/RK2)
 
     Returns:
-        the stimulus
+        updated voltage, updated recovery, spikes
     """
-    return j + 0
+    if integType == 1:
+        v_params = (j, w, a, b, g, tau_m)
+        _v = step_rk2(v, v_params, _dfv, dt)
+        w_params = (j, v, a, b, g, tau_w)
+        _w = step_rk2(w, w_params, _dfw, dt)
+    else: # integType == 0 (default -- Euler)
+        v_params = (j, w, a, b, g, tau_m)
+        _v = step_euler(v, v_params, _dfv, dt)
+        w_params = (j, v, a, b, g, tau_w)
+        _w = step_euler(w, w_params, _dfw, dt)
+    #s = (_v > v_thr).astype(jnp.float32)
+    s = _emit_spike(_v, v_thr)
+    return _v, _w, s
 
-class RateCell(Component): ## Rate-coded/real-valued cell
+class FitzhughNagumoCell(Component):
     """
-    A non-spiking cell driven by the gradient dynamics of neural generative
-    coding-driven predictive processing.
+    The Fitzhugh-Nagumo neuronal cell model; a two-variable simplification
+    of the Hodgkin-Huxley (squid axon) model. This cell model iteratively evolves
+    voltage "v" and recovery "w" (which represents the combined effects of
+    sodium channel deinactivation and potassium channel deactivation in the
+    Hodgkin-Huxley model).
+
+    The specific pair of differential equations that characterize this cell
+    are (for adjusting v and w, given current j, over time):
+
+    | tau_m * dv/dt = v - (v^3)/3 - w + j
+    | tau_w * dw/dt = v + a - b * w
+
+    | References:
+    | FitzHugh, Richard. "Impulses and physiological states in theoretical
+    | models of nerve membrane." Biophysical journal 1.6 (1961): 445-466.
+    |
+    | Nagumo, Jinichi, Suguru Arimoto, and Shuji Yoshizawa. "An active pulse
+    | transmission line simulating nerve axon." Proceedings of the IRE 50.10
+    | (1962): 2061-2070.
 
     Args:
         name: the string name of this cell
 
         n_units: number of cellular entities (neural population size)
 
-        tau_m: membrane/state time constant (milliseconds)
+        tau_m: membrane time constant
+
+        tau_w: recover variable time constant (Default: 12.5 ms)
+
+        alpha: dimensionless recovery variable shift factor "a" (Default: 0.7)
+
+        beta: dimensionless recovery variable scale factor "b" (Default: 0.8)
+
+        gamma: power-term divisor (Default: 3.)
+
+        v_thr: voltage/membrane threshold (to obtain action potentials in terms
+            of binary spikes)
 
-        leakRate: membrane/state leak value (Default: 0.)
+        v0: initial condition / reset for voltage
 
-        act_fx: string name of activation function/nonlinearity to use
+        w0: initial condition / reset for recovery
 
-        key: PRNG Key to control determinism of any underlying random values
+        integration_type: type of integration to use for this cell's dynamics;
+            current supported forms include "euler" (Euler/RK-1 integration)
+            and "midpoint" or "rk2" (midpoint method/RK-2 integration) (Default: "euler")
+
+            :Note: setting the integration type to the midpoint method will
+                increase the accuray of the estimate of the cell's evolution
+                at an increase in computational cost (and simulation time)
+
+        key: PRNG key to control determinism of any underlying synapses
             associated with this cell
 
         useVerboseDict: triggers slower, verbose dictionary mode (Default: False)
     """
 
     ## Class Methods for Compartment Names
     @classmethod
     def inputCompartmentName(cls):
-        return 'j' ## electrical current
+        return 'in'
 
     @classmethod
-    def outputCompartmentName(cls): # OR: activityName()
-        return 'zF' ## rate-coded output
+    def outputCompartmentName(cls):
+        return 'out'
 
     @classmethod
-    def pressureName(cls):
-        return 'j_td'
+    def voltageName(cls):
+        return 'v'
 
     @classmethod
-    def rateActivityName(cls):
-        return 'z'
+    def recoveryName(cls):
+        return 'w'
+
+    @classmethod
+    def timeOfLastSpikeCompartmentName(cls):
+        return 'tols'
 
     ## Bind Properties to Compartments for ease of use
     @property
     def inputCompartment(self):
         return self.compartments.get(self.inputCompartmentName(), None)
 
     @inputCompartment.setter
-    def inputCompartment(self, out):
-        self.compartments[self.inputCompartmentName()] = out
+    def inputCompartment(self, inp):
+        self.compartments[self.inputCompartmentName()] = inp
 
     @property
     def outputCompartment(self):
         return self.compartments.get(self.outputCompartmentName(), None)
 
     @outputCompartment.setter
     def outputCompartment(self, out):
         self.compartments[self.outputCompartmentName()] = out
 
     @property
-    def current(self):
-        return self.compartments.get(self.inputCompartmentName(), None)
-
-    @current.setter
-    def current(self, inp):
-        self.compartments[self.inputCompartmentName()] = inp
-
-    @property
-    def pressure(self):
-        return self.compartments.get(self.pressureName(), None)
+    def voltage(self):
+        return self.compartments.get(self.voltageName(), None)
 
-    @pressure.setter
-    def pressure(self, inp):
-        self.compartments[self.pressureName()] = inp
+    @voltage.setter
+    def voltage(self, t):
+        self.compartments[self.voltageName()] = t
 
     @property
-    def rateActivity(self):
-        return self.compartments.get(self.rateActivityName(), None)
+    def recovery(self):
+        return self.compartments.get(self.recoveryName(), None)
 
-    @rateActivity.setter
-    def rateActivity(self, out):
-        self.compartments[self.rateActivityName()] = out
+    @recovery.setter
+    def recovery(self, t):
+        self.compartments[self.recoveryName()] = t
 
     @property
-    def activity(self):
-        return self.compartments.get(self.outputCompartmentName(), None)
+    def timeOfLastSpike(self):
+        return self.compartments.get(self.timeOfLastSpikeCompartmentName(), None)
 
-    @activity.setter
-    def activity(self, out):
-        self.compartments[self.outputCompartmentName()] = out
+    @timeOfLastSpike.setter
+    def timeOfLastSpike(self, t):
+        self.compartments[self.timeOfLastSpikeCompartmentName()] = t
 
     # Define Functions
-    def __init__(self, name, n_units, tau_m, leakRate=0., act_fx="identity",
-                 key=None, useVerboseDict=False, directory=None, **kwargs):
+    def __init__(self, name, n_units, tau_m=1., tau_w=12.5, alpha=0.7,
+                 beta=0.8, gamma=3., v_thr=1.07, v0=0., w0=0.,
+                 integration_type="euler", key=None, useVerboseDict=False,
+                 **kwargs):
         super().__init__(name, useVerboseDict, **kwargs)
 
-        ##Random Number Set up
+        ## Random Number Set up
         self.key = key
         if self.key is None:
             self.key = random.PRNGKey(time.time_ns())
 
-        ## membrane parameter setup (affects ODE integration)
-        self.tau_m = tau_m ## membrane time constant -- setting to 0 triggers "stateless" mode
-        self.leakRate = leakRate ## degree to which rate neurons leak
+        ## Integration properties
+        self.integrationType = integration_type
+        self.intgFlag = get_integrator_code(self.integrationType)
+
+        ## Cell properties
+        self.tau_m = tau_m
+        self.tau_w = tau_w
+        self.alpha = alpha
+        self.beta = beta
+        self.gamma = gamma
+
+        self.v0 = v0 ## initial membrane potential/voltage condition
+        self.w0 = w0 ## initial w-parameter condition
+        self.v_thr = v_thr
 
-        ##Layer Size Setup
-        self.n_units = n_units
+        ## Layer Size Setup
         self.batch_size = 1
-
-        self.fx, self.dfx = create_function(fun_name=act_fx)
-
+        self.n_units = n_units
         self.reset()
 
     def verify_connections(self):
-        self.metadata.check_incoming_connections(self.inputCompartmentName(), min_connections=1)
+        pass
 
     def advance_state(self, t, dt, **kwargs):
-        if self.tau_m > 0.:
-            ### run one step of Euler integration over neuronal dynamics
-            ## Notes:
-            ## self.pressure <-- "top-down" expectation / contextual pressure
-            ## self.current <-- "bottom-up" data-dependent signal
-            dfx_val = self.dfx(self.rateActivity)
-            self.current = modulate(self.current, dfx_val)
-            self.rateActivity = run_cell(dt, self.current, self.pressure,
-                                         self.rateActivity, self.tau_m, leak_gamma=self.leakRate)
-            self.activity = self.fx(self.rateActivity)
-            self.current = None
-        else:
-            ## run in "stateless" mode (when no membrane time constant provided)
-            self.rateActivity = run_cell_stateless(self.current)
-            self.activity = self.fx(self.rateActivity)
-            #self.current = None
+        self.key, *subkeys = random.split(self.key, 2)
+
+        j = self.inputCompartment
+        v = self.voltage
+        w = self.recovery
+
+        v, w, s = run_cell(dt, j, v, w, self.v_thr, self.tau_m, self.tau_w, self.alpha,
+                           self.beta, self.gamma, self.intgFlag)
+
+        self.voltage = v
+        self.recovery = w
+        self.outputCompartment = s
+        self.timeOfLastSpike = update_times(t, self.outputCompartment, self.timeOfLastSpike)
 
     def reset(self, **kwargs):
-        self.current = jnp.zeros((self.batch_size, self.n_units))
-        self.pressure = jnp.zeros((self.batch_size, self.n_units))
-        self.rateActivity = jnp.zeros((self.batch_size, self.n_units))
-        self.activity = jnp.zeros((self.batch_size, self.n_units))
+        self.inputCompartment = None
+        self.voltage = jnp.zeros((self.batch_size, self.n_units)) + self.v0
+        self.recovery = jnp.zeros((self.batch_size, self.n_units)) + self.w0
+        self.outputCompartment = jnp.zeros((self.batch_size, self.n_units)) #None
+        self.timeOfLastSpike = jnp.zeros((self.batch_size, self.n_units))
 
     def save(self, **kwargs):
         pass
```

### Comparing `ngclearn-1.0b2/ngclearn/components/neurons/spiking/LIFCell.py` & `ngclearn-1.0b3/ngclearn/components/neurons/spiking/LIFCell.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b2/ngclearn/components/neurons/spiking/quadLIFCell.py` & `ngclearn-1.0b3/ngclearn/components/neurons/spiking/quadLIFCell.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b2/ngclearn/components/neurons/spiking/sLIFCell.py` & `ngclearn-1.0b3/ngclearn/components/neurons/spiking/sLIFCell.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from ngcsimlib.component import Component
 from jax import numpy as jnp, random, jit
 from functools import partial
 import time, sys
+from ngclearn.utils.surrogate_fx import secant_lif_estimator
 
 @jit
 def update_times(t, s, tols):
     """
     Updates time-of-last-spike (tols) variable.
 
     Args:
@@ -17,42 +18,14 @@
 
     Returns:
         updated tols variable
     """
     _tols = (1. - s) * tols + (s * t)
     return _tols
 
-@jit
-def apply_surrogate_dfx(j, c1=0.82, c2=0.08):
-    """
-    Applies a surrogate (derivative) function -- often used to approximate the
-    derivative through an action potential/spike's output value.
-
-    Args:
-        j: electrical current value
-
-        c1: control coefficient 1 (unnamed factor from paper - scales current
-            input; Default: 0.82 as in source paper)
-
-        c2: control coefficient 2 (unnamed factor from paper - scales, multiplicatively
-            with c1, the output the derivative surrogate; Default: 0.08 as in
-            source paper)
-
-    Returns:
-        surrogate output values (same shape as j)
-    """
-    # sech(x) = 1/cosh(x), cosh(x) = (e^x + e^(-x))/2
-    # c1 c2 sech^2(c2 j) for j > 0 and 0 for j <= 0
-    mask = (j > 0.).astype(jnp.float32)
-    dj = j * c2
-    cosh_j = (jnp.exp(dj) + jnp.exp(-dj))/2.
-    sech_j = 1./cosh_j #(cosh_x + 1e-6)
-    dv_dj = sech_j * (c1 * c2) # ~deriv w.r.t. j
-    return dv_dj * mask ## 0 if j < 0, otherwise, use dv/dj for j >= 0
-
 @partial(jit, static_argnums=[3,4])
 def modify_current(j, spikes, inh_weights, R_m, inh_R):
     """
     A simple function that modifies electrical current j via application of a
     scalar membrane resistance value and an approximate form of lateral inhibition.
     Note that if no inhibitory resistance is set (i.e., inh_R = 0), then no
     lateral inhibition is applied. Functionally, this routine carries out the
@@ -78,16 +51,51 @@
         modified electrical current value
     """
     _j = j * R_m
     if inh_R > 0.:
         _j = _j - (jnp.matmul(spikes, inh_weights) * inh_R)
     return _j
 
-@partial(jit, static_argnums=[6,7,8,9,10,11])
-def run_cell(dt, j, v, v_thr, tau_m, rfr, refract_T=1., thrGain=0.002,
+## co-routines for run_cell
+@partial(jit, static_argnums=[4,5,6])
+def _update_voltage(dt, j, v, rfr, tau_m, refract_T, v_min=None):
+    mask = (rfr >= refract_T).astype(jnp.float32) # get refractory mask
+    _v = (v + (-v + j) * (dt / tau_m)) * mask
+    if v_min is not None:
+        _v = jnp.maximum(v_min, _v)
+    #_v = v + (-v) * (dt / tau_m) + j * mask
+    return _v, mask
+
+@jit
+def _hyperpolarize(v, s):
+    _v = (1. - s) * v ## hyper-polarize cells
+    return _v
+
+@partial(jit, static_argnums=[3,4,5])
+def _update_threshold(dt, v_thr, spikes, thrGain=0.002, thrLeak=0.0005, rho_b = 0.):
+    ## update thresholds if applicable
+    if rho_b > 0.: ## run sparsity-enforcement threshold
+        dthr = jnp.sum(spikes, axis=1, keepdims=True) - 1.0
+        _v_thr = jnp.maximum(v_thr + dthr * rho_b, 0.025)
+    else: ## run simple adaptive threshold
+        thr_gain = spikes * thrGain
+        thr_leak = (v_thr * thrLeak)
+        _v_thr = v_thr + thr_gain - thr_leak
+    return _v_thr
+
+@partial(jit, static_argnums=[4])
+def _update_refract_and_spikes(dt, rfr, s, mask, sticky_spikes=False):
+    ## update refractory variables
+    _rfr = (rfr + dt) * (1. - s) + s * dt # set refract to dt
+    _s = s
+    if sticky_spikes == True: ## pin refractory spikes if configured
+        _s = s * mask + (1. - mask)
+    return _rfr, _s
+
+def run_cell(dt, j, v, v_thr, tau_m, rfr, spike_fx, refract_T=1., thrGain=0.002,
              thrLeak=0.0005, rho_b = 0., sticky_spikes=False, v_min=None):
     """
     Runs leaky integrator neuronal dynamics
 
     Args:
         dt: integration time constant (milliseconds, or ms)
 
@@ -97,14 +105,16 @@
 
         v_thr: voltage threshold value (at t)
 
         tau_m: cell membrane time constant
 
         rfr: refractory variable vector (one per neuronal cell)
 
+        spike_fx: spike emission function of form `spike_fx(v, v_thr)`
+
         refract_T: (relative) refractory time period (in ms; Default
             value is 1 ms)
 
         thrGain: the amount of threshold incremented per time step (if spike present)
 
         thrLeak: the amount of threshold value leaked per time step
 
@@ -114,33 +124,19 @@
         sticky_spikes: if True, then spikes are pinned at value of action potential
             (i.e., 1) for as long as the relative refractory occurs (this recovers
             the source paper's core spiking process)
 
     Returns:
         voltage(t+dt), spikes, threshold(t+dt), updated refactory variables
     """
-    mask = (rfr >= refract_T).astype(jnp.float32) # get refractory mask
-    new_voltage = (v + (-v + j) * (dt / tau_m)) * mask
-    if v_min is not None:
-        new_voltage = jnp.maximum(v_min, new_voltage)
-    #new_voltage = v + (-v) * (dt / tau_m) + j * mask
-    spikes = jnp.where(new_voltage > v_thr, 1, 0)
-    new_voltage = (1. - spikes) * new_voltage ## hyper-polarize cells
-    ## update thresholds if applicable
-    if rho_b > 0.: ## run sparsity-enforcement threshold
-        dthr = jnp.sum(spikes, axis=1, keepdims=True) - 1.0
-        new_thr = jnp.maximum(v_thr + dthr * rho_b, 0.025)
-    else: ## run simple adaptive threshold
-        thr_gain = spikes * thrGain
-        thr_leak = (v_thr * thrLeak)
-        new_thr = v_thr + thr_gain - thr_leak
-    ## update refractory variables
-    _rfr = (rfr + dt) * (1. - spikes)
-    if sticky_spikes == True: ## pin refractory spikes if configured
-        spikes = spikes * mask + (1. - mask)
+    new_voltage, mask = _update_voltage(dt, j, v, rfr, tau_m, refract_T, v_min)
+    spikes = spike_fx(new_voltage, v_thr)
+    new_voltage = _hyperpolarize(new_voltage, spikes)
+    new_thr = _update_threshold(dt, v_thr, spikes, thrGain, thrLeak, rho_b)
+    _rfr, spikes = _update_refract_and_spikes(dt, rfr, spikes, mask, sticky_spikes)
     return new_voltage, spikes, new_thr, _rfr
 
 class SLIFCell(Component): ## leaky integrate-and-fire cell
     """
     A spiking cell based on a simplified leaky integrate-and-fire (sLIF) model.
     This neuronal cell notably contains functionality required by the computational
     model employed by (Samadi et al., 2017, i.e., a surrogate derivative function
@@ -281,16 +277,16 @@
         return self.compartments.get(self.thresholdCompartmentName(), None)
 
     @threshold.setter
     def threshold(self, thr):
         self.compartments[self.thresholdCompartmentName()] = thr
 
     # Define Functions
-    def __init__(self, name, n_units, tau_m, R_m, thr, inhibit_R=6., thr_persist=False,
-                 thrGain=0.001, thrLeak=0.00005, rho_b=0., refract_T=1., sticky_spikes=True,
+    def __init__(self, name, n_units, tau_m, R_m, thr, inhibit_R=0., thr_persist=False,
+                 thrGain=0.0, thrLeak=0.0, rho_b=0., refract_T=0., sticky_spikes=False,
                  thr_jitter=0.05, key=None, useVerboseDict=False, directory=None, **kwargs):
         super().__init__(name, useVerboseDict, **kwargs)
 
         ##Random Number Set up
         self.key = key
         if self.key is None:
             self.key = random.PRNGKey(time.time_ns())
@@ -299,14 +295,17 @@
         self.tau_m = tau_m ## membrane time constant
         self.R_m = R_m ## resistance value
         self.refract_T = refract_T #5. # 2. ## refractory period  # ms
         self.v_min = -3.
         ## variable below determines if spikes pinned at 1 during refractory period?
         self.sticky_spikes = sticky_spikes
 
+        ## set up surrogate function for spike emission
+        self.spike_fx, self.d_spike_fx = secant_lif_estimator()
+
         ## create simple recurrent inhibitory pressure
         self.inh_R = inhibit_R ## lateral inhibitory magnitude
         self.key, subkey = random.split(self.key)
         self.inh_weights = random.uniform(subkey, (n_units, n_units), minval=0.025, maxval=1.)
         MV = 1. - jnp.eye(n_units)
         self.inh_weights = self.inh_weights * MV
 
@@ -341,22 +340,21 @@
         if self.refract is None:
             self.refract = jnp.zeros((self.batch_size, self.n_units)) + self.refract_T
         ## run one step of Euler integration over neuronal dynamics
         j_curr = self.current
         ## apply simplified inhibitory pressure
         j_curr = modify_current(j_curr, self.spikes, self.inh_weights, self.R_m, self.inh_R)
         self.current = j_curr # None ## store electrical current
-        self.surrogate = apply_surrogate_dfx(j_curr, c1=0.82, c2=0.08)
+        self.surrogate = self.d_spike_fx(j_curr, self.voltage, self.threshold, c1=0.82, c2=0.08)
         self.voltage, self.spikes, self.threshold, self.refract = \
             run_cell(dt, j_curr, self.voltage, self.threshold, self.tau_m,
-                     self.refract, self.refract_T, self.thrGain, self.thrLeak,
+                     self.refract, self.spike_fx, self.refract_T, self.thrGain, self.thrLeak,
                      self.rho_b, sticky_spikes=self.sticky_spikes, v_min=self.v_min)
         ## update tols
         self.timeOfLastSpike = update_times(t, self.spikes, self.timeOfLastSpike)
-        #self.timeOfLastSpike = (1 - self.spikes) * self.timeOfLastSpike + (self.spikes * t)
 
     def reset(self, **kwargs):
         self.voltage = jnp.zeros((self.batch_size, self.n_units))
         self.refract = jnp.zeros((self.batch_size, self.n_units)) + self.refract_T
         self.current = None
         self.surrogate = None
         self.timeOfLastSpike = jnp.zeros((self.batch_size, self.n_units))
```

### Comparing `ngclearn-1.0b2/ngclearn/components/other/expKernel.py` & `ngclearn-1.0b3/ngclearn/components/other/expKernel.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,20 +89,14 @@
         # cell compartments
         # self.comp["in"] = None
         # self.comp["epsp"] = None ## this emits a numeric "pulse" ()
         # self.comp["tf"] = [] # window of spike times
 
         ##Layer Size Setup
         self.n_units = n_units
-
-        if directory is None:
-            self.key, subkey = random.split(self.key)
-        else:
-            self.load(directory)
-
         self.reset()
 
     def verify_connections(self):
         self.metadata.check_incoming_connections(self.inputCompartmentName(),
                                                  min_connections=1)
 
     def advance_state(self, t, dt, **kwargs):
```

### Comparing `ngclearn-1.0b2/ngclearn/components/other/varTrace.py` & `ngclearn-1.0b3/ngclearn/components/other/varTrace.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,20 +110,14 @@
         self.tau_tr = tau_tr ## trace time constant
         self.a_delta = a_delta ## trace increment (if spike occurred)
         self.decay_type = decay_type ## lin --> linear decay; exp --> exponential decay
         self.decayFactor = None
 
         ##Layer Size Setup
         self.n_units = n_units
-
-        if directory is None:
-            self.key, subkey = random.split(self.key)
-        else:
-            self.load(directory)
-
         self.reset()
 
     def verify_connections(self):
         self.metadata.check_incoming_connections(self.inputCompartmentName(),
                                                  min_connections=1)
 
     def advance_state(self, t, dt, **kwargs):
```

### Comparing `ngclearn-1.0b2/ngclearn/components/synapses/hebbian/expSTDPSynapse.py` & `ngclearn-1.0b3/ngclearn/components/synapses/hebbian/expSTDPSynapse.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b2/ngclearn/components/synapses/hebbian/hebbianSynapse.py` & `ngclearn-1.0b3/ngclearn/components/synapses/hebbian/hebbianSynapse.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,17 @@
 from ngcsimlib.component import Component
 from jax import random, numpy as jnp, jit
 from functools import partial
 from ngclearn.utils.model_utils import initialize_params
+from ngclearn.utils.optim import SGD, Adam
 import time
 
-@partial(jit, static_argnums=[3])
-def update_eligibility(dt, Eg, dW, elg_tau):
-    """
-    Apply a signal modulator to j (typically of the form of a derivative/dampening function)
-
-    Args:
-        dt: integration time constant
-
-        Eg: current value of the eligibility trace
-
-        dW: synaptic update (at t) to update eligibility trace with
-
-        elg_tau: eligibility trace time constant
-
-    Returns:
-        updated eligibility trace tensor Eg
-    """
-    _Eg = Eg + (-Eg + dW) * (dt/elg_tau)
-    return _Eg
-
-@partial(jit, static_argnums=[3,4,5,6])
-def calc_update(pre, post, W, w_bound, is_nonnegative=True, signVal=1., w_decay=0.):
+@partial(jit, static_argnums=[3,4,5,6,7,8])
+def calc_update(pre, post, W, w_bound, is_nonnegative=True, signVal=1., w_decay=0.,
+                pre_wght=1., post_wght=1.):
     """
     Compute a tensor of adjustments to be applied to a synaptic value matrix.
 
     Args:
         pre: pre-synaptic statistic to drive Hebbian update
 
         post: post-synaptic statistic to drive Hebbian update
@@ -41,98 +23,72 @@
         is_nonnegative: (Unused)
 
         signVal: multiplicative factor to modulate final update by (good for
             flipping the signs of a computed synaptic change matrix)
 
         w_decay: synaptic decay factor to apply to this update
 
+        pre_wght: pre-synaptic weighting term (Default: 1.)
+
+        post_wght: post-synaptic weighting term (Default: 1.)
+
     Returns:
-        an update/adjustment matrix
+        an update/adjustment matrix, an update adjustment vector (for biases)
     """
-    dW = jnp.matmul(pre.T, post)
+    _pre = pre * pre_wght
+    _post = post * post_wght
+    dW = jnp.matmul(_pre.T, _post)
+    db = jnp.sum(_post, axis=0, keepdims=True)
     if w_bound > 0.:
         dW = dW * (w_bound - jnp.abs(W))
     if w_decay > 0.:
-        dW = dW - W * w_decay # jnp.matmul((1. - pre).T, (1. - post)) * w_decay
-    return dW * signVal
+        dW = dW - W * w_decay
+    return dW * signVal, db * signVal
 
-@partial(jit, static_argnums=[2,3,4])
-def adjust_synapses(dW, W, w_bound, eta, is_nonnegative=True):
+@partial(jit, static_argnums=[1,2])
+def enforce_constraints(W, w_bound, is_nonnegative=True):
     """
-    Evolves/changes the synpatic value matrix underlying this synaptic cable,
-    given a computed synaptic update.
+    Enforces constraints that the (synaptic) efficacies/values within matrix
+    `W` must adhere to.
 
     Args:
-        dW: synaptic adjustment matrix to be applied/used
-
         W: synaptic weight values (at time t)
 
         w_bound: maximum value to enforce over newly computed efficacies
 
-        eta: global learning rate to apply to the Hebbian update
-
         is_nonnegative: ensure updated value matrix is strictly non-negative
 
     Returns:
         the newly evolved synaptic weight value matrix
     """
-    _W = W + dW * eta
+    _W = W
     if w_bound > 0.:
         if is_nonnegative == True:
             _W = jnp.clip(_W, 0., w_bound)
         else:
             _W = jnp.clip(_W, -w_bound, w_bound)
     return _W
 
 @jit
-def apply_decay(dW, pre_s, post_s, w_decay):
-    _dW = dW - jnp.matmul((1. - pre_s).T, (1. - post_s)) * w_decay
-    return _dW
-
-@partial(jit, static_argnums=[4,5])
-def evolve(pre, post, W, w_bound, eta, is_nonnegative=True):
-    """
-    Evolves/changes the synpatic value matrix underlying this synaptic cable,
-    given relevant statistics.
-
-    Args:
-        pre: pre-synaptic statistic to drive Hebbian update
-
-        post: post-synaptic statistic to drive Hebbian update
-
-        W: synaptic weight values (at time t)
-
-        w_bound: maximum value to enforce over newly computed efficacies
-
-        eta: global learning rate to apply to the Hebbian update
-
-        is_nonnegative: ensure updated value matrix is strictly non-negative
-
-    Returns:
-        the newly evolved synaptic weight value matrix
-    """
-    dW = calc_update(pre, post, W, w_bound, is_nonnegative)
-    _W = adjust_synapses(dW, W, w_bound, eta, is_nonnegative)
-    return _W
-
-@jit
-def compute_layer(inp, weight):
+def compute_layer(inp, weight, biases):
     """
     Applies the transformation/projection induced by the synaptic efficacie
     associated with this synaptic cable
 
     Args:
         inp: signal input to run through this synaptic cable
 
         weight: this cable's synaptic value matrix
 
+        biases: this cable's bias value vector
+
     Returns:
         a projection/transformation of input "inp"
     """
-    return jnp.matmul(inp, weight)
+    return jnp.matmul(inp, weight) + biases
 
 class HebbianSynapse(Component):
     """
     A synaptic cable that adjusts its efficacies via a two-factor Hebbian
     adjustment rule.
 
     Args:
@@ -144,27 +100,44 @@
         eta: global learning rate
 
         wInit: a kernel to drive initialization of this synaptic cable's values;
             typically a tuple with 1st element as a string calling the name of
             initialization to use, e.g., ("uniform", -0.1, 0.1) samples U(-1,1)
             for each dimension/value of this cable's underlying value matrix
 
+        bInit: a kernel to drive initialization of biases for this synaptic cable
+            (Default: None, which turns off/disables biases)
+
         w_bound: maximum weight to softly bound this cable's value matrix to; if
             set to 0, then no synaptic value bounding will be applied
 
-        elg_tau: if > 0., triggers the use of an eligibility trace where this value
-            serves as its time constant
-
         is_nonnegative: enforce that synaptic efficacies are always non-negative
             after each synaptic update (if False, no constraint will be applied)
 
+        w_decay: degree to which (L2) synaptic weight decay is applied to the
+            computed Hebbian adjustment (Default: 0); note that decay is not
+            applied to any configured biases
+
         signVal: multiplicative factor to apply to final synaptic update before
-            it is applied to synapses; this is useful if gradient descent schemes
-            are to be applied (as Hebbian rules typically yield adjustments for
-            ascent)
+            it is applied to synapses; this is useful if gradient descent style
+            optimization is required (as Hebbian rules typically yield
+            adjustments for ascent)
+
+        optim_type: optimization scheme to physically alter synaptic values
+            once an update is computed (Default: "sgd"); supported schemes
+            include "sgd" and "adam"
+
+            :Note: technically, if "sgd" or "adam" is used but `signVal = 1`,
+                then the ascent form of each rule is employed (signVal = -1) or
+                a negative learning rate will mean a descent form of the
+                `optim_scheme` is being employed
+
+        pre_wght: pre-synaptic weighting factor (Default: 1.)
+
+        post_wght: post-synaptic weighting factor (Default: 1.)
 
         key: PRNG key to control determinism of any underlying random values
             associated with this synaptic cable
 
         useVerboseDict: triggers slower, verbose dictionary mode (Default: False)
 
         directory: string indicating directory on disk to save synaptic parameter
@@ -186,22 +159,14 @@
         return 'trigger'
 
     @classmethod
     def presynapticCompartmentName(cls):
         return 'pre'
 
     @classmethod
-    def postsynSpikeName(cls):
-        return 's_post'
-
-    @classmethod
-    def presynSpikeName(cls):
-        return 's_pre'
-
-    @classmethod
     def postsynapticCompartmentName(cls):
         return 'post'
 
     ## Bind Properties to Compartments for ease of use
     @property
     def trigger(self):
         return self.compartments.get(self.triggerName(), None)
@@ -238,97 +203,106 @@
     def postsynapticCompartment(self):
         return self.compartments.get(self.postsynapticCompartmentName(), None)
 
     @postsynapticCompartment.setter
     def postsynapticCompartment(self, x):
         self.compartments[self.postsynapticCompartmentName()] = x
 
-    @property
-    def presynSpike(self):
-        return self.compartments.get(self.presynSpikeName(), None)
-
-    @presynSpike.setter
-    def presynSpike(self, x):
-        self.compartments[self.presynSpikeName()] = x
-
-    @property
-    def postsynSpike(self):
-        return self.compartments.get(self.postsynSpikeName(), None)
-
-    @postsynSpike.setter
-    def postsynSpike(self, x):
-        self.compartments[self.postsynSpikeName()] = x
-
     # Define Functions
-    def __init__(self, name, shape, eta=0., wInit=("uniform", 0., 0.3), w_bound=1.,
-                 elg_tau=0., is_nonnegative=False, w_decay=0., signVal=1., key=None,
-                 useVerboseDict=False, directory=None, **kwargs):
+    def __init__(self, name, shape, eta=0., wInit=("uniform", 0., 0.3),
+                 bInit=None, w_bound=1., is_nonnegative=False, w_decay=0.,
+                 signVal=1., optim_type="sgd", pre_wght=1., post_wght=1., 
+                 key=None, useVerboseDict=False, directory=None, **kwargs):
         super().__init__(name, useVerboseDict, **kwargs)
 
-        ##Random Number Set up
+        ## random Number Set up
         self.key = key
         if self.key is None:
             self.key = random.PRNGKey(time.time_ns())
 
-        ##params
+        ## synaptic plasticity properties and characteristics
         self.shape = shape
         self.w_bounds = w_bound
         self.w_decay = w_decay ## synaptic decay
+        self.pre_wght = pre_wght
+        self.post_wght = post_wght
         self.eta = eta
         self.wInit = wInit
+        self.bInit = bInit
         self.is_nonnegative = is_nonnegative
         self.signVal = signVal
-        self.elg_tau = elg_tau
-        self.Eg = None
+
+        ## optimization / adjustment properties (given learning dynamics above)
+        self.opt = None
+        if optim_type == "adam":
+            self.opt = Adam(learning_rate=self.eta)
+        else: ## default is SGD
+            self.opt = SGD(learning_rate=self.eta)
 
         if directory is None:
             self.key, subkey = random.split(self.key)
             self.weights = initialize_params(subkey, wInit, shape)
+            if self.bInit is not None:
+                self.key, subkey = random.split(self.key)
+                self.biases = initialize_params(subkey, bInit, (1, shape[1]))
         else:
             self.load(directory)
 
         ##Reset to initialize stuff
         self.reset()
 
+        self.dW = None
+        self.db = None
+
     def verify_connections(self):
         self.metadata.check_incoming_connections(self.inputCompartmentName(), min_connections=1)
 
     def advance_state(self, **kwargs):
-        self.outputCompartment = compute_layer(self.inputCompartment, self.weights)
+        biases = 0.
+        if self.bInit != None:
+            biases = self.biases
+        self.outputCompartment = compute_layer(self.inputCompartment,
+                                               self.weights, biases)
 
     def evolve(self, t, dt, **kwargs):
-        if self.elg_tau > 0.:
-            trigger = self.trigger
-            dW = calc_update(self.presynapticCompartment, self.postsynapticCompartment,
+        dW, db = calc_update(self.presynapticCompartment, self.postsynapticCompartment,
                              self.weights, self.w_bounds, is_nonnegative=self.is_nonnegative,
-                             signVal=self.signVal)
-            self.Eg = update_eligibility(dt, self.Eg, dW, self.elg_tau)
-            if trigger > 0.:
-                self.weights = adjust_synapses(self.Eg, self.weights, self.w_bounds, self.eta,
-                                               is_nonnegative=self.is_nonnegative)
+                             signVal=self.signVal, w_decay=self.w_decay,
+                             pre_wght=self.pre_wght, post_wght=self.post_wght)
+        self.dW = dW
+        self.db = db
+        ## conduct a step of optimization - get newly evolved synaptic weight value matrix
+        if self.bInit != None:
+            theta = [self.weights, self.biases]
+            self.opt.update(theta, [dW, db])
+            self.weights = theta[0]
+            self.biases = theta[1]
         else:
-            dW = calc_update(self.presynapticCompartment, self.postsynapticCompartment,
-                             self.weights, self.w_bounds, is_nonnegative=self.is_nonnegative,
-                             signVal=self.signVal, w_decay=0.)
-            if self.w_decay > 0.:
-                dW = apply_decay(dW, self.presynSpike, self.postsynSpike, self.w_decay)
-            self.Eg = dW
-            self.weights = adjust_synapses(dW, self.weights, self.w_bounds, self.eta,
+            # ignore db since no biases configured
+            theta = [self.weights]
+            self.opt.update(theta, [dW])
+            self.weights = theta[0]
+        ## ensure synaptic efficacies adhere to constraints
+        self.weights = enforce_constraints(self.weights, self.w_bounds,
                                            is_nonnegative=self.is_nonnegative)
 
     def reset(self, **kwargs):
         self.inputCompartment = None
         self.outputCompartment = None
         self.presynapticCompartment = None
         self.postsynapticCompartment = None
-        self.presynSpike = None
-        self.postsynSpike = None
-        self.Eg = self.weights * 0
+        self.dW = None
+        self.db = None
 
     def save(self, directory, **kwargs):
         file_name = directory + "/" + self.name + ".npz"
-        jnp.savez(file_name, weights=self.weights)
+        if self.bInit != None:
+            jnp.savez(file_name, weights=self.weights, biases=self.biases)
+        else:
+            jnp.savez(file_name, weights=self.weights)
 
     def load(self, directory, **kwargs):
         file_name = directory + "/" + self.name + ".npz"
         data = jnp.load(file_name)
         self.weights = data['weights']
+        if self.bInit != None:
+            self.biases = data['biases']
```

### Comparing `ngclearn-1.0b2/ngclearn/components/synapses/hebbian/traceSTDPSynapse.py` & `ngclearn-1.0b3/ngclearn/components/synapses/hebbian/traceSTDPSynapse.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         if Aminus > 0.:
             ## calculate pre-synaptic term
             dWpre = -jnp.matmul(pre.T, x_post * Aminus)
     ## calc final weighted adjustment
     dW = (dWpost + dWpre) * eta
     _W = W + dW
     # if w_norm is not None:
-    #     _W = normalize_matrix(_W, w_norm, ord=1, axis=1) ## L1 norm constraint
+    #     _W = normalize_matrix(_W, w_norm, order=1, axis=1) ## L1 norm constraint
     #    #_W = _W * (w_norm/(jnp.linalg.norm(_W, axis=1, keepdims=True) + 1e-5))
     _W = jnp.clip(_W, 0.001, w_bound) # 0.01, w_bound)
     return _W
 
 @jit
 def compute_layer(inp, weight):
     """
@@ -241,15 +241,15 @@
         self.weights = evolve(dt, pre, x_pre, post, x_post, self.weights,
                               w_bound=self.w_bound, eta=self.eta,
                               x_tar=self.preTrace_target, mu=self.mu,
                               Aplus=self.Aplus, Aminus=self.Aminus,
                               w_norm=self.w_norm)
         if self.norm_T > 0:
             if t % (self.norm_T-1) == 0: #t % self.norm_t == 0:
-                self.weights = normalize_matrix(self.weights, self.w_norm, ord=1, axis=0)
+                self.weights = normalize_matrix(self.weights, self.w_norm, order=1, axis=0)
 
     def reset(self, **kwargs):
         self.inputCompartment = None
         self.outputCompartment = None
         self.presynapticTrace = None
         self.postsynapticTrace = None
         self.trigger = 1. ## default: assume synaptic change will occur
```

### Comparing `ngclearn-1.0b2/ngclearn/utils/density/gmm.py` & `ngclearn-1.0b3/ngclearn/utils/density/gmm.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b2/ngclearn/utils/io_utils.py` & `ngclearn-1.0b3/ngclearn/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b2/ngclearn/utils/optim/adam.py` & `ngclearn-1.0b3/ngclearn/utils/optim/adam.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b2/ngclearn/utils/optim/opt.py` & `ngclearn-1.0b3/ngclearn/utils/optim/opt.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b2/ngclearn/utils/optim/sgd.py` & `ngclearn-1.0b3/ngclearn/utils/optim/sgd.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b2/ngclearn/utils/patch_utils.py` & `ngclearn-1.0b3/ngclearn/utils/patch_utils.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b2/ngclearn/utils/viz/dim_reduce.py` & `ngclearn-1.0b3/ngclearn/utils/viz/dim_reduce.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         a matrix (K x 2) of projected vectors (to 2D space)
     """
     batch_size = 50
     z_dim = vectors.shape[1]
     z_2D = None
     if z_dim != 2:
         ipca = IncrementalPCA(n_components=2, batch_size=batch_size)
-        ipca.fit(vectors.numpy())
-        z_2D = ipca.transform(vectors.numpy())
+        ipca.fit(vectors)
+        z_2D = ipca.transform(vectors)
     else:
         z_2D = vectors
     return z_2D
 
 def extract_tsne_latents(vectors, perplexity=30): ## tSNE mapping routine
     """
     Projects collection of K vectors (stored in a matrix) to a two-dimensional (2D)
@@ -52,16 +52,16 @@
     if z_dim != 2:
         print(" > Projecting latents via iPCA...")
         n_comp = 32 #10 #16 #50
         if vectors.shape[1] < n_comp:
             n_comp = vectors.shape[1] - 2 #z_top.shape[1]-2
             n_comp = max(2, n_comp)
         ipca = IncrementalPCA(n_components=n_comp, batch_size=batch_size)
-        ipca.fit(vectors.numpy())
-        z_2D = ipca.transform(vectors.numpy())
+        ipca.fit(vectors)
+        z_2D = ipca.transform(vectors)
         print(" PCA.lat.shape = ",z_2D.shape)
         print(" > Finishing projection via t-SNE...")
         z_2D = TSNE(n_components=2,perplexity=perplexity, verbose=1).fit_transform(z_2D)
     else:
         z_2D = vectors
     return z_2D
```

### Comparing `ngclearn-1.0b2/ngclearn/utils/viz/raster.py` & `ngclearn-1.0b3/ngclearn/utils/viz/raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 import imageio.v3 as iio
 import jax.numpy as jnp
 
 #suffix = '.jpg' #.png
 
 def _create_raster_plot(spike_train, ax=None, s=1.5, c="black", marker="|",
-                       plot_fname=None, indices=None, tag="", suffix='.jpg'):
+                       plot_fname=None, indices=None, suffix='.jpg'):
     spk_ = spike_train
     # Process spikes and create the binary coordinate grid
     if len(spk_.shape) == 1:
         spk_ = jnp.expand_dims(spk_,axis=1)
     n_units = spk_.shape[1]
     if indices is not None and indices.shape[0] < spk_.shape[1]:
         spk_ = spk_[:,indices] # access specific neurons if requested
@@ -39,15 +39,15 @@
             plot_fname = "raster_plot" + suffix
         fig = plt.figure(facecolor="w", figsize=(10, 5))
         ax = fig.add_subplot(111)
         ax.scatter(spk_x, spk_y, s=s, c=c, marker=marker)
         yint = range(0, n_units)
         ax.set_yticks(yint)
         ax.set_yticklabels(yint, fontsize=12)
-        plt.title("Spike Train Raster Plot, {}".format(tag))
+        plt.title("Spike Train Raster Plot")
         plt.xlabel("Time Step")
         plt.ylabel("Neuron Index")
         plt.savefig(plot_fname)
         plt.clf()
         plt.close()
 
 def create_raster_plot(spike_train, ax=None, s=0.5, c="black",
```

### Comparing `ngclearn-1.0b2/ngclearn/utils/viz/synapse_plot.py` & `ngclearn-1.0b3/ngclearn/utils/viz/synapse_plot.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b2/ngclearn.egg-info/PKG-INFO` & `ngclearn-1.0b3/ngclearn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngclearn
-Version: 1.0b2
+Version: 1.0b3
 Summary: Simulation software for building and analyzing arbitrary predictive coding, spiking network, and biomimetic neural systems.
 Author-email: Alexander Ororbia <ago@cs.rit.edu>, William Gebhardt <wdg1351@rit.edu>
 License: BSD-3-Clause License
 Project-URL: Homepage, https://github.com/NACLab/ngc-learn
 Project-URL: Documentation, https://ngc-learn.readthedocs.io/
 Project-URL: Lab Page, https://www.cs.rit.edu/~ago/nac_lab.html
 Project-URL: Changelog, https://github.com/NACLab/ngc-learn/blob/main/history.txt
@@ -48,15 +48,17 @@
 
 It is currently maintained by the
 <a href="https://www.cs.rit.edu/~ago/nac_lab.html">Neural Adaptive Computing (NAC) laboratory</a>.
 
 ## <b>Documentation</b>
 
 Official documentation, including tutorials, can be found
-<a href="https://ngc-learn.readthedocs.io/en/latest/#">here</a>.
+<a href="https://ngc-learn.readthedocs.io/en/latest/#">here</a>. The model museum repo, 
+which implements several historical models, can be found 
+<a href="https://github.com/NACLab/ngc-museum">here</a>.
 
 The official blog-post related to the source paper behind this software library
 can be found
 <a href="https://go.nature.com/3rgl1K8">here</a>.<br>
 You can find the related paper <a href="https://www.nature.com/articles/s41467-022-29632-7">right here</a>, which
 was selected to appear in the Nature <i>Neuromorphic Hardware and Computing Collection</i> in 2023 and was
 chosen as one of the <i>Editors' Highlights for Applied Physics and Mathematics</i> in 2022.
@@ -90,15 +92,15 @@
 <!-- (Note: if using the `_generate_patch_set()` within the
 image patching utilities, then Patchify will be needed).-->
 
 ### User Installation
 
 <i>Setup</i>: The easiest way to install ngc-learn (CPU version) is through <code>pip</code>:
 <pre>
-$ python install ngclearn
+$ pip install ngclearn
 </pre>
 
 The documentation includes more detailed
 <a href="https://ngc-learn.readthedocs.io/en/latest/installation.html">installation instructions</a>.
 Note that this library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and 20.04.
 
 <!--
@@ -166,15 +168,15 @@
 If you are working on and developing with ngc-learn pulled from the github
 repo, then run the following command to set up an editable install:
 <pre>
 $ python install -e .
 </pre>
 
 **Version:**<br>
-1.0.2-Beta <!-- -Alpha -->
+1.0.3-Beta <!-- -Alpha -->
 
 Author:
 Alexander G. Ororbia II<br>
 Director, Neural Adaptive Computing (NAC) Laboratory<br>
 Rochester Institute of Technology, Department of Computer Science
 
 ## <b>Copyright:</b>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ngclearn Version: 1.0b2 Summary: Simulation
+Metadata-Version: 2.1 Name: ngclearn Version: 1.0b3 Summary: Simulation
 software for building and analyzing arbitrary predictive coding, spiking
 network, and biomimetic neural systems. Author-email: Alexander Ororbia
 cs.rit.edu>, William Gebhardt
 rit.edu> License: BSD-3-Clause License Project-URL: Homepage, https://
 github.com/NACLab/ngc-learn Project-URL: Documentation, https://ngc-
 learn.readthedocs.io/ Project-URL: Lab Page, https://www.cs.rit.edu/~ago/
 nac_lab.html Project-URL: Changelog, https://github.com/NACLab/ngc-learn/blob/
@@ -33,31 +33,32 @@
 [docs/images/ngc-learn-logo.png]nnggcc--lleeaarrnn is a Python library for building,
 simulating, and analyzing biomimetic systems, neurobiological agents, spiking
 neuronal networks, predictive coding circuitry, and models that learn via
 biologically-plausible forms of credit assignment. This simulation toolkit is
 built on top of JAX and is distributed under the 3-Clause BSD license. It is
 currently maintained by the _N_e_u_r_a_l_ _A_d_a_p_t_i_v_e_ _C_o_m_p_u_t_i_n_g_ _(_N_A_C_)_ _l_a_b_o_r_a_t_o_r_y. ##
 DDooccuummeennttaattiioonn Official documentation, including tutorials, can be found _h_e_r_e.
-The official blog-post related to the source paper behind this software library
-can be found _h_e_r_e.
+The model museum repo, which implements several historical models, can be found
+_h_e_r_e. The official blog-post related to the source paper behind this software
+library can be found _h_e_r_e.
 You can find the related paper _r_i_g_h_t_ _h_e_r_e, which was selected to appear in the
 Nature Neuromorphic Hardware and Computing Collection in 2023 and was chosen as
 one of the Editors' Highlights for Applied Physics and Mathematics in 2022. ##
 Installation ### Dependencies ngc-learn requires: 1) Python (>=3.10) 2) NumPy
 (>=1.26.0) 3) SciPy (>=1.7.0) 4) ngcsimlib (>=0.2.b1), (visit official page
 _h_e_r_e) 5) JAX (>= 0.4.18) (to enable GPU use, make sure to install one of the
 CUDA variants) --- ngc-learn 1.0.beta0 and later require Python 3.10 or newer
 as well as ngcsimlib >=0.2.b2. ngc-learn's plotting capabilities (routines
 within `ngclearn.utils.viz`) require Matplotlib (>=3.8.0) and imageio
 (>=2.31.5) and both plotting and density estimation tools (routines within
 ``ngclearn.utils.density``) will require Scikit-learn (>=0.24.2). Many of the
 tutorials will require Matplotlib (>=3.8.0), imageio (>=2.31.5), and Scikit-
 learn (>=0.24.2). ### User Installation Setup: The easiest way to install ngc-
 learn (CPU version) is through pip:
-$ python install ngclearn
+$ pip install ngclearn
 The documentation includes more detailed _i_n_s_t_a_l_l_a_t_i_o_n_ _i_n_s_t_r_u_c_t_i_o_n_s. Note that
 this library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and
 20.04. If the installation was successful, you should see the following if you
 test it against your Python interpreter, i.e., run the $ python command and
 complete the following sequence of steps as depicted in the screenshot below:
 [docs/images/test_ngclearn_install.png]Note: For access to the previous
 Tensorflow-2 version of ngc-learn (of which we no longer support), please visit
@@ -83,15 +84,15 @@
 [contributing guidelines](CONTRIBUTING.md). SSoouurrccee CCooddee You can check/pull the
 latest source code for this library via:
 $ git clone https://github.com/NACLab/ngc-learn.git
 If you are working on and developing with ngc-learn pulled from the github
 repo, then run the following command to set up an editable install:
 $ python install -e .
 **Version:**
-1.0.2-Beta Author: Alexander G. Ororbia II
+1.0.3-Beta Author: Alexander G. Ororbia II
 Director, Neural Adaptive Computing (NAC) Laboratory
 Rochester Institute of Technology, Department of Computer Science ## CCooppyyrriigghhtt::
 Copyright (C) 2021 The Neural Adaptive Computing Laboratory - All Rights
 Reserved
 You may use, distribute and modify this code under the terms of the BSD 3-
 clause license. You should have received a copy of the BSD 3-clause license
 with this software.
```

### Comparing `ngclearn-1.0b2/ngclearn.egg-info/SOURCES.txt` & `ngclearn-1.0b3/ngclearn.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -20,32 +20,39 @@
 ngclearn/components/neurons/__init__.py
 ngclearn/components/neurons/graded/__init__.py
 ngclearn/components/neurons/graded/gaussianErrorCell.py
 ngclearn/components/neurons/graded/laplacianErrorCell.py
 ngclearn/components/neurons/graded/rateCell.py
 ngclearn/components/neurons/spiking/LIFCell.py
 ngclearn/components/neurons/spiking/__init__.py
+ngclearn/components/neurons/spiking/fitzhughNagumoCell.py
 ngclearn/components/neurons/spiking/izhikevichCell.py
 ngclearn/components/neurons/spiking/quadLIFCell.py
 ngclearn/components/neurons/spiking/sLIFCell.py
 ngclearn/components/other/__init__.py
 ngclearn/components/other/expKernel.py
 ngclearn/components/other/varTrace.py
 ngclearn/components/synapses/__init__.py
 ngclearn/components/synapses/hebbian/__init__.py
 ngclearn/components/synapses/hebbian/expSTDPSynapse.py
 ngclearn/components/synapses/hebbian/hebbianSynapse.py
 ngclearn/components/synapses/hebbian/traceSTDPSynapse.py
 ngclearn/utils/__init__.py
+ngclearn/utils/data_loader.py
 ngclearn/utils/io_utils.py
+ngclearn/utils/metric_utils.py
 ngclearn/utils/model_utils.py
 ngclearn/utils/patch_utils.py
+ngclearn/utils/surrogate_fx.py
 ngclearn/utils/density/__init__.py
 ngclearn/utils/density/gmm.py
+ngclearn/utils/diffeq/__init__.py
+ngclearn/utils/diffeq/ode_utils.py
 ngclearn/utils/optim/__init__.py
 ngclearn/utils/optim/adam.py
 ngclearn/utils/optim/opt.py
 ngclearn/utils/optim/sgd.py
 ngclearn/utils/viz/__init__.py
 ngclearn/utils/viz/dim_reduce.py
 ngclearn/utils/viz/raster.py
+ngclearn/utils/viz/spike_plot.py
 ngclearn/utils/viz/synapse_plot.py
```

### Comparing `ngclearn-1.0b2/pyproject.toml` & `ngclearn-1.0b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ngclearn"
-version = "1.0.beta2"
+version = "1.0.beta3"
 description = "Simulation software for building and analyzing arbitrary predictive coding, spiking network, and biomimetic neural systems."
 authors = [
   {name = "Alexander Ororbia", email = "ago@cs.rit.edu"},
   {name = "William Gebhardt", email = "wdg1351@rit.edu"},
 ]
 readme = "README.md"
 keywords = ['python', 'ngc-learn', 'predictive-processing', 'predictive-coding',
```

