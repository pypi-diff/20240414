# Comparing `tmp/pydecs-2024.4.14.tar.gz` & `tmp/pydecs-2024.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydecs-2024.4.14.tar", last modified: Sun Apr 14 03:33:07 2024, max compression
+gzip compressed data, was "pydecs-2024.4.6.tar", last modified: Sat Apr  6 08:01:57 2024, max compression
```

## Comparing `pydecs-2024.4.14.tar` & `pydecs-2024.4.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2024-04-14 03:33:07.851205 pydecs-2024.4.14/
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    11357 2024-04-14 03:32:21.000000 pydecs-2024.4.14/LICENSE.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      647 2024-04-14 03:33:07.851205 pydecs-2024.4.14/PKG-INFO
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      484 2024-04-14 03:32:21.000000 pydecs-2024.4.14/README.md
-drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2024-04-14 03:33:07.427771 pydecs-2024.4.14/pydecs/
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      257 2024-04-14 03:32:21.000000 pydecs-2024.4.14/pydecs/__init__.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    36214 2024-04-14 03:32:21.000000 pydecs-2024.4.14/pydecs/aux_EdefCorrection_VASP.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     2700 2024-04-14 03:32:21.000000 pydecs-2024.4.14/pydecs/aux_check_equilibrium_phases.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     6569 2024-04-14 03:32:21.000000 pydecs-2024.4.14/pydecs/aux_convDOS.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1343 2024-04-14 03:32:21.000000 pydecs-2024.4.14/pydecs/aux_convGasEne.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1855 2024-04-14 03:32:21.000000 pydecs-2024.4.14/pydecs/aux_plot_defectdata.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      671 2024-04-14 03:32:21.000000 pydecs-2024.4.14/pydecs/common.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    13630 2024-04-14 03:32:21.000000 pydecs-2024.4.14/pydecs/defects.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    22348 2024-04-14 03:32:21.000000 pydecs-2024.4.14/pydecs/eqcond.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     7104 2024-04-14 03:32:21.000000 pydecs-2024.4.14/pydecs/host.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    68569 2024-04-14 03:32:21.000000 pydecs-2024.4.14/pydecs/inout.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     4681 2024-04-14 03:32:21.000000 pydecs-2024.4.14/pydecs/pydecs.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     9491 2024-04-14 03:32:21.000000 pydecs-2024.4.14/pydecs/reference_phases.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    32689 2024-04-14 03:32:21.000000 pydecs-2024.4.14/pydecs/solver.py
-drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2024-04-14 03:33:07.811900 pydecs-2024.4.14/pydecs.egg-info/
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      647 2024-04-14 03:33:06.000000 pydecs-2024.4.14/pydecs.egg-info/PKG-INFO
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      570 2024-04-14 03:33:06.000000 pydecs-2024.4.14/pydecs.egg-info/SOURCES.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2024-04-14 03:33:06.000000 pydecs-2024.4.14/pydecs.egg-info/dependency_links.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      420 2024-04-14 03:33:06.000000 pydecs-2024.4.14/pydecs.egg-info/entry_points.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2024-04-14 03:33:05.000000 pydecs-2024.4.14/pydecs.egg-info/not-zip-safe
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       35 2024-04-14 03:33:06.000000 pydecs-2024.4.14/pydecs.egg-info/requires.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        7 2024-04-14 03:33:06.000000 pydecs-2024.4.14/pydecs.egg-info/top_level.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       91 2024-04-14 03:32:21.000000 pydecs-2024.4.14/pyproject.toml
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1098 2024-04-14 03:33:07.882488 pydecs-2024.4.14/setup.cfg
+drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2024-04-06 08:01:57.842695 pydecs-2024.4.6/
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    11357 2024-04-06 07:44:30.000000 pydecs-2024.4.6/LICENSE.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      646 2024-04-06 08:01:57.834600 pydecs-2024.4.6/PKG-INFO
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      484 2024-04-06 07:44:30.000000 pydecs-2024.4.6/README.md
+drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2024-04-06 08:01:57.596332 pydecs-2024.4.6/pydecs/
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      257 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/__init__.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    36214 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/aux_EdefCorrection_VASP.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     2700 2024-04-06 07:59:58.000000 pydecs-2024.4.6/pydecs/aux_check_equilibrium_phases.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     6569 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/aux_convDOS.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1343 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/aux_convGasEne.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1855 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/aux_plot_defectdata.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      671 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/common.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    13630 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/defects.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    22348 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/eqcond.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     7104 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/host.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    67472 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/inout.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     4681 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/pydecs.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     9491 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/reference_phases.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    32689 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/solver.py
+drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2024-04-06 08:01:57.816057 pydecs-2024.4.6/pydecs.egg-info/
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      646 2024-04-06 08:01:56.000000 pydecs-2024.4.6/pydecs.egg-info/PKG-INFO
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      570 2024-04-06 08:01:57.000000 pydecs-2024.4.6/pydecs.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2024-04-06 08:01:56.000000 pydecs-2024.4.6/pydecs.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      420 2024-04-06 08:01:56.000000 pydecs-2024.4.6/pydecs.egg-info/entry_points.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2024-04-06 08:01:56.000000 pydecs-2024.4.6/pydecs.egg-info/not-zip-safe
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       35 2024-04-06 08:01:56.000000 pydecs-2024.4.6/pydecs.egg-info/requires.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        7 2024-04-06 08:01:56.000000 pydecs-2024.4.6/pydecs.egg-info/top_level.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       91 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pyproject.toml
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1098 2024-04-06 08:01:57.853235 pydecs-2024.4.6/setup.cfg
```

### Comparing `pydecs-2024.4.14/LICENSE.txt` & `pydecs-2024.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.14/PKG-INFO` & `pydecs-2024.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydecs
-Version: 2024.4.14
+Version: 2024.4.6
 Summary: This tool enables us to analyze equilibrium concentrations of point and complex defects in crystalline solids
 Home-page: https://gitlab.com/tkog/pydecs
 Author: Takafumi Ogawa
 Author-email: takafumi.ogawa.1+pydecs@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `pydecs-2024.4.14/pydecs/aux_EdefCorrection_VASP.py` & `pydecs-2024.4.6/pydecs/aux_EdefCorrection_VASP.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.14/pydecs/aux_check_equilibrium_phases.py` & `pydecs-2024.4.6/pydecs/aux_check_equilibrium_phases.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.14/pydecs/aux_convDOS.py` & `pydecs-2024.4.6/pydecs/aux_convDOS.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.14/pydecs/aux_convGasEne.py` & `pydecs-2024.4.6/pydecs/aux_convGasEne.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.14/pydecs/aux_plot_defectdata.py` & `pydecs-2024.4.6/pydecs/aux_plot_defectdata.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.14/pydecs/common.py` & `pydecs-2024.4.6/pydecs/common.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.14/pydecs/defects.py` & `pydecs-2024.4.6/pydecs/defects.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.14/pydecs/eqcond.py` & `pydecs-2024.4.6/pydecs/eqcond.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.14/pydecs/host.py` & `pydecs-2024.4.6/pydecs/host.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.14/pydecs/inout.py` & `pydecs-2024.4.6/pydecs/inout.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,32 +524,24 @@
             str1+=f"{k2}, "
         elif k1=="T":
             str1+=f"temperature, "
         elif k1=="fix_Natoms":
             for v2 in v1:
                 k2=f"fix_Natoms_{v2['element']}"
                 str1+=f"{k2}, "
-        elif k1=="fix_Natoms_linked":
-            for v2 in v1:
-                k2=f"fix_Natoms_linked_{v2['element']}"
-                str1+=f"{k2}, "
         else:
             str1+=f"{k1}, "
     fout1.write(str1[:-2]+"\n")
     for ieq1,eqc1 in enumerate(eqcond_list_in):
         str1=f"{ieq1+1:04}, "
         for k1,v1 in eqc1.items():
             if k1=="fix_Natoms":
                 for v2 in v1:
                     v3=f"{v2['target_Natoms']}"
                     str1+=f"{v3}, "
-            if k1=="fix_Natoms_linked":
-                for v2 in v1:
-                    v3=f"{v2['target_Natoms']}"
-                    str1+=f"{v3}, "
             else:
                 str1+=f"{v1}, "
         fout1.write(str1[:-2]+"\n")
     fout1.close()
 
 def output_density_with_eqcond(dens_in,eqcond_in,out_filename):
     add_list=[]
@@ -811,56 +803,38 @@
         if plot_params_in["dens_xaxis_parameter"].find("pressure_")==0:
             plot_params_in["dens_xaxis_log"]=True
         else:
             plot_params_in["dens_xaxis_log"]=False
 
     parameters_list_main=[]
     parameters_list_exclmain={}
-    lambda_including=[]
-    fix_Natoms_linked_including=[]
-    for k1,v1 in parameters_list2.items():
-        if k1.find("lambda_")==0:
-            lambda_including.append(k1)
-        if k1.find("fix_Natoms_linked_")==0:
-            fix_Natoms_linked_including.append(k1)
-    cnt_lambda = len(lambda_including)-1
-    bool_fix_Natoms_linked = False
-    if len(fix_Natoms_linked_including) > 1:
-        bool_fix_Natoms_linked = True
+    bool_rmlambda=False
+    bool_rmchempot=False
+    bool_rmpressure=True
+    if plot_params_in["dens_xaxis_parameter"].find("lambda_")==0:
+        bool_rmlambda=True
+        bool_rmchempot=True
+    if plot_params_in["dens_xaxis_parameter"].find("chempot_")==0:
+        bool_rmlambda=True
+        bool_rmchempot=True
+        bool_rmpressure=True
     for k1,v1 in parameters_list2.items():
         if k1==plot_params_in["dens_xaxis_parameter"]:
             parameters_list_main=v1
         else:
-            if plot_params_in["dens_xaxis_parameter"].find("chempot_")==0:
-                if k1.find("pressure_")==0 or k1.find("fix_Natoms_")==0 \
-                        or k1.find("lambda_")==0:
-                    continue
-                if k1.find("chempot_")==0 and len(lambda_including)==1:
-                    continue
-                if k1.find("chempot_")==0 and cnt_lambda>0:
-                    cnt_lambda-=1
-                    continue
+            if bool_rmlambda and k1.find("lambda_")==0:
+                if plot_params_in["dens_xaxis_parameter"].find("lambda_")==0:
+                    bool_rmlambda=False
+            elif bool_rmchempot and k1.find("chempot_")==0:
+                if plot_params_in["dens_xaxis_parameter"].find("chempot_")==0:
+                    bool_rmchempot=False
+            elif bool_rmpressure and k1.find("pressure_")==0:
+                a1=1
             else:
-                if k1.find("chempot_")==0:
-                    continue
-                if k1.find("lambda_")==0 and cnt_lambda>0:
-                    cnt_lambda-=1
-                    continue
-                if k1.find("fix_Natoms_linked_")==0:
-                    if plot_params_in["dens_xaxis_parameter"].find("fix_Natoms_linked_")==0:
-                        continue
-                    if bool_fix_Natoms_linked:
-                        bool_fix_Natoms_linked = False
-                        parameters_list_exclmain[k1]=v1
-                        continue
-                    else:
-                        continue
-            parameters_list_exclmain[k1]=v1
-    # print(parameters_list_exclmain)
-    # print(parameters_list_main)
+                parameters_list_exclmain[k1]=v1
 
     if len(parameters_list_main)<=3:
         print(f" WARNING(plot)::Num. of dens_xaxis_parameter values is very small!")
         fout1.write(f" WARNING(plot)::Num. of dens_xaxis_parameter values is very small!\n")
     if plot_params_in["dens_x_lower_limit"]=="NONE":
         plot_params_in["dens_x_lower_limit"]=min(parameters_list_main)
     if plot_params_in["dens_x_upper_limit"]=="NONE":
```

### Comparing `pydecs-2024.4.14/pydecs/pydecs.py` & `pydecs-2024.4.6/pydecs/pydecs.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.14/pydecs/reference_phases.py` & `pydecs-2024.4.6/pydecs/reference_phases.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.14/pydecs/solver.py` & `pydecs-2024.4.6/pydecs/solver.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.14/pydecs.egg-info/PKG-INFO` & `pydecs-2024.4.6/pydecs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydecs
-Version: 2024.4.14
+Version: 2024.4.6
 Summary: This tool enables us to analyze equilibrium concentrations of point and complex defects in crystalline solids
 Home-page: https://gitlab.com/tkog/pydecs
 Author: Takafumi Ogawa
 Author-email: takafumi.ogawa.1+pydecs@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `pydecs-2024.4.14/pydecs.egg-info/SOURCES.txt` & `pydecs-2024.4.6/pydecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.14/setup.cfg` & `pydecs-2024.4.6/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydecs
-version = 2024.04.14
+version = 2024.04.06
 description = This tool enables us to analyze equilibrium concentrations of point and complex defects in crystalline solids
 author = Takafumi Ogawa
 author_email = takafumi.ogawa.1+pydecs@gmail.com
 url = https://gitlab.com/tkog/pydecs
 lisense_file = LICENSE.txt
 classifiers = 
 	Intended Audience :: Science/Research
```

