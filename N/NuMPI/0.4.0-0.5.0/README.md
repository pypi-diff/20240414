# Comparing `tmp/numpi-0.4.0.tar.gz` & `tmp/numpi-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpi-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "numpi-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `numpi-0.4.0.tar` & `numpi-0.5.0.tar`

### file list

```diff
@@ -1,62 +1,18 @@
--rw-r--r--   0        0        0      522 2024-01-13 23:24:39.075760 numpi-0.4.0/.check_netcdf_capabilities.py
--rw-r--r--   0        0        0       31 2024-01-13 23:24:39.075760 numpi-0.4.0/.gitattributes
--rw-r--r--   0        0        0      437 2024-01-13 23:24:39.075760 numpi-0.4.0/.github/workflows/flake8.yml
--rw-r--r--   0        0        0     1105 2024-01-13 23:24:39.075760 numpi-0.4.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2366 2024-01-13 23:24:39.075760 numpi-0.4.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      106 2024-01-13 23:24:39.075760 numpi-0.4.0/.gitignore
--rw-r--r--   0        0        0      105 2024-01-13 23:24:39.075760 numpi-0.4.0/AUTHORS
--rw-r--r--   0        0        0     2034 2024-01-13 23:24:39.075760 numpi-0.4.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1506 2024-01-13 23:24:39.075760 numpi-0.4.0/ChangeLog.md
--rw-r--r--   0        0        0     1041 2024-01-13 23:24:39.075760 numpi-0.4.0/LICENSE.md
--rw-r--r--   0        0        0       79 2024-01-13 23:24:39.075760 numpi-0.4.0/MANIFEST.in
--rw-r--r--   0        0        0      634 2024-01-13 23:24:39.075760 numpi-0.4.0/NEMO_test_job.sh
--rw-r--r--   0        0        0     2684 2024-01-13 23:24:39.075760 numpi-0.4.0/NuMPI/DiscoverVersion.py
--rw-r--r--   0        0        0    10241 2024-01-13 23:24:39.075760 numpi-0.4.0/NuMPI/IO/MPIFileIO.py
--rw-r--r--   0        0        0    17465 2024-01-13 23:24:39.075760 numpi-0.4.0/NuMPI/IO/NetCDF.py
--rw-r--r--   0        0        0     1294 2024-01-13 23:24:39.075760 numpi-0.4.0/NuMPI/IO/__init__.py
--rw-r--r--   0        0        0     7465 2024-01-13 23:24:39.075760 numpi-0.4.0/NuMPI/MPIStub.py
--rw-r--r--   0        0        0    12486 2024-01-13 23:24:39.075760 numpi-0.4.0/NuMPI/Optimization/MPI_LBFGS_Matrix_H.py
--rw-r--r--   0        0        0     2129 2024-01-13 23:24:39.075760 numpi-0.4.0/NuMPI/Optimization/Wolfe.py
--rw-r--r--   0        0        0     1202 2024-01-13 23:24:39.075760 numpi-0.4.0/NuMPI/Optimization/__init__.py
--rw-r--r--   0        0        0     7670 2024-01-13 23:24:39.075760 numpi-0.4.0/NuMPI/Optimization/ccg_with_restart.py
--rw-r--r--   0        0        0     8232 2024-01-13 23:24:39.075760 numpi-0.4.0/NuMPI/Optimization/ccg_without_restart.py
--rw-r--r--   0        0        0    11946 2024-01-13 23:24:39.075760 numpi-0.4.0/NuMPI/Optimization/linesearch.py
--rw-r--r--   0        0        0     1668 2024-01-13 23:24:39.075760 numpi-0.4.0/NuMPI/Optimization/result.py
--rw-r--r--   0        0        0     6188 2024-01-13 23:24:39.075760 numpi-0.4.0/NuMPI/Tools/Reduction.py
--rw-r--r--   0        0        0     1198 2024-01-13 23:24:39.075760 numpi-0.4.0/NuMPI/Tools/__init__.py
--rw-r--r--   0        0        0     1571 2024-01-13 23:24:39.075760 numpi-0.4.0/NuMPI/__init__.py
--rw-r--r--   0        0        0     2078 2024-01-13 23:24:39.075760 numpi-0.4.0/README.md
--rwxr-xr-x   0        0        0      594 2024-01-13 23:24:39.075760 numpi-0.4.0/env.sh
--rw-r--r--   0        0        0    14652 2024-01-13 23:24:39.075760 numpi-0.4.0/examples/IO/append_data_to_existing_netcdf_file.ipynb
--rw-r--r--   0        0        0    53531 2024-01-13 23:24:39.075760 numpi-0.4.0/helpers/LBFGS_memory_profiling_line_by_line/Memory profiling LBFGS line by line.ipynb
--rw-r--r--   0        0        0     3070 2024-01-13 23:24:39.075760 numpi-0.4.0/helpers/Numpy Matrix Operations.ipynb
--rw-r--r--   0        0        0    17152 2024-01-13 23:24:39.075760 numpi-0.4.0/helpers/line_profiing_LBFGSB.ipynb
--rw-r--r--   0        0        0     1823 2024-01-13 23:24:39.075760 numpi-0.4.0/helpers/memoryprofiling_LBFGS.py
--rw-r--r--   0        0        0     3522 2024-01-13 23:24:39.075760 numpi-0.4.0/helpers/nb_fevals_scipy_vs_numpy.py
--rw-r--r--   0        0        0     2184 2024-01-13 23:24:39.075760 numpi-0.4.0/helpers/plot_helpers.py
--rw-r--r--   0        0        0     2828 2024-01-13 23:24:39.075760 numpi-0.4.0/helpers/profile_Rosenbrock.py
--rw-r--r--   0        0        0    47412 2024-01-13 23:24:39.079759 numpi-0.4.0/helpers/timing basic numpy operations.ipynb
--rw-r--r--   0        0        0     3371 2024-01-13 23:24:39.079759 numpi-0.4.0/maintenance/copyright.py
--rw-r--r--   0        0        0     1492 2024-01-13 23:24:39.079759 numpi-0.4.0/maintenance/replace_header.py
--rw-r--r--   0        0        0      305 2024-01-13 23:24:39.079759 numpi-0.4.0/maintenance/update_license_headers.sh
--rw-r--r--   0        0        0      977 2024-01-13 23:24:39.079759 numpi-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       71 2024-01-13 23:24:39.079759 numpi-0.4.0/pytest.ini
--rw-r--r--   0        0        0      176 2024-01-13 23:24:39.079759 numpi-0.4.0/run-tests.py
--rwxr-xr-x   0        0        0      129 2024-01-13 23:24:39.079759 numpi-0.4.0/run-tests.sh
--rw-r--r--   0        0        0       31 2024-01-13 23:24:39.079759 numpi-0.4.0/setup.cfg
--rw-r--r--   0        0        0    11954 2024-01-13 23:24:39.079759 numpi-0.4.0/test/IO/test_io.py
--rw-r--r--   0        0        0     7194 2024-01-13 23:24:39.079759 numpi-0.4.0/test/IO/test_netcdf.py
--rw-r--r--   0        0        0      169 2024-01-13 23:24:39.079759 numpi-0.4.0/test/IO/wrongnpyfile.npy
--rw-r--r--   0        0        0     8320 2024-01-13 23:24:39.079759 numpi-0.4.0/test/Optimization/MPI_minimization_problems.py
--rw-r--r--   0        0        0     1213 2024-01-13 23:24:39.079759 numpi-0.4.0/test/Optimization/__init__.py
--rw-r--r--   0        0        0     6623 2024-01-13 23:24:39.079759 numpi-0.4.0/test/Optimization/minimization_problems.py
--rw-r--r--   0        0        0     4404 2024-01-13 23:24:39.079759 numpi-0.4.0/test/Optimization/show_parallel_speedup.py
--rw-r--r--   0        0        0     4122 2024-01-13 23:24:39.079759 numpi-0.4.0/test/Optimization/test_LBFGS_interface.py
--rw-r--r--   0        0        0     5102 2024-01-13 23:24:39.079759 numpi-0.4.0/test/Optimization/test_MPI_LBFGS.py
--rw-r--r--   0        0        0     3037 2024-01-13 23:24:39.079759 numpi-0.4.0/test/Optimization/test_cg.py
--rw-r--r--   0        0        0     6329 2024-01-13 23:24:39.079759 numpi-0.4.0/test/Optimization/test_minimization_problems.py
--rw-r--r--   0        0        0    10538 2024-01-13 23:24:39.079759 numpi-0.4.0/test/Optimization/test_serial_LBFGS.py
--rw-r--r--   0        0        0    10541 2024-01-13 23:24:39.079759 numpi-0.4.0/test/Tools/test_reduction.py
--rw-r--r--   0        0        0     1161 2024-01-13 23:24:39.079759 numpi-0.4.0/test/__init__.py
--rw-r--r--   0        0        0     1652 2024-01-13 23:24:39.079759 numpi-0.4.0/test/conftest.py
--rw-r--r--   0        0        0     2991 1970-01-01 00:00:00.000000 numpi-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1041 2024-04-14 12:34:30.459115 numpi-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0    10241 2024-04-14 12:34:30.459115 numpi-0.5.0/NuMPI/IO/MPIFileIO.py
+-rw-r--r--   0        0        0    17465 2024-04-14 12:34:30.459115 numpi-0.5.0/NuMPI/IO/NetCDF.py
+-rw-r--r--   0        0        0     1294 2024-04-14 12:34:30.459115 numpi-0.5.0/NuMPI/IO/__init__.py
+-rw-r--r--   0        0        0     7465 2024-04-14 12:34:30.459115 numpi-0.5.0/NuMPI/MPIStub.py
+-rw-r--r--   0        0        0     7253 2024-04-14 12:34:30.459115 numpi-0.5.0/NuMPI/Optimization/CCGWithRestart.py
+-rw-r--r--   0        0        0     7693 2024-04-14 12:34:30.459115 numpi-0.5.0/NuMPI/Optimization/CCGWithoutRestart.py
+-rw-r--r--   0        0        0    15874 2024-04-14 12:34:30.459115 numpi-0.5.0/NuMPI/Optimization/LBFGS.py
+-rw-r--r--   0        0        0    11946 2024-04-14 12:34:30.459115 numpi-0.5.0/NuMPI/Optimization/LineSearch.py
+-rw-r--r--   0        0        0     1668 2024-04-14 12:34:30.459115 numpi-0.5.0/NuMPI/Optimization/Result.py
+-rw-r--r--   0        0        0     2129 2024-04-14 12:34:30.459115 numpi-0.5.0/NuMPI/Optimization/Wolfe.py
+-rw-r--r--   0        0        0     1190 2024-04-14 12:34:30.459115 numpi-0.5.0/NuMPI/Optimization/__init__.py
+-rw-r--r--   0        0        0     6188 2024-04-14 12:34:30.459115 numpi-0.5.0/NuMPI/Tools/Reduction.py
+-rw-r--r--   0        0        0     1198 2024-04-14 12:34:30.459115 numpi-0.5.0/NuMPI/Tools/__init__.py
+-rw-r--r--   0        0        0     1602 2024-04-14 12:34:30.459115 numpi-0.5.0/NuMPI/__init__.py
+-rw-r--r--   0        0        0     2078 2024-04-14 12:34:30.459115 numpi-0.5.0/README.md
+-rw-r--r--   0        0        0     1019 2024-04-14 12:34:30.463115 numpi-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3022 1970-01-01 00:00:00.000000 numpi-0.5.0/PKG-INFO
```

### Comparing `numpi-0.4.0/LICENSE.md` & `numpi-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `numpi-0.4.0/NuMPI/IO/MPIFileIO.py` & `numpi-0.5.0/NuMPI/IO/MPIFileIO.py`

 * *Files identical despite different names*

### Comparing `numpi-0.4.0/NuMPI/IO/NetCDF.py` & `numpi-0.5.0/NuMPI/IO/NetCDF.py`

 * *Files identical despite different names*

### Comparing `numpi-0.4.0/NuMPI/IO/__init__.py` & `numpi-0.5.0/NuMPI/IO/__init__.py`

 * *Files identical despite different names*

### Comparing `numpi-0.4.0/NuMPI/MPIStub.py` & `numpi-0.5.0/NuMPI/MPIStub.py`

 * *Files identical despite different names*

### Comparing `numpi-0.4.0/NuMPI/Optimization/MPI_LBFGS_Matrix_H.py` & `numpi-0.5.0/NuMPI/Optimization/LBFGS.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,39 +27,40 @@
 # flake8: noqa F821
 
 
 import numpy as np
 
 from .. import MPI
 from ..Tools import Reduction
-from .linesearch import scalar_search_wolfe2
-from .result import OptimizeResult
+from .LineSearch import scalar_search_wolfe2
+from .Result import OptimizeResult
+
 
 def donothing(*args, **kwargs):
     pass
 
 
-def steepest_descent_wolfe2(x0, f_gradf, pnp=None, maxiter=10, **kwargs):
+def steepest_descent_wolfe2(x0, f_gradf, pnp=None, maxiter=10, args=(), **kwargs):
     """
     For first Iteration there is no history. We make a steepest descent
     satisfying strong Wolfe Condition
     :return:
     """
     # x_old.shape=(-1,1)
-    phi0, grad0 = f_gradf(x0)
+    phi0, grad0 = f_gradf(x0, *args)
     grad0 = grad0.reshape((-1, 1))
 
     derphi0 = pnp.dot(grad0.T, -grad0).item()
     gradf = np.zeros_like(grad0)
 
     # stores the last evaluated gradf,
     # take care, the linesearch has to return the last evaluated value
     # TODO: Dangerous
     def _phi_phiprime(alpha):
-        phi, gradf[...] = f_gradf(x0 - grad0 * alpha)
+        phi, gradf[...] = f_gradf(x0 - grad0 * alpha, *args)
         phiprime = pnp.dot(gradf.T, -grad0).item()
         return phi, phiprime
 
     # like in lbfgsb
     # if (iter.eq. 0.and..not.boxed) then
     #    stp = min(one / dnorm, stpmx)
 
@@ -71,137 +72,165 @@
 
     assert derphi is not None, "Line Search in first steepest descent failed"
     x = x0 - grad0 * alpha
 
     return x, gradf, x0, grad0, phi, phi0, derphi
 
 
-def LBFGS(fun, x, args=(), jac=None, x_old=None, maxcor=10, gtol=1e-5,
-          ftol=2.2e-9, maxiter=15000,
-          maxls=20, linesearch_options=dict(c1=1e-3, c2=0.9),
-          pnp=Reduction(MPI.COMM_WORLD),
-          store_iterates=None, printdb=donothing, callback=None, **options):
-    r"""
+def l_bfgs(fun, x, args=(), jac=None, x_old=None, maxcor=10, gtol=1e-5, ftol=2.2e-9, maxiter=15000, maxls=20,
+           linesearch_options=dict(c1=1e-3, c2=0.9), disp=None, pnp=Reduction(MPI.COMM_WORLD), store_iterates=None,
+           printdb=donothing, callback=None, **options):
+    """
+    Limited-memory L-BFGS optimization with MPI parallelization.
 
-    convergence if |grad|_{\infty} <= gtol or <= ftol is satisfied
+    The optimization converges if |grad|_{\infty} <= gtol or <= ftol is satisfied.
 
     Parameters
     ----------
-    fun
-    x
-    args
-    jac
-    x_old: initial guess
-    maxcor: max number of history gradients stored
-    gtol:
-    ftol:
-    maxiter
-    maxls, default 20, as in scipy.optimize.fmin_l_bfgs_b
-    linesearch_options: further options for the linesearch
-    the result of the linesearch has to satisfy the strong wolfe condition
-    See Wright and Nocedal, 'Numerical Optimization',p.34
-    c1 parameter for the sufficient decrease condition
-    c2 parameter for the curvature condition
-    
-    default values are choosen here to match the implementation in
-    the Fortran subroutine L-BFGS-B 3.0 by
-    Ciyou Zhu, Richard Byrd, and Jorge Nocedal
-
-    See lbfgsb.f line 2497, with gtol=c2 and ftol=c1
-    
-    pnp
-    store_iterates: stores each iterate of x, only debugging
-    printdb
-    options
+    fun : callable
+        The objective function to be minimized.
+    x : ndarray
+        Initial guess.
+    args : tuple, optional
+        Extra arguments passed to the objective function and its derivatives (Jacobian).
+    jac : bool or callable, optional
+        Method for computing the gradient vector. If it is a callable, it should be a function that returns the gradient vector. If it is a Boolean and is True, then `fun` should return the gradient along with the objective function.
+    x_old : ndarray, optional
+        Initial guess for the previous value of x. If None, a steepest descent step will be performed.
+    maxcor : int, optional
+        The maximum number of variable metric corrections used to define the limited memory matrix.
+    gtol : float, optional
+        The iteration will stop when max{|proj g_i | i = 1, ..., n} <= gtol where pg_i is the i-th component of the projected gradient.
+    ftol : float, optional
+        The iteration will stop when (f^k - f^{k+1})/max{|f^k|,|f^{k+1}|,1} <= ftol.
+    maxiter : int, optional
+        Maximum number of iterations.
+    maxls : int, optional
+        Maximum number of line search steps (per iteration).
+    linesearch_options : dict, optional
+        A dictionary with optional settings for the line search parameters.
+    disp : int, optional
+        If disp is a positive integer, convergence messages will be printed.
+    pnp : Reduction, optional
+        Parallelization object from the NuMPI package.
+    store_iterates : bool, optional
+        If True, the result at each iteration is stored in a list.
+    printdb : callable, optional
+        Debugging print function.
+    callback : callable, optional
+        Called after each iteration.
+    options : dict, optional
+        A dictionary with optional settings for the optimization algorithm.
 
     Returns
     -------
-
+    result : OptimizeResult
+        The optimization result represented as a OptimizeResult object. Important attributes are: x the solution array, success a Boolean flag indicating if the optimizer exited successfully and message which describes the cause of the termination.
     """
+    # user can provide x in the shape of his convenience
+    # but we will work with the shape (-1, 1)
+    original_shape = x.shape
 
     if callback is None:
         callback = donothing
 
     # print("jac = {}, type = {}".format(jac, type(jac)))
     if jac is True:
-        def fun_grad(x):
+        def fun_grad(x, *args):
             """
-            reshapes the gradient in a convenient form
+            This function evaluates the objective function and its gradient at the point x.
+            It reshapes the gradient into a convenient form for further computations.
+
             Parameters
             ----------
-            x
+            x : ndarray
+                The point at which the objective function and its gradient are to be evaluated.
 
             Returns
             -------
-
+            f : float
+                The value of the objective function at the point x.
+            grad : ndarray
+                The gradient of the objective function at the point x, reshaped into a convenient form.
             """
-            f, grad = fun(x)
+            f, grad = fun(x.reshape(original_shape), *args)
             return f, grad.reshape((-1, 1))
 
     elif jac is False:
         raise NotImplementedError(
             "Numerical evaluation of gradient not implemented")
     else:
         # function and gradient provided sepatately
 
-        def fun_grad(x):
+        def fun_grad(x, *args):
             """
-            evaluates function and grad consequently (important, see issue #13)
-            and reshapes the gradient in a convenient form
+            This function evaluates the objective function and its gradient at the point x.
+            It reshapes the gradient into a convenient form for further computations.
+            The order of function and gradient evaluation is important (see issue #13).
+
             Parameters
             ----------
-            x
+            x : ndarray
+                The point at which the objective function and its gradient are to be evaluated.
 
             Returns
             -------
-
+            f : float
+                The value of the objective function at the point x.
+            grad : ndarray
+                The gradient of the objective function at the point x, reshaped into a convenient form.
             """
             # order matte
-            f = fun(x)
-            grad = jac(x).reshape((-1, 1))
+            f = fun(x.reshape(original_shape), *args)
+            grad = jac(x.reshape(original_shape), *args).reshape((-1, 1))
             return f, grad
 
-    # user can provide x in the shape of his convenience
-    # but we will work with the shape (-1, 1)
-    original_shape = x.shape
-
     x = x.reshape((-1, 1))
 
     if x_old is None:
         x_old = x.copy()
         x, grad, x_old, grad_old, phi, phi_old, derphi = \
             steepest_descent_wolfe2(x_old, fun_grad, pnp=pnp, maxiter=maxls,
-                                    **linesearch_options)
+                                    args=args, **linesearch_options)
     else:
-        phi_old, grad_old = fun_grad(
-            x_old)  # phi_old is never used, except for the convergence
+        # phi_old is never used, except for the convergence
+        phi_old, grad_old = fun_grad(x_old, *args)
         # criterion
-        phi, grad = fun_grad(x)
+        phi, grad = fun_grad(x, *args)
 
     # full history of x is sored here if wished
     iterates = list()
-    k = 1
+    iteration = 1
 
     # n = x.size  # number of degrees of freedom
     gamma = 1
 
     Slist = []  # history of the steps of x
     Ylist = []  # history of gradient differences
     R = np.zeros((0, 0))
 
     grad2 = pnp.sum(grad ** 2)
 
     alpha = 0  # line search step size
 
+    if disp:
+        iteration_title = "iteration"
+        phi_title = "f"
+        phi_change_title = "Δf"
+        max_grad_title = "max ∇ f"
+        abs_grad_title = "|∇ f|"
+        print(f"{iteration_title:<10} {phi_title:<10} {phi_change_title:<10} {max_grad_title:<10} {abs_grad_title:<10}")
+        print(f"---------- ---------- ---------- ---------- ----------")
+
     # Start loop
     # printdb(k)
     while True:
         # Update Sk,Yk
         # print("k= {}".format(k))
-        if k > maxcor:
+        if iteration > maxcor:
             # S = np.roll(S, -1)
             # S[:, -1] = (x - x_old).flat
 
             Slist[:-1] = Slist[1:]
             Slist[-1] = (x - x_old)
 
             # Y = np.roll(Y, -1)
@@ -225,107 +254,117 @@
         # if ((grad2 < g2tol if g2tol is not None else True) and
         #        (pnp.max(np.abs(grad)) < gtol if gtol is not None else
         #        True) and
         #        ((phi - phi_old) / max((1,abs(phi),abs(phi_old))) <= ftol
         #        if ftol is not None else True)):
         callback(x)
 
-        if (pnp.max(np.abs(grad)) < gtol):
+        max_grad = pnp.max(np.abs(grad))
+        abs_grad = np.linalg.norm(grad)
+        phi_change = phi_old - phi
+
+        if disp:
+            print(f"{iteration:<10} {phi:<10.7g} {phi_change:<10.7g} {max_grad:<10.7g} {abs_grad:<10.7g}")
+
+        if (max_grad < gtol):
+            print("CONVERGED because gradient tolerance was reached")
             result = OptimizeResult({
                 'success': True,
                 'x': x.reshape(
                     original_shape),
                 'fun': phi,
                 'jac': grad.reshape(
                     original_shape),
-                'nit': k,
+                'nit': iteration,
                 'message':
                     'CONVERGENCE: '
                     'NORM_OF_GRADIENT_<=_GTOL',
                 'iterates': iterates
             })
             # if iterates:
             #    result['iterates'] = iterates
             return result
 
-        if ((phi_old - phi) <= ftol * max((1, abs(phi), abs(phi_old)))):
+        if (phi_change <= ftol * max((1, abs(phi), abs(phi_old)))):
+            print("CONVERGED because function tolerance was reached")
             result = OptimizeResult({
                 'success': True,
                 'x': x.reshape(
                     original_shape),
                 'fun': phi,
                 'jac': grad.reshape(
                     original_shape),
-                'nit': k,
+                'nit': iteration,
                 'message':
                     'CONVERGENCE: '
                     'REL_REDUCTION_OF_F_<=_FACTR*EPSMCH',
                 'iterates': iterates
             })
             # if iterates:
             #    result['iterates'] = iterates
             return result
 
-        if k > maxiter:
+        if iteration > maxiter:
+            print("CONVERGED because maximum number of iterations reached")
             result = OptimizeResult({
                 'success': False,
                 'x': x.reshape(
                     original_shape),
                 'fun': phi,
                 'jac': grad.reshape(
                     original_shape),
-                'nit': k,
+                'nit': iteration,
                 'iterates': iterates
             })
 
             return result
         ###########
         # new iteration
 
         STgrad = np.array([pnp.dot(si.T, grad) for si in Slist]).reshape(-1, 1)
         YTgrad = np.array([pnp.dot(yi.T, grad) for yi in Ylist]).reshape(-1, 1)
         # STgrad = pnp.dot(S.T, grad)
         # YTgrad = pnp.dot(Y.T, grad)
 
-        if k > maxcor:
+        if iteration > maxcor:
             S_now_T_grad_prev = np.roll(STgrad_prev, -1)
             S_now_T_grad_prev[-1] = - alpha * gamma * grad2prev - alpha * (
                     STgrad_prev.T.dot(p1) + gamma * YTgrad_prev.T.dot(p2))
         else:  # straightforward Version
             S_now_T_grad_prev = np.array(
                 [pnp.dot(si.T, grad_old) for si in Slist]).reshape(-1, 1)
 
-        if k > maxcor:
+        if iteration > maxcor:
             R = np.roll(R, (-1, -1),
                         axis=(0, 1))  # mxm Matrix hold by all Processors
             R[-1, :] = 0
             STym1 = STgrad - S_now_T_grad_prev
             R[:, -1] = STym1.flat  # O(m x n)
 
-        elif k == 1:
+        elif iteration == 1:
             # Rm = np.triu(pnp.dot(S.T, Y))
             R = np.triu(np.array(
                 [[pnp.dot(si.T, yi).item() for yi in Ylist] for si in Slist]))
             # print(R)
         else:
             # Rm = np.vstack([Rm, np.zeros(k - 1)])
             # Rm = np.hstack([Rm, pnp.dot(S.T, Y[:, -1]).reshape(k, 1)])
-            R = np.vstack([R, np.zeros(k - 1)])
+            R = np.vstack([R, np.zeros(iteration - 1)])
             R = np.hstack([R, np.array(
-                [pnp.dot(si.T, Ylist[-1]) for si in Slist]).reshape(k, 1)])
-        if k > maxcor:
+                [pnp.dot(si.T, Ylist[-1]) for si in Slist]).reshape(iteration, 1)])
+        if iteration > maxcor:
             D = np.roll(D, (-1, -1), axis=(0, 1))
             # D[-1,-1] = np.dot(Y[:,-1],Y[:,-1])# yk-1Tyk-1 # TOOPTIMIZE
             D[-1, -1] = R[-1, -1]
         else:
             # D = np.diag(np.einsum("ik,ik -> k", S, Y))
             D = np.diag(R.diagonal())
-        assert D[-1, -1] > 0, "k = {}: ".format(k)  # Assumption of Theorem 2.2
+        assert D[-1, -1] > 0, "k = {}: ".format(iteration)  # Assumption of Theorem 2.2
 
-        if k > maxcor:
+        if iteration > maxcor:
             YTY = np.roll(YTY, (-1, -1), axis=(0, 1))
             YTY[-1, :-1] = YTY[:-1, -1] = (YTgrad[:-1] - YTgrad_prev[1:]).flat
             YTY[-1, -1] = grad2prev - grad2 + 2 * YTgrad[-1]
         else:
             # YTYm = pnp.dot(Y.T, Y)
             YTY = np.array(
                 [[pnp.dot(yi1.T, yi2).item() for yi2 in Ylist] for yi1 in
@@ -349,15 +388,15 @@
 
         phi_old = float(phi)
         # printdb("Linesearch: ")
         grad_old[:] = grad
         x_old[:] = x
 
         def _phi_phiprime(alpha):
-            phi, grad[...] = fun_grad(x - Hgrad * alpha)
+            phi, grad[...] = fun_grad(x - Hgrad * alpha, *args)
             phiprime = pnp.dot(grad.T, -Hgrad).item()
             return phi, phiprime
 
         # TODO: oldphi0: is it allowed to stay outside of the search
         #  direction ?
         alpha, phi, phi0, derphi = scalar_search_wolfe2(
             _phi_phiprime,
@@ -376,12 +415,12 @@
                 {
                     'x': x.copy().reshape(original_shape),
                     'fun': phi,
                     'jac': grad.reshape(original_shape)
                 })
             iterates.append(iterate)
 
-        printdb("k = {}".format(k))
-        k = k + 1
+        printdb("k = {}".format(iteration))
+        iteration = iteration + 1
 
         STgrad_prev = STgrad.copy()
         YTgrad_prev = YTgrad.copy()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `numpi-0.4.0/NuMPI/Optimization/Wolfe.py` & `numpi-0.5.0/NuMPI/Optimization/Wolfe.py`

 * *Files identical despite different names*

### Comparing `numpi-0.4.0/NuMPI/Optimization/__init__.py` & `numpi-0.5.0/NuMPI/Tools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 
-from .MPI_LBFGS_Matrix_H import LBFGS  # noqa F401
+from .Reduction import Reduction  # noqa F401
```

### Comparing `numpi-0.4.0/NuMPI/Optimization/ccg_with_restart.py` & `numpi-0.5.0/NuMPI/Optimization/CCGWithRestart.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,63 @@
 import numpy as np
 
 from inspect import signature
 
-from .result import OptimizeResult
+from .Result import OptimizeResult
 
 
-def constrained_conjugate_gradients(fun, hessp, x0, gtol=1e-8,
+def constrained_conjugate_gradients(fun, hessp, x0, args=(), gtol=1e-8,
                                     mean_value=None, residual_plot=False,
                                     maxiter=5000):
     """
     Implementation of constrained conjugate gradient algorithm as described in,
     I.A. Polonsky, L.M. Keer, Wear 231, 206 (1999).
 
-    See also
-    M.R. Hestenes, Conjugate Direction Methods in Optimization, Springer, New York, 1980, Chaps. 2, 3.
-    B.N. Pshenichny, Yu.M. Danilin,
-        Numerical Methods in Optimization Problems, Nauka, Moscow, 1975, Chap. 3, in Russian.
-    G. Zoutendijk, Mathematical Programming Methods, North Holland, Amsterdam, 1976, Chap. 16.
-
-    Application to contact problems with adhesion:
-    Rey, V. et al. Comput. Mech. 60, 69–81 (2017)
-
+    This function minimizes a given objective function using the constrained
+    conjugate gradient algorithm. The algorithm is described in detail in the
+    references provided.
 
     Parameters
     ----------
-    fun : callable.
-                The objective function to be minimized.
-                            fun(x) -> float(energy),ndarray(gradient)
-                where x is the input ndarray.
-                Note that energy is never used, you can return a dummy value.
-
+    fun : callable
+        The objective function to be minimized. The function should return a float
+        (energy) and an ndarray (gradient). Note that energy is never used, you can
+        return a dummy value.
     hessp : callable
-            Function to evaluate the hessian product of the objective.
-            Hessp should accept either 1 argument (desscent direction) or
-            2 arguments (x,descent direction).
-                            hessp(des_dir)->ndarray
-                                    or
-                            hessp(x,des_dir)->ndarray
-            where x is the input ndarray and des_dir is the descent direction.
-
+        Function to evaluate the hessian product of the objective. Hessp should
+        accept either 1 argument (descent direction) or 2 arguments (x, descent
+        direction).
     x0 : ndarray
-         Initial guess.
-         ValueError is raised if "None" is provided.
-
+        Initial guess. ValueError is raised if "None" is provided.
     gtol : float, optional
-           Default value : 1e-8
-           convergence criterion is max(abs) and norm2 of the projected
-           gradient < gtol.
-
+        Convergence criterion is max(abs) and norm2 of the projected gradient <
+        gtol. Default value is 1e-8.
     mean_value :  float, optional
-               If you want to apply the mean_value constraint then provide an
-               float value to the mean_value.
-
+        If you want to apply the mean_value constraint then provide a float value
+        to the mean_value.
     residual_plot : bool, optional
-                    Generates a plot between the residual and iterations.
-
+        If set to True, generates a plot between the residual and iterations.
     maxiter : int, optional
-              Default, maxiter=5000
-              Maximum number of iterations after which the program will exit.
+        Maximum number of iterations after which the program will exit. Default
+        value is 5000.
 
     Returns
     -------
     OptimizeResult  : scipy.optimize object.
-        Attributes:
-         success: bool
-         x: x,
-         jac: residual = gradient(x),
-         nit: n_iterations,
-         message: 'CONVERGENCE: NORM_OF_GRADIENT_<=_GTOL' or 'NO CONVERGENCE: MAXITERATIONS REACHED'
+        The result of the optimization. The object has the following attributes:
+        - success: bool, indicates if the optimization was successful
+        - x: ndarray, the optimized parameters
+        - jac: ndarray, the residual which is equal to the gradient at x
+        - nit: int, the number of iterations performed
+        - message: str, a message describing the reason for the termination
 
     References
     ----------
     ..[1] I.A. Polonsky, L.M. Keer, Wear 231, 206 (1999)
     """
-
     if not isinstance(mean_value, (type(None), int, float)):
         raise ValueError('Inappropriate type: {} for mean_value whereas a '
                          'float \
             or int is expected'.format(type(mean_value)))
 
     if not isinstance(residual_plot, bool):
         raise ValueError('Inappropriate type: {} for "residual_plot" whereas '
@@ -106,15 +86,15 @@
     while (n_iterations < maxiter + 1):
 
         '''Mask to truncate the negative values'''
         mask_neg = x <= 0
         x[mask_neg] = 0.0
 
         '''Initial residual or GAP'''
-        residual = fun(x)[1]
+        residual = fun(x, *args)[1]
 
         mask_c = x > 0
         if mean_value is not None:
             residual = residual - np.mean(residual[mask_c])
 
         G = np.sum(residual[mask_c] ** 2)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `numpi-0.4.0/NuMPI/Optimization/ccg_without_restart.py` & `numpi-0.5.0/NuMPI/Optimization/CCGWithoutRestart.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,86 +5,63 @@
 """
 
 import numpy as np
 
 from inspect import signature
 
 from ..Tools import Reduction
-from .result import OptimizeResult
+from .Result import OptimizeResult
 
 
-def constrained_conjugate_gradients(fun, hessp,
-                                    x0, mean_val=None,
-                                    gtol=1e-8,
-                                    maxiter=3000,
-                                    callback=None,
-                                    communicator=None,
-                                    bounds=None
-                                    ):
-    '''
+def constrained_conjugate_gradients(fun, hessp, x0, args=(), mean_val=None, gtol=1e-8, maxiter=3000, callback=None,
+                                    communicator=None, bounds=None):
+    """
     Constrained conjugate gradient algorithm from Bugnicourt et al. [1].
 
     Parameters
-    __________
-
-    fun :   callable.
-                The objective function to be minimized.
-                            fun(x) -> float(energy),ndarray(gradient)
-                where x is the input ndarray. The energy is actually never used.
-
+    ----------
+    fun : callable
+        The objective function to be minimized. The function should return a float
+        (energy) and an ndarray (gradient). Note that energy is never used, you can
+        return a dummy value.
     hessp : callable
-            Function to evaluate the hessian product of the objective.
-            Hessp should accept either 1 argument (descent direction) or
-            2 arguments (x,descent direction).
-                            hessp(des_dir)->ndarray
-                                    or
-                            hessp(x,des_dir)->ndarray
-            where x is the input ndarray and des_dir is the descent direction.
-
+        Function to evaluate the hessian product of the objective. Hessp should
+        accept either 1 argument (descent direction) or 2 arguments (x, descent
+        direction).
     x0 : ndarray
-         Initial guess.
-
+        Initial guess. ValueError is raised if "None" is provided.
     gtol : float, optional
-           Default value : 1e-8
-           convergence criterion is max(abs) and norm2 of the projected
-           gradient < gtol.
-    mean_value : int/float, optional
-               If you want to apply the mean_value constraint then provide an
-               int/float value to the mean_value.
-
+        Convergence criterion is max(abs) and norm2 of the projected gradient <
+        gtol. Default value is 1e-8.
+    mean_value :  int/float, optional
+        If you want to apply the mean_value constraint then provide an int/float
+        value to the mean_value.
     residual_plot : bool, optional
-                    Generates a plot between the residual and iterations.
-
+        If set to True, generates a plot between the residual and iterations.
     maxiter : int, optional
-              Default, maxiter=5000
-              Maximum number of iterations after which the program will exit.
+        Maximum number of iterations after which the program will exit. Default
+        value is 5000.
 
     Returns
     -------
     OptimizeResult  : scipy.optimize object.
-        Attributes:
-         success: bool
-         x: x,
-         jac: residual = gradient(x),
-         nit: n_iterations,
-         message: 'CONVERGENCE: NORM_OF_GRADIENT_<=_GTOL' or 'NO CONVERGENCE: MAXITERATIONS REACHED'
+        The result of the optimization. The object has the following attributes:
+        - success: bool, indicates if the optimization was successful
+        - x: ndarray, the optimized parameters
+        - jac: ndarray, the residual which is equal to the gradient at x
+        - nit: int, the number of iterations performed
+        - message: str, a message describing the reason for the termination
 
     References
-    __________
-
-    ..[1]   :   Bugnicourt, Romain & Sainsot, Philippe & Dureisseix, David &
-                Gauthier, Catherine & Lubrecht, Ton. (2018). FFT-Based Methods
-                for Solving a Rough Adhesive Contact: Description and
-                Convergence Study.
-                Tribology Letters. 66. 10.1007/s11249-017-0980-z.
-
-    ..[2]   :   Vollebregt, E. A. H. J Optim Theory Appl 162, 931–953 (2014)
-                The Bound-Constrained Conjugate Gradient Method for Non-negative Matrices
-
-    '''
+    ----------
+    ..[1] Bugnicourt, Romain & Sainsot, Philippe & Dureisseix, David &
+        Gauthier, Catherine & Lubrecht, Ton. (2018). FFT-Based Methods
+        for Solving a Rough Adhesive Contact: Description and
+        Convergence Study.
+    """
     if communicator is None:
         comm = np
         nb_DOF = x0.size
     else:
         comm = Reduction(communicator)
         nb_DOF = comm.sum(x0.size)
 
@@ -100,15 +77,15 @@
 
     if mean_val is not None and nb_bounds < nb_DOF:
         raise ValueError("mean_value constrained mode not compatible "
                          "with partially bound system")
         # There are ambiguities on how to compute the mean values
 
     '''Initial Residual = A^(-1).(U) - d A −1 .(U ) −  ∂ψadh/∂g'''
-    residual = fun(x)[1]
+    residual = fun(x, *args)[1]
 
     mask_neg = x <= bounds
     x[mask_neg] = bounds[mask_neg]
 
     if mean_val is not None:
         #
         mask_nonzero = x > bounds
@@ -171,15 +148,15 @@
                 / (comm.sum(x) / nb_DOF - mean_bounds) * (x - bounds)
         residual_old = residual
 
         '''
         In Bugnicourt's paper
         Residual = A^(-1).(U) - d A −1 .(U ) −  ∂ψadh/∂g
         '''
-        residual = fun(x)[1]
+        residual = fun(x, *args)[1]
 
         if mean_val is not None:
             mask_nonzero = x > bounds
             N_mask_nonzero = comm.sum(np.count_nonzero(mask_nonzero))
             residual = residual - comm.sum(
                 residual[mask_nonzero]) / N_mask_nonzero
 
@@ -220,21 +197,21 @@
             result = OptimizeResult(
                 {
                     'success': True,
                     'x': x,
                     'jac': residual,
                     'nit': i,
                     'message': 'CONVERGENCE: NORM_OF_GRADIENT_<=_GTOL',
-                    })
+                })
             return result
 
         elif i == maxiter - 1:
             result = OptimizeResult(
                 {
                     'success': False,
                     'x': x,
                     'jac': residual,
                     'nit': i,
                     'message': 'NO CONVERGENCE: MAXITERATIONS REACHED'
-                    })
+                })
 
             return result
```

### Comparing `numpi-0.4.0/NuMPI/Optimization/linesearch.py` & `numpi-0.5.0/NuMPI/Optimization/LineSearch.py`

 * *Files identical despite different names*

### Comparing `numpi-0.4.0/NuMPI/Optimization/result.py` & `numpi-0.5.0/NuMPI/Optimization/Result.py`

 * *Files identical despite different names*

### Comparing `numpi-0.4.0/NuMPI/Tools/Reduction.py` & `numpi-0.5.0/NuMPI/Tools/Reduction.py`

 * *Files identical despite different names*

### Comparing `numpi-0.4.0/NuMPI/Tools/__init__.py` & `numpi-0.5.0/NuMPI/Optimization/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 
-from .Reduction import Reduction  # noqa F401
+from .LBFGS import l_bfgs  # noqa F401
```

### Comparing `numpi-0.4.0/NuMPI/__init__.py` & `numpi-0.5.0/NuMPI/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,22 +22,24 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 
 import warnings
 
-from .DiscoverVersion import __version__  # noqa: F401
+from DiscoverVersion import get_version
 
 try:
     # raise ImportError()
     from mpi4py import MPI
 
     _has_mpi4py = True
 except ImportError:
     warnings.warn('Could not import mpi4py; '
                   'falling back to MPI stub implementation.', ImportWarning)
     from . import MPIStub as MPI  # noqa: F401
 
     _has_mpi4py = False
 
 from . import Tools, Optimization  # noqa: F401
+
+__version__ = get_version('NuMPI', __file__)
```

### Comparing `numpi-0.4.0/README.md` & `numpi-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `numpi-0.4.0/pyproject.toml` & `numpi-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["flit_core>=3.2", "numpy>1.15.0"]
+requires = ["flit_core>=3.2", "numpy>1.15.0", "DiscoverVersion"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "NuMPI"
 description = "Numerical tools for MPI-parallelized code"
 readme = "README.md"
 license = { file = "LICENSE.md" }
@@ -14,14 +14,15 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python"
 ]
 requires-python = ">=3.8.0"
 dynamic = ["version"]
 dependencies = [
+    "DiscoverVersion",
     "scipy>1.1.0",
     "netCDF4>=1.5.3,<=1.6.2,!=1.6.1"  # Those versions seem to work
 ]
 
 [project.optional-dependencies]
 mpi = [
     "mpi4py"
```

### Comparing `numpi-0.4.0/PKG-INFO` & `numpi-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: NuMPI
-Version: 0.4.0
+Version: 0.5.0
 Summary: Numerical tools for MPI-parallelized code
 Author-email: Antoine Sanner <antoine.sanner@imtek.uni-freiburg.de>, Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
+Requires-Dist: DiscoverVersion
 Requires-Dist: scipy>1.1.0
 Requires-Dist: netCDF4>=1.5.3,<=1.6.2,!=1.6.1
 Requires-Dist: mpi4py ; extra == "mpi"
 Requires-Dist: flake8<5 ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-flake8 ; extra == "test"
```

