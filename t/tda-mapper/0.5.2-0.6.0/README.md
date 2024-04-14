# Comparing `tmp/tda-mapper-0.5.2.tar.gz` & `tmp/tda_mapper-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tda-mapper-0.5.2.tar", last modified: Tue Mar 26 21:06:52 2024, max compression
+gzip compressed data, was "tda_mapper-0.6.0.tar", last modified: Sun Apr 14 11:00:26 2024, max compression
```

## Comparing `tda-mapper-0.5.2.tar` & `tda_mapper-0.6.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 21:06:52.900543 tda-mapper-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19440 2024-03-26 21:06:52.900543 tda-mapper-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 21:06:52.900543 tda-mapper-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 21:06:52.892543 tda-mapper-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 21:06:52.900543 tda-mapper-0.5.2/src/tda_mapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19440 2024-03-26 21:06:52.000000 tda-mapper-0.5.2/src/tda_mapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-26 21:06:52.000000 tda-mapper-0.5.2/src/tda_mapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 21:06:52.000000 tda-mapper-0.5.2/src/tda_mapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-26 21:06:52.000000 tda-mapper-0.5.2/src/tda_mapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-26 21:06:52.000000 tda-mapper-0.5.2/src/tda_mapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 21:06:52.896543 tda-mapper-0.5.2/src/tdamapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/src/tdamapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/src/tdamapper/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    11254 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/src/tdamapper/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/src/tdamapper/cover.py
--rw-r--r--   0 runner    (1001) docker     (127)    20823 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/src/tdamapper/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/src/tdamapper/proximity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 21:06:52.896543 tda-mapper-0.5.2/src/tdamapper/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/src/tdamapper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/src/tdamapper/utils/heap.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1369 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/src/tdamapper/utils/quickselect.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/src/tdamapper/utils/unionfind.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6597 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/src/tdamapper/utils/vptree.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8073 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/src/tdamapper/utils/vptree_flat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 21:06:52.896543 tda-mapper-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/tests/test_heap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/tests/test_knn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/tests/test_proximity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      877 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/tests/test_quickselect.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/tests/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/tests/test_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/tests/test_unionfind.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/tests/test_vptree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-03-26 21:06:22.000000 tda-mapper-0.5.2/tests/test_vptree_bench.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:00:26.042859 tda_mapper-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19456 2024-04-14 11:00:26.042859 tda_mapper-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 11:00:26.042859 tda_mapper-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:00:26.034859 tda_mapper-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:00:26.042859 tda_mapper-0.6.0/src/tda_mapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19456 2024-04-14 11:00:26.000000 tda_mapper-0.6.0/src/tda_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-14 11:00:26.000000 tda_mapper-0.6.0/src/tda_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 11:00:26.000000 tda_mapper-0.6.0/src/tda_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-14 11:00:26.000000 tda_mapper-0.6.0/src/tda_mapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 11:00:26.000000 tda_mapper-0.6.0/src/tda_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:00:26.038859 tda_mapper-0.6.0/src/tdamapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/src/tdamapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/src/tdamapper/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11254 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/src/tdamapper/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/src/tdamapper/cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20823 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/src/tdamapper/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/src/tdamapper/proximity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:00:26.038859 tda_mapper-0.6.0/src/tdamapper/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/src/tdamapper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/src/tdamapper/utils/heap.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1369 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/src/tdamapper/utils/quickselect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/src/tdamapper/utils/unionfind.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6597 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/src/tdamapper/utils/vptree.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8073 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/src/tdamapper/utils/vptree_flat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:00:26.042859 tda_mapper-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/tests/test_heap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/tests/test_knn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/tests/test_proximity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      877 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/tests/test_quickselect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/tests/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/tests/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/tests/test_unionfind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/tests/test_vptree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-14 10:59:59.000000 tda_mapper-0.6.0/tests/test_vptree_bench.py
```

### Comparing `tda-mapper-0.5.2/LICENSE` & `tda_mapper-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/PKG-INFO` & `tda_mapper-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: tda-mapper
-Version: 0.5.2
+Version: 0.6.0
 Summary: A simple and efficient Python implementation of Mapper algorithm for Topological Data Analysis
 Author-email: Luca Simi <lucasimi90@gmail.com>
+Maintainer-email: Luca Simi <lucasimi90@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -202,14 +203,16 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/lucasimi/tda-mapper-python
+Project-URL: Documentation, https://tda-mapper.readthedocs.io
+Project-URL: Issues, https://github.com/lucasimi/tda-mapper-python/issues
 Keywords: tda,mapper,topology,topological data analysis
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -218,44 +221,61 @@
 Requires-Dist: numpy>=1.20.1
 Requires-Dist: plotly>=4.14.3
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: scikit-learn; extra == "dev"
 
+![Logo](https://github.com/lucasimi/tda-mapper-python/raw/main/docs/source/logos/tda-mapper-logo-horizontal.png)
+
 [![PyPI version](https://badge.fury.io/py/tda-mapper.svg)](https://badge.fury.io/py/tda-mapper)
 [![downloads](https://img.shields.io/pypi/dm/tda-mapper)](https://pypi.python.org/pypi/tda-mapper/)
 [![test](https://github.com/lucasimi/tda-mapper-python/actions/workflows/test.yml/badge.svg)](https://github.com/lucasimi/tda-mapper-python/actions/workflows/test.yml)
 [![deploy](https://github.com/lucasimi/tda-mapper-python/actions/workflows/deploy.yml/badge.svg)](https://github.com/lucasimi/tda-mapper-python/actions/workflows/deploy.yml)
 [![docs](https://readthedocs.org/projects/tda-mapper/badge/?version=main)](https://tda-mapper.readthedocs.io/en/main/?badge=main)
 [![codecov](https://codecov.io/github/lucasimi/tda-mapper-python/graph/badge.svg?token=FWSD8JUG6R)](https://codecov.io/github/lucasimi/tda-mapper-python)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10642381.svg)](https://doi.org/10.5281/zenodo.10642381)
+[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://tda-mapper-app.streamlit.app/)
 
 # tda-mapper
 
-A simple and efficient Python implementation of Mapper algorithm for Topological Data Analysis
+A simple and efficient Python implementation of Mapper algorithm for
+Topological Data Analysis
 
 * **Installation**: `pip install tda-mapper`
 
 * **Documentation**: https://tda-mapper.readthedocs.io/en/main/
 
-The Mapper algorithm is a well-known technique in the field of topological data analysis that allows data to be represented as a graph.
-Mapper is used in various fields such as machine learning, data mining, and social sciences, due to its ability to preserve topological features of the underlying space, providing a visual representation that facilitates exploration and interpretation.
-For an in-depth coverage of Mapper you can read [the original paper](https://research.math.osu.edu/tgda/mapperPBG.pdf).
+* **Demo App**: https://tda-mapper-app.streamlit.app/
+
+The Mapper algorithm is a well-known technique in the field of topological
+data analysis that allows data to be represented as a graph.
+Mapper is used in various fields such as machine learning, data mining, and
+social sciences, due to its ability to preserve topological features of the
+underlying space, providing a visual representation that facilitates
+exploration and interpretation. For an in-depth coverage of Mapper you can
+read
+[the original paper](https://research.math.osu.edu/tgda/mapperPBG.pdf).
+
+This library contains an implementation of Mapper, where the construction 
+of open covers is based on *vp-trees* for improved performance and scalability.
+The details about this methodology are contained in
+[our preprint](https://doi.org/10.5281/zenodo.10659652).
 
 | Step 1 | Step 2 | Step 3 | Step 4 |
-|--------|--------|--------|--------|
+| ------ | ------ | ------ | ------ |
 | ![Step 1](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/mapper_1.png) | ![Step 2](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/mapper_2.png) | ![Step 3](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/mapper_3.png) | ![Step 2](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/mapper_4.png) |
 | Chose lens | Cover image | Run clustering | Build graph |
 
 ## Example
 
-[Here](https://github.com/lucasimi/tda-mapper-python/raw/main/tests/example.py) you can find an example to use to kickstart your analysis.
-In this toy-example we use a two-dimensional dataset of two concentric circles.
-The Mapper graph is a topological summary of the whole point cloud.
+[Here](https://github.com/lucasimi/tda-mapper-python/raw/main/tests/example.py)
+you can find an example to use to kickstart your analysis. In this toy-example
+we use a two-dimensional dataset of two concentric circles. The Mapper graph
+is a topological summary of the whole point cloud.
 
 ```python
 import numpy as np
 
 from sklearn.datasets import make_circles
 from sklearn.decomposition import PCA
 from sklearn.cluster import DBSCAN
@@ -298,35 +318,33 @@
     agg=np.nanstd,                  # aggregate on nodes according to std
 )
 
 fig_std = mapper_plot.plot()
 fig_std.show(config={'scrollZoom': True})
 ```
 
-| Dataset                                                                                          | Mapper graph (average)                                                                                       | Mapper graph (deviation)                                                                                               |
-|--------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------|
+| Dataset | Mapper graph (average) | Mapper graph (deviation) |
+| ------- | ---------------------- | ------------------------ |
 | ![Dataset](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/circles_dataset.png) | ![Mapper graph (average)](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/circles_mean.png) | ![Mapper graph (standard deviation)](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/circles_std.png) |
 
-More examples can be found in the documentation https://tda-mapper.readthedocs.io/en/main/.
-
-## Citations
+More examples can be found in the
+[documentation](https://tda-mapper.readthedocs.io/en/main/).
 
-To cite **tda-mapper** in your work you can use the Zenodo archive https://doi.org/10.5281/zenodo.10642381.
+### Demo App
 
-In the archive you can find a permanent reference to the exact version you used in your work.
+You can also run a demo app locally by running
 
-For example, to cite version `v0.4.0` you can use:
+```
+pip install -r app/requirements.txt
+streamlit run app/streamlit_app.py
+```
 
-    Simi, L. (2024). tda-mapper (v0.4.0). Zenodo. https://doi.org/10.5281/zenodo.10655755
+## Citations
 
-BibTeX entry:
-
-    @software{tda-mapper_v0.4.0,
-      author       = {Simi, Luca},
-      title        = {tda-mapper},
-      month        = feb,
-      year         = 2024,
-      publisher    = {Zenodo},
-      version      = {v0.4.0},
-      doi          = {10.5281/zenodo.10655755},
-      url          = {https://doi.org/10.5281/zenodo.10655755}
-    }
+If you want to use **tda-mapper** in your work or research, you can cite the
+[archive uploaded on Zenodo](https://doi.org/10.5281/zenodo.10642381),
+pointing to the specific version of the software used in your work.
+
+If you want to cite the methodology on which **tda-mapper** is based, you can
+use the
+[preprint](https://doi.org/10.5281/zenodo.10659651).
+``
```

### Comparing `tda-mapper-0.5.2/README.md` & `tda_mapper-0.6.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,54 @@
+![Logo](https://github.com/lucasimi/tda-mapper-python/raw/main/docs/source/logos/tda-mapper-logo-horizontal.png)
+
 [![PyPI version](https://badge.fury.io/py/tda-mapper.svg)](https://badge.fury.io/py/tda-mapper)
 [![downloads](https://img.shields.io/pypi/dm/tda-mapper)](https://pypi.python.org/pypi/tda-mapper/)
 [![test](https://github.com/lucasimi/tda-mapper-python/actions/workflows/test.yml/badge.svg)](https://github.com/lucasimi/tda-mapper-python/actions/workflows/test.yml)
 [![deploy](https://github.com/lucasimi/tda-mapper-python/actions/workflows/deploy.yml/badge.svg)](https://github.com/lucasimi/tda-mapper-python/actions/workflows/deploy.yml)
 [![docs](https://readthedocs.org/projects/tda-mapper/badge/?version=main)](https://tda-mapper.readthedocs.io/en/main/?badge=main)
 [![codecov](https://codecov.io/github/lucasimi/tda-mapper-python/graph/badge.svg?token=FWSD8JUG6R)](https://codecov.io/github/lucasimi/tda-mapper-python)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10642381.svg)](https://doi.org/10.5281/zenodo.10642381)
+[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://tda-mapper-app.streamlit.app/)
 
 # tda-mapper
 
-A simple and efficient Python implementation of Mapper algorithm for Topological Data Analysis
+A simple and efficient Python implementation of Mapper algorithm for
+Topological Data Analysis
 
 * **Installation**: `pip install tda-mapper`
 
 * **Documentation**: https://tda-mapper.readthedocs.io/en/main/
 
-The Mapper algorithm is a well-known technique in the field of topological data analysis that allows data to be represented as a graph.
-Mapper is used in various fields such as machine learning, data mining, and social sciences, due to its ability to preserve topological features of the underlying space, providing a visual representation that facilitates exploration and interpretation.
-For an in-depth coverage of Mapper you can read [the original paper](https://research.math.osu.edu/tgda/mapperPBG.pdf).
+* **Demo App**: https://tda-mapper-app.streamlit.app/
+
+The Mapper algorithm is a well-known technique in the field of topological
+data analysis that allows data to be represented as a graph.
+Mapper is used in various fields such as machine learning, data mining, and
+social sciences, due to its ability to preserve topological features of the
+underlying space, providing a visual representation that facilitates
+exploration and interpretation. For an in-depth coverage of Mapper you can
+read
+[the original paper](https://research.math.osu.edu/tgda/mapperPBG.pdf).
+
+This library contains an implementation of Mapper, where the construction 
+of open covers is based on *vp-trees* for improved performance and scalability.
+The details about this methodology are contained in
+[our preprint](https://doi.org/10.5281/zenodo.10659652).
 
 | Step 1 | Step 2 | Step 3 | Step 4 |
-|--------|--------|--------|--------|
+| ------ | ------ | ------ | ------ |
 | ![Step 1](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/mapper_1.png) | ![Step 2](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/mapper_2.png) | ![Step 3](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/mapper_3.png) | ![Step 2](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/mapper_4.png) |
 | Chose lens | Cover image | Run clustering | Build graph |
 
 ## Example
 
-[Here](https://github.com/lucasimi/tda-mapper-python/raw/main/tests/example.py) you can find an example to use to kickstart your analysis.
-In this toy-example we use a two-dimensional dataset of two concentric circles.
-The Mapper graph is a topological summary of the whole point cloud.
+[Here](https://github.com/lucasimi/tda-mapper-python/raw/main/tests/example.py)
+you can find an example to use to kickstart your analysis. In this toy-example
+we use a two-dimensional dataset of two concentric circles. The Mapper graph
+is a topological summary of the whole point cloud.
 
 ```python
 import numpy as np
 
 from sklearn.datasets import make_circles
 from sklearn.decomposition import PCA
 from sklearn.cluster import DBSCAN
@@ -74,35 +91,33 @@
     agg=np.nanstd,                  # aggregate on nodes according to std
 )
 
 fig_std = mapper_plot.plot()
 fig_std.show(config={'scrollZoom': True})
 ```
 
-| Dataset                                                                                          | Mapper graph (average)                                                                                       | Mapper graph (deviation)                                                                                               |
-|--------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------|
+| Dataset | Mapper graph (average) | Mapper graph (deviation) |
+| ------- | ---------------------- | ------------------------ |
 | ![Dataset](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/circles_dataset.png) | ![Mapper graph (average)](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/circles_mean.png) | ![Mapper graph (standard deviation)](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/circles_std.png) |
 
-More examples can be found in the documentation https://tda-mapper.readthedocs.io/en/main/.
-
-## Citations
+More examples can be found in the
+[documentation](https://tda-mapper.readthedocs.io/en/main/).
 
-To cite **tda-mapper** in your work you can use the Zenodo archive https://doi.org/10.5281/zenodo.10642381.
+### Demo App
 
-In the archive you can find a permanent reference to the exact version you used in your work.
+You can also run a demo app locally by running
 
-For example, to cite version `v0.4.0` you can use:
+```
+pip install -r app/requirements.txt
+streamlit run app/streamlit_app.py
+```
 
-    Simi, L. (2024). tda-mapper (v0.4.0). Zenodo. https://doi.org/10.5281/zenodo.10655755
+## Citations
 
-BibTeX entry:
-
-    @software{tda-mapper_v0.4.0,
-      author       = {Simi, Luca},
-      title        = {tda-mapper},
-      month        = feb,
-      year         = 2024,
-      publisher    = {Zenodo},
-      version      = {v0.4.0},
-      doi          = {10.5281/zenodo.10655755},
-      url          = {https://doi.org/10.5281/zenodo.10655755}
-    }
+If you want to use **tda-mapper** in your work or research, you can cite the
+[archive uploaded on Zenodo](https://doi.org/10.5281/zenodo.10642381),
+pointing to the specific version of the software used in your work.
+
+If you want to cite the methodology on which **tda-mapper** is based, you can
+use the
+[preprint](https://doi.org/10.5281/zenodo.10659651).
+``
```

### Comparing `tda-mapper-0.5.2/src/tda_mapper.egg-info/PKG-INFO` & `tda_mapper-0.6.0/src/tda_mapper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: tda-mapper
-Version: 0.5.2
+Version: 0.6.0
 Summary: A simple and efficient Python implementation of Mapper algorithm for Topological Data Analysis
 Author-email: Luca Simi <lucasimi90@gmail.com>
+Maintainer-email: Luca Simi <lucasimi90@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -202,14 +203,16 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/lucasimi/tda-mapper-python
+Project-URL: Documentation, https://tda-mapper.readthedocs.io
+Project-URL: Issues, https://github.com/lucasimi/tda-mapper-python/issues
 Keywords: tda,mapper,topology,topological data analysis
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -218,44 +221,61 @@
 Requires-Dist: numpy>=1.20.1
 Requires-Dist: plotly>=4.14.3
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: scikit-learn; extra == "dev"
 
+![Logo](https://github.com/lucasimi/tda-mapper-python/raw/main/docs/source/logos/tda-mapper-logo-horizontal.png)
+
 [![PyPI version](https://badge.fury.io/py/tda-mapper.svg)](https://badge.fury.io/py/tda-mapper)
 [![downloads](https://img.shields.io/pypi/dm/tda-mapper)](https://pypi.python.org/pypi/tda-mapper/)
 [![test](https://github.com/lucasimi/tda-mapper-python/actions/workflows/test.yml/badge.svg)](https://github.com/lucasimi/tda-mapper-python/actions/workflows/test.yml)
 [![deploy](https://github.com/lucasimi/tda-mapper-python/actions/workflows/deploy.yml/badge.svg)](https://github.com/lucasimi/tda-mapper-python/actions/workflows/deploy.yml)
 [![docs](https://readthedocs.org/projects/tda-mapper/badge/?version=main)](https://tda-mapper.readthedocs.io/en/main/?badge=main)
 [![codecov](https://codecov.io/github/lucasimi/tda-mapper-python/graph/badge.svg?token=FWSD8JUG6R)](https://codecov.io/github/lucasimi/tda-mapper-python)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10642381.svg)](https://doi.org/10.5281/zenodo.10642381)
+[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://tda-mapper-app.streamlit.app/)
 
 # tda-mapper
 
-A simple and efficient Python implementation of Mapper algorithm for Topological Data Analysis
+A simple and efficient Python implementation of Mapper algorithm for
+Topological Data Analysis
 
 * **Installation**: `pip install tda-mapper`
 
 * **Documentation**: https://tda-mapper.readthedocs.io/en/main/
 
-The Mapper algorithm is a well-known technique in the field of topological data analysis that allows data to be represented as a graph.
-Mapper is used in various fields such as machine learning, data mining, and social sciences, due to its ability to preserve topological features of the underlying space, providing a visual representation that facilitates exploration and interpretation.
-For an in-depth coverage of Mapper you can read [the original paper](https://research.math.osu.edu/tgda/mapperPBG.pdf).
+* **Demo App**: https://tda-mapper-app.streamlit.app/
+
+The Mapper algorithm is a well-known technique in the field of topological
+data analysis that allows data to be represented as a graph.
+Mapper is used in various fields such as machine learning, data mining, and
+social sciences, due to its ability to preserve topological features of the
+underlying space, providing a visual representation that facilitates
+exploration and interpretation. For an in-depth coverage of Mapper you can
+read
+[the original paper](https://research.math.osu.edu/tgda/mapperPBG.pdf).
+
+This library contains an implementation of Mapper, where the construction 
+of open covers is based on *vp-trees* for improved performance and scalability.
+The details about this methodology are contained in
+[our preprint](https://doi.org/10.5281/zenodo.10659652).
 
 | Step 1 | Step 2 | Step 3 | Step 4 |
-|--------|--------|--------|--------|
+| ------ | ------ | ------ | ------ |
 | ![Step 1](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/mapper_1.png) | ![Step 2](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/mapper_2.png) | ![Step 3](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/mapper_3.png) | ![Step 2](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/mapper_4.png) |
 | Chose lens | Cover image | Run clustering | Build graph |
 
 ## Example
 
-[Here](https://github.com/lucasimi/tda-mapper-python/raw/main/tests/example.py) you can find an example to use to kickstart your analysis.
-In this toy-example we use a two-dimensional dataset of two concentric circles.
-The Mapper graph is a topological summary of the whole point cloud.
+[Here](https://github.com/lucasimi/tda-mapper-python/raw/main/tests/example.py)
+you can find an example to use to kickstart your analysis. In this toy-example
+we use a two-dimensional dataset of two concentric circles. The Mapper graph
+is a topological summary of the whole point cloud.
 
 ```python
 import numpy as np
 
 from sklearn.datasets import make_circles
 from sklearn.decomposition import PCA
 from sklearn.cluster import DBSCAN
@@ -298,35 +318,33 @@
     agg=np.nanstd,                  # aggregate on nodes according to std
 )
 
 fig_std = mapper_plot.plot()
 fig_std.show(config={'scrollZoom': True})
 ```
 
-| Dataset                                                                                          | Mapper graph (average)                                                                                       | Mapper graph (deviation)                                                                                               |
-|--------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------|
+| Dataset | Mapper graph (average) | Mapper graph (deviation) |
+| ------- | ---------------------- | ------------------------ |
 | ![Dataset](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/circles_dataset.png) | ![Mapper graph (average)](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/circles_mean.png) | ![Mapper graph (standard deviation)](https://github.com/lucasimi/tda-mapper-python/raw/main/resources/circles_std.png) |
 
-More examples can be found in the documentation https://tda-mapper.readthedocs.io/en/main/.
-
-## Citations
+More examples can be found in the
+[documentation](https://tda-mapper.readthedocs.io/en/main/).
 
-To cite **tda-mapper** in your work you can use the Zenodo archive https://doi.org/10.5281/zenodo.10642381.
+### Demo App
 
-In the archive you can find a permanent reference to the exact version you used in your work.
+You can also run a demo app locally by running
 
-For example, to cite version `v0.4.0` you can use:
+```
+pip install -r app/requirements.txt
+streamlit run app/streamlit_app.py
+```
 
-    Simi, L. (2024). tda-mapper (v0.4.0). Zenodo. https://doi.org/10.5281/zenodo.10655755
+## Citations
 
-BibTeX entry:
-
-    @software{tda-mapper_v0.4.0,
-      author       = {Simi, Luca},
-      title        = {tda-mapper},
-      month        = feb,
-      year         = 2024,
-      publisher    = {Zenodo},
-      version      = {v0.4.0},
-      doi          = {10.5281/zenodo.10655755},
-      url          = {https://doi.org/10.5281/zenodo.10655755}
-    }
+If you want to use **tda-mapper** in your work or research, you can cite the
+[archive uploaded on Zenodo](https://doi.org/10.5281/zenodo.10642381),
+pointing to the specific version of the software used in your work.
+
+If you want to cite the methodology on which **tda-mapper** is based, you can
+use the
+[preprint](https://doi.org/10.5281/zenodo.10659651).
+``
```

### Comparing `tda-mapper-0.5.2/src/tda_mapper.egg-info/SOURCES.txt` & `tda_mapper-0.6.0/src/tda_mapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/src/tdamapper/clustering.py` & `tda_mapper-0.6.0/src/tdamapper/clustering.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/src/tdamapper/core.py` & `tda_mapper-0.6.0/src/tdamapper/core.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/src/tdamapper/cover.py` & `tda_mapper-0.6.0/src/tdamapper/cover.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/src/tdamapper/plot.py` & `tda_mapper-0.6.0/src/tdamapper/plot.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/src/tdamapper/proximity.py` & `tda_mapper-0.6.0/src/tdamapper/proximity.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/src/tdamapper/utils/heap.py` & `tda_mapper-0.6.0/src/tdamapper/utils/heap.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/src/tdamapper/utils/quickselect.py` & `tda_mapper-0.6.0/src/tdamapper/utils/quickselect.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/src/tdamapper/utils/unionfind.py` & `tda_mapper-0.6.0/src/tdamapper/utils/unionfind.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/src/tdamapper/utils/vptree.py` & `tda_mapper-0.6.0/src/tdamapper/utils/vptree.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/src/tdamapper/utils/vptree_flat.py` & `tda_mapper-0.6.0/src/tdamapper/utils/vptree_flat.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/tests/test_core.py` & `tda_mapper-0.6.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/tests/test_cover.py` & `tda_mapper-0.6.0/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/tests/test_heap.py` & `tda_mapper-0.6.0/tests/test_heap.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/tests/test_knn.py` & `tda_mapper-0.6.0/tests/test_knn.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/tests/test_plot.py` & `tda_mapper-0.6.0/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/tests/test_proximity.py` & `tda_mapper-0.6.0/tests/test_proximity.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/tests/test_quickselect.py` & `tda_mapper-0.6.0/tests/test_quickselect.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/tests/test_sklearn.py` & `tda_mapper-0.6.0/tests/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/tests/test_vptree.py` & `tda_mapper-0.6.0/tests/test_vptree.py`

 * *Files identical despite different names*

### Comparing `tda-mapper-0.5.2/tests/test_vptree_bench.py` & `tda_mapper-0.6.0/tests/test_vptree_bench.py`

 * *Files identical despite different names*

