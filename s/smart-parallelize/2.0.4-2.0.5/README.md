# Comparing `tmp/smart_parallelize-2.0.4.tar.gz` & `tmp/smart_parallelize-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_parallelize-2.0.4.tar", max compression
+gzip compressed data, was "smart_parallelize-2.0.5.tar", max compression
```

## Comparing `smart_parallelize-2.0.4.tar` & `smart_parallelize-2.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      560 2024-03-22 16:57:28.000000 smart_parallelize-2.0.4/README.md
--rw-r--r--   0        0        0      317 2024-04-09 22:33:58.860124 smart_parallelize-2.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.0.4/smart_parallelize/__init__.py
--rw-r--r--   0        0        0     4313 2024-04-05 18:40:15.452279 smart_parallelize-2.0.4/smart_parallelize/parallelize.py
--rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 smart_parallelize-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0      560 2024-03-22 16:57:28.000000 smart_parallelize-2.0.5/README.md
+-rw-r--r--   0        0        0      317 2024-04-14 20:31:42.010715 smart_parallelize-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.0.5/smart_parallelize/__init__.py
+-rw-r--r--   0        0        0     4337 2024-04-14 20:30:12.828920 smart_parallelize-2.0.5/smart_parallelize/parallelize.py
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 smart_parallelize-2.0.5/PKG-INFO
```

### Comparing `smart_parallelize-2.0.4/README.md` & `smart_parallelize-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `smart_parallelize-2.0.4/smart_parallelize/parallelize.py` & `smart_parallelize-2.0.5/smart_parallelize/parallelize.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,23 +34,24 @@
 
     def wrap(**kwargs): 
         def f2(**kwargs):
             par_args = list(kwargs.keys())[:n_args2parallelize]
             data_par_args = [kwargs[i] for i in par_args]
 
             fnc = np.vectorize(func)
-            print(fnc(**kwargs))
+            print('fnc', fnc(**kwargs))
             results = []
             for i, _ in enumerate(data_par_args[0]):
                 kwargs_0 = kwargs.copy()
                 for j, _ in enumerate(data_par_args):
                     kwargs_0[par_args[j]] = data_par_args[j][i]
                 r = func(**kwargs_0)
+                print('r', r)
                 results.append(r)
-            print(results)
+            print('results', results)
             return results
         @ray.remote(memory=MEM_PER_WORKER)
         def get_results(**kwargs):
             try:
                 args_names = ray.get(args_names_put)
                 args_vals  = ray.get(args_vals_put)
                 kwargs2 = dict(zip(args_names, args_vals))
@@ -88,54 +89,56 @@
             par_arg = {}
             for j in range(len(par_args)):
                 par_arg[par_args[j]] = arg2parallelize[j][i]
             workers.append(get_results.remote(**par_arg))
         result = ray.get(workers)
 
         r_test = result[0][0]
-        try:
+        if isinstance(r_test, tuple):
             n_outputs = len(r_test)
-        except TypeError:
+        else:
             n_outputs = 1
 
-        results = []
-        for i in range(n_outputs):
-            results.append([])
-        for i in range(len(result)):
-            for j in range(len(result[i])):
-                for k in range(n_outputs):
-                    try:
-                        results[k].append(result[i][j][k])
-                    except (TypeError, IndexError):
-                        results[k].append(result[i][j])
+        if n_outputs > 1:
+            results = []
+            for i in range(n_outputs):
+                results.append([])
+            for j in range(CPUS):
+                for output in result[j]:
+                    for k in range(n_outputs):
+                        results[k].append(output[k])
+        else:
+            results = []
+            for j in range(CPUS):
+                for output in result[j]:
+                    results.append(output)
+
         return results
     return wrap 
 
 
 if __name__ == "__main__":
     import timeit
     from scipy.integrate import quad
 
     @smart_parallelize
-    def func(x, y):
-        x = np.sum(x)
-        fnc = lambda x: np.exp(-x*y)
-        return quad(fnc, 0, x)[0]
+    def func(x):
+        return x
     
     x = np.ones((30,2))
     y = np.ones((30,))*2
     # y = 2
     start  = timeit.default_timer()
-    answer = func(x=x, y=y, n_args2parallelize=2)
+    answer = func(x=x)
     stop  = timeit.default_timer()
     print(stop - start)
     print(answer)
 
 
-    start  = timeit.default_timer()
-    answer = []
-    for i, val in enumerate(x):
-        sleep(1)
-        answer.append(val+y)
-    stop = timeit.default_timer()
-    print(stop - start)
+    # start  = timeit.default_timer()
+    # answer = []
+    # for i, val in enumerate(x):
+    #     sleep(1)
+    #     answer.append(val+y)
+    # stop = timeit.default_timer()
+    # print(stop - start)
```

### Comparing `smart_parallelize-2.0.4/PKG-INFO` & `smart_parallelize-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-parallelize
-Version: 2.0.4
+Version: 2.0.5
 Summary: 
 Author: Truman DeWalch
 Author-email: trumandewalch@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

