# Comparing `tmp/keopscore-2.2.2.tar.gz` & `tmp/keopscore-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keopscore-2.2.2.tar", last modified: Fri Feb  9 16:48:55 2024, max compression
+gzip compressed data, was "keopscore-2.2.3.tar", last modified: Sun Apr 14 08:15:47 2024, max compression
```

## Comparing `keopscore-2.2.2.tar` & `keopscore-2.2.3.tar`

### file list

```diff
@@ -1,206 +1,206 @@
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.409673 keopscore-2.2.2/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)       37 2022-03-10 16:01:04.000000 keopscore-2.2.2/MANIFEST.in
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1726 2024-02-09 16:48:55.409673 keopscore-2.2.2/PKG-INFO
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.393006 keopscore-2.2.2/keopscore/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1282 2024-01-18 16:53:57.000000 keopscore-2.2.2/keopscore/__init__.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.393006 keopscore-2.2.2/keopscore/binders/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4532 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/binders/LinkCompile.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/binders/__init__.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.393006 keopscore-2.2.2/keopscore/binders/cpp/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      928 2023-02-22 10:18:06.000000 keopscore-2.2.2/keopscore/binders/cpp/Cpu_link_compile.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/binders/cpp/__init__.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.396339 keopscore-2.2.2/keopscore/binders/nvrtc/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4487 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/binders/nvrtc/Gpu_link_compile.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/binders/nvrtc/__init__.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    25661 2024-01-18 14:07:49.000000 keopscore-2.2.2/keopscore/binders/nvrtc/keops_nvrtc.cpp
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4698 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/binders/nvrtc/nvrtc_jit.cpp
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.396339 keopscore-2.2.2/keopscore/config/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/config/__init__.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1275 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/config/chunks.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    10420 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/config/config.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.396339 keopscore-2.2.2/keopscore/formulas/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1830 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/formulas/Chunkable_Op.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1804 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/GetReduction.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.396339 keopscore-2.2.2/keopscore/formulas/LinearOperators/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2935 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/LinearOperators/AdjointOperator.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2003 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/LinearOperators/LinearOperator.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     5643 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/LinearOperators/SumLinOperator.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4829 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/LinearOperators/TraceOperator.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      129 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/LinearOperators/__init__.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     9114 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/Operation.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1145 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/VectorizedComplexScalarOp.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2588 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/VectorizedScalarOp.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      179 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/__init__.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.396339 keopscore-2.2.2/keopscore/formulas/autodiff/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1257 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/autodiff/Diff.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      205 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/autodiff/Diff_WithSavedForward.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1279 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/autodiff/Divergence.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1049 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/autodiff/Grad.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      221 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/autodiff/Grad_WithSavedForward.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      793 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/autodiff/Laplacian.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      228 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/autodiff/__init__.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/checks.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.399673 keopscore-2.2.2/keopscore/formulas/complex/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      386 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/complex/ComplexAbs.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      981 2023-02-22 10:18:06.000000 keopscore-2.2.2/keopscore/formulas/complex/ComplexAdd.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      456 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/complex/ComplexAngle.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      620 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/complex/ComplexDivide.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1609 2023-02-22 10:18:06.000000 keopscore-2.2.2/keopscore/formulas/complex/ComplexExp.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1424 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/formulas/complex/ComplexExp1j.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1150 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/formulas/complex/ComplexImag.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1403 2023-02-22 10:18:06.000000 keopscore-2.2.2/keopscore/formulas/complex/ComplexMult.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1146 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/formulas/complex/ComplexReal.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1518 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/formulas/complex/ComplexRealScal.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1359 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/formulas/complex/ComplexSquareAbs.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1011 2023-02-22 10:18:06.000000 keopscore-2.2.2/keopscore/formulas/complex/ComplexSubtract.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1333 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/formulas/complex/ComplexSum.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1226 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/formulas/complex/ComplexSumT.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      607 2023-02-22 10:18:06.000000 keopscore-2.2.2/keopscore/formulas/complex/Conj.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1073 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/formulas/complex/Imag2Complex.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1073 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/formulas/complex/Real2Complex.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      645 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/complex/__init__.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.399673 keopscore-2.2.2/keopscore/formulas/factorization/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4758 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/factorization/Factorize.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)       48 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/factorization/__init__.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.406340 keopscore-2.2.2/keopscore/formulas/maths/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      369 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Abs.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      484 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Acos.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4719 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/Add.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2213 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/formulas/maths/ArgMax.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2212 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/formulas/maths/ArgMin.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      481 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Asin.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      330 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Atan.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      512 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Atan2.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4874 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/formulas/maths/BSpline.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      843 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Clamp.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1066 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/formulas/maths/ClampInt.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1324 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/Concat.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      344 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Cos.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1136 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/formulas/maths/DiffClampInt.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2134 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/Divide.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1389 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/Elem.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1837 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/ElemT.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      598 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/Equal.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      401 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Exp.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1750 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/Extract.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2147 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/ExtractT.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      367 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Floor.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1353 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/GradMatrix.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      532 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/IfElse.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      153 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/IntInv.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      532 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/Inv.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1082 2023-02-22 10:18:06.000000 keopscore-2.2.2/keopscore/formulas/maths/Kron.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      582 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/LessOrEqual.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      553 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/LessThan.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      418 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Log.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2270 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/MatVecMult.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2033 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/formulas/maths/Max.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2026 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/formulas/maths/Min.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1779 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/Minus.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1129 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Mod.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     6086 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/Mult.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      209 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Norm2.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      214 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Normalize.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      634 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/NotEqual.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1603 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/OneHot.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1283 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/Pow.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      566 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Powf.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      363 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/ReLU.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      911 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/formulas/maths/Round.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      768 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Rsqrt.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2092 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/Scalprod.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      446 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Sign.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      341 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Sin.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      455 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/SinXDivX.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     7088 2024-01-18 16:53:57.000000 keopscore-2.2.2/keopscore/formulas/maths/SoftDTW_SqDist.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      164 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/SqDist.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      143 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/SqNorm2.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      312 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/SqNormDiag.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      208 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/SqNormIso.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      622 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Sqrt.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      762 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Square.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      362 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/Step.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4517 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/Subtract.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1753 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/Sum.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1357 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/SumT.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      333 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/SymSqNorm.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     7326 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/TensorDot.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1529 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/TensorProd.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2111 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/maths/VecMatMult.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      258 2023-02-22 10:18:06.000000 keopscore-2.2.2/keopscore/formulas/maths/WeightedSqDist.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      706 2023-02-22 10:18:06.000000 keopscore-2.2.2/keopscore/formulas/maths/WeightedSqNorm.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      516 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/formulas/maths/XLogX.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2804 2024-01-18 15:47:38.000000 keopscore-2.2.2/keopscore/formulas/maths/__init__.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.406340 keopscore-2.2.2/keopscore/formulas/reductions/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1348 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/reductions/ArgKMin_Reduction.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      967 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/reductions/ArgMax_Reduction.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      967 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/reductions/ArgMin_Reduction.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4137 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/reductions/KMin_ArgKMin_Reduction.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1044 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/reductions/KMin_Reduction.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      673 2023-02-22 10:18:06.000000 keopscore-2.2.2/keopscore/formulas/reductions/Max_ArgMax_Reduction.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1895 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/reductions/Max_ArgMax_Reduction_Base.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1136 2023-02-22 10:18:06.000000 keopscore-2.2.2/keopscore/formulas/reductions/Max_Reduction.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     5540 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/reductions/Max_SumShiftExpWeight_Reduction.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      674 2023-02-22 10:18:06.000000 keopscore-2.2.2/keopscore/formulas/reductions/Min_ArgMin_Reduction.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1887 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/reductions/Min_ArgMin_Reduction_Base.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1128 2023-02-22 10:18:06.000000 keopscore-2.2.2/keopscore/formulas/reductions/Min_Reduction.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1879 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/reductions/Reduction.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1742 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/reductions/Sum_Reduction.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      705 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/reductions/Zero_Reduction.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      699 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/reductions/__init__.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2667 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/reductions/sum_schemes.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.406340 keopscore-2.2.2/keopscore/formulas/variables/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1116 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/variables/IntCst.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1146 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/variables/RatCst.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2924 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/variables/Var.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      832 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/variables/Zero.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)       98 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/formulas/variables/__init__.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     8801 2024-02-07 09:31:44.000000 keopscore-2.2.2/keopscore/get_keops_dll.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.406340 keopscore-2.2.2/keopscore/include/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     3227 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/include/CudaSizes.h
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     3227 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/include/Ranges.h
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    14175 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/include/Sizes.h
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        1 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/include/__init__.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     3521 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/include/ranges_utils.h
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4280 2023-12-22 13:10:10.000000 keopscore-2.2.2/keopscore/include/utils_pe.h
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        6 2024-02-07 09:49:43.000000 keopscore-2.2.2/keopscore/keops_version
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1184 2024-01-18 14:06:08.000000 keopscore-2.2.2/keopscore/licence.txt
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.406340 keopscore-2.2.2/keopscore/mapreduce/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     6013 2023-05-17 13:17:58.000000 keopscore-2.2.2/keopscore/mapreduce/Chunk_Mode_Constants.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2450 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/mapreduce/MapReduce.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)       93 2022-03-15 15:17:07.000000 keopscore-2.2.2/keopscore/mapreduce/__init__.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.409673 keopscore-2.2.2/keopscore/mapreduce/cpu/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     3248 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/mapreduce/cpu/CpuAssignZero.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     3707 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/mapreduce/cpu/CpuReduc.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    13753 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/mapreduce/cpu/CpuReduc_ranges.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      117 2022-03-15 15:17:07.000000 keopscore-2.2.2/keopscore/mapreduce/cpu/__init__.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.409673 keopscore-2.2.2/keopscore/mapreduce/gpu/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1257 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/mapreduce/gpu/GpuAssignZero.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4036 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/mapreduce/gpu/GpuReduc1D.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    10783 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/mapreduce/gpu/GpuReduc1D_chunks.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     8251 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/mapreduce/gpu/GpuReduc1D_finalchunks.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     8975 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/mapreduce/gpu/GpuReduc1D_ranges.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    18422 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/mapreduce/gpu/GpuReduc1D_ranges_chunks.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    13971 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/mapreduce/gpu/GpuReduc1D_ranges_finalchunks.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    11012 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/mapreduce/gpu/GpuReduc2D.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      413 2022-03-15 15:17:07.000000 keopscore-2.2.2/keopscore/mapreduce/gpu/__init__.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      748 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/readme.md
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.409673 keopscore-2.2.2/keopscore/utils/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     3679 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/utils/Cache.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2166 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/utils/TestFormula.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     5465 2023-02-22 10:18:06.000000 keopscore-2.2.2/keopscore/utils/TestOperation.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4517 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/utils/Tree.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 keopscore-2.2.2/keopscore/utils/__init__.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    30262 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/utils/code_gen_utils.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     8962 2023-12-22 10:13:41.000000 keopscore-2.2.2/keopscore/utils/gpu_utils.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     6075 2024-02-07 09:31:44.000000 keopscore-2.2.2/keopscore/utils/math_functions.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     3954 2024-02-07 09:31:44.000000 keopscore-2.2.2/keopscore/utils/misc_utils.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:55.409673 keopscore-2.2.2/keopscore.egg-info/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1726 2024-02-09 16:48:55.000000 keopscore-2.2.2/keopscore.egg-info/PKG-INFO
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     6895 2024-02-09 16:48:55.000000 keopscore-2.2.2/keopscore.egg-info/SOURCES.txt
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        1 2024-02-09 16:48:55.000000 keopscore-2.2.2/keopscore.egg-info/dependency_links.txt
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)       10 2024-02-09 16:48:55.000000 keopscore-2.2.2/keopscore.egg-info/top_level.txt
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1184 2024-01-18 14:06:08.000000 keopscore-2.2.2/licence.txt
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      748 2022-03-10 16:01:04.000000 keopscore-2.2.2/readme.md
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)       38 2024-02-09 16:48:55.409673 keopscore-2.2.2/setup.cfg
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2733 2023-12-22 10:13:41.000000 keopscore-2.2.2/setup.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.882838 keopscore-2.2.3/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)       37 2022-03-10 16:01:04.000000 keopscore-2.2.3/MANIFEST.in
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1728 2024-04-14 08:15:47.882838 keopscore-2.2.3/PKG-INFO
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.849504 keopscore-2.2.3/keopscore/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1300 2024-04-14 08:10:33.000000 keopscore-2.2.3/keopscore/__init__.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.849504 keopscore-2.2.3/keopscore/binders/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4532 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/binders/LinkCompile.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/binders/__init__.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.852837 keopscore-2.2.3/keopscore/binders/cpp/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      928 2023-02-22 10:18:06.000000 keopscore-2.2.3/keopscore/binders/cpp/Cpu_link_compile.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/binders/cpp/__init__.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.852837 keopscore-2.2.3/keopscore/binders/nvrtc/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4487 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/binders/nvrtc/Gpu_link_compile.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/binders/nvrtc/__init__.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    25661 2024-01-18 14:07:49.000000 keopscore-2.2.3/keopscore/binders/nvrtc/keops_nvrtc.cpp
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4698 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/binders/nvrtc/nvrtc_jit.cpp
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.852837 keopscore-2.2.3/keopscore/config/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/config/__init__.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1275 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/config/chunks.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    10869 2024-04-14 08:10:33.000000 keopscore-2.2.3/keopscore/config/config.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.852837 keopscore-2.2.3/keopscore/formulas/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1830 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/formulas/Chunkable_Op.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1861 2024-04-14 08:10:33.000000 keopscore-2.2.3/keopscore/formulas/GetReduction.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.856171 keopscore-2.2.3/keopscore/formulas/LinearOperators/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2935 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/LinearOperators/AdjointOperator.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2003 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/LinearOperators/LinearOperator.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     5643 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/LinearOperators/SumLinOperator.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4829 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/LinearOperators/TraceOperator.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      129 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/LinearOperators/__init__.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     9163 2024-04-14 08:10:33.000000 keopscore-2.2.3/keopscore/formulas/Operation.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1145 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/VectorizedComplexScalarOp.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2588 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/VectorizedScalarOp.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      179 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/__init__.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.856171 keopscore-2.2.3/keopscore/formulas/autodiff/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1257 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/autodiff/Diff.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      205 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/autodiff/Diff_WithSavedForward.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1279 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/autodiff/Divergence.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1049 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/autodiff/Grad.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      221 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/autodiff/Grad_WithSavedForward.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      793 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/autodiff/Laplacian.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      228 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/autodiff/__init__.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/checks.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.859504 keopscore-2.2.3/keopscore/formulas/complex/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      386 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/complex/ComplexAbs.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      981 2023-02-22 10:18:06.000000 keopscore-2.2.3/keopscore/formulas/complex/ComplexAdd.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      456 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/complex/ComplexAngle.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      620 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/complex/ComplexDivide.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1609 2023-02-22 10:18:06.000000 keopscore-2.2.3/keopscore/formulas/complex/ComplexExp.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1424 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/formulas/complex/ComplexExp1j.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1150 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/formulas/complex/ComplexImag.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1403 2023-02-22 10:18:06.000000 keopscore-2.2.3/keopscore/formulas/complex/ComplexMult.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1146 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/formulas/complex/ComplexReal.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1518 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/formulas/complex/ComplexRealScal.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1359 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/formulas/complex/ComplexSquareAbs.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1011 2023-02-22 10:18:06.000000 keopscore-2.2.3/keopscore/formulas/complex/ComplexSubtract.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1333 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/formulas/complex/ComplexSum.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1226 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/formulas/complex/ComplexSumT.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      607 2023-02-22 10:18:06.000000 keopscore-2.2.3/keopscore/formulas/complex/Conj.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1073 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/formulas/complex/Imag2Complex.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1073 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/formulas/complex/Real2Complex.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      645 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/complex/__init__.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.859504 keopscore-2.2.3/keopscore/formulas/factorization/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4845 2024-04-14 08:10:33.000000 keopscore-2.2.3/keopscore/formulas/factorization/Factorize.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)       48 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/factorization/__init__.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.876171 keopscore-2.2.3/keopscore/formulas/maths/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      369 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Abs.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      484 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Acos.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4719 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/Add.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2213 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/formulas/maths/ArgMax.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2212 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/formulas/maths/ArgMin.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      481 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Asin.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      330 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Atan.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      512 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Atan2.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4874 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/formulas/maths/BSpline.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      843 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Clamp.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1066 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/formulas/maths/ClampInt.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1324 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/Concat.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      344 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Cos.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1136 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/formulas/maths/DiffClampInt.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2134 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/Divide.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1389 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/Elem.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1837 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/ElemT.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      598 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/Equal.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      401 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Exp.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1750 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/Extract.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2147 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/ExtractT.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      367 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Floor.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1353 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/GradMatrix.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      532 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/IfElse.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      153 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/IntInv.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      532 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/Inv.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1082 2023-02-22 10:18:06.000000 keopscore-2.2.3/keopscore/formulas/maths/Kron.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      582 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/LessOrEqual.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      553 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/LessThan.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      418 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Log.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2270 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/MatVecMult.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2033 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/formulas/maths/Max.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2026 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/formulas/maths/Min.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1779 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/Minus.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1129 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Mod.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     6086 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/Mult.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      209 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Norm2.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      214 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Normalize.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      634 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/NotEqual.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1603 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/OneHot.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1283 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/Pow.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      566 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Powf.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      363 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/ReLU.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      911 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/formulas/maths/Round.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      768 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Rsqrt.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2092 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/Scalprod.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      446 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Sign.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      341 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Sin.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      455 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/SinXDivX.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     7088 2024-01-18 16:53:57.000000 keopscore-2.2.3/keopscore/formulas/maths/SoftDTW_SqDist.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      164 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/SqDist.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      143 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/SqNorm2.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      312 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/SqNormDiag.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      208 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/SqNormIso.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      622 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Sqrt.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      762 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Square.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      362 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/Step.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4517 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/Subtract.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1753 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/Sum.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1357 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/SumT.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      333 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/SymSqNorm.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     7326 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/TensorDot.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1580 2024-02-13 09:21:17.000000 keopscore-2.2.3/keopscore/formulas/maths/TensorProd.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2111 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/maths/VecMatMult.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      258 2023-02-22 10:18:06.000000 keopscore-2.2.3/keopscore/formulas/maths/WeightedSqDist.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      706 2023-02-22 10:18:06.000000 keopscore-2.2.3/keopscore/formulas/maths/WeightedSqNorm.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      516 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/formulas/maths/XLogX.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2804 2024-01-18 15:47:38.000000 keopscore-2.2.3/keopscore/formulas/maths/__init__.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.876171 keopscore-2.2.3/keopscore/formulas/reductions/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1348 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/reductions/ArgKMin_Reduction.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      967 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/reductions/ArgMax_Reduction.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      967 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/reductions/ArgMin_Reduction.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4137 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/reductions/KMin_ArgKMin_Reduction.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1044 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/reductions/KMin_Reduction.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      673 2023-02-22 10:18:06.000000 keopscore-2.2.3/keopscore/formulas/reductions/Max_ArgMax_Reduction.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1895 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/reductions/Max_ArgMax_Reduction_Base.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1136 2023-02-22 10:18:06.000000 keopscore-2.2.3/keopscore/formulas/reductions/Max_Reduction.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     5540 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/reductions/Max_SumShiftExpWeight_Reduction.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      674 2023-02-22 10:18:06.000000 keopscore-2.2.3/keopscore/formulas/reductions/Min_ArgMin_Reduction.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1887 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/reductions/Min_ArgMin_Reduction_Base.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1128 2023-02-22 10:18:06.000000 keopscore-2.2.3/keopscore/formulas/reductions/Min_Reduction.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1879 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/reductions/Reduction.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1742 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/reductions/Sum_Reduction.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      705 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/reductions/Zero_Reduction.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      699 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/reductions/__init__.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2667 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/reductions/sum_schemes.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.879505 keopscore-2.2.3/keopscore/formulas/variables/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1116 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/variables/IntCst.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1146 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/variables/RatCst.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2924 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/variables/Var.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      832 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/variables/Zero.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)       98 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/formulas/variables/__init__.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     8828 2024-04-14 08:10:33.000000 keopscore-2.2.3/keopscore/get_keops_dll.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.879505 keopscore-2.2.3/keopscore/include/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     3227 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/include/CudaSizes.h
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     3227 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/include/Ranges.h
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    14175 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/include/Sizes.h
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        1 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/include/__init__.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     3521 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/include/ranges_utils.h
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4280 2023-12-22 13:10:10.000000 keopscore-2.2.3/keopscore/include/utils_pe.h
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        6 2024-04-14 08:11:22.000000 keopscore-2.2.3/keopscore/keops_version
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1184 2024-01-18 14:06:08.000000 keopscore-2.2.3/keopscore/licence.txt
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.879505 keopscore-2.2.3/keopscore/mapreduce/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     6013 2023-05-17 13:17:58.000000 keopscore-2.2.3/keopscore/mapreduce/Chunk_Mode_Constants.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2450 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/mapreduce/MapReduce.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)       93 2022-03-15 15:17:07.000000 keopscore-2.2.3/keopscore/mapreduce/__init__.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.879505 keopscore-2.2.3/keopscore/mapreduce/cpu/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     3248 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/mapreduce/cpu/CpuAssignZero.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     3707 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/mapreduce/cpu/CpuReduc.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    13753 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/mapreduce/cpu/CpuReduc_ranges.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      117 2022-03-15 15:17:07.000000 keopscore-2.2.3/keopscore/mapreduce/cpu/__init__.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.882838 keopscore-2.2.3/keopscore/mapreduce/gpu/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1257 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/mapreduce/gpu/GpuAssignZero.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4036 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/mapreduce/gpu/GpuReduc1D.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    10783 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/mapreduce/gpu/GpuReduc1D_chunks.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     8251 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/mapreduce/gpu/GpuReduc1D_finalchunks.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     8975 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/mapreduce/gpu/GpuReduc1D_ranges.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    18422 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/mapreduce/gpu/GpuReduc1D_ranges_chunks.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    13971 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/mapreduce/gpu/GpuReduc1D_ranges_finalchunks.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    11012 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/mapreduce/gpu/GpuReduc2D.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      413 2022-03-15 15:17:07.000000 keopscore-2.2.3/keopscore/mapreduce/gpu/__init__.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      748 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/readme.md
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.882838 keopscore-2.2.3/keopscore/utils/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     3679 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/utils/Cache.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2259 2024-04-14 08:10:33.000000 keopscore-2.2.3/keopscore/utils/TestFormula.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     5594 2024-04-14 08:10:33.000000 keopscore-2.2.3/keopscore/utils/TestOperation.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4576 2024-04-14 08:10:33.000000 keopscore-2.2.3/keopscore/utils/Tree.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 keopscore-2.2.3/keopscore/utils/__init__.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    30262 2023-12-22 10:13:41.000000 keopscore-2.2.3/keopscore/utils/code_gen_utils.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     9087 2024-04-14 08:10:33.000000 keopscore-2.2.3/keopscore/utils/gpu_utils.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     6075 2024-02-07 09:31:44.000000 keopscore-2.2.3/keopscore/utils/math_functions.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4091 2024-04-14 08:10:33.000000 keopscore-2.2.3/keopscore/utils/misc_utils.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:47.882838 keopscore-2.2.3/keopscore.egg-info/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1728 2024-04-14 08:15:47.000000 keopscore-2.2.3/keopscore.egg-info/PKG-INFO
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     6895 2024-04-14 08:15:47.000000 keopscore-2.2.3/keopscore.egg-info/SOURCES.txt
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        1 2024-04-14 08:15:47.000000 keopscore-2.2.3/keopscore.egg-info/dependency_links.txt
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)       10 2024-04-14 08:15:47.000000 keopscore-2.2.3/keopscore.egg-info/top_level.txt
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1184 2024-01-18 14:06:08.000000 keopscore-2.2.3/licence.txt
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      748 2022-03-10 16:01:04.000000 keopscore-2.2.3/readme.md
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)       38 2024-04-14 08:15:47.882838 keopscore-2.2.3/setup.cfg
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2735 2024-04-14 08:10:33.000000 keopscore-2.2.3/setup.py
```

### Comparing `keopscore-2.2.2/PKG-INFO` & `keopscore-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keopscore
-Version: 2.2.2
+Version: 2.2.3
 Summary: keopscore is the KeOps meta programming engine. This python module should be used through a binder (e.g. pykeops or rkeops)
 Home-page: http://www.kernel-operations.io/
 Author: B. Charlier, J. Feydy, J. Glaunes
 Author-email: benjamin.charlier@umontpellier.fr, jean.feydy@gmail.com, alexis.glaunes@parisdescartes.fr
 Project-URL: Bug Reports, https://github.com/getkeops/keops/issues
 Project-URL: Source, https://github.com/getkeops/keops
 Keywords: kernels gpu autodiff
@@ -12,15 +12,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ![logo pykeops](http://www.kernel-operations.io/keops/_images/keops_logo.png)
 
 **keopscore** contains the [KeOps](https://www.kernel-operations.io/) meta programming engine. Given a formula, 
 it generates the c++/cuda code executed on the fly.
```

### Comparing `keopscore-2.2.2/keopscore/__init__.py` & `keopscore-2.2.3/keopscore/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,8 +32,8 @@
     keopscoreconfig.config.init_cudalibs()
     from keopscore.binders.nvrtc.Gpu_link_compile import Gpu_link_compile
     from keopscore.binders.nvrtc.Gpu_link_compile import jit_compile_dll
 
     if not os.path.exists(jit_compile_dll()):
         Gpu_link_compile.compile_jit_compile_dll()
 
-from keopscore.config.config import show_gpu_config
+from keopscore.config.config import show_gpu_config, show_cuda_status
```

### Comparing `keopscore-2.2.2/keopscore/binders/LinkCompile.py` & `keopscore-2.2.3/keopscore/binders/LinkCompile.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/binders/cpp/Cpu_link_compile.py` & `keopscore-2.2.3/keopscore/binders/cpp/Cpu_link_compile.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/binders/nvrtc/Gpu_link_compile.py` & `keopscore-2.2.3/keopscore/binders/nvrtc/Gpu_link_compile.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/binders/nvrtc/keops_nvrtc.cpp` & `keopscore-2.2.3/keopscore/binders/nvrtc/keops_nvrtc.cpp`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/binders/nvrtc/nvrtc_jit.cpp` & `keopscore-2.2.3/keopscore/binders/nvrtc/nvrtc_jit.cpp`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/config/chunks.py` & `keopscore-2.2.3/keopscore/config/chunks.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/config/config.py` & `keopscore-2.2.3/keopscore/config/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import os
 from os.path import join
 import shutil
 from ctypes import CDLL, RTLD_GLOBAL
 import keopscore
 from ctypes.util import find_library
-from keopscore.utils.misc_utils import KeOps_Warning, KeOps_Error
+from keopscore.utils.misc_utils import KeOps_Warning, KeOps_Error, KeOps_Print
 import platform, sys
 
 # global parameters can be set here :
 use_cuda = True  # use cuda if possible
 use_OpenMP = True  # use OpenMP if possible (see function set_OpenMP below)
 
 # System Path
 base_dir_path = os.path.abspath(join(os.path.dirname(os.path.realpath(__file__)), ".."))
 template_path = join(base_dir_path, "templates")
 bindings_source_dir = join(base_dir_path)
-keops_cache_folder = join(
-    os.path.expanduser("~"), ".cache", f"keops{keopscore.__version__}"
-)
+
+keops_cache_folder = os.getenv("KEOPS_CACHE_FOLDER")
+if keops_cache_folder is None:
+    keops_cache_folder = join(
+        os.path.expanduser("~"), ".cache", f"keops{keopscore.__version__}"
+    )
 default_build_folder_name = (
     "_".join(platform.uname()[:3]) + f"_p{sys.version.split(' ')[0]}"
 )
 # In case user has specified CUDA_VISIBLE_DEVICES environment variable,
 # it is better to set the build folder name accordingly.
 specific_gpus = os.getenv("CUDA_VISIBLE_DEVICES")
 if specific_gpus:
@@ -226,35 +229,40 @@
         try:
             CDLL(libname)
             return True
         except OSError:
             return False
 
 
-cuda_dependencies = ["cuda", "nvrtc"]
-if all([find_and_try_library(lib) for lib in cuda_dependencies]):
-    # N.B. calling get_gpu_props issues a warning if cuda is not available, so we do not add another warning here
-    from keopscore.utils.gpu_utils import (
-        get_gpu_props,
-    )  # N.B. this import should be kept inside the if statement
-
-    cuda_available = get_gpu_props()[0] > 0
+if use_cuda:
+    cuda_dependencies = ["cuda", "nvrtc"]
+    if all([find_and_try_library(lib) for lib in cuda_dependencies]):
+        # N.B. calling get_gpu_props issues a warning if cuda is not available, so we do not add another warning here
+        from keopscore.utils.gpu_utils import (
+            get_gpu_props,
+        )  # N.B. this import should be kept inside the if statement
+
+        cuda_available = get_gpu_props()[0] > 0
+        if not cuda_available:
+            cuda_message = "Cuda libraries were detected on the system, but something is wrong with the GPU configuration ; using cpu only mode"
+            use_cuda = False
+        else:
+            cuda_message = "Cuda configuration is OK"
+    else:
+        cuda_available = False
+        cuda_message = "Cuda libraries were not detected on the system or could not be loaded ; using cpu only mode"
+        KeOps_Warning(cuda_message)
+        use_cuda = False
 else:
-    cuda_available = False
-    KeOps_Warning(
-        "Cuda libraries were not detected on the system or could not be loaded ; using cpu only mode"
-    )
+    cuda_message = "Cuda is disabled (use_cuda is set to False in the file config.py)"
 
-if not use_cuda and cuda_available:
-    KeOps_Warning(
-        "Cuda appears to be available on your system, but use_cuda is set to False in config.py. Using cpu only mode"
-    )
 
-if use_cuda and not cuda_available:
-    use_cuda = False
+def show_cuda_status(force_print=False):
+    KeOps_Print(cuda_message, force_print=force_print)
+
 
 if use_cuda:
     from keopscore.utils.gpu_utils import (
         libcuda_folder,
         libnvrtc_folder,
         get_cuda_include_path,
         get_cuda_version,
@@ -304,10 +312,10 @@
             "nvrtc_flags",
             "nvrtc_include",
             "cuda_include_path",
             "jit_source_file",
             "jit_source_header",
             "jit_binary",
         ):
-            print(elem + " : ", eval(elem))
+            KeOps_Print(elem + " : ", eval(elem))
     else:
-        print("gpu disabled")
+        KeOps_Print("gpu disabled")
```

### Comparing `keopscore-2.2.2/keopscore/formulas/Chunkable_Op.py` & `keopscore-2.2.3/keopscore/formulas/Chunkable_Op.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/GetReduction.py` & `keopscore-2.2.3/keopscore/formulas/GetReduction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import ast, inspect
 
 import keopscore
 import keopscore.formulas
+from keopscore.utils.misc_utils import KeOps_Print
 from keopscore.utils.code_gen_utils import get_hash_name
 from keopscore.formulas.reductions import *
 from keopscore.formulas.maths import *
 from keopscore.formulas.complex import *
 from keopscore.formulas.variables import *
 from keopscore.formulas.autodiff import *
 from keopscore.formulas.LinearOperators import *
@@ -41,9 +42,9 @@
     def check_formula(string):
         formula_class = dict(inspect.getmembers(keopscore.formulas))
         parsed = ast.parse(string)
         for node in ast.walk(parsed):
             if isinstance(node, ast.Call) and (
                 node.func.id not in formula_class.keys()
             ):
-                print(node.func.id)
+                KeOps_Print(node.func.id)
                 # raise NotImplementedError
```

### Comparing `keopscore-2.2.2/keopscore/formulas/LinearOperators/AdjointOperator.py` & `keopscore-2.2.3/keopscore/formulas/LinearOperators/AdjointOperator.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/LinearOperators/LinearOperator.py` & `keopscore-2.2.3/keopscore/formulas/LinearOperators/LinearOperator.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/LinearOperators/SumLinOperator.py` & `keopscore-2.2.3/keopscore/formulas/LinearOperators/SumLinOperator.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/LinearOperators/TraceOperator.py` & `keopscore-2.2.3/keopscore/formulas/LinearOperators/TraceOperator.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/Operation.py` & `keopscore-2.2.3/keopscore/formulas/Operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from keopscore.utils.code_gen_utils import new_c_varname, c_array
 from keopscore.utils.Tree import Tree
 import keopscore
-from keopscore.utils.misc_utils import KeOps_Error
+from keopscore.utils.misc_utils import KeOps_Error, KeOps_Print
 
 ###################
 ## Base class
 ###################
 
 
 class Operation(Tree):
@@ -68,20 +68,20 @@
          - out is a c_variable in which the result of the evaluation is stored
          - table is the list of c_variables corresponding to actual local variables
         required for evaluation : each Var(ind,*,*) corresponds to table[ind]"""
         from keopscore.formulas.variables.Var import Var
 
         string = f"\n{{\n// Starting code block for {self.__repr__()}.\n\n"
         if keopscore.debug_ops:
-            print(f"Building code block for {self.__repr__()}")
-            print("out=", out)
-            print("dim of out : ", out.dim)
-            print("table=", table)
+            KeOps_Print(f"Building code block for {self.__repr__()}")
+            KeOps_Print("out=", out)
+            KeOps_Print("dim of out : ", out.dim)
+            KeOps_Print("table=", table)
             for v in table:
-                print(f"dim of {v} : ", v.dim)
+                KeOps_Print(f"dim of {v} : ", v.dim)
         if keopscore.debug_ops_at_exec:
             string += f'printf("\\n\\nComputing {self.__repr__()} :\\n");\n'
         args = []
         # Evaluation of the child operations
         for child in self.children:
             if isinstance(child, Var):
                 # if the child of the operation is a Var, we do not need to evaluate it,
@@ -106,15 +106,15 @@
         # some debugging helper :
         if keopscore.debug_ops_at_exec:
             for arg in args:
                 string += arg.c_print
             string += out.c_print
             string += f'printf("\\n\\n");\n'
         if keopscore.debug_ops:
-            print(f"Finished building code block for {self.__repr__()}")
+            KeOps_Print(f"Finished building code block for {self.__repr__()}")
 
         string += f"\n\n// Finished code block for {self.__repr__()}.\n}}\n\n"
         return string
 
     def __mul__(self, other):
         """f*g redirects to Mult(f,g)"""
         from keopscore.formulas.maths.Mult import Mult
```

### Comparing `keopscore-2.2.2/keopscore/formulas/VectorizedComplexScalarOp.py` & `keopscore-2.2.3/keopscore/formulas/VectorizedComplexScalarOp.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/VectorizedScalarOp.py` & `keopscore-2.2.3/keopscore/formulas/VectorizedScalarOp.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/autodiff/Diff.py` & `keopscore-2.2.3/keopscore/formulas/autodiff/Diff.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/autodiff/Divergence.py` & `keopscore-2.2.3/keopscore/formulas/autodiff/Divergence.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/autodiff/Grad.py` & `keopscore-2.2.3/keopscore/formulas/autodiff/Grad.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/autodiff/Laplacian.py` & `keopscore-2.2.3/keopscore/formulas/autodiff/Laplacian.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/complex/ComplexAdd.py` & `keopscore-2.2.3/keopscore/formulas/complex/ComplexAdd.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/complex/ComplexDivide.py` & `keopscore-2.2.3/keopscore/formulas/complex/ComplexDivide.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/complex/ComplexExp.py` & `keopscore-2.2.3/keopscore/formulas/complex/ComplexExp.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/complex/ComplexExp1j.py` & `keopscore-2.2.3/keopscore/formulas/complex/ComplexExp1j.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/complex/ComplexImag.py` & `keopscore-2.2.3/keopscore/formulas/complex/ComplexImag.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/complex/ComplexMult.py` & `keopscore-2.2.3/keopscore/formulas/complex/ComplexMult.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/complex/ComplexReal.py` & `keopscore-2.2.3/keopscore/formulas/complex/ComplexReal.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/complex/ComplexRealScal.py` & `keopscore-2.2.3/keopscore/formulas/complex/ComplexRealScal.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/complex/ComplexSquareAbs.py` & `keopscore-2.2.3/keopscore/formulas/complex/ComplexSquareAbs.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/complex/ComplexSubtract.py` & `keopscore-2.2.3/keopscore/formulas/complex/ComplexSubtract.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/complex/ComplexSum.py` & `keopscore-2.2.3/keopscore/formulas/complex/ComplexSum.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/complex/ComplexSumT.py` & `keopscore-2.2.3/keopscore/formulas/complex/ComplexSumT.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/complex/Conj.py` & `keopscore-2.2.3/keopscore/formulas/complex/Conj.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/complex/Imag2Complex.py` & `keopscore-2.2.3/keopscore/formulas/complex/Imag2Complex.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/complex/Real2Complex.py` & `keopscore-2.2.3/keopscore/formulas/complex/Real2Complex.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/complex/__init__.py` & `keopscore-2.2.3/keopscore/formulas/complex/__init__.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/factorization/Factorize.py` & `keopscore-2.2.3/keopscore/formulas/factorization/Factorize.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from keopscore.formulas.variables import Var, Zero
 from keopscore.formulas.variables.IntCst import IntCst_Impl
 from keopscore.utils.code_gen_utils import new_c_varname, c_array
 from keopscore.formulas.Operation import Operation
 import keopscore
 from keopscore.utils.code_gen_utils import GetInds
+from keopscore.utils.misc_utils import KeOps_Print
 
 
 class Factorize_Impl(Operation):
     string_id = "Factorize"
 
     def recursive_str(self):
         f, g = self.children
@@ -28,20 +29,20 @@
          - out is a c_variable in which the result of the evaluation is stored
          - table is the list of c_variables corresponding to actual local variables
         required for evaluation : each Var(ind,*,*) corresponds to table[ind]"""
         from keopscore.formulas.variables.Var import Var
 
         string = f"\n{{\n// Starting code block for {self.__repr__()}.\n\n"
         if keopscore.debug_ops:
-            print(f"Building code block for {self.__repr__()}")
-            print("out=", out)
-            print("dim of out : ", out.dim)
-            print("table=", table)
+            KeOps_Print(f"Building code block for {self.__repr__()}")
+            KeOps_Print("out=", out)
+            KeOps_Print("dim of out : ", out.dim)
+            KeOps_Print("table=", table)
             for v in table:
-                print(f"dim of {v} : ", v.dim)
+                KeOps_Print(f"dim of {v} : ", v.dim)
         if keopscore.debug_ops_at_exec:
             string += f'printf("\\n\\nComputing {self.__repr__()} :\\n");\n'
 
         f, g = self.children
         (aliasvar,) = self.params
 
         # Evaluation of g
@@ -64,15 +65,15 @@
         newaliasvar = Var(newind, aliasvar.dim, aliasvar.cat)
         newf = f.replace(aliasvar, newaliasvar)
 
         # Evaluation of f
         string += newf(out, table)
 
         if keopscore.debug_ops:
-            print(f"Finished building code block for {self.__repr__()}")
+            KeOps_Print(f"Finished building code block for {self.__repr__()}")
 
         string += f"\n\n// Finished code block for {self.__repr__()}.\n}}\n\n"
         return string
 
     def DiffT(self, v, gradin):
         f, g = self.children
         (aliasvar,) = self.params
```

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Add.py` & `keopscore-2.2.3/keopscore/formulas/maths/Add.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/ArgMax.py` & `keopscore-2.2.3/keopscore/formulas/maths/ArgMax.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/ArgMin.py` & `keopscore-2.2.3/keopscore/formulas/maths/ArgMin.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Atan2.py` & `keopscore-2.2.3/keopscore/formulas/maths/Atan2.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/BSpline.py` & `keopscore-2.2.3/keopscore/formulas/maths/BSpline.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Clamp.py` & `keopscore-2.2.3/keopscore/formulas/maths/Clamp.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/ClampInt.py` & `keopscore-2.2.3/keopscore/formulas/maths/ClampInt.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Concat.py` & `keopscore-2.2.3/keopscore/formulas/maths/Concat.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/DiffClampInt.py` & `keopscore-2.2.3/keopscore/formulas/maths/DiffClampInt.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Divide.py` & `keopscore-2.2.3/keopscore/formulas/maths/Divide.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Elem.py` & `keopscore-2.2.3/keopscore/formulas/maths/Elem.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/ElemT.py` & `keopscore-2.2.3/keopscore/formulas/maths/ElemT.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Equal.py` & `keopscore-2.2.3/keopscore/formulas/maths/Equal.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Extract.py` & `keopscore-2.2.3/keopscore/formulas/maths/Extract.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/ExtractT.py` & `keopscore-2.2.3/keopscore/formulas/maths/ExtractT.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/GradMatrix.py` & `keopscore-2.2.3/keopscore/formulas/maths/GradMatrix.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/IfElse.py` & `keopscore-2.2.3/keopscore/formulas/maths/IfElse.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Inv.py` & `keopscore-2.2.3/keopscore/formulas/maths/Inv.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Kron.py` & `keopscore-2.2.3/keopscore/formulas/maths/Kron.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/LessOrEqual.py` & `keopscore-2.2.3/keopscore/formulas/maths/LessOrEqual.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/LessThan.py` & `keopscore-2.2.3/keopscore/formulas/maths/LessThan.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/MatVecMult.py` & `keopscore-2.2.3/keopscore/formulas/maths/MatVecMult.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Max.py` & `keopscore-2.2.3/keopscore/formulas/maths/Max.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Min.py` & `keopscore-2.2.3/keopscore/formulas/maths/Min.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Minus.py` & `keopscore-2.2.3/keopscore/formulas/maths/Minus.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Mod.py` & `keopscore-2.2.3/keopscore/formulas/maths/Mod.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Mult.py` & `keopscore-2.2.3/keopscore/formulas/maths/Mult.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/NotEqual.py` & `keopscore-2.2.3/keopscore/formulas/maths/NotEqual.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/OneHot.py` & `keopscore-2.2.3/keopscore/formulas/maths/OneHot.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Pow.py` & `keopscore-2.2.3/keopscore/formulas/maths/Pow.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Powf.py` & `keopscore-2.2.3/keopscore/formulas/maths/Powf.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Round.py` & `keopscore-2.2.3/keopscore/formulas/maths/Round.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Rsqrt.py` & `keopscore-2.2.3/keopscore/formulas/maths/Rsqrt.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Scalprod.py` & `keopscore-2.2.3/keopscore/formulas/maths/Scalprod.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/SoftDTW_SqDist.py` & `keopscore-2.2.3/keopscore/formulas/maths/SoftDTW_SqDist.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Sqrt.py` & `keopscore-2.2.3/keopscore/formulas/maths/Sqrt.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Square.py` & `keopscore-2.2.3/keopscore/formulas/maths/Square.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Subtract.py` & `keopscore-2.2.3/keopscore/formulas/maths/Subtract.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/Sum.py` & `keopscore-2.2.3/keopscore/formulas/maths/Sum.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/SumT.py` & `keopscore-2.2.3/keopscore/formulas/maths/SumT.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/TensorDot.py` & `keopscore-2.2.3/keopscore/formulas/maths/TensorDot.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/TensorProd.py` & `keopscore-2.2.3/keopscore/formulas/maths/TensorProd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from keopscore.formulas.Operation import Operation
 from keopscore.utils.code_gen_utils import (
     c_variable,
     c_for_loop,
 )
+from keopscore.utils.misc_utils import KeOps_Error
 
 
 ####################################
 ######    Tensor product       #####
 ####################################
```

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/VecMatMult.py` & `keopscore-2.2.3/keopscore/formulas/maths/VecMatMult.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/WeightedSqNorm.py` & `keopscore-2.2.3/keopscore/formulas/maths/WeightedSqNorm.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/XLogX.py` & `keopscore-2.2.3/keopscore/formulas/maths/XLogX.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/maths/__init__.py` & `keopscore-2.2.3/keopscore/formulas/maths/__init__.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/reductions/ArgKMin_Reduction.py` & `keopscore-2.2.3/keopscore/formulas/reductions/ArgKMin_Reduction.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/reductions/ArgMax_Reduction.py` & `keopscore-2.2.3/keopscore/formulas/reductions/ArgMax_Reduction.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/reductions/ArgMin_Reduction.py` & `keopscore-2.2.3/keopscore/formulas/reductions/ArgMin_Reduction.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/reductions/KMin_ArgKMin_Reduction.py` & `keopscore-2.2.3/keopscore/formulas/reductions/KMin_ArgKMin_Reduction.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/reductions/KMin_Reduction.py` & `keopscore-2.2.3/keopscore/formulas/reductions/KMin_Reduction.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/reductions/Max_ArgMax_Reduction.py` & `keopscore-2.2.3/keopscore/formulas/reductions/Max_ArgMax_Reduction.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/reductions/Max_ArgMax_Reduction_Base.py` & `keopscore-2.2.3/keopscore/formulas/reductions/Max_ArgMax_Reduction_Base.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/reductions/Max_Reduction.py` & `keopscore-2.2.3/keopscore/formulas/reductions/Max_Reduction.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/reductions/Max_SumShiftExpWeight_Reduction.py` & `keopscore-2.2.3/keopscore/formulas/reductions/Max_SumShiftExpWeight_Reduction.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/reductions/Min_ArgMin_Reduction.py` & `keopscore-2.2.3/keopscore/formulas/reductions/Min_ArgMin_Reduction.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/reductions/Min_ArgMin_Reduction_Base.py` & `keopscore-2.2.3/keopscore/formulas/reductions/Min_ArgMin_Reduction_Base.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/reductions/Min_Reduction.py` & `keopscore-2.2.3/keopscore/formulas/reductions/Min_Reduction.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/reductions/Reduction.py` & `keopscore-2.2.3/keopscore/formulas/reductions/Reduction.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/reductions/Sum_Reduction.py` & `keopscore-2.2.3/keopscore/formulas/reductions/Sum_Reduction.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/reductions/Zero_Reduction.py` & `keopscore-2.2.3/keopscore/formulas/reductions/Zero_Reduction.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/reductions/__init__.py` & `keopscore-2.2.3/keopscore/formulas/reductions/__init__.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/reductions/sum_schemes.py` & `keopscore-2.2.3/keopscore/formulas/reductions/sum_schemes.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/variables/IntCst.py` & `keopscore-2.2.3/keopscore/formulas/variables/IntCst.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/variables/RatCst.py` & `keopscore-2.2.3/keopscore/formulas/variables/RatCst.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/variables/Var.py` & `keopscore-2.2.3/keopscore/formulas/variables/Var.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/formulas/variables/Zero.py` & `keopscore-2.2.3/keopscore/formulas/variables/Zero.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/get_keops_dll.py` & `keopscore-2.2.3/keopscore/get_keops_dll.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     use_final_chunks,
     set_mult_var_highdim,
 )
 from keopscore.formulas import Zero_Reduction, Sum_Reduction
 from keopscore.formulas.GetReduction import GetReduction
 from keopscore.formulas.variables.Zero import Zero
 from keopscore.utils.Cache import Cache
-from keopscore.utils.code_gen_utils import KeOps_Error
+from keopscore.utils.misc_utils import KeOps_Error, KeOps_Print
 
 # Get every classes in mapreduce
 map_reduce = dict(inspect.getmembers(keopscore.mapreduce, inspect.isclass))
 
 
 def get_keops_dll_impl(
     map_reduce_id,
@@ -112,16 +112,16 @@
     map_reduce_class = map_reduce[map_reduce_id]
 
     map_reduce_obj = map_reduce_class(red_formula_string, aliases, *args)
 
     rf = map_reduce_obj.red_formula
 
     if keopscore.debug_ops:
-        print("In get_keops_dll, formula is :", rf)
-        print("formula.__repr__() is : ", rf.__repr__())
+        KeOps_Print("In get_keops_dll, formula is :", rf)
+        KeOps_Print("formula.__repr__() is : ", rf.__repr__())
         rf.make_dot()
 
     # detecting the case of formula being equal to zero, to bypass reduction.
     rf = map_reduce_obj.red_formula
     if isinstance(rf, Zero_Reduction) or (
         isinstance(rf.formula, Zero) and isinstance(rf, Sum_Reduction)
     ):
@@ -200,8 +200,8 @@
             KeOps_Error(
                 f"Invalid call to Python script {sys.argv[0]}. Argument number {k + 1} ({key}) should be of type {argtype} but is of type {type(argval)}"
             )
         argdict[key] = argval
 
     res = get_keops_dll(argdict["map_reduce_id"], *list(argdict.values())[1:])
     for item in res:
-        print(item)
+        KeOps_Print(item)
```

### Comparing `keopscore-2.2.2/keopscore/include/CudaSizes.h` & `keopscore-2.2.3/keopscore/include/CudaSizes.h`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/include/Ranges.h` & `keopscore-2.2.3/keopscore/include/Ranges.h`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/include/Sizes.h` & `keopscore-2.2.3/keopscore/include/Sizes.h`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/include/ranges_utils.h` & `keopscore-2.2.3/keopscore/include/ranges_utils.h`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/include/utils_pe.h` & `keopscore-2.2.3/keopscore/include/utils_pe.h`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/licence.txt` & `keopscore-2.2.3/keopscore/licence.txt`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/mapreduce/Chunk_Mode_Constants.py` & `keopscore-2.2.3/keopscore/mapreduce/Chunk_Mode_Constants.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/mapreduce/MapReduce.py` & `keopscore-2.2.3/keopscore/mapreduce/MapReduce.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/mapreduce/cpu/CpuAssignZero.py` & `keopscore-2.2.3/keopscore/mapreduce/cpu/CpuAssignZero.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/mapreduce/cpu/CpuReduc.py` & `keopscore-2.2.3/keopscore/mapreduce/cpu/CpuReduc.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/mapreduce/cpu/CpuReduc_ranges.py` & `keopscore-2.2.3/keopscore/mapreduce/cpu/CpuReduc_ranges.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/mapreduce/gpu/GpuAssignZero.py` & `keopscore-2.2.3/keopscore/mapreduce/gpu/GpuAssignZero.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/mapreduce/gpu/GpuReduc1D.py` & `keopscore-2.2.3/keopscore/mapreduce/gpu/GpuReduc1D.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/mapreduce/gpu/GpuReduc1D_chunks.py` & `keopscore-2.2.3/keopscore/mapreduce/gpu/GpuReduc1D_chunks.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/mapreduce/gpu/GpuReduc1D_finalchunks.py` & `keopscore-2.2.3/keopscore/mapreduce/gpu/GpuReduc1D_finalchunks.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/mapreduce/gpu/GpuReduc1D_ranges.py` & `keopscore-2.2.3/keopscore/mapreduce/gpu/GpuReduc1D_ranges.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/mapreduce/gpu/GpuReduc1D_ranges_chunks.py` & `keopscore-2.2.3/keopscore/mapreduce/gpu/GpuReduc1D_ranges_chunks.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/mapreduce/gpu/GpuReduc1D_ranges_finalchunks.py` & `keopscore-2.2.3/keopscore/mapreduce/gpu/GpuReduc1D_ranges_finalchunks.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/mapreduce/gpu/GpuReduc2D.py` & `keopscore-2.2.3/keopscore/mapreduce/gpu/GpuReduc2D.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/readme.md` & `keopscore-2.2.3/keopscore/readme.md`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/utils/Cache.py` & `keopscore-2.2.3/keopscore/utils/Cache.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/utils/TestFormula.py` & `keopscore-2.2.3/keopscore/utils/TestFormula.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import time
 import torch
 import numpy as np
 from torch.autograd import grad
 from pykeops.torch import Genred
 from keopscore.formulas import *
 import types
+from keopscore.utils.misc_utils import KeOps_Print
 
 
 def TestFormula(formula, tol=1e-4, dtype="float32", test_grad=False, randseed=None):
     # N.B. dtype can be 'float32', 'float64' or 'float16'
 
     if isinstance(formula, str):
         formula_str = formula
         formula = eval(formula_str)
     else:
         formula_str = formula.__repr__()
 
     if randseed is not None:
         torch.manual_seed(randseed)
 
-    print("")
+    KeOps_Print("")
 
     formula = eval(formula_str)
     vars = formula.Vars_
     nargs = 1 + max(var.ind for var in vars)
 
     #####################################################################
     # Declare random inputs:
@@ -48,34 +49,34 @@
     args = [None] * nargs
     for var in vars:
         MorN = M if var.cat == 0 else N
         args[var.ind] = rand(
             MorN, var.dim, dtype=torchtype, device=device, requires_grad=True
         )
 
-    print("Testing formula " + formula_str)
+    KeOps_Print("Testing formula " + formula_str)
 
     my_routine = Genred(formula_str, [], reduction_op="Sum", axis=1)
     c = my_routine(*args)
 
-    print("ok, no error")
-    print("5 first values :", *c.flatten()[:5].tolist())
+    KeOps_Print("ok, no error")
+    KeOps_Print("5 first values :", *c.flatten()[:5].tolist())
 
     ####################################################################
     # Compute the gradient
     # -----------------------
 
     if test_grad:
         e = torch.rand_like(c)
 
-        print("Testing gradient of formula " + formula_str)
+        KeOps_Print("Testing gradient of formula " + formula_str)
 
         g = grad(c, args, e)
 
-        print("ok, no error")
+        KeOps_Print("ok, no error")
         for k in range(nargs):
             app_str = f"number {k}" if len(args) > 1 else ""
-            print(
+            KeOps_Print(
                 f"5 first values for gradient {app_str}:", *g[k].flatten()[:5].tolist()
             )
         return c, g
     return c
```

### Comparing `keopscore-2.2.2/keopscore/utils/TestOperation.py` & `keopscore-2.2.3/keopscore/utils/TestOperation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import time
 import torch
 import numpy as np
 from torch.autograd import grad
 from pykeops.torch import Genred
 from keopscore.formulas import *
 import types
+from keopscore.utils.misc_utils import KeOps_Print
 
 
 def TestOperation(op_str, tol=1e-4, dtype="float32", test_grad=True):
     # N.B. dtype can be 'float32', 'float64' or 'float16'
 
-    print("")
+    KeOps_Print("")
 
     keops_op = eval(op_str)
     if isinstance(keops_op, types.FunctionType):
         op_class_str = f"{op_str}_Impl"
         exec(f"from {keops_op.__module__} import {op_class_str}")
         keops_op_class = eval(op_class_str)
     else:
@@ -32,19 +33,19 @@
             elif hasattr(keops_op_class, "Derivative"):
                 from inspect import signature
 
                 nargs = len(signature(keops_op_class.Derivative).parameters)
                 if hasattr(keops_op_class, "test_params"):
                     nargs -= len(keops_op_class.test_params)
             else:
-                print("no test available for " + op_str)
+                KeOps_Print("no test available for " + op_str)
                 return None
             dims = [3] * nargs
     else:
-        print("no test available for " + op_str)
+        KeOps_Print("no test available for " + op_str)
         return None
 
     #####################################################################
     # Declare random inputs:
 
     M = 3000
     N = 5000
@@ -94,51 +95,51 @@
         + ","
         + ",".join(str(p) for p in params)
         + ")"
     )
 
     variables = list(f"v{k} = V{argcats[k]}({dims[k]})" for k in range(nargs))
 
-    print("Testing operation " + op_str)
+    KeOps_Print("Testing operation " + op_str)
 
     my_routine = Genred(formula, variables, reduction_op="Sum", axis=1)
     c = my_routine(*args)
 
-    print("ok, no error")
-    print("5 first values :", *c.flatten()[:5].tolist())
+    KeOps_Print("ok, no error")
+    KeOps_Print("5 first values :", *c.flatten()[:5].tolist())
 
     ####################################################################
     # Compute the gradient
     # -----------------------
 
     if test_grad:
         e = torch.rand_like(c)
 
-        print("Testing gradient of operation " + op_str)
+        KeOps_Print("Testing gradient of operation " + op_str)
 
         g = grad(c, args, e)
 
-        print("ok, no error")
+        KeOps_Print("ok, no error")
         for k in range(nargs):
             app_str = f"number {k}" if len(args) > 1 else ""
-            print(
+            KeOps_Print(
                 f"5 first values for gradient {app_str}:", *g[k].flatten()[:5].tolist()
             )
 
     if not hasattr(keops_op_class, "torch_op"):
         torch_op_str = keops_op_class.string_id.lower()
         if not torch_op_str in dir(torch):
             return "no_torch"
         torch_op = "torch." + torch_op_str
     else:
         if keops_op_class.torch_op is None:
             return "no_torch"
         torch_op = keops_op_class.torch_op
 
-    print("Comparing with PyTorch implementation ")
+    KeOps_Print("Comparing with PyTorch implementation ")
 
     torch_args = [None] * nargs
     for k in range(nargs):
         torch_args[k] = (
             args[k][:, None, :] if argcats[k] == "i" else args[k][None, :, :]
         )
 
@@ -146,28 +147,28 @@
     # The equivalent code with a "vanilla" pytorch implementation
 
     if isinstance(torch_op, str):
         torch_op = eval(torch_op)
 
     c_torch = torch_op(*torch_args, *params).sum(dim=1)
     err_op = torch.norm(c - c_torch).item() / torch.norm(c_torch).item()
-    print("relative error for operation :", err_op)
+    KeOps_Print("relative error for operation :", err_op)
 
     if test_grad:
         if (
             not hasattr(keops_op_class, "no_torch_grad")
             or not keops_op_class.no_torch_grad
         ):
             g_torch = grad(c_torch, args, e)
             err_gr = [None] * nargs
             for k in range(nargs):
                 app_str = f"number {k}" if len(args) > 1 else ""
                 err_gr[k] = (
                     torch.norm(g[k] - g_torch[k]) / torch.norm(g_torch[k])
                 ).item()
-                print(f"relative error for gradient {app_str}:", err_gr[k])
+                KeOps_Print(f"relative error for gradient {app_str}:", err_gr[k])
         else:
-            print("no gradient for torch")
+            KeOps_Print("no gradient for torch")
             return abs(err_op) > tol
         return abs(err_op) > tol, list(abs(err) > tol for err in err_gr)
     else:
         return abs(err_op) > tol
```

### Comparing `keopscore-2.2.2/keopscore/utils/Tree.py` & `keopscore-2.2.3/keopscore/utils/Tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from keopscore.utils.misc_utils import KeOps_Print
+
+
 class Tree:
     """a custom class for handling a tree structure.
     Currently we use it only to recursively print a formula or reduction"""
 
     def recursive_str(self):
         if hasattr(self, "print_spec"):
             idstr, mode, level = self.print_spec
@@ -104,15 +107,15 @@
                             graph [rankdir=LR];
                             {string}
                         }}
                   """
         text_file = open(filename, "w")
         text_file.write(string)
         text_file.close()
-        print(f"Saved formula graph to file {filename}.")
+        KeOps_Print(f"Saved formula graph to file {filename}.")
 
     def __str__(self):
         return self.nice_print()  # self.recursive_str()
 
     def __repr__(self):
         return self.recursive_str()
```

### Comparing `keopscore-2.2.2/keopscore/utils/code_gen_utils.py` & `keopscore-2.2.3/keopscore/utils/code_gen_utils.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/utils/gpu_utils.py` & `keopscore-2.2.3/keopscore/utils/gpu_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,17 @@
     # if not successfull, we try a few standard locations:
     cuda_version = get_cuda_version(out_type="string")
     cuda_paths_to_try_start = [
         join(os.path.sep, "opt", "cuda"),
         join(os.path.sep, "usr", "local", "cuda"),
         join(os.path.sep, "usr", "local", f"cuda-{cuda_version}"),
     ]
+    path_conda = os.getenv("CONDA_PREFIX")
+    if path_conda is not None:
+        cuda_paths_to_try_start.append(path_conda)
     cuda_paths_to_try_end = [
         "include",
         join("targets", "x86_64-linux", "include"),
     ]
     for path_start in cuda_paths_to_try_start:
         for path_end in cuda_paths_to_try_end:
             path = join(path_start, path_end)
```

### Comparing `keopscore-2.2.2/keopscore/utils/math_functions.py` & `keopscore-2.2.3/keopscore/utils/math_functions.py`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/keopscore/utils/misc_utils.py` & `keopscore-2.2.3/keopscore/utils/misc_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 #######################################################################
 
 import keopscore
 from os.path import join
 import re
 
 
+def KeOps_Print(message, force_print=False, **kwargs):
+    if keopscore.verbose or force_print:
+        print(message, **kwargs)
+
+
 def KeOps_Message(message, use_tag=True, **kwargs):
     if keopscore.verbose:
         tag = "[KeOps] " if use_tag else ""
         message = tag + message
         print(message, **kwargs)
 
 
@@ -36,15 +41,15 @@
     python_version = sys.version_info
     if python_version >= (3, 7):
         import subprocess
 
         out = subprocess.run(command, shell=True, capture_output=True)
         if out.stderr != b"":
             KeOps_Warning("There were warnings or errors :", newline=True)
-            print(out.stderr.decode("utf-8"))
+            KeOps_Print(out.stderr.decode("utf-8"))
     elif python_version >= (3, 5):
         import subprocess
 
         subprocess.run(
             command,
             shell=True,
         )
```

### Comparing `keopscore-2.2.2/keopscore.egg-info/PKG-INFO` & `keopscore-2.2.3/keopscore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keopscore
-Version: 2.2.2
+Version: 2.2.3
 Summary: keopscore is the KeOps meta programming engine. This python module should be used through a binder (e.g. pykeops or rkeops)
 Home-page: http://www.kernel-operations.io/
 Author: B. Charlier, J. Feydy, J. Glaunes
 Author-email: benjamin.charlier@umontpellier.fr, jean.feydy@gmail.com, alexis.glaunes@parisdescartes.fr
 Project-URL: Bug Reports, https://github.com/getkeops/keops/issues
 Project-URL: Source, https://github.com/getkeops/keops
 Keywords: kernels gpu autodiff
@@ -12,15 +12,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ![logo pykeops](http://www.kernel-operations.io/keops/_images/keops_logo.png)
 
 **keopscore** contains the [KeOps](https://www.kernel-operations.io/) meta programming engine. Given a formula, 
 it generates the c++/cuda code executed on the fly.
```

### Comparing `keopscore-2.2.2/keopscore.egg-info/SOURCES.txt` & `keopscore-2.2.3/keopscore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/licence.txt` & `keopscore-2.2.3/licence.txt`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/readme.md` & `keopscore-2.2.3/readme.md`

 * *Files identical despite different names*

### Comparing `keopscore-2.2.2/setup.py` & `keopscore-2.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     url="http://www.kernel-operations.io/",
     project_urls={
         "Bug Reports": "https://github.com/getkeops/keops/issues",
         "Source": "https://github.com/getkeops/keops",
     },
     author="B. Charlier, J. Feydy, J. Glaunes",
     author_email="benjamin.charlier@umontpellier.fr, jean.feydy@gmail.com, alexis.glaunes@parisdescartes.fr",
-    python_requires=">=3",
+    python_requires=">=3.8",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
```

