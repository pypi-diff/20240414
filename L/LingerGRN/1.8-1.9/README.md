# Comparing `tmp/LingerGRN-1.8.tar.gz` & `tmp/LingerGRN-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LingerGRN-1.8.tar", last modified: Mon Dec 11 14:05:52 2023, max compression
+gzip compressed data, was "LingerGRN-1.9.tar", last modified: Mon Dec 11 14:54:30 2023, max compression
```

## Comparing `LingerGRN-1.8.tar` & `LingerGRN-1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 qiuyuey  (432122) cuuser   (10000)        0 2023-12-11 14:05:52.117224 LingerGRN-1.8/
--rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)     1066 2023-10-12 02:45:49.000000 LingerGRN-1.8/LICENSE
-drwxr-xr-x   0 qiuyuey  (432122) cuuser   (10000)        0 2023-12-11 14:05:52.109224 LingerGRN-1.8/LingerGRN/
--rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)    11703 2023-12-11 14:04:37.000000 LingerGRN-1.8/LingerGRN/LINGER_tr.py
--rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)    33727 2023-11-07 02:13:37.000000 LingerGRN-1.8/LingerGRN/LL_net.py
--rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)     7500 2023-11-21 16:35:26.000000 LingerGRN-1.8/LingerGRN/TF_activity.py
--rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)        0 2023-10-12 02:38:34.000000 LingerGRN-1.8/LingerGRN/__init__.py
--rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)      647 2023-10-12 02:39:28.000000 LingerGRN-1.8/LingerGRN/immupute_dis.py
--rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)     9385 2023-12-11 13:16:14.000000 LingerGRN-1.8/LingerGRN/preprocess.py
--rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)     1764 2023-12-11 12:16:19.000000 LingerGRN-1.8/LingerGRN/pseudo_bulk.py
-drwxr-xr-x   0 qiuyuey  (432122) cuuser   (10000)        0 2023-12-11 14:05:52.115224 LingerGRN-1.8/LingerGRN.egg-info/
--rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)      226 2023-12-11 14:05:52.000000 LingerGRN-1.8/LingerGRN.egg-info/PKG-INFO
--rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)      585 2023-12-11 14:05:52.000000 LingerGRN-1.8/LingerGRN.egg-info/SOURCES.txt
--rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)        1 2023-12-11 14:05:52.000000 LingerGRN-1.8/LingerGRN.egg-info/dependency_links.txt
--rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)       50 2023-12-11 14:05:52.000000 LingerGRN-1.8/LingerGRN.egg-info/requires.txt
--rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)       10 2023-12-11 14:05:52.000000 LingerGRN-1.8/LingerGRN.egg-info/top_level.txt
--rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)      226 2023-12-11 14:05:52.116224 LingerGRN-1.8/PKG-INFO
--rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)     3394 2023-12-10 04:59:55.000000 LingerGRN-1.8/README.md
--rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)       38 2023-12-11 14:05:52.117224 LingerGRN-1.8/setup.cfg
--rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)      635 2023-12-11 14:05:44.000000 LingerGRN-1.8/setup.py
+drwxr-xr-x   0 qiuyuey  (432122) cuuser   (10000)        0 2023-12-11 14:54:30.124385 LingerGRN-1.9/
+-rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)     1066 2023-10-12 02:45:49.000000 LingerGRN-1.9/LICENSE
+drwxr-xr-x   0 qiuyuey  (432122) cuuser   (10000)        0 2023-12-11 14:54:30.117385 LingerGRN-1.9/LingerGRN/
+-rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)    11742 2023-12-11 14:53:57.000000 LingerGRN-1.9/LingerGRN/LINGER_tr.py
+-rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)    33727 2023-11-07 02:13:37.000000 LingerGRN-1.9/LingerGRN/LL_net.py
+-rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)     7500 2023-11-21 16:35:26.000000 LingerGRN-1.9/LingerGRN/TF_activity.py
+-rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)        0 2023-10-12 02:38:34.000000 LingerGRN-1.9/LingerGRN/__init__.py
+-rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)      647 2023-10-12 02:39:28.000000 LingerGRN-1.9/LingerGRN/immupute_dis.py
+-rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)     9385 2023-12-11 13:16:14.000000 LingerGRN-1.9/LingerGRN/preprocess.py
+-rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)     1764 2023-12-11 12:16:19.000000 LingerGRN-1.9/LingerGRN/pseudo_bulk.py
+drwxr-xr-x   0 qiuyuey  (432122) cuuser   (10000)        0 2023-12-11 14:54:30.122385 LingerGRN-1.9/LingerGRN.egg-info/
+-rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)      226 2023-12-11 14:54:30.000000 LingerGRN-1.9/LingerGRN.egg-info/PKG-INFO
+-rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)      585 2023-12-11 14:54:30.000000 LingerGRN-1.9/LingerGRN.egg-info/SOURCES.txt
+-rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)        1 2023-12-11 14:54:30.000000 LingerGRN-1.9/LingerGRN.egg-info/dependency_links.txt
+-rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)       50 2023-12-11 14:54:30.000000 LingerGRN-1.9/LingerGRN.egg-info/requires.txt
+-rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)       10 2023-12-11 14:54:30.000000 LingerGRN-1.9/LingerGRN.egg-info/top_level.txt
+-rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)      226 2023-12-11 14:54:30.123385 LingerGRN-1.9/PKG-INFO
+-rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)     3394 2023-12-10 04:59:55.000000 LingerGRN-1.9/README.md
+-rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)       38 2023-12-11 14:54:30.124385 LingerGRN-1.9/setup.cfg
+-rw-r--r--   0 qiuyuey  (432122) cuuser   (10000)      635 2023-12-11 14:54:09.000000 LingerGRN-1.9/setup.py
```

### Comparing `LingerGRN-1.8/LICENSE` & `LingerGRN-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `LingerGRN-1.8/LingerGRN/LINGER_tr.py` & `LingerGRN-1.9/LingerGRN/LINGER_tr.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,22 +266,24 @@
             REindex_bulk=idxRE_all.values[:,0]
             TFindex_bulk=idx_bulk.values[:,2]
             input_size_all=idx_bulk.values[:,3]
             fisherall = torch.load(GRNdir+'fisher_'+chr+'.pt')
             netall=torch.load(GRNdir+'all_models_'+chr+'.pt')
             res = Parallel(n_jobs = n_jobs)(delayed(sc_nn)(ii,gene_chr,TFindex,TFindex_bulk,REindex,REindex_bulk,REindex_bulk_match,Target,netall,adj_matrix_all,Exp,TF_match,input_size_all,fisherall,Opn,l1_lambda,fisher_w)
 for ii in range(N))
-            for ii in tqdm(range(N)):   #res=sc_nn(ii,gene_chr,TFindex,TFindex_bulk,REindex,REindex_bulk,REindex_bulk_match,Target,netall,adj_matrix_all,Exp,TF_match,input_size_all,fisherall,Opn,l1_lambda,fisher_w)
+            for ii in tqdm(range(N)):
+                warnings.filterwarnings("ignore")
+                res=sc_nn(ii,gene_chr,TFindex,TFindex_bulk,REindex,REindex_bulk,REindex_bulk_match,Target,netall,adj_matrix_all,Exp,TF_match,input_size_all,fisherall,Opn,l1_lambda,fisher_w)
                 index_all=gene_chr.index[ii]
-                if res[ii][4]==1:
-                    result[index_all,0]=res[ii][2]
-                    result[index_all,1]=res[ii][3]
-                    netall_s[index_all]=res[ii][0]
-                    shapall_s[index_all]=res[ii][1]
-                    Lossall[index_all,]=res[ii][5].T
+                if res[4]==1:
+                    result[index_all,0]=res[2]
+                    result[index_all,1]=res[3]
+                    netall_s[index_all]=res[0]
+                    shapall_s[index_all]=res[1]
+                    Lossall[index_all,]=res[5].T
                 else:
                     result[index_all,0]=-100
             result=pd.DataFrame(result)
             result.index=data_merge['Symbol'].values
             genetemp=data_merge[data_merge['chr']==chr]['Symbol'].values
             result=result.loc[genetemp]
             result.to_csv(outdir+'result_'+chr+'.txt',sep='\t')
```

### Comparing `LingerGRN-1.8/LingerGRN/LL_net.py` & `LingerGRN-1.9/LingerGRN/LL_net.py`

 * *Files identical despite different names*

### Comparing `LingerGRN-1.8/LingerGRN/TF_activity.py` & `LingerGRN-1.9/LingerGRN/TF_activity.py`

 * *Files identical despite different names*

### Comparing `LingerGRN-1.8/LingerGRN/immupute_dis.py` & `LingerGRN-1.9/LingerGRN/immupute_dis.py`

 * *Files identical despite different names*

### Comparing `LingerGRN-1.8/LingerGRN/preprocess.py` & `LingerGRN-1.9/LingerGRN/preprocess.py`

 * *Files identical despite different names*

### Comparing `LingerGRN-1.8/LingerGRN/pseudo_bulk.py` & `LingerGRN-1.9/LingerGRN/pseudo_bulk.py`

 * *Files identical despite different names*

### Comparing `LingerGRN-1.8/LingerGRN.egg-info/SOURCES.txt` & `LingerGRN-1.9/LingerGRN.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LingerGRN-1.8/README.md` & `LingerGRN-1.9/README.md`

 * *Files identical despite different names*

### Comparing `LingerGRN-1.8/setup.py` & `LingerGRN-1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='LingerGRN',
-    version='1.8',
+    version='1.9',
     description='Gene regulatory network inference',
     author='Kaya Yuan',
     author_email='qyyuan33@gmail.com',
     packages=['LingerGRN'],
     license = "MIT",
     url='https://github.com/Durenlab/LINGER',
     install_requires=['torch', 'scipy', 'numpy', 'pandas', 'shap', 'scikit-learn', 'joblib'],
```

