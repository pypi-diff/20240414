# Comparing `tmp/pycvodes-0.9.1.tar.gz` & `tmp/pycvodes-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycvodes-0.9.1.tar", last modified: Tue Dec 19 17:43:10 2017, max compression
+gzip compressed data, was "dist/pycvodes-0.9.2.tar", last modified: Tue Feb  6 15:24:07 2018, max compression
```

## Comparing `pycvodes-0.9.1.tar` & `pycvodes-0.9.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2017-12-19 17:43:10.000000 pycvodes-0.9.1/
--rw-rw-r--   0 bjorn      (528) bjorn      (528)       38 2017-09-15 10:03:42.000000 pycvodes-0.9.1/AUTHORS
--rw-rw-r--   0 bjorn      (528) bjorn      (528)      126 2017-09-15 10:03:42.000000 pycvodes-0.9.1/MANIFEST.in
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     3246 2017-12-19 17:37:13.000000 pycvodes-0.9.1/CHANGES.rst
-drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2017-12-19 17:43:10.000000 pycvodes-0.9.1/external/
-drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2017-12-19 17:43:10.000000 pycvodes-0.9.1/external/anyode/
-drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2017-12-19 17:43:10.000000 pycvodes-0.9.1/external/anyode/cython_def/
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     1079 2017-10-02 21:23:20.000000 pycvodes-0.9.1/external/anyode/cython_def/anyode_numpy.pxd
--rw-rw-r--   0 bjorn      (528) bjorn      (528)      209 2017-09-15 10:03:42.000000 pycvodes-0.9.1/external/anyode/cython_def/anyode.pxd
-drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2017-12-19 17:43:10.000000 pycvodes-0.9.1/external/anyode/include/
-drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2017-12-19 17:43:10.000000 pycvodes-0.9.1/external/anyode/include/anyode/
--rw-rw-r--   0 bjorn      (528) bjorn      (528)      820 2017-09-15 10:03:42.000000 pycvodes-0.9.1/external/anyode/include/anyode/anyode_buffer.hpp
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     5266 2017-09-15 10:03:42.000000 pycvodes-0.9.1/external/anyode/include/anyode/anyode_decomposition.hpp
--rw-rw-r--   0 bjorn      (528) bjorn      (528)    12270 2017-09-15 10:03:42.000000 pycvodes-0.9.1/external/anyode/include/anyode/anyode_numpy.hpp
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     5867 2017-10-02 21:23:20.000000 pycvodes-0.9.1/external/anyode/include/anyode/anyode.hpp
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     3971 2017-09-15 10:03:42.000000 pycvodes-0.9.1/external/anyode/include/anyode/anyode_iterative.hpp
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     4117 2017-09-15 10:03:42.000000 pycvodes-0.9.1/external/anyode/include/anyode/anyode_blas_lapack.hpp
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     7497 2017-09-15 10:03:42.000000 pycvodes-0.9.1/external/anyode/include/anyode/anyode_matrix.hpp
--rw-rw-r--   0 bjorn      (528) bjorn      (528)      738 2017-09-15 10:03:42.000000 pycvodes-0.9.1/external/anyode/include/anyode/anyode_parallel.hpp
-drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2017-12-19 17:43:10.000000 pycvodes-0.9.1/pycvodes.egg-info/
--rw-rw-r--   0 bjorn      (528) bjorn      (528)        1 2017-12-19 17:43:10.000000 pycvodes-0.9.1/pycvodes.egg-info/dependency_links.txt
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     1172 2017-12-19 17:43:10.000000 pycvodes-0.9.1/pycvodes.egg-info/SOURCES.txt
--rw-rw-r--   0 bjorn      (528) bjorn      (528)        9 2017-12-19 17:43:10.000000 pycvodes-0.9.1/pycvodes.egg-info/top_level.txt
--rw-rw-r--   0 bjorn      (528) bjorn      (528)       54 2017-12-19 17:43:10.000000 pycvodes-0.9.1/pycvodes.egg-info/requires.txt
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     5690 2017-12-19 17:43:10.000000 pycvodes-0.9.1/pycvodes.egg-info/PKG-INFO
--rw-rw-r--   0 bjorn      (528) bjorn      (528)      255 2017-12-19 17:43:10.000000 pycvodes-0.9.1/setup.cfg
--rwxrwxr-x   0 bjorn      (528) bjorn      (528)     5422 2017-09-15 10:03:42.000000 pycvodes-0.9.1/setup.py
-drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2017-12-19 17:43:10.000000 pycvodes-0.9.1/pycvodes/
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     9864 2017-10-02 21:23:20.000000 pycvodes-0.9.1/pycvodes/__init__.py
-drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2017-12-19 17:43:10.000000 pycvodes-0.9.1/pycvodes/tests/
--rw-rw-r--   0 bjorn      (528) bjorn      (528)        0 2017-09-15 10:03:42.000000 pycvodes-0.9.1/pycvodes/tests/__init__.py
--rw-rw-r--   0 bjorn      (528) bjorn      (528)    15097 2017-10-02 21:23:20.000000 pycvodes-0.9.1/pycvodes/tests/test_cvodes_numpy.py
--rw-rw-r--   0 bjorn      (528) bjorn      (528)   623334 2017-12-19 17:43:02.000000 pycvodes-0.9.1/pycvodes/_cvodes.cpp
--rw-rw-r--   0 bjorn      (528) bjorn      (528)       22 2017-12-19 17:43:10.000000 pycvodes-0.9.1/pycvodes/_release.py
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     1596 2017-09-15 10:03:42.000000 pycvodes-0.9.1/pycvodes/_util.py
-drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2017-12-19 17:43:10.000000 pycvodes-0.9.1/pycvodes/include/
--rw-rw-r--   0 bjorn      (528) bjorn      (528)    17851 2017-12-19 17:36:50.000000 pycvodes-0.9.1/pycvodes/include/cvodes_anyode.hpp
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     4987 2017-11-14 12:48:40.000000 pycvodes-0.9.1/pycvodes/include/cvodes_anyode_parallel.hpp
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     1184 2017-10-02 21:23:20.000000 pycvodes-0.9.1/pycvodes/include/cvodes_anyode_parallel.pxd
--rw-rw-r--   0 bjorn      (528) bjorn      (528)      762 2017-09-15 10:03:42.000000 pycvodes-0.9.1/pycvodes/include/cvodes_cxx.pxd
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     1134 2017-12-19 17:36:50.000000 pycvodes-0.9.1/pycvodes/include/cvodes_anyode.pxd
--rw-rw-r--   0 bjorn      (528) bjorn      (528)    32546 2017-10-02 21:23:20.000000 pycvodes-0.9.1/pycvodes/include/cvodes_cxx.hpp
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     1178 2017-09-15 10:03:42.000000 pycvodes-0.9.1/pycvodes/include/cvodes_anyode_nogil.pxd
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     3392 2017-09-15 10:03:42.000000 pycvodes-0.9.1/pycvodes/include/sundials_cxx.hpp
--rw-rw-r--   0 bjorn      (528) bjorn      (528)       85 2017-12-19 17:43:10.000000 pycvodes-0.9.1/pycvodes/_config.py
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     5690 2017-12-19 17:43:10.000000 pycvodes-0.9.1/PKG-INFO
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     4221 2017-09-15 10:03:42.000000 pycvodes-0.9.1/README.rst
--rw-rw-r--   0 bjorn      (528) bjorn      (528)     1303 2017-09-15 10:03:42.000000 pycvodes-0.9.1/LICENSE
+drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2018-02-06 15:24:07.000000 pycvodes-0.9.2/
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)       38 2017-12-19 17:44:45.000000 pycvodes-0.9.2/AUTHORS
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      126 2017-12-19 17:44:45.000000 pycvodes-0.9.2/MANIFEST.in
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     3283 2018-02-06 15:21:48.000000 pycvodes-0.9.2/CHANGES.rst
+drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2018-02-06 15:24:07.000000 pycvodes-0.9.2/external/
+drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2018-02-06 15:24:07.000000 pycvodes-0.9.2/external/anyode/
+drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2018-02-06 15:24:07.000000 pycvodes-0.9.2/external/anyode/cython_def/
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     1079 2017-12-19 17:44:45.000000 pycvodes-0.9.2/external/anyode/cython_def/anyode_numpy.pxd
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      209 2017-12-19 17:44:45.000000 pycvodes-0.9.2/external/anyode/cython_def/anyode.pxd
+drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2018-02-06 15:24:07.000000 pycvodes-0.9.2/external/anyode/include/
+drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2018-02-06 15:24:07.000000 pycvodes-0.9.2/external/anyode/include/anyode/
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      820 2018-02-06 15:20:54.000000 pycvodes-0.9.2/external/anyode/include/anyode/anyode_buffer.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     5266 2018-02-06 15:20:54.000000 pycvodes-0.9.2/external/anyode/include/anyode/anyode_decomposition.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)    12270 2018-02-06 15:20:54.000000 pycvodes-0.9.2/external/anyode/include/anyode/anyode_numpy.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     5903 2018-02-06 15:20:54.000000 pycvodes-0.9.2/external/anyode/include/anyode/anyode.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     3928 2018-02-06 15:20:54.000000 pycvodes-0.9.2/external/anyode/include/anyode/anyode_iterative.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     4117 2018-02-06 15:20:54.000000 pycvodes-0.9.2/external/anyode/include/anyode/anyode_blas_lapack.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     7497 2018-02-06 15:20:54.000000 pycvodes-0.9.2/external/anyode/include/anyode/anyode_matrix.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      738 2018-02-06 15:20:54.000000 pycvodes-0.9.2/external/anyode/include/anyode/anyode_parallel.hpp
+drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2018-02-06 15:24:07.000000 pycvodes-0.9.2/pycvodes.egg-info/
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)        1 2018-02-06 15:24:07.000000 pycvodes-0.9.2/pycvodes.egg-info/dependency_links.txt
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     1172 2018-02-06 15:24:07.000000 pycvodes-0.9.2/pycvodes.egg-info/SOURCES.txt
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)        9 2018-02-06 15:24:07.000000 pycvodes-0.9.2/pycvodes.egg-info/top_level.txt
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)       54 2018-02-06 15:24:07.000000 pycvodes-0.9.2/pycvodes.egg-info/requires.txt
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     6537 2018-02-06 15:24:07.000000 pycvodes-0.9.2/pycvodes.egg-info/PKG-INFO
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      255 2018-02-06 15:24:07.000000 pycvodes-0.9.2/setup.cfg
+-rwxrwxr-x   0 bjorn      (528) bjorn      (528)     5499 2017-12-30 17:10:13.000000 pycvodes-0.9.2/setup.py
+drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2018-02-06 15:24:07.000000 pycvodes-0.9.2/pycvodes/
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     9864 2017-12-19 17:44:45.000000 pycvodes-0.9.2/pycvodes/__init__.py
+drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2018-02-06 15:24:07.000000 pycvodes-0.9.2/pycvodes/tests/
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)        0 2017-12-19 17:44:45.000000 pycvodes-0.9.2/pycvodes/tests/__init__.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)    15097 2017-12-19 17:44:45.000000 pycvodes-0.9.2/pycvodes/tests/test_cvodes_numpy.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)   642354 2018-02-06 15:22:52.000000 pycvodes-0.9.2/pycvodes/_cvodes.cpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)       22 2018-02-06 15:24:07.000000 pycvodes-0.9.2/pycvodes/_release.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     1596 2017-12-19 17:44:45.000000 pycvodes-0.9.2/pycvodes/_util.py
+drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2018-02-06 15:24:07.000000 pycvodes-0.9.2/pycvodes/include/
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)    19030 2018-01-31 14:41:47.000000 pycvodes-0.9.2/pycvodes/include/cvodes_anyode.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     4987 2017-12-19 17:44:45.000000 pycvodes-0.9.2/pycvodes/include/cvodes_anyode_parallel.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     1184 2017-12-19 17:44:45.000000 pycvodes-0.9.2/pycvodes/include/cvodes_anyode_parallel.pxd
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      762 2017-12-19 17:44:45.000000 pycvodes-0.9.2/pycvodes/include/cvodes_cxx.pxd
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     1134 2017-12-19 17:44:45.000000 pycvodes-0.9.2/pycvodes/include/cvodes_anyode.pxd
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)    38745 2017-12-30 17:10:13.000000 pycvodes-0.9.2/pycvodes/include/cvodes_cxx.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     1178 2017-12-19 17:44:45.000000 pycvodes-0.9.2/pycvodes/include/cvodes_anyode_nogil.pxd
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     3392 2017-12-19 17:44:45.000000 pycvodes-0.9.2/pycvodes/include/sundials_cxx.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)       89 2018-02-06 15:24:07.000000 pycvodes-0.9.2/pycvodes/_config.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     6537 2018-02-06 15:24:07.000000 pycvodes-0.9.2/PKG-INFO
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     4964 2018-01-26 16:55:53.000000 pycvodes-0.9.2/README.rst
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     1303 2017-12-19 17:44:45.000000 pycvodes-0.9.2/LICENSE
```

### Comparing `pycvodes-0.9.1/CHANGES.rst` & `pycvodes-0.9.2/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+v0.9.2
+======
+- Bump AnyODE version
+
 v0.9.1
 ======
 - variable tidx exposed in simple_adaptive
 
 v0.9.0
 ======
 - adaptive integration now reallocs its own space (allows direct transfer of ownership to e.g. numpy arrays)
```

### Comparing `pycvodes-0.9.1/external/anyode/cython_def/anyode_numpy.pxd` & `pycvodes-0.9.2/external/anyode/cython_def/anyode_numpy.pxd`

 * *Files identical despite different names*

### Comparing `pycvodes-0.9.1/external/anyode/include/anyode/anyode_buffer.hpp` & `pycvodes-0.9.2/external/anyode/include/anyode/anyode_buffer.hpp`

 * *Files identical despite different names*

### Comparing `pycvodes-0.9.1/external/anyode/include/anyode/anyode_decomposition.hpp` & `pycvodes-0.9.2/external/anyode/include/anyode/anyode_decomposition.hpp`

 * *Files identical despite different names*

### Comparing `pycvodes-0.9.1/external/anyode/include/anyode/anyode_numpy.hpp` & `pycvodes-0.9.2/external/anyode/include/anyode/anyode_numpy.hpp`

 * *Files identical despite different names*

### Comparing `pycvodes-0.9.1/external/anyode/include/anyode/anyode.hpp` & `pycvodes-0.9.2/external/anyode/include/anyode/anyode.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #ifdef ANYODE_HPP_D47BAD58870311E6B95F2F58DEFE6E37
 
-#if ANYODE_HPP_D47BAD58870311E6B95F2F58DEFE6E37 != 10
+#if ANYODE_HPP_D47BAD58870311E6B95F2F58DEFE6E37 != 11
 #error "Multiple anyode.hpp files included with version mismatch"
 #endif
 
 #else
-#define ANYODE_HPP_D47BAD58870311E6B95F2F58DEFE6E37 10
+#define ANYODE_HPP_D47BAD58870311E6B95F2F58DEFE6E37 11
 
 
 #include <string>
 #include <unordered_map>
 #include <vector>
 
 namespace AnyODE {
@@ -17,14 +17,15 @@
 
     enum class Status : int {success = 0, recoverable_error = 1, unrecoverable_error = -1};
 
     template <typename Real_t=double>
     struct OdeSysBase {
         int nfev=0, njev=0;
         void * integrator = nullptr;
+        void * user_data = nullptr;
         std::unordered_map<std::string, int> last_integration_info;
         std::unordered_map<std::string, double> last_integration_info_dbl;
         std::unordered_map<std::string, std::vector<double> > last_integration_info_vecdbl;
         std::unordered_map<std::string, std::vector<int> > last_integration_info_vecint;
         Real_t default_dx0 = 0.0;  // *may* be used by `get_dx0`, 0 signifies solver default
         bool autonomous_exprs = false;
         bool use_get_dx_max = false;  // whether get_dx_max should be called
```

### Comparing `pycvodes-0.9.1/external/anyode/include/anyode/anyode_iterative.hpp` & `pycvodes-0.9.2/external/anyode/include/anyode/anyode_iterative.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
                                        Real_t /* gamma */,
                                        Real_t /* delta */,
                                        const Real_t * const __restrict__ ewt
                                        ) override
         {
             // See 4.6.9 on page 75 in cvs_guide.pdf (Sundials 2.6.2)
             // Solves P*z = r, where P ~= I - gamma*J
-            const int ny = this->get_ny();
             if (ewt)
                 throw std::runtime_error("Not implemented.");
             m_nprec_solve++;
 
             ignore(t); ignore(fy); ignore(y);
             int info = m_decomp_cache->solve(r, z);
             if (info == 0)
```

### Comparing `pycvodes-0.9.1/external/anyode/include/anyode/anyode_blas_lapack.hpp` & `pycvodes-0.9.2/external/anyode/include/anyode/anyode_blas_lapack.hpp`

 * *Files identical despite different names*

### Comparing `pycvodes-0.9.1/external/anyode/include/anyode/anyode_matrix.hpp` & `pycvodes-0.9.2/external/anyode/include/anyode/anyode_matrix.hpp`

 * *Files identical despite different names*

### Comparing `pycvodes-0.9.1/external/anyode/include/anyode/anyode_parallel.hpp` & `pycvodes-0.9.2/external/anyode/include/anyode/anyode_parallel.hpp`

 * *Files identical despite different names*

### Comparing `pycvodes-0.9.1/pycvodes.egg-info/SOURCES.txt` & `pycvodes-0.9.2/pycvodes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycvodes-0.9.1/pycvodes.egg-info/PKG-INFO` & `pycvodes-0.9.2/pycvodes.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 1.1
 Name: pycvodes
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python binding for cvodes from the sundials library.
 Home-page: https://github.com/bjodah/pycvodes
 Author: Bjoern I. Dahlgren
 Author-email: bjodah@gmail.com
 License: BSD
 Description-Content-Type: UNKNOWN
 Description: pycvodes
         ========
         
         .. image:: http://hera.physchem.kth.se:9090/api/badges/bjodah/pycvodes/status.svg
            :target: http://hera.physchem.kth.se:9090/bjodah/pycvodes
-           :alt: Build status
+           :alt: Build status on private Drone server
+        .. image:: https://circleci.com/gh/bjodah/pycvodes.svg?style=svg
+           :target: https://circleci.com/gh/bjodah/pycvodes
+           :alt: Build status on CircleCI
+        .. image:: https://secure.travis-ci.org/bjodah/pycvodes.svg?branch=master
+           :target: http://travis-ci.org/bjodah/pycvodes
+           :alt: Build status on Travis-CI
         .. image:: https://img.shields.io/pypi/v/pycvodes.svg
            :target: https://pypi.python.org/pypi/pycvodes
            :alt: PyPI version
         .. image:: https://img.shields.io/pypi/l/pycvodes.svg
            :target: https://github.com/bjodah/pycvodes/blob/master/LICENSE
            :alt: License
         .. image:: http://hera.physchem.kth.se/~pycvodes/branches/master/htmlcov/coverage.svg
@@ -25,26 +31,31 @@
         .. image:: https://zenodo.org/badge/43224425.svg
            :target: https://zenodo.org/badge/latestdoi/43224425
         
         `pycvodes <https://github.com/bjodah/pycvodes>`_ provides a
         `Python <http://www.python.org>`_ binding to the
         `Ordinary Differential Equation <https://en.wikipedia.org/wiki/Ordinary_differential_equation>`_
         integration routines from `cvodes <https://computation.llnl.gov/casc/sundials/description/description.html#descr_cvodes>`_ in the
-        `SUNDIALS suite <https://computation.llnl.gov/casc/sundials/main.html>`_. ``pcyvodes`` allows a user to numerically integrate
+        `SUNDIALS suite <https://computation.llnl.gov/casc/sundials/main.html>`_. ``pycvodes`` allows a user to numerically integrate
         (systems of) differential equations. Note that routines for sensitivity analysis is not yet exposed in this binding (which makes
         the functionality essentially the same as cvode). 
         
         The following multistep methods are available:
         
         - ``bdf``: Backward differentiation formula (of order 1 to 5)
         - ``adams``: implicit Adams method (order 1 to 12)
         
         Note that bdf (as an implicit stepper) requires a user supplied
         callback for calculating the jacobian.
         
+        You may also want to know that you can use ``pycvodes`` from
+        `pyodesys <https://github.com/bjodah/pyodesys>`_
+        which can e.g. derive the Jacobian analytically for you (pyodesys also provides
+        plotting functions, C++ code-generation and more).
+        
         Documentation
         -------------
         Autogenerated API documentation for latest stable release is found here:
         `<https://bjodah.github.io/pycvodes/latest>`_
         (and the development version for the current master branch are found here:
         `<http://hera.physchem.kth.se/~pycvodes/branches/master/html>`_).
         
@@ -70,14 +81,16 @@
         
         .. code:: python
         
            >>> from pycvodes import _config
            >>> _config.env['LAPACK']  # doctest: +SKIP
            'lapack,blas'
         
+        If you use ``pip`` to install ``pycvodes`` note that you will need to install sundials
+        (and its development headers, with cvodes enabled) prior to installing pycvodes.
         
         Examples
         --------
         The classic van der Pol oscillator (see `examples/van_der_pol.py <examples/van_der_pol.py>`_)
         
         .. code:: python
```

### Comparing `pycvodes-0.9.1/setup.py` & `pycvodes-0.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,29 +21,30 @@
 
 
 def _path_under_setup(*args):
     return os.path.join(os.path.dirname(__file__), *args)
 
 release_py_path = _path_under_setup(pkg_name, '_release.py')
 config_py_path = _path_under_setup(pkg_name, '_config.py')
-env = None  # silence pyflakes, 'env' is actually set on the next line
-exec(open(config_py_path).read())
-for k, v in list(env.items()):
-    env[k] = os.environ.get('%s_%s' % (pkg_name.upper(), k), v)
 
 
 USE_CYTHON = os.path.exists(_path_under_setup(pkg_name, '_cvodes.pyx'))
 package_include = os.path.join(pkg_name, 'include')
 
 # Cythonize .pyx file if it exists (not in source distribution)
 ext_modules = []
 
 if len(sys.argv) > 1 and '--help' not in sys.argv[1:] and sys.argv[1] not in (
         '--help-commands', 'egg_info', 'clean', '--version'):
     import numpy as np
+    env = None  # silence pyflakes, 'env' is actually set on the next line
+    exec(open(config_py_path).read())
+    for k, v in list(env.items()):
+        env[k] = os.environ.get('%s_%s' % (pkg_name.upper(), k), v)
+
     ext = '.pyx' if USE_CYTHON else '.cpp'
     sources = [os.path.join(pkg_name, '_cvodes'+ext)]
     ext_modules = [Extension('%s._cvodes' % pkg_name, sources)]
     if USE_CYTHON:
         from Cython.Build import cythonize
         ext_modules = cythonize(ext_modules, include_path=[
             package_include,
@@ -132,14 +133,16 @@
         if TAGGED_RELEASE:
             # Same commit should generate different sdist files
             # depending on tagged version (set PYCVODES_RELEASE_VERSION)
             # this will ensure source distributions contain the correct version
             shutil.move(release_py_path, release_py_path+'__temp__')
             open(release_py_path, 'wt').write(
                 "__version__ = '{}'\n".format(__version__))
-        shutil.move(config_py_path, config_py_path+'__temp__')
-        open(config_py_path, 'wt').write("env = {}\n".format(pprint.pformat(env)))
+        if ext_modules:
+            shutil.move(config_py_path, config_py_path+'__temp__')
+            open(config_py_path, 'wt').write("env = {}\n".format(pprint.pformat(env)))
         setup(**setup_kwargs)
     finally:
         if TAGGED_RELEASE:
             shutil.move(release_py_path+'__temp__', release_py_path)
-        shutil.move(config_py_path+'__temp__', config_py_path)
+        if ext_modules:
+            shutil.move(config_py_path+'__temp__', config_py_path)
```

### Comparing `pycvodes-0.9.1/pycvodes/__init__.py` & `pycvodes-0.9.2/pycvodes/__init__.py`

 * *Files identical despite different names*

### Comparing `pycvodes-0.9.1/pycvodes/tests/test_cvodes_numpy.py` & `pycvodes-0.9.2/pycvodes/tests/test_cvodes_numpy.py`

 * *Files identical despite different names*

### Comparing `pycvodes-0.9.1/pycvodes/_cvodes.cpp` & `pycvodes-0.9.2/pycvodes/_cvodes.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-/* Generated by Cython 0.26 */
+/* Generated by Cython 0.27.3 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "pycvodes/include/cvodes_anyode.hpp", 
+            "pycvodes/include/cvodes_anyode.hpp",
             "pycvodes/include/cvodes_cxx.hpp"
-        ], 
+        ],
         "include_dirs": [
             "pycvodes/include"
-        ], 
-        "language": "c++", 
-        "name": "pycvodes._cvodes", 
+        ],
+        "language": "c++",
+        "name": "pycvodes._cvodes",
         "sources": [
             "pycvodes/_cvodes.pyx"
         ]
-    }, 
+    },
     "module_name": "pycvodes._cvodes"
 }
 END: Cython Metadata */
 
 #define PY_SSIZE_T_CLEAN
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
-#elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03020000)
-    #error Cython requires Python 2.6+ or Python 3.2+.
+#elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
+    #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_26"
+#define CYTHON_ABI "0_27_3"
+#define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
@@ -47,15 +48,15 @@
   #define DL_IMPORT(t) t
 #endif
 #ifndef DL_EXPORT
   #define DL_EXPORT(t) t
 #endif
 #define __PYX_COMMA ,
 #ifndef HAVE_LONG_LONG
-  #if PY_VERSION_HEX >= 0x03030000 || (PY_MAJOR_VERSION == 2 && PY_VERSION_HEX >= 0x02070000)
+  #if PY_VERSION_HEX >= 0x02070000
     #define HAVE_LONG_LONG
   #endif
 #endif
 #ifndef PY_LONG_LONG
   #define PY_LONG_LONG LONG_LONG
 #endif
 #ifndef Py_HUGE_VAL
@@ -63,16 +64,22 @@
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
-  #undef CYTHON_USE_ASYNC_SLOTS
-  #define CYTHON_USE_ASYNC_SLOTS 0
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 0
+  #elif !defined(CYTHON_USE_ASYNC_SLOTS)
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #undef CYTHON_USE_UNICODE_INTERNALS
   #define CYTHON_USE_UNICODE_INTERNALS 0
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
   #undef CYTHON_USE_PYLONG_INTERNALS
@@ -83,21 +90,27 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #undef CYTHON_USE_TP_FINALIZE
+  #define CYTHON_USE_TP_FINALIZE 0
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -114,21 +127,31 @@
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #undef CYTHON_USE_TP_FINALIZE
+  #define CYTHON_USE_TP_FINALIZE 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #if PY_VERSION_HEX < 0x02070000
+    #undef CYTHON_USE_PYTYPE_LOOKUP
+    #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
+    #define CYTHON_USE_PYTYPE_LOOKUP 1
+  #endif
   #if PY_MAJOR_VERSION < 3
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
@@ -160,14 +183,20 @@
   #endif
   #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
     #define CYTHON_FAST_PYCALL 1
   #endif
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT (0 && PY_VERSION_HEX >= 0x03050000)
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #include "longintrepr.h"
   #undef SHIFT
@@ -215,14 +244,35 @@
 #endif
 #if CYTHON_FAST_PYCCALL
 #define __Pyx_PyFastCFunction_Check(func)\
     ((PyCFunction_Check(func) && (METH_FASTCALL == (PyCFunction_GET_FLAGS(func) & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS)))))
 #else
 #define __Pyx_PyFastCFunction_Check(func) 0
 #endif
+#if !CYTHON_FAST_THREAD_STATE || PY_VERSION_HEX < 0x02070000
+  #define __Pyx_PyThreadState_Current PyThreadState_GET()
+#elif PY_VERSION_HEX >= 0x03060000
+  #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
+#elif PY_VERSION_HEX >= 0x03000000
+  #define __Pyx_PyThreadState_Current PyThreadState_GET()
+#else
+  #define __Pyx_PyThreadState_Current _PyThreadState_Current
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
+#define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
+#else
+#define __Pyx_PyDict_NewPresized(n)  PyDict_New()
+#endif
+#if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
+  #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
+  #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
+#else
+  #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
+  #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
+#endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
   #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
                                               0 : _PyUnicode_Ready((PyObject *)(op)))
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
@@ -298,15 +348,14 @@
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
 #ifndef PySet_CheckExact
   #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
 #endif
-#define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
   #define PyInt_FromString             PyLong_FromString
@@ -349,23 +398,25 @@
   #define __has_cpp_attribute(x) 0
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
   #else
+    #define __Pyx_PyType_AsAsync(obj) ((__Pyx_PyAsyncMethodsStruct*) (Py_TYPE(obj)->tp_reserved))
+  #endif
+#else
+  #define __Pyx_PyType_AsAsync(obj) NULL
+#endif
+#ifndef __Pyx_PyAsyncMethodsStruct
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
-    #define __Pyx_PyType_AsAsync(obj) ((__Pyx_PyAsyncMethodsStruct*) (Py_TYPE(obj)->tp_reserved))
-  #endif
-#else
-  #define __Pyx_PyType_AsAsync(obj) NULL
 #endif
 #ifndef CYTHON_RESTRICT
   #if defined(__GNUC__)
     #define CYTHON_RESTRICT __restrict__
   #elif defined(_MSC_VER) && _MSC_VER >= 1400
     #define CYTHON_RESTRICT __restrict
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
@@ -412,28 +463,36 @@
            typedef unsigned __int32  uint32_t;
         #endif
     #endif
 #else
    #include <stdint.h>
 #endif
 #ifndef CYTHON_FALLTHROUGH
-  #ifdef __cplusplus
+  #if defined(__cplusplus) && __cplusplus >= 201103L
     #if __has_cpp_attribute(fallthrough)
       #define CYTHON_FALLTHROUGH [[fallthrough]]
     #elif __has_cpp_attribute(clang::fallthrough)
       #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
+    #elif __has_cpp_attribute(gnu::fallthrough)
+      #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
     #endif
   #endif
   #ifndef CYTHON_FALLTHROUGH
-    #if __has_attribute(fallthrough) || (defined(__GNUC__) && defined(__attribute__))
+    #if __has_attribute(fallthrough)
       #define CYTHON_FALLTHROUGH __attribute__((fallthrough))
     #else
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
+  #if defined(__clang__ ) && defined(__apple_build_version__)
+    #if __apple_build_version__ < 7000000
+      #undef  CYTHON_FALLTHROUGH
+      #define CYTHON_FALLTHROUGH
+    #endif
+  #endif
 #endif
 
 #ifndef __cplusplus
   #error "Cython files generated with the C++ option must be compiled with a C++ compiler."
 #endif
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
@@ -481,22 +540,14 @@
 
 
 #define __PYX_ERR(f_index, lineno, Ln_error) \
 { \
   __pyx_filename = __pyx_f[f_index]; __pyx_lineno = lineno; __pyx_clineno = __LINE__; goto Ln_error; \
 }
 
-#if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
-  #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
-#else
-  #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
-  #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
-#endif
-
 #ifndef __PYX_EXTERN_C
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
@@ -519,15 +570,15 @@
 #include "anyode/anyode_numpy.hpp"
 #include "cvodes_cxx.hpp"
 #include "cvodes_anyode.hpp"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
-#ifdef PYREX_WITHOUT_ASSERTIONS
+#if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
 
 typedef struct {PyObject **p; const char *s; const Py_ssize_t n; const char* encoding;
                 const char is_unicode; const char is_str; const char intern; } __Pyx_StringTabEntry;
 
 #define __PYX_DEFAULT_STRING_ENCODING_IS_ASCII 0
@@ -550,16 +601,16 @@
 #if defined (__cplusplus) && __cplusplus >= 201103L
     #include <cstdlib>
     #define __Pyx_sst_abs(value) std::abs(value)
 #elif SIZEOF_INT >= SIZEOF_SIZE_T
     #define __Pyx_sst_abs(value) abs(value)
 #elif SIZEOF_LONG >= SIZEOF_SIZE_T
     #define __Pyx_sst_abs(value) labs(value)
-#elif defined (_MSC_VER) && defined (_M_X64)
-    #define __Pyx_sst_abs(value) _abs64(value)
+#elif defined (_MSC_VER)
+    #define __Pyx_sst_abs(value) ((Py_ssize_t)_abs64(value))
 #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define __Pyx_sst_abs(value) llabs(value)
 #elif defined (__GNUC__)
     #define __Pyx_sst_abs(value) __builtin_llabs(value)
 #else
     #define __Pyx_sst_abs(value) ((value<0) ? -value : value)
 #endif
@@ -573,42 +624,45 @@
 #if PY_MAJOR_VERSION < 3
     #define __Pyx_PyStr_FromString        __Pyx_PyBytes_FromString
     #define __Pyx_PyStr_FromStringAndSize __Pyx_PyBytes_FromStringAndSize
 #else
     #define __Pyx_PyStr_FromString        __Pyx_PyUnicode_FromString
     #define __Pyx_PyStr_FromStringAndSize __Pyx_PyUnicode_FromStringAndSize
 #endif
+#define __Pyx_PyBytes_AsWritableString(s)     ((char*) PyBytes_AS_STRING(s))
+#define __Pyx_PyBytes_AsWritableSString(s)    ((signed char*) PyBytes_AS_STRING(s))
+#define __Pyx_PyBytes_AsWritableUString(s)    ((unsigned char*) PyBytes_AS_STRING(s))
+#define __Pyx_PyBytes_AsString(s)     ((const char*) PyBytes_AS_STRING(s))
+#define __Pyx_PyBytes_AsSString(s)    ((const signed char*) PyBytes_AS_STRING(s))
+#define __Pyx_PyBytes_AsUString(s)    ((const unsigned char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyObject_AsWritableString(s)    ((char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsWritableSString(s)    ((signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if PY_MAJOR_VERSION < 3
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u) {
     const Py_UNICODE *u_end = u;
     while (*u_end++) ;
     return (size_t)(u_end - u - 1);
 }
-#else
-#define __Pyx_Py_UNICODE_strlen Py_UNICODE_strlen
-#endif
 #define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
 #define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 #define __Pyx_PyBool_FromLong(b) ((b) ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False))
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
+#define __Pyx_PySequence_Tuple(obj)\
+    (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
@@ -701,15 +755,15 @@
   #define unlikely(x) __builtin_expect(!!(x), 0)
 #else /* !__GNUC__ or GCC < 2.95 */
   #define likely(x)   (x)
   #define unlikely(x) (x)
 #endif /* __GNUC__ */
 static CYTHON_INLINE void __Pyx_pretend_to_initialize(void* ptr) { (void)ptr; }
 
-static PyObject *__pyx_m;
+static PyObject *__pyx_m = NULL;
 static PyObject *__pyx_d;
 static PyObject *__pyx_b;
 static PyObject *__pyx_cython_runtime;
 static PyObject *__pyx_empty_tuple;
 static PyObject *__pyx_empty_bytes;
 static PyObject *__pyx_empty_unicode;
 static int __pyx_lineno;
@@ -779,195 +833,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":725
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":743
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":726
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":744
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":727
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":745
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":728
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":746
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":732
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":750
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":733
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":751
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":734
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":752
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":735
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":753
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":739
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":757
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":740
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":758
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":749
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":767
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":750
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":768
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":751
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":769
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":753
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":771
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":754
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":772
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":755
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":773
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":757
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":775
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":758
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":776
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":760
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":778
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":761
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":779
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":762
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":780
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -994,42 +1048,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":764
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":782
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":765
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":783
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":766
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":784
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":768
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":786
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1188,58 +1242,90 @@
 /* RaiseNoneIterError.proto */
 static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
 
 /* UnpackTupleError.proto */
 static void __Pyx_UnpackTupleError(PyObject *, Py_ssize_t index);
 
 /* UnpackTuple2.proto */
-static CYTHON_INLINE int __Pyx_unpack_tuple2(PyObject* tuple, PyObject** value1, PyObject** value2,
-                                             int is_tuple, int has_known_size, int decref_tuple);
+#define __Pyx_unpack_tuple2(tuple, value1, value2, is_tuple, has_known_size, decref_tuple)\
+    (likely(is_tuple || PyTuple_Check(tuple)) ?\
+        (likely(has_known_size || PyTuple_GET_SIZE(tuple) == 2) ?\
+            __Pyx_unpack_tuple2_exact(tuple, value1, value2, decref_tuple) :\
+            (__Pyx_UnpackTupleError(tuple, 2), -1)) :\
+        __Pyx_unpack_tuple2_generic(tuple, value1, value2, has_known_size, decref_tuple))
+static CYTHON_INLINE int __Pyx_unpack_tuple2_exact(
+    PyObject* tuple, PyObject** value1, PyObject** value2, int decref_tuple);
+static int __Pyx_unpack_tuple2_generic(
+    PyObject* tuple, PyObject** value1, PyObject** value2, int has_known_size, int decref_tuple);
 
 /* dict_iter.proto */
 static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* dict, int is_dict, PyObject* method_name,
                                                    Py_ssize_t* p_orig_length, int* p_is_dict);
 static CYTHON_INLINE int __Pyx_dict_iter_next(PyObject* dict_or_iter, Py_ssize_t orig_length, Py_ssize_t* ppos,
                                               PyObject** pkey, PyObject** pvalue, PyObject** pitem, int is_dict);
 
 /* GetModuleGlobalName.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetModuleGlobalName(PyObject *name);
 
+/* IsLittleEndian.proto */
+static CYTHON_INLINE int __Pyx_Is_Little_Endian(void);
+
 /* BufferFormatCheck.proto */
-static CYTHON_INLINE int  __Pyx_GetBufferAndValidate(Py_buffer* buf, PyObject* obj,
-    __Pyx_TypeInfo* dtype, int flags, int nd, int cast, __Pyx_BufFmt_StackElem* stack);
-static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info);
 static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts);
 static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
                               __Pyx_BufFmt_StackElem* stack,
                               __Pyx_TypeInfo* type);
 
+/* BufferGetAndValidate.proto */
+#define __Pyx_GetBufferAndValidate(buf, obj, dtype, flags, nd, cast, stack)\
+    ((obj == Py_None || obj == NULL) ?\
+    (__Pyx_ZeroBuffer(buf), 0) :\
+    __Pyx__GetBufferAndValidate(buf, obj, dtype, flags, nd, cast, stack))
+static int  __Pyx__GetBufferAndValidate(Py_buffer* buf, PyObject* obj,
+    __Pyx_TypeInfo* dtype, int flags, int nd, int cast, __Pyx_BufFmt_StackElem* stack);
+static void __Pyx_ZeroBuffer(Py_buffer* buf);
+static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info);
+static Py_ssize_t __Pyx_minusones[] = { -1, -1, -1, -1, -1, -1, -1, -1 };
+static Py_ssize_t __Pyx_zeros[] = { 0, 0, 0, 0, 0, 0, 0, 0 };
+
 /* ExtTypeTest.proto */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
 
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
-#define __Pyx_PyThreadState_assign  __pyx_tstate = PyThreadState_GET();
+#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
+#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
 #else
 #define __Pyx_PyThreadState_declare
 #define __Pyx_PyThreadState_assign
+#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
 #endif
 
 /* PyErrFetchRestore.proto */
 #if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
 #define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
 static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+#else
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#endif
 #else
+#define __Pyx_PyErr_Clear() PyErr_Clear()
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
 #define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
 #endif
 
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
@@ -1249,16 +1335,18 @@
 
 /* ParseKeywords.proto */
 static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
 /* ArgTypeTest.proto */
-static CYTHON_INLINE int __Pyx_ArgTypeTest(PyObject *obj, PyTypeObject *type, int none_allowed,
-    const char *name, int exact);
+#define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
+    ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
+        __Pyx__ArgTypeTest(obj, type, name, exact))
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* PySequenceContains.proto */
 static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
     int result = PySequence_Contains(seq, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
@@ -1290,15 +1378,15 @@
                                                               int wraparound, int boundscheck);
 #define __Pyx_GetItemInt_Tuple(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Tuple_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
     (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
                                                               int wraparound, int boundscheck);
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
 /* GetException.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
@@ -1376,15 +1464,19 @@
 #define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* CLineInTraceback.proto */
-static int __Pyx_CLineForTraceback(int c_line);
+#ifdef CYTHON_CLINE_IN_TRACEBACK
+#define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
+#else
+static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
+#endif
 
 /* CodeObjectCache.proto */
 typedef struct {
     PyCodeObject* code_object;
     int code_line;
 } __Pyx_CodeObjectCacheEntry;
 struct __Pyx_CodeObjectCache {
@@ -1420,18 +1512,14 @@
     static void __Pyx_ReleaseBuffer(Py_buffer *view);
 #else
     #define __Pyx_GetBuffer PyObject_GetBuffer
     #define __Pyx_ReleaseBuffer PyBuffer_Release
 #endif
 
 
-/* None.proto */
-static Py_ssize_t __Pyx_zeros[] = {0, 0, 0, 0, 0, 0, 0, 0};
-static Py_ssize_t __Pyx_minusones[] = {-1, -1, -1, -1, -1, -1, -1, -1};
-
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CppExceptionConversion.proto */
@@ -1585,14 +1673,26 @@
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
+/* FastTypeChecks.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
+static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
+static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
+static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
+#else
+#define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
+#define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
+#define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
+#endif
+
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* PyIdentifierFromString.proto */
 #if !defined(__Pyx_PyIdentifier_FromString)
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_PyIdentifier_FromString(s) PyString_FromString(s)
@@ -1632,14 +1732,16 @@
 
 /* Module declarations from 'libcpp.string' */
 
 /* Module declarations from 'libcpp.vector' */
 
 /* Module declarations from 'cpython.ref' */
 
+/* Module declarations from 'cpython.mem' */
+
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
@@ -1654,14 +1756,16 @@
 /* Module declarations from 'anyode_numpy' */
 
 /* Module declarations from 'cvodes_cxx' */
 
 /* Module declarations from 'cvodes_anyode' */
 
 /* Module declarations from 'pycvodes._cvodes' */
+static PyObject *__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_k;
+static PyObject *__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_v;
 static PyObject *__pyx_f_8pycvodes_7_cvodes_get_last_info(AnyODE::PyOdeSys *, struct __pyx_opt_args_8pycvodes_7_cvodes_get_last_info *__pyx_optional_args); /*proto*/
 static PyObject *__pyx_f_8pycvodes_7_cvodes__reshape_roots(PyArrayObject *, int); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &); /*proto*/
@@ -1670,14 +1774,15 @@
 static PyObject *__pyx_convert_vector_to_py_double(const std::vector<double>  &); /*proto*/
 static PyObject *__pyx_convert_unordered_map_to_py_std_3a__3a_string____std_3a__3a_vector_3c_double_3e___(std::unordered_map<std::string,std::vector<double> >  const &); /*proto*/
 static PyObject *__pyx_convert_vector_to_py_int(const std::vector<int>  &); /*proto*/
 static PyObject *__pyx_convert_unordered_map_to_py_std_3a__3a_string____std_3a__3a_vector_3c_int_3e___(std::unordered_map<std::string,std::vector<int> >  const &); /*proto*/
 static std::string __pyx_convert_string_from_py_std__in_string(PyObject *); /*proto*/
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t = { "float64_t", NULL, sizeof(__pyx_t_5numpy_float64_t), { 0 }, 0, 'R', 0, 0 };
 #define __Pyx_MODULE_NAME "pycvodes._cvodes"
+extern int __pyx_module_is_main_pycvodes___cvodes;
 int __pyx_module_is_main_pycvodes___cvodes = 0;
 
 /* Implementation of 'pycvodes._cvodes' */
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_ImportError;
@@ -1984,14 +2089,22 @@
  *     info = {str(k.decode('utf-8')): v for k, v in dict(odesys.last_integration_info).items()}
  *     info.update({str(k.decode('utf-8')): v for k, v in dict(odesys.last_integration_info_dbl).items()})
  */
 
 static PyObject *__pyx_f_8pycvodes_7_cvodes_get_last_info(AnyODE::PyOdeSys *__pyx_v_odesys, struct __pyx_opt_args_8pycvodes_7_cvodes_get_last_info *__pyx_optional_args) {
   PyObject *__pyx_v_success = ((PyObject *)Py_True);
   PyObject *__pyx_v_info = NULL;
+  PyObject *__pyx_8genexpr1__pyx_v_k = NULL;
+  PyObject *__pyx_8genexpr1__pyx_v_v = NULL;
+  PyObject *__pyx_8genexpr2__pyx_v_k = NULL;
+  PyObject *__pyx_8genexpr2__pyx_v_v = NULL;
+  PyObject *__pyx_8genexpr3__pyx_v_k = NULL;
+  PyObject *__pyx_8genexpr3__pyx_v_v = NULL;
+  PyObject *__pyx_8genexpr4__pyx_v_k = NULL;
+  PyObject *__pyx_8genexpr4__pyx_v_v = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
@@ -2015,16 +2128,14 @@
  * 
  * cdef dict get_last_info(PyOdeSys * odesys, success=True):
  *     info = {str(k.decode('utf-8')): v for k, v in dict(odesys.last_integration_info).items()}             # <<<<<<<<<<<<<<
  *     info.update({str(k.decode('utf-8')): v for k, v in dict(odesys.last_integration_info_dbl).items()})
  *     info.update({str(k.decode('utf-8')): np.array(v, dtype=np.float64) for k, v in dict(odesys.last_integration_info_vecdbl).items()})
  */
   { /* enter inner scope */
-    PyObject *__pyx_8genexpr1__pyx_v_k = NULL;
-    PyObject *__pyx_8genexpr1__pyx_v_v = NULL;
     __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = 0;
     __pyx_t_6 = __pyx_convert_unordered_map_to_py_std_3a__3a_string____int(__pyx_v_odesys->last_integration_info); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 32, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 32, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_7);
@@ -2063,20 +2174,20 @@
       __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_6, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 32, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_t_7, (PyObject*)__pyx_8genexpr1__pyx_v_v))) __PYX_ERR(0, 32, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_k);
-    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v);
+    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_k); __pyx_8genexpr1__pyx_v_k = 0;
+    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v); __pyx_8genexpr1__pyx_v_v = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
-    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_k);
-    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v);
+    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_k); __pyx_8genexpr1__pyx_v_k = 0;
+    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v); __pyx_8genexpr1__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_v_info = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "pycvodes/_cvodes.pyx":33
@@ -2085,16 +2196,14 @@
  *     info.update({str(k.decode('utf-8')): v for k, v in dict(odesys.last_integration_info_dbl).items()})             # <<<<<<<<<<<<<<
  *     info.update({str(k.decode('utf-8')): np.array(v, dtype=np.float64) for k, v in dict(odesys.last_integration_info_vecdbl).items()})
  *     info.update({str(k.decode('utf-8')): np.array(v, dtype=int) for k, v in dict(odesys.last_integration_info_vecint).items()})
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_info, __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   { /* enter inner scope */
-    PyObject *__pyx_8genexpr2__pyx_v_k = NULL;
-    PyObject *__pyx_8genexpr2__pyx_v_v = NULL;
     __pyx_t_7 = PyDict_New(); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 33, __pyx_L11_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_4 = 0;
     __pyx_t_9 = __pyx_convert_unordered_map_to_py_std_3a__3a_string____double(__pyx_v_odesys->last_integration_info_dbl); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 33, __pyx_L11_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 33, __pyx_L11_error)
     __Pyx_GOTREF(__pyx_t_10);
@@ -2133,20 +2242,20 @@
       __pyx_t_10 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_9, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 33, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       if (unlikely(PyDict_SetItem(__pyx_t_7, (PyObject*)__pyx_t_10, (PyObject*)__pyx_8genexpr2__pyx_v_v))) __PYX_ERR(0, 33, __pyx_L11_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_k);
-    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_v);
+    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_k); __pyx_8genexpr2__pyx_v_k = 0;
+    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_v); __pyx_8genexpr2__pyx_v_v = 0;
     goto __pyx_L14_exit_scope;
     __pyx_L11_error:;
-    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_k);
-    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_v);
+    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_k); __pyx_8genexpr2__pyx_v_k = 0;
+    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_v); __pyx_8genexpr2__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L14_exit_scope:;
   } /* exit inner scope */
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_6)) {
@@ -2200,16 +2309,14 @@
  *     info.update({str(k.decode('utf-8')): np.array(v, dtype=np.float64) for k, v in dict(odesys.last_integration_info_vecdbl).items()})             # <<<<<<<<<<<<<<
  *     info.update({str(k.decode('utf-8')): np.array(v, dtype=int) for k, v in dict(odesys.last_integration_info_vecint).items()})
  *     info['nfev'] = odesys.nfev
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_info, __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   { /* enter inner scope */
-    PyObject *__pyx_8genexpr3__pyx_v_k = NULL;
-    PyObject *__pyx_8genexpr3__pyx_v_v = NULL;
     __pyx_t_10 = PyDict_New(); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 34, __pyx_L17_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_3 = 0;
     __pyx_t_6 = __pyx_convert_unordered_map_to_py_std_3a__3a_string____std_3a__3a_vector_3c_double_3e___(__pyx_v_odesys->last_integration_info_vecdbl); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 34, __pyx_L17_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 34, __pyx_L17_error)
     __Pyx_GOTREF(__pyx_t_9);
@@ -2254,15 +2361,15 @@
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 34, __pyx_L17_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_INCREF(__pyx_8genexpr3__pyx_v_v);
       __Pyx_GIVEREF(__pyx_8genexpr3__pyx_v_v);
       PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_8genexpr3__pyx_v_v);
-      __pyx_t_12 = PyDict_New(); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 34, __pyx_L17_error)
+      __pyx_t_12 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 34, __pyx_L17_error)
       __Pyx_GOTREF(__pyx_t_12);
       __pyx_t_13 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 34, __pyx_L17_error)
       __Pyx_GOTREF(__pyx_t_13);
       __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_float64); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 34, __pyx_L17_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_dtype, __pyx_t_14) < 0) __PYX_ERR(0, 34, __pyx_L17_error)
@@ -2273,20 +2380,20 @@
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       if (unlikely(PyDict_SetItem(__pyx_t_10, (PyObject*)__pyx_t_9, (PyObject*)__pyx_t_14))) __PYX_ERR(0, 34, __pyx_L17_error)
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
     }
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_k);
-    __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_v);
+    __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_k); __pyx_8genexpr3__pyx_v_k = 0;
+    __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_v); __pyx_8genexpr3__pyx_v_v = 0;
     goto __pyx_L20_exit_scope;
     __pyx_L17_error:;
-    __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_k);
-    __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_v);
+    __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_k); __pyx_8genexpr3__pyx_v_k = 0;
+    __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_v); __pyx_8genexpr3__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L20_exit_scope:;
   } /* exit inner scope */
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_7)) {
@@ -2340,16 +2447,14 @@
  *     info.update({str(k.decode('utf-8')): np.array(v, dtype=int) for k, v in dict(odesys.last_integration_info_vecint).items()})             # <<<<<<<<<<<<<<
  *     info['nfev'] = odesys.nfev
  *     info['njev'] = odesys.njev
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_info, __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   { /* enter inner scope */
-    PyObject *__pyx_8genexpr4__pyx_v_k = NULL;
-    PyObject *__pyx_8genexpr4__pyx_v_v = NULL;
     __pyx_t_14 = PyDict_New(); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 35, __pyx_L23_error)
     __Pyx_GOTREF(__pyx_t_14);
     __pyx_t_4 = 0;
     __pyx_t_7 = __pyx_convert_unordered_map_to_py_std_3a__3a_string____std_3a__3a_vector_3c_int_3e___(__pyx_v_odesys->last_integration_info_vecint); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 35, __pyx_L23_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 35, __pyx_L23_error)
     __Pyx_GOTREF(__pyx_t_9);
@@ -2394,33 +2499,33 @@
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 35, __pyx_L23_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_INCREF(__pyx_8genexpr4__pyx_v_v);
       __Pyx_GIVEREF(__pyx_8genexpr4__pyx_v_v);
       PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_8genexpr4__pyx_v_v);
-      __pyx_t_6 = PyDict_New(); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 35, __pyx_L23_error)
+      __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 35, __pyx_L23_error)
       __Pyx_GOTREF(__pyx_t_6);
       if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, ((PyObject *)(&PyInt_Type))) < 0) __PYX_ERR(0, 35, __pyx_L23_error)
       __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_7, __pyx_t_6); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 35, __pyx_L23_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (unlikely(PyDict_SetItem(__pyx_t_14, (PyObject*)__pyx_t_9, (PyObject*)__pyx_t_11))) __PYX_ERR(0, 35, __pyx_L23_error)
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     }
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_k);
-    __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_v);
+    __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_k); __pyx_8genexpr4__pyx_v_k = 0;
+    __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_v); __pyx_8genexpr4__pyx_v_v = 0;
     goto __pyx_L26_exit_scope;
     __pyx_L23_error:;
-    __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_k);
-    __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_v);
+    __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_k); __pyx_8genexpr4__pyx_v_k = 0;
+    __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_v); __pyx_8genexpr4__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L26_exit_scope:;
   } /* exit inner scope */
   __pyx_t_10 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_10)) {
@@ -2533,14 +2638,22 @@
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_XDECREF(__pyx_t_13);
   __Pyx_XDECREF(__pyx_t_14);
   __Pyx_AddTraceback("pycvodes._cvodes.get_last_info", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_info);
+  __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_k);
+  __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v);
+  __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_k);
+  __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_v);
+  __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_k);
+  __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_v);
+  __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_k);
+  __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_v);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "pycvodes/_cvodes.pyx":41
  *     return info
@@ -3504,15 +3617,15 @@
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
-            if (likely(exc_type == PyExc_StopIteration || PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
             else __PYX_ERR(0, 68, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_at, __pyx_t_7);
@@ -4044,15 +4157,15 @@
         #endif
       }
     } else {
       __pyx_t_7 = __pyx_t_6(__pyx_t_11);
       if (unlikely(!__pyx_t_7)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
-          if (likely(exc_type == PyExc_StopIteration || PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
           else __PYX_ERR(0, 78, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_7);
     }
     __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_7);
@@ -4293,14 +4406,15 @@
         PyErr_Fetch(&__pyx_t_19, &__pyx_t_20, &__pyx_t_21);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_xyout_arr.rcbuffer->pybuffer, (PyObject*)__pyx_v_xyout_arr, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
           Py_XDECREF(__pyx_t_19); Py_XDECREF(__pyx_t_20); Py_XDECREF(__pyx_t_21);
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_19, __pyx_t_20, __pyx_t_21);
         }
+        __pyx_t_19 = __pyx_t_20 = __pyx_t_21 = 0;
       }
       __pyx_pybuffernd_xyout_arr.diminfo[0].strides = __pyx_pybuffernd_xyout_arr.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_xyout_arr.diminfo[0].shape = __pyx_pybuffernd_xyout_arr.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_xyout_arr.diminfo[1].strides = __pyx_pybuffernd_xyout_arr.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_xyout_arr.diminfo[1].shape = __pyx_pybuffernd_xyout_arr.rcbuffer->pybuffer.shape[1];
       if (unlikely(__pyx_t_17 < 0)) __PYX_ERR(0, 98, __pyx_L16_error)
     }
     __pyx_t_18 = 0;
     __pyx_v_xyout_arr = ((PyArrayObject *)__pyx_t_11);
     __pyx_t_11 = 0;
@@ -4357,15 +4471,15 @@
  */
       __pyx_t_1 = (__pyx_v_return_on_root != 0);
       if (__pyx_t_1) {
       } else {
         __pyx_t_2 = __pyx_t_1;
         goto __pyx_L20_bool_binop_done;
       }
-      __pyx_t_5 = PyObject_Length(__pyx_v_xout); if (unlikely(__pyx_t_5 == -1)) __PYX_ERR(0, 104, __pyx_L16_error)
+      __pyx_t_5 = PyObject_Length(__pyx_v_xout); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 104, __pyx_L16_error)
       __pyx_t_1 = (((__pyx_v_root_indices[(__pyx_v_root_indices.size() - 1)]) == (__pyx_t_5 - 1)) != 0);
       __pyx_t_2 = __pyx_t_1;
       __pyx_L20_bool_binop_done:;
       if (__pyx_t_2) {
 
         /* "pycvodes/_cvodes.pyx":105
  *         if return_on_error:
@@ -4630,19 +4744,19 @@
  *         return xout, yout.reshape(yout_shape), info
  *     finally:
  *         del odesys             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*finally:*/ {
+    __pyx_L16_error:;
     /*exception exit:*/{
       __Pyx_PyThreadState_declare
-      __pyx_L16_error:;
-      __pyx_t_21 = 0; __pyx_t_20 = 0; __pyx_t_19 = 0; __pyx_t_25 = 0; __pyx_t_26 = 0; __pyx_t_27 = 0;
       __Pyx_PyThreadState_assign
+      __pyx_t_21 = 0; __pyx_t_20 = 0; __pyx_t_19 = 0; __pyx_t_25 = 0; __pyx_t_26 = 0; __pyx_t_27 = 0;
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_25, &__pyx_t_26, &__pyx_t_27);
@@ -4653,15 +4767,14 @@
       __Pyx_XGOTREF(__pyx_t_25);
       __Pyx_XGOTREF(__pyx_t_26);
       __Pyx_XGOTREF(__pyx_t_27);
       __pyx_t_17 = __pyx_lineno; __pyx_t_23 = __pyx_clineno; __pyx_t_24 = __pyx_filename;
       {
         delete __pyx_v_odesys;
       }
-      __Pyx_PyThreadState_assign
       if (PY_MAJOR_VERSION >= 3) {
         __Pyx_XGIVEREF(__pyx_t_25);
         __Pyx_XGIVEREF(__pyx_t_26);
         __Pyx_XGIVEREF(__pyx_t_27);
         __Pyx_ExceptionReset(__pyx_t_25, __pyx_t_26, __pyx_t_27);
       }
       __Pyx_XGIVEREF(__pyx_t_21);
@@ -5555,15 +5668,15 @@
           #endif
         }
       } else {
         __pyx_t_3 = __pyx_t_12(__pyx_t_1);
         if (unlikely(!__pyx_t_3)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
-            if (likely(exc_type == PyExc_StopIteration || PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
             else __PYX_ERR(0, 145, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_3);
       }
       __Pyx_XDECREF_SET(__pyx_v_at, __pyx_t_3);
@@ -6496,19 +6609,19 @@
 
   /* "pycvodes/_cvodes.pyx":178
  *         return yout.reshape((xout.size, ny)) if nderiv == 0 else yout, info
  *     finally:
  *         del odesys             # <<<<<<<<<<<<<<
  */
   /*finally:*/ {
+    __pyx_L14_error:;
     /*exception exit:*/{
       __Pyx_PyThreadState_declare
-      __pyx_L14_error:;
-      __pyx_t_24 = 0; __pyx_t_25 = 0; __pyx_t_26 = 0; __pyx_t_27 = 0; __pyx_t_28 = 0; __pyx_t_29 = 0;
       __Pyx_PyThreadState_assign
+      __pyx_t_24 = 0; __pyx_t_25 = 0; __pyx_t_26 = 0; __pyx_t_27 = 0; __pyx_t_28 = 0; __pyx_t_29 = 0;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_27, &__pyx_t_28, &__pyx_t_29);
@@ -6519,15 +6632,14 @@
       __Pyx_XGOTREF(__pyx_t_27);
       __Pyx_XGOTREF(__pyx_t_28);
       __Pyx_XGOTREF(__pyx_t_29);
       __pyx_t_17 = __pyx_lineno; __pyx_t_22 = __pyx_clineno; __pyx_t_23 = __pyx_filename;
       {
         delete __pyx_v_odesys;
       }
-      __Pyx_PyThreadState_assign
       if (PY_MAJOR_VERSION >= 3) {
         __Pyx_XGIVEREF(__pyx_t_27);
         __Pyx_XGIVEREF(__pyx_t_28);
         __Pyx_XGIVEREF(__pyx_t_29);
         __Pyx_ExceptionReset(__pyx_t_27, __pyx_t_28, __pyx_t_29);
       }
       __Pyx_XGIVEREF(__pyx_t_24);
@@ -6584,15 +6696,15 @@
   __Pyx_XDECREF(__pyx_v_at);
   __Pyx_XDECREF(__pyx_v_info);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":197
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":214
  *         # experimental exception made for __getbuffer__ and __releasebuffer__
  *         # -- the details of this may change.
  *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
  *             # This implementation of getbuffer is geared towards Cython
  *             # requirements, and does not yet fullfill the PEP.
  */
 
@@ -6631,372 +6743,372 @@
   char *__pyx_t_7;
   __Pyx_RefNannySetupContext("__getbuffer__", 0);
   if (__pyx_v_info != NULL) {
     __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(__pyx_v_info->obj);
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":203
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":220
  *             # of flags
  * 
  *             if info == NULL: return             # <<<<<<<<<<<<<<
  * 
  *             cdef int copy_shape, i, ndim
  */
   __pyx_t_1 = ((__pyx_v_info == NULL) != 0);
   if (__pyx_t_1) {
     __pyx_r = 0;
     goto __pyx_L0;
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":206
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":223
  * 
  *             cdef int copy_shape, i, ndim
  *             cdef int endian_detector = 1             # <<<<<<<<<<<<<<
  *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
  * 
  */
   __pyx_v_endian_detector = 1;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":207
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":224
  *             cdef int copy_shape, i, ndim
  *             cdef int endian_detector = 1
  *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
  * 
  *             ndim = PyArray_NDIM(self)
  */
   __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":209
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":226
  *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
  * 
  *             ndim = PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  */
   __pyx_v_ndim = PyArray_NDIM(__pyx_v_self);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":211
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":228
  *             ndim = PyArray_NDIM(self)
  * 
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
  *                 copy_shape = 1
  *             else:
  */
   __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
   if (__pyx_t_1) {
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":212
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":229
  * 
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  *                 copy_shape = 1             # <<<<<<<<<<<<<<
  *             else:
  *                 copy_shape = 0
  */
     __pyx_v_copy_shape = 1;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":211
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":228
  *             ndim = PyArray_NDIM(self)
  * 
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
  *                 copy_shape = 1
  *             else:
  */
     goto __pyx_L4;
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":214
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":231
  *                 copy_shape = 1
  *             else:
  *                 copy_shape = 0             # <<<<<<<<<<<<<<
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  */
   /*else*/ {
     __pyx_v_copy_shape = 0;
   }
   __pyx_L4:;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":216
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":233
  *                 copy_shape = 0
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")
  */
   __pyx_t_2 = (((__pyx_v_flags & PyBUF_C_CONTIGUOUS) == PyBUF_C_CONTIGUOUS) != 0);
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L6_bool_binop_done;
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":217
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":234
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_C_CONTIGUOUS)):             # <<<<<<<<<<<<<<
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  */
   __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_C_CONTIGUOUS) != 0)) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L6_bool_binop_done:;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":216
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":233
  *                 copy_shape = 0
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")
  */
   if (__pyx_t_1) {
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":218
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":235
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 218, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 235, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 218, __pyx_L1_error)
+    __PYX_ERR(1, 235, __pyx_L1_error)
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":216
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":233
  *                 copy_shape = 0
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")
  */
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":220
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":237
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  */
   __pyx_t_2 = (((__pyx_v_flags & PyBUF_F_CONTIGUOUS) == PyBUF_F_CONTIGUOUS) != 0);
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L9_bool_binop_done;
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":221
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":238
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_F_CONTIGUOUS)):             # <<<<<<<<<<<<<<
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  * 
  */
   __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_F_CONTIGUOUS) != 0)) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L9_bool_binop_done:;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":220
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":237
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  */
   if (__pyx_t_1) {
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":222
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":239
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
  * 
  *             info.buf = PyArray_DATA(self)
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 222, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 239, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 222, __pyx_L1_error)
+    __PYX_ERR(1, 239, __pyx_L1_error)
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":220
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":237
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  */
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":224
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":241
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  * 
  *             info.buf = PyArray_DATA(self)             # <<<<<<<<<<<<<<
  *             info.ndim = ndim
  *             if copy_shape:
  */
   __pyx_v_info->buf = PyArray_DATA(__pyx_v_self);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":225
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":242
  * 
  *             info.buf = PyArray_DATA(self)
  *             info.ndim = ndim             # <<<<<<<<<<<<<<
  *             if copy_shape:
  *                 # Allocate new buffer for strides and shape info.
  */
   __pyx_v_info->ndim = __pyx_v_ndim;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":226
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":243
  *             info.buf = PyArray_DATA(self)
  *             info.ndim = ndim
  *             if copy_shape:             # <<<<<<<<<<<<<<
  *                 # Allocate new buffer for strides and shape info.
  *                 # This is allocated as one block, strides first.
  */
   __pyx_t_1 = (__pyx_v_copy_shape != 0);
   if (__pyx_t_1) {
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":229
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":246
  *                 # Allocate new buffer for strides and shape info.
  *                 # This is allocated as one block, strides first.
- *                 info.strides = <Py_ssize_t*>stdlib.malloc(sizeof(Py_ssize_t) * <size_t>ndim * 2)             # <<<<<<<<<<<<<<
+ *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)             # <<<<<<<<<<<<<<
  *                 info.shape = info.strides + ndim
  *                 for i in range(ndim):
  */
-    __pyx_v_info->strides = ((Py_ssize_t *)malloc((((sizeof(Py_ssize_t)) * ((size_t)__pyx_v_ndim)) * 2)));
+    __pyx_v_info->strides = ((Py_ssize_t *)PyObject_Malloc((((sizeof(Py_ssize_t)) * 2) * ((size_t)__pyx_v_ndim))));
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":230
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":247
  *                 # This is allocated as one block, strides first.
- *                 info.strides = <Py_ssize_t*>stdlib.malloc(sizeof(Py_ssize_t) * <size_t>ndim * 2)
+ *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
  *                 info.shape = info.strides + ndim             # <<<<<<<<<<<<<<
  *                 for i in range(ndim):
  *                     info.strides[i] = PyArray_STRIDES(self)[i]
  */
     __pyx_v_info->shape = (__pyx_v_info->strides + __pyx_v_ndim);
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":231
- *                 info.strides = <Py_ssize_t*>stdlib.malloc(sizeof(Py_ssize_t) * <size_t>ndim * 2)
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":248
+ *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
  *                 info.shape = info.strides + ndim
  *                 for i in range(ndim):             # <<<<<<<<<<<<<<
  *                     info.strides[i] = PyArray_STRIDES(self)[i]
  *                     info.shape[i] = PyArray_DIMS(self)[i]
  */
     __pyx_t_4 = __pyx_v_ndim;
     for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
       __pyx_v_i = __pyx_t_5;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":232
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":249
  *                 info.shape = info.strides + ndim
  *                 for i in range(ndim):
  *                     info.strides[i] = PyArray_STRIDES(self)[i]             # <<<<<<<<<<<<<<
  *                     info.shape[i] = PyArray_DIMS(self)[i]
  *             else:
  */
       (__pyx_v_info->strides[__pyx_v_i]) = (PyArray_STRIDES(__pyx_v_self)[__pyx_v_i]);
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":233
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":250
  *                 for i in range(ndim):
  *                     info.strides[i] = PyArray_STRIDES(self)[i]
  *                     info.shape[i] = PyArray_DIMS(self)[i]             # <<<<<<<<<<<<<<
  *             else:
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
  */
       (__pyx_v_info->shape[__pyx_v_i]) = (PyArray_DIMS(__pyx_v_self)[__pyx_v_i]);
     }
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":226
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":243
  *             info.buf = PyArray_DATA(self)
  *             info.ndim = ndim
  *             if copy_shape:             # <<<<<<<<<<<<<<
  *                 # Allocate new buffer for strides and shape info.
  *                 # This is allocated as one block, strides first.
  */
     goto __pyx_L11;
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":235
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":252
  *                     info.shape[i] = PyArray_DIMS(self)[i]
  *             else:
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
  *             info.suboffsets = NULL
  */
   /*else*/ {
     __pyx_v_info->strides = ((Py_ssize_t *)PyArray_STRIDES(__pyx_v_self));
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":236
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":253
  *             else:
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  *             info.suboffsets = NULL
  *             info.itemsize = PyArray_ITEMSIZE(self)
  */
     __pyx_v_info->shape = ((Py_ssize_t *)PyArray_DIMS(__pyx_v_self));
   }
   __pyx_L11:;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":237
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":254
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
  *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
  *             info.itemsize = PyArray_ITEMSIZE(self)
  *             info.readonly = not PyArray_ISWRITEABLE(self)
  */
   __pyx_v_info->suboffsets = NULL;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":238
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":255
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
  *             info.suboffsets = NULL
  *             info.itemsize = PyArray_ITEMSIZE(self)             # <<<<<<<<<<<<<<
  *             info.readonly = not PyArray_ISWRITEABLE(self)
  * 
  */
   __pyx_v_info->itemsize = PyArray_ITEMSIZE(__pyx_v_self);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":239
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":256
  *             info.suboffsets = NULL
  *             info.itemsize = PyArray_ITEMSIZE(self)
  *             info.readonly = not PyArray_ISWRITEABLE(self)             # <<<<<<<<<<<<<<
  * 
  *             cdef int t
  */
   __pyx_v_info->readonly = (!(PyArray_ISWRITEABLE(__pyx_v_self) != 0));
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":242
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":259
  * 
  *             cdef int t
  *             cdef char* f = NULL             # <<<<<<<<<<<<<<
  *             cdef dtype descr = self.descr
  *             cdef int offset
  */
   __pyx_v_f = NULL;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":243
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":260
  *             cdef int t
  *             cdef char* f = NULL
  *             cdef dtype descr = self.descr             # <<<<<<<<<<<<<<
  *             cdef int offset
  * 
  */
   __pyx_t_3 = ((PyObject *)__pyx_v_self->descr);
   __Pyx_INCREF(__pyx_t_3);
   __pyx_v_descr = ((PyArray_Descr *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":246
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":263
  *             cdef int offset
  * 
  *             cdef bint hasfields = PyDataType_HASFIELDS(descr)             # <<<<<<<<<<<<<<
  * 
  *             if not hasfields and not copy_shape:
  */
   __pyx_v_hasfields = PyDataType_HASFIELDS(__pyx_v_descr);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":248
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":265
  *             cdef bint hasfields = PyDataType_HASFIELDS(descr)
  * 
  *             if not hasfields and not copy_shape:             # <<<<<<<<<<<<<<
  *                 # do not call releasebuffer
  *                 info.obj = None
  */
   __pyx_t_2 = ((!(__pyx_v_hasfields != 0)) != 0);
@@ -7006,38 +7118,38 @@
     goto __pyx_L15_bool_binop_done;
   }
   __pyx_t_2 = ((!(__pyx_v_copy_shape != 0)) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L15_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":250
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":267
  *             if not hasfields and not copy_shape:
  *                 # do not call releasebuffer
  *                 info.obj = None             # <<<<<<<<<<<<<<
  *             else:
  *                 # need to call releasebuffer
  */
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     __Pyx_GOTREF(__pyx_v_info->obj);
     __Pyx_DECREF(__pyx_v_info->obj);
     __pyx_v_info->obj = Py_None;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":248
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":265
  *             cdef bint hasfields = PyDataType_HASFIELDS(descr)
  * 
  *             if not hasfields and not copy_shape:             # <<<<<<<<<<<<<<
  *                 # do not call releasebuffer
  *                 info.obj = None
  */
     goto __pyx_L14;
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":253
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":270
  *             else:
  *                 # need to call releasebuffer
  *                 info.obj = self             # <<<<<<<<<<<<<<
  * 
  *             if not hasfields:
  */
   /*else*/ {
@@ -7045,35 +7157,35 @@
     __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
     __Pyx_GOTREF(__pyx_v_info->obj);
     __Pyx_DECREF(__pyx_v_info->obj);
     __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
   }
   __pyx_L14:;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":255
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":272
  *                 info.obj = self
  * 
  *             if not hasfields:             # <<<<<<<<<<<<<<
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or
  */
   __pyx_t_1 = ((!(__pyx_v_hasfields != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":256
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":273
  * 
  *             if not hasfields:
  *                 t = descr.type_num             # <<<<<<<<<<<<<<
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):
  */
     __pyx_t_4 = __pyx_v_descr->type_num;
     __pyx_v_t = __pyx_t_4;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":257
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":274
  *             if not hasfields:
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  */
     __pyx_t_2 = ((__pyx_v_descr->byteorder == '>') != 0);
@@ -7085,15 +7197,15 @@
     if (!__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L19_bool_binop_done;
     }
     __pyx_L20_next_or:;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":258
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":275
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
  *                     raise ValueError(u"Non-native byte order not supported")
  *                 if   t == NPY_BYTE:        f = "b"
  */
     __pyx_t_2 = ((__pyx_v_descr->byteorder == '<') != 0);
@@ -7102,337 +7214,337 @@
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L19_bool_binop_done;
     }
     __pyx_t_2 = ((!(__pyx_v_little_endian != 0)) != 0);
     __pyx_t_1 = __pyx_t_2;
     __pyx_L19_bool_binop_done:;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":257
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":274
  *             if not hasfields:
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  */
     if (__pyx_t_1) {
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":259
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":276
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"
  */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 259, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 276, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 259, __pyx_L1_error)
+      __PYX_ERR(1, 276, __pyx_L1_error)
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":257
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":274
  *             if not hasfields:
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  */
     }
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":260
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":277
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  *                 if   t == NPY_BYTE:        f = "b"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_UBYTE:       f = "B"
  *                 elif t == NPY_SHORT:       f = "h"
  */
     switch (__pyx_v_t) {
       case NPY_BYTE:
       __pyx_v_f = ((char *)"b");
       break;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":261
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":278
  *                     raise ValueError(u"Non-native byte order not supported")
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_SHORT:       f = "h"
  *                 elif t == NPY_USHORT:      f = "H"
  */
       case NPY_UBYTE:
       __pyx_v_f = ((char *)"B");
       break;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":262
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":279
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"
  *                 elif t == NPY_SHORT:       f = "h"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_USHORT:      f = "H"
  *                 elif t == NPY_INT:         f = "i"
  */
       case NPY_SHORT:
       __pyx_v_f = ((char *)"h");
       break;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":263
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":280
  *                 elif t == NPY_UBYTE:       f = "B"
  *                 elif t == NPY_SHORT:       f = "h"
  *                 elif t == NPY_USHORT:      f = "H"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_INT:         f = "i"
  *                 elif t == NPY_UINT:        f = "I"
  */
       case NPY_USHORT:
       __pyx_v_f = ((char *)"H");
       break;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":264
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":281
  *                 elif t == NPY_SHORT:       f = "h"
  *                 elif t == NPY_USHORT:      f = "H"
  *                 elif t == NPY_INT:         f = "i"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_UINT:        f = "I"
  *                 elif t == NPY_LONG:        f = "l"
  */
       case NPY_INT:
       __pyx_v_f = ((char *)"i");
       break;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":265
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":282
  *                 elif t == NPY_USHORT:      f = "H"
  *                 elif t == NPY_INT:         f = "i"
  *                 elif t == NPY_UINT:        f = "I"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_LONG:        f = "l"
  *                 elif t == NPY_ULONG:       f = "L"
  */
       case NPY_UINT:
       __pyx_v_f = ((char *)"I");
       break;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":266
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":283
  *                 elif t == NPY_INT:         f = "i"
  *                 elif t == NPY_UINT:        f = "I"
  *                 elif t == NPY_LONG:        f = "l"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_ULONG:       f = "L"
  *                 elif t == NPY_LONGLONG:    f = "q"
  */
       case NPY_LONG:
       __pyx_v_f = ((char *)"l");
       break;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":267
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":284
  *                 elif t == NPY_UINT:        f = "I"
  *                 elif t == NPY_LONG:        f = "l"
  *                 elif t == NPY_ULONG:       f = "L"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_LONGLONG:    f = "q"
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  */
       case NPY_ULONG:
       __pyx_v_f = ((char *)"L");
       break;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":268
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":285
  *                 elif t == NPY_LONG:        f = "l"
  *                 elif t == NPY_ULONG:       f = "L"
  *                 elif t == NPY_LONGLONG:    f = "q"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  *                 elif t == NPY_FLOAT:       f = "f"
  */
       case NPY_LONGLONG:
       __pyx_v_f = ((char *)"q");
       break;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":269
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":286
  *                 elif t == NPY_ULONG:       f = "L"
  *                 elif t == NPY_LONGLONG:    f = "q"
  *                 elif t == NPY_ULONGLONG:   f = "Q"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_FLOAT:       f = "f"
  *                 elif t == NPY_DOUBLE:      f = "d"
  */
       case NPY_ULONGLONG:
       __pyx_v_f = ((char *)"Q");
       break;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":270
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":287
  *                 elif t == NPY_LONGLONG:    f = "q"
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  *                 elif t == NPY_FLOAT:       f = "f"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_DOUBLE:      f = "d"
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  */
       case NPY_FLOAT:
       __pyx_v_f = ((char *)"f");
       break;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":271
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":288
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  *                 elif t == NPY_FLOAT:       f = "f"
  *                 elif t == NPY_DOUBLE:      f = "d"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  */
       case NPY_DOUBLE:
       __pyx_v_f = ((char *)"d");
       break;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":272
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":289
  *                 elif t == NPY_FLOAT:       f = "f"
  *                 elif t == NPY_DOUBLE:      f = "d"
  *                 elif t == NPY_LONGDOUBLE:  f = "g"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  */
       case NPY_LONGDOUBLE:
       __pyx_v_f = ((char *)"g");
       break;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":273
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":290
  *                 elif t == NPY_DOUBLE:      f = "d"
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  *                 elif t == NPY_CFLOAT:      f = "Zf"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
  */
       case NPY_CFLOAT:
       __pyx_v_f = ((char *)"Zf");
       break;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":274
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":291
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  *                 elif t == NPY_CDOUBLE:     f = "Zd"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
  *                 elif t == NPY_OBJECT:      f = "O"
  */
       case NPY_CDOUBLE:
       __pyx_v_f = ((char *)"Zd");
       break;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":275
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":292
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_OBJECT:      f = "O"
  *                 else:
  */
       case NPY_CLONGDOUBLE:
       __pyx_v_f = ((char *)"Zg");
       break;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":276
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":293
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
  *                 elif t == NPY_OBJECT:      f = "O"             # <<<<<<<<<<<<<<
  *                 else:
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  */
       case NPY_OBJECT:
       __pyx_v_f = ((char *)"O");
       break;
       default:
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":278
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":295
  *                 elif t == NPY_OBJECT:      f = "O"
  *                 else:
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
  *                 info.format = f
  *                 return
  */
-      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 278, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 295, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_6 = PyUnicode_Format(__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 278, __pyx_L1_error)
+      __pyx_t_6 = PyUnicode_Format(__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 295, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 278, __pyx_L1_error)
+      __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 295, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_6);
       __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_t_3, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 278, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_t_3, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 295, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(1, 278, __pyx_L1_error)
+      __PYX_ERR(1, 295, __pyx_L1_error)
       break;
     }
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":279
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":296
  *                 else:
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  *                 info.format = f             # <<<<<<<<<<<<<<
  *                 return
  *             else:
  */
     __pyx_v_info->format = __pyx_v_f;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":280
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":297
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  *                 info.format = f
  *                 return             # <<<<<<<<<<<<<<
  *             else:
- *                 info.format = <char*>stdlib.malloc(_buffer_format_string_len)
+ *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
  */
     __pyx_r = 0;
     goto __pyx_L0;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":255
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":272
  *                 info.obj = self
  * 
  *             if not hasfields:             # <<<<<<<<<<<<<<
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or
  */
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":282
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":299
  *                 return
  *             else:
- *                 info.format = <char*>stdlib.malloc(_buffer_format_string_len)             # <<<<<<<<<<<<<<
+ *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)             # <<<<<<<<<<<<<<
  *                 info.format[0] = c'^' # Native data types, manual alignment
  *                 offset = 0
  */
   /*else*/ {
-    __pyx_v_info->format = ((char *)malloc(0xFF));
+    __pyx_v_info->format = ((char *)PyObject_Malloc(0xFF));
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":283
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":300
  *             else:
- *                 info.format = <char*>stdlib.malloc(_buffer_format_string_len)
+ *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
  *                 info.format[0] = c'^' # Native data types, manual alignment             # <<<<<<<<<<<<<<
  *                 offset = 0
  *                 f = _util_dtypestring(descr, info.format + 1,
  */
     (__pyx_v_info->format[0]) = '^';
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":284
- *                 info.format = <char*>stdlib.malloc(_buffer_format_string_len)
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":301
+ *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
  *                 info.format[0] = c'^' # Native data types, manual alignment
  *                 offset = 0             # <<<<<<<<<<<<<<
  *                 f = _util_dtypestring(descr, info.format + 1,
  *                                       info.format + _buffer_format_string_len,
  */
     __pyx_v_offset = 0;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":285
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":302
  *                 info.format[0] = c'^' # Native data types, manual alignment
  *                 offset = 0
  *                 f = _util_dtypestring(descr, info.format + 1,             # <<<<<<<<<<<<<<
  *                                       info.format + _buffer_format_string_len,
  *                                       &offset)
  */
-    __pyx_t_7 = __pyx_f_5numpy__util_dtypestring(__pyx_v_descr, (__pyx_v_info->format + 1), (__pyx_v_info->format + 0xFF), (&__pyx_v_offset)); if (unlikely(__pyx_t_7 == NULL)) __PYX_ERR(1, 285, __pyx_L1_error)
+    __pyx_t_7 = __pyx_f_5numpy__util_dtypestring(__pyx_v_descr, (__pyx_v_info->format + 1), (__pyx_v_info->format + 0xFF), (&__pyx_v_offset)); if (unlikely(__pyx_t_7 == ((char *)NULL))) __PYX_ERR(1, 302, __pyx_L1_error)
     __pyx_v_f = __pyx_t_7;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":288
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":305
  *                                       info.format + _buffer_format_string_len,
  *                                       &offset)
  *                 f[0] = c'\0' # Terminate format string             # <<<<<<<<<<<<<<
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  */
     (__pyx_v_f[0]) = '\x00';
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":197
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":214
  *         # experimental exception made for __getbuffer__ and __releasebuffer__
  *         # -- the details of this may change.
  *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
  *             # This implementation of getbuffer is geared towards Cython
  *             # requirements, and does not yet fullfill the PEP.
  */
 
@@ -7456,20 +7568,20 @@
   }
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_descr);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":290
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":307
  *                 f[0] = c'\0' # Terminate format string
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
  *             if PyArray_HASFIELDS(self):
- *                 stdlib.free(info.format)
+ *                 PyObject_Free(info.format)
  */
 
 /* Python wrapper */
 static CYTHON_UNUSED void __pyx_pw_5numpy_7ndarray_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info); /*proto*/
 static CYTHON_UNUSED void __pyx_pw_5numpy_7ndarray_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__releasebuffer__ (wrapper)", 0);
@@ -7480,111 +7592,111 @@
 }
 
 static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__releasebuffer__", 0);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":291
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":308
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
- *                 stdlib.free(info.format)
+ *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  */
   __pyx_t_1 = (PyArray_HASFIELDS(__pyx_v_self) != 0);
   if (__pyx_t_1) {
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":292
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":309
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  *             if PyArray_HASFIELDS(self):
- *                 stdlib.free(info.format)             # <<<<<<<<<<<<<<
+ *                 PyObject_Free(info.format)             # <<<<<<<<<<<<<<
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 stdlib.free(info.strides)
+ *                 PyObject_Free(info.strides)
  */
-    free(__pyx_v_info->format);
+    PyObject_Free(__pyx_v_info->format);
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":291
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":308
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
- *                 stdlib.free(info.format)
+ *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  */
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":293
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":310
  *             if PyArray_HASFIELDS(self):
- *                 stdlib.free(info.format)
+ *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 stdlib.free(info.strides)
+ *                 PyObject_Free(info.strides)
  *                 # info.shape was stored after info.strides in the same block
  */
   __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
   if (__pyx_t_1) {
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":294
- *                 stdlib.free(info.format)
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":311
+ *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 stdlib.free(info.strides)             # <<<<<<<<<<<<<<
+ *                 PyObject_Free(info.strides)             # <<<<<<<<<<<<<<
  *                 # info.shape was stored after info.strides in the same block
  * 
  */
-    free(__pyx_v_info->strides);
+    PyObject_Free(__pyx_v_info->strides);
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":293
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":310
  *             if PyArray_HASFIELDS(self):
- *                 stdlib.free(info.format)
+ *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 stdlib.free(info.strides)
+ *                 PyObject_Free(info.strides)
  *                 # info.shape was stored after info.strides in the same block
  */
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":290
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":307
  *                 f[0] = c'\0' # Terminate format string
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
  *             if PyArray_HASFIELDS(self):
- *                 stdlib.free(info.format)
+ *                 PyObject_Free(info.format)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":770
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":788
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":771
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":789
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 771, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 789, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":770
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":788
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7595,43 +7707,43 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":773
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":791
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":774
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":792
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 774, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 792, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":773
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":791
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7642,43 +7754,43 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":776
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":794
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":777
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":795
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 795, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":776
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":794
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7689,43 +7801,43 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":779
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":797
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":780
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":798
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 798, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":779
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":797
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7736,43 +7848,43 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":782
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":800
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":783
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":801
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 801, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":782
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":800
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7783,17 +7895,91 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":785
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":803
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
+
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":804
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
+ *         return <tuple>d.subarray.shape
+ *     else:
+ */
+  __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
+  if (__pyx_t_1) {
+
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":805
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
+ *     else:
+ *         return ()
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
+    __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
+    goto __pyx_L0;
+
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":804
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
+ *         return <tuple>d.subarray.shape
+ *     else:
+ */
+  }
+
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":807
+ *         return <tuple>d.subarray.shape
+ *     else:
+ *         return ()             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:
+ */
+  /*else*/ {
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_INCREF(__pyx_empty_tuple);
+    __pyx_r = __pyx_empty_tuple;
+    goto __pyx_L0;
+  }
+
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":803
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":809
+ *         return ()
+ * 
  * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
  *     # Recursive utility function used in __getbuffer__ to get format
  *     # string. The new location in the format string is returned.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy__util_dtypestring(PyArray_Descr *__pyx_v_descr, char *__pyx_v_f, char *__pyx_v_end, int *__pyx_v_offset) {
   PyArray_Descr *__pyx_v_child = 0;
@@ -7812,73 +7998,73 @@
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_t_7;
   long __pyx_t_8;
   char *__pyx_t_9;
   __Pyx_RefNannySetupContext("_util_dtypestring", 0);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":790
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":814
  * 
  *     cdef dtype child
  *     cdef int endian_detector = 1             # <<<<<<<<<<<<<<
  *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
  *     cdef tuple fields
  */
   __pyx_v_endian_detector = 1;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":791
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":815
  *     cdef dtype child
  *     cdef int endian_detector = 1
  *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
  *     cdef tuple fields
  * 
  */
   __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":794
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":818
  *     cdef tuple fields
  * 
  *     for childname in descr.names:             # <<<<<<<<<<<<<<
  *         fields = descr.fields[childname]
  *         child, new_offset = fields
  */
   if (unlikely(__pyx_v_descr->names == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(1, 794, __pyx_L1_error)
+    __PYX_ERR(1, 818, __pyx_L1_error)
   }
   __pyx_t_1 = __pyx_v_descr->names; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
   for (;;) {
     if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 794, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 818, __pyx_L1_error)
     #else
-    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 794, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 818, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_childname, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":795
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":819
  * 
  *     for childname in descr.names:
  *         fields = descr.fields[childname]             # <<<<<<<<<<<<<<
  *         child, new_offset = fields
  * 
  */
     if (unlikely(__pyx_v_descr->fields == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 795, __pyx_L1_error)
+      __PYX_ERR(1, 819, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_descr->fields, __pyx_v_childname); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 795, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_descr->fields, __pyx_v_childname); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 819, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(PyTuple_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(1, 795, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(1, 819, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_fields, ((PyObject*)__pyx_t_3));
     __pyx_t_3 = 0;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":796
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":820
  *     for childname in descr.names:
  *         fields = descr.fields[childname]
  *         child, new_offset = fields             # <<<<<<<<<<<<<<
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:
  */
     if (likely(__pyx_v_fields != Py_None)) {
@@ -7887,76 +8073,76 @@
       Py_ssize_t size = Py_SIZE(sequence);
       #else
       Py_ssize_t size = PySequence_Size(sequence);
       #endif
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(1, 796, __pyx_L1_error)
+        __PYX_ERR(1, 820, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       #else
-      __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 796, __pyx_L1_error)
+      __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 820, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 796, __pyx_L1_error)
+      __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 820, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       #endif
     } else {
-      __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 796, __pyx_L1_error)
+      __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 820, __pyx_L1_error)
     }
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_dtype))))) __PYX_ERR(1, 796, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_dtype))))) __PYX_ERR(1, 820, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_child, ((PyArray_Descr *)__pyx_t_3));
     __pyx_t_3 = 0;
     __Pyx_XDECREF_SET(__pyx_v_new_offset, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":798
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":822
  *         child, new_offset = fields
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  */
-    __pyx_t_4 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 798, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 822, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = PyNumber_Subtract(__pyx_v_new_offset, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 798, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Subtract(__pyx_v_new_offset, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 822, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 798, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 822, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_6 = ((((__pyx_v_end - __pyx_v_f) - ((int)__pyx_t_5)) < 15) != 0);
     if (__pyx_t_6) {
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":799
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":823
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
  * 
  *         if ((child.byteorder == c'>' and little_endian) or
  */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 799, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 823, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 799, __pyx_L1_error)
+      __PYX_ERR(1, 823, __pyx_L1_error)
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":798
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":822
  *         child, new_offset = fields
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  */
     }
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":801
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":825
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")
  */
     __pyx_t_7 = ((__pyx_v_child->byteorder == '>') != 0);
@@ -7968,15 +8154,15 @@
     if (!__pyx_t_7) {
     } else {
       __pyx_t_6 = __pyx_t_7;
       goto __pyx_L7_bool_binop_done;
     }
     __pyx_L8_next_or:;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":802
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":826
  * 
  *         if ((child.byteorder == c'>' and little_endian) or
  *             (child.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
  *             raise ValueError(u"Non-native byte order not supported")
  *             # One could encode it in the format string and have Cython
  */
     __pyx_t_7 = ((__pyx_v_child->byteorder == '<') != 0);
@@ -7985,544 +8171,544 @@
       __pyx_t_6 = __pyx_t_7;
       goto __pyx_L7_bool_binop_done;
     }
     __pyx_t_7 = ((!(__pyx_v_little_endian != 0)) != 0);
     __pyx_t_6 = __pyx_t_7;
     __pyx_L7_bool_binop_done:;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":801
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":825
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")
  */
     if (__pyx_t_6) {
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":803
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":827
  *         if ((child.byteorder == c'>' and little_endian) or
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
  *             # One could encode it in the format string and have Cython
  *             # complain instead, BUT: < and > in format strings also imply
  */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 803, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 827, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 803, __pyx_L1_error)
+      __PYX_ERR(1, 827, __pyx_L1_error)
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":801
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":825
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")
  */
     }
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":813
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":837
  * 
  *         # Output padding bytes
  *         while offset[0] < new_offset:             # <<<<<<<<<<<<<<
  *             f[0] = 120 # "x"; pad byte
  *             f += 1
  */
     while (1) {
-      __pyx_t_3 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 813, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 837, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_new_offset, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 813, __pyx_L1_error)
+      __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_new_offset, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 837, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 813, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 837, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (!__pyx_t_6) break;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":814
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":838
  *         # Output padding bytes
  *         while offset[0] < new_offset:
  *             f[0] = 120 # "x"; pad byte             # <<<<<<<<<<<<<<
  *             f += 1
  *             offset[0] += 1
  */
       (__pyx_v_f[0]) = 0x78;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":815
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":839
  *         while offset[0] < new_offset:
  *             f[0] = 120 # "x"; pad byte
  *             f += 1             # <<<<<<<<<<<<<<
  *             offset[0] += 1
  * 
  */
       __pyx_v_f = (__pyx_v_f + 1);
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":816
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":840
  *             f[0] = 120 # "x"; pad byte
  *             f += 1
  *             offset[0] += 1             # <<<<<<<<<<<<<<
  * 
  *         offset[0] += child.itemsize
  */
       __pyx_t_8 = 0;
       (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + 1);
     }
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":818
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":842
  *             offset[0] += 1
  * 
  *         offset[0] += child.itemsize             # <<<<<<<<<<<<<<
  * 
  *         if not PyDataType_HASFIELDS(child):
  */
     __pyx_t_8 = 0;
     (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + __pyx_v_child->elsize);
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":820
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":844
  *         offset[0] += child.itemsize
  * 
  *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
  *             t = child.type_num
  *             if end - f < 5:
  */
     __pyx_t_6 = ((!(PyDataType_HASFIELDS(__pyx_v_child) != 0)) != 0);
     if (__pyx_t_6) {
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":821
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":845
  * 
  *         if not PyDataType_HASFIELDS(child):
  *             t = child.type_num             # <<<<<<<<<<<<<<
  *             if end - f < 5:
  *                 raise RuntimeError(u"Format string allocated too short.")
  */
-      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_child->type_num); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 821, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_child->type_num); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 845, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_XDECREF_SET(__pyx_v_t, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":822
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":846
  *         if not PyDataType_HASFIELDS(child):
  *             t = child.type_num
  *             if end - f < 5:             # <<<<<<<<<<<<<<
  *                 raise RuntimeError(u"Format string allocated too short.")
  * 
  */
       __pyx_t_6 = (((__pyx_v_end - __pyx_v_f) < 5) != 0);
       if (__pyx_t_6) {
 
-        /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":823
+        /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":847
  *             t = child.type_num
  *             if end - f < 5:
  *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
  * 
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  */
-        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 823, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 847, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_Raise(__pyx_t_4, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __PYX_ERR(1, 823, __pyx_L1_error)
+        __PYX_ERR(1, 847, __pyx_L1_error)
 
-        /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":822
+        /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":846
  *         if not PyDataType_HASFIELDS(child):
  *             t = child.type_num
  *             if end - f < 5:             # <<<<<<<<<<<<<<
  *                 raise RuntimeError(u"Format string allocated too short.")
  * 
  */
       }
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":826
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":850
  * 
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  *             if   t == NPY_BYTE:        f[0] =  98 #"b"             # <<<<<<<<<<<<<<
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_BYTE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 826, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_BYTE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 850, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 826, __pyx_L1_error)
+      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 850, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 826, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 850, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 98;
         goto __pyx_L15;
       }
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":827
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":851
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  *             if   t == NPY_BYTE:        f[0] =  98 #"b"
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"             # <<<<<<<<<<<<<<
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UBYTE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 827, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UBYTE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 851, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 827, __pyx_L1_error)
+      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 851, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 827, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 851, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 66;
         goto __pyx_L15;
       }
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":828
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":852
  *             if   t == NPY_BYTE:        f[0] =  98 #"b"
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"             # <<<<<<<<<<<<<<
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_SHORT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 828, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_SHORT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 852, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 828, __pyx_L1_error)
+      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 852, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 828, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 852, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x68;
         goto __pyx_L15;
       }
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":829
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":853
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"             # <<<<<<<<<<<<<<
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_USHORT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 829, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_USHORT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 853, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 829, __pyx_L1_error)
+      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 853, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 829, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 853, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 72;
         goto __pyx_L15;
       }
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":830
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":854
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  *             elif t == NPY_INT:         f[0] = 105 #"i"             # <<<<<<<<<<<<<<
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_INT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 830, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_INT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 854, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 830, __pyx_L1_error)
+      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 854, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 830, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 854, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x69;
         goto __pyx_L15;
       }
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":831
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":855
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  *             elif t == NPY_UINT:        f[0] =  73 #"I"             # <<<<<<<<<<<<<<
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UINT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 831, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UINT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 855, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 831, __pyx_L1_error)
+      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 855, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 831, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 855, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 73;
         goto __pyx_L15;
       }
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":832
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":856
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  *             elif t == NPY_LONG:        f[0] = 108 #"l"             # <<<<<<<<<<<<<<
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 832, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 856, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 832, __pyx_L1_error)
+      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 856, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 832, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 856, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x6C;
         goto __pyx_L15;
       }
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":833
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":857
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"             # <<<<<<<<<<<<<<
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 833, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 857, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 833, __pyx_L1_error)
+      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 857, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 833, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 857, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 76;
         goto __pyx_L15;
       }
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":834
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":858
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"             # <<<<<<<<<<<<<<
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGLONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 834, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGLONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 858, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 834, __pyx_L1_error)
+      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 858, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 834, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 858, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x71;
         goto __pyx_L15;
       }
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":835
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":859
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"             # <<<<<<<<<<<<<<
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONGLONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 835, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONGLONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 859, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 835, __pyx_L1_error)
+      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 859, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 835, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 859, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 81;
         goto __pyx_L15;
       }
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":836
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":860
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"             # <<<<<<<<<<<<<<
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_FLOAT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 836, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_FLOAT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 860, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 836, __pyx_L1_error)
+      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 860, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 836, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 860, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x66;
         goto __pyx_L15;
       }
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":837
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":861
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"             # <<<<<<<<<<<<<<
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_DOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 837, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_DOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 861, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 837, __pyx_L1_error)
+      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 861, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 837, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 861, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x64;
         goto __pyx_L15;
       }
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":838
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":862
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"             # <<<<<<<<<<<<<<
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 838, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 862, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 838, __pyx_L1_error)
+      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 862, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 838, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 862, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x67;
         goto __pyx_L15;
       }
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":839
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":863
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf             # <<<<<<<<<<<<<<
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
  */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CFLOAT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 839, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CFLOAT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 863, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 839, __pyx_L1_error)
+      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 863, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 839, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 863, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 90;
         (__pyx_v_f[1]) = 0x66;
         __pyx_v_f = (__pyx_v_f + 1);
         goto __pyx_L15;
       }
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":840
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":864
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd             # <<<<<<<<<<<<<<
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
  */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 840, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 864, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 840, __pyx_L1_error)
+      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 864, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 840, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 864, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 90;
         (__pyx_v_f[1]) = 0x64;
         __pyx_v_f = (__pyx_v_f + 1);
         goto __pyx_L15;
       }
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":841
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":865
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg             # <<<<<<<<<<<<<<
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
  *             else:
  */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CLONGDOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 841, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CLONGDOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 865, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 841, __pyx_L1_error)
+      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 865, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 841, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 865, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 90;
         (__pyx_v_f[1]) = 0x67;
         __pyx_v_f = (__pyx_v_f + 1);
         goto __pyx_L15;
       }
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":842
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":866
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"             # <<<<<<<<<<<<<<
  *             else:
  *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_OBJECT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 842, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_OBJECT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 866, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 842, __pyx_L1_error)
+      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 866, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 842, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 866, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 79;
         goto __pyx_L15;
       }
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":844
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":868
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
  *             else:
  *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
  *             f += 1
  *         else:
  */
       /*else*/ {
-        __pyx_t_3 = PyUnicode_Format(__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 844, __pyx_L1_error)
+        __pyx_t_3 = PyUnicode_Format(__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 868, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 844, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 868, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_GIVEREF(__pyx_t_3);
         PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
         __pyx_t_3 = 0;
-        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 844, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 868, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_Raise(__pyx_t_3, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __PYX_ERR(1, 844, __pyx_L1_error)
+        __PYX_ERR(1, 868, __pyx_L1_error)
       }
       __pyx_L15:;
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":845
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":869
  *             else:
  *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  *             f += 1             # <<<<<<<<<<<<<<
  *         else:
  *             # Cython ignores struct boundary information ("T{...}"),
  */
       __pyx_v_f = (__pyx_v_f + 1);
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":820
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":844
  *         offset[0] += child.itemsize
  * 
  *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
  *             t = child.type_num
  *             if end - f < 5:
  */
       goto __pyx_L13;
     }
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":849
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":873
  *             # Cython ignores struct boundary information ("T{...}"),
  *             # so don't output it
  *             f = _util_dtypestring(child, f, end, offset)             # <<<<<<<<<<<<<<
  *     return f
  * 
  */
     /*else*/ {
-      __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_child, __pyx_v_f, __pyx_v_end, __pyx_v_offset); if (unlikely(__pyx_t_9 == NULL)) __PYX_ERR(1, 849, __pyx_L1_error)
+      __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_child, __pyx_v_f, __pyx_v_end, __pyx_v_offset); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(1, 873, __pyx_L1_error)
       __pyx_v_f = __pyx_t_9;
     }
     __pyx_L13:;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":794
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":818
  *     cdef tuple fields
  * 
  *     for childname in descr.names:             # <<<<<<<<<<<<<<
  *         fields = descr.fields[childname]
  *         child, new_offset = fields
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":850
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":874
  *             # so don't output it
  *             f = _util_dtypestring(child, f, end, offset)
  *     return f             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_f;
   goto __pyx_L0;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":785
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":809
+ *         return ()
  * 
  * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
  *     # Recursive utility function used in __getbuffer__ to get format
  *     # string. The new location in the format string is returned.
  */
 
   /* function exit code */
@@ -8538,185 +8724,185 @@
   __Pyx_XDECREF(__pyx_v_childname);
   __Pyx_XDECREF(__pyx_v_new_offset);
   __Pyx_XDECREF(__pyx_v_t);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":966
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":990
  * 
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *      cdef PyObject* baseptr
  *      if base is None:
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   PyObject *__pyx_v_baseptr;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":968
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":992
  * cdef inline void set_array_base(ndarray arr, object base):
  *      cdef PyObject* baseptr
  *      if base is None:             # <<<<<<<<<<<<<<
  *          baseptr = NULL
  *      else:
  */
   __pyx_t_1 = (__pyx_v_base == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":969
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":993
  *      cdef PyObject* baseptr
  *      if base is None:
  *          baseptr = NULL             # <<<<<<<<<<<<<<
  *      else:
  *          Py_INCREF(base) # important to do this before decref below!
  */
     __pyx_v_baseptr = NULL;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":968
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":992
  * cdef inline void set_array_base(ndarray arr, object base):
  *      cdef PyObject* baseptr
  *      if base is None:             # <<<<<<<<<<<<<<
  *          baseptr = NULL
  *      else:
  */
     goto __pyx_L3;
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":971
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":995
  *          baseptr = NULL
  *      else:
  *          Py_INCREF(base) # important to do this before decref below!             # <<<<<<<<<<<<<<
  *          baseptr = <PyObject*>base
  *      Py_XDECREF(arr.base)
  */
   /*else*/ {
     Py_INCREF(__pyx_v_base);
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":972
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":996
  *      else:
  *          Py_INCREF(base) # important to do this before decref below!
  *          baseptr = <PyObject*>base             # <<<<<<<<<<<<<<
  *      Py_XDECREF(arr.base)
  *      arr.base = baseptr
  */
     __pyx_v_baseptr = ((PyObject *)__pyx_v_base);
   }
   __pyx_L3:;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":973
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":997
  *          Py_INCREF(base) # important to do this before decref below!
  *          baseptr = <PyObject*>base
  *      Py_XDECREF(arr.base)             # <<<<<<<<<<<<<<
  *      arr.base = baseptr
  * 
  */
   Py_XDECREF(__pyx_v_arr->base);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":974
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":998
  *          baseptr = <PyObject*>base
  *      Py_XDECREF(arr.base)
  *      arr.base = baseptr             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_v_arr->base = __pyx_v_baseptr;
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":966
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":990
  * 
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *      cdef PyObject* baseptr
  *      if base is None:
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":976
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1000
  *      arr.base = baseptr
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     if arr.base is NULL:
  *         return None
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":977
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1001
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     if arr.base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_arr->base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":978
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1002
  * cdef inline object get_array_base(ndarray arr):
  *     if arr.base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     else:
  *         return <object>arr.base
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_None);
     __pyx_r = Py_None;
     goto __pyx_L0;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":977
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1001
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     if arr.base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     else:
  */
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":980
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1004
  *         return None
  *     else:
  *         return <object>arr.base             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_arr->base));
     __pyx_r = ((PyObject *)__pyx_v_arr->base);
     goto __pyx_L0;
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":976
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1000
  *      arr.base = baseptr
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     if arr.base is NULL:
  *         return None
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":985
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1009
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_array()
  */
 
@@ -8729,15 +8915,15 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":986
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1010
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_array()
  *     except Exception:
  */
   {
@@ -8745,86 +8931,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":987
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1011
  * cdef inline int import_array() except -1:
  *     try:
  *         _import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == -1)) __PYX_ERR(1, 987, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1011, __pyx_L3_error)
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":986
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1010
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
-    __Pyx_PyThreadState_assign
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":988
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1012
  *     try:
  *         _import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 988, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1012, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":989
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1013
  *         _import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 989, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1013, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 989, __pyx_L5_except_error)
+      __PYX_ERR(1, 1013, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":986
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1010
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_array()
  *     except Exception:
  */
-    __Pyx_PyThreadState_assign
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":985
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1009
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_array()
  */
 
@@ -8839,15 +9023,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":991
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1015
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8860,15 +9044,15 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":992
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1016
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -8876,86 +9060,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":993
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1017
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == -1)) __PYX_ERR(1, 993, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1017, __pyx_L3_error)
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":992
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1016
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
-    __Pyx_PyThreadState_assign
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":994
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1018
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 994, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1018, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":995
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1019
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 995, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1019, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 995, __pyx_L5_except_error)
+      __PYX_ERR(1, 1019, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":992
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1016
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
-    __Pyx_PyThreadState_assign
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":991
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1015
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8970,15 +9152,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":997
+/* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1021
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8991,15 +9173,15 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":998
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1022
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -9007,83 +9189,81 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":999
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1023
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == -1)) __PYX_ERR(1, 999, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1023, __pyx_L3_error)
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":998
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1022
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
-    __Pyx_PyThreadState_assign
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":1000
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1024
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1000, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1024, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":1001
+      /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1025
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__37, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1001, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__37, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1025, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1001, __pyx_L5_except_error)
+      __PYX_ERR(1, 1025, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":998
+    /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1022
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
-    __Pyx_PyThreadState_assign
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":997
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1021
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -9358,15 +9538,15 @@
   /* "map.to_py":202
  * @cname("__pyx_convert_unordered_map_to_py_std_3a__3a_string____int")
  * cdef object __pyx_convert_unordered_map_to_py_std_3a__3a_string____int(const map[X,Y]& s):
  *     o = {}             # <<<<<<<<<<<<<<
  *     cdef const map[X,Y].value_type *key_value
  *     cdef map[X,Y].const_iterator iter = s.begin()
  */
-  __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_o = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "map.to_py":204
  *     o = {}
  *     cdef const map[X,Y].value_type *key_value
@@ -9468,15 +9648,15 @@
   /* "map.to_py":202
  * @cname("__pyx_convert_unordered_map_to_py_std_3a__3a_string____double")
  * cdef object __pyx_convert_unordered_map_to_py_std_3a__3a_string____double(const map[X,Y]& s):
  *     o = {}             # <<<<<<<<<<<<<<
  *     cdef const map[X,Y].value_type *key_value
  *     cdef map[X,Y].const_iterator iter = s.begin()
  */
-  __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_o = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "map.to_py":204
  *     o = {}
  *     cdef const map[X,Y].value_type *key_value
@@ -9646,15 +9826,15 @@
   /* "map.to_py":202
  * @cname("__pyx_convert_unordered_map_to_py_std_3a__3a_string____std_3a__3a_vector_3c_double_3e___")
  * cdef object __pyx_convert_unordered_map_to_py_std_3a__3a_string____std_3a__3a_vector_3c_double_3e___(const map[X,Y]& s):
  *     o = {}             # <<<<<<<<<<<<<<
  *     cdef const map[X,Y].value_type *key_value
  *     cdef map[X,Y].const_iterator iter = s.begin()
  */
-  __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_o = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "map.to_py":204
  *     o = {}
  *     cdef const map[X,Y].value_type *key_value
@@ -9824,15 +10004,15 @@
   /* "map.to_py":202
  * @cname("__pyx_convert_unordered_map_to_py_std_3a__3a_string____std_3a__3a_vector_3c_int_3e___")
  * cdef object __pyx_convert_unordered_map_to_py_std_3a__3a_string____std_3a__3a_vector_3c_int_3e___(const map[X,Y]& s):
  *     o = {}             # <<<<<<<<<<<<<<
  *     cdef const map[X,Y].value_type *key_value
  *     cdef map[X,Y].const_iterator iter = s.begin()
  */
-  __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_o = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "map.to_py":204
  *     o = {}
  *     cdef const map[X,Y].value_type *key_value
@@ -9939,15 +10119,15 @@
   /* "string.from_py":15
  * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:
  *     cdef Py_ssize_t length
  *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)             # <<<<<<<<<<<<<<
  *     return string(data, length)
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_AsStringAndSize(__pyx_v_o, (&__pyx_v_length)); if (unlikely(__pyx_t_1 == NULL)) __PYX_ERR(2, 15, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_AsStringAndSize(__pyx_v_o, (&__pyx_v_length)); if (unlikely(__pyx_t_1 == ((char const *)NULL))) __PYX_ERR(2, 15, __pyx_L1_error)
   __pyx_v_data = __pyx_t_1;
 
   /* "string.from_py":16
  *     cdef Py_ssize_t length
  *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
  *     return string(data, length)             # <<<<<<<<<<<<<<
  * 
@@ -9974,25 +10154,39 @@
 }
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
+#if CYTHON_PEP489_MULTI_PHASE_INIT
+static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
+static int __pyx_pymod_exec__cvodes(PyObject* module); /*proto*/
+static PyModuleDef_Slot __pyx_moduledef_slots[] = {
+  {Py_mod_create, (void*)__pyx_pymod_create},
+  {Py_mod_exec, (void*)__pyx_pymod_exec__cvodes},
+  {0, NULL}
+};
+#endif
+
 static struct PyModuleDef __pyx_moduledef = {
-  #if PY_VERSION_HEX < 0x03020000
-    { PyObject_HEAD_INIT(NULL) NULL, 0, NULL },
-  #else
     PyModuleDef_HEAD_INIT,
-  #endif
     "_cvodes",
     0, /* m_doc */
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+    0, /* m_size */
+  #else
     -1, /* m_size */
+  #endif
     __pyx_methods /* m_methods */,
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+    __pyx_moduledef_slots, /* m_slots */
+  #else
     NULL, /* m_reload */
+  #endif
     NULL, /* m_traverse */
     NULL, /* m_clear */
     NULL /* m_free */
 };
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
@@ -10117,16 +10311,16 @@
   {&__pyx_n_s_yout, __pyx_k_yout, sizeof(__pyx_k_yout), 0, 0, 1, 1},
   {&__pyx_n_s_yout_shape, __pyx_k_yout_shape, sizeof(__pyx_k_yout_shape), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 73, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 78, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(1, 799, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 989, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(1, 823, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 1013, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -10380,108 +10574,108 @@
  *             linear_solver, maxl, eps_lin, nderiv, autorestart, return_on_error)
  *         info = get_last_info(odesys, success=False if return_on_error and nreached < xout.size else True)
  */
   __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_UTF_8); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":218
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":235
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  */
-  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_C_contiguous); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 218, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_C_contiguous); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 235, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__29);
   __Pyx_GIVEREF(__pyx_tuple__29);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":222
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":239
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
  * 
  *             info.buf = PyArray_DATA(self)
  */
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_Fortran_contiguou); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_Fortran_contiguou); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(1, 239, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__30);
   __Pyx_GIVEREF(__pyx_tuple__30);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":259
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":276
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"
  */
-  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_u_Non_native_byte_order_not_suppor); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(1, 259, __pyx_L1_error)
+  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_u_Non_native_byte_order_not_suppor); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(1, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__31);
   __Pyx_GIVEREF(__pyx_tuple__31);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":799
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":823
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
  * 
  *         if ((child.byteorder == c'>' and little_endian) or
  */
-  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(1, 799, __pyx_L1_error)
+  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(1, 823, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__32);
   __Pyx_GIVEREF(__pyx_tuple__32);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":803
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":827
  *         if ((child.byteorder == c'>' and little_endian) or
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
  *             # One could encode it in the format string and have Cython
  *             # complain instead, BUT: < and > in format strings also imply
  */
-  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_u_Non_native_byte_order_not_suppor); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 803, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_u_Non_native_byte_order_not_suppor); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 827, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":823
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":847
  *             t = child.type_num
  *             if end - f < 5:
  *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
  * 
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  */
-  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor_2); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(1, 823, __pyx_L1_error)
+  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor_2); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(1, 847, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__34);
   __Pyx_GIVEREF(__pyx_tuple__34);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":989
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1013
  *         _import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(1, 989, __pyx_L1_error)
+  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(1, 1013, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__35);
   __Pyx_GIVEREF(__pyx_tuple__35);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":995
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1019
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(1, 995, __pyx_L1_error)
+  __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(1, 1019, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__36);
   __Pyx_GIVEREF(__pyx_tuple__36);
 
-  /* "../../.local/lib/python2.7/site-packages/Cython/Includes/numpy/__init__.pxd":1001
+  /* "../../../../opt/miniconda3/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1025
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__37 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(1, 1001, __pyx_L1_error)
+  __pyx_tuple__37 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(1, 1025, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__37);
   __Pyx_GIVEREF(__pyx_tuple__37);
 
   /* "pycvodes/_cvodes.pyx":23
  * cnp.import_array()  # Numpy C-API initialization
  * 
  * steppers = ('adams', 'bdf')             # <<<<<<<<<<<<<<
@@ -10520,27 +10714,27 @@
  * def adaptive(rhs, jac, cnp.ndarray[cnp.float64_t, mode='c'] y0, double x0, double xend, atol,             # <<<<<<<<<<<<<<
  *              double rtol, str method='bdf', int nsteps=500, double dx0=0.0, double dx_min=0.0,
  *              double dx_max=0.0, roots=None, cb_kwargs=None, int lband=-1, int uband=-1, int nroots=0,
  */
   __pyx_tuple__41 = PyTuple_Pack(51, __pyx_n_s_rhs, __pyx_n_s_jac, __pyx_n_s_y0, __pyx_n_s_x0, __pyx_n_s_xend, __pyx_n_s_atol, __pyx_n_s_rtol, __pyx_n_s_method, __pyx_n_s_nsteps, __pyx_n_s_dx0, __pyx_n_s_dx_min, __pyx_n_s_dx_max, __pyx_n_s_roots, __pyx_n_s_cb_kwargs, __pyx_n_s_lband, __pyx_n_s_uband, __pyx_n_s_nroots, __pyx_n_s_iter_type, __pyx_n_s_linear_solver, __pyx_n_s_maxl, __pyx_n_s_eps_lin, __pyx_n_s_nderiv, __pyx_n_s_return_on_root, __pyx_n_s_autorestart, __pyx_n_s_return_on_error, __pyx_n_s_record_rhs_xvals, __pyx_n_s_record_jac_xvals, __pyx_n_s_record_order, __pyx_n_s_record_fpe, __pyx_n_s_record_steps, __pyx_n_s_dx0cb, __pyx_n_s_dx_max_cb, __pyx_n_s_autonomous_exprs, __pyx_n_s_nprealloc, __pyx_n_s_ny, __pyx_n_s_with_jacobian, __pyx_n_s_odesys, __pyx_n_s_root_indices, __pyx_n_s_atol_vec, __pyx_n_s_td, __pyx_n_s_xyout, __pyx_n_s_xyout_arr, __pyx_n_s_xyout_dims, __pyx_n_s_nout, __pyx_n_s_at, __pyx_n_s_i, __pyx_n_s_xout, __pyx_n_s_yout, __pyx_n_s_success, __pyx_n_s_info, __pyx_n_s_yout_shape); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__41);
   __Pyx_GIVEREF(__pyx_tuple__41);
-  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(34, 0, 51, 0, 0, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pycvodes__cvodes_pyx, __pyx_n_s_adaptive, 46, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(34, 0, 51, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pycvodes__cvodes_pyx, __pyx_n_s_adaptive, 46, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 46, __pyx_L1_error)
 
   /* "pycvodes/_cvodes.pyx":122
  * 
  * 
  * def predefined(rhs, jac,             # <<<<<<<<<<<<<<
  *                cnp.ndarray[cnp.float64_t, mode='c'] y0,
  *                cnp.ndarray[cnp.float64_t, ndim=1] xout, atol,
  */
   __pyx_tuple__43 = PyTuple_Pack(42, __pyx_n_s_rhs, __pyx_n_s_jac, __pyx_n_s_y0, __pyx_n_s_xout, __pyx_n_s_atol, __pyx_n_s_rtol, __pyx_n_s_method, __pyx_n_s_nsteps, __pyx_n_s_dx0, __pyx_n_s_dx_min, __pyx_n_s_dx_max, __pyx_n_s_roots, __pyx_n_s_cb_kwargs, __pyx_n_s_lband, __pyx_n_s_uband, __pyx_n_s_nroots, __pyx_n_s_iter_type, __pyx_n_s_linear_solver, __pyx_n_s_maxl, __pyx_n_s_eps_lin, __pyx_n_s_nderiv, __pyx_n_s_return_on_root, __pyx_n_s_autorestart, __pyx_n_s_return_on_error, __pyx_n_s_record_rhs_xvals, __pyx_n_s_record_jac_xvals, __pyx_n_s_record_order, __pyx_n_s_record_fpe, __pyx_n_s_record_steps, __pyx_n_s_dx0cb, __pyx_n_s_dx_max_cb, __pyx_n_s_autonomous_exprs, __pyx_n_s_ny, __pyx_n_s_yout, __pyx_n_s_with_jacobian, __pyx_n_s_nreached, __pyx_n_s_odesys, __pyx_n_s_root_indices, __pyx_n_s_roots_output, __pyx_n_s_atol_vec, __pyx_n_s_at, __pyx_n_s_info); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__43);
   __Pyx_GIVEREF(__pyx_tuple__43);
-  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(32, 0, 42, 0, 0, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pycvodes__cvodes_pyx, __pyx_n_s_predefined, 122, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(32, 0, 42, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pycvodes__cvodes_pyx, __pyx_n_s_predefined, 122, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -10560,25 +10754,69 @@
 
 #if PY_MAJOR_VERSION < 3
 PyMODINIT_FUNC init_cvodes(void); /*proto*/
 PyMODINIT_FUNC init_cvodes(void)
 #else
 PyMODINIT_FUNC PyInit__cvodes(void); /*proto*/
 PyMODINIT_FUNC PyInit__cvodes(void)
+#if CYTHON_PEP489_MULTI_PHASE_INIT
+{
+  return PyModuleDef_Init(&__pyx_moduledef);
+}
+static int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name) {
+    PyObject *value = PyObject_GetAttrString(spec, from_name);
+    int result = 0;
+    if (likely(value)) {
+        result = PyDict_SetItemString(moddict, to_name, value);
+        Py_DECREF(value);
+    } else if (PyErr_ExceptionMatches(PyExc_AttributeError)) {
+        PyErr_Clear();
+    } else {
+        result = -1;
+    }
+    return result;
+}
+static PyObject* __pyx_pymod_create(PyObject *spec, CYTHON_UNUSED PyModuleDef *def) {
+    PyObject *module = NULL, *moddict, *modname;
+    if (__pyx_m)
+        return __Pyx_NewRef(__pyx_m);
+    modname = PyObject_GetAttrString(spec, "name");
+    if (unlikely(!modname)) goto bad;
+    module = PyModule_NewObject(modname);
+    Py_DECREF(modname);
+    if (unlikely(!module)) goto bad;
+    moddict = PyModule_GetDict(module);
+    if (unlikely(!moddict)) goto bad;
+    if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "loader", "__loader__") < 0)) goto bad;
+    if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "origin", "__file__") < 0)) goto bad;
+    if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "parent", "__package__") < 0)) goto bad;
+    if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "submodule_search_locations", "__path__") < 0)) goto bad;
+    return module;
+bad:
+    Py_XDECREF(module);
+    return NULL;
+}
+
+
+static int __pyx_pymod_exec__cvodes(PyObject *__pyx_pyinit_module)
+#endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   __Pyx_RefNannyDeclarations
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+  if (__pyx_m && __pyx_m == __pyx_pyinit_module) return 0;
+  #endif
   #if CYTHON_REFNANNY
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
   if (!__Pyx_RefNanny) {
       PyErr_Clear();
       __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
       if (!__Pyx_RefNanny)
           Py_FatalError("failed to import 'refnanny' module");
@@ -10597,31 +10835,39 @@
   #endif
   #ifdef __Pyx_Coroutine_USED
   if (__pyx_Coroutine_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Generator_USED
   if (__pyx_Generator_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
+  #ifdef __Pyx_AsyncGen_USED
+  if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  #endif
   #ifdef __Pyx_StopAsyncIteration_USED
   if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
   #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   #ifdef WITH_THREAD /* Python build with threading support? */
   PyEval_InitThreads();
   #endif
   #endif
   /*--- Module creation code ---*/
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+  __pyx_m = __pyx_pyinit_module;
+  Py_INCREF(__pyx_m);
+  #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("_cvodes", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   #endif
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_COMPILING_IN_PYPY
   Py_INCREF(__pyx_b);
   #endif
@@ -10643,30 +10889,32 @@
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global init code ---*/
+  __pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_k = Py_None; Py_INCREF(Py_None);
+  __pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_v = Py_None; Py_INCREF(Py_None);
   /*--- Variable export code ---*/
   /*--- Function export code ---*/
   /*--- Type init code ---*/
   /*--- Type import code ---*/
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__Pyx_BUILTIN_MODULE_NAME, "type", 
   #if CYTHON_COMPILING_IN_PYPY
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   0); if (unlikely(!__pyx_ptype_7cpython_4type_type)) __PYX_ERR(3, 9, __pyx_L1_error)
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType("numpy", "dtype", sizeof(PyArray_Descr), 0); if (unlikely(!__pyx_ptype_5numpy_dtype)) __PYX_ERR(1, 155, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType("numpy", "flatiter", sizeof(PyArrayIterObject), 0); if (unlikely(!__pyx_ptype_5numpy_flatiter)) __PYX_ERR(1, 168, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType("numpy", "broadcast", sizeof(PyArrayMultiIterObject), 0); if (unlikely(!__pyx_ptype_5numpy_broadcast)) __PYX_ERR(1, 172, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType("numpy", "ndarray", sizeof(PyArrayObject), 0); if (unlikely(!__pyx_ptype_5numpy_ndarray)) __PYX_ERR(1, 181, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType("numpy", "ufunc", sizeof(PyUFuncObject), 0); if (unlikely(!__pyx_ptype_5numpy_ufunc)) __PYX_ERR(1, 861, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType("numpy", "dtype", sizeof(PyArray_Descr), 0); if (unlikely(!__pyx_ptype_5numpy_dtype)) __PYX_ERR(1, 163, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType("numpy", "flatiter", sizeof(PyArrayIterObject), 0); if (unlikely(!__pyx_ptype_5numpy_flatiter)) __PYX_ERR(1, 185, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType("numpy", "broadcast", sizeof(PyArrayMultiIterObject), 0); if (unlikely(!__pyx_ptype_5numpy_broadcast)) __PYX_ERR(1, 189, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType("numpy", "ndarray", sizeof(PyArrayObject), 0); if (unlikely(!__pyx_ptype_5numpy_ndarray)) __PYX_ERR(1, 198, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType("numpy", "ufunc", sizeof(PyUFuncObject), 0); if (unlikely(!__pyx_ptype_5numpy_ufunc)) __PYX_ERR(1, 885, __pyx_L1_error)
   /*--- Variable import code ---*/
   /*--- Function import code ---*/
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
@@ -10697,15 +10945,15 @@
   /* "pycvodes/_cvodes.pyx":21
  *     void PyArray_ENABLEFLAGS(cnp.ndarray arr, int flags)
  * 
  * cnp.import_array()  # Numpy C-API initialization             # <<<<<<<<<<<<<<
  * 
  * steppers = ('adams', 'bdf')
  */
-  __pyx_t_2 = __pyx_f_5numpy_import_array(); if (unlikely(__pyx_t_2 == -1)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_5numpy_import_array(); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 21, __pyx_L1_error)
 
   /* "pycvodes/_cvodes.pyx":23
  * cnp.import_array()  # Numpy C-API initialization
  * 
  * steppers = ('adams', 'bdf')             # <<<<<<<<<<<<<<
  * requires_jac = ('bdf',)
  * 
@@ -10724,30 +10972,30 @@
   /* "pycvodes/_cvodes.pyx":26
  * requires_jac = ('bdf',)
  * 
  * iter_types = {'default': 0, 'functional': 1, 'newton': 2}  # grep "define CV_FUNCTIONAL" cvodes.h             # <<<<<<<<<<<<<<
  * linear_solvers = {'default': 0, 'dense': 1, 'banded': 2, 'gmres': 10, 'gmres_classic': 11, 'bicgstab': 20, 'tfqmr': 30}
  * 
  */
-  __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_default, __pyx_int_0) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_functional, __pyx_int_1) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_newton, __pyx_int_2) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_iter_types, __pyx_t_1) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pycvodes/_cvodes.pyx":27
  * 
  * iter_types = {'default': 0, 'functional': 1, 'newton': 2}  # grep "define CV_FUNCTIONAL" cvodes.h
  * linear_solvers = {'default': 0, 'dense': 1, 'banded': 2, 'gmres': 10, 'gmres_classic': 11, 'bicgstab': 20, 'tfqmr': 30}             # <<<<<<<<<<<<<<
  * 
  * fpes = {str(k.decode('utf-8')): v for k, v in dict(_fpes).items()}
  */
-  __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_default, __pyx_int_0) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dense, __pyx_int_1) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_banded, __pyx_int_2) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_gmres, __pyx_int_10) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_gmres_classic, __pyx_int_11) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_bicgstab, __pyx_int_20) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
@@ -10759,16 +11007,14 @@
  * linear_solvers = {'default': 0, 'dense': 1, 'banded': 2, 'gmres': 10, 'gmres_classic': 11, 'bicgstab': 20, 'tfqmr': 30}
  * 
  * fpes = {str(k.decode('utf-8')): v for k, v in dict(_fpes).items()}             # <<<<<<<<<<<<<<
  * 
  * cdef dict get_last_info(PyOdeSys * odesys, success=True):
  */
   { /* enter inner scope */
-    PyObject *__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_k = NULL;
-    PyObject *__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_v = NULL;
     __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = 0;
     __pyx_t_6 = __pyx_convert_unordered_map_to_py_std_3a__3a_string____int(cvodes_cxx::fpes); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 29, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 29, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_7);
@@ -10786,17 +11032,21 @@
     __pyx_t_7 = 0;
     while (1) {
       __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_3, __pyx_t_5, &__pyx_t_4, &__pyx_t_7, &__pyx_t_6, NULL, __pyx_t_2);
       if (unlikely(__pyx_t_8 == 0)) break;
       if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 29, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_k, __pyx_t_7);
+      __Pyx_XGOTREF(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_k);
+      __Pyx_DECREF_SET(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_k, __pyx_t_7);
+      __Pyx_GIVEREF(__pyx_t_7);
       __pyx_t_7 = 0;
-      __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_v, __pyx_t_6);
+      __Pyx_XGOTREF(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_v);
+      __Pyx_DECREF_SET(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_v, __pyx_t_6);
+      __Pyx_GIVEREF(__pyx_t_6);
       __pyx_t_6 = 0;
       __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_k, __pyx_n_s_decode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 29, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__40, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 29, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 29, __pyx_L4_error)
@@ -10807,20 +11057,24 @@
       __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_6, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 29, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_t_7, (PyObject*)__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_v))) __PYX_ERR(0, 29, __pyx_L4_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_k);
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_v);
+    __Pyx_GOTREF(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_k);
+    __Pyx_DECREF_SET(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_k, Py_None);
+    __Pyx_GOTREF(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_v);
+    __Pyx_DECREF_SET(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_v, Py_None);
     goto __pyx_L7_exit_scope;
     __pyx_L4_error:;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_k);
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_v);
+    __Pyx_GOTREF(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_k);
+    __Pyx_DECREF_SET(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_k, Py_None);
+    __Pyx_GOTREF(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_v);
+    __Pyx_DECREF_SET(__pyx_7genexpr__pyx_v_8pycvodes_7_cvodes_v, Py_None);
     goto __pyx_L1_error;
     __pyx_L7_exit_scope:;
   } /* exit inner scope */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_fpes, __pyx_t_1) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pycvodes/_cvodes.pyx":46
@@ -10848,15 +11102,15 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pycvodes/_cvodes.pyx":1
  * # -*- coding: utf-8; mode: cython -*-             # <<<<<<<<<<<<<<
  * # distutils: language = c++
  * 
  */
-  __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "string.from_py":13
  * 
  * @cname("__pyx_convert_string_from_py_std__in_string")
@@ -10879,18 +11133,20 @@
     }
     Py_DECREF(__pyx_m); __pyx_m = 0;
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init pycvodes._cvodes");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
-  #if PY_MAJOR_VERSION < 3
-  return;
-  #else
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+  return (__pyx_m != NULL) ? 0 : -1;
+  #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
+  #else
+  return;
   #endif
 }
 
 /* --- Runtime support code --- */
 /* Refnanny */
 #if CYTHON_REFNANNY
 static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname) {
@@ -10921,18 +11177,18 @@
     }
     return result;
 }
 
 /* IterFinish */
 static CYTHON_INLINE int __Pyx_IterFinish(void) {
 #if CYTHON_FAST_THREAD_STATE
-    PyThreadState *tstate = PyThreadState_GET();
+    PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject* exc_type = tstate->curexc_type;
     if (unlikely(exc_type)) {
-        if (likely(exc_type == PyExc_StopIteration) || PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)) {
+        if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) {
             PyObject *exc_value, *exc_tb;
             exc_value = tstate->curexc_value;
             exc_tb = tstate->curexc_traceback;
             tstate->curexc_type = 0;
             tstate->curexc_value = 0;
             tstate->curexc_traceback = 0;
             Py_DECREF(exc_type);
@@ -10959,15 +11215,15 @@
 
 /* PyFunctionFastCall */
 #if CYTHON_FAST_PYCALL
 #include "frameobject.h"
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
-    PyThreadState *tstate = PyThreadState_GET();
+    PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject **fastlocals;
     Py_ssize_t i;
     PyObject *result;
     assert(globals != NULL);
     /* XXX Perhaps we should create a specialized
        PyFrame_New() that doesn't take locals, but does
        take builtins without sanity checking them.
@@ -11122,15 +11378,15 @@
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
 #ifdef __Pyx_CyFunction_USED
-    if (likely(PyCFunction_Check(func) || PyObject_TypeCheck(func, __pyx_CyFunctionType))) {
+    if (likely(PyCFunction_Check(func) || __Pyx_TypeCheck(func, __pyx_CyFunctionType))) {
 #else
     if (likely(PyCFunction_Check(func))) {
 #endif
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
         }
     }
@@ -11261,49 +11517,54 @@
       __Pyx_RaiseNeedMoreValuesError(PyTuple_GET_SIZE(t));
     } else {
       __Pyx_RaiseTooManyValuesError(index);
     }
 }
 
 /* UnpackTuple2 */
-  static CYTHON_INLINE int __Pyx_unpack_tuple2(PyObject* tuple, PyObject** pvalue1, PyObject** pvalue2,
-                                             int is_tuple, int has_known_size, int decref_tuple) {
-    Py_ssize_t index;
-    PyObject *value1 = NULL, *value2 = NULL, *iter = NULL;
-    if (!is_tuple && unlikely(!PyTuple_Check(tuple))) {
-        iternextfunc iternext;
-        iter = PyObject_GetIter(tuple);
-        if (unlikely(!iter)) goto bad;
-        if (decref_tuple) { Py_DECREF(tuple); tuple = NULL; }
-        iternext = Py_TYPE(iter)->tp_iternext;
-        value1 = iternext(iter); if (unlikely(!value1)) { index = 0; goto unpacking_failed; }
-        value2 = iternext(iter); if (unlikely(!value2)) { index = 1; goto unpacking_failed; }
-        if (!has_known_size && unlikely(__Pyx_IternextUnpackEndCheck(iternext(iter), 2))) goto bad;
-        Py_DECREF(iter);
-    } else {
-        if (!has_known_size && unlikely(PyTuple_GET_SIZE(tuple) != 2)) {
-            __Pyx_UnpackTupleError(tuple, 2);
-            goto bad;
-        }
+  static CYTHON_INLINE int __Pyx_unpack_tuple2_exact(
+        PyObject* tuple, PyObject** pvalue1, PyObject** pvalue2, int decref_tuple) {
+    PyObject *value1 = NULL, *value2 = NULL;
 #if CYTHON_COMPILING_IN_PYPY
-        value1 = PySequence_ITEM(tuple, 0);
-        if (unlikely(!value1)) goto bad;
-        value2 = PySequence_ITEM(tuple, 1);
-        if (unlikely(!value2)) goto bad;
-#else
-        value1 = PyTuple_GET_ITEM(tuple, 0);
-        value2 = PyTuple_GET_ITEM(tuple, 1);
-        Py_INCREF(value1);
-        Py_INCREF(value2);
+    value1 = PySequence_ITEM(tuple, 0);  if (unlikely(!value1)) goto bad;
+    value2 = PySequence_ITEM(tuple, 1);  if (unlikely(!value2)) goto bad;
+#else
+    value1 = PyTuple_GET_ITEM(tuple, 0);  Py_INCREF(value1);
+    value2 = PyTuple_GET_ITEM(tuple, 1);  Py_INCREF(value2);
 #endif
-        if (decref_tuple) { Py_DECREF(tuple); }
+    if (decref_tuple) {
+        Py_DECREF(tuple);
     }
     *pvalue1 = value1;
     *pvalue2 = value2;
     return 0;
+#if CYTHON_COMPILING_IN_PYPY
+bad:
+    Py_XDECREF(value1);
+    Py_XDECREF(value2);
+    if (decref_tuple) { Py_XDECREF(tuple); }
+    return -1;
+#endif
+}
+static int __Pyx_unpack_tuple2_generic(PyObject* tuple, PyObject** pvalue1, PyObject** pvalue2,
+                                       int has_known_size, int decref_tuple) {
+    Py_ssize_t index;
+    PyObject *value1 = NULL, *value2 = NULL, *iter = NULL;
+    iternextfunc iternext;
+    iter = PyObject_GetIter(tuple);
+    if (unlikely(!iter)) goto bad;
+    if (decref_tuple) { Py_DECREF(tuple); tuple = NULL; }
+    iternext = Py_TYPE(iter)->tp_iternext;
+    value1 = iternext(iter); if (unlikely(!value1)) { index = 0; goto unpacking_failed; }
+    value2 = iternext(iter); if (unlikely(!value2)) { index = 1; goto unpacking_failed; }
+    if (!has_known_size && unlikely(__Pyx_IternextUnpackEndCheck(iternext(iter), 2))) goto bad;
+    Py_DECREF(iter);
+    *pvalue1 = value1;
+    *pvalue2 = value2;
+    return 0;
 unpacking_failed:
     if (!has_known_size && __Pyx_IterFinish() == 0)
         __Pyx_RaiseNeedMoreValuesError(index);
 bad:
     Py_XDECREF(iter);
     Py_XDECREF(value1);
     Py_XDECREF(value2);
@@ -11319,26 +11580,28 @@
     if (is_dict) {
 #if !CYTHON_COMPILING_IN_PYPY
         *p_orig_length = PyDict_Size(iterable);
         Py_INCREF(iterable);
         return iterable;
 #elif PY_MAJOR_VERSION >= 3
         static PyObject *py_items = NULL, *py_keys = NULL, *py_values = NULL;
-        const char *name = PyUnicode_AsUTF8(method_name);
         PyObject **pp = NULL;
-        if (strcmp(name, "iteritems") == 0) pp = &py_items;
-        else if (strcmp(name, "iterkeys") == 0) pp = &py_keys;
-        else if (strcmp(name, "itervalues") == 0) pp = &py_values;
-        if (pp) {
-            if (!*pp) {
-                *pp = PyUnicode_FromString(name + 4);
-                if (!*pp)
-                    return NULL;
+        if (method_name) {
+            const char *name = PyUnicode_AsUTF8(method_name);
+            if (strcmp(name, "iteritems") == 0) pp = &py_items;
+            else if (strcmp(name, "iterkeys") == 0) pp = &py_keys;
+            else if (strcmp(name, "itervalues") == 0) pp = &py_values;
+            if (pp) {
+                if (!*pp) {
+                    *pp = PyUnicode_FromString(name + 4);
+                    if (!*pp)
+                        return NULL;
+                }
+                method_name = *pp;
             }
-            method_name = *pp;
         }
 #endif
     }
     *p_orig_length = 0;
     if (method_name) {
         PyObject* iter;
         iterable = __Pyx_PyObject_CallMethod0(iterable, method_name);
@@ -11436,20 +11699,27 @@
         PyErr_Clear();
 #endif
         result = __Pyx_GetBuiltinName(name);
     }
     return result;
 }
 
-/* BufferFormatCheck */
-    static CYTHON_INLINE int __Pyx_IsLittleEndian(void) {
-  unsigned int n = 1;
-  return *(unsigned char*)(&n) != 0;
+/* IsLittleEndian */
+    static CYTHON_INLINE int __Pyx_Is_Little_Endian(void)
+{
+  union {
+    uint32_t u32;
+    uint8_t u8[4];
+  } S;
+  S.u32 = 0x01020304;
+  return S.u8[0] == 4;
 }
-static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
+
+/* BufferFormatCheck */
+    static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
                               __Pyx_BufFmt_StackElem* stack,
                               __Pyx_TypeInfo* type) {
   stack[0].field = &ctx->root;
   stack[0].parent_offset = 0;
   ctx->root.type = type;
   ctx->root.name = "buffer dtype";
   ctx->root.offset = 0;
@@ -11762,15 +12032,15 @@
       }
     }
   } while (ctx->enc_count);
   ctx->enc_type = 0;
   ctx->is_complex = 0;
   return 0;
 }
-static CYTHON_INLINE PyObject *
+static PyObject *
 __pyx_buffmt_parse_array(__Pyx_BufFmt_Context* ctx, const char** tsp)
 {
     const char *ts = *tsp;
     int i = 0, number;
     int ndim = ctx->head->field->type->ndim;
 ;
     ++ts;
@@ -11827,24 +12097,24 @@
         return ts;
       case ' ':
       case '\r':
       case '\n':
         ++ts;
         break;
       case '<':
-        if (!__Pyx_IsLittleEndian()) {
+        if (!__Pyx_Is_Little_Endian()) {
           PyErr_SetString(PyExc_ValueError, "Little-endian buffer not supported on big-endian compiler");
           return NULL;
         }
         ctx->new_packmode = '=';
         ++ts;
         break;
       case '>':
       case '!':
-        if (__Pyx_IsLittleEndian()) {
+        if (__Pyx_Is_Little_Endian()) {
           PyErr_SetString(PyExc_ValueError, "Big-endian buffer not supported on little-endian compiler");
           return NULL;
         }
         ctx->new_packmode = '=';
         ++ts;
         break;
       case '=':
@@ -11939,68 +12209,69 @@
           int number = __Pyx_BufFmt_ExpectNumber(&ts);
           if (number == -1) return NULL;
           ctx->new_count = (size_t)number;
         }
     }
   }
 }
-static CYTHON_INLINE void __Pyx_ZeroBuffer(Py_buffer* buf) {
+
+/* BufferGetAndValidate */
+      static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info) {
+  if (unlikely(info->buf == NULL)) return;
+  if (info->suboffsets == __Pyx_minusones) info->suboffsets = NULL;
+  __Pyx_ReleaseBuffer(info);
+}
+static void __Pyx_ZeroBuffer(Py_buffer* buf) {
   buf->buf = NULL;
   buf->obj = NULL;
   buf->strides = __Pyx_zeros;
   buf->shape = __Pyx_zeros;
   buf->suboffsets = __Pyx_minusones;
 }
-static CYTHON_INLINE int __Pyx_GetBufferAndValidate(
+static int __Pyx__GetBufferAndValidate(
         Py_buffer* buf, PyObject* obj,  __Pyx_TypeInfo* dtype, int flags,
         int nd, int cast, __Pyx_BufFmt_StackElem* stack)
 {
-  if (obj == Py_None || obj == NULL) {
+  buf->buf = NULL;
+  if (unlikely(__Pyx_GetBuffer(obj, buf, flags) == -1)) {
     __Pyx_ZeroBuffer(buf);
-    return 0;
+    return -1;
   }
-  buf->buf = NULL;
-  if (__Pyx_GetBuffer(obj, buf, flags) == -1) goto fail;
-  if (buf->ndim != nd) {
+  if (unlikely(buf->ndim != nd)) {
     PyErr_Format(PyExc_ValueError,
                  "Buffer has wrong number of dimensions (expected %d, got %d)",
                  nd, buf->ndim);
     goto fail;
   }
   if (!cast) {
     __Pyx_BufFmt_Context ctx;
     __Pyx_BufFmt_Init(&ctx, stack, dtype);
     if (!__Pyx_BufFmt_CheckString(&ctx, buf->format)) goto fail;
   }
-  if ((unsigned)buf->itemsize != dtype->size) {
+  if (unlikely((unsigned)buf->itemsize != dtype->size)) {
     PyErr_Format(PyExc_ValueError,
       "Item size of buffer (%" CYTHON_FORMAT_SSIZE_T "d byte%s) does not match size of '%s' (%" CYTHON_FORMAT_SSIZE_T "d byte%s)",
       buf->itemsize, (buf->itemsize > 1) ? "s" : "",
       dtype->name, (Py_ssize_t)dtype->size, (dtype->size > 1) ? "s" : "");
     goto fail;
   }
   if (buf->suboffsets == NULL) buf->suboffsets = __Pyx_minusones;
   return 0;
 fail:;
-  __Pyx_ZeroBuffer(buf);
+  __Pyx_SafeReleaseBuffer(buf);
   return -1;
 }
-static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info) {
-  if (info->buf == NULL) return;
-  if (info->suboffsets == __Pyx_minusones) info->suboffsets = NULL;
-  __Pyx_ReleaseBuffer(info);
-}
 
 /* ExtTypeTest */
       static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
-    if (likely(PyObject_TypeCheck(obj, type)))
+    if (likely(__Pyx_TypeCheck(obj, type)))
         return 1;
     PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
                  Py_TYPE(obj)->tp_name, type->tp_name);
     return 0;
 }
 
 /* PyErrFetchRestore */
@@ -12166,37 +12437,31 @@
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
 /* ArgTypeTest */
-      static void __Pyx_RaiseArgumentTypeInvalid(const char* name, PyObject *obj, PyTypeObject *type) {
-    PyErr_Format(PyExc_TypeError,
-        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
-        name, type->tp_name, Py_TYPE(obj)->tp_name);
-}
-static CYTHON_INLINE int __Pyx_ArgTypeTest(PyObject *obj, PyTypeObject *type, int none_allowed,
-    const char *name, int exact)
+      static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
 {
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
-    if (none_allowed && obj == Py_None) return 1;
     else if (exact) {
-        if (likely(Py_TYPE(obj) == type)) return 1;
         #if PY_MAJOR_VERSION == 2
-        else if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
+        if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
         #endif
     }
     else {
-        if (likely(PyObject_TypeCheck(obj, type))) return 1;
+        if (likely(__Pyx_TypeCheck(obj, type))) return 1;
     }
-    __Pyx_RaiseArgumentTypeInvalid(name, obj, type);
+    PyErr_Format(PyExc_TypeError,
+        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
+        name, type->tp_name, Py_TYPE(obj)->tp_name);
     return 0;
 }
 
 /* RaiseException */
       #if PY_MAJOR_VERSION < 3
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
                         CYTHON_UNUSED PyObject *cause) {
@@ -12308,19 +12573,15 @@
             }
         }
     } else {
         PyErr_SetString(PyExc_TypeError,
             "raise: exception class must be a subclass of BaseException");
         goto bad;
     }
-#if PY_VERSION_HEX >= 0x03030000
     if (cause) {
-#else
-    if (cause && cause != Py_None) {
-#endif
         PyObject *fixed_cause;
         if (cause == Py_None) {
             fixed_cause = NULL;
         } else if (PyExceptionClass_Check(cause)) {
             fixed_cause = PyObject_CallObject(cause, NULL);
             if (fixed_cause == NULL)
                 goto bad;
@@ -12340,15 +12601,15 @@
 #if CYTHON_COMPILING_IN_PYPY
         PyObject *tmp_type, *tmp_value, *tmp_tb;
         PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
         Py_INCREF(tb);
         PyErr_Restore(tmp_type, tmp_value, tb);
         Py_XDECREF(tmp_tb);
 #else
-        PyThreadState *tstate = PyThreadState_GET();
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
 #endif
@@ -12356,15 +12617,15 @@
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
 /* PyIntBinop */
-        #if !CYTHON_COMPILING_IN_PYPY
+      #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_AddCObj(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, CYTHON_UNUSED int inplace) {
     #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_CheckExact(op2))) {
         const long a = intval;
         long x;
         long b = PyInt_AS_LONG(op2);
             x = (long)((unsigned long)a + b);
@@ -12472,21 +12733,21 @@
             return PyFloat_FromDouble(result);
     }
     return (inplace ? PyNumber_InPlaceAdd : PyNumber_Add)(op1, op2);
 }
 #endif
 
 /* BufferFallbackError */
-        static void __Pyx_RaiseBufferFallbackError(void) {
+      static void __Pyx_RaiseBufferFallbackError(void) {
   PyErr_SetString(PyExc_ValueError,
      "Buffer acquisition failed on assignment; and then reacquiring the old buffer failed too!");
 }
 
 /* GetItemInt */
-        static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
+      static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
     if (!j) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
     return r;
 }
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
@@ -12565,15 +12826,15 @@
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* GetException */
-        #if CYTHON_FAST_THREAD_STATE
+      #if CYTHON_FAST_THREAD_STATE
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb) {
 #endif
     PyObject *local_type, *local_value, *local_tb;
 #if CYTHON_FAST_THREAD_STATE
     PyObject *tmp_type, *tmp_value, *tmp_tb;
@@ -12602,20 +12863,29 @@
     Py_XINCREF(local_tb);
     Py_XINCREF(local_type);
     Py_XINCREF(local_value);
     *type = local_type;
     *value = local_value;
     *tb = local_tb;
 #if CYTHON_FAST_THREAD_STATE
+    #if PY_VERSION_HEX >= 0x030700A2
+    tmp_type = tstate->exc_state.exc_type;
+    tmp_value = tstate->exc_state.exc_value;
+    tmp_tb = tstate->exc_state.exc_traceback;
+    tstate->exc_state.exc_type = local_type;
+    tstate->exc_state.exc_value = local_value;
+    tstate->exc_state.exc_traceback = local_tb;
+    #else
     tmp_type = tstate->exc_type;
     tmp_value = tstate->exc_value;
     tmp_tb = tstate->exc_traceback;
     tstate->exc_type = local_type;
     tstate->exc_value = local_value;
     tstate->exc_traceback = local_tb;
+    #endif
     Py_XDECREF(tmp_type);
     Py_XDECREF(tmp_value);
     Py_XDECREF(tmp_tb);
 #else
     PyErr_SetExcInfo(local_type, local_value, local_tb);
 #endif
     return 0;
@@ -12626,23 +12896,32 @@
     Py_XDECREF(local_type);
     Py_XDECREF(local_value);
     Py_XDECREF(local_tb);
     return -1;
 }
 
 /* SwapException */
-          #if CYTHON_FAST_THREAD_STATE
+        #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
+    #if PY_VERSION_HEX >= 0x030700A2
+    tmp_type = tstate->exc_state.exc_type;
+    tmp_value = tstate->exc_state.exc_value;
+    tmp_tb = tstate->exc_state.exc_traceback;
+    tstate->exc_state.exc_type = *type;
+    tstate->exc_state.exc_value = *value;
+    tstate->exc_state.exc_traceback = *tb;
+    #else
     tmp_type = tstate->exc_type;
     tmp_value = tstate->exc_value;
     tmp_tb = tstate->exc_traceback;
     tstate->exc_type = *type;
     tstate->exc_value = *value;
     tstate->exc_traceback = *tb;
+    #endif
     *type = tmp_type;
     *value = tmp_value;
     *tb = tmp_tb;
 }
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
@@ -12651,61 +12930,91 @@
     *type = tmp_type;
     *value = tmp_value;
     *tb = tmp_tb;
 }
 #endif
 
 /* SaveResetException */
-          #if CYTHON_FAST_THREAD_STATE
+        #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    #if PY_VERSION_HEX >= 0x030700A2
+    *type = tstate->exc_state.exc_type;
+    *value = tstate->exc_state.exc_value;
+    *tb = tstate->exc_state.exc_traceback;
+    #else
     *type = tstate->exc_type;
     *value = tstate->exc_value;
     *tb = tstate->exc_traceback;
+    #endif
     Py_XINCREF(*type);
     Py_XINCREF(*value);
     Py_XINCREF(*tb);
 }
 static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
+    #if PY_VERSION_HEX >= 0x030700A2
+    tmp_type = tstate->exc_state.exc_type;
+    tmp_value = tstate->exc_state.exc_value;
+    tmp_tb = tstate->exc_state.exc_traceback;
+    tstate->exc_state.exc_type = type;
+    tstate->exc_state.exc_value = value;
+    tstate->exc_state.exc_traceback = tb;
+    #else
     tmp_type = tstate->exc_type;
     tmp_value = tstate->exc_value;
     tmp_tb = tstate->exc_traceback;
     tstate->exc_type = type;
     tstate->exc_value = value;
     tstate->exc_traceback = tb;
+    #endif
     Py_XDECREF(tmp_type);
     Py_XDECREF(tmp_value);
     Py_XDECREF(tmp_tb);
 }
 #endif
 
 /* BufferIndexError */
-          static void __Pyx_RaiseBufferIndexError(int axis) {
+        static void __Pyx_RaiseBufferIndexError(int axis) {
   PyErr_Format(PyExc_IndexError,
      "Out of bounds on buffer access (axis %d)", axis);
 }
 
 /* PyErrExceptionMatches */
-          #if CYTHON_FAST_THREAD_STATE
+        #if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
+    return 0;
+}
 static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
     PyObject *exc_type = tstate->curexc_type;
     if (exc_type == err) return 1;
     if (unlikely(!exc_type)) return 0;
-    return PyErr_GivenExceptionMatches(exc_type, err);
+    if (unlikely(PyTuple_Check(err)))
+        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
 }
 #endif
 
 /* Import */
-          static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
+        static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
     PyObject *empty_list = 0;
     PyObject *module = 0;
     PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
     PyObject *list;
-    #if PY_VERSION_HEX < 0x03030000
+    #if PY_MAJOR_VERSION < 3
     PyObject *py_import;
     py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
     if (!py_import)
         goto bad;
     #endif
     if (from_list)
         list = from_list;
@@ -12721,93 +13030,87 @@
     empty_dict = PyDict_New();
     if (!empty_dict)
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
             if (strchr(__Pyx_MODULE_NAME, '.')) {
-                #if PY_VERSION_HEX < 0x03030000
-                PyObject *py_level = PyInt_FromLong(1);
-                if (!py_level)
-                    goto bad;
-                module = PyObject_CallFunctionObjArgs(py_import,
-                    name, global_dict, empty_dict, list, py_level, NULL);
-                Py_DECREF(py_level);
-                #else
                 module = PyImport_ImportModuleLevelObject(
                     name, global_dict, empty_dict, list, 1);
-                #endif
                 if (!module) {
                     if (!PyErr_ExceptionMatches(PyExc_ImportError))
                         goto bad;
                     PyErr_Clear();
                 }
             }
             level = 0;
         }
         #endif
         if (!module) {
-            #if PY_VERSION_HEX < 0x03030000
+            #if PY_MAJOR_VERSION < 3
             PyObject *py_level = PyInt_FromLong(level);
             if (!py_level)
                 goto bad;
             module = PyObject_CallFunctionObjArgs(py_import,
                 name, global_dict, empty_dict, list, py_level, NULL);
             Py_DECREF(py_level);
             #else
             module = PyImport_ImportModuleLevelObject(
                 name, global_dict, empty_dict, list, level);
             #endif
         }
     }
 bad:
-    #if PY_VERSION_HEX < 0x03030000
+    #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_import);
     #endif
     Py_XDECREF(empty_list);
     Py_XDECREF(empty_dict);
     return module;
 }
 
 /* CLineInTraceback */
-          static int __Pyx_CLineForTraceback(int c_line) {
-#ifdef CYTHON_CLINE_IN_TRACEBACK
-    return ((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0;
-#else
-    PyObject **cython_runtime_dict;
+        #ifndef CYTHON_CLINE_IN_TRACEBACK
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
+    PyObject *ptype, *pvalue, *ptraceback;
+#if CYTHON_COMPILING_IN_CPYTHON
+    PyObject **cython_runtime_dict;
+#endif
+    __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
+#if CYTHON_COMPILING_IN_CPYTHON
     cython_runtime_dict = _PyObject_GetDictPtr(__pyx_cython_runtime);
-    if (unlikely(!cython_runtime_dict)) {
-      PyObject *ptype, *pvalue, *ptraceback;
-      PyObject *use_cline_obj;
-      PyErr_Fetch(&ptype, &pvalue, &ptraceback);
-      use_cline_obj = __Pyx_PyObject_GetAttrStr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
+    if (likely(cython_runtime_dict)) {
+      use_cline = PyDict_GetItem(*cython_runtime_dict, __pyx_n_s_cline_in_traceback);
+    } else
+#endif
+    {
+      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
       if (use_cline_obj) {
         use_cline = PyObject_Not(use_cline_obj) ? Py_False : Py_True;
         Py_DECREF(use_cline_obj);
       } else {
+        PyErr_Clear();
         use_cline = NULL;
       }
-      PyErr_Restore(ptype, pvalue, ptraceback);
-    } else {
-      use_cline = PyDict_GetItem(*_PyObject_GetDictPtr(__pyx_cython_runtime), __pyx_n_s_cline_in_traceback);
     }
     if (!use_cline) {
         c_line = 0;
         PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (PyObject_Not(use_cline) != 0) {
         c_line = 0;
     }
+    __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
-#endif
 }
+#endif
 
 /* CodeObjectCache */
-          static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
+        static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
         if (code_line < entries[mid].code_line) {
@@ -12879,15 +13182,15 @@
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
-          #include "compile.h"
+        #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyObject *py_srcfile = 0;
@@ -12938,61 +13241,63 @@
     Py_XDECREF(py_funcname);
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
+    PyThreadState *tstate = __Pyx_PyThreadState_Current;
     if (c_line) {
-        c_line = __Pyx_CLineForTraceback(c_line);
+        c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
         if (!py_code) goto bad;
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
-        PyThreadState_GET(), /*PyThreadState *tstate,*/
-        py_code,             /*PyCodeObject *code,*/
-        __pyx_d,      /*PyObject *globals,*/
-        0                    /*PyObject *locals*/
+        tstate,            /*PyThreadState *tstate,*/
+        py_code,           /*PyCodeObject *code,*/
+        __pyx_d,    /*PyObject *globals,*/
+        0                  /*PyObject *locals*/
     );
     if (!py_frame) goto bad;
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
 #if PY_MAJOR_VERSION < 3
 static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags) {
     if (PyObject_CheckBuffer(obj)) return PyObject_GetBuffer(obj, view, flags);
-        if (PyObject_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) return __pyx_pw_5numpy_7ndarray_1__getbuffer__(obj, view, flags);
+        if (__Pyx_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) return __pyx_pw_5numpy_7ndarray_1__getbuffer__(obj, view, flags);
     PyErr_Format(PyExc_TypeError, "'%.200s' does not have the buffer interface", Py_TYPE(obj)->tp_name);
     return -1;
 }
 static void __Pyx_ReleaseBuffer(Py_buffer *view) {
     PyObject *obj = view->obj;
     if (!obj) return;
     if (PyObject_CheckBuffer(obj)) {
         PyBuffer_Release(view);
         return;
     }
-        if (PyObject_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) { __pyx_pw_5numpy_7ndarray_3__releasebuffer__(obj, view); return; }
-    Py_DECREF(obj);
+    if ((0)) {}
+        else if (__Pyx_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) __pyx_pw_5numpy_7ndarray_3__releasebuffer__(obj, view);
     view->obj = NULL;
+    Py_DECREF(obj);
 }
 #endif
 
 
-          /* CIntFromPyVerify */
-          #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
+        /* CIntFromPyVerify */
+        #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
     {\
         func_type value = func_value;\
         if (sizeof(target_type) < sizeof(func_type)) {\
@@ -13006,15 +13311,15 @@
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
 /* CIntToPy */
-          static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+        static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
     const int neg_one = (int) -1, const_zero = (int) 0;
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
         if (sizeof(int) < sizeof(long)) {
             return PyInt_FromLong((long) value);
         } else if (sizeof(int) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
@@ -13037,15 +13342,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-          static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+        static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
     const long neg_one = (long) -1, const_zero = (long) 0;
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
         if (sizeof(long) < sizeof(long)) {
             return PyInt_FromLong((long) value);
         } else if (sizeof(long) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
@@ -13068,15 +13373,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* Declarations */
-          #if CYTHON_CCOMPLEX
+        #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return x + y*(__pyx_t_float_complex)_Complex_I;
@@ -13088,15 +13393,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-          #if CYTHON_CCOMPLEX
+        #if CYTHON_CCOMPLEX
 #else
     static CYTHON_INLINE int __Pyx_c_eq_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_sum_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
         __pyx_t_float_complex z;
         z.real = a.real + b.real;
@@ -13223,15 +13528,15 @@
             z.imag = z_r * sinf(z_theta);
             return z;
         }
     #endif
 #endif
 
 /* Declarations */
-          #if CYTHON_CCOMPLEX
+        #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return ::std::complex< double >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return x + y*(__pyx_t_double_complex)_Complex_I;
@@ -13243,15 +13548,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-          #if CYTHON_CCOMPLEX
+        #if CYTHON_CCOMPLEX
 #else
     static CYTHON_INLINE int __Pyx_c_eq_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_sum_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
         __pyx_t_double_complex z;
         z.real = a.real + b.real;
@@ -13378,15 +13683,15 @@
             z.imag = z_r * sin(z_theta);
             return z;
         }
     #endif
 #endif
 
 /* CIntToPy */
-          static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value) {
+        static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value) {
     const enum NPY_TYPES neg_one = (enum NPY_TYPES) -1, const_zero = (enum NPY_TYPES) 0;
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
         if (sizeof(enum NPY_TYPES) < sizeof(long)) {
             return PyInt_FromLong((long) value);
         } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
@@ -13409,15 +13714,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(enum NPY_TYPES),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-          static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
+        static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
     const int neg_one = (int) -1, const_zero = (int) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(int) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
@@ -13598,15 +13903,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CIntFromPy */
-          static CYTHON_INLINE unsigned int __Pyx_PyInt_As_unsigned_int(PyObject *x) {
+        static CYTHON_INLINE unsigned int __Pyx_PyInt_As_unsigned_int(PyObject *x) {
     const unsigned int neg_one = (unsigned int) -1, const_zero = (unsigned int) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(unsigned int) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(unsigned int, long, PyInt_AS_LONG(x))
         } else {
@@ -13787,15 +14092,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to unsigned int");
     return (unsigned int) -1;
 }
 
 /* CIntFromPy */
-          static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
+        static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
     const size_t neg_one = (size_t) -1, const_zero = (size_t) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(size_t) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(size_t, long, PyInt_AS_LONG(x))
         } else {
@@ -13976,15 +14281,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to size_t");
     return (size_t) -1;
 }
 
 /* CIntFromPy */
-          static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
+        static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
     const long neg_one = (long) -1, const_zero = (long) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(long) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
@@ -14164,16 +14469,88 @@
     return (long) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
+/* FastTypeChecks */
+        #if CYTHON_COMPILING_IN_CPYTHON
+static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
+    while (a) {
+        a = a->tp_base;
+        if (a == b)
+            return 1;
+    }
+    return b == &PyBaseObject_Type;
+}
+static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b) {
+    PyObject *mro;
+    if (a == b) return 1;
+    mro = a->tp_mro;
+    if (likely(mro)) {
+        Py_ssize_t i, n;
+        n = PyTuple_GET_SIZE(mro);
+        for (i = 0; i < n; i++) {
+            if (PyTuple_GET_ITEM(mro, i) == (PyObject *)b)
+                return 1;
+        }
+        return 0;
+    }
+    return __Pyx_InBases(a, b);
+}
+#if PY_MAJOR_VERSION == 2
+static int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject* exc_type2) {
+    PyObject *exception, *value, *tb;
+    int res;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&exception, &value, &tb);
+    res = exc_type1 ? PyObject_IsSubclass(err, exc_type1) : 0;
+    if (unlikely(res == -1)) {
+        PyErr_WriteUnraisable(err);
+        res = 0;
+    }
+    if (!res) {
+        res = PyObject_IsSubclass(err, exc_type2);
+        if (unlikely(res == -1)) {
+            PyErr_WriteUnraisable(err);
+            res = 0;
+        }
+    }
+    __Pyx_ErrRestore(exception, value, tb);
+    return res;
+}
+#else
+static CYTHON_INLINE int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject *exc_type2) {
+    int res = exc_type1 ? __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type1) : 0;
+    if (!res) {
+        res = __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
+    }
+    return res;
+}
+#endif
+static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject* exc_type) {
+    if (likely(err == exc_type)) return 1;
+    if (likely(PyExceptionClass_Check(err))) {
+        return __Pyx_inner_PyErr_GivenExceptionMatches2(err, NULL, exc_type);
+    }
+    return PyErr_GivenExceptionMatches(err, exc_type);
+}
+static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *exc_type1, PyObject *exc_type2) {
+    if (likely(err == exc_type1 || err == exc_type2)) return 1;
+    if (likely(PyExceptionClass_Check(err))) {
+        return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
+    }
+    return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
+}
+#endif
+
 /* CheckBinaryVersion */
-          static int __Pyx_check_binary_version(void) {
+        static int __Pyx_check_binary_version(void) {
     char ctversion[4], rtversion[4];
     PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
     PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
     if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
         char message[200];
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
@@ -14181,15 +14558,15 @@
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* ModuleImport */
-          #ifndef __PYX_HAVE_RT_ImportModule
+        #ifndef __PYX_HAVE_RT_ImportModule
 #define __PYX_HAVE_RT_ImportModule
 static PyObject *__Pyx_ImportModule(const char *name) {
     PyObject *py_name = 0;
     PyObject *py_module = 0;
     py_name = __Pyx_PyIdentifier_FromString(name);
     if (!py_name)
         goto bad;
@@ -14199,15 +14576,15 @@
 bad:
     Py_XDECREF(py_name);
     return 0;
 }
 #endif
 
 /* TypeImport */
-          #ifndef __PYX_HAVE_RT_ImportType
+        #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(const char *module_name, const char *class_name,
     size_t size, int strict)
 {
     PyObject *py_module = 0;
     PyObject *result = 0;
     PyObject *py_name = 0;
@@ -14264,15 +14641,15 @@
     Py_XDECREF(py_module);
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* InitStrings */
-          static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
+        static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
         #if PY_MAJOR_VERSION < 3
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
@@ -14303,54 +14680,61 @@
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
     return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
 }
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject* o) {
     Py_ssize_t ignore;
     return __Pyx_PyObject_AsStringAndSize(o, &ignore);
 }
-static CYTHON_INLINE const char* __Pyx_PyObject_AsStringAndSize(PyObject* o, Py_ssize_t *length) {
-#if CYTHON_COMPILING_IN_CPYTHON && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
-    if (
-#if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
-            __Pyx_sys_getdefaultencoding_not_ascii &&
-#endif
-            PyUnicode_Check(o)) {
-#if PY_VERSION_HEX < 0x03030000
-        char* defenc_c;
-        PyObject* defenc = _PyUnicode_AsDefaultEncodedString(o, NULL);
-        if (!defenc) return NULL;
-        defenc_c = PyBytes_AS_STRING(defenc);
+#if __PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
+#if !CYTHON_PEP393_ENABLED
+static const char* __Pyx_PyUnicode_AsStringAndSize(PyObject* o, Py_ssize_t *length) {
+    char* defenc_c;
+    PyObject* defenc = _PyUnicode_AsDefaultEncodedString(o, NULL);
+    if (!defenc) return NULL;
+    defenc_c = PyBytes_AS_STRING(defenc);
 #if __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
-        {
-            char* end = defenc_c + PyBytes_GET_SIZE(defenc);
-            char* c;
-            for (c = defenc_c; c < end; c++) {
-                if ((unsigned char) (*c) >= 128) {
-                    PyUnicode_AsASCIIString(o);
-                    return NULL;
-                }
+    {
+        char* end = defenc_c + PyBytes_GET_SIZE(defenc);
+        char* c;
+        for (c = defenc_c; c < end; c++) {
+            if ((unsigned char) (*c) >= 128) {
+                PyUnicode_AsASCIIString(o);
+                return NULL;
             }
         }
+    }
 #endif
-        *length = PyBytes_GET_SIZE(defenc);
-        return defenc_c;
+    *length = PyBytes_GET_SIZE(defenc);
+    return defenc_c;
+}
 #else
-        if (__Pyx_PyUnicode_READY(o) == -1) return NULL;
+static CYTHON_INLINE const char* __Pyx_PyUnicode_AsStringAndSize(PyObject* o, Py_ssize_t *length) {
+    if (unlikely(__Pyx_PyUnicode_READY(o) == -1)) return NULL;
 #if __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
-        if (PyUnicode_IS_ASCII(o)) {
-            *length = PyUnicode_GET_LENGTH(o);
-            return PyUnicode_AsUTF8(o);
-        } else {
-            PyUnicode_AsASCIIString(o);
-            return NULL;
-        }
+    if (likely(PyUnicode_IS_ASCII(o))) {
+        *length = PyUnicode_GET_LENGTH(o);
+        return PyUnicode_AsUTF8(o);
+    } else {
+        PyUnicode_AsASCIIString(o);
+        return NULL;
+    }
 #else
-        return PyUnicode_AsUTF8AndSize(o, length);
+    return PyUnicode_AsUTF8AndSize(o, length);
+#endif
+}
 #endif
 #endif
+static CYTHON_INLINE const char* __Pyx_PyObject_AsStringAndSize(PyObject* o, Py_ssize_t *length) {
+#if __PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
+    if (
+#if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
+            __Pyx_sys_getdefaultencoding_not_ascii &&
+#endif
+            PyUnicode_Check(o)) {
+        return __Pyx_PyUnicode_AsStringAndSize(o, length);
     } else
 #endif
 #if (!CYTHON_COMPILING_IN_PYPY) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
     if (PyByteArray_Check(o)) {
         *length = PyByteArray_GET_SIZE(o);
         return PyByteArray_AS_STRING(o);
     } else
@@ -14366,57 +14750,75 @@
     }
 }
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject* x) {
    int is_true = x == Py_True;
    if (is_true | (x == Py_False) | (x == Py_None)) return is_true;
    else return PyObject_IsTrue(x);
 }
+static PyObject* __Pyx_PyNumber_IntOrLongWrongResultType(PyObject* result, const char* type_name) {
+#if PY_MAJOR_VERSION >= 3
+    if (PyLong_Check(result)) {
+        if (PyErr_WarnFormat(PyExc_DeprecationWarning, 1,
+                "__int__ returned non-int (type %.200s).  "
+                "The ability to return an instance of a strict subclass of int "
+                "is deprecated, and may be removed in a future version of Python.",
+                Py_TYPE(result)->tp_name)) {
+            Py_DECREF(result);
+            return NULL;
+        }
+        return result;
+    }
+#endif
+    PyErr_Format(PyExc_TypeError,
+                 "__%.4s__ returned non-%.4s (type %.200s)",
+                 type_name, type_name, Py_TYPE(result)->tp_name);
+    Py_DECREF(result);
+    return NULL;
+}
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x) {
 #if CYTHON_USE_TYPE_SLOTS
   PyNumberMethods *m;
 #endif
   const char *name = NULL;
   PyObject *res = NULL;
 #if PY_MAJOR_VERSION < 3
-  if (PyInt_Check(x) || PyLong_Check(x))
+  if (likely(PyInt_Check(x) || PyLong_Check(x)))
 #else
-  if (PyLong_Check(x))
+  if (likely(PyLong_Check(x)))
 #endif
     return __Pyx_NewRef(x);
 #if CYTHON_USE_TYPE_SLOTS
   m = Py_TYPE(x)->tp_as_number;
   #if PY_MAJOR_VERSION < 3
   if (m && m->nb_int) {
     name = "int";
-    res = PyNumber_Int(x);
+    res = m->nb_int(x);
   }
   else if (m && m->nb_long) {
     name = "long";
-    res = PyNumber_Long(x);
+    res = m->nb_long(x);
   }
   #else
-  if (m && m->nb_int) {
+  if (likely(m && m->nb_int)) {
     name = "int";
-    res = PyNumber_Long(x);
+    res = m->nb_int(x);
   }
   #endif
 #else
-  res = PyNumber_Int(x);
+  if (!PyBytes_CheckExact(x) && !PyUnicode_CheckExact(x)) {
+    res = PyNumber_Int(x);
+  }
 #endif
-  if (res) {
+  if (likely(res)) {
 #if PY_MAJOR_VERSION < 3
-    if (!PyInt_Check(res) && !PyLong_Check(res)) {
+    if (unlikely(!PyInt_Check(res) && !PyLong_Check(res))) {
 #else
-    if (!PyLong_Check(res)) {
+    if (unlikely(!PyLong_CheckExact(res))) {
 #endif
-      PyErr_Format(PyExc_TypeError,
-                   "__%.4s__ returned non-%.4s (type %.200s)",
-                   name, name, Py_TYPE(res)->tp_name);
-      Py_DECREF(res);
-      return NULL;
+        return __Pyx_PyNumber_IntOrLongWrongResultType(res, name);
     }
   }
   else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_TypeError,
                     "an integer is required");
   }
   return res;
```

### Comparing `pycvodes-0.9.1/pycvodes/_util.py` & `pycvodes-0.9.2/pycvodes/_util.py`

 * *Files identical despite different names*

### Comparing `pycvodes-0.9.1/pycvodes/include/cvodes_anyode.hpp` & `pycvodes-0.9.2/pycvodes/include/cvodes_anyode.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -43,39 +43,75 @@
         AnyODE::Status status = odesys.roots(t, NV_DATA_S(y), gout);
         if (status == AnyODE::Status::recoverable_error)
             throw std::runtime_error("There are only unrecoverable errors for roots().");
         return handle_status_(status);
     }
 
     template <class OdeSys>
-    int jac_dense_cb(long int N, realtype t,
-                     N_Vector y, N_Vector fy, DlsMat Jac, void *user_data,
-                     N_Vector tmp1, N_Vector tmp2, N_Vector tmp3){
+    int jac_dense_cb(
+#if SUNDIALS_VERSION_MAJOR < 3
+                     long int N,
+#endif
+                     realtype t,
+                     N_Vector y, N_Vector fy,
+#if SUNDIALS_VERSION_MAJOR < 3
+                     DlsMat Jac,
+#else
+                     SUNMatrix Jac,
+#endif
+                     void *user_data,
+                     N_Vector tmp1, N_Vector tmp2, N_Vector tmp3
+                     ){
         // callback of req. signature wrapping OdeSys method.
-        AnyODE::ignore(N); AnyODE::ignore(tmp1); AnyODE::ignore(tmp2); AnyODE::ignore(tmp3);
+#if SUNDIALS_VERSION_MAJOR < 3
+        AnyODE::ignore(N);
+#endif
+        AnyODE::ignore(tmp1); AnyODE::ignore(tmp2); AnyODE::ignore(tmp3);
         auto& odesys = *static_cast<OdeSys*>(user_data);
         if (odesys.record_jac_xvals)
             odesys.last_integration_info_vecdbl["jac_xvals"].push_back(t);
-        AnyODE::Status status = odesys.dense_jac_cmaj(t, NV_DATA_S(y), NV_DATA_S(fy), DENSE_COL(Jac, 0), Jac->ldim);
+        AnyODE::Status status = odesys.dense_jac_cmaj(t, NV_DATA_S(y), NV_DATA_S(fy),
+#if SUNDIALS_VERSION_MAJOR < 3
+                                                      DENSE_COL(Jac, 0), Jac->ldim
+#else
+                                                      SM_DATA_D(Jac), odesys.get_ny()
+#endif
+                                                      );
         return handle_status_(status);
     }
 
     template <typename OdeSys>
-    int jac_band_cb(long int N, long int mupper, long int mlower, realtype t,
-                    N_Vector y, N_Vector fy, DlsMat Jac, void *user_data,
+    int jac_band_cb(
+#if SUNDIALS_VERSION_MAJOR < 3
+                    long int N, long int mupper, long int mlower,
+#endif
+                    realtype t,
+                    N_Vector y, N_Vector fy,
+#if SUNDIALS_VERSION_MAJOR < 3
+                    DlsMat Jac,
+#else
+                    SUNMatrix Jac,
+#endif
+                    void *user_data,
                     N_Vector tmp1, N_Vector tmp2, N_Vector tmp3){
-        AnyODE::ignore(N); AnyODE::ignore(tmp1); AnyODE::ignore(tmp2); AnyODE::ignore(tmp3);
+        AnyODE::ignore(tmp1); AnyODE::ignore(tmp2); AnyODE::ignore(tmp3);
         auto& odesys = *static_cast<OdeSys*>(user_data);
+#if SUNDIALS_VERSION_MAJOR < 3
         if (odesys.get_mupper() != mupper)
             throw std::runtime_error("mupper mismatch");
         if (odesys.get_mlower() != mlower)
             throw std::runtime_error("mlower mismatch");
+        auto Jac_ = Jac;
+        AnyODE::ignore(N);
+#else
+        auto Jac_ = SM_CONTENT_B(Jac);
+#endif
         if (odesys.record_jac_xvals)
             odesys.last_integration_info_vecdbl["jac_xvals"].push_back(t);
-        AnyODE::Status status = odesys.banded_jac_cmaj(t, NV_DATA_S(y), NV_DATA_S(fy), Jac->data + Jac->s_mu - Jac->mu, Jac->ldim);
+        AnyODE::Status status = odesys.banded_jac_cmaj(t, NV_DATA_S(y), NV_DATA_S(fy), Jac_->data + Jac_->s_mu - Jac_->mu, Jac_->ldim);
         return handle_status_(status);
     }
 
 
     template <typename OdeSys>
     int jac_times_vec_cb(N_Vector v, N_Vector Jv, realtype t, N_Vector y,
                          N_Vector fy, void *user_data, N_Vector tmp){
@@ -87,36 +123,47 @@
             throw std::runtime_error("There are only unrecoverable errors for JacTimesVec().");
         return handle_status_(status);
     }
 
     template <typename OdeSys> // Section 4.6.9 Preconditioning in cvs_guide.pdf
     int jac_prec_solve_cb(realtype t, N_Vector y, N_Vector fy, N_Vector r,
                           N_Vector z, realtype gamma, realtype delta, int lr,
-                          void *user_data, N_Vector tmp){
+                          void *user_data
+#if SUNDIALS_VERSION_MAJOR < 3
+                          , N_Vector tmp
+#endif
+                          ){
         // callback of req. signature wrapping OdeSys method.
+#if SUNDIALS_VERSION_MAJOR < 3
         AnyODE::ignore(tmp);  // delta used for iterative methods
+#endif
         double * ewt {nullptr};
         auto& odesys = *static_cast<OdeSys*>(user_data);
         if (lr != 1)
             throw std::runtime_error("Only left preconditioning implemented.");
         AnyODE::Status status =  odesys.prec_solve_left(t, NV_DATA_S(y), NV_DATA_S(fy), NV_DATA_S(r),
                                                         NV_DATA_S(z), gamma, delta, ewt);
         return handle_status_(status);
     }
 
     template <typename OdeSys>
     int prec_setup_cb(realtype t, N_Vector y, N_Vector fy, booleantype jok,
-                      booleantype *jcurPtr, realtype gamma, void *user_data,
-                      N_Vector tmp1, N_Vector tmp2, N_Vector tmp3){
+                      booleantype *jcurPtr, realtype gamma, void *user_data
+#if SUNDIALS_VERSION_MAJOR < 3
+                      ,N_Vector tmp1, N_Vector tmp2, N_Vector tmp3
+#endif
+                      ){
         // callback of req. signature wrapping OdeSys method.
+#if SUNDIALS_VERSION_MAJOR < 3
         AnyODE::ignore(tmp1); AnyODE::ignore(tmp2); AnyODE::ignore(tmp3);
+#endif
         auto& odesys = *static_cast<OdeSys*>(user_data);
         bool jac_recomputed = false;
         AnyODE::Status status = odesys.prec_setup(t, NV_DATA_S(y), NV_DATA_S(fy), jok, jac_recomputed, gamma);
-        (*jcurPtr) = (jac_recomputed) ? TRUE : FALSE;
+        (*jcurPtr) = (jac_recomputed) ? SUNTRUE : SUNFALSE;
         return handle_status_(status);
     }
 
     template <class OdeSys>
     CVodeIntegrator get_integrator(OdeSys * odesys,
                                    const std::vector<realtype> atol,
                                    const realtype rtol,
@@ -144,15 +191,17 @@
         integr.record_steps = odesys->record_steps;
         integr.set_user_data(static_cast<void *>(odesys));
         integr.init(rhs_cb<OdeSys>, t0, y0, ny);
         if (nroots > 0)
             integr.root_init(nroots, roots_cb<OdeSys>);
         if (atol.size() == 1){
             integr.set_tol(rtol, atol[0]);
-        }else{
+        } else if (atol.size() != (size_t)ny) {
+            throw std::runtime_error("atol of incorrect length");
+        } else {
             integr.set_tol(rtol, atol);
         }
         integr.set_init_step(dx0);
         if (dx_min != 0.0)
             integr.set_min_step(dx_min);
         if (dx_max != 0.0)
             integr.set_max_step(dx_max);
```

### Comparing `pycvodes-0.9.1/pycvodes/include/cvodes_anyode_parallel.hpp` & `pycvodes-0.9.2/pycvodes/include/cvodes_anyode_parallel.hpp`

 * *Files identical despite different names*

### Comparing `pycvodes-0.9.1/pycvodes/include/cvodes_anyode_parallel.pxd` & `pycvodes-0.9.2/pycvodes/include/cvodes_anyode_parallel.pxd`

 * *Files identical despite different names*

### Comparing `pycvodes-0.9.1/pycvodes/include/cvodes_cxx.pxd` & `pycvodes-0.9.2/pycvodes/include/cvodes_cxx.pxd`

 * *Files identical despite different names*

### Comparing `pycvodes-0.9.1/pycvodes/include/cvodes_anyode.pxd` & `pycvodes-0.9.2/pycvodes/include/cvodes_anyode.pxd`

 * *Files identical despite different names*

### Comparing `pycvodes-0.9.1/pycvodes/include/cvodes_cxx.hpp` & `pycvodes-0.9.2/pycvodes/include/cvodes_cxx.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -15,20 +15,34 @@
 #include <unordered_map> // std::unordered_map
 #include <sstream>
 #include <stdlib.h>
 #include <iostream>
 
 #include "sundials_cxx.hpp" // sundials_cxx::nvector_serial::Vector
 #include <cvodes/cvodes_spils.h>
+#if SUNDIALS_VERSION_MAJOR >= 3
+#include <cvodes/cvodes_direct.h> /* CVODE fcts., CV_BDF, CV_ADAMS */
+#include <sunmatrix/sunmatrix_dense.h>
+#include <sunmatrix/sunmatrix_band.h>
+#include <sunmatrix/sunmatrix_sparse.h>
+#include <sunlinsol/sunlinsol_lapackdense.h>
+#include <sunlinsol/sunlinsol_lapackband.h>
+#include <sunlinsol/sunlinsol_spgmr.h>
+#include <sunlinsol/sunlinsol_spbcgs.h>
+#include <sunlinsol/sunlinsol_sptfqmr.h>
+#else
 #include <cvodes/cvodes_spgmr.h>
 #include <cvodes/cvodes_spbcgs.h>
 #include <cvodes/cvodes_sptfqmr.h>
+#include <cvodes/cvodes_lapack.h>       /* prototype for CVDense */
+#define SUNTRUE TRUE
+#define SUNFALSE FALSE
+#endif
 #include <cvodes/cvodes.h> /* CVODE fcts., CV_BDF, CV_ADAMS */
 #include <cvodes/cvodes_impl.h> /* CVodeMem */
-#include <cvodes/cvodes_lapack.h>       /* prototype for CVDense */
 #include <cvodes/cvodes_diag.h>       /* prototype for CVDiag */
 
 
 //pragma STDC FENV_ACCESS on  // GCC 5.4 does not seem to support the pragma
 
 namespace {
     class StreamFmt
@@ -106,14 +120,20 @@
         default:
             throw std::runtime_error("Unhandled flag");
         }
     }
 
     class CVodeIntegrator{ // Thin wrapper class of CVode in CVODES
         FILE *errfp = nullptr;
+#if SUNDIALS_VERSION_MAJOR >= 3
+        SUNMatrix A_ = nullptr;
+        SUNLinearSolver LS_ = nullptr;
+        N_Vector y_ = nullptr;
+        IterLinSolEnum solver_;
+#endif
     public:
         void *mem {nullptr};
         long int ny {0};
         int verbosity = 50;  // "50%" -- plenty of room for future tuning.
         bool autonomous_exprs = false;
         bool record_order = false, record_fpe = false, record_steps = false;
         std::vector<int> orders_seen, fpes_seen;
@@ -124,39 +144,60 @@
                 throw std::bad_alloc(); // "CVodeCreate failed (allocation failed)."
         }
         ~CVodeIntegrator(){
             if (this->mem)
                 CVodeFree(&(this->mem));
             if (this->errfp)
                 fclose(errfp);
+#if SUNDIALS_VERSION_MAJOR >= 3
+            if (this->y_)
+                N_VDestroy(this->y_);
+            if (this->LS_)
+                SUNLinSolFree(this->LS_);
+            if (this->A_)
+                SUNMatDestroy(this->A_);
+#endif
         }
         // init
         void init(CVRhsFn cb, realtype t0, N_Vector y) {
-            int status = CVodeInit(this->mem, cb, t0, y);
+            this->ny = NV_LENGTH_S(y);
+#if SUNDIALS_VERSION_MAJOR >= 3
+            if (y_)
+                throw std::runtime_error("y_ already allocated");
+            y_ = N_VNew_Serial(NV_LENGTH_S(y));
+            std::memcpy(NV_DATA_S(y_), NV_DATA_S(y), ny*sizeof(realtype));
+#else
+            auto y_ = y;
+#endif
+            int status = CVodeInit(this->mem, cb, t0, y_);
             if (status == CV_ILL_INPUT)
                 throw std::runtime_error("CVodeInit failed (CV_ILL_INPUT).");
             else if (status == CV_MEM_FAIL)
                 throw std::bad_alloc(); // "CVodeInit failed (allocation failed).";
             else
                 check_flag(status);
-            this->ny = NV_LENGTH_S(y);
         }
         void init(CVRhsFn cb, realtype t0, SVector &y) {
             this->init(cb, t0, y.n_vec);
         }
         void init(CVRhsFn cb, realtype t0, const realtype * const y, int ny) {
             SVector yvec (ny, const_cast<realtype*>(y));
             this->init(cb, t0, yvec.n_vec);
             // it is ok that yvec is destructed here
             // (see CVodeInit in cvodes.c which at L848 calls cvAllocVectors (L3790))
         }
 
         // reinit
         void reinit(realtype t0, N_Vector y){
-            CVodeReInit(this->mem, t0, y);
+#if SUNDIALS_VERSION_MAJOR >= 3
+            std::memcpy(NV_DATA_S(y_), NV_DATA_S(y), NV_LENGTH_S(y)*sizeof(realtype));
+#else
+            auto y_ = y;
+#endif
+            CVodeReInit(this->mem, t0, y_);
         }
         void reinit(realtype t0, SVector &y){
             reinit(t0, y.n_vec);
         }
         void reinit(realtype t0, const realtype * const y, int ny){
             SVector yvec (ny, const_cast<realtype*>(y));
             reinit(t0, yvec.n_vec);
@@ -241,59 +282,151 @@
         void set_user_data(void *user_data){
             int status = CVodeSetUserData(this->mem, user_data);
             if (status < 0)
                 throw std::runtime_error("CVodeSetUserData failed.");
         }
         // diagonal  solver
         void set_linear_solver_to_diag(){
-            int status = CVDiag(this->mem);
+            int status;
+            status = CVDiag(this->mem);
             if (status < 0)
                 throw std::runtime_error("CVDiag failed.");
         }
 
         // dense jacobian
         void set_linear_solver_to_dense(int ny){
-            int status = CVLapackDense(this->mem, ny);
+            int status;
+#if SUNDIALS_VERSION_MAJOR >= 3
+            if (A_ == nullptr){
+                if (A_)
+                    throw std::runtime_error("matrix already set");
+                A_ = SUNDenseMatrix(ny, ny);
+                if (!A_)
+                    throw std::runtime_error("SUNDenseMatrix failed.");
+            }
+            if (LS_ == nullptr){
+                if (LS_)
+                    throw std::runtime_error("linear solver already set");
+                LS_ = SUNLapackDense(y_, A_);
+                if (!LS_)
+                    throw std::runtime_error("SUNDenseLinearSolver failed.");
+            }
+            status = CVDlsSetLinearSolver(this->mem, LS_, A_);
+            if (status < 0)
+                throw std::runtime_error("CVDlsSetLinearSolver failed.");
+#else
+            status = CVLapackDense(this->mem, ny);
             if (status != CVDLS_SUCCESS)
                 throw std::runtime_error("CVLapackDense failed");
+#endif
         }
-        void set_dense_jac_fn(CVDlsDenseJacFn djac){
-            int status = CVDlsSetDenseJacFn(this->mem, djac);
+        void set_dense_jac_fn(
+#if SUNDIALS_VERSION_MAJOR >= 3
+                              CVDlsJacFn
+#else
+                              CVDlsDenseJacFn
+#endif
+                              djac
+                              ){
+            int status;
+#if SUNDIALS_VERSION_MAJOR >= 3
+            status = CVDlsSetJacFn(this->mem, djac);
+            if (status < 0)
+                throw std::runtime_error("CVDlsSetJacFn failed.");
+#else
+            status = CVDlsSetDenseJacFn(this->mem, djac);
             if (status < 0)
                 throw std::runtime_error("CVDlsSetDenseJacFn failed.");
+#endif
         }
 
         // banded jacobian
         void set_linear_solver_to_banded(int N, int mupper, int mlower){
-            int status = CVLapackBand(this->mem, N, mupper, mlower);
+            int status;
+#if SUNDIALS_VERSION_MAJOR >= 3
+            if (A_ == nullptr){
+                if (A_)
+                    throw std::runtime_error("matrix already set");
+                A_ = SUNBandMatrix(ny, mupper, mlower, std::min(N-1, mlower+mupper));
+                if (!A_)
+                    throw std::runtime_error("SUNDenseMatrix failed.");
+            }
+            if (LS_ == nullptr){
+                if (LS_)
+                    throw std::runtime_error("linear solver already set");
+                LS_ = SUNLapackBand(y_, A_);
+                if (!LS_)
+                    throw std::runtime_error("SUNDenseLinearSolver failed.");
+            }
+            status = CVDlsSetLinearSolver(this->mem, LS_, A_);
+            if (status < 0)
+                throw std::runtime_error("CVDlsSetLinearSolver failed.");
+#else
+            status = CVLapackBand(this->mem, N, mupper, mlower);
             if (status != CVDLS_SUCCESS)
                 throw std::runtime_error("CVLapackBand failed");
+#endif
         }
-        void set_band_jac_fn(CVDlsBandJacFn djac){
-            int status = CVDlsSetBandJacFn(this->mem, djac);
+        void set_band_jac_fn(
+#if SUNDIALS_VERSION_MAJOR >= 3
+                             CVDlsJacFn
+#else
+                             CVDlsBandJacFn
+#endif
+                             djac){
+            int status;
+#if SUNDIALS_VERSION_MAJOR >= 3
+            if (A_ == nullptr or LS_ == nullptr)
+                throw std::runtime_error("set_linear_solver_to_banded not called?");
+            status = CVDlsSetJacFn(this->mem, djac);
+            if (status < 0)
+                throw std::runtime_error("CVDlsSetJacFn failed.");
+#else
+            status = CVDlsSetBandJacFn(this->mem, djac);
             if (status < 0)
                 throw std::runtime_error("CVDlsSetBandJacFn failed.");
+#endif
         }
 
         // Iterative Linear solvers
         void set_linear_solver_to_iterative(IterLinSolEnum solver, int maxl=0, PrecType ptyp=PrecType::Left){
             int flag;
+#if SUNDIALS_VERSION_MAJOR >= 3
+            if (LS_)
+                throw std::runtime_error("linear solver already set.");
+#endif
             switch (solver) {
             case IterLinSolEnum::GMRES:
+#if SUNDIALS_VERSION_MAJOR >= 3
+                LS_ = SUNSPGMR(y_, static_cast<int>(ptyp), maxl);
+#else
                 flag = CVSpgmr(this->mem, static_cast<int>(ptyp), maxl);
+#endif
                 break;
             case IterLinSolEnum::BICGSTAB:
+#if SUNDIALS_VERSION_MAJOR >= 3
+                LS_ = SUNSPBCGS(y_, static_cast<int>(ptyp), maxl);
+#else
                 flag = CVSpbcg(this->mem, static_cast<int>(ptyp), maxl);
                 break;
+#endif
             case IterLinSolEnum::TFQMR:
+#if SUNDIALS_VERSION_MAJOR >= 3
+                LS_ = SUNSPTFQMR(y_, static_cast<int>(ptyp), maxl);
+#else
                 flag = CVSptfqmr(this->mem, static_cast<int>(ptyp), maxl);
                 break;
+#endif
             default:
                 throw std::runtime_error("unknown solver kind.");
             }
+#if SUNDIALS_VERSION_MAJOR >= 3
+            flag = CVSpilsSetLinearSolver(this->mem, LS_);
+            solver_ = solver;
+#endif
             switch (flag){
             case CVSPILS_SUCCESS:
                 break;
             case CVSPILS_MEM_NULL:
                 throw std::runtime_error("set_linear_solver_to_iterative failed (cvode_mem is NULL)");
             case CVSPILS_ILL_INPUT:
                 throw std::runtime_error("PREC_LEFT invalid.");
@@ -309,36 +442,83 @@
                 throw std::runtime_error("cvode_mem is NULL");
             case CVSPILS_LMEM_NULL:
                 throw std::runtime_error("CVSPILS linear solver has not been initialized)");
             }
             if ((check_ill_input) && (flag == CVSPILS_ILL_INPUT))
                 throw std::runtime_error("Bad input.");
         }
-        void set_jac_times_vec_fn(CVSpilsJacTimesVecFn jac_times_vec_fn){
-            int flag = CVSpilsSetJacTimesVecFn(this->mem, jac_times_vec_fn);
+        void set_jac_times_vec_fn(CVSpilsJacTimesVecFn jtimes){
+#if SUNDIALS_VERSION_MAJOR >= 3
+            int flag = CVSpilsSetJacTimes(this->mem, NULL, jtimes);
+#else
+            int flag = CVSpilsSetJacTimesVecFn(this->mem, jtimes);
+#endif
             this->cvspils_check_flag(flag);
         }
+#if SUNDIALS_VERSION_MAJOR >=3
+        void set_jac_times_vec_fn(CVSpilsJacTimesSetupFn jtsetup,
+                                  CVSpilsJacTimesVecFn jtimes){
+            int flag = CVSpilsSetJacTimes(this->mem, jtsetup, jtimes);
+            this->cvspils_check_flag(flag);
+        }
+#endif
         void set_preconditioner(CVSpilsPrecSetupFn setup_fn, CVSpilsPrecSolveFn solve_fn){
             int flag = CVSpilsSetPreconditioner(this->mem, setup_fn, solve_fn);
             this->cvspils_check_flag(flag);
         }
         void set_iter_eps_lin(realtype delta){
             int flag = CVSpilsSetEpsLin(this->mem, delta);
             this->cvspils_check_flag(flag, true);
         }
         void set_prec_type(PrecType pretyp){
-            int flag = CVSpilsSetPrecType(this->mem, (int)pretyp);
+            int flag;
+#if SUNDIALS_VERSION_MAJOR >= 3
+            switch(solver_){
+            case IterLinSolEnum::GMRES:
+                flag = SUNSPGMRSetPrecType(LS_, (int)pretyp); break;
+            case IterLinSolEnum::BICGSTAB:
+                flag = SUNSPBCGSSetPrecType(LS_, (int)pretyp); break;
+            case IterLinSolEnum::TFQMR:
+                flag = SUNSPTFQMRSetPrecType(LS_, (int)pretyp); break;
+            default:
+                throw std::runtime_error("unknown solver kind.");
+            }
+#else
+            flag = CVSpilsSetPrecType(this->mem, (int)pretyp);
+#endif
             this->cvspils_check_flag(flag, true);
         }
         void set_gram_schmidt_type(GramSchmidtType gs_type){
-            int flag = CVSpilsSetGSType(this->mem, (int)gs_type);
+            int flag;
+#if SUNDIALS_VERSION_MAJOR >= 3
+            if (solver_ == IterLinSolEnum::GMRES)
+                flag = SUNSPGMRSetGSType(LS_, (int)gs_type);
+            else
+                throw std::runtime_error("Setting Gram-Schmidt type only makes sense for GMRES");
+#else
+            flag = CVSpilsSetGSType(this->mem, (int)gs_type);
+#endif
             this->cvspils_check_flag(flag, true);
         }
         void set_krylov_max_len(int maxl){
-            int flag = CVSpilsSetMaxl(this->mem, maxl);
+            int flag;
+#if SUNDIALS_VERSION_MAJOR >= 3
+            switch(solver_){
+            case IterLinSolEnum::GMRES:
+                throw std::runtime_error("GMRES has no max length option");
+            case IterLinSolEnum::BICGSTAB:
+                flag = SUNSPBCGSSetMaxl(LS_, maxl); break;
+            case IterLinSolEnum::TFQMR:
+                flag = SUNSPTFQMRSetMaxl(LS_, maxl); break;
+            default:
+                throw std::runtime_error("unknown solver kind.");
+            }
+#else
+            flag = CVSpilsSetMaxl(this->mem, maxl);
+#endif
             this->cvspils_check_flag(flag);
         }
         int get_current_order() {
             int qcur;
             CVodeGetCurrentOrder(this->mem, &qcur);
             return qcur;
         }
```

### Comparing `pycvodes-0.9.1/pycvodes/include/cvodes_anyode_nogil.pxd` & `pycvodes-0.9.2/pycvodes/include/cvodes_anyode_nogil.pxd`

 * *Files identical despite different names*

### Comparing `pycvodes-0.9.1/pycvodes/include/sundials_cxx.hpp` & `pycvodes-0.9.2/pycvodes/include/sundials_cxx.hpp`

 * *Files identical despite different names*

### Comparing `pycvodes-0.9.1/PKG-INFO` & `pycvodes-0.9.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 1.1
 Name: pycvodes
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python binding for cvodes from the sundials library.
 Home-page: https://github.com/bjodah/pycvodes
 Author: Bjoern I. Dahlgren
 Author-email: bjodah@gmail.com
 License: BSD
 Description-Content-Type: UNKNOWN
 Description: pycvodes
         ========
         
         .. image:: http://hera.physchem.kth.se:9090/api/badges/bjodah/pycvodes/status.svg
            :target: http://hera.physchem.kth.se:9090/bjodah/pycvodes
-           :alt: Build status
+           :alt: Build status on private Drone server
+        .. image:: https://circleci.com/gh/bjodah/pycvodes.svg?style=svg
+           :target: https://circleci.com/gh/bjodah/pycvodes
+           :alt: Build status on CircleCI
+        .. image:: https://secure.travis-ci.org/bjodah/pycvodes.svg?branch=master
+           :target: http://travis-ci.org/bjodah/pycvodes
+           :alt: Build status on Travis-CI
         .. image:: https://img.shields.io/pypi/v/pycvodes.svg
            :target: https://pypi.python.org/pypi/pycvodes
            :alt: PyPI version
         .. image:: https://img.shields.io/pypi/l/pycvodes.svg
            :target: https://github.com/bjodah/pycvodes/blob/master/LICENSE
            :alt: License
         .. image:: http://hera.physchem.kth.se/~pycvodes/branches/master/htmlcov/coverage.svg
@@ -25,26 +31,31 @@
         .. image:: https://zenodo.org/badge/43224425.svg
            :target: https://zenodo.org/badge/latestdoi/43224425
         
         `pycvodes <https://github.com/bjodah/pycvodes>`_ provides a
         `Python <http://www.python.org>`_ binding to the
         `Ordinary Differential Equation <https://en.wikipedia.org/wiki/Ordinary_differential_equation>`_
         integration routines from `cvodes <https://computation.llnl.gov/casc/sundials/description/description.html#descr_cvodes>`_ in the
-        `SUNDIALS suite <https://computation.llnl.gov/casc/sundials/main.html>`_. ``pcyvodes`` allows a user to numerically integrate
+        `SUNDIALS suite <https://computation.llnl.gov/casc/sundials/main.html>`_. ``pycvodes`` allows a user to numerically integrate
         (systems of) differential equations. Note that routines for sensitivity analysis is not yet exposed in this binding (which makes
         the functionality essentially the same as cvode). 
         
         The following multistep methods are available:
         
         - ``bdf``: Backward differentiation formula (of order 1 to 5)
         - ``adams``: implicit Adams method (order 1 to 12)
         
         Note that bdf (as an implicit stepper) requires a user supplied
         callback for calculating the jacobian.
         
+        You may also want to know that you can use ``pycvodes`` from
+        `pyodesys <https://github.com/bjodah/pyodesys>`_
+        which can e.g. derive the Jacobian analytically for you (pyodesys also provides
+        plotting functions, C++ code-generation and more).
+        
         Documentation
         -------------
         Autogenerated API documentation for latest stable release is found here:
         `<https://bjodah.github.io/pycvodes/latest>`_
         (and the development version for the current master branch are found here:
         `<http://hera.physchem.kth.se/~pycvodes/branches/master/html>`_).
         
@@ -70,14 +81,16 @@
         
         .. code:: python
         
            >>> from pycvodes import _config
            >>> _config.env['LAPACK']  # doctest: +SKIP
            'lapack,blas'
         
+        If you use ``pip`` to install ``pycvodes`` note that you will need to install sundials
+        (and its development headers, with cvodes enabled) prior to installing pycvodes.
         
         Examples
         --------
         The classic van der Pol oscillator (see `examples/van_der_pol.py <examples/van_der_pol.py>`_)
         
         .. code:: python
```

### Comparing `pycvodes-0.9.1/README.rst` & `pycvodes-0.9.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 pycvodes
 ========
 
 .. image:: http://hera.physchem.kth.se:9090/api/badges/bjodah/pycvodes/status.svg
    :target: http://hera.physchem.kth.se:9090/bjodah/pycvodes
-   :alt: Build status
+   :alt: Build status on private Drone server
+.. image:: https://circleci.com/gh/bjodah/pycvodes.svg?style=svg
+   :target: https://circleci.com/gh/bjodah/pycvodes
+   :alt: Build status on CircleCI
+.. image:: https://secure.travis-ci.org/bjodah/pycvodes.svg?branch=master
+   :target: http://travis-ci.org/bjodah/pycvodes
+   :alt: Build status on Travis-CI
 .. image:: https://img.shields.io/pypi/v/pycvodes.svg
    :target: https://pypi.python.org/pypi/pycvodes
    :alt: PyPI version
 .. image:: https://img.shields.io/pypi/l/pycvodes.svg
    :target: https://github.com/bjodah/pycvodes/blob/master/LICENSE
    :alt: License
 .. image:: http://hera.physchem.kth.se/~pycvodes/branches/master/htmlcov/coverage.svg
@@ -16,26 +22,31 @@
 .. image:: https://zenodo.org/badge/43224425.svg
    :target: https://zenodo.org/badge/latestdoi/43224425
 
 `pycvodes <https://github.com/bjodah/pycvodes>`_ provides a
 `Python <http://www.python.org>`_ binding to the
 `Ordinary Differential Equation <https://en.wikipedia.org/wiki/Ordinary_differential_equation>`_
 integration routines from `cvodes <https://computation.llnl.gov/casc/sundials/description/description.html#descr_cvodes>`_ in the
-`SUNDIALS suite <https://computation.llnl.gov/casc/sundials/main.html>`_. ``pcyvodes`` allows a user to numerically integrate
+`SUNDIALS suite <https://computation.llnl.gov/casc/sundials/main.html>`_. ``pycvodes`` allows a user to numerically integrate
 (systems of) differential equations. Note that routines for sensitivity analysis is not yet exposed in this binding (which makes
 the functionality essentially the same as cvode). 
 
 The following multistep methods are available:
 
 - ``bdf``: Backward differentiation formula (of order 1 to 5)
 - ``adams``: implicit Adams method (order 1 to 12)
 
 Note that bdf (as an implicit stepper) requires a user supplied
 callback for calculating the jacobian.
 
+You may also want to know that you can use ``pycvodes`` from
+`pyodesys <https://github.com/bjodah/pyodesys>`_
+which can e.g. derive the Jacobian analytically for you (pyodesys also provides
+plotting functions, C++ code-generation and more).
+
 Documentation
 -------------
 Autogenerated API documentation for latest stable release is found here:
 `<https://bjodah.github.io/pycvodes/latest>`_
 (and the development version for the current master branch are found here:
 `<http://hera.physchem.kth.se/~pycvodes/branches/master/html>`_).
 
@@ -61,14 +72,16 @@
 
 .. code:: python
 
    >>> from pycvodes import _config
    >>> _config.env['LAPACK']  # doctest: +SKIP
    'lapack,blas'
 
+If you use ``pip`` to install ``pycvodes`` note that you will need to install sundials
+(and its development headers, with cvodes enabled) prior to installing pycvodes.
 
 Examples
 --------
 The classic van der Pol oscillator (see `examples/van_der_pol.py <examples/van_der_pol.py>`_)
 
 .. code:: python
```

### Comparing `pycvodes-0.9.1/LICENSE` & `pycvodes-0.9.2/LICENSE`

 * *Files identical despite different names*

