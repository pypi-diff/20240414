# Comparing `tmp/spit-0.1.8.tar.gz` & `tmp/spit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/berilerdogdu/Desktop/SPIT/dist/.tmp-h2dat82d/spit-0.1.8.tar", last modified: Sat Dec 16 06:29:55 2023, max compression
+gzip compressed data, was "/Users/berilerdogdu/Desktop/SPIT/dist/.tmp-es5ve703/spit-0.1.9.tar", last modified: Sun Dec 17 20:10:03 2023, max compression
```

## Comparing `spit-0.1.8.tar` & `spit-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2023-12-16 06:29:55.000000 spit-0.1.8/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)    35149 2023-11-08 19:32:56.000000 spit-0.1.8/LICENSE
--rw-r--r--   0 berilerdogdu   (501) staff       (20)       78 2023-12-06 19:33:46.000000 spit-0.1.8/MANIFEST.in
--rw-r--r--   0 berilerdogdu   (501) staff       (20)       93 2023-12-16 06:29:55.000000 spit-0.1.8/PKG-INFO
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     3543 2023-11-08 19:32:56.000000 spit-0.1.8/README.md
--rw-r--r--   0 berilerdogdu   (501) staff       (20)       38 2023-12-16 06:29:55.000000 spit-0.1.8/setup.cfg
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      642 2023-12-16 06:29:35.000000 spit-0.1.8/setup.py
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2023-12-16 06:29:55.000000 spit-0.1.8/spit/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)        0 2023-11-08 19:32:56.000000 spit-0.1.8/spit/__init__.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     1173 2023-11-08 19:32:56.000000 spit-0.1.8/spit/cluster_samples.py
--rwxr-xr-x   0 berilerdogdu   (501) staff       (20)     6999 2023-11-16 08:13:50.000000 spit-0.1.8/spit/confounding_analysis.py
--rwxr-xr-x   0 berilerdogdu   (501) staff       (20)    12799 2023-12-16 06:29:24.000000 spit-0.1.8/spit/dtu_detection.py
--rwxr-xr-x   0 berilerdogdu   (501) staff       (20)     9555 2023-11-09 08:10:49.000000 spit-0.1.8/spit/filter_and_transform_tx_counts.py
--rwxr-xr-x   0 berilerdogdu   (501) staff       (20)      773 2023-11-08 19:32:56.000000 spit-0.1.8/spit/get_p_cutoff.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     1545 2023-11-08 23:24:22.000000 spit-0.1.8/spit/import_infreps.py
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2023-12-16 06:29:55.000000 spit-0.1.8/spit/parameter_fitting/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     4482 2023-12-08 22:31:19.000000 spit-0.1.8/spit/parameter_fitting/LOOCV.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)        0 2023-11-08 19:32:56.000000 spit-0.1.8/spit/parameter_fitting/__init__.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     6735 2023-12-06 03:08:31.000000 spit-0.1.8/spit/parameter_fitting/filter_and_simulate_tx_counts.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     6779 2023-12-06 04:21:53.000000 spit-0.1.8/spit/parameter_fitting/simulate_dtu_exp.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     4786 2023-11-08 19:32:56.000000 spit-0.1.8/spit/plot_spit_charts.py
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2023-12-16 06:29:55.000000 spit-0.1.8/spit/r_scripts/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     3251 2023-11-08 19:32:56.000000 spit-0.1.8/spit/r_scripts/hclust.R
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     1326 2023-11-08 23:21:57.000000 spit-0.1.8/spit/r_scripts/tximport_quant_files.R
--rw-r--r--   0 berilerdogdu   (501) staff       (20)    11991 2023-12-14 02:49:26.000000 spit-0.1.8/spit/run_spit.py
--rwxr-xr-x   0 berilerdogdu   (501) staff       (20)     6217 2023-12-16 06:29:19.000000 spit-0.1.8/spit/spit_test.py
--rwxr-xr-x   0 berilerdogdu   (501) staff       (20)     2824 2023-12-06 03:01:39.000000 spit-0.1.8/spit/transform_tx_counts_to_ifs.py
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2023-12-16 06:29:55.000000 spit-0.1.8/spit.egg-info/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)       93 2023-12-16 06:29:55.000000 spit-0.1.8/spit.egg-info/PKG-INFO
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      706 2023-12-16 06:29:55.000000 spit-0.1.8/spit.egg-info/SOURCES.txt
--rw-r--r--   0 berilerdogdu   (501) staff       (20)        1 2023-12-16 06:29:55.000000 spit-0.1.8/spit.egg-info/dependency_links.txt
--rw-r--r--   0 berilerdogdu   (501) staff       (20)       44 2023-12-16 06:29:55.000000 spit-0.1.8/spit.egg-info/entry_points.txt
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      146 2023-12-16 06:29:55.000000 spit-0.1.8/spit.egg-info/requires.txt
--rw-r--r--   0 berilerdogdu   (501) staff       (20)        5 2023-12-16 06:29:55.000000 spit-0.1.8/spit.egg-info/top_level.txt
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2023-12-17 20:10:03.000000 spit-0.1.9/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)    35149 2023-12-17 20:03:44.000000 spit-0.1.9/LICENSE
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)       78 2023-12-17 20:03:44.000000 spit-0.1.9/MANIFEST.in
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)       93 2023-12-17 20:10:03.000000 spit-0.1.9/PKG-INFO
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     3788 2023-12-17 20:03:44.000000 spit-0.1.9/README.md
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)       38 2023-12-17 20:10:03.000000 spit-0.1.9/setup.cfg
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      642 2023-12-17 20:09:12.000000 spit-0.1.9/setup.py
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2023-12-17 20:10:03.000000 spit-0.1.9/spit/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)        0 2023-12-17 20:03:44.000000 spit-0.1.9/spit/__init__.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     1173 2023-12-17 20:03:44.000000 spit-0.1.9/spit/cluster_samples.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     6999 2023-12-17 20:03:44.000000 spit-0.1.9/spit/confounding_analysis.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)    12799 2023-12-17 20:03:44.000000 spit-0.1.9/spit/dtu_detection.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     9555 2023-12-17 20:03:44.000000 spit-0.1.9/spit/filter_and_transform_tx_counts.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      773 2023-12-17 20:03:44.000000 spit-0.1.9/spit/get_p_cutoff.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     1545 2023-12-17 20:03:44.000000 spit-0.1.9/spit/import_infreps.py
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2023-12-17 20:10:03.000000 spit-0.1.9/spit/parameter_fitting/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     4482 2023-12-17 20:03:44.000000 spit-0.1.9/spit/parameter_fitting/LOOCV.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)        0 2023-12-17 20:03:44.000000 spit-0.1.9/spit/parameter_fitting/__init__.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     6735 2023-12-17 20:03:44.000000 spit-0.1.9/spit/parameter_fitting/filter_and_simulate_tx_counts.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     6779 2023-12-17 20:03:44.000000 spit-0.1.9/spit/parameter_fitting/simulate_dtu_exp.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     4786 2023-12-17 20:03:44.000000 spit-0.1.9/spit/plot_spit_charts.py
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2023-12-17 20:10:03.000000 spit-0.1.9/spit/r_scripts/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     3251 2023-12-17 20:03:44.000000 spit-0.1.9/spit/r_scripts/hclust.R
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     1326 2023-12-17 20:03:44.000000 spit-0.1.9/spit/r_scripts/tximport_quant_files.R
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)    11991 2023-12-17 20:03:44.000000 spit-0.1.9/spit/run_spit.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     6172 2023-12-17 20:03:44.000000 spit-0.1.9/spit/spit_test.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     2824 2023-12-17 20:03:44.000000 spit-0.1.9/spit/transform_tx_counts_to_ifs.py
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2023-12-17 20:10:03.000000 spit-0.1.9/spit.egg-info/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)       93 2023-12-17 20:10:03.000000 spit-0.1.9/spit.egg-info/PKG-INFO
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      706 2023-12-17 20:10:03.000000 spit-0.1.9/spit.egg-info/SOURCES.txt
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)        1 2023-12-17 20:10:03.000000 spit-0.1.9/spit.egg-info/dependency_links.txt
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)       44 2023-12-17 20:10:03.000000 spit-0.1.9/spit.egg-info/entry_points.txt
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      146 2023-12-17 20:10:03.000000 spit-0.1.9/spit.egg-info/requires.txt
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)        5 2023-12-17 20:10:03.000000 spit-0.1.9/spit.egg-info/top_level.txt
```

### Comparing `spit-0.1.8/LICENSE` & `spit-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spit-0.1.8/README.md` & `spit-0.1.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -11,43 +11,44 @@
 Detecting DTU events for single-gene genetic traits is relatively uncomplicated; however, the heterogeneity of populations with complex diseases presents an intricate challenge due to the presence of diverse causal events and undetermined subtypes.
 SPIT can detect DTU events exclusive to subgroups as well as DTU events shared amongst all case samples. Downstream of DTU analysis, SPIT uses detected DTU events to provide insight into potentially hierarchical subgrouping patterns present in complex disease populations using hierarchical clustering.
 
 SPIT is equally effective on relatively homogeneous populations, and proves to be applicable for diverse scenarios, including simple genetic disorders, tissue-to-tissue comparisons and other types of DTU studies. SPIT consistently maintains notably low false discovery rates regardless of the level of dispersion in the datasets.
 
 ### How to use SPIT?
 
+SPIT is available as a PyPI package and can be installed by calling:
+```
+pip install spit
+```
+
 An extensive step-by-step guide that demonstrates the application of SPIT using a mock dataset is provided [here](https://colab.research.google.com/drive/1u3NpleqcAfNz_0EAgO2UHItozd9PsF1w?usp=sharing).
 
 Users can also directly upload their datasets into this Colab environment and easily run SPIT [online](https://colab.research.google.com/drive/1u3NpleqcAfNz_0EAgO2UHItozd9PsF1w?usp=sharing).
 
-### Parameter-fitting
+### Parameter-fitting with GNU Parallel
 
-If you wish to run the parameter-fitting module, please clone this project and follow these steps:
+If you would like to optimize hyper-parameters based on the dispersion levels on your own data  set, you can easily do so using the package module "fit_parameters". However, this is a computationally expensive process and might take some time. Multi-threading via GNU Parallel is an option. If you wish to run the parameter-fitting module with GNU Parallel, please clone this project and follow these steps:
 - Navigate into the "parameter_fitting" directory, and generate your 10 DTU simulations by running:
 ```
 sh simulate_exps.sh -i [tx_counts_file] -m [tx2gene_file] -l [pheno_file]
 ```
 Please note that your input files should follow the formatting requirements described in the Colab notebook. For detailed explanations of what these files should contain, please refer to the [tutorial](https://colab.research.google.com/drive/1u3NpleqcAfNz_0EAgO2UHItozd9PsF1w?usp=sharing).
 
 - Run SPIT with combinations of **b** and **k** parameters to search for the optimal choice for your dataset:
 ```
 sh run_SPIT_search_params.sh [#number of threads] -m [tx2gene_file]
 ```
-If you have multiple threads available, the run is distributed accordingly via GNU Parallel. The maximum number of threads that can be used is equal to the number of simulated experiments (10). For example, if you would like to run with 10 threads, run:
+The maximum number of threads that can be used is equal to the number of simulated experiments (10). For example, if you would like to run with 10 threads, run:
 
 ```
 sh run_SPIT_search_params.sh 10 -m [tx2gene_file]
 ```
-Otherwise, please run as:
-```
-sh run_SPIT_search_params.sh 1 -m [tx2gene_file]
-```
 - Run the leave-one-out cross-validation (LOOCV) step to see the optimal parameters in all 10 experiments as:
 ```
 python LOOCV.py -m tx2gene_file.txt -P venns.pdf
 ```
-The output PDF file (venns.pdf) will include the optimal parameters at each iteratioin of the LOOCV process along with corresponding true positive and false positive rates and *F*-scores. 
+The output PDF file (venns.pdf) will include the optimal parameters at each iteration of the LOOCV process along with corresponding true positive and false positive rates and *F*-scores. 
 
 ##### If you use SPIT, please cite:
 Erdogdu, B., Varabyou, A., Hicks, S.C., Salzberg, S.L. & Pertea, M. Detecting differential transcript usage in complex diseases with SPIT. bioRxiv, 2023.2007.2010.548289 (2023)
 
 ##### Please use [this Google group](https://groups.google.com/g/spit_dtu) to post your questions, comments, or bug reports.
```

### Comparing `spit-0.1.8/setup.py` & `spit-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='spit',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'matplotlib>=3.4.3',
         'matplotlib_venn>=0.11.6',
         'numpy>=1.20.3',
         'pandas>=1.3.4',
```

### Comparing `spit-0.1.8/spit/cluster_samples.py` & `spit-0.1.9/spit/cluster_samples.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.8/spit/confounding_analysis.py` & `spit-0.1.9/spit/confounding_analysis.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.8/spit/dtu_detection.py` & `spit-0.1.9/spit/dtu_detection.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.8/spit/filter_and_transform_tx_counts.py` & `spit-0.1.9/spit/filter_and_transform_tx_counts.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.8/spit/get_p_cutoff.py` & `spit-0.1.9/spit/get_p_cutoff.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.8/spit/import_infreps.py` & `spit-0.1.9/spit/import_infreps.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.8/spit/parameter_fitting/LOOCV.py` & `spit-0.1.9/spit/parameter_fitting/LOOCV.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.8/spit/parameter_fitting/filter_and_simulate_tx_counts.py` & `spit-0.1.9/spit/parameter_fitting/filter_and_simulate_tx_counts.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.8/spit/parameter_fitting/simulate_dtu_exp.py` & `spit-0.1.9/spit/parameter_fitting/simulate_dtu_exp.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.8/spit/plot_spit_charts.py` & `spit-0.1.9/spit/plot_spit_charts.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.8/spit/r_scripts/hclust.R` & `spit-0.1.9/spit/r_scripts/hclust.R`

 * *Files identical despite different names*

### Comparing `spit-0.1.8/spit/r_scripts/tximport_quant_files.R` & `spit-0.1.9/spit/r_scripts/tximport_quant_files.R`

 * *Files identical despite different names*

### Comparing `spit-0.1.8/spit/run_spit.py` & `spit-0.1.9/spit/run_spit.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.8/spit/spit_test.py` & `spit-0.1.9/spit/spit_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,40 +98,37 @@
         s = int(ctrl_sample_size/2)
         tx_matrix = np.transpose(IFs[samples].to_numpy()).astype(float)
         m_1, m_2 = get_random_halves(tx_matrix, s)
         if(s <= 16):
             m_1 = complete_w_rand_samples(m_1, ctrl_sample_size)
             m_2 = complete_w_rand_samples(m_2, case_sample_size)
             p_arr, min_it_p_val = run_mann_whitney_u(m_1, m_2)
-            min_it_p_val = np.sort(p_arr)[int(num_of_it*0.05)]
+            min_it_p_val = np.random.choice(np.sort(p_arr)[0:int(m_1.shape[1]*0.01)])
         elif(s>n_small):
             rand_if = random.uniform(0, 1)
             m_1_left, m_1_right = split_distributions(m_1, rand_if)
             m_2_left, m_2_right = split_distributions(m_2, rand_if)
             m_1_left_f, m_2_left_f = filter_on_sample_size(m_1_left, m_2_left, n_small)
             m_1_right_f, m_2_right_f = filter_on_sample_size(m_1_right, m_2_right, n_small)
             min_it_p_val, p_arr = compare_tails(m_1_left_f, m_1_right_f, m_2_left_f, m_2_right_f)
         else:
             p_arr, min_it_p_val = run_mann_whitney_u(m_1, m_2)
         if(min_it_p_val == 1 | len(p_arr) == 0):
             pass
         perm_p_arr.append(p_arr)
-        if(s <= 16):
-            i = int(num_of_it*0.05)
-            min_tx_ind = np.argsort(p_arr)[i]
-        else:
+        if (s > 16):
             i = 0
             min_tx_ind = np.nanargmin(p_arr)
-        while((min_tx_ind in sampled_txs) and (len(sampled_txs) < tx_matrix.shape[1])):
-            i+=1
-            min_tx_ind = np.argsort(p_arr)[i]
-            if(np.isnan(p_arr[min_tx_ind])):
-                break
-        sampled_txs.add(min_tx_ind)
-        min_it_p_val = p_arr[min_tx_ind]
+            while((min_tx_ind in sampled_txs) and (len(sampled_txs) < tx_matrix.shape[1])):
+                i+=1
+                min_tx_ind = np.argsort(p_arr)[i]
+                if(np.isnan(p_arr[min_tx_ind])):
+                    break
+            sampled_txs.add(min_tx_ind)
+            min_it_p_val = p_arr[min_tx_ind]
         min_perm_p_arr.append(min_it_p_val)
     perm_p_medians = pd.DataFrame(np.transpose(np.array(perm_p_arr))).set_index(IFs.index).median(axis = 1)
     return min_perm_p_arr, perm_p_medians
 
 def write_min_p_values(min_perm_p_arr, p_values_file):
     p_cutoff = np.min(np.array(min_perm_p_arr))
     with open(p_values_file, 'w') as f:
```

### Comparing `spit-0.1.8/spit/transform_tx_counts_to_ifs.py` & `spit-0.1.9/spit/transform_tx_counts_to_ifs.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.8/spit.egg-info/SOURCES.txt` & `spit-0.1.9/spit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

