# Comparing `tmp/jarvis-tools-2024.3.4.tar.gz` & `tmp/jarvis-tools-2024.4.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarvis-tools-2024.3.4.tar", last modified: Wed Mar 20 07:14:03 2024, max compression
+gzip compressed data, was "jarvis-tools-2024.4.10.tar", last modified: Sun Apr 14 14:32:21 2024, max compression
```

## Comparing `jarvis-tools-2024.3.4.tar` & `jarvis-tools-2024.4.10.tar`

### file list

```diff
@@ -1,281 +1,282 @@
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.564155 jarvis-tools-2024.3.4/
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1878 2024-03-19 18:34:36.000000 jarvis-tools-2024.3.4/LICENSE.rst
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3510 2024-03-20 07:14:03.560155 jarvis-tools-2024.3.4/PKG-INFO
--rw-r--r--   0 knc6     (54782) 642div   (36677)    14481 2024-03-19 18:34:36.000000 jarvis-tools-2024.3.4/README.rst
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.008158 jarvis-tools-2024.3.4/jarvis/
--rw-r--r--   0 knc6     (54782) 642div   (36677)      244 2024-03-20 07:11:04.000000 jarvis-tools-2024.3.4/jarvis/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.012158 jarvis-tools-2024.3.4/jarvis/ai/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/ai/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.020158 jarvis-tools-2024.3.4/jarvis/ai/descriptors/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       48 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/ai/descriptors/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    48400 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/ai/descriptors/cfid.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1370 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/ai/descriptors/coulomb.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      511 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/ai/descriptors/elemental.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.020158 jarvis-tools-2024.3.4/jarvis/ai/gcn/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/ai/gcn/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.024158 jarvis-tools-2024.3.4/jarvis/ai/pkgs/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/ai/pkgs/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.032158 jarvis-tools-2024.3.4/jarvis/ai/pkgs/lgbm/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       28 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/ai/pkgs/lgbm/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1148 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/ai/pkgs/lgbm/classification.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     9541 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/ai/pkgs/lgbm/regression.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.040158 jarvis-tools-2024.3.4/jarvis/ai/pkgs/sklearn/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       44 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/ai/pkgs/sklearn/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5144 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/ai/pkgs/sklearn/classification.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    11368 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/ai/pkgs/sklearn/hyper_params.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2969 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/ai/pkgs/sklearn/regression.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3585 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/ai/pkgs/utils.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.044158 jarvis-tools-2024.3.4/jarvis/ai/uncertainty/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       34 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/ai/uncertainty/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5573 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/ai/uncertainty/gaussian_process_uncertainty.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7534 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/ai/uncertainty/lgbm_quantile_uncertainty.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.044158 jarvis-tools-2024.3.4/jarvis/analysis/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.048158 jarvis-tools-2024.3.4/jarvis/analysis/darkmatter/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       51 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/darkmatter/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      786 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/darkmatter/metrics.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.060158 jarvis-tools-2024.3.4/jarvis/analysis/defects/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/defects/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2328 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/defects/substitutions.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     9305 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/defects/surface.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5048 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/defects/vacancy.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.064158 jarvis-tools-2024.3.4/jarvis/analysis/diffraction/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       49 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/diffraction/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6825 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/diffraction/atomic_scattering_params.json
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7327 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/diffraction/xrd.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.068158 jarvis-tools-2024.3.4/jarvis/analysis/elastic/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       43 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/elastic/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6602 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/elastic/tensor.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.072158 jarvis-tools-2024.3.4/jarvis/analysis/interface/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       53 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/interface/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    14764 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/interface/zur.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.076158 jarvis-tools-2024.3.4/jarvis/analysis/magnetism/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       46 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/magnetism/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     8101 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/magnetism/magmom_setup.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.080158 jarvis-tools-2024.3.4/jarvis/analysis/periodic/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       49 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/periodic/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5907 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/periodic/ptable.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.088158 jarvis-tools-2024.3.4/jarvis/analysis/phonon/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       49 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/phonon/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3934 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/phonon/dos.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1189 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/phonon/force_constants.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6473 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/phonon/ir.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.096158 jarvis-tools-2024.3.4/jarvis/analysis/solarefficiency/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       59 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/solarefficiency/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    35436 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/solarefficiency/am1.5G.dat
--rw-r--r--   0 knc6     (54782) 642div   (36677)    14217 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/solarefficiency/solar.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.100158 jarvis-tools-2024.3.4/jarvis/analysis/stem/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       38 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/stem/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7315 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/stem/convolution_apprx.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.104158 jarvis-tools-2024.3.4/jarvis/analysis/stm/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       67 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/stm/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    10094 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/stm/tersoff_hamann.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.112157 jarvis-tools-2024.3.4/jarvis/analysis/structure/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       46 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/structure/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    21798 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/structure/neighbors.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    25663 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/structure/spacegroup.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.120157 jarvis-tools-2024.3.4/jarvis/analysis/thermodynamics/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       42 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/thermodynamics/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    14613 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/thermodynamics/energetics.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4527 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/thermodynamics/unary.json
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4781 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/thermodynamics/unary_qe_tb.json
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.124158 jarvis-tools-2024.3.4/jarvis/analysis/topological/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       50 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/topological/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    11892 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/analysis/topological/spillage.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.172157 jarvis-tools-2024.3.4/jarvis/core/
--rw-r--r--   0 knc6     (54782) 642div   (36677)  1421253 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/core/Elements.json
--rw-r--r--   0 knc6     (54782) 642div   (36677)       49 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/core/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    28393 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/core/atom_init.json
--rw-r--r--   0 knc6     (54782) 642div   (36677)    67369 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/core/atoms.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4313 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/core/circuits.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5258 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/core/composition.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)  1162701 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/core/element_charge.json
--rw-r--r--   0 knc6     (54782) 642div   (36677)    22651 2024-03-20 05:11:21.000000 jarvis-tools-2024.3.4/jarvis/core/graphs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    10693 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/core/image.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    37783 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/core/kpoints.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    17427 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/core/lattice.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    47766 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/core/magpie.json
--rw-r--r--   0 knc6     (54782) 642div   (36677)    12121 2024-03-20 03:28:49.000000 jarvis-tools-2024.3.4/jarvis/core/specie.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2891 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/core/spectrum.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     8933 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/core/utils.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.192157 jarvis-tools-2024.3.4/jarvis/db/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       53 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/db/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    26622 2024-03-19 18:36:20.000000 jarvis-tools-2024.3.4/jarvis/db/figshare.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      378 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/db/jsonutils.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7761 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/db/lammps_to_xml.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    10649 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/db/qe_to_xml.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    16857 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/db/restapi.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    75218 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/db/vasp_to_xml.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     9586 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/db/webpages.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.192157 jarvis-tools-2024.3.4/jarvis/io/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       76 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.200157 jarvis-tools-2024.3.4/jarvis/io/boltztrap/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       67 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/boltztrap/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6511 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/boltztrap/inputs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6767 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/boltztrap/outputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.204157 jarvis-tools-2024.3.4/jarvis/io/calphad/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       61 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/calphad/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4228 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/calphad/write_decorated_poscar.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.212157 jarvis-tools-2024.3.4/jarvis/io/lammps/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       52 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/lammps/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    14622 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/lammps/inputs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    20748 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/lammps/outputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.216157 jarvis-tools-2024.3.4/jarvis/io/nexus/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/nexus/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4519 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/nexus/inputs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)       36 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/nexus/outputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.220157 jarvis-tools-2024.3.4/jarvis/io/pennylane/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       61 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/pennylane/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2196 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/pennylane/inputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.228157 jarvis-tools-2024.3.4/jarvis/io/phonopy/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       43 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/phonopy/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4501 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/phonopy/fcmat2hr.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6844 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/phonopy/inputs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5696 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/phonopy/outputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.236157 jarvis-tools-2024.3.4/jarvis/io/prismatic/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       50 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/prismatic/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      674 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/prismatic/inputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.240157 jarvis-tools-2024.3.4/jarvis/io/qe/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       57 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/qe/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    15328 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/qe/inputs.py
--rwxr-xr-x   0 knc6     (54782) 642div   (36677)    29549 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/qe/outputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.248157 jarvis-tools-2024.3.4/jarvis/io/qiskit/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       56 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/qiskit/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    12104 2024-03-19 18:34:48.000000 jarvis-tools-2024.3.4/jarvis/io/qiskit/inputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.252157 jarvis-tools-2024.3.4/jarvis/io/tequila/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       60 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/tequila/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2702 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/tequila/inputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.260157 jarvis-tools-2024.3.4/jarvis/io/vasp/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       56 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/vasp/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1522 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/vasp/default_potcars.json
--rw-r--r--   0 knc6     (54782) 642div   (36677)    20248 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/vasp/inputs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    82300 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/vasp/outputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.272157 jarvis-tools-2024.3.4/jarvis/io/wannier/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       61 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/wannier/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4550 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/wannier/default_semicore.json
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6929 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/wannier/inputs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    34195 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/wannier/outputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.280156 jarvis-tools-2024.3.4/jarvis/io/wanniertools/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       60 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/wanniertools/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    10376 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/wanniertools/inputs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3818 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/wanniertools/outputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.288156 jarvis-tools-2024.3.4/jarvis/io/wien2k/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       55 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/wien2k/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3238 2024-03-19 19:19:17.000000 jarvis-tools-2024.3.4/jarvis/io/wien2k/inputs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3353 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/wien2k/outputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.296157 jarvis-tools-2024.3.4/jarvis/io/zeopp/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/zeopp/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2184 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/io/zeopp/inputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.300156 jarvis-tools-2024.3.4/jarvis/tasks/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.308156 jarvis-tools-2024.3.4/jarvis/tasks/boltztrap/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       56 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/boltztrap/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      608 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/boltztrap/run.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.312156 jarvis-tools-2024.3.4/jarvis/tasks/lammps/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       55 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/lammps/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    13948 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/lammps/lammps.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.344156 jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3463 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/displace.mod
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6416 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/inelast.mod
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6449 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/inelast_min.mod
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6418 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/inelast_nobox.mod
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6415 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/inelastcomb.mod
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6389 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/inelastreax.mod
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2653 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/relax.mod
--rw-r--r--   0 knc6     (54782) 642div   (36677)      145 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/run0.mod
--rw-r--r--   0 knc6     (54782) 642div   (36677)      917 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/templates.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.352156 jarvis-tools-2024.3.4/jarvis/tasks/nexus/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       34 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/nexus/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3243 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/nexus/qmc.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.356156 jarvis-tools-2024.3.4/jarvis/tasks/phonopy/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       54 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/phonopy/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      765 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/phonopy/run.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.376156 jarvis-tools-2024.3.4/jarvis/tasks/qe/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       29 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/qe/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    19582 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/qe/converg.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3665 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/qe/master_super.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4209 2024-03-19 18:37:20.000000 jarvis-tools-2024.3.4/jarvis/tasks/qe/qe.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    10588 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/qe/super.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7387 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/qe/super_tetra.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5873 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/queue_jobs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.384156 jarvis-tools-2024.3.4/jarvis/tasks/vasp/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       61 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/vasp/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    66478 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tasks/vasp/vasp.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.388156 jarvis-tools-2024.3.4/jarvis/tests/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.388156 jarvis-tools-2024.3.4/jarvis/tests/testfiles/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.400156 jarvis-tools-2024.3.4/jarvis/tests/testfiles/ai/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/ai/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      950 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/ai/test_ai_uncertainty.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    67390 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/ai/test_desc.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2206 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/ai/test_pkgs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.404156 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.408156 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/darkmatter/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/darkmatter/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      464 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/darkmatter/test_metrics.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.416156 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/defects/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/defects/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      444 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/defects/test_subs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3252 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/defects/test_surface.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1216 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/defects/test_vacancy.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.424156 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/elastic/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/elastic/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2577 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/elastic/test_tensor.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.428156 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/interface/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/interface/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     8683 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/interface/test_zur.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.432156 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/magnetism/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/magnetism/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      589 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/magnetism/test_magnetism.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.440156 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/phonon/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/phonon/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5121 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/phonon/test_dos.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      326 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/phonon/test_fc.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1279 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/phonon/test_ir.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.444156 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/solar/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/solar/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1399 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/solar/test_solar.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.452155 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/stm/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/stm/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1672 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/stm/test_stm.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.464156 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/structure/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/structure/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      390 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/structure/test_energetics.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1301 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/structure/test_neighbors.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3585 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/structure/test_spacegroup.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.472155 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/thermodynamics/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/thermodynamics/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1554 2024-03-19 18:34:37.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/thermodynamics/test_energetics.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.476155 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/topological/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-19 18:34:38.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/topological/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      424 2024-03-19 18:34:38.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/topological/test_spillage.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.516155 jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-19 18:34:38.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5666 2024-03-19 18:34:38.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/p.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5483 2024-03-19 18:34:38.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/test_atoms.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      262 2024-03-19 18:34:38.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/test_circuits.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      481 2024-03-19 18:34:38.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/test_composition.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2844 2024-03-19 18:34:38.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/test_graph.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    11116 2024-03-19 18:34:38.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/test_kpoints.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1507 2024-03-19 18:34:38.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/test_latice.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      339 2024-03-19 18:34:38.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/test_pdb.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      551 2024-03-19 18:34:38.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/test_specie.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      541 2024-03-19 18:34:38.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/test_utils.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.520155 jarvis-tools-2024.3.4/jarvis/tests/testfiles/db/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-19 18:34:38.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/db/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1496 2024-03-19 18:34:38.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/db/test_figshare.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.532155 jarvis-tools-2024.3.4/jarvis/tests/testfiles/tasks/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-19 18:34:39.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/tasks/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      804 2024-03-19 18:34:39.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/tasks/test_lammps.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      696 2024-03-19 18:34:39.000000 jarvis-tools-2024.3.4/jarvis/tests/testfiles/tasks/test_vasp.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-20 07:14:03.548155 jarvis-tools-2024.3.4/jarvis_tools.egg-info/
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3510 2024-03-20 07:14:02.000000 jarvis-tools-2024.3.4/jarvis_tools.egg-info/PKG-INFO
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7565 2024-03-20 07:14:02.000000 jarvis-tools-2024.3.4/jarvis_tools.egg-info/SOURCES.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)        1 2024-03-20 07:14:02.000000 jarvis-tools-2024.3.4/jarvis_tools.egg-info/dependency_links.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)      304 2024-03-20 07:14:02.000000 jarvis-tools-2024.3.4/jarvis_tools.egg-info/requires.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)        7 2024-03-20 07:14:02.000000 jarvis-tools-2024.3.4/jarvis_tools.egg-info/top_level.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)      195 2024-03-20 07:14:03.568155 jarvis-tools-2024.3.4/setup.cfg
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2644 2024-03-20 07:11:04.000000 jarvis-tools-2024.3.4/setup.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.740308 jarvis-tools-2024.4.10/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1878 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/LICENSE.rst
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3442 2024-04-14 14:32:21.740308 jarvis-tools-2024.4.10/PKG-INFO
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    14481 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/README.rst
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:18.588327 jarvis-tools-2024.4.10/jarvis/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      245 2024-04-14 13:11:23.000000 jarvis-tools-2024.4.10/jarvis/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:18.592327 jarvis-tools-2024.4.10/jarvis/ai/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:18.704326 jarvis-tools-2024.4.10/jarvis/ai/descriptors/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       48 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/descriptors/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    48400 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/descriptors/cfid.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1370 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/descriptors/coulomb.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      511 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/descriptors/elemental.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:18.716326 jarvis-tools-2024.4.10/jarvis/ai/gcn/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/gcn/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:18.780326 jarvis-tools-2024.4.10/jarvis/ai/pkgs/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/pkgs/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:18.840325 jarvis-tools-2024.4.10/jarvis/ai/pkgs/lgbm/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       28 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/pkgs/lgbm/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1148 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/pkgs/lgbm/classification.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     9541 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/pkgs/lgbm/regression.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:18.932325 jarvis-tools-2024.4.10/jarvis/ai/pkgs/sklearn/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       44 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/pkgs/sklearn/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5144 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/pkgs/sklearn/classification.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    11368 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/pkgs/sklearn/hyper_params.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2969 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/pkgs/sklearn/regression.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3585 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/pkgs/utils.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.000324 jarvis-tools-2024.4.10/jarvis/ai/uncertainty/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       34 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/uncertainty/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5573 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/uncertainty/gaussian_process_uncertainty.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7534 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/uncertainty/lgbm_quantile_uncertainty.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.024324 jarvis-tools-2024.4.10/jarvis/analysis/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.052324 jarvis-tools-2024.4.10/jarvis/analysis/darkmatter/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       51 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/darkmatter/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      786 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/darkmatter/metrics.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.148323 jarvis-tools-2024.4.10/jarvis/analysis/defects/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/defects/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2328 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/defects/substitutions.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     9305 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/defects/surface.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5048 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/defects/vacancy.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.180323 jarvis-tools-2024.4.10/jarvis/analysis/diffraction/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       49 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/diffraction/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6825 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/diffraction/atomic_scattering_params.json
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7327 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/diffraction/xrd.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.200323 jarvis-tools-2024.4.10/jarvis/analysis/elastic/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       43 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/elastic/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6602 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/elastic/tensor.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.260323 jarvis-tools-2024.4.10/jarvis/analysis/interface/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       53 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/interface/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    14764 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/interface/zur.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.296323 jarvis-tools-2024.4.10/jarvis/analysis/magnetism/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       46 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/magnetism/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     8101 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/magnetism/magmom_setup.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.332322 jarvis-tools-2024.4.10/jarvis/analysis/periodic/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       49 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/periodic/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5907 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/periodic/ptable.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.424322 jarvis-tools-2024.4.10/jarvis/analysis/phonon/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       49 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/phonon/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3934 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/phonon/dos.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1189 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/phonon/force_constants.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6473 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/phonon/ir.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.496321 jarvis-tools-2024.4.10/jarvis/analysis/solarefficiency/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       59 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/solarefficiency/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    35436 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/solarefficiency/am1.5G.dat
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    14217 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/solarefficiency/solar.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.544321 jarvis-tools-2024.4.10/jarvis/analysis/stem/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       38 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/stem/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7315 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/stem/convolution_apprx.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.564321 jarvis-tools-2024.4.10/jarvis/analysis/stm/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       67 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/stm/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    10094 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/stm/tersoff_hamann.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.588321 jarvis-tools-2024.4.10/jarvis/analysis/structure/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       46 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/structure/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    21798 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/structure/neighbors.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    25663 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/structure/spacegroup.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.696320 jarvis-tools-2024.4.10/jarvis/analysis/thermodynamics/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       42 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/thermodynamics/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    14613 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/thermodynamics/energetics.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4527 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/thermodynamics/unary.json
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4781 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/thermodynamics/unary_qe_tb.json
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.716320 jarvis-tools-2024.4.10/jarvis/analysis/topological/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       50 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/topological/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    11892 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/topological/spillage.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.856319 jarvis-tools-2024.4.10/jarvis/core/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)  1421253 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/Elements.json
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       49 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    28393 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/atom_init.json
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    74159 2024-04-14 12:46:57.000000 jarvis-tools-2024.4.10/jarvis/core/atoms.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4313 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/circuits.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5258 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/composition.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)  1162701 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/element_charge.json
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    22713 2024-04-14 12:39:39.000000 jarvis-tools-2024.4.10/jarvis/core/graphs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    10693 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/image.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    37783 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/kpoints.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    17427 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/lattice.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    47766 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/magpie.json
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    12121 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/specie.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2891 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/spectrum.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     8933 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/utils.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.968319 jarvis-tools-2024.4.10/jarvis/db/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       53 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/db/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    26622 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/db/figshare.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      378 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/db/jsonutils.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7761 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/db/lammps_to_xml.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    10649 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/db/qe_to_xml.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    17359 2024-03-31 16:17:56.000000 jarvis-tools-2024.4.10/jarvis/db/restapi.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    75218 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/db/vasp_to_xml.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     9586 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/db/webpages.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.992318 jarvis-tools-2024.4.10/jarvis/io/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       76 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.048318 jarvis-tools-2024.4.10/jarvis/io/boltztrap/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       67 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/boltztrap/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6511 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/boltztrap/inputs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6767 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/boltztrap/outputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.100318 jarvis-tools-2024.4.10/jarvis/io/calphad/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       61 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/calphad/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4228 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/calphad/write_decorated_poscar.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.156318 jarvis-tools-2024.4.10/jarvis/io/lammps/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       52 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/lammps/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    14615 2024-03-31 15:24:29.000000 jarvis-tools-2024.4.10/jarvis/io/lammps/inputs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    20760 2024-03-31 15:15:06.000000 jarvis-tools-2024.4.10/jarvis/io/lammps/outputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.240317 jarvis-tools-2024.4.10/jarvis/io/nexus/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/nexus/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4519 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/nexus/inputs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       36 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/nexus/outputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.280317 jarvis-tools-2024.4.10/jarvis/io/pennylane/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       61 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/pennylane/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2196 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/pennylane/inputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.344316 jarvis-tools-2024.4.10/jarvis/io/phonopy/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       43 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/phonopy/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4501 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/phonopy/fcmat2hr.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6844 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/phonopy/inputs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5696 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/phonopy/outputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.372316 jarvis-tools-2024.4.10/jarvis/io/prismatic/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       50 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/prismatic/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      674 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/prismatic/inputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.428316 jarvis-tools-2024.4.10/jarvis/io/qe/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       57 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/qe/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    15329 2024-03-31 13:46:58.000000 jarvis-tools-2024.4.10/jarvis/io/qe/inputs.py
+-rwxr-xr-x   0 knc6     (54782) 642div   (36677)    29549 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/qe/outputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.468316 jarvis-tools-2024.4.10/jarvis/io/qiskit/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       56 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/qiskit/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    12104 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/qiskit/inputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.508315 jarvis-tools-2024.4.10/jarvis/io/tequila/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       60 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/tequila/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2702 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/tequila/inputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.536315 jarvis-tools-2024.4.10/jarvis/io/vasp/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       56 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/vasp/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1522 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/vasp/default_potcars.json
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    20248 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/vasp/inputs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    82300 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/vasp/outputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.568315 jarvis-tools-2024.4.10/jarvis/io/wannier/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       61 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wannier/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4550 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wannier/default_semicore.json
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6929 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wannier/inputs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    34195 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wannier/outputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.620315 jarvis-tools-2024.4.10/jarvis/io/wanniertools/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       60 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wanniertools/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    10376 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wanniertools/inputs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3818 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wanniertools/outputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.656315 jarvis-tools-2024.4.10/jarvis/io/wien2k/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       55 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wien2k/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3238 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wien2k/inputs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3353 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wien2k/outputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.688314 jarvis-tools-2024.4.10/jarvis/io/zeopp/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/zeopp/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2184 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/zeopp/inputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.736314 jarvis-tools-2024.4.10/jarvis/tasks/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.748314 jarvis-tools-2024.4.10/jarvis/tasks/boltztrap/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       56 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/boltztrap/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      608 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/boltztrap/run.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.784314 jarvis-tools-2024.4.10/jarvis/tasks/lammps/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       55 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    14071 2024-03-31 15:50:24.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/lammps.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.956313 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3463 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/displace.mod
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6416 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelast.mod
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6449 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelast_min.mod
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6418 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelast_nobox.mod
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6415 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelastcomb.mod
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6389 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelastreax.mod
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2653 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/relax.mod
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      145 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/run0.mod
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      917 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/templates.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.964313 jarvis-tools-2024.4.10/jarvis/tasks/nexus/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       34 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/nexus/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3243 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/nexus/qmc.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.996313 jarvis-tools-2024.4.10/jarvis/tasks/phonopy/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       54 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/phonopy/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      765 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/phonopy/run.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.088312 jarvis-tools-2024.4.10/jarvis/tasks/qe/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       29 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/qe/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    19582 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/qe/converg.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3665 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/qe/master_super.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4209 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/qe/qe.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    10626 2024-04-14 12:24:55.000000 jarvis-tools-2024.4.10/jarvis/tasks/qe/super.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7387 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/qe/super_tetra.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5873 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/queue_jobs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.108312 jarvis-tools-2024.4.10/jarvis/tasks/vasp/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       61 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/vasp/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    66478 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/vasp/vasp.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.132312 jarvis-tools-2024.4.10/jarvis/tests/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.136312 jarvis-tools-2024.4.10/jarvis/tests/testfiles/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.160312 jarvis-tools-2024.4.10/jarvis/tests/testfiles/ai/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/ai/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      950 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/ai/test_ai_uncertainty.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    67390 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/ai/test_desc.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2206 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/ai/test_pkgs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.168312 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.172312 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/darkmatter/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/darkmatter/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      464 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/darkmatter/test_metrics.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.216311 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/defects/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/defects/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      444 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/defects/test_subs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3252 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/defects/test_surface.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1216 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/defects/test_vacancy.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.236311 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/elastic/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/elastic/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2577 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/elastic/test_tensor.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.264311 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/interface/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/interface/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     8683 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/interface/test_zur.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.296311 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/magnetism/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/magnetism/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      589 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/magnetism/test_magnetism.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.336311 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/phonon/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/phonon/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5121 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/phonon/test_dos.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      326 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/phonon/test_fc.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1279 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/phonon/test_ir.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.372310 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/solar/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/solar/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1399 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/solar/test_solar.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.380310 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/stm/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/stm/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1672 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/stm/test_stm.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.396310 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/structure/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/structure/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      390 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/structure/test_energetics.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1301 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/structure/test_neighbors.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3585 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/structure/test_spacegroup.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.408310 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/thermodynamics/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/thermodynamics/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1554 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/thermodynamics/test_energetics.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.428310 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/topological/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/topological/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      424 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/topological/test_spillage.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.612309 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5666 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/p.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6750 2024-04-14 12:36:23.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_atoms.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      262 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_circuits.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      481 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_composition.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2844 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_graph.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    11116 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_kpoints.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1507 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_latice.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      339 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_pdb.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      551 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_specie.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      541 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_utils.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.644309 jarvis-tools-2024.4.10/jarvis/tests/testfiles/db/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/db/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1496 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/db/test_figshare.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      154 2024-03-31 16:20:05.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/db/test_restapi.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.700308 jarvis-tools-2024.4.10/jarvis/tests/testfiles/tasks/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:33.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/tasks/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      804 2024-03-31 13:46:33.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/tasks/test_lammps.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      696 2024-03-31 13:46:33.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/tasks/test_vasp.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.728308 jarvis-tools-2024.4.10/jarvis_tools.egg-info/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3442 2024-04-14 14:32:17.000000 jarvis-tools-2024.4.10/jarvis_tools.egg-info/PKG-INFO
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7607 2024-04-14 14:32:17.000000 jarvis-tools-2024.4.10/jarvis_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        1 2024-04-14 14:32:17.000000 jarvis-tools-2024.4.10/jarvis_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      265 2024-04-14 14:32:17.000000 jarvis-tools-2024.4.10/jarvis_tools.egg-info/requires.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        7 2024-04-14 14:32:17.000000 jarvis-tools-2024.4.10/jarvis_tools.egg-info/top_level.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      195 2024-04-14 14:32:21.744308 jarvis-tools-2024.4.10/setup.cfg
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2649 2024-04-14 12:40:04.000000 jarvis-tools-2024.4.10/setup.py
```

### Comparing `jarvis-tools-2024.3.4/LICENSE.rst` & `jarvis-tools-2024.4.10/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/PKG-INFO` & `jarvis-tools-2024.4.10/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis-tools
-Version: 2024.3.4
+Version: 2024.4.10
 Summary: jarvis-tools: an open-source software package for data-driven atomistic materials design. https://jarvis.nist.gov/
 Home-page: https://github.com/usnistgov/jarvis
 Author: Kamal Choudhary
 Author-email: kamal.choudhary@nist.gov
 License: NIST
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Development Status :: 4 - Beta
@@ -18,16 +18,14 @@
 Requires-Dist: matplotlib>=3.0.0
 Requires-Dist: spglib>=1.14.1
 Requires-Dist: joblib>=0.14.1
 Requires-Dist: requests>=2.23.0
 Requires-Dist: toolz>=0.9.0
 Requires-Dist: xmltodict>=0.11.0
 Requires-Dist: tqdm>=4.41.1
-Requires-Dist: mkdocs-material>=9.0.5
-Requires-Dist: markdown>=3.2.1
 Provides-Extra: ai
 Requires-Dist: torch; extra == "ai"
 Requires-Dist: dgl; extra == "ai"
 Requires-Dist: keras; extra == "ai"
 Requires-Dist: tensorflow; extra == "ai"
 Requires-Dist: scikit-learn; extra == "ai"
 Requires-Dist: flask; extra == "ai"
```

### Comparing `jarvis-tools-2024.3.4/README.rst` & `jarvis-tools-2024.4.10/README.rst`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/ai/descriptors/cfid.py` & `jarvis-tools-2024.4.10/jarvis/ai/descriptors/cfid.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/ai/descriptors/coulomb.py` & `jarvis-tools-2024.4.10/jarvis/ai/descriptors/coulomb.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/ai/pkgs/lgbm/classification.py` & `jarvis-tools-2024.4.10/jarvis/ai/pkgs/lgbm/classification.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/ai/pkgs/lgbm/regression.py` & `jarvis-tools-2024.4.10/jarvis/ai/pkgs/lgbm/regression.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/ai/pkgs/sklearn/classification.py` & `jarvis-tools-2024.4.10/jarvis/ai/pkgs/sklearn/classification.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/ai/pkgs/sklearn/hyper_params.py` & `jarvis-tools-2024.4.10/jarvis/ai/pkgs/sklearn/hyper_params.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/ai/pkgs/sklearn/regression.py` & `jarvis-tools-2024.4.10/jarvis/ai/pkgs/sklearn/regression.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/ai/pkgs/utils.py` & `jarvis-tools-2024.4.10/jarvis/ai/pkgs/utils.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/ai/uncertainty/gaussian_process_uncertainty.py` & `jarvis-tools-2024.4.10/jarvis/ai/uncertainty/gaussian_process_uncertainty.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/ai/uncertainty/lgbm_quantile_uncertainty.py` & `jarvis-tools-2024.4.10/jarvis/ai/uncertainty/lgbm_quantile_uncertainty.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/darkmatter/metrics.py` & `jarvis-tools-2024.4.10/jarvis/analysis/darkmatter/metrics.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/defects/substitutions.py` & `jarvis-tools-2024.4.10/jarvis/analysis/defects/substitutions.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/defects/surface.py` & `jarvis-tools-2024.4.10/jarvis/analysis/defects/surface.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/defects/vacancy.py` & `jarvis-tools-2024.4.10/jarvis/analysis/defects/vacancy.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/diffraction/atomic_scattering_params.json` & `jarvis-tools-2024.4.10/jarvis/analysis/diffraction/atomic_scattering_params.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/diffraction/xrd.py` & `jarvis-tools-2024.4.10/jarvis/analysis/diffraction/xrd.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/elastic/tensor.py` & `jarvis-tools-2024.4.10/jarvis/analysis/elastic/tensor.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/interface/zur.py` & `jarvis-tools-2024.4.10/jarvis/analysis/interface/zur.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/magnetism/magmom_setup.py` & `jarvis-tools-2024.4.10/jarvis/analysis/magnetism/magmom_setup.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/periodic/ptable.py` & `jarvis-tools-2024.4.10/jarvis/analysis/periodic/ptable.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/phonon/dos.py` & `jarvis-tools-2024.4.10/jarvis/analysis/phonon/dos.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/phonon/force_constants.py` & `jarvis-tools-2024.4.10/jarvis/analysis/phonon/force_constants.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/phonon/ir.py` & `jarvis-tools-2024.4.10/jarvis/analysis/phonon/ir.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/solarefficiency/am1.5G.dat` & `jarvis-tools-2024.4.10/jarvis/analysis/solarefficiency/am1.5G.dat`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/solarefficiency/solar.py` & `jarvis-tools-2024.4.10/jarvis/analysis/solarefficiency/solar.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/stem/convolution_apprx.py` & `jarvis-tools-2024.4.10/jarvis/analysis/stem/convolution_apprx.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/stm/tersoff_hamann.py` & `jarvis-tools-2024.4.10/jarvis/analysis/stm/tersoff_hamann.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/structure/neighbors.py` & `jarvis-tools-2024.4.10/jarvis/analysis/structure/neighbors.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/structure/spacegroup.py` & `jarvis-tools-2024.4.10/jarvis/analysis/structure/spacegroup.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/thermodynamics/energetics.py` & `jarvis-tools-2024.4.10/jarvis/analysis/thermodynamics/energetics.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/thermodynamics/unary.json` & `jarvis-tools-2024.4.10/jarvis/analysis/thermodynamics/unary.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/thermodynamics/unary_qe_tb.json` & `jarvis-tools-2024.4.10/jarvis/analysis/thermodynamics/unary_qe_tb.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/analysis/topological/spillage.py` & `jarvis-tools-2024.4.10/jarvis/analysis/topological/spillage.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/core/Elements.json` & `jarvis-tools-2024.4.10/jarvis/core/Elements.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/core/atom_init.json` & `jarvis-tools-2024.4.10/jarvis/core/atom_init.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/core/atoms.py` & `jarvis-tools-2024.4.10/jarvis/core/atoms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module provides classes to specify atomic structure."""
+
 import numpy as np
 from jarvis.core.composition import Composition
 from jarvis.core.specie import Specie, atomic_numbers_to_symbols
 from jarvis.core.lattice import Lattice, lattice_coords_transformer
 from collections import OrderedDict
 from jarvis.core.utils import get_counts
 import itertools
@@ -14,14 +15,15 @@
 )
 import os
 import math
 import tempfile
 import random
 import string
 import datetime
+from collections import defaultdict
 
 amu_gm = 1.66054e-24
 ang_cm = 1e-8
 
 
 class Atoms(object):
     """
@@ -694,22 +696,31 @@
             props=d["props"],
             coords=d["coords"],
             cartesian=d["cartesian"],
         )
 
     def remove_site_by_index(self, site=0):
         """Remove an atom by its index number."""
+        return self.remove_sites_by_indices(indices=[site])
+
+    def remove_sites_by_indices(self, indices=[0], in_place=False):
+        """Remove multiple atoms by their corresponding indices number."""
         new_els = []
         new_coords = []
         new_props = []
         for ii, i in enumerate(self.frac_coords):
-            if ii != site:
+            if ii not in indices:
                 new_els.append(self.elements[ii])
                 new_coords.append(self.frac_coords[ii])
                 new_props.append(self.props[ii])
+        if in_place:
+            self.elements = new_els
+            self.coords = new_coords
+            self.props = new_props
+            return self
         return Atoms(
             lattice_mat=self.lattice_mat,
             elements=new_els,
             coords=np.array(new_coords),
             props=new_props,
             cartesian=False,
         )
@@ -1210,14 +1221,165 @@
         tvects = frac_points[
             np.all(frac_points < 1 - 1e-10, axis=1)
             & np.all(frac_points >= -1e-10, axis=1)
         ]
         assert len(tvects) == round(abs(np.linalg.det(supercell_matrix)))
         return tvects
 
+    def describe(
+        self,
+        xrd_peaks=5,
+        xrd_round=1,
+        cutoff=4,
+        take_n_bonds=2,
+        include_spg=True,
+    ):
+        """Describe for NLP applications."""
+        from jarvis.analysis.diffraction.xrd import XRD
+
+        if include_spg:
+            from jarvis.analysis.structure.spacegroup import Spacegroup3D
+
+            spg = Spacegroup3D(self)
+        theta, d_hkls, intens = XRD().simulate(atoms=self)
+        #     x = atoms.atomwise_angle_and_radial_distribution()
+        #     bond_distances = {}
+        #     for i, j in x[-1]["different_bond"].items():
+        #         bond_distances[i.replace("_", "-")] = ", ".join(
+        #             map(str, (sorted(list(set([round(jj, 2) for jj in j])))))
+        #         )
+        dists = defaultdict(list)
+        elements = self.elements
+        for i in self.get_all_neighbors(r=cutoff):
+            for j in i:
+                key = "-".join(sorted([elements[j[0]], elements[j[1]]]))
+                dists[key].append(j[2])
+        bond_distances = {}
+        for i, j in dists.items():
+            dist = sorted(set([round(k, 2) for k in j]))
+            if len(dist) >= take_n_bonds:
+                dist = dist[0:take_n_bonds]
+            bond_distances[i] = ", ".join(map(str, dist))
+        fracs = {}
+        for i, j in (self.composition.atomic_fraction).items():
+            fracs[i] = round(j, 3)
+        info = {}
+        chem_info = {
+            "atomic_formula": self.composition.reduced_formula,
+            "prototype": self.composition.prototype,
+            "molecular_weight": round(self.composition.weight / 2, 2),
+            "atomic_fraction": (fracs),
+            "atomic_X": ", ".join(
+                map(str, [Specie(s).X for s in self.uniq_species])
+            ),
+            "atomic_Z": ", ".join(
+                map(str, [Specie(s).Z for s in self.uniq_species])
+            ),
+        }
+        struct_info = {
+            "lattice_parameters": ", ".join(
+                map(str, [round(j, 2) for j in self.lattice.abc])
+            ),
+            "lattice_angles": ", ".join(
+                map(str, [round(j, 2) for j in self.lattice.angles])
+            ),
+            # "spg_number": spg.space_group_number,
+            # "spg_symbol": spg.space_group_symbol,
+            "top_k_xrd_peaks": ", ".join(
+                map(
+                    str,
+                    sorted(list(set([round(i, xrd_round) for i in theta])))[
+                        0:xrd_peaks
+                    ],
+                )
+            ),
+            "density": round(self.density, 3),
+            # "crystal_system": spg.crystal_system,
+            # "point_group": spg.point_group_symbol,
+            # "wyckoff": ", ".join(list(set(spg._dataset["wyckoffs"]))),
+            "bond_distances": bond_distances,
+        }
+        if include_spg:
+            struct_info["spg_number"] = spg.space_group_number
+            struct_info["spg_symbol"] = spg.space_group_symbol
+            struct_info["crystal_system"] = spg.crystal_system
+            struct_info["point_group"] = spg.point_group_symbol
+            struct_info["wyckoff"] = ", ".join(
+                list(set(spg._dataset["wyckoffs"]))
+            )
+            struct_info["natoms_primitive"] = spg.primitive_atoms.num_atoms
+            struct_info[
+                "natoms_conventional"
+            ] = spg.conventional_standard_structure.num_atoms
+        info["chemical_info"] = chem_info
+        info["structure_info"] = struct_info
+        line = "The number of atoms are: " + str(
+            self.num_atoms
+        )  # +"., The elements are: "+",".join(atoms.elements)+". "
+        for i, j in info.items():
+            if not isinstance(j, dict):
+                line += "The " + i + " is " + j + ". "
+            else:
+                # print("i",i)
+                # print("j",j)
+                for ii, jj in j.items():
+                    tmp = ""
+                    if isinstance(jj, dict):
+                        for iii, jjj in jj.items():
+                            tmp += iii + ": " + str(jjj) + " "
+                    else:
+                        tmp = jj
+                    line += "The " + ii + " is " + str(tmp) + ". "
+        line1 = line
+        # print('bond_distances', struct_info['bond_distances'])
+        tmp = ""
+        p = struct_info["bond_distances"]
+        for ii, (kk, vv) in enumerate(p.items()):
+            if ii == len(p) - 1:
+                punc = " Å."
+            else:
+                punc = " Å; "
+            tmp += kk + ": " + vv + punc
+        line2 = (
+            chem_info["atomic_formula"]
+            + " crystallizes in the "
+            + struct_info["crystal_system"]
+            + " "
+            + str(struct_info["spg_symbol"])
+            + " spacegroup, "
+            + struct_info["point_group"]
+            + " pointgroup with a prototype of "
+            + str(chem_info["prototype"])
+            # " and a molecular weight of " +
+            # str(chem_info['molecular_weight']) +
+            + ". The atomic fractions are: "
+            + str(chem_info["atomic_fraction"])
+            .replace("{", "")
+            .replace("}", "")
+            + " with electronegaticities as "
+            + str(chem_info["atomic_X"])
+            + " and atomic numbers as "
+            + str(chem_info["atomic_Z"])
+            + ". The bond distances are: "
+            + str(tmp)
+            + "The lattice lengths are: "
+            + struct_info["lattice_parameters"]
+            + " Å, and the lattice angles are: "
+            + struct_info["lattice_angles"]
+            + "º with some of the top XRD peaks at "
+            + struct_info["top_k_xrd_peaks"]
+            + "º with "
+            + "Wyckoff symbols "
+            + struct_info["wyckoff"]
+            + "."
+        )
+        info["desc_1"] = line1
+        info["desc_2"] = line2
+        return info
+
     def make_supercell_matrix(self, scaling_matrix):
         """
         Adapted from Pymatgen.
 
         Makes a supercell. Allowing to have sites outside the unit cell.
 
         Args:
@@ -1264,14 +1426,18 @@
         )
 
     def make_supercell(self, dim=[2, 2, 2]):
         """Make supercell of dimension dim."""
         dim = np.array(dim)
         if dim.shape == (3, 3):
             dim = np.array([int(np.linalg.norm(v)) for v in dim])
+        return self.make_supercell_matrix(dim)
+
+    def make_supercell_old(self, dim=[2, 2, 2]):
+        """Make supercell of dimension dim using for loop."""
         coords = self.frac_coords
         all_symbs = self.elements  # [i.symbol for i in s.species]
         nat = len(coords)
 
         new_nat = nat * dim[0] * dim[1] * dim[2]
         new_coords = np.zeros((new_nat, 3))
         new_symbs = []  # np.chararray((new_nat))
@@ -1427,14 +1593,25 @@
                 )
             else:
                 rest = rest + " ".join(map(str, i)) + "\n"
 
         result = header + middle + rest
         return result
 
+    def clone(self):
+        """Clones the class instance."""
+        return Atoms(
+            lattice_mat=self.lattice_mat,
+            elements=self.elements,
+            coords=self.frac_coords,
+            props=self.props,
+            cartesian=self.cartesian,
+            show_props=self.show_props,
+        )
+
 
 class VacuumPadding(object):
     """Adds vaccum padding to make 2D structure or making molecules."""
 
     def __init__(self, atoms, vacuum=20.0):
         """
         Initialize object.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jarvis-tools-2024.3.4/jarvis/core/circuits.py` & `jarvis-tools-2024.4.10/jarvis/core/circuits.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/core/composition.py` & `jarvis-tools-2024.4.10/jarvis/core/composition.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/core/element_charge.json` & `jarvis-tools-2024.4.10/jarvis/core/element_charge.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/core/graphs.py` & `jarvis-tools-2024.4.10/jarvis/core/graphs.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,16 @@
 
 
 def nearest_neighbor_edges(
     atoms=None,
     cutoff=8,
     max_neighbors=12,
     id=None,
-    use_canonize=False,
+    use_canonize=True,
+    # use_canonize=False,
 ):
     """Construct k-NN edge list."""
     # returns List[List[Tuple[site, distance, index, image]]]
     all_neighbors = atoms.get_all_neighbors(r=cutoff)
 
     # if a site has too few neighbors, increase the cutoff radius
     min_nbrs = min(len(neighborlist) for neighborlist in all_neighbors)
@@ -196,15 +197,16 @@
         neighbor_strategy="k-nearest",
         cutoff=8.0,
         max_neighbors=12,
         atom_features="cgcnn",
         max_attempts=3,
         id: Optional[str] = None,
         compute_line_graph: bool = True,
-        use_canonize: bool = False,
+        use_canonize: bool = True,
+        # use_canonize: bool = False,
     ):
         """Obtain a DGLGraph for Atoms object."""
         if neighbor_strategy == "k-nearest":
             edges = nearest_neighbor_edges(
                 atoms=atoms,
                 cutoff=cutoff,
                 max_neighbors=max_neighbors,
```

### Comparing `jarvis-tools-2024.3.4/jarvis/core/image.py` & `jarvis-tools-2024.4.10/jarvis/core/image.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/core/kpoints.py` & `jarvis-tools-2024.4.10/jarvis/core/kpoints.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/core/lattice.py` & `jarvis-tools-2024.4.10/jarvis/core/lattice.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/core/magpie.json` & `jarvis-tools-2024.4.10/jarvis/core/magpie.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/core/specie.py` & `jarvis-tools-2024.4.10/jarvis/core/specie.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/core/spectrum.py` & `jarvis-tools-2024.4.10/jarvis/core/spectrum.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/core/utils.py` & `jarvis-tools-2024.4.10/jarvis/core/utils.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/db/figshare.py` & `jarvis-tools-2024.4.10/jarvis/db/figshare.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/db/lammps_to_xml.py` & `jarvis-tools-2024.4.10/jarvis/db/lammps_to_xml.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/db/qe_to_xml.py` & `jarvis-tools-2024.4.10/jarvis/db/qe_to_xml.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/db/restapi.py` & `jarvis-tools-2024.4.10/jarvis/db/restapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,38 @@
 """Module to access or upload data in JARVIS-API."""
+
 import requests
 import pprint
 import os
 import glob
 from jarvis.db.jsonutils import dumpjson
 import string
 from collections import OrderedDict
 import json
 
 
+def jarvisdft_optimade(
+    prefix="https://jarvis.nist.gov/optimade/jarvisdft/v1/structures/?filter=",
+    query="elements HAS  ALL C,Si",
+):
+    url = prefix + query
+    vals = []
+    while True:
+        if url is not None:
+            # print('url', url)
+            response = requests.get(url)
+            data = response.json()["data"]
+            for i in data:
+                vals.append(i)
+            url = response.json()["links"]["next"]
+        else:
+            break
+    return vals
+
+
 class Api(object):
     """Class for handling functions for JARVIS-API."""
 
     def __init__(
         self,
         base_url="https://jarvis.nist.gov",
         user_info_file_path="/users/knc6/myinfo",
```

### Comparing `jarvis-tools-2024.3.4/jarvis/db/vasp_to_xml.py` & `jarvis-tools-2024.4.10/jarvis/db/vasp_to_xml.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/db/webpages.py` & `jarvis-tools-2024.4.10/jarvis/db/webpages.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/boltztrap/inputs.py` & `jarvis-tools-2024.4.10/jarvis/io/boltztrap/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/boltztrap/outputs.py` & `jarvis-tools-2024.4.10/jarvis/io/boltztrap/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/calphad/write_decorated_poscar.py` & `jarvis-tools-2024.4.10/jarvis/io/calphad/write_decorated_poscar.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/lammps/inputs.py` & `jarvis-tools-2024.4.10/jarvis/io/lammps/inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,18 +57,18 @@
         elements = atoms.elements
         # num_atoms = atoms.num_atoms
         a, b, c = atoms.lattice.abc
         xlo, ylo, zlo = origin
         xhi = a + xlo
         m = atoms.lattice._lat
         xy = np.dot(m[1], m[0] / a)
-        yhi = np.sqrt(b ** 2 - xy ** 2) + ylo
+        yhi = np.sqrt(b**2 - xy**2) + ylo
         xz = np.dot(m[2], m[0] / a)
         yz = (np.dot(m[1], m[2]) - xy * xz) / (yhi - ylo)
-        zhi = np.sqrt(c ** 2 - xz ** 2 - yz ** 2) + zlo
+        zhi = np.sqrt(c**2 - xz**2 - yz**2) + zlo
         rot_matrix = np.linalg.solve(
             [[xhi - xlo, 0, 0], [xy, yhi - ylo, 0], [xz, yz, zhi - zlo]], m
         )
         # box = np.array([[xlo, xhi], [ylo, yhi], [zlo, zhi], [xy, xz, yz]])
         box = np.array([xlo, xhi, ylo, yhi, zlo, zhi, xy, xz, yz])
         new_coords = (np.dot(rot_matrix, atoms.cart_coords.T)).T
         unique_elements = list(set(elements))
@@ -90,15 +90,15 @@
         )
 
     def read_data(
         self,
         filename="lammps.data",
         element_order=[],
         potential_file="pot.mod",
-        verbose=True,
+        verbose=False,
         has_charges=True,
     ):
         """Read Lammps data file."""
         # n_atoms = len(self._species)
         if element_order == []:
             # Reading potential file for element order
             if verbose:
@@ -175,15 +175,15 @@
                     typ[j] = symb[int(((lines[i + j + 2]).split()[1])) - 1]
                     if has_charges:
                         q[j] = float((lines[i + j + 2]).split()[2])
                     x[j] = float((lines[i + j + 2]).split()[it + 1])
                     y[j] = float((lines[i + j + 2]).split()[it + 2])
                     z[j] = float((lines[i + j + 2]).split()[it + 3])
                     coords.append([x[j], y[j], z[j]])
-                    print(coords[-1])
+                    # print(coords[-1])
         f.close()
         # print ("info",(typ),'coo',(coords),'latt',lat)
         typ_sp = [str(i, "utf-8") for i in typ]
         # print ('typ_sp',typ_sp)
         atoms = Atoms(
             lattice_mat=lat,
             elements=typ_sp,
```

### Comparing `jarvis-tools-2024.3.4/jarvis/io/lammps/outputs.py` & `jarvis-tools-2024.4.10/jarvis/io/lammps/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Function to analze LAMMPS output."""
+
 import numpy as np
 import glob
 import os
 from jarvis.analysis.elastic.tensor import ElasticTensor
 from jarvis.io.lammps.inputs import LammpsData
-from jarvis.io.phonopy.outputs import bandstructure_plot, total_dos
 from jarvis.core.atoms import Atoms
 
 
 def parse_potential_mod(mod="potential.mod"):
     """Parse potentials.mod input file."""
     info = {}
     f = open(mod, "r")
@@ -247,14 +247,16 @@
     path="bulk@mp-1487_fold", jid="x", atoms_to_dict=False
 ):
     """
     Parse individual LAMMPS material run.
 
     with optimization, vacancy, phonon, surface etc.
     """
+    from jarvis.io.phonopy.outputs import bandstructure_plot, total_dos
+
     cwd = os.getcwd()
     jid_file = os.path.join(path, "JARVISFF-ID")
     if os.path.exists(jid_file):
         f = open(jid_file, "r")
         lines = f.read().splitlines()
         f.close()
         jid = lines[0]
@@ -371,15 +373,17 @@
         info["band_distances"] = band_distances
         info["band_labels"] = band_labels
         info["band_label_points"] = band_label_points
     os.chdir(cwd)
     return info
 
 
-def parse_full_ff_folder(path="Mishin-Ni-Al-2009.eam.alloy_nist",):
+def parse_full_ff_folder(
+    path="Mishin-Ni-Al-2009.eam.alloy_nist",
+):
     """Parse complete FF calculation folder."""
     cwd = os.getcwd()
     os.chdir(path)
     print("path", path)
     tmp_path = path + "/*_fold"
     for i in glob.glob(tmp_path):
         print(i)
```

### Comparing `jarvis-tools-2024.3.4/jarvis/io/nexus/inputs.py` & `jarvis-tools-2024.4.10/jarvis/io/nexus/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/pennylane/inputs.py` & `jarvis-tools-2024.4.10/jarvis/io/pennylane/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/phonopy/fcmat2hr.py` & `jarvis-tools-2024.4.10/jarvis/io/phonopy/fcmat2hr.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/phonopy/inputs.py` & `jarvis-tools-2024.4.10/jarvis/io/phonopy/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/phonopy/outputs.py` & `jarvis-tools-2024.4.10/jarvis/io/phonopy/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/prismatic/inputs.py` & `jarvis-tools-2024.4.10/jarvis/io/prismatic/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/qe/inputs.py` & `jarvis-tools-2024.4.10/jarvis/io/qe/inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         if psp_dir is None:
             psp_dir = str(
                 os.path.join(os.path.dirname(__file__), psp_temp_name)
             )
             # Download GBRV PSPs by default
             if url is None:
                 url = (
-                    "http://www.physics.rutgers.edu/"
+                    "https://www.physics.rutgers.edu/"
                     "gbrv/all_pbesol_UPF_v1.5.tar.gz"
                 )
                 print("Please cite for PSPs:")
                 print("https://doi.org/10.1016/j.commatsci.2013.08.053")
             if not os.path.exists(psp_dir):
                 print("Downloading PSPs")
                 tar_file_name = str(
```

### Comparing `jarvis-tools-2024.3.4/jarvis/io/qe/outputs.py` & `jarvis-tools-2024.4.10/jarvis/io/qe/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/qiskit/inputs.py` & `jarvis-tools-2024.4.10/jarvis/io/qiskit/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/tequila/inputs.py` & `jarvis-tools-2024.4.10/jarvis/io/tequila/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/vasp/default_potcars.json` & `jarvis-tools-2024.4.10/jarvis/io/vasp/default_potcars.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/vasp/inputs.py` & `jarvis-tools-2024.4.10/jarvis/io/vasp/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/vasp/outputs.py` & `jarvis-tools-2024.4.10/jarvis/io/vasp/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/wannier/default_semicore.json` & `jarvis-tools-2024.4.10/jarvis/io/wannier/default_semicore.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/wannier/inputs.py` & `jarvis-tools-2024.4.10/jarvis/io/wannier/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/wannier/outputs.py` & `jarvis-tools-2024.4.10/jarvis/io/wannier/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/wanniertools/inputs.py` & `jarvis-tools-2024.4.10/jarvis/io/wanniertools/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/wanniertools/outputs.py` & `jarvis-tools-2024.4.10/jarvis/io/wanniertools/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/wien2k/inputs.py` & `jarvis-tools-2024.4.10/jarvis/io/wien2k/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/wien2k/outputs.py` & `jarvis-tools-2024.4.10/jarvis/io/wien2k/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/io/zeopp/inputs.py` & `jarvis-tools-2024.4.10/jarvis/io/zeopp/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/boltztrap/run.py` & `jarvis-tools-2024.4.10/jarvis/tasks/boltztrap/run.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/lammps/lammps.py` & `jarvis-tools-2024.4.10/jarvis/tasks/lammps/lammps.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,19 +138,23 @@
 
     # def phonon(self):
     #     pass
     def phonons(
         self, atoms=None, lammps_cmd="", enforce_c_size=15.0, parameters={}
     ):
         """Make Phonon calculation setup."""
-        from phonopy import Phonopy
-        from phonopy.file_IO import (
-            #    parse_FORCE_CONSTANTS,
-            write_FORCE_CONSTANTS,
-        )
+        try:
+            from phonopy import Phonopy
+            from phonopy.file_IO import (
+                #    parse_FORCE_CONSTANTS,
+                write_FORCE_CONSTANTS,
+            )
+        except Exception as exp:
+            print("Phonopy check", exp)
+            pass
 
         bulk = atoms.phonopy_converter()
 
         dim = get_supercell_dims(atoms, enforce_c_size=enforce_c_size)
         atoms = atoms.make_supercell([dim[0], dim[1], dim[2]])
 
         Poscar(atoms).write_file("POSCAR")
```

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/displace.mod` & `jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/displace.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/inelast.mod` & `jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelast.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/inelast_min.mod` & `jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelast_min.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/inelast_nobox.mod` & `jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelast_nobox.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/inelastcomb.mod` & `jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelastcomb.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/inelastreax.mod` & `jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelastreax.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/relax.mod` & `jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/relax.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/lammps/templates/templates.py` & `jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/templates.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/nexus/qmc.py` & `jarvis-tools-2024.4.10/jarvis/tasks/nexus/qmc.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/phonopy/run.py` & `jarvis-tools-2024.4.10/jarvis/tasks/phonopy/run.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/qe/converg.py` & `jarvis-tools-2024.4.10/jarvis/tasks/qe/converg.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/qe/master_super.py` & `jarvis-tools-2024.4.10/jarvis/tasks/qe/master_super.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/qe/qe.py` & `jarvis-tools-2024.4.10/jarvis/tasks/qe/qe.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/qe/super.py` & `jarvis-tools-2024.4.10/jarvis/tasks/qe/super.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,16 @@
             "control": {
                 "calculation": "'scf'",
                 "restart_mode": "'from_scratch'",
                 "prefix": "'QE'",
                 "outdir": "'./'",
                 "tstress": ".true.",
                 "tprnfor": ".true.",
-                "disk_io": "'nowf'",
+                "disk_io": "'low'",
+                # "disk_io": "'nowf'",
                 "pseudo_dir": None,
                 "verbosity": "'high'",
                 "nstep": 100,
                 "etot_conv_thr": "1.0d-5",
                 "forc_conv_thr": "1.0d-4",
             },
             "system": {
```

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/qe/super_tetra.py` & `jarvis-tools-2024.4.10/jarvis/tasks/qe/super_tetra.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/queue_jobs.py` & `jarvis-tools-2024.4.10/jarvis/tasks/queue_jobs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tasks/vasp/vasp.py` & `jarvis-tools-2024.4.10/jarvis/tasks/vasp/vasp.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/ai/test_ai_uncertainty.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/ai/test_ai_uncertainty.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/ai/test_desc.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/ai/test_desc.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/ai/test_pkgs.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/ai/test_pkgs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/defects/test_surface.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/defects/test_surface.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/defects/test_vacancy.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/defects/test_vacancy.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/elastic/test_tensor.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/elastic/test_tensor.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/interface/test_zur.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/interface/test_zur.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/magnetism/test_magnetism.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/magnetism/test_magnetism.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/phonon/test_dos.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/phonon/test_dos.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/phonon/test_ir.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/phonon/test_ir.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/solar/test_solar.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/solar/test_solar.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/stm/test_stm.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/stm/test_stm.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/structure/test_neighbors.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/structure/test_neighbors.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/structure/test_spacegroup.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/structure/test_spacegroup.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/analysis/thermodynamics/test_energetics.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/thermodynamics/test_energetics.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/p.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/p.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/test_atoms.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_atoms.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,20 +3,26 @@
     compare_atoms,
     VacuumPadding,
     get_supercell_dims,
     build_xanes_poscar,
     OptimadeAdaptor,
 )
 
-
+import numpy as np
 import os
 from jarvis.db.figshare import get_jid_data, data
 import tarfile
 import tempfile
 
+FIXTURES = {
+    "lattice_mat": [[2.715, 2.715, 0], [0, 2.715, 2.715], [2.715, 0, 2.715]],
+    "coords": [[0, 0, 0], [0.25, 0.2, 0.25]],
+    "elements": ["Si", "Si"],
+}
+
 new_file, filename = tempfile.mkstemp()
 
 
 example_fold_tgz = os.path.join(
     os.path.dirname(__file__),
     "..",
     "..",
@@ -51,19 +57,34 @@
     "examples",
     "vasp",
     "SiOptb88",
     "SiOptb88",
     "POSCAR",
 )
 
-cif_example = os.path.join(os.path.dirname(__file__), "1000052.cif",)
-cif_example2 = os.path.join(os.path.dirname(__file__), "Bacomp.cif",)
-cif_example3 = os.path.join(os.path.dirname(__file__), "mock.cif",)
-cif_example4 = os.path.join(os.path.dirname(__file__), "exp_000034.cif",)
-cif_example5 = os.path.join(os.path.dirname(__file__), "1000000.cif",)
+cif_example = os.path.join(
+    os.path.dirname(__file__),
+    "1000052.cif",
+)
+cif_example2 = os.path.join(
+    os.path.dirname(__file__),
+    "Bacomp.cif",
+)
+cif_example3 = os.path.join(
+    os.path.dirname(__file__),
+    "mock.cif",
+)
+cif_example4 = os.path.join(
+    os.path.dirname(__file__),
+    "exp_000034.cif",
+)
+cif_example5 = os.path.join(
+    os.path.dirname(__file__),
+    "1000000.cif",
+)
 
 
 def test_from_cif():
     a = Atoms.from_cif(cif_example)
     a = Atoms.from_cif(cif_example2)
     a = Atoms.from_cif(cif_example3)
     a = Atoms.from_cif(cif_example4)
@@ -72,18 +93,19 @@
     lines = f.read()
     f.close()
     x = Atoms.from_cif(from_string=lines)
 
 
 def test_basic_atoms():
 
-    box = [[2.715, 2.715, 0], [0, 2.715, 2.715], [2.715, 0, 2.715]]
-    coords = [[0, 0, 0], [0.25, 0.2, 0.25]]
-    elements = ["Si", "Si"]
-    Si = Atoms(lattice_mat=box, coords=coords, elements=elements)
+    Si = Atoms(
+        lattice_mat=FIXTURES["lattice_mat"],
+        coords=FIXTURES["coords"],
+        elements=FIXTURES["elements"],
+    )
     dim = get_supercell_dims(Si)
     build_xanes_poscar(atoms=Si, filename_with_prefix=True)
     assert dim == [3, 3, 3]
 
     opt = OptimadeAdaptor(Si)
     opt_info = opt.to_optimade()
     opt = OptimadeAdaptor()
@@ -92,29 +114,31 @@
     polar = Si.check_polar
     Si.props = ["a", "a"]
     vac_pad = VacuumPadding(Si)
     den_2d = round(vac_pad.get_effective_2d_slab().density, 2)
     den_0d = round(vac_pad.get_effective_molecule().density, 2)
     den_lll_red = round(Si.get_lll_reduced_structure().density, 2)
     strng = Si.get_string()
+    scell_nat_old = Si.make_supercell_old([2, 2, 2]).num_atoms
+    descr = Si.describe()
     scell_nat = Si.make_supercell([2, 2, 2]).num_atoms
     scell_nat2 = Si.make_supercell_matrix(
         [[2, 0, 0], [0, 2, 0], [0, 0, 2]]
     ).num_atoms
     # print("scell_nat,scell_nat2", scell_nat, scell_nat2)
     # print(Si.make_supercell([2, 2, 2]))
     # print()
     # print(Si.make_supercell_matrix([[2, 0, 0], [0, 2, 0], [0, 0, 2]]))
     com = round(Si.get_center_of_mass()[0], 3)
     rem = (Si.make_supercell([2, 2, 2]).remove_site_by_index(site=0)).num_atoms
     prim = Si.get_primitive_atoms
     print(prim.cart_coords)
     conv = Si.get_conventional_atoms
-    spgn=Si.get_spacegroup
-    comp=compare_atoms(atoms1=prim,atoms2=conv)
+    spgn = Si.get_spacegroup
+    comp = compare_atoms(atoms1=prim, atoms2=conv)
     assert round(prim.cart_coords[0][0], 2) == round(4.37815150, 2)
     # print ('raw_distance_matrix', prim.raw_distance_matrix)
     # print ('raw_distance_matrix', Si.raw_distance_matrix)
     # print ('distance_matrix', Si.pymatgen_converter().distance_matrix)
     assert round(prim.raw_distance_matrix[0][1], 2) == round(
         4.42386329832851, 2
     )
@@ -205,9 +229,41 @@
     m1.write_xyz(filename)
     m3 = Atoms.from_xyz(filename)
 
     cmd = "rm atoms.xyz POSCAR atoms.cif"
     os.system(cmd)
 
 
-# test_basic_atoms()
-# def test_basic_atoms():
+def test_clone():
+    Si = Atoms(
+        lattice_mat=FIXTURES["lattice_mat"],
+        coords=FIXTURES["coords"],
+        elements=FIXTURES["elements"],
+    )
+    Si2 = Si.clone()
+    np.testing.assert_array_equal(Si2.lattice_mat, Si.lattice_mat)
+    np.testing.assert_array_equal(Si2.coords, Si.coords)
+    assert Si2.props == Si.props
+    assert Si2.elements == Si.elements
+    assert Si2.cartesian == Si.cartesian
+    assert Si2.show_props == Si.show_props
+
+
+def test_remove_sites_by_indices():
+    Si = Atoms(
+        lattice_mat=FIXTURES["lattice_mat"],
+        coords=FIXTURES["coords"],
+        elements=FIXTURES["elements"],
+    )
+    Si_supercell = Si.make_supercell([2, 2, 2])
+    print("Si_supercell", Si_supercell)
+    Si2_supercell_without_two_atoms = Si_supercell.remove_sites_by_indices(
+        indices=[0, 1]
+    )
+    print(
+        "Si2_supercell_without_two_atoms.num_atoms",
+        Si2_supercell_without_two_atoms.num_atoms,
+    )
+    assert Si2_supercell_without_two_atoms.num_atoms == 14
+
+
+# test_remove_sites_by_indices()
```

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/test_graph.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_graph.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/test_kpoints.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_kpoints.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/test_latice.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_latice.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/test_specie.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_specie.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/core/test_utils.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/db/test_figshare.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/db/test_figshare.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/tasks/test_lammps.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/tasks/test_lammps.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis/tests/testfiles/tasks/test_vasp.py` & `jarvis-tools-2024.4.10/jarvis/tests/testfiles/tasks/test_vasp.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.3.4/jarvis_tools.egg-info/PKG-INFO` & `jarvis-tools-2024.4.10/jarvis_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis-tools
-Version: 2024.3.4
+Version: 2024.4.10
 Summary: jarvis-tools: an open-source software package for data-driven atomistic materials design. https://jarvis.nist.gov/
 Home-page: https://github.com/usnistgov/jarvis
 Author: Kamal Choudhary
 Author-email: kamal.choudhary@nist.gov
 License: NIST
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Development Status :: 4 - Beta
@@ -18,16 +18,14 @@
 Requires-Dist: matplotlib>=3.0.0
 Requires-Dist: spglib>=1.14.1
 Requires-Dist: joblib>=0.14.1
 Requires-Dist: requests>=2.23.0
 Requires-Dist: toolz>=0.9.0
 Requires-Dist: xmltodict>=0.11.0
 Requires-Dist: tqdm>=4.41.1
-Requires-Dist: mkdocs-material>=9.0.5
-Requires-Dist: markdown>=3.2.1
 Provides-Extra: ai
 Requires-Dist: torch; extra == "ai"
 Requires-Dist: dgl; extra == "ai"
 Requires-Dist: keras; extra == "ai"
 Requires-Dist: tensorflow; extra == "ai"
 Requires-Dist: scikit-learn; extra == "ai"
 Requires-Dist: flask; extra == "ai"
```

### Comparing `jarvis-tools-2024.3.4/jarvis_tools.egg-info/SOURCES.txt` & `jarvis-tools-2024.4.10/jarvis_tools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,15 @@
 jarvis/tests/testfiles/core/test_kpoints.py
 jarvis/tests/testfiles/core/test_latice.py
 jarvis/tests/testfiles/core/test_pdb.py
 jarvis/tests/testfiles/core/test_specie.py
 jarvis/tests/testfiles/core/test_utils.py
 jarvis/tests/testfiles/db/__init__.py
 jarvis/tests/testfiles/db/test_figshare.py
+jarvis/tests/testfiles/db/test_restapi.py
 jarvis/tests/testfiles/tasks/__init__.py
 jarvis/tests/testfiles/tasks/test_lammps.py
 jarvis/tests/testfiles/tasks/test_vasp.py
 jarvis_tools.egg-info/PKG-INFO
 jarvis_tools.egg-info/SOURCES.txt
 jarvis_tools.egg-info/dependency_links.txt
 jarvis_tools.egg-info/requires.txt
```

### Comparing `jarvis-tools-2024.3.4/setup.py` & `jarvis-tools-2024.4.10/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 base_dir = os.path.dirname(__file__)
 # with open(os.path.join(base_dir, "README.rst")) as f:
 with open(os.path.join(base_dir, "README.md")) as f:
     long_d = f.read()
 
 setup(
     name="jarvis-tools",
-    version="2024.3.4",
+    version="2024.4.10",
     long_description=long_d,
     install_requires=[
         "numpy>=1.20.1",
         "scipy>=1.5.0",
         "matplotlib>=3.0.0",
         "spglib>=1.14.1",
         "joblib>=0.14.1",
         "requests>=2.23.0",
         "toolz>=0.9.0",
         "xmltodict>=0.11.0",
         "tqdm>=4.41.1",
-        "mkdocs-material>=9.0.5",
-        "markdown>=3.2.1",
+        # "mkdocs-material>=9.0.5",
+        # "markdown>=3.2.1",
         # "absl-py==1.4.0",
     ],
     package_data={
         "jarvis.core": [
             "Elements.json",
             "magpie.json",
             "element_charge.json",
```

