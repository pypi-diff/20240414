# Comparing `tmp/cad_to_dagmc-0.6.2.tar.gz` & `tmp/cad_to_dagmc-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cad_to_dagmc-0.6.2.tar", last modified: Mon Mar 18 23:51:43 2024, max compression
+gzip compressed data, was "cad_to_dagmc-0.7.0.tar", last modified: Sat Apr 13 23:51:49 2024, max compression
```

## Comparing `cad_to_dagmc-0.6.2.tar` & `cad_to_dagmc-0.7.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:51:43.424714 cad_to_dagmc-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:51:43.408714 cad_to_dagmc-0.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:51:43.412714 cad_to_dagmc-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/.github/workflows/anaconda-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/.github/workflows/ci_with_benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/.github/workflows/ci_with_install.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/.github/workflows/ci_with_pip_install.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-03-18 23:51:43.424714 cad_to_dagmc-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:51:43.412714 cad_to_dagmc-0.6.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:51:43.412714 cad_to_dagmc-0.6.2/examples/surface_mesh/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/examples/surface_mesh/cadquery_assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/examples/surface_mesh/cadquery_compound.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/examples/surface_mesh/cadquery_object_and_stp_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/examples/surface_mesh/cadquery_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/examples/surface_mesh/create_stp_files_for_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/examples/surface_mesh/curved_cadquery_object_to_dagmc_surface_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/examples/surface_mesh/multiple_cadquery_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/examples/surface_mesh/multiple_stp_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/examples/surface_mesh/single_cadquery_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/examples/surface_mesh/single_stp_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/examples/surface_mesh/single_stp_file_multiple_volumes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:51:43.416714 cad_to_dagmc-0.6.2/examples/unstrucutred_volume_mesh/
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/examples/unstrucutred_volume_mesh/curved_cadquery_object_to_dagmc_volume_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/examples/unstrucutred_volume_mesh/simulate_unstrucutred_volume_mesh_with_openmc.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 23:51:43.424714 cad_to_dagmc-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:51:43.416714 cad_to_dagmc-0.6.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-18 23:51:43.000000 cad_to_dagmc-0.6.2/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:51:43.416714 cad_to_dagmc-0.6.2/src/cad_to_dagmc/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/src/cad_to_dagmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18108 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/src/cad_to_dagmc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:51:43.424714 cad_to_dagmc-0.6.2/src/cad_to_dagmc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-03-18 23:51:43.000000 cad_to_dagmc-0.6.2/src/cad_to_dagmc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-03-18 23:51:43.000000 cad_to_dagmc-0.6.2/src/cad_to_dagmc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 23:51:43.000000 cad_to_dagmc-0.6.2/src/cad_to_dagmc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-18 23:51:43.000000 cad_to_dagmc-0.6.2/src/cad_to_dagmc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-18 23:51:43.000000 cad_to_dagmc-0.6.2/src/cad_to_dagmc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:51:43.424714 cad_to_dagmc-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    71272 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/ENDFB-7.1-NNDC_H1.h5
--rw-r--r--   0 runner    (1001) docker     (127)   267095 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/ball_reactor.brep
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/create_brep_file_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)  1760716 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/curved_extrude.stp
--rw-r--r--   0 runner    (1001) docker     (127)    54400 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/extrude_rectangle.step
--rw-r--r--   0 runner    (1001) docker     (127)    22142 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/extrude_rectangle.stp
--rw-r--r--   0 runner    (1001) docker     (127)    87541 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/multi_volume_cylinders.stp
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/one_cube.brep
--rw-r--r--   0 runner    (1001) docker     (127)    54148 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/single_cube.step
--rw-r--r--   0 runner    (1001) docker     (127)    15945 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/single_cube.stp
--rw-r--r--   0 runner    (1001) docker     (127)   212436 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/single_volume_thin.stp
--rw-r--r--   0 runner    (1001) docker     (127)  2013134 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/single_volume_thin.vtk
--rw-r--r--   0 runner    (1001) docker     (127)    11805 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/test_brep_file.brep
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/test_file_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/test_h5m_in_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/test_loading_from_file_vs_shape_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/test_python_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/test_two_joined_cubes.brep
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/test_two_sep_cubes.brep
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    33452 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/two_connected_cubes.stp
--rw-r--r--   0 runner    (1001) docker     (127)    33391 2024-03-18 23:51:29.000000 cad_to_dagmc-0.6.2/tests/two_disconnected_cubes.stp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:51:49.843331 cad_to_dagmc-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:51:49.827331 cad_to_dagmc-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:51:49.831331 cad_to_dagmc-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/.github/workflows/anaconda-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/.github/workflows/ci_with_benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/.github/workflows/ci_with_install.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/.github/workflows/ci_with_pip_install.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-13 23:51:49.843331 cad_to_dagmc-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:51:49.827331 cad_to_dagmc-0.7.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:51:49.831331 cad_to_dagmc-0.7.0/examples/surface_mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/examples/surface_mesh/cadquery_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/examples/surface_mesh/cadquery_compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/examples/surface_mesh/cadquery_object_and_stp_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/examples/surface_mesh/cadquery_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/examples/surface_mesh/curved_cadquery_object_to_dagmc_surface_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/examples/surface_mesh/from_gmsh_mesh_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/examples/surface_mesh/multiple_cadquery_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/examples/surface_mesh/multiple_stp_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/examples/surface_mesh/single_cadquery_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/examples/surface_mesh/single_stp_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/examples/surface_mesh/single_stp_file_multiple_volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:51:49.835331 cad_to_dagmc-0.7.0/examples/unstrucutred_volume_mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/examples/unstrucutred_volume_mesh/curved_cadquery_object_to_dagmc_volume_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/examples/unstrucutred_volume_mesh/simulate_unstrucutred_volume_mesh_with_openmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 23:51:49.843331 cad_to_dagmc-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:51:49.835331 cad_to_dagmc-0.7.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-13 23:51:49.000000 cad_to_dagmc-0.7.0/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:51:49.835331 cad_to_dagmc-0.7.0/src/cad_to_dagmc/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/src/cad_to_dagmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21495 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/src/cad_to_dagmc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:51:49.843331 cad_to_dagmc-0.7.0/src/cad_to_dagmc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-13 23:51:49.000000 cad_to_dagmc-0.7.0/src/cad_to_dagmc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-13 23:51:49.000000 cad_to_dagmc-0.7.0/src/cad_to_dagmc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 23:51:49.000000 cad_to_dagmc-0.7.0/src/cad_to_dagmc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-13 23:51:49.000000 cad_to_dagmc-0.7.0/src/cad_to_dagmc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 23:51:49.000000 cad_to_dagmc-0.7.0/src/cad_to_dagmc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:51:49.843331 cad_to_dagmc-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    71272 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/ENDFB-7.1-NNDC_H1.h5
+-rw-r--r--   0 runner    (1001) docker     (127)   267095 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/ball_reactor.brep
+-rw-r--r--   0 runner    (1001) docker     (127)  1760716 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/curved_extrude.stp
+-rw-r--r--   0 runner    (1001) docker     (127)    54400 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/extrude_rectangle.step
+-rw-r--r--   0 runner    (1001) docker     (127)    22142 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/extrude_rectangle.stp
+-rw-r--r--   0 runner    (1001) docker     (127)    87541 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/multi_volume_cylinders.stp
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/one_cube.brep
+-rw-r--r--   0 runner    (1001) docker     (127)    54148 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/single_cube.step
+-rw-r--r--   0 runner    (1001) docker     (127)    15945 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/single_cube.stp
+-rw-r--r--   0 runner    (1001) docker     (127)   212436 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/single_volume_thin.stp
+-rw-r--r--   0 runner    (1001) docker     (127)  2013134 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/single_volume_thin.vtk
+-rw-r--r--   0 runner    (1001) docker     (127)    11805 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/test_brep_file.brep
+-rw-r--r--   0 runner    (1001) docker     (127)     7805 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/test_file_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/test_h5m_in_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/test_loading_from_file_vs_shape_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/test_python_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/test_two_joined_cubes.brep
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/test_two_sep_cubes.brep
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33452 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/two_connected_cubes.stp
+-rw-r--r--   0 runner    (1001) docker     (127)    33391 2024-04-13 23:51:38.000000 cad_to_dagmc-0.7.0/tests/two_disconnected_cubes.stp
```

### Comparing `cad_to_dagmc-0.6.2/.github/workflows/anaconda-publish.yml` & `cad_to_dagmc-0.7.0/.github/workflows/anaconda-publish.yml`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/.github/workflows/black.yml` & `cad_to_dagmc-0.7.0/.github/workflows/black.yml`

 * *Files 19% similar despite different names*

```diff
@@ -9,24 +9,24 @@
   run:
     shell: bash
 
 jobs:
   black:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         ref: ${{ github.head_ref }}
     - name: Setup Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v5
       with:
         python-version: 3.x
     - name: Install black
       run: |
         python -m pip install --upgrade pip
         pip install black
     - name: Run black
       run: |
         black --line-length 100 .
-    - uses: stefanzweifel/git-auto-commit-action@v4
+    - uses: stefanzweifel/git-auto-commit-action@v5
       with:
         commit_message: "[skip ci] Apply formatting changes"
```

### Comparing `cad_to_dagmc-0.6.2/.github/workflows/ci_with_benchmarks.yml` & `cad_to_dagmc-0.7.0/.github/workflows/ci_with_benchmarks.yml`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/.github/workflows/ci_with_install.yml` & `cad_to_dagmc-0.7.0/.github/workflows/ci_with_install.yml`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,17 @@
   push:
     branches:
       - main
 
 jobs:
   testing:
     runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python-version: ["3.10", "3.11", "3.12"]
     steps:
       - name: Checkout repository
         uses: actions/checkout@v4
 
       - name: install non pypi dependencies
         shell: bash
         run: |
@@ -33,28 +36,28 @@
           source "${HOME}/conda/etc/profile.d/conda.sh"
           source "${HOME}/conda/etc/profile.d/mamba.sh"
           sudo apt-get --allow-releaseinfo-change update
           sudo apt-get update -y
           sudo apt-get upgrade -y
           sudo apt-get install -y libgl1-mesa-glx libgl1-mesa-dev libglu1-mesa-dev freeglut3-dev libosmesa6 libosmesa6-dev libgles2-mesa-dev libarchive-dev libpangocairo-1.0-0
           mamba activate
-          mamba create -y --name cad_to_dagmc python=3.10
+          mamba create -y --name cad_to_dagmc python=${{ matrix.python-version }}
           mamba activate cad_to_dagmc
           mamba install -y -c conda-forge "openmc=0.14.0=dagmc*nompi*" gmsh python-gmsh
           python -m pip install --upgrade pip 
           python -m pip install .
           python -c "import cad_to_dagmc"
           python -m pip install .[tests]
           pytest -v tests
-          python examples/surface_mesh/create_stp_files_for_examples.py
           python examples/surface_mesh/cadquery_assembly.py
           python examples/surface_mesh/cadquery_compound.py
           python examples/surface_mesh/cadquery_object_and_stp_file.py
           python examples/surface_mesh/cadquery_text.py
           python examples/surface_mesh/curved_cadquery_object_to_dagmc_surface_mesh.py
           python examples/surface_mesh/multiple_cadquery_objects.py
           python examples/surface_mesh/multiple_stp_files.py
           python examples/surface_mesh/single_stp_file_multiple_volumes.py
           python examples/surface_mesh/single_cadquery_object.py
           python examples/surface_mesh/single_stp_file.py
+          python examples/surface_mesh/from_gmsh_mesh_file.py
           python examples/unstrucutred_volume_mesh/curved_cadquery_object_to_dagmc_volume_mesh.py
           python examples/unstrucutred_volume_mesh/simulate_unstrucutred_volume_mesh_with_openmc.py
```

### Comparing `cad_to_dagmc-0.6.2/.github/workflows/python-publish.yml` & `cad_to_dagmc-0.7.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/.gitignore` & `cad_to_dagmc-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/LICENSE` & `cad_to_dagmc-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/PKG-INFO` & `cad_to_dagmc-0.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cad_to_dagmc
-Version: 0.6.2
+Version: 0.7.0
 Summary: Converts CAD files to a DAGMC h5m file
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 Project-URL: Homepage, https://github.com/fusion-energy/cad_to_dagmc
 Project-URL: Bug Tracker, https://github.com/fusion-energy/cad_to_dagmc/issues
 Keywords: dagmc,geometry,plot,slice
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -47,29 +47,78 @@
 
 This package is tested with [pytest tests](https://github.com/fusion-energy/cad_to_dagmc/tree/main/tests) and also the DAGMC geometry made with this package is compared to simulation carried out with native constructive solid geometry, see [Model Benchmark Zoo](https://github.com/fusion-energy/model_benchmark_zoo) for more details.
 
 Also checkout these other software projects that also create DAGMC geometry [CAD-to-OpenMC](https://github.com/openmsr/CAD_to_OpenMC), [Stellarmesh](https://github.com/Thea-Energy/stellarmesh) and [Coreform Cubit](https://coreform.com/products/coreform-cubit/)
 
 # Installation options
 
+- Install using Mamba
+- Install using Conda
 - Install using Mamba and pip
 - Install using Conda and pip
 - Install using pip and source compilations
 
+## Install using Mamba
+
+In principle, installing any Conda/Mamba distribution will work. A few Conda/Mamba options are:
+- [Miniforge](https://github.com/conda-forge/miniforge) (recommended as it includes mamba)
+- [Anaconda](https://www.anaconda.com/download)
+- [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
+
+This example assumes you have installed the Miniforge option or separately have installed Mamba with ```conda install -c conda-forge mamba -y```
+
+Create a new environment, I've chosen Python 3.10 here but newer versions are
+also supported.
+```bash
+mamba create --name new_env python=3.10 -y
+```
+
+Activate the environment
+```bash
+mamba activate new_env
+```
+
+Then you can install the cad_to_dagmc package
+```bash
+mamba install -y -c conda-forge cad_to_dagmc
+```
+
+## Install using Conda
+
+In principle, installing any Conda/Mamba distribution will work. A few Conda/Mamba options are:
+- [Miniforge](https://github.com/conda-forge/miniforge) (recommended as it includes mamba)
+- [Anaconda](https://www.anaconda.com/download)
+- [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
+
+Create a new environment, I've chosen Python 3.10 here but newer versions are
+also supported.
+```bash
+conda create --name new_env python=3.10 -y
+```
+
+Activate the environment
+```bash
+conda activate new_env
+```
+
+Then you can install the cad_to_dagmc package
+```bash
+conda install -y -c conda-forge cad_to_dagmc
+```
 
 ## Install using Mamba and pip
 
 In principle, installing any Conda/Mamba distribution will work. A few Conda/Mamba options are:
 - [Miniforge](https://github.com/conda-forge/miniforge) (recommended as it includes mamba)
 - [Anaconda](https://www.anaconda.com/download)
 - [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
 
 This example assumes you have installed the Miniforge option or separately have installed Mamba with ```conda install -c conda-forge mamba -y```
 
-Create a new conda environment, I've chosen Python 3.10 here but newer versions are
+Create a new environment, I've chosen Python 3.10 here but newer versions are
 also supported.
 ```bash
 mamba create --name new_env python=3.10 -y
 ```
 
 Activate the environment
 ```bash
@@ -77,45 +126,45 @@
 ```
 
 Install the dependencies
 ```bash
 mamba install -y -c conda-forge "moab>=5.3.0" gmsh python-gmsh
 ```
 
-Then you can install the cad_to_dagmc package with ```pip```
+Then you can install the cad_to_dagmc package
 ```bash
 pip install cad_to_dagmc
 ```
 
 
 ## Install using Conda and pip
 
 In principle, installing any Conda/Mamba distribution will work. A few Conda/Mamba options are:
 - [Miniforge](https://github.com/conda-forge/miniforge) (recommended as it includes mamba)
 - [Anaconda](https://www.anaconda.com/download)
 - [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
 
 This example uses Conda to install some dependencies that are not available via PyPi.
 
-Create a new conda environment
+Create a new environment
 ```bash
 conda create --name new_env python=3.10 -y
 ```
 
 Activate the environment
 ```bash
 conda activate new_env
 ```
 
 Install the dependencies
 ```bash
 conda install -y -c conda-forge "moab>=5.3.0" gmsh python-gmsh
 ```
 
-Then you can install the cad_to_dagmc package with ```pip```
+Then you can install the cad_to_dagmc package
 ```bash
 pip install cad_to_dagmc
 ```
 
 ## Install using pip and source compilations
 
 It should possible to avoid the use of conda and installing using pip and compiling from source.
@@ -126,51 +175,36 @@
 
 Then you can install the cad_to_dagmc package with ```pip```
 
 ```bash
 pip install cad_to_dagmc
 ```
 
-## Install with transport code (e.g OpenMC)
+## Install with OpenMC or other particle transport codes
 
 You may also want to install OpenMC with DAGMC to make use of the h5m geometry files produced in simulations. However you could also use other supported particle transport codes such as MCNP, FLUKA and others [link to DAGMC documentation](https://svalinn.github.io/DAGMC/).
 
 To install OpenMC you can run ```mamba install -c conda-forge openmc``` however this more specific command makes sure the latest version of OpenMC which contains DAGMC is chosen by conda / mamba
 ```bash
 mamba install -c conda-forge -y "openmc=0.14.0=dagmc*nompi*"
 ```
 
 It might not be possible to install OpenMC and cad-to-dagmc in the same conda/mamba python environment so you may have to create a new conda/mamba environment and install OpenMC there.
 
 Another option would be to [install OpenMC from source](https://docs.openmc.org/en/stable/quickinstall.html) which would also need compiling with MOAB and DAGMC options.
 
 
-
 # Known incompatibilities
 
 The package requires newer versions of Linux. For example the package does not work on Ubuntu 18.04 or older.
 
 The package requires newer versions of pip. It is recommended to ensure that your version of pip is up to date. This can be done with ```python -m pip install --upgrade pip```
 
 Installing one of the package dependancies (gmsh) with pip appears to result in occational errors when passing cad objects between cadquery / ocp and gmsh. The conda install gmsh appears to work fine.
 
-# Usage - with OpenMC
-
-You may also want to install OpenMC with DAGMC to make use of the h5m geometry files produced in simulations. However you could also use other supported particle transport codes such as MCNP, FLUKA and others supported by [DAGMC](https://svalinn.github.io/DAGMC/).
-
-You can run ```mamba install -c conda-forge openmc``` however this may choose to install OpenMC without DAGMC included.
-
-You can be more specific with conda/mamba commands to make sure the latest version of OpenMC which contains DAGMC is chosen by conda / mamba
-```bash
-mamba install -c conda-forge -y "openmc=0.14.0=dagmc*nompi*"
-```
-
-You could also [install OpenMC from source](https://docs.openmc.org/en/stable/quickinstall.html) which might be prefered as it can be tricky for the conda enviroment to get resolved.
-
-
 
 # Usage - creation of DAGMC h5m files
 
 For examples see the [examples folder](https://github.com/fusion-energy/cad_to_dagmc/tree/main/examples)
 
 # Usage - simulation with transport code
```

### Comparing `cad_to_dagmc-0.6.2/README.md` & `cad_to_dagmc-0.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -26,29 +26,78 @@
 
 This package is tested with [pytest tests](https://github.com/fusion-energy/cad_to_dagmc/tree/main/tests) and also the DAGMC geometry made with this package is compared to simulation carried out with native constructive solid geometry, see [Model Benchmark Zoo](https://github.com/fusion-energy/model_benchmark_zoo) for more details.
 
 Also checkout these other software projects that also create DAGMC geometry [CAD-to-OpenMC](https://github.com/openmsr/CAD_to_OpenMC), [Stellarmesh](https://github.com/Thea-Energy/stellarmesh) and [Coreform Cubit](https://coreform.com/products/coreform-cubit/)
 
 # Installation options
 
+- Install using Mamba
+- Install using Conda
 - Install using Mamba and pip
 - Install using Conda and pip
 - Install using pip and source compilations
 
+## Install using Mamba
+
+In principle, installing any Conda/Mamba distribution will work. A few Conda/Mamba options are:
+- [Miniforge](https://github.com/conda-forge/miniforge) (recommended as it includes mamba)
+- [Anaconda](https://www.anaconda.com/download)
+- [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
+
+This example assumes you have installed the Miniforge option or separately have installed Mamba with ```conda install -c conda-forge mamba -y```
+
+Create a new environment, I've chosen Python 3.10 here but newer versions are
+also supported.
+```bash
+mamba create --name new_env python=3.10 -y
+```
+
+Activate the environment
+```bash
+mamba activate new_env
+```
+
+Then you can install the cad_to_dagmc package
+```bash
+mamba install -y -c conda-forge cad_to_dagmc
+```
+
+## Install using Conda
+
+In principle, installing any Conda/Mamba distribution will work. A few Conda/Mamba options are:
+- [Miniforge](https://github.com/conda-forge/miniforge) (recommended as it includes mamba)
+- [Anaconda](https://www.anaconda.com/download)
+- [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
+
+Create a new environment, I've chosen Python 3.10 here but newer versions are
+also supported.
+```bash
+conda create --name new_env python=3.10 -y
+```
+
+Activate the environment
+```bash
+conda activate new_env
+```
+
+Then you can install the cad_to_dagmc package
+```bash
+conda install -y -c conda-forge cad_to_dagmc
+```
 
 ## Install using Mamba and pip
 
 In principle, installing any Conda/Mamba distribution will work. A few Conda/Mamba options are:
 - [Miniforge](https://github.com/conda-forge/miniforge) (recommended as it includes mamba)
 - [Anaconda](https://www.anaconda.com/download)
 - [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
 
 This example assumes you have installed the Miniforge option or separately have installed Mamba with ```conda install -c conda-forge mamba -y```
 
-Create a new conda environment, I've chosen Python 3.10 here but newer versions are
+Create a new environment, I've chosen Python 3.10 here but newer versions are
 also supported.
 ```bash
 mamba create --name new_env python=3.10 -y
 ```
 
 Activate the environment
 ```bash
@@ -56,45 +105,45 @@
 ```
 
 Install the dependencies
 ```bash
 mamba install -y -c conda-forge "moab>=5.3.0" gmsh python-gmsh
 ```
 
-Then you can install the cad_to_dagmc package with ```pip```
+Then you can install the cad_to_dagmc package
 ```bash
 pip install cad_to_dagmc
 ```
 
 
 ## Install using Conda and pip
 
 In principle, installing any Conda/Mamba distribution will work. A few Conda/Mamba options are:
 - [Miniforge](https://github.com/conda-forge/miniforge) (recommended as it includes mamba)
 - [Anaconda](https://www.anaconda.com/download)
 - [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
 
 This example uses Conda to install some dependencies that are not available via PyPi.
 
-Create a new conda environment
+Create a new environment
 ```bash
 conda create --name new_env python=3.10 -y
 ```
 
 Activate the environment
 ```bash
 conda activate new_env
 ```
 
 Install the dependencies
 ```bash
 conda install -y -c conda-forge "moab>=5.3.0" gmsh python-gmsh
 ```
 
-Then you can install the cad_to_dagmc package with ```pip```
+Then you can install the cad_to_dagmc package
 ```bash
 pip install cad_to_dagmc
 ```
 
 ## Install using pip and source compilations
 
 It should possible to avoid the use of conda and installing using pip and compiling from source.
@@ -105,51 +154,36 @@
 
 Then you can install the cad_to_dagmc package with ```pip```
 
 ```bash
 pip install cad_to_dagmc
 ```
 
-## Install with transport code (e.g OpenMC)
+## Install with OpenMC or other particle transport codes
 
 You may also want to install OpenMC with DAGMC to make use of the h5m geometry files produced in simulations. However you could also use other supported particle transport codes such as MCNP, FLUKA and others [link to DAGMC documentation](https://svalinn.github.io/DAGMC/).
 
 To install OpenMC you can run ```mamba install -c conda-forge openmc``` however this more specific command makes sure the latest version of OpenMC which contains DAGMC is chosen by conda / mamba
 ```bash
 mamba install -c conda-forge -y "openmc=0.14.0=dagmc*nompi*"
 ```
 
 It might not be possible to install OpenMC and cad-to-dagmc in the same conda/mamba python environment so you may have to create a new conda/mamba environment and install OpenMC there.
 
 Another option would be to [install OpenMC from source](https://docs.openmc.org/en/stable/quickinstall.html) which would also need compiling with MOAB and DAGMC options.
 
 
-
 # Known incompatibilities
 
 The package requires newer versions of Linux. For example the package does not work on Ubuntu 18.04 or older.
 
 The package requires newer versions of pip. It is recommended to ensure that your version of pip is up to date. This can be done with ```python -m pip install --upgrade pip```
 
 Installing one of the package dependancies (gmsh) with pip appears to result in occational errors when passing cad objects between cadquery / ocp and gmsh. The conda install gmsh appears to work fine.
 
-# Usage - with OpenMC
-
-You may also want to install OpenMC with DAGMC to make use of the h5m geometry files produced in simulations. However you could also use other supported particle transport codes such as MCNP, FLUKA and others supported by [DAGMC](https://svalinn.github.io/DAGMC/).
-
-You can run ```mamba install -c conda-forge openmc``` however this may choose to install OpenMC without DAGMC included.
-
-You can be more specific with conda/mamba commands to make sure the latest version of OpenMC which contains DAGMC is chosen by conda / mamba
-```bash
-mamba install -c conda-forge -y "openmc=0.14.0=dagmc*nompi*"
-```
-
-You could also [install OpenMC from source](https://docs.openmc.org/en/stable/quickinstall.html) which might be prefered as it can be tricky for the conda enviroment to get resolved.
-
-
 
 # Usage - creation of DAGMC h5m files
 
 For examples see the [examples folder](https://github.com/fusion-energy/cad_to_dagmc/tree/main/examples)
 
 # Usage - simulation with transport code
```

### Comparing `cad_to_dagmc-0.6.2/examples/surface_mesh/cadquery_compound.py` & `cad_to_dagmc-0.7.0/examples/surface_mesh/cadquery_compound.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 r2 = s2.lineTo(3.0, 0).lineTo(3.0, 1.0).spline(spline_points, includeCurrent=True).close()
 cq_shape_2 = r2.extrude(1)
 
 
 compound_of_shapes = cq.Compound.makeCompound([cq_shape_1.val(), cq_shape_2.val()])
 
 my_model = CadToDagmc()
-my_model.add_cadquery_object(object=compound_of_shapes)
-my_model.export_dagmc_h5m_file(max_mesh_size=0.2, min_mesh_size=0.1, material_tags=["mat1", "mat2"])
+my_model.add_cadquery_object(cadquery_object=compound_of_shapes, material_tags=["mat1", "mat2"])
+my_model.export_dagmc_h5m_file(max_mesh_size=0.2, min_mesh_size=0.1)
```

### Comparing `cad_to_dagmc-0.6.2/examples/surface_mesh/curved_cadquery_object_to_dagmc_surface_mesh.py` & `cad_to_dagmc-0.7.0/examples/surface_mesh/curved_cadquery_object_to_dagmc_surface_mesh.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,17 @@
     .circle(2)
     .cutThruAll()
 )
 
 
 my_model = CadToDagmc()
 
-my_model.add_cadquery_object(result)
+my_model.add_cadquery_object(
+    cadquery_object=result,
+    material_tags=["mat1"],
+)
 
 my_model.export_dagmc_h5m_file(
     filename="cadquery_objects_and_stp_files.h5m",
     max_mesh_size=1,
     min_mesh_size=0.1,
-    material_tags=["mat1"],
 )
```

### Comparing `cad_to_dagmc-0.6.2/examples/unstrucutred_volume_mesh/curved_cadquery_object_to_dagmc_volume_mesh.py` & `cad_to_dagmc-0.7.0/examples/unstrucutred_volume_mesh/curved_cadquery_object_to_dagmc_volume_mesh.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/examples/unstrucutred_volume_mesh/simulate_unstrucutred_volume_mesh_with_openmc.py` & `cad_to_dagmc-0.7.0/examples/unstrucutred_volume_mesh/simulate_unstrucutred_volume_mesh_with_openmc.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 openmc.config["cross_sections"] = "cross_sections.xml"
 
 umesh = openmc.UnstructuredMesh("umesh.h5m", library="moab")
 mesh_filter = openmc.MeshFilter(umesh)
 tally = openmc.Tally(name="unstrucutred_mesh_tally")
 tally.filters = [mesh_filter]
 tally.scores = ["flux"]
-tally.estimator = "tracklength"
 my_tallies = openmc.Tallies([tally])
 
 
 mat1 = openmc.Material()
 mat1.add_nuclide("H1", 1, percent_type="ao")
 mat1.set_density("g/cm3", 0.001)
 my_materials = openmc.Materials([mat1])
@@ -34,15 +33,14 @@
 cell1 = openmc.Cell(region=region1)
 cell1.fill = mat1
 
 my_geometry = openmc.Geometry([cell1])
 
 my_settings = openmc.Settings()
 my_settings.batches = 10
-my_settings.inactive = 0
 my_settings.particles = 5000
 my_settings.run_mode = "fixed source"
 
 # Create a DT point source
 my_source = openmc.IndependentSource()
 my_source.space = openmc.stats.Point((0, 0, 0))
 my_source.angle = openmc.stats.Isotropic()
```

### Comparing `cad_to_dagmc-0.6.2/pyproject.toml` & `cad_to_dagmc-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/src/cad_to_dagmc/core.py` & `cad_to_dagmc-0.7.0/src/cad_to_dagmc/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -185,29 +185,31 @@
 
     file_set = moab_core.create_meshset()
 
     moab_core.add_entities(file_set, all_sets)
 
     moab_core.write_file(h5m_filename)
 
+    print(f"written DAGMC file {h5m_filename}")
+
     return h5m_filename
 
 
 def _mesh_brep(
-    brep_object: str,
+    occ_shape: str,
     min_mesh_size: float = 1,
     max_mesh_size: float = 10,
     mesh_algorithm: int = 1,
     dimensions: int = 2,
 ):
     """Creates a conformal surface meshes of the volumes in a Brep file using
     Gmsh.
 
     Args:
-        brep_object: the filename of the Brep file to convert
+        occ_shape: the occ_shape of the Brep file to convert
         min_mesh_size: the minimum mesh element size to use in Gmsh. Passed
             into gmsh.option.setNumber("Mesh.MeshSizeMin", min_mesh_size)
         max_mesh_size: the maximum mesh element size to use in Gmsh. Passed
             into gmsh.option.setNumber("Mesh.MeshSizeMax", max_mesh_size)
         mesh_algorithm: The Gmsh mesh algorithm number to use. Passed into
             gmsh.option.setNumber("Mesh.Algorithm", mesh_algorithm)
         dimensions: The number of dimensions, 2 for a surface mesh 3 for a
@@ -216,43 +218,40 @@
     Returns:
         The resulting gmsh object and volumes
     """
 
     gmsh.initialize()
     gmsh.option.setNumber("General.Terminal", 1)
     gmsh.model.add("made_with_cad_to_dagmc_package")
-    volumes = gmsh.model.occ.importShapesNativePointer(brep_object)
+    volumes = gmsh.model.occ.importShapesNativePointer(occ_shape)
     gmsh.model.occ.synchronize()
 
     gmsh.option.setNumber("Mesh.Algorithm", mesh_algorithm)
     gmsh.option.setNumber("Mesh.MeshSizeMin", min_mesh_size)
     gmsh.option.setNumber("Mesh.MeshSizeMax", max_mesh_size)
     gmsh.model.mesh.generate(dimensions)
 
     return gmsh, volumes
 
 
-def _mesh_to_h5m_in_memory_method(
-    volumes,
-) -> str:
-    """Converts gmsh volumes into a DAGMC h5m file.
+def mesh_to_vertices_and_triangles(
+    dims_and_vol_ids,
+):
+    """Converts gmsh volumes into vertices and triangles for each face.
 
     Args:
         volumes: the volumes in the gmsh file, found with gmsh.model.occ.importShapes
-        material_tags: A list of material tags to tag the DAGMC volumes with.
-            Should be in the same order as the volumes
-        h5m_filename: the filename of the DAGMC h5m file to write
 
     Returns:
         vertices and triangles (grouped by solid then by face)
     """
 
     n = 3  # number of verts in a triangles
     triangles_by_solid_by_face = {}
-    for dim_and_vol in volumes:
+    for dim_and_vol in dims_and_vol_ids:
         # removes all groups so that the following getEntitiesForPhysicalGroup
         # command only finds surfaces for the volume
         gmsh.model.removePhysicalGroups()
 
         vol_id = dim_and_vol[1]
         entities_in_volume = gmsh.model.getAdjacencies(3, vol_id)
         surfaces_in_volume = entities_in_volume[1]
@@ -298,71 +297,162 @@
 def _get_ids_from_imprinted_assembly(solid_id_dict):
     ids = []
     for id in list(solid_id_dict.values()):
         ids.append(id[0])
     return ids
 
 
+def _check_material_tags(material_tags, iterable_solids):
+    if material_tags:
+        if len(material_tags) != len(iterable_solids):
+            msg = (
+                "When setting material_tags the number of material_tags \n"
+                "should be equal to the number of volumes in the CAD \n"
+                f"geometry {len(iterable_solids)} volumes found in model \n"
+                f"and {len(material_tags)} material_tags found"
+            )
+            raise ValueError(msg)
+        for material_tag in material_tags:
+            if not isinstance(material_tag, str):
+                msg = f"material_tags should be an iterable of strings."
+                raise ValueError(msg)
+
+
 def order_material_ids_by_brep_order(original_ids, scrambled_id, material_tags):
     material_tags_in_brep_order = []
     for brep_id in scrambled_id:
         id_of_solid_in_org = original_ids.index(brep_id)
         material_tags_in_brep_order.append(material_tags[id_of_solid_in_org])
     return material_tags_in_brep_order
 
 
+class MeshToDagmc:
+    """Convert a GMSH mesh file to a DAGMC h5m file"""
+
+    def __init__(self, filename: str):
+        self.filename = filename
+
+    # TODO add export_unstructured_mesh_file
+    # TODO add add_gmsh_msh_file
+
+    def export_dagmc_h5m_file(
+        self,
+        material_tags: typing.Iterable[str],
+        implicit_complement_material_tag: typing.Optional[str] = None,
+        filename: str = "dagmc.h5m",
+    ):
+        """Saves a DAGMC h5m file of the geometry
+
+        Args:
+            material_tags (typing.Iterable[str]): the names of the DAGMC
+                material tags to assign. These will need to be in the same
+                order as the volumes in the GMESH mesh and match the
+                material tags used in the neutronics code (e.g. OpenMC).
+            implicit_complement_material_tag (typing.Optional[str], optional):
+                the name of the material tag to use for the implicit
+                complement (void space). Defaults to None which is a vacuum.
+            filename (str, optional): _description_. Defaults to "dagmc.h5m".
+
+        Raises:
+            ValueError: _description_
+
+        Returns:
+            _type_: _description_
+        """
+
+        gmsh.initialize()
+        self.mesh_file = gmsh.open(self.filename)
+        dims_and_vol_ids = gmsh.model.getEntities(3)
+
+        if len(dims_and_vol_ids) != len(material_tags):
+            msg = f"Number of volumes {len(dims_and_vol_ids)} is not equal to number of material tags {len(material_tags)}"
+            raise ValueError(msg)
+
+        vertices, triangles_by_solid_by_face = mesh_to_vertices_and_triangles(
+            dims_and_vol_ids=dims_and_vol_ids
+        )
+
+        gmsh.finalize()
+
+        h5m_filename = _vertices_to_h5m(
+            vertices=vertices,
+            triangles_by_solid_by_face=triangles_by_solid_by_face,
+            material_tags=material_tags,
+            h5m_filename=filename,
+            implicit_complement_material_tag=implicit_complement_material_tag,
+        )
+
+        return h5m_filename
+
+
 class CadToDagmc:
+    """Converts Step files and CadQuery parts to a DAGMC h5m file"""
+
     def __init__(self):
         self.parts = []
+        self.material_tags = []
 
     def add_stp_file(
         self,
         filename: str,
         scale_factor: float = 1.0,
+        material_tags: typing.Optional[typing.Iterable[str]] = None,
     ):
         """Loads the parts from stp file into the model.
 
         Args:
             filename: the filename used to save the html graph.
-            material_tags: the names of the DAGMC material tags to assign.
-                These will need to be in the same order as the volumes in the
-                STP file and match the material tags used in the neutronics
-                code (e.g. OpenMC).
+            material_tags (typing.Iterable[str]): the names of the DAGMC
+                material tags to assign. These will need to be in the
+                same order as the volumes in the geometry added (STP
+                file and CadQuery objects) and match the material tags
+                used in the neutronics code (e.g. OpenMC).
             scale_factor: a scaling factor to apply to the geometry that can be
                 used to increase the size or decrease the size of the geometry.
                 Useful when converting the geometry to cm for use in neutronics
                 simulations.
         """
         part = importers.importStep(str(filename)).val()
 
         if scale_factor == 1.0:
             scaled_part = part
         else:
             scaled_part = part.scale(scale_factor)
-        self.add_cadquery_object(object=scaled_part)
+        self.add_cadquery_object(cadquery_object=scaled_part, material_tags=material_tags)
 
     def add_cadquery_object(
         self,
-        object: typing.Union[
+        cadquery_object: typing.Union[
             cq.assembly.Assembly, cq.occ_impl.shapes.Compound, cq.occ_impl.shapes.Solid
         ],
+        material_tags: typing.Optional[typing.Iterable[str]] = None,
     ):
         """Loads the parts from CadQuery object into the model.
 
         Args:
-            object: the cadquery object to convert
+            cadquery_object: the cadquery object to convert, can be a CadQuery assembly
+                cadquery workplane or a cadquery solid
+            material_tags (Optional typing.Iterable[str]): the names of the
+                DAGMC material tags to assign. These will need to be in the
+                same order as the volumes in the geometry added (STP file and
+                CadQuery objects) and match the material tags used in the
+                neutronics code (e.g. OpenMC).
         """
 
-        if isinstance(object, cq.assembly.Assembly):
-            object = object.toCompound()
+        if isinstance(cadquery_object, cq.assembly.Assembly):
+            cadquery_object = cadquery_object.toCompound()
 
-        if isinstance(object, (cq.occ_impl.shapes.Compound, cq.occ_impl.shapes.Solid)):
-            iterable_solids = object.Solids()
+        if isinstance(cadquery_object, (cq.occ_impl.shapes.Compound, cq.occ_impl.shapes.Solid)):
+            iterable_solids = cadquery_object.Solids()
         else:
-            iterable_solids = object.val().Solids()
+            iterable_solids = cadquery_object.val().Solids()
+
+        _check_material_tags(material_tags, iterable_solids)
+        if material_tags:
+            self.material_tags = self.material_tags + material_tags
         self.parts = self.parts + iterable_solids
 
     def export_unstructured_mesh_file(
         self,
         filename: str = "umesh.h5m",
         min_mesh_size: float = 1,
         max_mesh_size: float = 5,
@@ -371,16 +461,16 @@
 
         assembly = cq.Assembly()
         for part in self.parts:
             assembly.add(part)
 
         imprinted_assembly, _ = cq.occ_impl.assembly.imprint(assembly)
 
-        gmsh, volumes = _mesh_brep(
-            brep_object=imprinted_assembly.wrapped._address(),
+        gmsh, _ = _mesh_brep(
+            occ_shape=imprinted_assembly.wrapped._address(),
             min_mesh_size=min_mesh_size,
             max_mesh_size=max_mesh_size,
             mesh_algorithm=mesh_algorithm,
             dimensions=3,
         )
 
         # gmesh writes out a vtk file that is converted by pymoab into a h5 file
@@ -388,14 +478,16 @@
 
         moab_core = core.Core()
         moab_core.load_file(filename + ".vtk")
         moab_core.write_file(filename)
 
         gmsh.finalize()
 
+        return gmsh
+
     def export_gmsh_mesh_file(
         self,
         filename: str = "mesh.msh",
         min_mesh_size: float = 1,
         max_mesh_size: float = 5,
         mesh_algorithm: int = 1,
         dimensions: int = 2,
@@ -414,86 +506,86 @@
 
         assembly = cq.Assembly()
         for part in self.parts:
             assembly.add(part)
 
         imprinted_assembly, _ = cq.occ_impl.assembly.imprint(assembly)
 
-        gmsh, volumes = _mesh_brep(
-            brep_object=imprinted_assembly.wrapped._address(),
+        gmsh, _ = _mesh_brep(
+            occ_shape=imprinted_assembly.wrapped._address(),
             min_mesh_size=min_mesh_size,
             max_mesh_size=max_mesh_size,
             mesh_algorithm=mesh_algorithm,
             dimensions=dimensions,
         )
 
         gmsh.write(filename)
 
+        print(f"written GMSH mesh file {filename}")
+
         gmsh.finalize()
 
     def export_dagmc_h5m_file(
         self,
-        material_tags: typing.Iterable[str],
         filename: str = "dagmc.h5m",
         min_mesh_size: float = 1,
         max_mesh_size: float = 5,
         mesh_algorithm: int = 1,
         implicit_complement_material_tag: typing.Optional[str] = None,
-    ):
+    ) -> str:
         """Saves a DAGMC h5m file of the geometry
 
         Args:
-            filename
-            min_mesh_size: the minimum size of mesh elements to use.
-            max_mesh_size: the maximum size of mesh elements to use.
-            mesh_algorithm: the gmsh mesh algorithm to use.
-            material_tags: the names of the DAGMC material tags to assign.
-                These will need to be in the same order as the volumes in the
-                geometry geometry added (STP file and CadQuery objects) and
-                match the material tags used in the neutronics code (e.g. OpenMC).
-            implicit_complement_material_tag: the name of the material tag to
-                use for the implicit complement (void space). Defaults to None
-                which is a vacuum.
+
+            filename (str, optional): the filename to use for the saved DAGMC file. Defaults to "dagmc.h5m".
+            min_mesh_size (float, optional): the minimum size of mesh elements to use. Defaults to 1.
+            max_mesh_size (float, optional): the maximum size of mesh elements to use. Defaults to 5.
+            mesh_algorithm (int, optional): the GMSH mesh algorithm to use.. Defaults to 1.
+            implicit_complement_material_tag (typing.Optional[str], optional):
+                the name of the material tag to use for the implicit complement
+                (void space). Defaults to None which is a vacuum. Defaults to None.
+
+        Returns:
+            str: the DAGMC filename saved
         """
+
         assembly = cq.Assembly()
         for part in self.parts:
             assembly.add(part)
 
         imprinted_assembly, imprinted_solids_with_org_id = cq.occ_impl.assembly.imprint(assembly)
 
         original_ids = _get_ids_from_assembly(assembly)
         scrambled_ids = _get_ids_from_imprinted_assembly(imprinted_solids_with_org_id)
 
         # both id lists should be the same length as each other and the same
         # length as the self.material_tags
 
-        if len(original_ids) != len(material_tags):
-            msg = f"Number of volumes {len(original_ids)} is not equal to number of material tags {len(material_tags)}"
+        if len(original_ids) != len(self.material_tags):
+            msg = f"Number of volumes {len(original_ids)} is not equal to number of material tags {len(self.material_tags)}"
             raise ValueError(msg)
 
         material_tags_in_brep_order = order_material_ids_by_brep_order(
-            original_ids, scrambled_ids, material_tags
+            original_ids, scrambled_ids, self.material_tags
         )
 
+        _check_material_tags(material_tags_in_brep_order, self.parts)
+
         gmsh, volumes = _mesh_brep(
-            brep_object=imprinted_assembly.wrapped._address(),  # in memory address
+            occ_shape=imprinted_assembly.wrapped._address(),  # in memory address
             min_mesh_size=min_mesh_size,
             max_mesh_size=max_mesh_size,
             mesh_algorithm=mesh_algorithm,
         )
 
-        if isinstance(material_tags_in_brep_order, str):
-            msg = f"material_tags should be a list of strings, not a single string."
-            raise ValueError(msg)
-
-        if len(volumes) != len(material_tags_in_brep_order):
-            msg = f"{len(volumes)} volumes found in Brep file is not equal to the number of material_tags {len(material_tags_in_brep_order)} provided."
-            raise ValueError(msg)
+        dims_and_vol_ids = volumes
 
-        vertices, triangles_by_solid_by_face = _mesh_to_h5m_in_memory_method(volumes=volumes)
+        vertices, triangles_by_solid_by_face = mesh_to_vertices_and_triangles(
+            dims_and_vol_ids=dims_and_vol_ids
+        )
 
         gmsh.finalize()
 
         # checks and fixes triangle fix_normals within vertices_to_h5m
         return _vertices_to_h5m(
             vertices=vertices,
             triangles_by_solid_by_face=triangles_by_solid_by_face,
```

### Comparing `cad_to_dagmc-0.6.2/src/cad_to_dagmc.egg-info/PKG-INFO` & `cad_to_dagmc-0.7.0/src/cad_to_dagmc.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cad_to_dagmc
-Version: 0.6.2
+Version: 0.7.0
 Summary: Converts CAD files to a DAGMC h5m file
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 Project-URL: Homepage, https://github.com/fusion-energy/cad_to_dagmc
 Project-URL: Bug Tracker, https://github.com/fusion-energy/cad_to_dagmc/issues
 Keywords: dagmc,geometry,plot,slice
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -47,29 +47,78 @@
 
 This package is tested with [pytest tests](https://github.com/fusion-energy/cad_to_dagmc/tree/main/tests) and also the DAGMC geometry made with this package is compared to simulation carried out with native constructive solid geometry, see [Model Benchmark Zoo](https://github.com/fusion-energy/model_benchmark_zoo) for more details.
 
 Also checkout these other software projects that also create DAGMC geometry [CAD-to-OpenMC](https://github.com/openmsr/CAD_to_OpenMC), [Stellarmesh](https://github.com/Thea-Energy/stellarmesh) and [Coreform Cubit](https://coreform.com/products/coreform-cubit/)
 
 # Installation options
 
+- Install using Mamba
+- Install using Conda
 - Install using Mamba and pip
 - Install using Conda and pip
 - Install using pip and source compilations
 
+## Install using Mamba
+
+In principle, installing any Conda/Mamba distribution will work. A few Conda/Mamba options are:
+- [Miniforge](https://github.com/conda-forge/miniforge) (recommended as it includes mamba)
+- [Anaconda](https://www.anaconda.com/download)
+- [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
+
+This example assumes you have installed the Miniforge option or separately have installed Mamba with ```conda install -c conda-forge mamba -y```
+
+Create a new environment, I've chosen Python 3.10 here but newer versions are
+also supported.
+```bash
+mamba create --name new_env python=3.10 -y
+```
+
+Activate the environment
+```bash
+mamba activate new_env
+```
+
+Then you can install the cad_to_dagmc package
+```bash
+mamba install -y -c conda-forge cad_to_dagmc
+```
+
+## Install using Conda
+
+In principle, installing any Conda/Mamba distribution will work. A few Conda/Mamba options are:
+- [Miniforge](https://github.com/conda-forge/miniforge) (recommended as it includes mamba)
+- [Anaconda](https://www.anaconda.com/download)
+- [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
+
+Create a new environment, I've chosen Python 3.10 here but newer versions are
+also supported.
+```bash
+conda create --name new_env python=3.10 -y
+```
+
+Activate the environment
+```bash
+conda activate new_env
+```
+
+Then you can install the cad_to_dagmc package
+```bash
+conda install -y -c conda-forge cad_to_dagmc
+```
 
 ## Install using Mamba and pip
 
 In principle, installing any Conda/Mamba distribution will work. A few Conda/Mamba options are:
 - [Miniforge](https://github.com/conda-forge/miniforge) (recommended as it includes mamba)
 - [Anaconda](https://www.anaconda.com/download)
 - [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
 
 This example assumes you have installed the Miniforge option or separately have installed Mamba with ```conda install -c conda-forge mamba -y```
 
-Create a new conda environment, I've chosen Python 3.10 here but newer versions are
+Create a new environment, I've chosen Python 3.10 here but newer versions are
 also supported.
 ```bash
 mamba create --name new_env python=3.10 -y
 ```
 
 Activate the environment
 ```bash
@@ -77,45 +126,45 @@
 ```
 
 Install the dependencies
 ```bash
 mamba install -y -c conda-forge "moab>=5.3.0" gmsh python-gmsh
 ```
 
-Then you can install the cad_to_dagmc package with ```pip```
+Then you can install the cad_to_dagmc package
 ```bash
 pip install cad_to_dagmc
 ```
 
 
 ## Install using Conda and pip
 
 In principle, installing any Conda/Mamba distribution will work. A few Conda/Mamba options are:
 - [Miniforge](https://github.com/conda-forge/miniforge) (recommended as it includes mamba)
 - [Anaconda](https://www.anaconda.com/download)
 - [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
 
 This example uses Conda to install some dependencies that are not available via PyPi.
 
-Create a new conda environment
+Create a new environment
 ```bash
 conda create --name new_env python=3.10 -y
 ```
 
 Activate the environment
 ```bash
 conda activate new_env
 ```
 
 Install the dependencies
 ```bash
 conda install -y -c conda-forge "moab>=5.3.0" gmsh python-gmsh
 ```
 
-Then you can install the cad_to_dagmc package with ```pip```
+Then you can install the cad_to_dagmc package
 ```bash
 pip install cad_to_dagmc
 ```
 
 ## Install using pip and source compilations
 
 It should possible to avoid the use of conda and installing using pip and compiling from source.
@@ -126,51 +175,36 @@
 
 Then you can install the cad_to_dagmc package with ```pip```
 
 ```bash
 pip install cad_to_dagmc
 ```
 
-## Install with transport code (e.g OpenMC)
+## Install with OpenMC or other particle transport codes
 
 You may also want to install OpenMC with DAGMC to make use of the h5m geometry files produced in simulations. However you could also use other supported particle transport codes such as MCNP, FLUKA and others [link to DAGMC documentation](https://svalinn.github.io/DAGMC/).
 
 To install OpenMC you can run ```mamba install -c conda-forge openmc``` however this more specific command makes sure the latest version of OpenMC which contains DAGMC is chosen by conda / mamba
 ```bash
 mamba install -c conda-forge -y "openmc=0.14.0=dagmc*nompi*"
 ```
 
 It might not be possible to install OpenMC and cad-to-dagmc in the same conda/mamba python environment so you may have to create a new conda/mamba environment and install OpenMC there.
 
 Another option would be to [install OpenMC from source](https://docs.openmc.org/en/stable/quickinstall.html) which would also need compiling with MOAB and DAGMC options.
 
 
-
 # Known incompatibilities
 
 The package requires newer versions of Linux. For example the package does not work on Ubuntu 18.04 or older.
 
 The package requires newer versions of pip. It is recommended to ensure that your version of pip is up to date. This can be done with ```python -m pip install --upgrade pip```
 
 Installing one of the package dependancies (gmsh) with pip appears to result in occational errors when passing cad objects between cadquery / ocp and gmsh. The conda install gmsh appears to work fine.
 
-# Usage - with OpenMC
-
-You may also want to install OpenMC with DAGMC to make use of the h5m geometry files produced in simulations. However you could also use other supported particle transport codes such as MCNP, FLUKA and others supported by [DAGMC](https://svalinn.github.io/DAGMC/).
-
-You can run ```mamba install -c conda-forge openmc``` however this may choose to install OpenMC without DAGMC included.
-
-You can be more specific with conda/mamba commands to make sure the latest version of OpenMC which contains DAGMC is chosen by conda / mamba
-```bash
-mamba install -c conda-forge -y "openmc=0.14.0=dagmc*nompi*"
-```
-
-You could also [install OpenMC from source](https://docs.openmc.org/en/stable/quickinstall.html) which might be prefered as it can be tricky for the conda enviroment to get resolved.
-
-
 
 # Usage - creation of DAGMC h5m files
 
 For examples see the [examples folder](https://github.com/fusion-energy/cad_to_dagmc/tree/main/examples)
 
 # Usage - simulation with transport code
```

### Comparing `cad_to_dagmc-0.6.2/src/cad_to_dagmc.egg-info/SOURCES.txt` & `cad_to_dagmc-0.7.0/src/cad_to_dagmc.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 .github/workflows/ci_with_install.yml
 .github/workflows/ci_with_pip_install.yml
 .github/workflows/python-publish.yml
 examples/surface_mesh/cadquery_assembly.py
 examples/surface_mesh/cadquery_compound.py
 examples/surface_mesh/cadquery_object_and_stp_file.py
 examples/surface_mesh/cadquery_text.py
-examples/surface_mesh/create_stp_files_for_examples.py
 examples/surface_mesh/curved_cadquery_object_to_dagmc_surface_mesh.py
+examples/surface_mesh/from_gmsh_mesh_file.py
 examples/surface_mesh/multiple_cadquery_objects.py
 examples/surface_mesh/multiple_stp_files.py
 examples/surface_mesh/single_cadquery_object.py
 examples/surface_mesh/single_stp_file.py
 examples/surface_mesh/single_stp_file_multiple_volumes.py
 examples/unstrucutred_volume_mesh/curved_cadquery_object_to_dagmc_volume_mesh.py
 examples/unstrucutred_volume_mesh/simulate_unstrucutred_volume_mesh_with_openmc.py
@@ -27,15 +27,14 @@
 src/cad_to_dagmc.egg-info/PKG-INFO
 src/cad_to_dagmc.egg-info/SOURCES.txt
 src/cad_to_dagmc.egg-info/dependency_links.txt
 src/cad_to_dagmc.egg-info/requires.txt
 src/cad_to_dagmc.egg-info/top_level.txt
 tests/ENDFB-7.1-NNDC_H1.h5
 tests/ball_reactor.brep
-tests/create_brep_file_for_testing.py
 tests/curved_extrude.stp
 tests/extrude_rectangle.step
 tests/extrude_rectangle.stp
 tests/multi_volume_cylinders.stp
 tests/one_cube.brep
 tests/single_cube.step
 tests/single_cube.stp
```

### Comparing `cad_to_dagmc-0.6.2/tests/ENDFB-7.1-NNDC_H1.h5` & `cad_to_dagmc-0.7.0/tests/ENDFB-7.1-NNDC_H1.h5`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/tests/ball_reactor.brep` & `cad_to_dagmc-0.7.0/tests/ball_reactor.brep`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/tests/curved_extrude.stp` & `cad_to_dagmc-0.7.0/tests/curved_extrude.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/tests/extrude_rectangle.step` & `cad_to_dagmc-0.7.0/tests/extrude_rectangle.step`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/tests/extrude_rectangle.stp` & `cad_to_dagmc-0.7.0/tests/extrude_rectangle.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/tests/multi_volume_cylinders.stp` & `cad_to_dagmc-0.7.0/tests/multi_volume_cylinders.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/tests/one_cube.brep` & `cad_to_dagmc-0.7.0/tests/one_cube.brep`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/tests/single_cube.step` & `cad_to_dagmc-0.7.0/tests/single_cube.step`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/tests/single_cube.stp` & `cad_to_dagmc-0.7.0/tests/single_cube.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/tests/single_volume_thin.stp` & `cad_to_dagmc-0.7.0/tests/single_volume_thin.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/tests/single_volume_thin.vtk` & `cad_to_dagmc-0.7.0/tests/single_volume_thin.vtk`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/tests/test_brep_file.brep` & `cad_to_dagmc-0.7.0/tests/test_brep_file.brep`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/tests/test_file_creation.py` & `cad_to_dagmc-0.7.0/tests/test_file_creation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cad_to_dagmc import CadToDagmc
+from cad_to_dagmc import CadToDagmc, MeshToDagmc
 from pathlib import Path
 import cadquery as cq
 import pymoab as mb
 from pymoab import core, types
 
 """
 Tests that check that:
@@ -44,33 +44,39 @@
     return vol_mat
 
 
 def test_h5m_with_single_volume_list():
     """Simple geometry, a single 4 sided shape"""
 
     h5m_file = "tests/single_cube.h5m"
-
+    mesh_file = "test.msh"
     my_model = CadToDagmc()
-    my_model.add_stp_file(filename="tests/single_cube.stp")
-    my_model.export_dagmc_h5m_file(filename=h5m_file, material_tags=["mat1"])
-    my_model.export_gmsh_mesh_file(filename="test.msh")
-    assert Path("test.msh").is_file()
+    my_model.add_stp_file(filename="tests/single_cube.stp", material_tags=["mat1"])
+    my_model.export_dagmc_h5m_file(filename=h5m_file)
+    my_model.export_gmsh_mesh_file(filename=mesh_file)
+    assert Path(mesh_file).is_file()
     my_model.export_gmsh_mesh_file(filename="test3d.msh", dimensions=3)
     assert Path("test3d.msh").is_file()
     assert get_volumes_and_materials_from_h5m(h5m_file) == {1: "mat:mat1"}
 
+    h5m_file = "tests/single_cube_from_mesh.h5m"
+    my_model2 = MeshToDagmc(mesh_file)
+    my_model2.export_dagmc_h5m_file(filename=h5m_file, material_tags=["mat2"])
+    assert Path(h5m_file).is_file()
+    assert get_volumes_and_materials_from_h5m(h5m_file) == {1: "mat:mat2"}
+
 
 def test_h5m_with_single_volume_2():
     """Simple geometry, a single 4 sided shape"""
 
     h5m_file = "tests/curved_extrude.h5m"
 
     my_model = CadToDagmc()
-    my_model.add_stp_file(filename="tests/curved_extrude.stp")
-    my_model.export_dagmc_h5m_file(filename=h5m_file, material_tags=["mat1"])
+    my_model.add_stp_file(filename="tests/curved_extrude.stp", material_tags=["mat1"])
+    my_model.export_dagmc_h5m_file(filename=h5m_file)
 
     assert get_volumes_and_materials_from_h5m(h5m_file) == {1: "mat:mat1"}
 
 
 def test_h5m_with_multi_volume_not_touching():
     stp_files = [
         "tests/two_disconnected_cubes.stp",
@@ -79,17 +85,17 @@
         ["mat1", "mat2"],
     ]
     h5m_files = [
         "tests/two_disconnected_cubes.h5m",
     ]
     for stp_file, mat_tags, h5m_file in zip(stp_files, material_tags, h5m_files):
         my_model = CadToDagmc()
-        my_model.add_stp_file(filename=stp_file)
+        my_model.add_stp_file(filename=stp_file, material_tags=mat_tags)
 
-        my_model.export_dagmc_h5m_file(filename=h5m_file, material_tags=mat_tags)
+        my_model.export_dagmc_h5m_file(filename=h5m_file)
 
         tags_dict = {}
         for counter, loop_mat_tag in enumerate(mat_tags, 1):
             tags_dict[counter] = f"mat:{loop_mat_tag}"
         assert get_volumes_and_materials_from_h5m(h5m_file) == tags_dict
 
 
@@ -104,23 +110,28 @@
     ]
     h5m_files = [
         "tests/multi_volume_cylinders.h5m",
         "tests/two_connected_cubes.h5m",
     ]
     for stp_file, mat_tags, h5m_file in zip(stp_files, material_tags, h5m_files):
         my_model = CadToDagmc()
-        my_model.add_stp_file(stp_file)
+        my_model.add_stp_file(stp_file, material_tags=mat_tags)
 
-        my_model.export_dagmc_h5m_file(filename=h5m_file, material_tags=mat_tags)
+        my_model.export_dagmc_h5m_file(filename=h5m_file)
+        my_model.export_gmsh_mesh_file(filename=h5m_file + ".msh")
 
         tags_dict = {}
         for counter, loop_mat_tag in enumerate(mat_tags, 1):
             tags_dict[counter] = f"mat:{loop_mat_tag}"
         assert get_volumes_and_materials_from_h5m(h5m_file) == tags_dict
 
+        my_model2 = MeshToDagmc(filename=h5m_file + ".msh")
+        my_model2.export_dagmc_h5m_file(filename=h5m_file, material_tags=mat_tags)
+        assert get_volumes_and_materials_from_h5m(h5m_file) == tags_dict
+
 
 def test_cq_compound():
     # make other shapes from the CadQuery examples
     spline_points = [
         (2.75, 1.5),
         (2.5, 1.75),
         (2.0, 1.5),
@@ -137,20 +148,22 @@
     s2 = cq.Workplane("XY")
     r2 = s2.lineTo(3.0, 0).lineTo(3.0, 1.0).spline(spline_points, includeCurrent=True).close()
     cq_shape_2 = r2.extrude(1)
 
     compound_of_workplanes = cq.Compound.makeCompound([cq_shape_1.val(), cq_shape_2.val()])
 
     my_model = CadToDagmc()
-    my_model.add_cadquery_object(object=compound_of_workplanes)
+    my_model.add_cadquery_object(
+        cadquery_object=compound_of_workplanes,
+        material_tags=["mat1", "mat2"],
+    )
     my_model.export_dagmc_h5m_file(
         filename="compound_dagmc.h5m",
         max_mesh_size=0.2,
         min_mesh_size=0.1,
-        material_tags=["mat1", "mat2"],
     )
 
     assert Path("compound_dagmc.h5m").is_file()
     assert get_volumes_and_materials_from_h5m("compound_dagmc.h5m") == {
         1: "mat:mat1",
         2: "mat:mat2",
     }
@@ -189,15 +202,15 @@
         ["mat1", "mat2"],
     ]
     gmsh_mesh_files = [
         "tests/two_disconnected_cubes.msh",
     ]
     for stp_file, mat_tags, gmsh_mesh_file in zip(stp_files, material_tags, gmsh_mesh_files):
         my_model = CadToDagmc()
-        my_model.add_stp_file(filename=stp_file)
+        my_model.add_stp_file(filename=stp_file, material_tags=mat_tags)
 
         my_model.export_gmsh_mesh_file(filename=gmsh_mesh_file)
 
 
 def test_gmsh_mesh_with_multi_volume_touching():
     stp_files = [
         "tests/multi_volume_cylinders.stp",
@@ -209,14 +222,14 @@
     ]
     gmsh_mesh_files = [
         "tests/multi_volume_cylinders.msh",
         "tests/two_connected_cubes.msh",
     ]
     for stp_file, mat_tags, gmsh_mesh_file in zip(stp_files, material_tags, gmsh_mesh_files):
         my_model = CadToDagmc()
-        my_model.add_stp_file(stp_file)
+        my_model.add_stp_file(stp_file, material_tags=mat_tags)
 
         my_model.export_gmsh_mesh_file(filename=gmsh_mesh_file)
 
         tags_dict = {}
         for counter, loop_mat_tag in enumerate(mat_tags, 1):
             tags_dict[counter] = f"mat:{loop_mat_tag}"
```

### Comparing `cad_to_dagmc-0.6.2/tests/test_h5m_in_transport.py` & `cad_to_dagmc-0.7.0/tests/test_h5m_in_transport.py`

 * *Files 9% similar despite different names*

```diff
@@ -129,19 +129,17 @@
     material_tags = [f"material_{n}" for n in range(1, volumes + 1)]
 
     workplane1 = cq.Workplane("XY").cylinder(height=10, radius=4)
     workplane2 = cq.Workplane("XY").moveTo(0, 15).cylinder(height=10, radius=5)
     # cq.Assembly().add(workplane1).add(workplane2)
 
     my_model = CadToDagmc()
-    my_model.add_cadquery_object(workplane1)
-    my_model.add_cadquery_object(workplane2)
-    my_model.export_dagmc_h5m_file(
-        filename=h5m_filename, material_tags=[material_tags[0], material_tags[1]]
-    )
+    my_model.add_cadquery_object(workplane1, material_tags=[material_tags[0]])
+    my_model.add_cadquery_object(workplane2, material_tags=[material_tags[1]])
+    my_model.export_dagmc_h5m_file(filename=h5m_filename)
 
     transport_particles_on_h5m_geometry(
         h5m_filename=h5m_filename,
         material_tags=material_tags,
         nuclides=["H1"] * len(material_tags),
     )
 
@@ -151,16 +149,16 @@
     h5m_filename = "one_cylinder.h5m"
     volumes = 1
     material_tags = [f"material_{n}" for n in range(1, volumes + 1)]
 
     workplane1 = cq.Workplane("XY").cylinder(height=10, radius=4)
 
     my_model = CadToDagmc()
-    my_model.add_cadquery_object(workplane1)
-    my_model.export_dagmc_h5m_file(filename=h5m_filename, material_tags=[material_tags[0]])
+    my_model.add_cadquery_object(workplane1, material_tags=[material_tags[0]])
+    my_model.export_dagmc_h5m_file(filename=h5m_filename)
 
     transport_particles_on_h5m_geometry(
         h5m_filename=h5m_filename,
         material_tags=material_tags,
         nuclides=["H1"] * len(material_tags),
     )
 
@@ -171,18 +169,18 @@
     volumes = 2
     material_tags = [f"material_{n}" for n in range(1, volumes + 1)]
 
     workplane1 = cq.Workplane("XY").cylinder(height=10, radius=4)
     workplane2 = cq.Workplane("XY").cylinder(height=10, radius=5).cut(workplane1)
 
     my_model = CadToDagmc()
-    my_model.add_cadquery_object(workplane1)
-    my_model.add_cadquery_object(workplane2)
+    my_model.add_cadquery_object(workplane1, material_tags=[material_tags[0]])
+    my_model.add_cadquery_object(workplane2, material_tags=[material_tags[1]])
     my_model.export_dagmc_h5m_file(
-        filename=h5m_filename, material_tags=[material_tags[0], material_tags[1]]
+        filename=h5m_filename,
     )
 
     transport_particles_on_h5m_geometry(
         h5m_filename=h5m_filename,
         material_tags=material_tags,
         nuclides=["H1"] * len(material_tags),
     )
@@ -191,16 +189,16 @@
 @pytest.mark.skipif(openmc is None, reason="openmc tests only required for CI")
 def test_h5m_with_single_volume_list():
     """The simplest geometry, a single 4 sided shape with lists instead of np arrays"""
 
     h5m_file = "tests/single_cube.h5m"
 
     my_model = CadToDagmc()
-    my_model.add_stp_file(filename="tests/single_cube.stp")
-    my_model.export_dagmc_h5m_file(filename=h5m_file, material_tags=["mat1"])
+    my_model.add_stp_file(filename="tests/single_cube.stp", material_tags=["mat1"])
+    my_model.export_dagmc_h5m_file(filename=h5m_file)
 
     h5m_files = [
         "tests/single_cube.h5m",
     ]
 
     for h5m_file in h5m_files:
         transport_particles_on_h5m_geometry(
@@ -212,16 +210,18 @@
 
 @pytest.mark.skipif(openmc is None, reason="openmc tests only required for CI")
 def test_h5m_with_multi_volume_not_touching():
 
     h5m_file = "tests/two_disconnected_cubes.h5m"
 
     my_model = CadToDagmc()
-    my_model.add_stp_file(filename="tests/two_disconnected_cubes.stp")
-    my_model.export_dagmc_h5m_file(filename=h5m_file, material_tags=["mat1", "mat2"])
+    my_model.add_stp_file(
+        filename="tests/two_disconnected_cubes.stp", material_tags=["mat1", "mat2"]
+    )
+    my_model.export_dagmc_h5m_file(filename=h5m_file)
 
     transport_particles_on_h5m_geometry(
         h5m_filename="tests/two_disconnected_cubes.h5m",
         material_tags=["mat1", "mat2"],
         nuclides=["H1", "H1"],
     )
 
@@ -239,16 +239,19 @@
     h5m_files = [
         "tests/multi_volume_cylinders.h5m",
         "tests/two_connected_cubes.h5m",
     ]
     for stp_file, mat_tags, h5m_file in zip(stp_files, material_tags, h5m_files):
 
         my_model = CadToDagmc()
-        my_model.add_stp_file(stp_file)
+        my_model.add_stp_file(
+            filename=stp_file,
+            material_tags=mat_tags,
+        )
 
-        my_model.export_dagmc_h5m_file(filename=h5m_file, material_tags=mat_tags)
+        my_model.export_dagmc_h5m_file(filename=h5m_file)
 
         transport_particles_on_h5m_geometry(
             h5m_filename=h5m_file,
             material_tags=mat_tags,
             nuclides=["H1"] * len(mat_tags),
         )
```

### Comparing `cad_to_dagmc-0.6.2/tests/test_loading_from_file_vs_shape_object.py` & `cad_to_dagmc-0.7.0/tests/test_loading_from_file_vs_shape_object.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/tests/test_python_api.py` & `cad_to_dagmc-0.7.0/tests/test_python_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,36 +44,33 @@
 
 def test_max_mesh_size_impacts_file_size():
     """Checks the reducing max_mesh_size value increases the file size"""
 
     sphere = cq.Workplane().sphere(100)
 
     c2d = CadToDagmc()
-    c2d.add_cadquery_object(sphere)
+    c2d.add_cadquery_object(sphere, material_tags=["m1"])
     os.system("rm *.h5m")
     c2d.export_dagmc_h5m_file(
         min_mesh_size=10,
         max_mesh_size=20,
         mesh_algorithm=1,
         filename="test_10_30.h5m",
-        material_tags=["m1"],
     )
     c2d.export_dagmc_h5m_file(
         min_mesh_size=20,
         max_mesh_size=30,
         mesh_algorithm=1,
         filename="test_20_30.h5m",
-        material_tags=["m1"],
     )
     c2d.export_dagmc_h5m_file(
         min_mesh_size=20,
         max_mesh_size=25,
         mesh_algorithm=1,
         filename="test_20_25.h5m",
-        material_tags=["m1"],
     )
 
     assert Path("test_10_30.h5m").is_file()
     assert Path("test_20_30.h5m").is_file()
     assert Path("test_20_25.h5m").is_file()
 
     large_file = Path("test_10_30.h5m").stat().st_size
@@ -87,24 +84,22 @@
     """Checks that a h5m file is created with the correct tags"""
 
     sphere1 = cq.Workplane().sphere(20)
     sphere2 = cq.Workplane().moveTo(100, 100).sphere(20)
     sphere3 = cq.Workplane().moveTo(-100, -100).sphere(20)
 
     c2d = CadToDagmc()
-    c2d.add_cadquery_object(sphere1)
-    c2d.add_cadquery_object(sphere2)
-    c2d.add_cadquery_object(sphere3)
+    c2d.add_cadquery_object(sphere1, material_tags=["mat1"])
+    c2d.add_cadquery_object(sphere2, material_tags=["mat2"])
+    c2d.add_cadquery_object(sphere3, material_tags=["mat3"])
 
     test_h5m_filename = "test_dagmc.h5m"
     os.system(f"rm {test_h5m_filename}")
 
-    returned_filename = c2d.export_dagmc_h5m_file(
-        filename=test_h5m_filename, material_tags=["mat1", "mat2", "mat3"]
-    )
+    returned_filename = c2d.export_dagmc_h5m_file(filename=test_h5m_filename)
 
     assert Path(test_h5m_filename).is_file()
     assert Path(returned_filename).is_file()
     assert test_h5m_filename == returned_filename
 
     assert get_volumes_and_materials_from_h5m(test_h5m_filename) == {
         1: "mat:mat1",
```

### Comparing `cad_to_dagmc-0.6.2/tests/test_two_joined_cubes.brep` & `cad_to_dagmc-0.7.0/tests/test_two_joined_cubes.brep`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/tests/test_two_sep_cubes.brep` & `cad_to_dagmc-0.7.0/tests/test_two_sep_cubes.brep`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/tests/test_version.py` & `cad_to_dagmc-0.7.0/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/tests/two_connected_cubes.stp` & `cad_to_dagmc-0.7.0/tests/two_connected_cubes.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.6.2/tests/two_disconnected_cubes.stp` & `cad_to_dagmc-0.7.0/tests/two_disconnected_cubes.stp`

 * *Files identical despite different names*

