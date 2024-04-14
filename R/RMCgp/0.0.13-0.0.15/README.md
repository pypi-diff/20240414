# Comparing `tmp/RMCgp-0.0.13.tar.gz` & `tmp/RMCgp-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RMCgp-0.0.13.tar", last modified: Thu Apr  4 01:49:24 2024, max compression
+gzip compressed data, was "RMCgp-0.0.15.tar", last modified: Sun Apr 14 05:04:49 2024, max compression
```

## Comparing `RMCgp-0.0.13.tar` & `RMCgp-0.0.15.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-04 01:49:24.796918 RMCgp-0.0.13/
--rw-r--r--   0 taung      (501) staff       (20)    11344 2024-03-29 05:02:13.000000 RMCgp-0.0.13/LICENSE.txt
--rw-r--r--   0 taung      (501) staff       (20)      807 2024-04-04 01:49:24.796659 RMCgp-0.0.13/PKG-INFO
--rw-r--r--   0 taung      (501) staff       (20)     2065 2024-03-29 06:55:32.000000 RMCgp-0.0.13/README.md
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-04 01:49:24.792339 RMCgp-0.0.13/RMC/
--rw-r--r--   0 taung      (501) staff       (20)      194 2024-03-29 03:57:09.000000 RMCgp-0.0.13/RMC/__init__.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-04 01:49:24.792795 RMCgp-0.0.13/RMC/costfunctions/
--rw-r--r--   0 taung      (501) staff       (20)       87 2024-04-01 23:53:14.000000 RMCgp-0.0.13/RMC/costfunctions/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)      908 2024-04-02 05:45:17.000000 RMCgp-0.0.13/RMC/costfunctions/finalCosts.py
--rw-r--r--   0 taung      (501) staff       (20)     2234 2024-04-02 00:02:53.000000 RMCgp-0.0.13/RMC/costfunctions/runningCosts.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-04 01:49:24.793079 RMCgp-0.0.13/RMC/design/
--rw-r--r--   0 taung      (501) staff       (20)       45 2024-03-29 03:57:09.000000 RMCgp-0.0.13/RMC/design/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)      943 2024-04-03 23:22:58.000000 RMCgp-0.0.13/RMC/design/generate_design.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-04 01:49:24.793355 RMCgp-0.0.13/RMC/emulator/
--rw-r--r--   0 taung      (501) staff       (20)     1372 2024-03-29 03:57:09.000000 RMCgp-0.0.13/RMC/emulator/GP.py
--rw-r--r--   0 taung      (501) staff       (20)       33 2024-03-29 03:57:09.000000 RMCgp-0.0.13/RMC/emulator/__init__.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-04 01:49:24.793935 RMCgp-0.0.13/RMC/model/
--rw-r--r--   0 taung      (501) staff       (20)       43 2024-03-29 03:57:09.000000 RMCgp-0.0.13/RMC/model/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)     1834 2024-04-02 00:55:41.000000 RMCgp-0.0.13/RMC/model/hybridcontrol.py
--rw-r--r--   0 taung      (501) staff       (20)    10355 2024-04-04 01:22:21.000000 RMCgp-0.0.13/RMC/model/hybridrunner.py
--rw-r--r--   0 taung      (501) staff       (20)      376 2024-04-02 00:24:04.000000 RMCgp-0.0.13/RMC/model/test_inputs.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-04 01:49:24.794412 RMCgp-0.0.13/RMC/optimization/
--rw-r--r--   0 taung      (501) staff       (20)       49 2024-03-29 03:57:09.000000 RMCgp-0.0.13/RMC/optimization/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)     1973 2024-04-04 00:16:01.000000 RMCgp-0.0.13/RMC/optimization/onestepOptimization.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-04 01:49:24.795146 RMCgp-0.0.13/RMC/simulate/
--rw-r--r--   0 taung      (501) staff       (20)      652 2024-03-29 03:57:09.000000 RMCgp-0.0.13/RMC/simulate/CIR.py
--rw-r--r--   0 taung      (501) staff       (20)      635 2024-03-29 03:57:09.000000 RMCgp-0.0.13/RMC/simulate/OU.py
--rw-r--r--   0 taung      (501) staff       (20)       62 2024-03-29 03:57:09.000000 RMCgp-0.0.13/RMC/simulate/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)     3417 2024-04-03 21:15:18.000000 RMCgp-0.0.13/RMC/simulate/sim.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-04 01:49:24.796061 RMCgp-0.0.13/RMCgp.egg-info/
--rw-r--r--   0 taung      (501) staff       (20)      807 2024-04-04 01:49:24.000000 RMCgp-0.0.13/RMCgp.egg-info/PKG-INFO
--rw-r--r--   0 taung      (501) staff       (20)      664 2024-04-04 01:49:24.000000 RMCgp-0.0.13/RMCgp.egg-info/SOURCES.txt
--rw-r--r--   0 taung      (501) staff       (20)        1 2024-04-04 01:49:24.000000 RMCgp-0.0.13/RMCgp.egg-info/dependency_links.txt
--rw-r--r--   0 taung      (501) staff       (20)        1 2024-04-04 01:49:24.000000 RMCgp-0.0.13/RMCgp.egg-info/not-zip-safe
--rw-r--r--   0 taung      (501) staff       (20)      137 2024-04-04 01:49:24.000000 RMCgp-0.0.13/RMCgp.egg-info/requires.txt
--rw-r--r--   0 taung      (501) staff       (20)        4 2024-04-04 01:49:24.000000 RMCgp-0.0.13/RMCgp.egg-info/top_level.txt
--rw-r--r--   0 taung      (501) staff       (20)       38 2024-04-04 01:49:24.796972 RMCgp-0.0.13/setup.cfg
--rw-r--r--   0 taung      (501) staff       (20)     1474 2024-04-04 01:49:19.000000 RMCgp-0.0.13/setup.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-14 05:04:49.353339 RMCgp-0.0.15/
+-rw-r--r--   0 taung      (501) staff       (20)    11344 2024-03-29 05:02:13.000000 RMCgp-0.0.15/LICENSE.txt
+-rw-r--r--   0 taung      (501) staff       (20)      807 2024-04-14 05:04:49.353098 RMCgp-0.0.15/PKG-INFO
+-rw-r--r--   0 taung      (501) staff       (20)     2065 2024-03-29 06:55:32.000000 RMCgp-0.0.15/README.md
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-14 05:04:49.344726 RMCgp-0.0.15/RMC/
+-rw-r--r--   0 taung      (501) staff       (20)      194 2024-03-29 03:57:09.000000 RMCgp-0.0.15/RMC/__init__.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-14 05:04:49.345629 RMCgp-0.0.15/RMC/costfunctions/
+-rw-r--r--   0 taung      (501) staff       (20)       87 2024-04-01 23:53:14.000000 RMCgp-0.0.15/RMC/costfunctions/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)      908 2024-04-02 05:45:17.000000 RMCgp-0.0.15/RMC/costfunctions/finalCosts.py
+-rw-r--r--   0 taung      (501) staff       (20)     2234 2024-04-02 00:02:53.000000 RMCgp-0.0.15/RMC/costfunctions/runningCosts.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-14 05:04:49.346258 RMCgp-0.0.15/RMC/design/
+-rw-r--r--   0 taung      (501) staff       (20)       45 2024-03-29 03:57:09.000000 RMCgp-0.0.15/RMC/design/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)      943 2024-04-03 23:22:58.000000 RMCgp-0.0.15/RMC/design/generate_design.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-14 05:04:49.347002 RMCgp-0.0.15/RMC/emulator/
+-rw-r--r--   0 taung      (501) staff       (20)     1372 2024-03-29 03:57:09.000000 RMCgp-0.0.15/RMC/emulator/GP.py
+-rw-r--r--   0 taung      (501) staff       (20)       33 2024-03-29 03:57:09.000000 RMCgp-0.0.15/RMC/emulator/__init__.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-14 05:04:49.348593 RMCgp-0.0.15/RMC/model/
+-rw-r--r--   0 taung      (501) staff       (20)       43 2024-03-29 03:57:09.000000 RMCgp-0.0.15/RMC/model/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)     1834 2024-04-02 00:55:41.000000 RMCgp-0.0.15/RMC/model/hybridcontrol.py
+-rw-r--r--   0 taung      (501) staff       (20)    10628 2024-04-14 00:34:05.000000 RMCgp-0.0.15/RMC/model/hybridrunner.py
+-rw-r--r--   0 taung      (501) staff       (20)      376 2024-04-02 00:24:04.000000 RMCgp-0.0.15/RMC/model/test_inputs.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-14 05:04:49.349148 RMCgp-0.0.15/RMC/optimization/
+-rw-r--r--   0 taung      (501) staff       (20)       49 2024-03-29 03:57:09.000000 RMCgp-0.0.15/RMC/optimization/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)     1973 2024-04-04 00:16:01.000000 RMCgp-0.0.15/RMC/optimization/onestepOptimization.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-14 05:04:49.350764 RMCgp-0.0.15/RMC/simulate/
+-rw-r--r--   0 taung      (501) staff       (20)      678 2024-04-13 22:03:27.000000 RMCgp-0.0.15/RMC/simulate/CIR.py
+-rw-r--r--   0 taung      (501) staff       (20)      661 2024-04-13 22:03:23.000000 RMCgp-0.0.15/RMC/simulate/OU.py
+-rw-r--r--   0 taung      (501) staff       (20)       87 2024-04-13 22:45:04.000000 RMCgp-0.0.15/RMC/simulate/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)      685 2024-04-13 22:45:29.000000 RMCgp-0.0.15/RMC/simulate/jacobi.py
+-rw-r--r--   0 taung      (501) staff       (20)     3895 2024-04-13 22:34:36.000000 RMCgp-0.0.15/RMC/simulate/sim.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-14 05:04:49.352245 RMCgp-0.0.15/RMCgp.egg-info/
+-rw-r--r--   0 taung      (501) staff       (20)      807 2024-04-14 05:04:49.000000 RMCgp-0.0.15/RMCgp.egg-info/PKG-INFO
+-rw-r--r--   0 taung      (501) staff       (20)      687 2024-04-14 05:04:49.000000 RMCgp-0.0.15/RMCgp.egg-info/SOURCES.txt
+-rw-r--r--   0 taung      (501) staff       (20)        1 2024-04-14 05:04:49.000000 RMCgp-0.0.15/RMCgp.egg-info/dependency_links.txt
+-rw-r--r--   0 taung      (501) staff       (20)        1 2024-04-14 05:04:49.000000 RMCgp-0.0.15/RMCgp.egg-info/not-zip-safe
+-rw-r--r--   0 taung      (501) staff       (20)      137 2024-04-14 05:04:49.000000 RMCgp-0.0.15/RMCgp.egg-info/requires.txt
+-rw-r--r--   0 taung      (501) staff       (20)        4 2024-04-14 05:04:49.000000 RMCgp-0.0.15/RMCgp.egg-info/top_level.txt
+-rw-r--r--   0 taung      (501) staff       (20)       38 2024-04-14 05:04:49.353388 RMCgp-0.0.15/setup.cfg
+-rw-r--r--   0 taung      (501) staff       (20)     1474 2024-04-14 05:03:59.000000 RMCgp-0.0.15/setup.py
```

### Comparing `RMCgp-0.0.13/LICENSE.txt` & `RMCgp-0.0.15/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.13/PKG-INFO` & `RMCgp-0.0.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RMCgp
-Version: 0.0.13
+Version: 0.0.15
 Summary: RMC for stochastic control.
 Home-page: https://github.com/thihaa2019/RMCgp
 Author: Thiha Aung
 Author-email: taung@ucsb.edu
 Maintainer: Thiha Aung
 Maintainer-email: taung@ucsb.edu
 License: Apache-2.0
```

### Comparing `RMCgp-0.0.13/README.md` & `RMCgp-0.0.15/README.md`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.13/RMC/costfunctions/finalCosts.py` & `RMCgp-0.0.15/RMC/costfunctions/finalCosts.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.13/RMC/costfunctions/runningCosts.py` & `RMCgp-0.0.15/RMC/costfunctions/runningCosts.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.13/RMC/design/generate_design.py` & `RMCgp-0.0.15/RMC/design/generate_design.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.13/RMC/emulator/GP.py` & `RMCgp-0.0.15/RMC/emulator/GP.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.13/RMC/model/hybridcontrol.py` & `RMCgp-0.0.15/RMC/model/hybridcontrol.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.13/RMC/model/hybridrunner.py` & `RMCgp-0.0.15/RMC/model/hybridrunner.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,33 +98,37 @@
 
         value_map = valueGP(value_input,value_output,kernel= kern,normalizer=True)
         value_map.optimize()
         self.MSE_evaluation(value_output.flatten(),value_map.predict(value_input)[0].flatten(),"Value")
         return value_map
     
     def v_evaluation(self,X_prev,drift_p1,drift_p2,vol_p1,vol_p2,I_next,policy_map,value_map,*args):
-        target,lower_target,upper_target = args
+        target,lower_target,upper_target,step = args
         assert isinstance(target,(int,float)), "One step target is a scalar"
         reshape_dim = 1 # no reshaping
         X_prev_rep = X_prev
         I_next_rep = I_next
         if self.batch_size!=0:  
             reshape_dim = self.batch_size
             X_prev_rep= np.repeat(X_prev,self.batch_size)
             I_next_rep= np.repeat(I_next,self.batch_size)
 
-        X_next_rep= self.process.onestepsimulate(int(self.nsim*reshape_dim),X_prev_rep,drift_p1,drift_p2,vol_p1,vol_p2)
+        X_next_rep= self.process.onestepsimulate(int(self.nsim*reshape_dim),X_prev_rep,drift_p1,drift_p2,vol_p1,vol_p2,step)
         power_outputs = policy_map.predict(np.column_stack((X_next_rep,I_next_rep)))[0].flatten()
         LB = np.maximum(self.Bmin,self.charging_eff*(self.Ilb- I_next_rep)/self.dt)
         UB = np.minimum(self.Bmax,(self.Iub-I_next_rep)/(self.charging_eff*self.dt))
-
         pos_outputs = np.where(power_outputs>0)
-        # cannot charge more than X is available
+        # When X> M , cap B>0 by X-B, do not charge more and make Ot< Mt, when Ot guaranteed > M given X
         upper_charging_bound  = np.maximum(X_next_rep[pos_outputs]-target,0)
         power_outputs[pos_outputs] = np.minimum(power_outputs[pos_outputs],upper_charging_bound)
+
+        # DO NOT CHARGE WHEN X < M, otherwise Ot= X-B < X< M
+        # Dont make undersupply worse
+        idx = (X_next_rep < target ) & (power_outputs>0)
+        power_outputs[idx]=0
         power_outputs = np.maximum(LB,np.minimum(power_outputs,UB))
         I_nextnext = I_next_rep + power_outputs *(self.charging_eff *(power_outputs>0) + 1/self.charging_eff * (power_outputs<0))*self.dt
         if isinstance(value_map,final_SOCcontraint):
             pointwise_v = self.running_cost.cost(power_outputs,X_next_rep,target,lower_target,upper_target) * self.dt + value_map.cost(I_nextnext)
         if isinstance(value_map,GPy.core.GP):
             inp = np.column_stack((X_next_rep,I_nextnext))
             pointwise_v = self.running_cost.cost(power_outputs,X_next_rep,target,lower_target,upper_target) * self.dt + value_map.predict(inp)[0].flatten()
@@ -138,42 +142,42 @@
         # need to be fixed
         #self.X_lowers[0] = self.process.mean_vec[0] - 2.5*self.process.std_vec[3]
         #self.X_uppers[0] = self.process.mean_vec[0] + 2.5*self.process.std_vec[3]
 
         self.values[-1] = self.final_cost 
         X_prev,I_next = design_generator(self.nsim,self.X_lowers[-3],self.X_uppers[-3],self.Ilb,self.Iub).create_samples
         X_next = self.process.onestepsimulate(self.nsim,X_prev,self.process.drift_p1[-2],self.process.drift_p2[-2],\
-                                              self.process.diffusion_p1[-2],self.process.diffusion_p2[-2])
+                                              self.process.diffusion_p1[-2],self.process.diffusion_p2[-2],-2)
         self.policies[-1] = self.train_policy(X_next,I_next,self.values[-1],self.targets[-1],self.lower_targets[-1],self.upper_targets[-1])
 
         
         pointwise_values = self.v_evaluation(X_prev,self.process.drift_p1[-2],self.process.drift_p2[-2],\
                                              self.process.diffusion_p1[-2],self.process.diffusion_p2[-2],\
                                              I_next,self.policies[-1],self.values[-1],\
-                                                self.targets[-1],self.lower_targets[-1],self.upper_targets[-1])
+                                                self.targets[-1],self.lower_targets[-1],self.upper_targets[-1],-2)
         
         for iStep in range(self.nstep-1,0,-1):
             self.values[iStep-1] = self.train_value(X_prev,I_next,pointwise_values)
 
             print("Timestep: "+ str(self.t[iStep]))
 
             print("_"*50)
 
             if iStep!=1:
                 X_prev,I_next = design_generator(self.nsim,self.X_lowers[iStep-2],self.X_uppers[iStep-2],self.Ilb,self.Iub).create_samples
                 X_next = self.process.onestepsimulate(self.nsim,X_prev,self.process.drift_p1[iStep-2],self.process.drift_p2[iStep-2],\
-                                                self.process.diffusion_p1[iStep-2],self.process.diffusion_p2[iStep-2])
+                                                self.process.diffusion_p1[iStep-2],self.process.diffusion_p2[iStep-2],iStep-2)
 
                 self.policies[iStep-1] = self.train_policy(X_next,I_next,self.values[iStep-1],self.targets[iStep-1],self.lower_targets[iStep-1],self.upper_targets[iStep-1])
 
         
                 pointwise_values = self.v_evaluation(X_prev,self.process.drift_p1[iStep-2],self.process.drift_p2[iStep-2],\
                                              self.process.diffusion_p1[iStep-2],self.process.diffusion_p2[iStep-2],\
                                              I_next,self.policies[iStep-1],self.values[iStep-1],\
-                                            self.targets[iStep-1],self.lower_targets[iStep-1],self.upper_targets[iStep-1])
+                                            self.targets[iStep-1],self.lower_targets[iStep-1],self.upper_targets[iStep-1],iStep-2)
         
             else:
                 X_0,I_0 = design_generator(self.nsim,self.X_lowers[0],self.X_uppers[0],self.Ilb,self.Iub).create_samples
                 #self.optimizer.q = self.values[iStep-1]
                 self.policies[iStep-1] = self.train_policy(X_0,I_0,self.values[iStep-1],self.targets[iStep-1],self.lower_targets[iStep-1],self.upper_targets[iStep-1])
                 print("Timestep: "+ str(self.t[iStep-1]))
                 print("_"*50)
```

### Comparing `RMCgp-0.0.13/RMC/optimization/onestepOptimization.py` & `RMCgp-0.0.15/RMC/optimization/onestepOptimization.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.13/RMC/simulate/CIR.py` & `RMCgp-0.0.15/RMC/simulate/jacobi.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from .sim import Sim
 import numpy as np
 
-class CIR(Sim):
-    def __init__(self,X0,nstep,nsim,maturity,mean_rev_rate,mean_rev_levels,vol):
+class Jacobi(Sim):
+    def __init__(self,X0,nstep,nsim,maturity,mean_rev_rate,mean_rev_levels,vol,UB,LB,noises):
         self.mean_rev_rate = mean_rev_rate
         self.mean_rev_levels = mean_rev_levels
         self.sigmas = vol
 
-        super(CIR,self).__init__(X0,nstep,nsim,maturity,(self.mean_rev_rate,self.mean_rev_levels),self.drift_func,\
-                                (self.sigmas,self.mean_rev_levels),self.diffusion_func)
+        super(Jacobi,self).__init__(X0,nstep,nsim,maturity,(self.mean_rev_rate,self.mean_rev_levels),self.drift_func,\
+                                (self.sigmas,self.mean_rev_levels),self.diffusion_func,UB,LB,noises)
 
 
     @staticmethod
     def drift_func(alpha_t,m_t,x_t):
         return  alpha_t * (m_t- x_t)
 
     @staticmethod
     def diffusion_func(sigma_t,m_t,x_t):
-        return sigma_t * np.sqrt(x_t)
-
+        return sigma_t *(x_t) * (1-x_t)
```

### Comparing `RMCgp-0.0.13/RMC/simulate/OU.py` & `RMCgp-0.0.15/RMC/simulate/CIR.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from .sim import Sim
 import numpy as np
-class OU(Sim):
 
-    def __init__(self,X0,nstep,nsim,maturity,mean_rev_rate,mean_rev_levels,vol):
+class CIR(Sim):
+    def __init__(self,X0,nstep,nsim,maturity,mean_rev_rate,mean_rev_levels,vol,UB,LB,noises):
         self.mean_rev_rate = mean_rev_rate
         self.mean_rev_levels = mean_rev_levels
         self.sigmas = vol
 
-        super(OU,self).__init__(X0,nstep,nsim,maturity,(self.mean_rev_rate,self.mean_rev_levels),self.drift_func,\
-                                (self.sigmas,self.mean_rev_levels),self.diffusion_func)
+        super(CIR,self).__init__(X0,nstep,nsim,maturity,(self.mean_rev_rate,self.mean_rev_levels),self.drift_func,\
+                                (self.sigmas,self.mean_rev_levels),self.diffusion_func,UB,LB,noises)
 
 
     @staticmethod
     def drift_func(alpha_t,m_t,x_t):
         return  alpha_t * (m_t- x_t)
 
     @staticmethod
     def diffusion_func(sigma_t,m_t,x_t):
-        return sigma_t
+        return sigma_t * np.sqrt(x_t)
```

### Comparing `RMCgp-0.0.13/RMC/simulate/sim.py` & `RMCgp-0.0.15/RMC/simulate/sim.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,31 +3,41 @@
 class Sim():
 
     """
     drift is a function of 3 parameters p1scalar, p2vector(t), p3X(t)
     
     
     """
-    def __init__(self,X0,nstep,nsim,maturity,drift_parameters,drift_function,diffusion_parameters,diffusion_function):
+    def __init__(self,X0,nstep,nsim,maturity,drift_parameters,drift_function,diffusion_parameters,diffusion_function,UB,LB,noises):
 
         if isinstance(X0,(list,np.ndarray)):
             assert len(X0)==nsim, "X0 and nsim must have same size"
         self.X0 = X0
 
         assert maturity>0, "Maturity cannot be 0 or less."
         assert nstep>0, "Number of steps cannot be 0 or less."
         self.maturity = maturity
         self.nstep    = nstep
         self.dt = maturity/nstep
         self.t = np.linspace(0,maturity,nstep+1)
+        self.UB = UB
+        self.LB = LB
+        # noises must be shape nsimxnstep columns
+
         if nsim==None:
             self.nsim = 10000
         else:
             self.nsim = nsim
 
+        # Standard mean 0 var 1 nosies
+
+        self.noises = noises
+        if self.noises is None:
+            self.noises = np.random.normal(0,1,size = (self.nsim,self.nstep))
+
         self.drift = drift_function
         assert isinstance(drift_parameters[0],(np.ndarray,list)) and isinstance(drift_parameters[1],(np.ndarray,list)),\
             "Drift Parameters must be array"
         self.drift_p1 = drift_parameters[0]
         self.drift_p2 = drift_parameters[1]
         if len(self.drift_p1)==1:
             self.drift_p1 = list(self.drift_p1)* self.nstep
@@ -42,38 +52,40 @@
         if len(self.diffusion_p1)==1:
             self.diffusion_p1 = list(self.diffusion_p1)* self.nstep
         if len(self.diffusion_p2)==1:
             self.diffusion_p2 = list(self.diffusion_p2)* self.nstep
 
         self.sim_trajectories = self.simulate()
     
-    def simulate(self,BM = None,given_BM = False):
+    def simulate(self):
         self.Xs = np.zeros((self.nsim,self.nstep+1))
         self.Xs[:,0] = np.ones(self.nsim)* self.X0
-
-        if not given_BM:
-            dW = np.random.normal(0,1,size = (self.nsim,self.nstep) ) * np.sqrt(self.dt)
-        else:
-            dW = BM
-
+        #normal (0,1) 
+        dW = self.noises
         for i in range(1,self.nstep+1):
             self.Xs[:,i] = np.abs(self.Xs[:,i-1] +self.drift(self.drift_p1[i-1],self.drift_p2[i-1],self.Xs[:,i-1]) * self.dt +\
-                            self.diffusion(self.diffusion_p1[i-1],self.diffusion_p2[i-1],self.Xs[:,i-1])* dW[:,i-1])
+                            self.diffusion(self.diffusion_p1[i-1],self.diffusion_p2[i-1],self.Xs[:,i-1])* dW[:,i-1] * np.sqrt(self.dt))
+            self.Xs[:,i] = np.minimum(self.Xs[:,i],self.UB)
+            self.Xs[:,i] = np.maximum(self.Xs[:,i],self.LB)
         return self.Xs
     @property
     def mean_vec(self):
         return np.mean(self.sim_trajectories,axis = 0)
     @property
     def std_vec(self):
         return np.std(self.sim_trajectories,axis= 0, ddof = 1)
 
-    def onestepsimulate(self,nsim,X_start,drift_p1,drift_p2,vol_p1,vol_p2):
-        dW = np.random.normal(0,1,size = nsim) * np.sqrt(self.dt)
+    def onestepsimulate(self,nsim,X_start,drift_p1,drift_p2,vol_p1,vol_p2,step_num):
+        # boostrap the noises accordingly
+        dW = np.random.choice(self.noises[step_num,:],size=nsim, replace = True)
         X_next = np.abs(X_start +self.drift(drift_p1,drift_p2,X_start) * self.dt +\
-                            self.diffusion(vol_p1,vol_p2,X_start)* dW)
+                            self.diffusion(vol_p1,vol_p2,X_start)* dW * np.sqrt(self.dt))
+        
+        X_next = np.minimum(X_next,self.UB)
+        X_next = np.maximum(X_next,self.LB)
         return X_next.flatten()
     def cor(self,i,j):
         if i <=0 or i >= self.nstep+1:
             raise ValueError("Invalid index for i.")
         if j <= 0 or j >= self.nstep+1:
             raise ValueError("Invalid index for j.")
```

### Comparing `RMCgp-0.0.13/RMCgp.egg-info/PKG-INFO` & `RMCgp-0.0.15/RMCgp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RMCgp
-Version: 0.0.13
+Version: 0.0.15
 Summary: RMC for stochastic control.
 Home-page: https://github.com/thihaa2019/RMCgp
 Author: Thiha Aung
 Author-email: taung@ucsb.edu
 Maintainer: Thiha Aung
 Maintainer-email: taung@ucsb.edu
 License: Apache-2.0
```

### Comparing `RMCgp-0.0.13/RMCgp.egg-info/SOURCES.txt` & `RMCgp-0.0.15/RMCgp.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 RMC/model/hybridrunner.py
 RMC/model/test_inputs.py
 RMC/optimization/__init__.py
 RMC/optimization/onestepOptimization.py
 RMC/simulate/CIR.py
 RMC/simulate/OU.py
 RMC/simulate/__init__.py
+RMC/simulate/jacobi.py
 RMC/simulate/sim.py
 RMCgp.egg-info/PKG-INFO
 RMCgp.egg-info/SOURCES.txt
 RMCgp.egg-info/dependency_links.txt
 RMCgp.egg-info/not-zip-safe
 RMCgp.egg-info/requires.txt
 RMCgp.egg-info/top_level.txt
```

### Comparing `RMCgp-0.0.13/setup.py` & `RMCgp-0.0.15/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "GPy>=1.13.0",
     "scikit-learn>=1.3.0",
     "scipy>=1.1.4",
     "matplotlib>=3.8.0"
 ]
 
 setuptools.setup(name='RMCgp',
-                 version='0.0.13',
+                 version='0.0.15',
                  author='Thiha Aung',
                  author_email='taung@ucsb.edu',
                  maintainer='Thiha Aung',
                  maintainer_email='taung@ucsb.edu',
                  description='RMC for stochastic control.',
                  long_description=readme,
                  url='https://github.com/thihaa2019/RMCgp',
```

