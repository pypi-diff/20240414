# Comparing `tmp/pyodeint-0.9.7.tar.gz` & `tmp/pyodeint-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyodeint-0.9.7.tar", last modified: Sun Jul 29 16:57:50 2018, max compression
+gzip compressed data, was "dist/pyodeint-0.9.8.tar", last modified: Sun Jul 29 19:29:38 2018, max compression
```

## Comparing `pyodeint-0.9.7.tar` & `pyodeint-0.9.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 16:57:50.000000 pyodeint-0.9.7/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       38 2018-07-29 12:45:55.000000 pyodeint-0.9.7/AUTHORS
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2273 2018-07-29 16:54:03.000000 pyodeint-0.9.7/CHANGES.rst
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1303 2018-07-29 12:45:55.000000 pyodeint-0.9.7/LICENSE
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      126 2018-07-29 12:45:55.000000 pyodeint-0.9.7/MANIFEST.in
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5765 2018-07-29 16:57:50.000000 pyodeint-0.9.7/PKG-INFO
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4287 2018-07-29 12:46:00.000000 pyodeint-0.9.7/README.rst
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 16:57:50.000000 pyodeint-0.9.7/external/
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 16:57:50.000000 pyodeint-0.9.7/external/anyode/
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 16:57:50.000000 pyodeint-0.9.7/external/anyode/cython_def/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      608 2018-07-29 16:53:07.000000 pyodeint-0.9.7/external/anyode/cython_def/anyode.pxd
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      812 2018-07-29 16:53:07.000000 pyodeint-0.9.7/external/anyode/cython_def/anyode_numpy.pxd
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 16:57:50.000000 pyodeint-0.9.7/external/anyode/include/
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 16:57:50.000000 pyodeint-0.9.7/external/anyode/include/anyode/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     9884 2018-07-29 16:52:58.000000 pyodeint-0.9.7/external/anyode/include/anyode/anyode.hpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    12205 2018-07-29 16:52:58.000000 pyodeint-0.9.7/external/anyode/include/anyode/anyode_numpy.hpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      738 2018-07-29 16:52:58.000000 pyodeint-0.9.7/external/anyode/include/anyode/anyode_parallel.hpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      433 2018-07-29 16:52:58.000000 pyodeint-0.9.7/external/anyode/include/anyode/anyode_util.hpp
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 16:57:50.000000 pyodeint-0.9.7/pyodeint/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5246 2018-07-29 12:45:55.000000 pyodeint-0.9.7/pyodeint/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)   468345 2018-07-29 16:54:47.000000 pyodeint-0.9.7/pyodeint/_odeint.cpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       22 2018-07-29 16:57:50.000000 pyodeint-0.9.7/pyodeint/_release.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2019 2018-07-29 12:45:55.000000 pyodeint-0.9.7/pyodeint/_util.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 16:57:50.000000 pyodeint-0.9.7/pyodeint/include/
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 16:57:50.000000 pyodeint-0.9.7/pyodeint/include/boost/
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 16:57:50.000000 pyodeint-0.9.7/pyodeint/include/boost/numeric/
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 16:57:50.000000 pyodeint-0.9.7/pyodeint/include/boost/numeric/odeint/
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 16:57:50.000000 pyodeint-0.9.7/pyodeint/include/boost/numeric/odeint/stepper/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     7520 2018-07-29 12:45:55.000000 pyodeint-0.9.7/pyodeint/include/boost/numeric/odeint/stepper/rosenbrock4_controller.hpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    21375 2018-07-29 12:46:00.000000 pyodeint-0.9.7/pyodeint/include/odeint_anyode.hpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1246 2018-07-29 12:45:55.000000 pyodeint-0.9.7/pyodeint/include/odeint_anyode.pxd
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1238 2018-07-29 12:45:55.000000 pyodeint-0.9.7/pyodeint/include/odeint_anyode_nogil.pxd
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3295 2018-07-29 12:45:55.000000 pyodeint-0.9.7/pyodeint/include/odeint_anyode_parallel.hpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      870 2018-07-29 12:45:55.000000 pyodeint-0.9.7/pyodeint/include/odeint_anyode_parallel.pxd
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 16:57:50.000000 pyodeint-0.9.7/pyodeint/tests/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 12:45:55.000000 pyodeint-0.9.7/pyodeint/tests/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6832 2018-07-29 12:45:55.000000 pyodeint-0.9.7/pyodeint/tests/test_odeint_numpy.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 16:57:50.000000 pyodeint-0.9.7/pyodeint.egg-info/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5765 2018-07-29 16:57:50.000000 pyodeint-0.9.7/pyodeint.egg-info/PKG-INFO
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      914 2018-07-29 16:57:50.000000 pyodeint-0.9.7/pyodeint.egg-info/SOURCES.txt
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        1 2018-07-29 16:57:50.000000 pyodeint-0.9.7/pyodeint.egg-info/dependency_links.txt
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       45 2018-07-29 16:57:50.000000 pyodeint-0.9.7/pyodeint.egg-info/requires.txt
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        9 2018-07-29 16:57:50.000000 pyodeint-0.9.7/pyodeint.egg-info/top_level.txt
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      255 2018-07-29 16:57:50.000000 pyodeint-0.9.7/setup.cfg
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)     4428 2018-07-29 12:46:00.000000 pyodeint-0.9.7/setup.py
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 19:29:38.000000 pyodeint-0.9.8/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       38 2018-07-29 17:12:28.000000 pyodeint-0.9.8/AUTHORS
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2310 2018-07-29 19:29:01.000000 pyodeint-0.9.8/CHANGES.rst
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1303 2018-07-29 17:12:28.000000 pyodeint-0.9.8/LICENSE
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      126 2018-07-29 17:12:28.000000 pyodeint-0.9.8/MANIFEST.in
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5765 2018-07-29 19:29:38.000000 pyodeint-0.9.8/PKG-INFO
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4287 2018-07-29 17:12:28.000000 pyodeint-0.9.8/README.rst
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 19:29:38.000000 pyodeint-0.9.8/external/
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 19:29:38.000000 pyodeint-0.9.8/external/anyode/
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 19:29:38.000000 pyodeint-0.9.8/external/anyode/cython_def/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      608 2018-07-29 17:12:28.000000 pyodeint-0.9.8/external/anyode/cython_def/anyode.pxd
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      812 2018-07-29 17:12:28.000000 pyodeint-0.9.8/external/anyode/cython_def/anyode_numpy.pxd
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 19:29:38.000000 pyodeint-0.9.8/external/anyode/include/
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 19:29:38.000000 pyodeint-0.9.8/external/anyode/include/anyode/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     9884 2018-07-29 17:12:28.000000 pyodeint-0.9.8/external/anyode/include/anyode/anyode.hpp
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    12205 2018-07-29 17:12:28.000000 pyodeint-0.9.8/external/anyode/include/anyode/anyode_numpy.hpp
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      738 2018-07-29 17:12:28.000000 pyodeint-0.9.8/external/anyode/include/anyode/anyode_parallel.hpp
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      433 2018-07-29 17:12:28.000000 pyodeint-0.9.8/external/anyode/include/anyode/anyode_util.hpp
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 19:29:38.000000 pyodeint-0.9.8/pyodeint/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5246 2018-07-29 17:12:28.000000 pyodeint-0.9.8/pyodeint/__init__.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)   468345 2018-07-29 19:29:23.000000 pyodeint-0.9.8/pyodeint/_odeint.cpp
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       22 2018-07-29 19:29:38.000000 pyodeint-0.9.8/pyodeint/_release.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2019 2018-07-29 17:12:28.000000 pyodeint-0.9.8/pyodeint/_util.py
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 19:29:38.000000 pyodeint-0.9.8/pyodeint/include/
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 19:29:38.000000 pyodeint-0.9.8/pyodeint/include/boost/
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 19:29:38.000000 pyodeint-0.9.8/pyodeint/include/boost/numeric/
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 19:29:38.000000 pyodeint-0.9.8/pyodeint/include/boost/numeric/odeint/
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 19:29:38.000000 pyodeint-0.9.8/pyodeint/include/boost/numeric/odeint/stepper/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     7520 2018-07-29 17:12:28.000000 pyodeint-0.9.8/pyodeint/include/boost/numeric/odeint/stepper/rosenbrock4_controller.hpp
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    21423 2018-07-29 19:28:08.000000 pyodeint-0.9.8/pyodeint/include/odeint_anyode.hpp
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1246 2018-07-29 17:12:28.000000 pyodeint-0.9.8/pyodeint/include/odeint_anyode.pxd
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1238 2018-07-29 17:12:28.000000 pyodeint-0.9.8/pyodeint/include/odeint_anyode_nogil.pxd
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3295 2018-07-29 17:12:28.000000 pyodeint-0.9.8/pyodeint/include/odeint_anyode_parallel.hpp
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      870 2018-07-29 17:12:28.000000 pyodeint-0.9.8/pyodeint/include/odeint_anyode_parallel.pxd
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 19:29:38.000000 pyodeint-0.9.8/pyodeint/tests/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 17:12:28.000000 pyodeint-0.9.8/pyodeint/tests/__init__.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6832 2018-07-29 17:12:28.000000 pyodeint-0.9.8/pyodeint/tests/test_odeint_numpy.py
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2018-07-29 19:29:38.000000 pyodeint-0.9.8/pyodeint.egg-info/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5765 2018-07-29 19:29:38.000000 pyodeint-0.9.8/pyodeint.egg-info/PKG-INFO
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      914 2018-07-29 19:29:38.000000 pyodeint-0.9.8/pyodeint.egg-info/SOURCES.txt
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        1 2018-07-29 19:29:38.000000 pyodeint-0.9.8/pyodeint.egg-info/dependency_links.txt
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       45 2018-07-29 19:29:38.000000 pyodeint-0.9.8/pyodeint.egg-info/requires.txt
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        9 2018-07-29 19:29:38.000000 pyodeint-0.9.8/pyodeint.egg-info/top_level.txt
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      255 2018-07-29 19:29:38.000000 pyodeint-0.9.8/setup.cfg
+-rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)     4428 2018-07-29 17:12:28.000000 pyodeint-0.9.8/setup.py
```

### Comparing `pyodeint-0.9.7/CHANGES.rst` & `pyodeint-0.9.8/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+v0.9.8
+======
+- Fix MSVC __restrict
+
 v0.9.7
 ======
 - Fix MSVC for AnyODE 16+
 
 v0.9.6
 ======
 - Maintainence release of 0.9.x branch
```

### Comparing `pyodeint-0.9.7/LICENSE` & `pyodeint-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodeint-0.9.7/PKG-INFO` & `pyodeint-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodeint
-Version: 0.9.7
+Version: 0.9.8
 Summary: Python binding for odeint from boost.
 Home-page: https://github.com/bjodah/pyodeint
 Author: Björn Dahlgren
 Author-email: bjodah@DELETEMEgmail.com
 License: BSD
 Description: pyodeint
         ========
```

### Comparing `pyodeint-0.9.7/README.rst` & `pyodeint-0.9.8/README.rst`

 * *Files identical despite different names*

### Comparing `pyodeint-0.9.7/external/anyode/cython_def/anyode.pxd` & `pyodeint-0.9.8/external/anyode/cython_def/anyode.pxd`

 * *Files identical despite different names*

### Comparing `pyodeint-0.9.7/external/anyode/cython_def/anyode_numpy.pxd` & `pyodeint-0.9.8/external/anyode/cython_def/anyode_numpy.pxd`

 * *Files identical despite different names*

### Comparing `pyodeint-0.9.7/external/anyode/include/anyode/anyode.hpp` & `pyodeint-0.9.8/external/anyode/include/anyode/anyode.hpp`

 * *Files identical despite different names*

### Comparing `pyodeint-0.9.7/external/anyode/include/anyode/anyode_numpy.hpp` & `pyodeint-0.9.8/external/anyode/include/anyode/anyode_numpy.hpp`

 * *Files identical despite different names*

### Comparing `pyodeint-0.9.7/external/anyode/include/anyode/anyode_parallel.hpp` & `pyodeint-0.9.8/external/anyode/include/anyode/anyode_parallel.hpp`

 * *Files identical despite different names*

### Comparing `pyodeint-0.9.7/pyodeint/__init__.py` & `pyodeint-0.9.8/pyodeint/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodeint-0.9.7/pyodeint/_odeint.cpp` & `pyodeint-0.9.8/pyodeint/_odeint.cpp`

 * *Files identical despite different names*

### Comparing `pyodeint-0.9.7/pyodeint/_util.py` & `pyodeint-0.9.8/pyodeint/_util.py`

 * *Files identical despite different names*

### Comparing `pyodeint-0.9.7/pyodeint/include/boost/numeric/odeint/stepper/rosenbrock4_controller.hpp` & `pyodeint-0.9.8/pyodeint/include/boost/numeric/odeint/stepper/rosenbrock4_controller.hpp`

 * *Files identical despite different names*

### Comparing `pyodeint-0.9.7/pyodeint/include/odeint_anyode.hpp` & `pyodeint-0.9.8/pyodeint/include/odeint_anyode.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -119,15 +119,15 @@
                long int mxsteps, int autorestart=0, bool return_on_error=false) :
             m_odesys(odesys), m_dx0(dx0), m_dx_max(dx_max), m_atol(atol), m_rtol(rtol), m_styp(styp),
             m_mxsteps(mxsteps), m_autorestart(autorestart), m_return_on_error(return_on_error) {}
 
         std::pair<std::vector<value_type>, std::vector<value_type> >
         adaptive(const value_type x0,
                  const value_type xend,
-                 const value_type * const __restrict__ y0){
+                 const value_type * const ANYODE_RESTRICT y0){
             std::time_t cputime0 = std::clock();
             auto t_start = std::chrono::high_resolution_clock::now();
             std::pair<std::vector<value_type>, std::vector<value_type> > result;
             try{
                 if ( m_styp == StepType::bulirsch_stoer ) {
                     this->adaptive_bulirsch_stoer(x0, xend, y0);
                 } else if ( m_styp == StepType::dopri5 ) {
@@ -168,17 +168,17 @@
                 std::chrono::high_resolution_clock::now() - t_start).count();
             return std::make_pair(this->m_xout, this->m_yout);
         impossible_adaptive:
             throw std::runtime_error("Impossible: unknown StepType!");
         }
 
         int predefined(const int nx,
-                       const value_type * const __restrict__ xout,
-                       const value_type * const __restrict__ y0,
-                       value_type * const __restrict__ yout){
+                       const value_type * const ANYODE_RESTRICT xout,
+                       const value_type * const ANYODE_RESTRICT y0,
+                       value_type * const ANYODE_RESTRICT yout){
             int nreached;
             std::time_t cputime0 = std::clock();
             auto t_start = std::chrono::high_resolution_clock::now();
             std::copy(y0, y0 + (this->m_odesys->get_ny()), yout);
             try {
                 if ( m_styp == StepType::bulirsch_stoer ) {
                     this->predefined_bulirsch_stoer(nx, xout, y0, yout, &nreached);
@@ -240,32 +240,32 @@
             if (this->m_nsteps == this->m_mxsteps)
                 throw std::runtime_error(StreamFmt() << "Maximum number of steps reached: " << this->m_nsteps);
             m_nsteps++;
         }
 
         void adaptive_bulirsch_stoer(const value_type x0,
                                      const value_type xend,
-                                     const value_type * const __restrict__ y0
+                                     const value_type * const ANYODE_RESTRICT y0
                                      ){
             const int ny = this->m_odesys->get_ny();
             auto f = [&](const vector_type &yarr, vector_type &dydx, value_type xval) {
                 this->m_odesys->rhs(xval, &(yarr.data()[0]), &(dydx.data()[0]));
             };
             auto stepper = bulirsch_stoer_dense_out< vector_type, value_type >(
                 this->m_atol, this->m_rtol, 1.0, 1.0, this->m_dx_max);
             auto y_ = vec_from_ptr(y0, ny);
             this->reset();
             integrate_adaptive(stepper, f, y_, x0, xend, this->m_dx0,
                                std::bind(&Integr::obs_adaptive, this, _1, _2));
         }
 
         void predefined_bulirsch_stoer(const int nx,
-                                       const value_type * const __restrict__ xout,
-                                       const value_type * const __restrict__ y0,
-                                       value_type * const __restrict__ yout,
+                                       const value_type * const ANYODE_RESTRICT xout,
+                                       const value_type * const ANYODE_RESTRICT y0,
+                                       value_type * const ANYODE_RESTRICT yout,
                                        int * nreached){
             *nreached = 0;
             const auto ny = this->m_odesys->get_ny();
             vector_type y_ = vec_from_ptr(y0, ny);
             vector_type xout_ = vec_from_ptr(xout, nx);
             auto f = [&](const vector_type &yarr, vector_type &dydx, value_type xval) {
                 this->m_odesys->rhs(xval, &(yarr.data()[0]), &(dydx.data()[0]));
@@ -288,32 +288,32 @@
                 if (!m_return_on_error)
                     throw;
             }
         }
 
         void adaptive_dopri5(const value_type x0,
                              const value_type xend,
-                             const value_type * const __restrict__ y0){
+                             const value_type * const ANYODE_RESTRICT y0){
             const int ny = this->m_odesys->get_ny();
             auto f = [&](const vector_type &yarr, vector_type &dydx, value_type xval) {
                 this->m_odesys->rhs(xval, &(yarr.data()[0]), &(dydx.data()[0]));
             };
 
             auto stepper = make_dense_output<runge_kutta_dopri5<vector_type, value_type> >(
                 this->m_atol, this->m_rtol, this->m_dx_max);
             auto y_ = vec_from_ptr(y0, ny);
             this->reset();
             integrate_adaptive(stepper, f, y_, x0, xend, this->m_dx0,
                                std::bind(&Integr::obs_adaptive, this, _1, _2));
         }
 
         void predefined_dopri5(const int nx,
-                               const value_type * const __restrict__ xout,
-                               const value_type * const __restrict__ y0,
-                              value_type * const __restrict__ yout,
+                               const value_type * const ANYODE_RESTRICT xout,
+                               const value_type * const ANYODE_RESTRICT y0,
+                              value_type * const ANYODE_RESTRICT yout,
                               int * nreached){
             *nreached = 0;
             const auto ny = this->m_odesys->get_ny();
             vector_type y_ = vec_from_ptr(y0, ny);
             vector_type xout_ = vec_from_ptr(xout, nx);
             auto f = [&](const vector_type &yarr, vector_type &dydx, value_type xval) {
                 this->m_odesys->rhs(xval, &(yarr.data()[0]), &(dydx.data()[0]));
@@ -336,15 +336,15 @@
                 if (!m_return_on_error)
                     throw;
             }
         }
 
         void adaptive_rosenbrock4(const value_type x0,
                                   const value_type xend,
-                                  const value_type * const __restrict__ y0){
+                                  const value_type * const ANYODE_RESTRICT y0){
             const int ny = this->m_odesys->get_ny();
             auto f = [&](const vector_type &yarr, vector_type &dydx, value_type xval) {
                 this->m_odesys->rhs(xval, &(yarr.data()[0]), &(dydx.data()[0]));
             };
             auto j = [&](const vector_type & yarr, matrix_type &Jmat,
                                      const value_type & xval, vector_type &dfdx) {
                 this->m_odesys->dense_jac_rmaj(xval, &(yarr.data()[0]), nullptr, &(Jmat.data()[0]), ny, &(dfdx.data()[0]));
@@ -353,17 +353,17 @@
             auto y_ = vec_from_ptr(y0, ny);
             this->reset();
             integrate_adaptive(stepper, std::make_pair(f, j), y_, x0, xend, this->m_dx0,
                                               std::bind(&Integr::obs_adaptive, this, _1, _2));
         }
 
         void predefined_rosenbrock4(const int nx,
-                                    const value_type * const __restrict__ xout,
-                                    const value_type * const __restrict__ y0,
-                                    value_type * const __restrict__ yout,
+                                    const value_type * const ANYODE_RESTRICT xout,
+                                    const value_type * const ANYODE_RESTRICT y0,
+                                    value_type * const ANYODE_RESTRICT yout,
                                     int * nreached){
             *nreached = 0;
             const auto ny = this->m_odesys->get_ny();
             vector_type y_ = vec_from_ptr(y0, ny);
             vector_type xout_ = vec_from_ptr(xout, nx);
             auto f = [&](const vector_type &yarr, vector_type &dydx, value_type xval) {
                 this->m_odesys->rhs(xval, &(yarr.data()[0]), &(dydx.data()[0]));
```

### Comparing `pyodeint-0.9.7/pyodeint/include/odeint_anyode.pxd` & `pyodeint-0.9.8/pyodeint/include/odeint_anyode.pxd`

 * *Files identical despite different names*

### Comparing `pyodeint-0.9.7/pyodeint/include/odeint_anyode_nogil.pxd` & `pyodeint-0.9.8/pyodeint/include/odeint_anyode_nogil.pxd`

 * *Files identical despite different names*

### Comparing `pyodeint-0.9.7/pyodeint/include/odeint_anyode_parallel.hpp` & `pyodeint-0.9.8/pyodeint/include/odeint_anyode_parallel.hpp`

 * *Files identical despite different names*

### Comparing `pyodeint-0.9.7/pyodeint/include/odeint_anyode_parallel.pxd` & `pyodeint-0.9.8/pyodeint/include/odeint_anyode_parallel.pxd`

 * *Files identical despite different names*

### Comparing `pyodeint-0.9.7/pyodeint/tests/test_odeint_numpy.py` & `pyodeint-0.9.8/pyodeint/tests/test_odeint_numpy.py`

 * *Files identical despite different names*

### Comparing `pyodeint-0.9.7/pyodeint.egg-info/PKG-INFO` & `pyodeint-0.9.8/pyodeint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodeint
-Version: 0.9.7
+Version: 0.9.8
 Summary: Python binding for odeint from boost.
 Home-page: https://github.com/bjodah/pyodeint
 Author: Björn Dahlgren
 Author-email: bjodah@DELETEMEgmail.com
 License: BSD
 Description: pyodeint
         ========
```

### Comparing `pyodeint-0.9.7/pyodeint.egg-info/SOURCES.txt` & `pyodeint-0.9.8/pyodeint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyodeint-0.9.7/setup.py` & `pyodeint-0.9.8/setup.py`

 * *Files identical despite different names*

