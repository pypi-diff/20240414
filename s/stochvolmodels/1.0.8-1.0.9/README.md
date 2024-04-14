# Comparing `tmp/stochvolmodels-1.0.8.tar.gz` & `tmp/stochvolmodels-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stochvolmodels-1.0.8.tar", max compression
+gzip compressed data, was "stochvolmodels-1.0.9.tar", max compression
```

## Comparing `stochvolmodels-1.0.8.tar` & `stochvolmodels-1.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35802 2022-08-10 05:48:35.000000 stochvolmodels-1.0.8/LICENSE.txt
--rw-r--r--   0        0        0     1594 2023-12-06 15:27:23.673068 stochvolmodels-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     8540 2023-12-03 17:09:02.000000 stochvolmodels-1.0.8/README.md
--rw-r--r--   0        0        0     3345 2023-12-06 14:45:26.728810 stochvolmodels-1.0.8/stochvolmodels/__init__.py
--rw-r--r--   0        0        0        0 2022-08-08 12:33:11.000000 stochvolmodels-1.0.8/stochvolmodels/data/__init__.py
--rw-r--r--   0        0        0    13285 2023-12-05 15:25:41.871241 stochvolmodels-1.0.8/stochvolmodels/data/option_chain.py
--rw-r--r--   0        0        0    63709 2023-11-26 10:08:33.000000 stochvolmodels-1.0.8/stochvolmodels/data/test_option_chain.py
--rw-r--r--   0        0        0        0 2023-12-05 14:56:51.993117 stochvolmodels-1.0.8/stochvolmodels/pricers/__init__.py
--rw-r--r--   0        0        0        0 2022-08-06 06:57:02.000000 stochvolmodels-1.0.8/stochvolmodels/pricers/core/__init__.py
--rw-r--r--   0        0        0    11381 2023-02-26 07:20:57.000000 stochvolmodels-1.0.8/stochvolmodels/pricers/core/bsm_pricer.py
--rw-r--r--   0        0        0      264 2022-08-09 14:55:12.000000 stochvolmodels-1.0.8/stochvolmodels/pricers/core/config.py
--rw-r--r--   0        0        0     1963 2022-11-11 09:13:29.000000 stochvolmodels-1.0.8/stochvolmodels/pricers/core/mc_payoffs.py
--rw-r--r--   0        0        0    13140 2023-12-05 14:29:14.605932 stochvolmodels-1.0.8/stochvolmodels/pricers/core/mgf_pricer.py
--rw-r--r--   0        0        0    12426 2023-02-11 21:27:16.000000 stochvolmodels-1.0.8/stochvolmodels/pricers/core/normal_pricer.py
--rw-r--r--   0        0        0    40945 2023-12-05 14:07:16.474283 stochvolmodels-1.0.8/stochvolmodels/pricers/hawkes_jd_pricer.py
--rw-r--r--   0        0        0    18585 2023-12-05 14:07:16.446238 stochvolmodels-1.0.8/stochvolmodels/pricers/heston_pricer.py
--rw-r--r--   0        0        0        0 2022-02-14 15:41:19.000000 stochvolmodels-1.0.8/stochvolmodels/pricers/logsv/__init__.py
--rw-r--r--   0        0        0    19351 2022-08-10 06:02:37.000000 stochvolmodels-1.0.8/stochvolmodels/pricers/logsv/affine_expansion.py
--rw-r--r--   0        0        0     7368 2022-08-10 06:02:37.000000 stochvolmodels-1.0.8/stochvolmodels/pricers/logsv/vol_moments_ode.py
--rw-r--r--   0        0        0    39163 2023-12-06 15:08:07.492598 stochvolmodels-1.0.8/stochvolmodels/pricers/logsv_pricer.py
--rw-r--r--   0        0        0    26446 2023-02-11 10:25:50.000000 stochvolmodels-1.0.8/stochvolmodels/pricers/model_pricer.py
--rw-r--r--   0        0        0        0 2022-08-10 05:05:50.000000 stochvolmodels-1.0.8/stochvolmodels/tests/__init__.py
--rw-r--r--   0        0        0     7510 2023-12-05 14:07:16.498959 stochvolmodels-1.0.8/stochvolmodels/tests/bsm_mgf_pricer.py
--rw-r--r--   0        0        0     5004 2022-08-10 07:03:07.000000 stochvolmodels-1.0.8/stochvolmodels/tests/qv_pricer.py
--rw-r--r--   0        0        0        0 2021-09-23 21:21:24.000000 stochvolmodels-1.0.8/stochvolmodels/utils/__init__.py
--rw-r--r--   0        0        0     2991 2023-11-21 19:13:45.000000 stochvolmodels-1.0.8/stochvolmodels/utils/funcs.py
--rw-r--r--   0        0        0    15274 2023-02-10 09:36:46.000000 stochvolmodels-1.0.8/stochvolmodels/utils/plots.py
--rw-r--r--   0        0        0     9984 1970-01-01 00:00:00.000000 stochvolmodels-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35802 2022-08-10 05:48:35.968019 stochvolmodels-1.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     1594 2023-12-06 19:53:46.095894 stochvolmodels-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     8540 2023-12-03 17:09:02.327163 stochvolmodels-1.0.9/README.md
+-rw-r--r--   0        0        0     3345 2023-12-06 14:45:26.000000 stochvolmodels-1.0.9/stochvolmodels/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-08 12:33:11.995884 stochvolmodels-1.0.9/stochvolmodels/data/__init__.py
+-rw-r--r--   0        0        0    13285 2023-12-05 15:25:41.000000 stochvolmodels-1.0.9/stochvolmodels/data/option_chain.py
+-rw-r--r--   0        0        0    63709 2023-11-26 10:08:33.131673 stochvolmodels-1.0.9/stochvolmodels/data/test_option_chain.py
+-rw-r--r--   0        0        0        0 2023-12-05 14:56:51.000000 stochvolmodels-1.0.9/stochvolmodels/pricers/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-06 06:57:02.689634 stochvolmodels-1.0.9/stochvolmodels/pricers/core/__init__.py
+-rw-r--r--   0        0        0    11381 2023-02-26 07:20:57.147315 stochvolmodels-1.0.9/stochvolmodels/pricers/core/bsm_pricer.py
+-rw-r--r--   0        0        0      264 2022-08-09 14:55:12.495917 stochvolmodels-1.0.9/stochvolmodels/pricers/core/config.py
+-rw-r--r--   0        0        0     1963 2022-11-11 09:13:29.000000 stochvolmodels-1.0.9/stochvolmodels/pricers/core/mc_payoffs.py
+-rw-r--r--   0        0        0    13140 2023-12-05 14:29:14.000000 stochvolmodels-1.0.9/stochvolmodels/pricers/core/mgf_pricer.py
+-rw-r--r--   0        0        0    12426 2023-02-11 21:27:16.000000 stochvolmodels-1.0.9/stochvolmodels/pricers/core/normal_pricer.py
+-rw-r--r--   0        0        0    40945 2023-12-05 14:07:16.000000 stochvolmodels-1.0.9/stochvolmodels/pricers/hawkes_jd_pricer.py
+-rw-r--r--   0        0        0    18585 2023-12-05 14:07:16.000000 stochvolmodels-1.0.9/stochvolmodels/pricers/heston_pricer.py
+-rw-r--r--   0        0        0        0 2022-02-14 15:41:19.145907 stochvolmodels-1.0.9/stochvolmodels/pricers/logsv/__init__.py
+-rw-r--r--   0        0        0    19351 2022-08-10 06:02:37.646870 stochvolmodels-1.0.9/stochvolmodels/pricers/logsv/affine_expansion.py
+-rw-r--r--   0        0        0     7368 2022-08-10 06:02:37.807658 stochvolmodels-1.0.9/stochvolmodels/pricers/logsv/vol_moments_ode.py
+-rw-r--r--   0        0        0    39626 2023-12-06 15:44:10.000000 stochvolmodels-1.0.9/stochvolmodels/pricers/logsv_pricer.py
+-rw-r--r--   0        0        0    26451 2023-12-06 19:53:31.526669 stochvolmodels-1.0.9/stochvolmodels/pricers/model_pricer.py
+-rw-r--r--   0        0        0        0 2022-08-10 05:05:50.154058 stochvolmodels-1.0.9/stochvolmodels/tests/__init__.py
+-rw-r--r--   0        0        0     7510 2023-12-05 14:07:16.000000 stochvolmodels-1.0.9/stochvolmodels/tests/bsm_mgf_pricer.py
+-rw-r--r--   0        0        0     5004 2022-08-10 07:03:07.372775 stochvolmodels-1.0.9/stochvolmodels/tests/qv_pricer.py
+-rw-r--r--   0        0        0        0 2021-09-23 21:21:24.480697 stochvolmodels-1.0.9/stochvolmodels/utils/__init__.py
+-rw-r--r--   0        0        0     2991 2023-11-21 19:13:45.543605 stochvolmodels-1.0.9/stochvolmodels/utils/funcs.py
+-rw-r--r--   0        0        0    15274 2023-02-10 09:36:46.546682 stochvolmodels-1.0.9/stochvolmodels/utils/plots.py
+-rw-r--r--   0        0        0     9984 1970-01-01 00:00:00.000000 stochvolmodels-1.0.9/PKG-INFO
```

### Comparing `stochvolmodels-1.0.8/LICENSE.txt` & `stochvolmodels-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stochvolmodels-1.0.8/pyproject.toml` & `stochvolmodels-1.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2273 746f 6368 766f 6c6d  ame = "stochvolm
 00000020: 6f64 656c 7322 0d0a 7665 7273 696f 6e20  odels"..version 
-00000030: 3d20 2231 2e30 2e38 220d 0a64 6573 6372  = "1.0.8"..descr
+00000030: 3d20 2231 2e30 2e39 220d 0a64 6573 6372  = "1.0.9"..descr
 00000040: 6970 7469 6f6e 203d 2022 496d 706c 656d  iption = "Implem
 00000050: 656e 7461 7469 6f6e 206f 6620 7374 6f63  entation of stoc
 00000060: 6861 7374 6963 2076 6f6c 6174 696c 6974  hastic volatilit
 00000070: 7920 6d6f 6465 6c73 2066 6f72 206f 7074  y models for opt
 00000080: 696f 6e20 7072 6963 696e 6722 0d0a 6c69  ion pricing"..li
 00000090: 6365 6e73 6520 3d20 224c 4943 454e 5345  cense = "LICENSE
 000000a0: 2e74 7874 220d 0a61 7574 686f 7273 203d  .txt"..authors =
```

### Comparing `stochvolmodels-1.0.8/README.md` & `stochvolmodels-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `stochvolmodels-1.0.8/stochvolmodels/__init__.py` & `stochvolmodels-1.0.9/stochvolmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `stochvolmodels-1.0.8/stochvolmodels/data/option_chain.py` & `stochvolmodels-1.0.9/stochvolmodels/data/option_chain.py`

 * *Files identical despite different names*

### Comparing `stochvolmodels-1.0.8/stochvolmodels/data/test_option_chain.py` & `stochvolmodels-1.0.9/stochvolmodels/data/test_option_chain.py`

 * *Files identical despite different names*

### Comparing `stochvolmodels-1.0.8/stochvolmodels/pricers/core/bsm_pricer.py` & `stochvolmodels-1.0.9/stochvolmodels/pricers/core/bsm_pricer.py`

 * *Files identical despite different names*

### Comparing `stochvolmodels-1.0.8/stochvolmodels/pricers/core/mc_payoffs.py` & `stochvolmodels-1.0.9/stochvolmodels/pricers/core/mc_payoffs.py`

 * *Files identical despite different names*

### Comparing `stochvolmodels-1.0.8/stochvolmodels/pricers/core/mgf_pricer.py` & `stochvolmodels-1.0.9/stochvolmodels/pricers/core/mgf_pricer.py`

 * *Files identical despite different names*

### Comparing `stochvolmodels-1.0.8/stochvolmodels/pricers/core/normal_pricer.py` & `stochvolmodels-1.0.9/stochvolmodels/pricers/core/normal_pricer.py`

 * *Files identical despite different names*

### Comparing `stochvolmodels-1.0.8/stochvolmodels/pricers/hawkes_jd_pricer.py` & `stochvolmodels-1.0.9/stochvolmodels/pricers/hawkes_jd_pricer.py`

 * *Files identical despite different names*

### Comparing `stochvolmodels-1.0.8/stochvolmodels/pricers/heston_pricer.py` & `stochvolmodels-1.0.9/stochvolmodels/pricers/heston_pricer.py`

 * *Files identical despite different names*

### Comparing `stochvolmodels-1.0.8/stochvolmodels/pricers/logsv/affine_expansion.py` & `stochvolmodels-1.0.9/stochvolmodels/pricers/logsv/affine_expansion.py`

 * *Files identical despite different names*

### Comparing `stochvolmodels-1.0.8/stochvolmodels/pricers/logsv/vol_moments_ode.py` & `stochvolmodels-1.0.9/stochvolmodels/pricers/logsv/vol_moments_ode.py`

 * *Files identical despite different names*

### Comparing `stochvolmodels-1.0.8/stochvolmodels/pricers/logsv_pricer.py` & `stochvolmodels-1.0.9/stochvolmodels/pricers/logsv_pricer.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,16 @@
                                      nb_path=nb_path,
                                      **kwargs)
 
     @timer
     def calibrate_model_params_to_chain(self,
                                         option_chain: OptionChain,
                                         params0: LogSvParams,
+                                        params_min: LogSvParams = LogSvParams(sigma0=0.1, theta=0.1, kappa1=0.25, kappa2=0.25, beta=-3.0, volvol=0.2),
+                                        params_max: LogSvParams = LogSvParams(sigma0=1.5, theta=1.5, kappa1=10.0, kappa2=10.0, beta=3.0, volvol=3.0),
                                         is_vega_weighted: bool = True,
                                         is_unit_ttm_vega: bool = False,
                                         model_calibration_type: LogsvModelCalibrationType = LogsvModelCalibrationType.PARAMS5,
                                         constraints_type: ConstraintsType = ConstraintsType.UNCONSTRAINT,
                                         **kwargs
                                         ) -> LogSvParams:
         """
@@ -245,19 +247,19 @@
             weights = to_flat_np_array(vegas_ttms)
         else:
             weights = np.ones_like(market_vols)
 
         # implement different calibrato types
         if model_calibration_type == LogsvModelCalibrationType.PARAMS4:
             # fit: v0, theta, beta, volvol; kappa1, kappa2 is given with params0
-            if params0 is not None:
-                p0 = np.array([params0.sigma0, params0.theta, params0.beta, params0.volvol])
-            else:
-                p0 = np.array([0.8, 0.8, -0.2, 2.0])
-            bounds = ((0.01, 2.0), (0.01, 2.0), (-5.0, 3.0), (0.1, 10.0))
+            p0 = np.array([params0.sigma0, params0.theta, params0.beta, params0.volvol])
+            bounds = ((params_min.sigma0, params_max.sigma0),
+                      (params_min.theta, params_max.theta),
+                      (params_min.beta, params_max.beta),
+                      (params_min.volvol, params_max.volvol))
 
             def objective(pars: np.ndarray, args: np.ndarray) -> float:
                 v0, theta, beta, volvol = pars[0], pars[1], pars[2], pars[3]
                 params = LogSvParams(sigma0=v0, theta=theta, kappa1=params0.kappa1,
                                      kappa2=params0.kappa2, beta=beta, volvol=volvol)
                 model_vols = self.compute_model_ivols_for_chain(option_chain=option_chain, params=params,
                                                                 vol_scaler=vol_scaler)
@@ -276,19 +278,20 @@
                 v0, theta, beta, volvol = pars[0], pars[1], pars[2], pars[3]
                 vartheta2 = beta * beta + volvol * volvol
                 kappa = params0.kappa1 + params0.kappa2 * theta
                 return kappa - 1.5 * vartheta2
 
         elif model_calibration_type == LogsvModelCalibrationType.PARAMS5:
             # fit: v0, theta, kappa1, beta, volvol; kappa2 is mapped as kappa1 / theta
-            if params0 is not None:
-                p0 = np.array([params0.sigma0, params0.theta, params0.kappa1, params0.beta, params0.volvol])
-            else:
-                p0 = np.array([0.8, 0.8, 4.0, -0.2, 2.0])
-            bounds = ((0.01, 2.0), (0.01, 2.0), (0.5, 7.0), (-5.0, 3.0), (0.1, 10.0))
+            p0 = np.array([params0.sigma0, params0.theta, params0.kappa1, params0.beta, params0.volvol])
+            bounds = ((params_min.sigma0, params_max.sigma0),
+                      (params_min.theta, params_max.theta),
+                      (params_min.kappa1, params_max.kappa1),
+                      (params_min.beta, params_max.beta),
+                      (params_min.volvol, params_max.volvol))
 
             def objective(pars: np.ndarray, args: np.ndarray) -> float:
                 v0, theta, kappa1, beta, volvol = pars[0], pars[1], pars[2], pars[3], pars[4]
                 params = LogSvParams(sigma0=v0, theta=theta, kappa1=kappa1, kappa2=None, beta=beta, volvol=volvol)
                 model_vols = self.compute_model_ivols_for_chain(option_chain=option_chain, params=params, vol_scaler=vol_scaler)
                 resid = np.nansum(weights * np.square(to_flat_np_array(model_vols) - market_vols))
                 return resid
```

### Comparing `stochvolmodels-1.0.8/stochvolmodels/pricers/model_pricer.py` & `stochvolmodels-1.0.9/stochvolmodels/pricers/model_pricer.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,15 @@
             with sns.axes_style('darkgrid'):
                 fig, ax = plt.subplots(1, 1, figsize=plot.FIGSIZE, tight_layout=True)
             axs = np.array([[ax, np.nan], [np.nan, np.nan]])
         elif num_slices == 2:
             with sns.axes_style('darkgrid'):
                 fig, axs = plt.subplots(2, 1, figsize=plot.FIGSIZE, tight_layout=True)
             axs = np.array([[axs[0], np.nan], [axs[1], np.nan]])
-        elif num_slices == 4:
+        elif num_slices in [3, 4]:
             with sns.axes_style('darkgrid'):
                 fig, axs = plt.subplots(2, 2, figsize=plot.FIGSIZE, tight_layout=True)
         else:
             raise NotImplementedError
 
         atm_vols = option_chain.get_chain_atm_vols()
         for idx, ttm in enumerate(option_chain.ttms):
```

### Comparing `stochvolmodels-1.0.8/stochvolmodels/tests/bsm_mgf_pricer.py` & `stochvolmodels-1.0.9/stochvolmodels/tests/bsm_mgf_pricer.py`

 * *Files identical despite different names*

### Comparing `stochvolmodels-1.0.8/stochvolmodels/tests/qv_pricer.py` & `stochvolmodels-1.0.9/stochvolmodels/tests/qv_pricer.py`

 * *Files identical despite different names*

### Comparing `stochvolmodels-1.0.8/stochvolmodels/utils/funcs.py` & `stochvolmodels-1.0.9/stochvolmodels/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `stochvolmodels-1.0.8/stochvolmodels/utils/plots.py` & `stochvolmodels-1.0.9/stochvolmodels/utils/plots.py`

 * *Files identical despite different names*

### Comparing `stochvolmodels-1.0.8/PKG-INFO` & `stochvolmodels-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stochvolmodels
-Version: 1.0.8
+Version: 1.0.9
 Summary: Implementation of stochastic volatility models for option pricing
 Home-page: https://github.com/ArturSepp/StochVolModels
 License: LICENSE.txt
 Keywords: volatility,options,Black-Scholes,Heston,Monte-Carlo
 Author: Artur Sepp
 Author-email: artursepp@gmail.com
 Maintainer: Artur Sepp
```

