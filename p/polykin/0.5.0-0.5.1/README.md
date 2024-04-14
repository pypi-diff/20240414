# Comparing `tmp/polykin-0.5.0.tar.gz` & `tmp/polykin-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polykin-0.5.0.tar", max compression
+gzip compressed data, was "polykin-0.5.1.tar", max compression
```

## Comparing `polykin-0.5.0.tar` & `polykin-0.5.1.tar`

### file list

```diff
@@ -1,71 +1,73 @@
--rw-r--r--   0        0        0     1066 2024-03-23 15:55:31.750555 polykin-0.5.0/LICENSE
--rw-r--r--   0        0        0     3061 2024-03-23 15:55:31.750555 polykin-0.5.0/README.md
--rw-r--r--   0        0        0     1783 2024-03-23 15:55:31.766555 polykin-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      701 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/__init__.py
--rw-r--r--   0        0        0      366 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/copolymerization/__init__.py
--rw-r--r--   0        0        0     4533 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/copolymerization/binary.py
--rw-r--r--   0        0        0     6932 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/copolymerization/copodataset.py
--rw-r--r--   0        0        0     7024 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/copolymerization/fitting.py
--rw-r--r--   0        0        0    19611 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/copolymerization/multicomponent.py
--rw-r--r--   0        0        0    17186 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/copolymerization/penultimate.py
--rw-r--r--   0        0        0    24437 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/copolymerization/terminal.py
--rw-r--r--   0        0        0      362 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/distributions/__init__.py
--rw-r--r--   0        0        0    11409 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/distributions/analyticaldistributions.py
--rw-r--r--   0        0        0    27752 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/distributions/base.py
--rw-r--r--   0        0        0     7334 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/distributions/datadistribution.py
--rw-r--r--   0        0        0    30255 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/distributions/sampledata.py
--rw-r--r--   0        0        0      335 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/kinetics/__init__.py
--rw-r--r--   0        0        0     9523 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/kinetics/arrhenius.py
--rw-r--r--   0        0        0      846 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/kinetics/base.py
--rw-r--r--   0        0        0     4153 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/kinetics/cldpropagation.py
--rw-r--r--   0        0        0     5015 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/kinetics/cldtermination.py
--rw-r--r--   0        0        0     3764 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/kinetics/eyring.py
--rw-r--r--   0        0        0      198 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/math/__init__.py
--rw-r--r--   0        0        0     2418 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/math/derivatives.py
--rw-r--r--   0        0        0     9964 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/math/jcr.py
--rw-r--r--   0        0        0      281 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/properties/__init__.py
--rw-r--r--   0        0        0      284 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/properties/diffusion/__init__.py
--rw-r--r--   0        0        0     4774 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/properties/diffusion/liquid.py
--rw-r--r--   0        0        0     3861 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/properties/diffusion/vapor.py
--rw-r--r--   0        0        0    11932 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/properties/diffusion/vrentasduda.py
--rw-r--r--   0        0        0      323 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/properties/equations/__init__.py
--rw-r--r--   0        0        0    11019 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/properties/equations/base.py
--rw-r--r--   0        0        0    14174 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/properties/equations/dippr.py
--rw-r--r--   0        0        0     6550 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/properties/equations/vapor_pressure.py
--rw-r--r--   0        0        0     3070 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/properties/equations/viscosity.py
--rw-r--r--   0        0        0     4274 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/properties/mixing_rules.py
--rw-r--r--   0        0        0     3348 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/properties/pvt_polymer/Flory_parameters.tsv
--rw-r--r--   0        0        0     3722 2024-03-23 15:55:31.766555 polykin-0.5.0/src/polykin/properties/pvt_polymer/HartmannHaque_parameters.tsv
--rw-r--r--   0        0        0     3298 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/properties/pvt_polymer/SanchezLacombe_parameters.tsv
--rw-r--r--   0        0        0     2954 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/properties/pvt_polymer/Tait_parameters.tsv
--rw-r--r--   0        0        0      213 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/properties/pvt_polymer/__init__.py
--rw-r--r--   0        0        0     6555 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/properties/pvt_polymer/base.py
--rw-r--r--   0        0        0    10348 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/properties/pvt_polymer/eos.py
--rw-r--r--   0        0        0     5566 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/properties/pvt_polymer/tait.py
--rw-r--r--   0        0        0      272 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/properties/thermal_conductivity/__init__.py
--rw-r--r--   0        0        0     2116 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/properties/thermal_conductivity/liquid.py
--rw-r--r--   0        0        0     7195 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/properties/thermal_conductivity/vapor.py
--rw-r--r--   0        0        0     7723 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/properties/vaporization_enthalpy.py
--rw-r--r--   0        0        0      247 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/properties/viscosity/__init__.py
--rw-r--r--   0        0        0     1790 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/properties/viscosity/liquid.py
--rw-r--r--   0        0        0    12709 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/properties/viscosity/vapor.py
--rw-r--r--   0        0        0      215 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/stepgrowth/__init__.py
--rw-r--r--   0        0        0    34496 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/stepgrowth/solutions.py
--rw-r--r--   0        0        0      195 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/thermo/__init__.py
--rw-r--r--   0        0        0      265 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/thermo/acm/__init__.py
--rw-r--r--   0        0        0     4898 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/thermo/acm/base.py
--rw-r--r--   0        0        0    12554 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/thermo/acm/floryhuggins.py
--rw-r--r--   0        0        0     1524 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/thermo/acm/ideal.py
--rw-r--r--   0        0        0     8190 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/thermo/acm/nrtl.py
--rw-r--r--   0        0        0     8058 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/thermo/acm/uniquac.py
--rw-r--r--   0        0        0      260 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/thermo/eos/__init__.py
--rw-r--r--   0        0        0     6526 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/thermo/eos/base.py
--rw-r--r--   0        0        0    15526 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/thermo/eos/cubic.py
--rw-r--r--   0        0        0     1888 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/thermo/eos/idealgas.py
--rw-r--r--   0        0        0     9624 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/thermo/eos/virial.py
--rw-r--r--   0        0        0       86 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/utils/__init__.py
--rw-r--r--   0        0        0      356 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/utils/exceptions.py
--rw-r--r--   0        0        0     3082 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/utils/math.py
--rw-r--r--   0        0        0     9976 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/utils/tools.py
--rw-r--r--   0        0        0     1088 2024-03-23 15:55:31.770555 polykin-0.5.0/src/polykin/utils/types.py
--rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 polykin-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-14 21:31:23.594301 polykin-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3022 2024-04-14 21:31:23.594301 polykin-0.5.1/README.md
+-rw-r--r--   0        0        0     1801 2024-04-14 21:31:23.614301 polykin-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      701 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/__init__.py
+-rw-r--r--   0        0        0      366 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/copolymerization/__init__.py
+-rw-r--r--   0        0        0     4533 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/copolymerization/binary.py
+-rw-r--r--   0        0        0     6932 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/copolymerization/copodataset.py
+-rw-r--r--   0        0        0    12850 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/copolymerization/fitting.py
+-rw-r--r--   0        0        0    19779 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/copolymerization/multicomponent.py
+-rw-r--r--   0        0        0    17038 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/copolymerization/penultimate.py
+-rw-r--r--   0        0        0    24303 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/copolymerization/terminal.py
+-rw-r--r--   0        0        0      362 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/distributions/__init__.py
+-rw-r--r--   0        0        0    11409 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/distributions/analyticaldistributions.py
+-rw-r--r--   0        0        0    27752 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/distributions/base.py
+-rw-r--r--   0        0        0     7334 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/distributions/datadistribution.py
+-rw-r--r--   0        0        0    30255 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/distributions/sampledata.py
+-rw-r--r--   0        0        0      335 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/kinetics/__init__.py
+-rw-r--r--   0        0        0     9460 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/kinetics/arrhenius.py
+-rw-r--r--   0        0        0      846 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/kinetics/base.py
+-rw-r--r--   0        0        0     4078 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/kinetics/cldpropagation.py
+-rw-r--r--   0        0        0     4936 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/kinetics/cldtermination.py
+-rw-r--r--   0        0        0     3704 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/kinetics/eyring.py
+-rw-r--r--   0        0        0      198 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/math/__init__.py
+-rw-r--r--   0        0        0     2418 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/math/derivatives.py
+-rw-r--r--   0        0        0     9805 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/math/jcr.py
+-rw-r--r--   0        0        0      281 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/__init__.py
+-rw-r--r--   0        0        0      284 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/diffusion/__init__.py
+-rw-r--r--   0        0        0     4669 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/diffusion/liquid.py
+-rw-r--r--   0        0        0     3759 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/diffusion/vapor.py
+-rw-r--r--   0        0        0    11866 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/diffusion/vrentasduda.py
+-rw-r--r--   0        0        0      323 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/equations/__init__.py
+-rw-r--r--   0        0        0    10887 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/equations/base.py
+-rw-r--r--   0        0        0    14174 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/equations/dippr.py
+-rw-r--r--   0        0        0     6429 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/equations/vapor_pressure.py
+-rw-r--r--   0        0        0     3070 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/equations/viscosity.py
+-rw-r--r--   0        0        0     4274 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/mixing_rules.py
+-rw-r--r--   0        0        0     3348 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/pvt_polymer/Flory_parameters.tsv
+-rw-r--r--   0        0        0     3722 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/pvt_polymer/HartmannHaque_parameters.tsv
+-rw-r--r--   0        0        0     3298 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/pvt_polymer/SanchezLacombe_parameters.tsv
+-rw-r--r--   0        0        0     2954 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/pvt_polymer/Tait_parameters.tsv
+-rw-r--r--   0        0        0      213 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/pvt_polymer/__init__.py
+-rw-r--r--   0        0        0     6555 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/pvt_polymer/base.py
+-rw-r--r--   0        0        0    10277 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/pvt_polymer/eos.py
+-rw-r--r--   0        0        0     5566 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/pvt_polymer/tait.py
+-rw-r--r--   0        0        0      272 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/thermal_conductivity/__init__.py
+-rw-r--r--   0        0        0     2159 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/thermal_conductivity/liquid.py
+-rw-r--r--   0        0        0     7252 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/thermal_conductivity/vapor.py
+-rw-r--r--   0        0        0     7619 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/vaporization_enthalpy.py
+-rw-r--r--   0        0        0      247 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/viscosity/__init__.py
+-rw-r--r--   0        0        0     1802 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/viscosity/liquid.py
+-rw-r--r--   0        0        0    12768 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/properties/viscosity/vapor.py
+-rw-r--r--   0        0        0      215 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/stepgrowth/__init__.py
+-rw-r--r--   0        0        0    34496 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/stepgrowth/solutions.py
+-rw-r--r--   0        0        0      195 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/__init__.py
+-rw-r--r--   0        0        0      287 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/acm/__init__.py
+-rw-r--r--   0        0        0    12659 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/acm/base.py
+-rw-r--r--   0        0        0    12655 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/acm/floryhuggins.py
+-rw-r--r--   0        0        0      886 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/acm/ideal.py
+-rw-r--r--   0        0        0     7621 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/acm/nrtl.py
+-rw-r--r--   0        0        0     9363 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/acm/polynrtl.py
+-rw-r--r--   0        0        0     7513 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/acm/uniquac.py
+-rw-r--r--   0        0        0     4953 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/acm/wilson.py
+-rw-r--r--   0        0        0      260 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/eos/__init__.py
+-rw-r--r--   0        0        0     6544 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/eos/base.py
+-rw-r--r--   0        0        0    15285 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/eos/cubic.py
+-rw-r--r--   0        0        0     1976 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/eos/idealgas.py
+-rw-r--r--   0        0        0     9579 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/eos/virial.py
+-rw-r--r--   0        0        0       86 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/utils/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/utils/exceptions.py
+-rw-r--r--   0        0        0     3082 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/utils/math.py
+-rw-r--r--   0        0        0     9976 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/utils/tools.py
+-rw-r--r--   0        0        0     1088 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/utils/types.py
+-rw-r--r--   0        0        0     4131 1970-01-01 00:00:00.000000 polykin-0.5.1/PKG-INFO
```

### Comparing `polykin-0.5.0/LICENSE` & `polykin-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/README.md` & `polykin-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [![codecov](https://codecov.io/gh/HugoMVale/polykin/branch/main/graph/badge.svg?token=QfqQLX2rHx)](https://codecov.io/gh/HugoMVale/polykin)
 [![Latest Commit](https://img.shields.io/github/last-commit/HugoMVale/polykin)](https://img.shields.io/github/last-commit/HugoMVale/polykin)
 
 PolyKin is an open-source polymerization kinetics library for Python. It is still at an early
 development stage, but the following modules can already be used:
 
 - Activity coefficient models
-  - [50%] Cubic (Redlich-Kwong, Soave, Peng-Robinson)
   - [x] Ideal solution
   - [x] Flory-Huggins
   - [x] NRTL
   - [ ] Poly-NRTL
   - [x] UNIQUAC
+  - [x] Wilson
 - Copolymerization
   - [x] Implicit penultimate model
   - [x] Penultimate model
   - [x] Terminal model
   - [x] Mayo-Lewis equation (binary, ternary and multicomponent)
   - [x] Monomer dift equation (multicomponent)
   - [ ] Fitting methods
```

#### html2text {}

```diff
@@ -2,35 +2,34 @@
 test.yml/badge.svg)](https://github.com/HugoMVale/polykin/actions) [![codecov]
 (https://codecov.io/gh/HugoMVale/polykin/branch/main/graph/
 badge.svg?token=QfqQLX2rHx)](https://codecov.io/gh/HugoMVale/polykin) [![Latest
 Commit](https://img.shields.io/github/last-commit/HugoMVale/polykin)](https://
 img.shields.io/github/last-commit/HugoMVale/polykin) PolyKin is an open-source
 polymerization kinetics library for Python. It is still at an early development
 stage, but the following modules can already be used: - Activity coefficient
-models - [50%] Cubic (Redlich-Kwong, Soave, Peng-Robinson) - [x] Ideal solution
-- [x] Flory-Huggins - [x] NRTL - [ ] Poly-NRTL - [x] UNIQUAC - Copolymerization
-- [x] Implicit penultimate model - [x] Penultimate model - [x] Terminal model -
-[x] Mayo-Lewis equation (binary, ternary and multicomponent) - [x] Monomer dift
-equation (multicomponent) - [ ] Fitting methods - Equations of state - [50%]
-Cubic (Redlich-Kwong, Soave, Peng-Robinson) - [x] Ideal gas - [ ] Sanchez-
-Lacombe - [x] Virial equation - [ ] Database - Distributions - [x] Flory - [ ]
-Gold - [x] Log-normal - [x] Poison - [x] Schulz-Zimm - Kinetics - [x] Arrhenius
-- [x] Eyring - [x] Propagation half-length - [x] Termination composite model -
-Math - [x] Joint confidence regions - [ ] Models - Physical property
-correlations - [x] Antoine - [x] DIPPR - [x] Wagner - [x] Yaws - Step-growth
-polymerization - [x] Analytical solutions for $M_n$ and $M_w$ - Transport
-properties (estimation methods, mixing rules, etc.) - Diffusivity - [x] Binary
-gas mixtures - [x] Binary liquid mixtures - [x] Binary polymer solutions - [ ]
-Multicomponent polymer solutions - Thermal conductivity - [x] Gases - [x]
-Liquids - [ ] Polymer solutions - Viscosity - [x] Gases - [x] Liquids - [ ]
-Polymer solutions ## Documentation Please refer to the package [homepage]
-(https://hugomvale.github.io/polykin/). ## Tutorials The main features of
-PolyKin are explained and illustrated through a series of [tutorials](https://
-hugomvale.github.io/polykin/tutorials/) based on Jupyter [notebooks](https://
-github.com/HugoMVale/polykin/tree/main/docs/tutorials), which can be launched
-online via Binder.
+models - [x] Ideal solution - [x] Flory-Huggins - [x] NRTL - [ ] Poly-NRTL -
+[x] UNIQUAC - [x] Wilson - Copolymerization - [x] Implicit penultimate model -
+[x] Penultimate model - [x] Terminal model - [x] Mayo-Lewis equation (binary,
+ternary and multicomponent) - [x] Monomer dift equation (multicomponent) - [ ]
+Fitting methods - Equations of state - [50%] Cubic (Redlich-Kwong, Soave, Peng-
+Robinson) - [x] Ideal gas - [ ] Sanchez-Lacombe - [x] Virial equation - [ ]
+Database - Distributions - [x] Flory - [ ] Gold - [x] Log-normal - [x] Poison -
+[x] Schulz-Zimm - Kinetics - [x] Arrhenius - [x] Eyring - [x] Propagation half-
+length - [x] Termination composite model - Math - [x] Joint confidence regions
+- [ ] Models - Physical property correlations - [x] Antoine - [x] DIPPR - [x]
+Wagner - [x] Yaws - Step-growth polymerization - [x] Analytical solutions for
+$M_n$ and $M_w$ - Transport properties (estimation methods, mixing rules, etc.)
+- Diffusivity - [x] Binary gas mixtures - [x] Binary liquid mixtures - [x]
+Binary polymer solutions - [ ] Multicomponent polymer solutions - Thermal
+conductivity - [x] Gases - [x] Liquids - [ ] Polymer solutions - Viscosity -
+[x] Gases - [x] Liquids - [ ] Polymer solutions ## Documentation Please refer
+to the package [homepage](https://hugomvale.github.io/polykin/). ## Tutorials
+The main features of PolyKin are explained and illustrated through a series of
+[tutorials](https://hugomvale.github.io/polykin/tutorials/) based on Jupyter
+[notebooks](https://github.com/HugoMVale/polykin/tree/main/docs/tutorials),
+which can be launched online via Binder.
                            _[_M_W_D_ _o_f_ _a_ _p_o_l_y_m_e_r_ _b_l_e_n_d_]
 ## Installation PolyKin currently runs on Python 3.9+. You can install it from
 PyPI via `pip` (or `poetry`): ```console pip install polykin # poetry add
 polykin ``` Alternatively, you may install it directly from the source code
 repository: ```console git clone https://github.com/HugoMVale/polykin.git cd
 polykin pip install . # poetry install ```
```

### Comparing `polykin-0.5.0/pyproject.toml` & `polykin-0.5.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polykin"
-version = "0.5.0"
+version = "0.5.1"
 description = "A polymerization kinetics library."
 authors = ["HugoMVale <57530119+HugoMVale@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hugomvale.github.io/polykin/"
 repository = "https://github.com/HugoMVale/polykin"
 documentation = "https://hugomvale.github.io/polykin/"
@@ -16,33 +16,25 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Chemistry",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.13"
+python = ">=3.9,<4.0"
 mpmath = "^1.3.0"
 pydantic = "^1.10.13"
 numpy = "^1.23.5"
 scipy = "^1.11.4"
 matplotlib = "^3.7.1"
 nptyping = "^2.5.0"
 pandas = ">=1.5.3"
 # sqlalchemy = "^2.0.22"
 # numba = "^0.58.1"
 
-[tool.poetry.group.dev]
-optional = true
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.4.4"
-coverage = "^7.4.0"
-pytest-xdist = "^3.5.0"
-pytest-cov = "^4.1.0"
-
 [tool.poetry.group.docs]
 optional = true
 [tool.poetry.group.docs.dependencies]
 ipykernel = "^6.20.0"
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.5.3"
 mkdocs-jupyter = "^0.24.6"
@@ -52,14 +44,22 @@
 black = "^23.3.0"
 mkdocstrings = { extras = ["python"], version = "^0.22.0" }
 mkdocs-bibtex = "^2.11.0"
 markdown-exec = "^1.6.0"
 mkdocs-gallery = "^0.7.8"
 mkdocs-table-reader-plugin = "^2.0.3"
 mkdocs-autorefs = "^0.5.0"
+griffe-inherited-docstrings = "^1.0.0"
+
+[tool.poetry.group.dev]
+optional = true
+[tool.poetry.group.dev.dependencies]
+pytest = "^8.1.1"
+pytest-xdist = "^3.5.0"
+pytest-cov = "^5.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = ["-n=2", "--import-mode=importlib"]
```

### Comparing `polykin-0.5.0/src/polykin/__init__.py` & `polykin-0.5.1/src/polykin/__init__.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/copolymerization/binary.py` & `polykin-0.5.1/src/polykin/copolymerization/binary.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/copolymerization/copodataset.py` & `polykin-0.5.1/src/polykin/copolymerization/copodataset.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/copolymerization/multicomponent.py` & `polykin-0.5.1/src/polykin/copolymerization/multicomponent.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,27 +159,27 @@
 
     where $P_{ij}$ are the transition probabilitites, which can be computed
     from the instantaneous monomer composition and the reactivity matrix.
 
     Parameters
     ----------
     f : FloatVectorLike | None
-        Vector (N) of instantaneous monomer composition.
+        Vector (N) of instantaneous monomer compositions, $f_i$.
     r : FloatSquareMatrix | None
-        Reactivity ratio matrix (NxN), $r_{ij}=k_{ii}/k_{ij}$.
+        Matrix (NxN) of reactivity ratios, $r_{ij}=k_{ii}/k_{ij}$.
     P : FloatSquareMatrix | None
-        Transition probability matrix (NxN), $P_{ij}$. If `None`, it will be
-        computed internally. When calculating other quantities (e.g., sequence
-        lengths, tuples) that also depend on $P$, it is more efficient to
-        precompute $P$ once and use it in all cases.
+        Matrix (NxN) of transition probabilities, $P_{ij}$. If `None`, it will
+        be computed internally. When calculating other quantities (e.g.,
+        sequence lengths, tuples) that also depend on $P$, it is more efficient
+        to precompute $P$ once and use it in all cases.
 
     Returns
     -------
     FloatVector
-        Vector (N) of instantaneous copolymer composition.
+        Vector (N) of instantaneous copolymer compositions, $F_i$.
 
     !!! note annotate "See also"
 
         * [`inst_copolymer_binary`](inst_copolymer_binary.md):
           specific method for binary systems.
         * [`inst_copolymer_ternary`](inst_copolymer_ternary.md):
           specific method for terpolymer systems.
@@ -247,28 +247,28 @@
     with initial condition $f_i(0)=f_{i,0}$, where $f_i$ and $F_i$ are,
     respectively, the instantaneous comonomer and copolymer composition of
     monomer $i$, and $x$ is the total molar monomer conversion.
 
     Parameters
     ----------
     f0 : FloatVectorLike
-        Vector (N) of initial instantaneous comonomer composition.
+        Vector (N) of initial instantaneous comonomer compositions.
     r : FloatSquareMatrix
-        Reactivity ratio matrix (NxN).
+        Matrix (NxN) of reactivity ratios, $r_{ij}=k_{ii}/k_{ij}$.
     x : FloatVectorLike
         Vector (M) of total monomer conversion values where the drift is to be
         evaluated.
     rtol : float
         Relative tolerance of ODE solver.
 
     Returns
     -------
     FloatMatrix
         Matrix (MxN) of monomer fraction of monomer $i$ at the specified
-        total monomer conversion(s), $f_i(x)$.
+        total monomer conversion(s), $f_i(x_j)$.
 
     !!! note annotate "See also"
 
         * [`inst_copolymer_multi`](inst_copolymer_multi.md):
           instantaneous copolymer composition.
 
     Examples
@@ -327,35 +327,36 @@
                       ) -> FloatSquareMatrix:
     r"""Calculate the instantaneous transition probabilities for a
     multicomponent system.
 
     For a multicomponent system, the transition probabilities are given
     by:
 
-    $$ P_{ij} = \frac{r_{ij}^{-1} f_j}{\sum_k r_{ik}^{-1} f_k} $$
+    $$ P_{ij} = \frac{r_{ij}^{-1} f_j}
+                     {\displaystyle \sum_{k=1}^{N} r_{ik}^{-1} f_k} $$
 
     where $f_i$ is the molar fraction of monomer $i$ and $r_{ij}=k_{ii}/k_{ij}$
     is the multicomponent reactivity ratio matrix.
 
     **References**
 
     *   NA Dotson, R Galván, RL Laurence, and M Tirrel. Polymerization
         process modeling, Wiley, 1996, p. 178.
 
     Parameters
     ----------
     f : FloatVectorLike
-        Vector (N) of instantaneous monomer composition.
+        Vector (N) of instantaneous monomer compositions, $f_i$.
     r : FloatSquareMatrix
-        Reactivity ratio matrix (NxN), $r_{ij}=k_{ii}/k_{ij}$.
+        Matrix (NxN) of reactivity ratios, $r_{ij}=k_{ii}/k_{ij}$.
 
     Returns
     -------
     FloatSquareMatrix
-        Matrix (NxN) of transition probabilities.
+        Matrix (NxN) of transition probabilities, $P_{ij}$.
 
     !!! note annotate "See also"
 
         * [`inst_copolymer_multi`](inst_copolymer_multi.md):
           instantaneous copolymer composition.
         * [`sequence_multi`](sequence_multi.md):
           instantaneous sequence lengths.
@@ -406,15 +407,15 @@
     For a multicomponent system, the probability of finding $k$ consecutive
     units of monomer $i$ in a chain is:
 
     $$ S_{i,k} = (1 - P_{ii})P_{ii}^{k-1} $$
 
     and the corresponding number-average sequence length is:
 
-    $$ \bar{S}_i = \sum_k k S_{i,k} = \frac{1}{1 - P_{ii}} $$
+    $$ \bar{S}_i = \sum_{k=1}^{\infty} k S_{i,k} = \frac{1}{1 - P_{ii}} $$
 
     where $P_{ii}$ is the self-transition probability $i \rightarrow i$, which
     is a function of the monomer composition and the reactivity ratios.
 
     **References**
 
     * NA Dotson, R Galván, RL Laurence, and M Tirrel. Polymerization
@@ -511,26 +512,27 @@
 
     *   NA Dotson, R Galván, RL Laurence, and M Tirrel. Polymerization
         process modeling, Wiley, 1996, p. 179.
 
     Parameters
     ----------
     P : FloatSquareMatrix
-        Transition probability matrix (NxN), $P_{ij}$.
+        Matrix (NxN) of transition probabilities, $P_{ij}$.
     n : int
-        Tuple length,.e.g monads(1), diads(2), triads(3), etc.
+        Tuple length,.e.g monads (1), diads (2), triads (3), etc.
     F : FloatVectorLike | None
-        Instantaneous copolymer composition, $F_i$. If `None`, the value will
-        be computed internally. When calculating tuples of various lengths, it
-        is more efficient to precompute $F$ and use it in all tuple cases.
+        Vector (N) of instantaneous copolymer composition, $F_i$. If `None`,
+        the value will be computed internally. When calculating tuples of
+        various lengths, it is more efficient to precompute $F$ and use it in
+        all tuple cases.
 
     Returns
     -------
     dict[tuple[int, ...], float]
-        Tuple molar fractions.
+        Tuple of molar fractions.
 
     !!! note annotate "See also"
 
         * [`sequence_multi`](sequence_multi.md):
           instantaneous sequence lengths.
         * [`transitions_multi`](transitions_multi.md):
           instantaneous transition probabilities.
```

### Comparing `polykin-0.5.0/src/polykin/copolymerization/penultimate.py` & `polykin-0.5.1/src/polykin/copolymerization/penultimate.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,14 @@
                  s2: float,
                  k1: Optional[Arrhenius] = None,
                  k2: Optional[Arrhenius] = None,
                  M1: str = 'M1',
                  M2: str = 'M2',
                  name: str = ''
                  ) -> None:
-        """Construct `PenultimateModel` with the given parameters."""
 
         check_bounds(r11, 0., np.inf, 'r11')
         check_bounds(r12, 0., np.inf, 'r12')
         check_bounds(r21, 0., np.inf, 'r21')
         check_bounds(r22, 0., np.inf, 'r22')
         check_bounds(s1, 0., np.inf, 's1')
         check_bounds(s2, 0., np.inf, 's2')
@@ -448,15 +447,14 @@
                  s2: float,
                  k1: Optional[Arrhenius] = None,
                  k2: Optional[Arrhenius] = None,
                  M1: str = 'M1',
                  M2: str = 'M2',
                  name: str = ''
                  ) -> None:
-        """Construct `ImplicitPenultimateModel` with the given parameters."""
 
         check_bounds(s1, 0., np.inf, 's1')
         check_bounds(s2, 0., np.inf, 's2')
 
         self.s1 = s1
         self.s2 = s2
         super().__init__(r1, r2, k1, k2, M1, M2, name)
```

### Comparing `polykin-0.5.0/src/polykin/copolymerization/terminal.py` & `polykin-0.5.1/src/polykin/copolymerization/terminal.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     def __init__(self,
                  k1: Optional[Arrhenius],
                  k2: Optional[Arrhenius],
                  M1: str,
                  M2: str,
                  name: str
                  ) -> None:
-        """Construct `CopoModel` with the given parameters."""
 
         if M1 and M2 and M1.lower() != M2.lower():
             self.M1 = M1
             self.M2 = M2
         else:
             raise ValueError("`M1` and `M2` must be non-empty and different.")
 
@@ -497,15 +496,14 @@
                  r2: float,
                  k1: Optional[Arrhenius] = None,
                  k2: Optional[Arrhenius] = None,
                  M1: str = 'M1',
                  M2: str = 'M2',
                  name: str = ''
                  ) -> None:
-        """Construct `TerminalCopoModel` with the given parameters."""
 
         check_bounds(r1, 0., np.inf, 'r1')
         check_bounds(r2, 0., np.inf, 'r2')
 
         # Perhaps this could be upgraded to exception, but I don't want to be
         # too restrictive (one does find literature data with (r1,r2)>1)
         if r1 > 1. and r2 > 1.:
```

### Comparing `polykin-0.5.0/src/polykin/distributions/analyticaldistributions.py` & `polykin-0.5.1/src/polykin/distributions/analyticaldistributions.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/distributions/base.py` & `polykin-0.5.1/src/polykin/distributions/base.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/distributions/datadistribution.py` & `polykin-0.5.1/src/polykin/distributions/datadistribution.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/distributions/sampledata.py` & `polykin-0.5.1/src/polykin/distributions/sampledata.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/kinetics/arrhenius.py` & `polykin-0.5.1/src/polykin/kinetics/arrhenius.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,14 @@
                  T0: Union[float, FloatArrayLike] = np.inf,
                  Tmin: Union[float, FloatArrayLike] = 0.0,
                  Tmax: Union[float, FloatArrayLike] = np.inf,
                  unit: str = '-',
                  symbol: str = 'k',
                  name: str = ''
                  ) -> None:
-        """Construct `Arrhenius` with the given parameters."""
 
         # Convert lists to arrays
         k0, EaR, T0, Tmin, Tmax = \
             convert_FloatOrArrayLike_to_FloatOrArray([k0, EaR, T0, Tmin, Tmax])
 
         # Check shapes
         self._shape = check_shapes([k0, EaR], [T0, Tmin, Tmax])
```

### Comparing `polykin-0.5.0/src/polykin/kinetics/base.py` & `polykin-0.5.1/src/polykin/kinetics/base.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/kinetics/cldpropagation.py` & `polykin-0.5.1/src/polykin/kinetics/cldpropagation.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 
     def __init__(self,
                  kp: Union[Arrhenius, Eyring],
                  C: float = 10.,
                  ihalf: float = 1.0,
                  name: str = ''
                  ) -> None:
-        """Construct `PropagationHalfLength` with the given parameters."""
 
         check_type(kp, (Arrhenius, Eyring), 'kp')
         check_bounds(C, 1., 100., 'C')
         check_bounds(ihalf, 0.1, 10, 'ihalf')
 
         self.kp = kp
         self.C = C
```

### Comparing `polykin-0.5.0/src/polykin/kinetics/cldtermination.py` & `polykin-0.5.1/src/polykin/kinetics/cldtermination.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,15 +69,14 @@
     def __init__(self,
                  kt11: Union[Arrhenius, Eyring],
                  icrit: int,
                  aS: float = 0.5,
                  aL: float = 0.2,
                  name: str = ''
                  ) -> None:
-        """Construct `TerminationCompositeModel` with the given parameters."""
 
         check_type(kt11, (Arrhenius, Eyring), 'k11')
         check_bounds(icrit, 1, 200, 'icrit')
         check_bounds(aS, 0, 1, 'alpha_short')
         check_bounds(aL, 0, 0.5, 'alpha_long')
 
         self.kt11 = kt11
```

### Comparing `polykin-0.5.0/src/polykin/kinetics/eyring.py` & `polykin-0.5.1/src/polykin/kinetics/eyring.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,15 +71,14 @@
                  DHa: Union[float, FloatArrayLike],
                  kappa: Union[float, FloatArrayLike] = 1.0,
                  Tmin: Union[float, FloatArrayLike] = 0.0,
                  Tmax: Union[float, FloatArrayLike] = np.inf,
                  symbol: str = 'k',
                  name: str = ''
                  ) -> None:
-        """Construct `Eyring` with the given parameters."""
 
         # Convert lists to arrays
         DSa, DHa, kappa, Tmin, Tmax = \
             convert_FloatOrArrayLike_to_FloatOrArray(
                 [DSa, DHa, kappa, Tmin, Tmax])
 
         # Check shapes
```

### Comparing `polykin-0.5.0/src/polykin/math/derivatives.py` & `polykin-0.5.1/src/polykin/math/derivatives.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/math/jcr.py` & `polykin-0.5.1/src/polykin/math/jcr.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # Copyright Hugo Vale 2024
 
 from typing import Callable, Optional
 
 import numpy as np
 from matplotlib.axes._axes import Axes
 from matplotlib.patches import Ellipse
-from numpy import arctan, cos, sin, sqrt
+from numpy import arctan, cos, exp, log, sin, sqrt
 from scipy.integrate import solve_ivp
 from scipy.optimize import root_scalar
 from scipy.stats.distributions import f as Fdist
 from scipy.stats.distributions import t as tdist
 
 from polykin.utils.exceptions import (ODESolverError, RootSolverError,
                                       ShapeError)
 from polykin.utils.math import eps
 from polykin.utils.tools import check_bounds
-from polykin.utils.types import Float2x2Matrix
+from polykin.utils.types import Float2x2Matrix, FloatVector
 
 __all__ = ['confidence_ellipse',
            'confidence_region']
 
 
 def confidence_ellipse(ax: Axes,
                        center: tuple[float, float],
@@ -63,24 +63,24 @@
     where $t$ is Student's $t$ distribution.
 
     **Reference**
 
     *   Vugrin, K. W., L. P. Swiler, R. M. Roberts, N. J. Stucky-Mack, and
     S. P. Sullivan (2007), Confidence region estimation techniques for
     nonlinear regression in groundwater flow: Three case studies, Water
-    Resour. Res., 43, W03423, doi:10.1029/2005WR004804.
+    Resour. Res., 43.
 
     Parameters
     ----------
     ax : Axes
         Matplotlib Axes object to which ellipse will be patched.
     center : tuple[float, float]
         Point estimate of the model parameters, $\hat{\beta}$.
     cov : Float2x2Matrix
-        Scaled variance-covariance matrix (2x2), $\hat{V}$.
+        Scaled variance-covariance matrix, $\hat{V}$.
     ndata : int
         Number of data points.
     alpha : float
         Significance level, $\alpha$.
     color : str
         Color of ellipse contour and center.
     label : str | None
@@ -137,25 +137,21 @@
     if confint:
         ci = sqrt(np.diag(cov))*tdist.ppf(1. - alpha/2, ndata - npar)
         ax.errorbar(*center, xerr=ci[0], yerr=ci[1], color=color)
 
     return None
 
 
-def confidence_region(ax: Axes,
-                      center: tuple[float, float],
-                      sse: Callable[[tuple[float, float]], float],
+def confidence_region(center: tuple[float, float],
+                      sse: Callable[[float, float], float],
                       ndata: int,
                       alpha: float = 0.05,
                       width: Optional[float] = None,
-                      rtol: float = 1e-4,
-                      color: str = 'black',
-                      label: Optional[str] = None,
-                      npoints: int = 200
-                      ) -> None:
+                      rtol: float = 1e-4
+                      ) -> tuple[FloatVector, FloatVector]:
     r"""Generate a confidence region for 2 jointly estimated parameters
     using a rigorous method.
 
     The joint $100(1-\alpha)\%$ confidence region (JCR) for the parameters
     $\beta=(\beta_1, \beta_2)$ is represented by the domain of values that
     satisfy the following condition:
 
@@ -176,107 +172,111 @@
         to naive 2D mesh screening approaches, but the number of $S(\beta)$
         evaluations remains large (typically several hundreds). Therefore, the
         applicability of this method depends on the cost of evaluating
         $S(\beta)$.
 
     **Reference**
 
+    * Arutjunjan, R., Schaefer, B. M., Kreutz, C., Constructing Exact
+    Confidence Regions on Parameter Manifolds of Non-Linear Models, 2022.
+
     *   Vugrin, K. W., L. P. Swiler, R. M. Roberts, N. J. Stucky-Mack, and
     S. P. Sullivan (2007), Confidence region estimation techniques for
     nonlinear regression in groundwater flow: Three case studies, Water
-    Resour. Res., 43, W03423, doi:10.1029/2005WR004804.
-
-    * Arutjunjan, R., Schaefer, B. M., Kreutz, C., Constructing Exact
-    Confidence Regions on Parameter Manifolds of Non-Linear Models, 2022,
-    https://doi.org/10.48550/arXiv.2211.03421.
+    Resour. Res., 43.
 
     Parameters
     ----------
-    ax : Axes
-        Matplotlib Axes object to which the joint confidence region will be
-        added.
     center : tuple[float, float]
         Point estimate of the model parameters, $\hat{\beta}$.
-    sse : Callable[[tuple[float, float]], float]
+    sse : Callable[[float, float], float]
         Error sum of squares function, $S(\beta_1, \beta_2)$.
     ndata : int
         Number of data points.
     alpha : float
         Significance level, $\alpha$.
     width : float | None
         Initial guess of the width of the joint confidence region at its
         center. If `None`, it is assumed that `width=0.5*center[0]`.
     rtol : float
-        Relative tolerance of ODE solver.
-    color : str
-        Color of confidence region boundary and center.
-    label : str | None
-        Ellipse label.
-    npoints : int
-        Number of points used to draw the confidence region.
+        Relative tolerance of ODE solver. The default value may be decreased
+        by one or more orders of magnitude if the resolution of the JCR appears
+        insufficient.
+
+    Returns
+    -------
+    tuple[FloatVector, FloatVector]
+        Coordinates (x, y) of the confidence region.
 
     !!! note annotate "See also"
 
         * [`confidence_ellipse`](confidence_ellipse.md): alternative method
         based on linear approximation.
 
     """
 
     # Method implementation is specific for 2D
     npar = 2
     if len(center) != npar:
         raise ShapeError(f"`center` must be a vector of length {npar}.")
 
     # Check inputs
-    check_bounds(alpha, 0.001, 0.90, 'alpha')
+    check_bounds(alpha, 0.001, 0.99, 'alpha')
     check_bounds(ndata, npar + 1, np.inf, 'ndata')
 
     # Boundary
     Fval = Fdist.ppf(1. - alpha, npar, ndata - npar)
-    sse_boundary = sse(center)*(1. + npar/(ndata - npar)*Fval)
+    sse_boundary = sse(*center)*(1. + npar/(ndata - npar)*Fval)
 
     # Find boundary radius at 3 o'clock
     sol = root_scalar(
-        f=lambda r: sse((center[0] + r, center[1])) - sse_boundary,
+        f=lambda r: sse(center[0] + r, center[1]) - sse_boundary,
         method='secant',
         x0=0,
         x1=width/2 if width is not None else 0.25*center[0])
     if not sol.converged:
         raise RootSolverError(sol.flag)
     else:
         r0 = sol.root
 
+    # Transform 'sse' to log-radial coordinates
+    def f(s: float, q: float) -> float:
+        r = exp(s)
+        x = center[0] + r*cos(q)
+        y = center[1] + r*sin(q)
+        return sse(x, y)
+
     # Move along boundary using radial coordinates
-    def rdot(theta: float, r: float) -> float:
-        "Calculate dr/dtheta along a path of constant 'sse'."
-        a = sin(theta)
-        b = cos(theta)
-        x = center[0] + r*b
-        y = center[1] + r*a
-        sse_0 = sse((x, y))
+    # Imagine a particle transported by a velocity field orthogonal to 'sse'
+    def dydt(t: float, y: np.ndarray) -> np.ndarray:
+        s = y[0]
+        q = y[1]
         h = 2*sqrt(eps)
-        hx = max(h, abs(x)*h)
-        hy = max(h, abs(y)*h)
-        sse_x = (sse((x + hx, y)) - sse_0)/hx
-        sse_y = (sse((x, y + hy)) - sse_0)/hy
-        return r*(a*sse_x - b*sse_y)/(a*sse_y + b*sse_x)
-
-    theta_span = (0, 2*np.pi)
-    sol = solve_ivp(rdot, theta_span, [r0],
-                    t_eval=np.linspace(*theta_span, npoints),
-                    method='RK45',
-                    atol=0., rtol=rtol)
+        f_s = (f(s + h, q) - f(s - h, q))/h
+        f_q = (f(s, q + h) - f(s, q - h))/h
+        ydot = np.empty_like(y)
+        ydot[0] = -f_q
+        ydot[1] = f_s
+        return ydot
+
+    # Stop the trajectory after one revolution
+    def event(t: float, y: np.ndarray) -> float:
+        return y[1] - 2*np.pi
+    event.terminal = True
+
+    sol = solve_ivp(dydt, (0., 1e10), (log(r0), 0.),
+                    method='LSODA',
+                    events=event,
+                    atol=[0, 1*rtol], rtol=rtol)
     if not sol.success:
         raise ODESolverError(sol.message)
     else:
-        theta = sol.t
-        r = sol.y[0, :]
-        if not np.isclose(r[0], r[-1], atol=0, rtol=10*rtol):
+        r = exp(sol.y[0, :])
+        theta = sol.y[1, :]
+        if not np.isclose(r[0], r[-1], atol=min(*center), rtol=10*rtol):
             print("Warning: offset between start and end positions of JCR > 10*rtol.")
 
-    # Convert to cartesian coordinates and plot
+    # Convert to cartesian coordinates
     x = center[0] + r*cos(theta)
     y = center[1] + r*sin(theta)
-    ax.plot(x, y, color=color, label=label)
-    ax.scatter(*center, c=color, s=5)
 
-    return None
+    return (x, y)
```

### Comparing `polykin-0.5.0/src/polykin/properties/diffusion/liquid.py` & `polykin-0.5.1/src/polykin/properties/diffusion/liquid.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # PolyKin: A polymerization kinetics library for Python.
 #
 # Copyright Hugo Vale 2023
 
-"""This module implements methods to estimate the binary diffusion
-coefficient in liquid solutions.
-"""
-
 from math import sqrt
 from typing import Literal
 
 __all__ = ['DL_Wilke_Chang',
            'DL_Hayduk_Minhas',
            ]
```

### Comparing `polykin-0.5.0/src/polykin/properties/diffusion/vapor.py` & `polykin-0.5.1/src/polykin/properties/diffusion/vapor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # PolyKin: A polymerization kinetics library for Python.
 #
 # Copyright Hugo Vale 2023
 
-"""This module implements methods to estimate the binary diffusion
-coefficient in gas solutions.
-"""
-
 from typing import Optional
 
 from numpy import exp, sqrt
 
 __all__ = ['DV_Wilke_Lee']
```

### Comparing `polykin-0.5.0/src/polykin/properties/diffusion/vrentasduda.py` & `polykin-0.5.1/src/polykin/properties/diffusion/vrentasduda.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,18 +59,18 @@
     D0 : float
         Pre-exponential factor.
         Unit = L²/T.
     E : float
         Activation energy required to overcome the atractive forces
         between neighboring molecules.
         Units = J/mol/K.
-    V1star : float
+    v1star : float
         Specific volume of solvent at 0 K.
         Unit = L³/M.
-    V2star : float
+    v2star : float
         Specific volume of polymer at 0 K.
         Unit = L³/M.
     z : float
         Ratio between the critical volume of the polymer and the
         solvent jumping units, $\xi$.
     K11 : float
         Free-volume parameter of solvent.
@@ -102,15 +102,15 @@
     Examples
     --------
     Estimate the mutual and self-diffusion coefficient of toluene in
     polyvinylacetate at 20 wt% toluene and 25°C.
 
     >>> from polykin.properties.diffusion import VrentasDudaBinary
     >>> d = VrentasDudaBinary(
-    ...     D0=4.82e-4, E=0., V1star=0.917, V2star=0.728, z=0.82,
+    ...     D0=4.82e-4, E=0., v1star=0.917, v2star=0.728, z=0.82,
     ...     K11=1.45e-3, K12=4.33e-4, K21=-86.32, K22=-258.2, X=0.5,
     ...     unit='cm²/s',
     ...     name='Tol(1)/PVAc(2)')
 
     >>> D = d(0.2, 25., Tunit='C')
     >>> print(f"D = {D:.2e} {d.unit}")
     D = 3.79e-08 cm²/s
@@ -119,64 +119,63 @@
     >>> print(f"D1 = {D1:.2e} {d.unit}")
     D1 = 7.40e-08 cm²/s
 
     """  # noqa: E501
 
     D0: float
     E: float
-    V1star: float
-    V2star: float
+    v1star: float
+    v2star: float
     z: float
     K11: float
     K12: float
     K21: float
     K22: float
     Tg1: float
     Tg2: float
     y: float
     X: float
     unit: str
 
     def __init__(self,
                  D0: float,
                  E: float,
-                 V1star: float,
-                 V2star: float,
+                 v1star: float,
+                 v2star: float,
                  z: float,
                  K11: float,
                  K12: float,
                  K21: float,
                  K22: float,
                  Tg1: float = 0.,
                  Tg2: float = 0.,
                  y: float = 1.,
                  X: float = 0.5,
                  unit: str = 'm²/s',
                  name: str = ''
                  ) -> None:
-        r"""Construct `VrentasDuda` with the given parameters."""
 
         check_bounds(D0, 0., np.inf, 'D0')
         check_bounds(E, 0., np.inf, 'E')
-        check_bounds(V1star, 0., np.inf, 'V1star')
-        check_bounds(V2star, 0., np.inf, 'V2star')
+        check_bounds(v1star, 0., np.inf, 'v1star')
+        check_bounds(v2star, 0., np.inf, 'v2star')
         check_bounds(z, 0., np.inf, 'z')
         check_bounds(K11, 0., np.inf, 'K11')
         check_bounds(K12, 0., np.inf, 'K12')
         check_bounds(K21, -np.inf, np.inf, 'K21')
         check_bounds(K22, -np.inf, np.inf, 'K22')
         check_bounds(Tg1, 0., np.inf, 'Tg1')
         check_bounds(Tg2, 0., np.inf, 'Tg2')
         check_bounds(y, 0.5, 1., 'y')
         check_bounds(X, -10, 10, 'X')
 
         self.D0 = D0
         self.E = E
-        self.V1star = V1star
-        self.V2star = V2star
+        self.v1star = v1star
+        self.v2star = v2star
         self.z = z
         self.K11 = K11
         self.K12 = K12
         self.K21 = K21
         self.K22 = K22
         self.Tg1 = Tg1
         self.Tg2 = Tg2
@@ -187,16 +186,16 @@
 
     def __repr__(self) -> str:
         return (
             f"name: {self.name}\n"
             f"unit: {self.unit}\n"
             f"D0:   {self.D0}\n"
             f"E:    {self.E}\n"
-            f"V1*:  {self.V1star}\n"
-            f"V2*:  {self.V2star}\n"
+            f"v1*:  {self.v1star}\n"
+            f"v2*:  {self.v2star}\n"
             f"ξ:    {self.z}\n"
             f"K11:  {self.K11}\n"
             f"K12:  {self.K12}\n"
             f"K21:  {self.K21}\n"
             f"K22:  {self.K22}\n"
             f"Tg1:  {self.Tg1}\n"
             f"Tg2:  {self.Tg2}\n"
@@ -264,16 +263,16 @@
         -------
         float | FloatArray
             Solvent self-diffusion coefficient, $D_1$.
         """
 
         D0 = self.D0
         E = self.E
-        V1star = self.V1star
-        V2star = self.V2star
+        V1star = self.v1star
+        V2star = self.v2star
         z = self.z
         K11 = self.K11
         K12 = self.K12
         K21 = self.K21
         K22 = self.K22
         Tg1 = self.Tg1
         Tg2 = self.Tg2
```

### Comparing `polykin-0.5.0/src/polykin/properties/equations/base.py` & `polykin-0.5.1/src/polykin/properties/equations/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     symbol: str
 
     def __init__(self,
                  unit: str,
                  symbol: str,
                  name: str
                  ) -> None:
-        """Construct `PropertyEquation` with the given inputs."""
+
         self.unit = unit
         self.symbol = symbol
         self.name = name
 
 
 class PropertyEquationT(PropertyEquation):
     r"""_Abstract_ temperature-dependent property equation, $Y(T)$"""
@@ -46,15 +46,14 @@
     def __init__(self,
                  Trange: tuple[Union[float, FloatArray],
                                Union[float, FloatArray]],
                  unit: str,
                  symbol: str,
                  name: str
                  ) -> None:
-        """Construct `PropertyEquationT` with the given inputs."""
 
         check_bounds(Trange[0], 0, np.inf, 'Tmin')
         check_bounds(Trange[1], 0, np.inf, 'Tmax')
         check_bounds(Trange[1]-Trange[0], eps, np.inf, 'Tmax-Tmin')
         self.Trange = Trange
         super().__init__(unit, symbol, name)
```

### Comparing `polykin-0.5.0/src/polykin/properties/equations/dippr.py` & `polykin-0.5.1/src/polykin/properties/equations/dippr.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/properties/equations/vapor_pressure.py` & `polykin-0.5.1/src/polykin/properties/equations/vapor_pressure.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,15 +77,14 @@
                  base10: bool = True,
                  Tmin: float = 0.0,
                  Tmax: float = np.inf,
                  unit: str = 'Pa',
                  symbol: str = 'P^*',
                  name: str = ''
                  ) -> None:
-        """Construct `Antoine` with the given parameters."""
 
         self.p = {'A': A, 'B': B, 'C': C, 'base10': base10}
         super().__init__((Tmin, Tmax), unit, symbol, name)
 
     @staticmethod
     def equation(T: Union[float, FloatArray],
                  A: float,
@@ -188,15 +187,14 @@
                  Tc: float,
                  Tmin: float = 0.0,
                  Tmax: float = np.inf,
                  unit: str = 'Pa',
                  symbol: str = 'P^*',
                  name: str = ''
                  ) -> None:
-        """Construct `Wagner` with the given parameters."""
 
         self.p = {'a': a, 'b': b, 'c': c, 'd': d, 'Pc': Pc, 'Tc': Tc}
         super().__init__((Tmin, Tmax), unit, symbol, name)
 
     @staticmethod
     def equation(T: Union[float, FloatArray],
                  a: float,
```

### Comparing `polykin-0.5.0/src/polykin/properties/equations/viscosity.py` & `polykin-0.5.1/src/polykin/properties/equations/viscosity.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/properties/mixing_rules.py` & `polykin-0.5.1/src/polykin/properties/mixing_rules.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/properties/pvt_polymer/Flory_parameters.tsv` & `polykin-0.5.1/src/polykin/properties/pvt_polymer/Flory_parameters.tsv`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/properties/pvt_polymer/HartmannHaque_parameters.tsv` & `polykin-0.5.1/src/polykin/properties/pvt_polymer/HartmannHaque_parameters.tsv`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/properties/pvt_polymer/SanchezLacombe_parameters.tsv` & `polykin-0.5.1/src/polykin/properties/pvt_polymer/SanchezLacombe_parameters.tsv`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/properties/pvt_polymer/Tait_parameters.tsv` & `polykin-0.5.1/src/polykin/properties/pvt_polymer/Tait_parameters.tsv`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/properties/pvt_polymer/base.py` & `polykin-0.5.1/src/polykin/properties/pvt_polymer/base.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/properties/pvt_polymer/eos.py` & `polykin-0.5.1/src/polykin/properties/pvt_polymer/eos.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
                  P0: float,
                  Tmin: float = 0.0,
                  Tmax: float = np.inf,
                  Pmin: float = 0.0,
                  Pmax: float = np.inf,
                  name: str = ''
                  ) -> None:
-        """Construct `PolymerEoSReduced` with the given parameters."""
 
         # Check bounds
         check_bounds(V0, 0, np.inf, 'V0')
         check_bounds(T0, 0, np.inf, 'T0')
         check_bounds(P0, 0, np.inf, 'P0')
 
         self.V0 = V0
```

### Comparing `polykin-0.5.0/src/polykin/properties/pvt_polymer/tait.py` & `polykin-0.5.1/src/polykin/properties/pvt_polymer/tait.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/properties/thermal_conductivity/liquid.py` & `polykin-0.5.1/src/polykin/properties/thermal_conductivity/liquid.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,17 +16,18 @@
              k: FloatVectorLike,
              rho: FloatVectorLike,
              ) -> float:
     r"""Calculate the thermal conductivity of a liquid mixture from the
     thermal conductivities of the pure components using the Li mixing rule.
 
     $$ \begin{aligned}
-        k_m &= \sum_i \sum_j \phi_i \phi_j k_{ij} \\
+        k_m &= \sum_{i=1}^N \sum_{j=1}^N \phi_i \phi_j k_{ij} \\
         k_{ij} &= \frac{2}{\frac{1}{k_i} + \frac{1}{k_j}} \\
-       \phi_i &= \frac{\frac{w_i}{\rho_i}}{\sum_j \frac{w_j}{\rho_j}}
+        \phi_i &= \frac{\frac{w_i}{\rho_i}}
+                       {\sum_{j=1}^N \frac{w_j}{\rho_j}}
     \end{aligned} $$
 
     !!! note
 
         In this equation, the units of mass fraction $w_i$ and density $\rho_i$
         are arbitrary, as they cancel out when considering the ratio of the
         numerator to the denominator.
```

### Comparing `polykin-0.5.0/src/polykin/properties/thermal_conductivity/vapor.py` & `polykin-0.5.1/src/polykin/properties/thermal_conductivity/vapor.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,15 +191,16 @@
                       k: FloatVectorLike,
                       M: FloatVectorLike
                       ) -> float:
     r"""Calculate the thermal conductivity of a gas mixture from the thermal
     conductivities of the pure components using the mixing rule of Wassilijewa,
     with the simplification of Herning and Zipperer.
 
-    $$ k_m = \frac{\sum _i y_i M_i^{1/2} k_i}{\sum _i y_i M_i^{1/2}} $$
+    $$ k_m = \frac{\displaystyle \sum_{i=1}^N y_i M_i^{1/2} k_i}
+                  {\displaystyle \sum_{i=1}^N y_i M_i^{1/2}} $$
 
     !!! note
 
         In this equation, the units of mole fraction $y_i$ and molar mass
         $M_i$ are arbitrary, as they cancel out when considering the ratio of
         the numerator to the denominator.
```

### Comparing `polykin-0.5.0/src/polykin/properties/vaporization_enthalpy.py` & `polykin-0.5.1/src/polykin/properties/vaporization_enthalpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 # PolyKin: A polymerization kinetics library for Python.
 #
-# Copyright Hugo Vale 2023
+# Copyright Hugo Vale 2024
 
-""" This module provides correlations to estimate the enthalpy of vaporization
-of pure components.
-"""
 
 from typing import Literal, Optional, Union
 
 import numpy as np
-
 from numpy import log, log10
 from scipy.constants import R
 
 from polykin.utils.types import FloatArray, FloatArrayLike
 
 __all__ = ['DHVL_Pitzer',
            'DHVL_Vetere',
```

### Comparing `polykin-0.5.0/src/polykin/properties/viscosity/liquid.py` & `polykin-0.5.1/src/polykin/properties/viscosity/liquid.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,19 +17,19 @@
                  hydrocarbons: bool = False,
                  ) -> float:
     r"""Calculate the viscosity of a liquid mixture from the viscosities of the
     pure components using the mixing rules recommended in Perry's.
 
     For hydrocarbon mixtures:
 
-    $$ \mu_m = \left ( \sum_i x_i \mu_i^{1/3} \right )^3 $$
+    $$ \mu_m = \left ( \sum_{i=1}^N x_i \mu_i^{1/3} \right )^3 $$
 
     and for nonhydrocarbon mixtures:
 
-    $$ \ln{\mu_m} = \sum_i x_i \ln{\mu_i} $$
+    $$ \ln{\mu_m} = \sum_{i=1}^N x_i \ln{\mu_i} $$
 
     **References**
 
     *   Perry, R. H., D. W. Green, and J. Maloney. Perrys Chemical Engineers
         Handbook, 7th ed. 1999, p. 2-367.
 
     Parameters
```

### Comparing `polykin-0.5.0/src/polykin/properties/viscosity/vapor.py` & `polykin-0.5.1/src/polykin/properties/viscosity/vapor.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,16 @@
                             mu: FloatVectorLike,
                             M: FloatVectorLike
                             ) -> float:
     r"""Calculate the viscosity of a gas mixture from the viscosities of the
     pure components using the mixing rule of Wilke with the approximation of
     Herning and Zipperer.
 
-    $$ \mu_m = \frac{\sum _i y_i M_i^{1/2} \mu_i}{\sum _i y_i M_i^{1/2}} $$
+    $$ \mu_m = \frac{\displaystyle \sum_{i=1}^N y_i M_i^{1/2} \mu_i}
+                    {\displaystyle \sum_{i=1}^N y_i M_i^{1/2}} $$
 
     !!! note
 
         In this equation, the units of mole fraction $y_i$ and molar mass
         $M_i$ are arbitrary, as they cancel out when considering the ratio of
         the numerator to the denominator.
```

### Comparing `polykin-0.5.0/src/polykin/stepgrowth/solutions.py` & `polykin-0.5.1/src/polykin/stepgrowth/solutions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PolyKin: A polymerization kinetics library for Python.
 #
-# Copyright Hugo Vale 2023
+# Copyright Hugo Vale 2024
 
 
 from typing import Union
 
 import numpy as np
 from numpy import dot, sqrt
```

### Comparing `polykin-0.5.0/src/polykin/thermo/acm/floryhuggins.py` & `polykin-0.5.1/src/polykin/thermo/acm/floryhuggins.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from polykin.utils.tools import check_bounds
 from polykin.utils.types import (FloatArray, FloatSquareMatrix, FloatVector,
                                  Number)
 
 # from .base import ActivityCoefficientModel
 
 __all__ = ['FloryHuggins',
-           'FloryHuggins_a',
-           'FloryHuggins2_a']
+           'FloryHuggins_activity',
+           'FloryHuggins2_activity']
 
 
 class FloryHuggins():
     r"""[Flory-Huggings](https://en.wikipedia.org/wiki/Flory–Huggins_solution_theory)
     multicomponent activity coefficient model.
 
     This model is based on the following Gibbs energy of mixing per mole of
@@ -50,27 +50,27 @@
     *   P.J. Flory, Principles of polymer chemistry, 1953.
 
     Parameters
     ----------
     N : int
         Number of components.
     a : FloatSquareMatrix | None
-        Matrix (NxN) of parameters, by default 0. Only the upper triangle must
+        Matrix (N,N) of parameters, by default 0. Only the upper triangle must
         be supplied.
     b : FloatSquareMatrix | None
-        Matrix (NxN) of parameters, by default 0. Only the upper triangle must
+        Matrix (N,N) of parameters, by default 0. Only the upper triangle must
         be supplied.
     c : FloatSquareMatrix | None
-        Matrix (NxN) of parameters, by default 0. Only the upper triangle must
+        Matrix (N,N) of parameters, by default 0. Only the upper triangle must
         be supplied.
     d : FloatSquareMatrix | None
-        Matrix (NxN) of parameters, by default 0. Only the upper triangle must
+        Matrix (N,N) of parameters, by default 0. Only the upper triangle must
         be supplied.
     e : FloatSquareMatrix | None
-        Matrix (NxN) of parameters, by default 0. Only the upper triangle must
+        Matrix (N,N) of parameters, by default 0. Only the upper triangle must
         be supplied.
 
     """
 
     _N: int
     _a: FloatSquareMatrix
     _b: FloatSquareMatrix
@@ -244,21 +244,21 @@
             for polymers.
 
         Returns
         -------
         FloatVector
             Activities of all components.
         """
-        return FloryHuggins_a(phi, m, self.chi(T))
+        return FloryHuggins_activity(phi, m, self.chi(T))
 
 
-def FloryHuggins_a(phi: FloatVector,
-                   m: FloatVector,
-                   chi: FloatSquareMatrix
-                   ) -> FloatVector:
+def FloryHuggins_activity(phi: FloatVector,
+                          m: FloatVector,
+                          chi: FloatSquareMatrix
+                          ) -> FloatVector:
     r"""Calculate the activities of a multicomponent mixture according to the
     Flory-Huggins model.
 
     $$ 
     \ln{a_i} = \ln{\phi_i} + 1 - m_i \left(\sum_j \frac{\phi_j}{m_j} - 
     \sum_j \phi_j \chi_{ij} + \sum_j \sum_{k>j} \phi_j \phi_k \chi_{jk} \right)
     $$
@@ -291,37 +291,37 @@
         composition variable must match the one used in the determination of
         $\chi_{ij}$.
     m : FloatVector
         Characteristic size of all components, typically equal to 1 for small
         molecules and equal to the average degree of polymerization for
         polymers.
     chi : FloatSquareMatrix
-        Matrix (NxN) of interaction parameters, $\chi_{ij}$. It is expected
+        Matrix (N,N) of interaction parameters, $\chi_{ij}$. It is expected
         (but not checked) that $\chi_{ij}=\chi_{ji}$ and $\chi_{ii}=0$.
 
     Returns
     -------
     FloatVector
         Activities of all components.
 
     !!! note annotate "See also"
 
-        * [`FloryHuggins2_a`](FloryHuggins2_a.md): equivalent method for
-          binary solvent-polymer systems.
+        * [`FloryHuggins2_activity`](FloryHuggins2_activity.md): equivalent
+        method for binary solvent-polymer systems.
     """
     A = dot(phi, 1/m)
     B = dot(chi, phi)
     C = 0.5*dot(phi, dot(phi, chi))
     return phi*exp(1 - m*(A - B + C))
 
 
-def FloryHuggins2_a(phi1: Union[float, FloatArray],
-                    m: Union[float, FloatArray],
-                    chi: Union[float, FloatArray]
-                    ) -> Union[float, FloatArray]:
+def FloryHuggins2_activity(phi1: Union[float, FloatArray],
+                           m: Union[float, FloatArray],
+                           chi: Union[float, FloatArray]
+                           ) -> Union[float, FloatArray]:
     r"""Calculate the solvent activity of a binary polymer solution according
     to the Flory-Huggins model.
 
     $$ \ln{a_1} = \ln \phi_1 + \left(\ 1 - \frac{1}{m} \right)(1-\phi_1)
                   + \chi_{12}(1-\phi_1)^2 $$
 
     where $\phi_1$ is the volume, mass or segment fraction of the solvent in
@@ -359,16 +359,16 @@
     Returns
     -------
     FloatVector
         Activity of the solvent.
 
     !!! note annotate "See also"
 
-        * [`FloryHuggins_a`](FloryHuggins_a.md): equivalent method for
-          multicomponent systems.
+        * [`FloryHuggins_activity`](FloryHuggins_activity.md): equivalent
+        method for multicomponent systems.
 
     Examples
     --------
     Calculate the activity of ethylbenzene in a ethylbenzene-polybutadiene
     solution with 25 wt% solvent content. Assume $\chi=0.29$.
     >>> from polykin.thermo.acm import FloryHuggins2_gamma
     >>> gamma = FloryHuggins2_gamma(phi1=0.25, m=1e6, chi=0.29)
```

### Comparing `polykin-0.5.0/src/polykin/thermo/acm/ideal.py` & `polykin-0.5.1/src/polykin/thermo/eos/idealgas.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,88 @@
 # PolyKin: A polymerization kinetics library for Python.
 #
-# Copyright Hugo Vale 2024
+# Copyright Hugo Vale 2023
 
-import numpy as np
+from typing import Union
 
-from polykin.utils.types import FloatVector
+import numpy as np
+from numpy import log
+from scipy.constants import R
 
-from .base import ACM
+from polykin.utils.types import FloatArray, FloatVector
 
-__all__ = ['IdealSolution']
+from .base import GasEoS
 
+__all__ = ['IdealGas']
 
-class IdealSolution(ACM):
-    r"""[Ideal solution](https://en.wikipedia.org/wiki/Ideal_solution) model.
 
-    This model is based on the following trivial molar excess Gibbs energy
-    expression:
+class IdealGas(GasEoS):
+    r"""Ideal gas equation of state.
 
-    $$ g^{E} = 0 $$
+    This EOS is based on the following $P(v,T)$ relationship:
 
-    Parameters
-    ----------
-    N : int
-        Number of components.
+    $$ P = \frac{R T}{v} $$
 
-    """
+    where $P$ is the pressure, $T$ is the temperature, and $v$ is the molar
+    volume.
 
-    def __init__(self,
-                 N: int
-                 ) -> None:
-        """Construct `IdealSolution`."""
-        super().__init__(N)
+    !!! important
 
-    def gE(self, T: float, x: FloatVector) -> float:
-        r"""Molar excess Gibbs energy, $g^{E}$.
+        The ideal gas model is very convenient, but its validity is limited to
+        low pressures and high temperatures.
+    """
 
-        Parameters
-        ----------
-        T : float
-            Temperature. Unit = K.
-        x : FloatVector
-            Mole fractions of all components. Unit = mol/mol.
+    def Z(self,
+          T=None,
+          P=None,
+          y=None):
+        r"""Calculate the compressibility factor of the fluid.
 
         Returns
         -------
         float
-            Molar excess Gibbs energy. Unit = J/mol.
+            Compressibility factor of the vapor.
         """
-        return 0.
+        return 1.
 
-    def gamma(self, T: float, x: FloatVector) -> FloatVector:
-        r"""Activity coefficients, $\gamma_i$.
-
-        $$ \gamma_i = 1 $$
+    def P(self,
+          T: Union[float, FloatArray],
+          v: Union[float, FloatArray],
+          y=None
+          ) -> Union[float, FloatArray]:
+        r"""Calculate the pressure of the fluid.
 
         Parameters
         ----------
-        T : float
+        T : float | FloatArray
             Temperature. Unit = K.
-        x : FloatVector
-            Mole fractions of all components. Unit = mol/mol.
+        v : float | FloatArray
+            Molar volume. Unit = m³/mol.
+
+        Returns
+        -------
+        float | FloatArray
+             Pressure. Unit = Pa.
+        """
+        return R*T/v
+
+    def phiV(self,
+             T=None,
+             P=None,
+             y=None
+             ) -> FloatVector:
+        r"""Calculate the fugacity coefficients of all components in the vapor
+        phase.
 
         Returns
         -------
         FloatVector
-            Activity coefficients of all components.
+            Fugacity coefficients of all components.
         """
-        return np.ones_like(x)
+        if y is None:
+            return np.array([1.])
+        else:
+            return np.ones_like(y)
+
+    def DA(self, T, V, n, v0):
+        nT = n.sum()
+        return -nT*R*T*log(V/(nT*v0))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `polykin-0.5.0/src/polykin/thermo/acm/nrtl.py` & `polykin-0.5.1/src/polykin/thermo/acm/nrtl.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 from scipy.constants import gas_constant as R
 
 from polykin.utils.exceptions import ShapeError
 from polykin.utils.math import enforce_symmetry
 from polykin.utils.tools import check_bounds
 from polykin.utils.types import FloatSquareMatrix, FloatVector
 
-from .base import ACM
+from .base import SmallSpeciesActivityModel
 
 __all__ = ['NRTL', 'NRTL_gamma']
 
 
-class NRTL(ACM):
+class NRTL(SmallSpeciesActivityModel):
     r"""[NRTL](https://en.wikipedia.org/wiki/Non-random_two-liquid_model)
     multicomponent activity coefficient model.
 
     This model is based on the following molar excess Gibbs energy
     expression:
 
     $$ \frac{g^{E}}{RT} = 
         \sum_i x_i \frac{\displaystyle\sum_j x_j \tau_{ji} G_{ji}}
         {\displaystyle\sum_j x_j G_{ji}} $$
 
-    where $x_i$ are the mole fractions, $\tau_{ij}$ are the dimensionless
-    interaction parameters, $\alpha_{ij}$ are the non-randomness parameters,
-    and $G_{ij}=\exp(-\alpha_{ij} \tau_{ij})$. 
+    where $x_i$ are the mole fractions, $\tau_{ij}$ are the interaction
+    parameters, $\alpha_{ij}$ are the non-randomness parameters, and
+    $G_{ij}=\exp(-\alpha_{ij} \tau_{ij})$. 
 
     In this particular implementation, the model parameters are allowed to
     depend on temperature according to the following empirical relationship
     (as done in Aspen Plus):
 
     \begin{aligned}
     \tau_{ij} &= a_{ij} + b_{ij}/T + e_{ij} \ln{T} + f_{ij} T \\
@@ -52,28 +52,30 @@
         thermodynamic excess functions for liquid mixtures. AIChE J.,
         14: 135-144.
 
     Parameters
     ----------
     N : int
         Number of components.
-    a : FloatSquareMatrix | None
-        Matrix (NxN) of parameters, by default 0.
-    b : FloatSquareMatrix | None
-        Matrix (NxN) of parameters, by default 0.
-    c : FloatSquareMatrix | None
-        Matrix (NxN) of parameters, by default 0.3. Only the upper triangle
-        must be supplied.
-    d : FloatSquareMatrix | None
-        Matrix (NxN) of parameters, by default 0. Only the upper triangle
-        must be supplied.
-    e : FloatSquareMatrix | None
-        Matrix (NxN) of parameters, by default 0.
-    f : FloatSquareMatrix | None
-        Matrix (NxN) of parameters, by default 0.
+    a : FloatSquareMatrix (N,N) | None
+        Matrix of interaction parameters, by default 0.
+    b : FloatSquareMatrix (N,N) | None
+        Matrix of interaction parameters, by default 0. Unit = K.
+    c : FloatSquareMatrix (N,N) | None
+        Matrix of interaction parameters, by default 0.3. Only the upper
+        triangle must be supplied.
+    d : FloatSquareMatrix (N,N) | None
+        Matrix of interaction parameters, by default 0. Only the upper triangle
+        must be supplied. Unit = 1/K.
+    e : FloatSquareMatrix (N,N) | None
+        Matrix of interaction parameters, by default 0.
+    f : FloatSquareMatrix (N,N) | None
+        Matrix of interaction parameters, by default 0.
+    name: str
+        Name.
 
     !!! note annotate "See also"
 
         * [`NRTL_gamma`](NRTL_gamma.md): related activity coefficient method.
 
     """
 
@@ -87,17 +89,17 @@
     def __init__(self,
                  N: int,
                  a: Optional[FloatSquareMatrix] = None,
                  b: Optional[FloatSquareMatrix] = None,
                  c: Optional[FloatSquareMatrix] = None,
                  d: Optional[FloatSquareMatrix] = None,
                  e: Optional[FloatSquareMatrix] = None,
-                 f: Optional[FloatSquareMatrix] = None
+                 f: Optional[FloatSquareMatrix] = None,
+                 name: str = ''
                  ) -> None:
-        """Construct `NRTL` with the given parameters."""
 
         # Set default values
         if a is None:
             a = np.zeros((N, N))
         if b is None:
             b = np.zeros((N, N))
         if c is None:
@@ -126,95 +128,71 @@
             np.fill_diagonal(array, 0.)
 
         # Ensure alpha_ij=alpha_ji
         for array in [c, d]:
             np.fill_diagonal(array, 0.)
             enforce_symmetry(array)
 
-        super().__init__(N)
+        super().__init__(N, name)
         self._a = a
         self._b = b
         self._c = c
         self._d = d
         self._e = e
         self._f = f
 
     @functools.cache
-    def alpha(self, T: float) -> FloatSquareMatrix:
+    def alpha(self,
+              T: float
+              ) -> FloatSquareMatrix:
         r"""Compute matrix of non-randomness parameters.
 
         $$ \alpha_{ij} = c_{ij} + d_{ij}(T - 273.15) $$
 
         Parameters
         ----------
         T : float
             Temperature. Unit = K.
 
         Returns
         -------
-        FloatSquareMatrix
-            Matrix of non-randomness parameters.
+        FloatSquareMatrix (N,N)
+            Non-randomness parameters.
         """
         return self._c + self._d*(T - 273.15)
 
     @functools.cache
-    def tau(self, T: float) -> FloatSquareMatrix:
-        r"""Compute the matrix of dimensionless interaction parameters.
+    def tau(self,
+            T: float
+            ) -> FloatSquareMatrix:
+        r"""Compute the matrix of interaction parameters.
 
         $$ \tau_{ij} = a_{ij} + b_{ij}/T + e_{ij} \ln{T} + f_{ij} T $$
 
         Parameters
         ----------
         T : float
             Temperature. Unit = K.
 
         Returns
         -------
-        FloatSquareMatrix
-            Matrix of dimensionless interaction parameters.
+        FloatSquareMatrix (N,N)
+            Interaction parameters.
         """
         return self._a + self._b/T + self._e*log(T) + self._f*T
 
     def gE(self, T: float, x: FloatVector) -> float:
-        r"""Molar excess Gibbs energy, $g^{E}$.
-
-        Parameters
-        ----------
-        x : FloatVector
-            Mole fractions of all components. Unit = mol/mol.
-        T : float
-            Temperature. Unit = K.
-
-        Returns
-        -------
-        float
-            Molar excess Gibbs energy. Unit = J/mol.
-        """
         tau = self.tau(T)
         alpha = self.alpha(T)
         G = exp(-alpha*tau)
         A = dot(x, tau*G)
         B = dot(x, G)
         return R*T*dot(x, A/B)
 
     def gamma(self, T: float, x: FloatVector) -> FloatVector:
-        r"""Activity coefficients, $\gamma_i$.
-
-        Parameters
-        ----------
-        T : float
-            Temperature. Unit = K.
-        x : FloatVector
-            Mole fractions of all components. Unit = mol/mol.
-
-        Returns
-        -------
-        FloatVector
-            Activity coefficients of all components.
-        """
         return NRTL_gamma(x, self.tau(T), self.alpha(T))
 
 
 def NRTL_gamma(x: FloatVector,
                tau: FloatSquareMatrix,
                alpha: FloatSquareMatrix
                ) -> FloatVector:
@@ -223,38 +201,38 @@
 
     $$ \ln{\gamma_i} = \frac{\displaystyle\sum_{k}{x_{k}\tau_{ki}G_{ki}}}
     {\displaystyle\sum_{k}{x_{k}G_{ki}}}
     +\sum_{j}{\frac{x_{j}G_{ij}}{\displaystyle\sum_{k}{x_{k}G_{kj}}}}
     {\left ({\tau_{ij}-\frac{\displaystyle\sum_{k}{x_{k}\tau_{kj}G_{kj}}}
     {\displaystyle\sum_{k}{x_{k}G_{kj}}}}\right )} $$
 
-    where $x_i$ are the mole fractions, $\tau_{ij}$ are the dimensionless
-    interaction parameters, $\alpha_{ij}$ are the non-randomness parameters,
-    and $G_{ij}=\exp(-\alpha_{ij} \tau_{ij})$.
+    where $x_i$ are the mole fractions, $\tau_{ij}$ are the interaction
+    parameters, $\alpha_{ij}$ are the non-randomness parameters, and 
+    $G_{ij}=\exp(-\alpha_{ij} \tau_{ij})$.
 
     **References**
 
     *   Renon, H. and Prausnitz, J.M. (1968), Local compositions in
         thermodynamic excess functions for liquid mixtures. AIChE J.,
         14: 135-144.
 
     Parameters
     ----------
-    x : FloatVector
+    x : FloatVector (N)
         Mole fractions of all components. Unit = mol/mol.
-    tau : FloatSquareMatrix
-        Matrix (NxN) of dimensionless interaction parameters, $\tau_{ij}$. It
-        is expected (but not checked) that $\tau_{ii}=0$.
-    alpha : FloatSquareMatrix
-        Matrix (NxN) of non-randomness parameters, $\alpha_{ij}$. It is
-        expected (but not checked) that $\alpha_{ij}=\alpha_{ji}$.
+    tau : FloatSquareMatrix (N,N)
+        Interaction parameters, $\tau_{ij}$. It is expected (but not checked)
+        that $\tau_{ii}=0$.
+    alpha : FloatSquareMatrix (N,N)
+        Non-randomness parameters, $\alpha_{ij}$. It is expected (but not
+        checked) that $\alpha_{ij}=\alpha_{ji}$.
 
     Returns
     -------
-    FloatVector
+    FloatVector (N)
         Activity coefficients of all components.
 
     !!! note annotate "See also"
 
         * [`NRTL`](NRTL.md): related class.
     """
```

### Comparing `polykin-0.5.0/src/polykin/thermo/acm/uniquac.py` & `polykin-0.5.1/src/polykin/thermo/acm/uniquac.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 from numpy import dot, exp, log
 from scipy.constants import gas_constant as R
 
 from polykin.utils.exceptions import ShapeError
 from polykin.utils.tools import check_bounds
 from polykin.utils.types import FloatSquareMatrix, FloatVector, FloatVectorLike
 
-from .base import ACM
+from .base import SmallSpeciesActivityModel
 
 __all__ = ['UNIQUAC', 'UNIQUAC_gamma']
 
 
-class UNIQUAC(ACM):
+class UNIQUAC(SmallSpeciesActivityModel):
     r"""[UNIQUAC](https://en.wikipedia.org/wiki/UNIQUAC) multicomponent
     activity coefficient model.
 
     This model is based on the following molar excess Gibbs energy
     expression:
 
     \begin{aligned}
@@ -56,26 +56,28 @@
         liquid mixtures: A new expression for the excess Gibbs energy of partly
         or completely miscible systems. AIChE J., 21: 116-128.
 
     Parameters
     ----------
     N : int
         Number of components.
-    q : FloatVectorLike
-        Vector (N) of pure-component relative surface areas.
-    r : FloatVectorLike
-        Vector (N) of pure-component relative volumes.
-    a : FloatSquareMatrix | None
-        Matrix (NxN) of parameters, by default 0.
-    b : FloatSquareMatrix | None
-        Matrix (NxN) of parameters, by default 0.
-    c : FloatSquareMatrix | None
-        Matrix (NxN) of parameters, by default 0.
-    d : FloatSquareMatrix | None
-        Matrix (NxN) of parameters, by default 0.
+    q : FloatVectorLike (N)
+        Relative surface areas of all components.
+    r : FloatVectorLike (N)
+        Relative volumes of all components.
+    a : FloatSquareMatrix (N,N) | None
+        Matrix of interaction parameters, by default 0.
+    b : FloatSquareMatrix (N,N) | None
+        Matrix of interaction parameters, by default 0. Unit = K.
+    c : FloatSquareMatrix (N,N) | None
+        Matrix of interaction parameters, by default 0.
+    d : FloatSquareMatrix (N,N) | None
+        Matrix of interaction parameters, by default 0.
+    name : str
+        Name.
 
     !!! note annotate "See also"
 
         * [`UNIQUAC_gamma`](UNIQUAC_gamma.md): related activity coefficient
           method.
 
     """
@@ -90,17 +92,17 @@
     def __init__(self,
                  N: int,
                  q: FloatVectorLike,
                  r: FloatVectorLike,
                  a: Optional[FloatSquareMatrix] = None,
                  b: Optional[FloatSquareMatrix] = None,
                  c: Optional[FloatSquareMatrix] = None,
-                 d: Optional[FloatSquareMatrix] = None
+                 d: Optional[FloatSquareMatrix] = None,
+                 name: str = ''
                  ) -> None:
-        """Construct `UNIQUAC` with the given parameters."""
 
         # Set default values
         if a is None:
             a = np.zeros((N, N))
         if b is None:
             b = np.zeros((N, N))
         if c is None:
@@ -124,84 +126,64 @@
         check_bounds(a, -50., 50., 'a')
         check_bounds(b, -1.5e4, 1.5e4, 'b')
 
         # Ensure tau_ii=1
         for array in [a, b, c, d]:
             np.fill_diagonal(array, 0.)
 
-        super().__init__(N)
+        super().__init__(N, name)
         self._q = q
         self._r = r
         self._a = a
         self._b = b
         self._c = c
         self._d = d
 
     @functools.cache
-    def tau(self, T: float) -> FloatSquareMatrix:
-        r"""Compute the matrix of dimensionless interaction parameters.
+    def tau(self,
+            T: float
+            ) -> FloatSquareMatrix:
+        r"""Compute the matrix of interaction parameters.
 
         $$ \tau_{ij} = \exp( a_{ij} + b_{ij}/T + c_{ij} \ln{T} + d_{ij} T ) $$
 
         Parameters
         ----------
         T : float
             Temperature. Unit = K.
 
         Returns
         -------
-        FloatSquareMatrix
-            Matrix of dimensionless interaction parameters.
+        FloatSquareMatrix (N,N)
+            Interaction parameters.
         """
         return exp(self._a + self._b/T + self._c*log(T) + self._d*T)
 
-    def gE(self, T: float, x: FloatVector) -> float:
-        r"""Molar excess Gibbs energy, $g^{E}$.
-
-        Parameters
-        ----------
-        x : FloatVector
-            Mole fractions of all components. Unit = mol/mol.
-        T : float
-            Temperature. Unit = K.
-
-        Returns
-        -------
-        float
-            Molar excess Gibbs energy. Unit = J/mol.
-        """
+    def gE(self,
+           T: float,
+           x: FloatVector
+           ) -> float:
 
         r = self._r
         q = self._q
         tau = self.tau(T)
 
         phi = x*r/dot(x, r)
         theta = x*q/dot(x, q)
 
         p = x > 0.
         gC = np.sum(x[p]*(log(phi[p]/x[p]) + 5*q[p]*log(theta[p]/phi[p])))
         gR = -np.sum(q[p]*x[p]*log(dot(theta, tau)[p]))
 
         return R*T*(gC + gR)
 
-    def gamma(self, T: float, x: FloatVector) -> FloatVector:
-        r"""Activity coefficients, $\gamma_i$.
-
-        Parameters
-        ----------
-        T : float
-            Temperature. Unit = K.
-        x : FloatVector
-            Mole fractions of all components. Unit = mol/mol.
-
-        Returns
-        -------
-        FloatVector
-            Activity coefficients of all components.
-        """
+    def gamma(self,
+              T: float,
+              x: FloatVector
+              ) -> FloatVector:
         return UNIQUAC_gamma(x, self._q, self._r, self.tau(T))
 
 
 def UNIQUAC_gamma(x: FloatVector,
                   q: FloatVector,
                   r: FloatVector,
                   tau: FloatSquareMatrix
@@ -235,27 +217,27 @@
         liquid mixtures: A new expression for the excess Gibbs energy of partly
         or completely miscible systems. AIChE J., 21: 116-128.
     *   JM Smith, HC Van Ness, MM Abbott. Introduction to chemical engineering
         thermodynamics, 5th edition, 1996, p. 740-741.
 
     Parameters
     ----------
-    x : FloatVector
+    x : FloatVector (N)
         Mole fractions of all components. Unit = mol/mol.
-    q : FloatVector
-        Vector (N) of pure-component relative surface areas.
-    r : FloatVector
-        Vector (N) of pure-component relative volumes.
-    tau : FloatSquareMatrix
-        Matrix (NxN) of dimensionless interaction parameters, $\tau_{ij}$. It
-        is expected (but not checked) that $\tau_{ii}=1$.
+    q : FloatVector (N)
+        Relative surface areas of all components.
+    r : FloatVector (N)
+        Relative volumes of all components. 
+    tau : FloatSquareMatrix (N,N)
+        Interaction parameters, $\tau_{ij}$. It is expected (but not checked)
+        that $\tau_{ii}=1$.
 
     Returns
     -------
-    FloatVector
+    FloatVector (N)
         Activity coefficients of all components.
 
     !!! note annotate "See also"
 
         * [`UNIQUAC`](UNIQUAC.md): related class.
 
     """
```

### Comparing `polykin-0.5.0/src/polykin/thermo/eos/base.py` & `polykin-0.5.1/src/polykin/thermo/eos/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,30 +45,30 @@
             Pressure. Unit = Pa.
         y : FloatVector
             Mole fractions of all components. Unit = mol/mol.
 
         Returns
         -------
         FloatVector
-            Molar volume of the gas and/or liquid phases. Unit = m³/mol.
+            Molar volume of the vapor and/or liquid phases. Unit = m³/mol.
         """
         return self.Z(T, P, y)*R*T/P
 
-    def fv(self,
+    def fV(self,
             T: float,
             P: float,
             y: FloatVector
            ) -> FloatVector:
-        r"""Calculate the fugacity of all components in the gas phase.
+        r"""Calculate the fugacity of all components in the vapor phase.
 
         $$ \hat{f}_i = \hat{\phi}_i y_i P $$
 
-        $\hat{f}_i$ is the fugacity in the gas phase, $\hat{\phi}_i(T,P,y)$ is
-        the fugacity coefficient, $P$ is the pressure, and $y_i$ is the mole
-        fraction in the gas phase.
+        $\hat{f}_i$ is the fugacity in the vapor phase, $\hat{\phi}_i(T,P,y)$
+        is the fugacity coefficient, $P$ is the pressure, and $y_i$ is the mole
+        fraction in the vapor phase.
 
         Parameters
         ----------
         T : float
             Temperature. Unit = K.
         P : float
             Pressure. Unit = Pa.
@@ -76,15 +76,15 @@
             Mole fractions of all components. Unit = mol/mol.
 
         Returns
         -------
         FloatVector
             Fugacity coefficients of all components.
         """
-        return self.phi(T, P, y)*y*P
+        return self.phiV(T, P, y)*y*P
 
     @abstractmethod
     def P(self,
           T: float,
           v: float,
           y: FloatVector
           ) -> float:
@@ -135,15 +135,15 @@
             Pressure. Unit = Pa.
         y : FloatVector
             Mole fractions of all components. Unit = mol/mol.
 
         Returns
         -------
         FloatVector
-            Compressibility factor of the gas and/or liquid phases.
+            Compressibility factor of the vapor and/or liquid phases.
         """
         pass
 
     @abstractmethod
     def DA(self,
            T: float,
            V: float,
@@ -170,20 +170,20 @@
         -------
         FloatVector
             Helmholtz energy departure, $A - A^{\circ}$. Unit = J.
         """
         pass
 
     @abstractmethod
-    def phi(self,
-            T: float,
-            P: float,
-            y: FloatVector
-            ) -> FloatVector:
-        r"""Calculate the fugacity coefficients of all components in the gas
+    def phiV(self,
+             T: float,
+             P: float,
+             y: FloatVector
+             ) -> FloatVector:
+        r"""Calculate the fugacity coefficients of all components in the vapor
         phase.
 
         Parameters
         ----------
         T : float
             Temperature. Unit = K.
         P : float
```

### Comparing `polykin-0.5.0/src/polykin/thermo/eos/cubic.py` & `polykin-0.5.1/src/polykin/thermo/eos/cubic.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 
     def __init__(self,
                  Tc: Union[float, FloatVectorLike],
                  Pc: Union[float, FloatVectorLike],
                  w: Union[float, FloatVectorLike],
                  k: Optional[FloatSquareMatrix]
                  ) -> None:
-        """Construct `Cubic` with the given parameters."""
 
         Tc, Pc, w = convert_FloatOrVectorLike_to_FloatVector([Tc, Pc, w])
 
         self.Tc = Tc
         self.Pc = Pc
         self.w = w
         self.k = k
@@ -181,15 +180,15 @@
             Pressure. Unit = Pa.
         y : FloatVector
             Mole fractions of all components. Unit = mol/mol.
 
         Returns
         -------
         FloatVector
-            Compressibility factor of the gas and/or liquid phases.
+            Compressibility factor of the vapor and/or liquid phases.
         """
         A = self.am(T, y)*P/(R*T)**2
         B = self.bm(y)*P/(R*T)
         return Z_cubic_roots(self._u, self._w, A, B)
 
     def Bm(self,
            T: float,
@@ -219,31 +218,31 @@
         return self.bm(y) - self.am(T, y)/(R*T)
 
     @abstractmethod
     def _alpha(self, T: float) -> FloatVector:
         pass
 
     def DA(self, T, V, n, v0):
-        nt = n.sum()
-        y = n/nt
+        nT = n.sum()
+        y = n/nT
         u = self._u
         w = self._w
         d = sqrt(u**2 - 4*w)
         am = self.am(T, y)
         bm = self.bm(y)
 
-        return nt*am/(bm*d)*log((2*V + nt*bm*(u - d))/(2*V + nt*bm*(u + d))) \
-            - nt*R*T*log((V - nt*bm)/(nt*v0))
+        return nT*am/(bm*d)*log((2*V + nT*bm*(u - d))/(2*V + nT*bm*(u + d))) \
+            - nT*R*T*log((V - nT*bm)/(nT*v0))
 
-    def phi(self,
-            T: float,
-            P: float,
-            y: FloatVector
-            ) -> FloatVector:
-        r"""Calculate the fugacity coefficients of all components in the gas
+    def phiV(self,
+             T: float,
+             P: float,
+             y: FloatVector
+             ) -> FloatVector:
+        r"""Calculate the fugacity coefficients of all components in the vapor
         phase.
 
         \begin{aligned}
         \ln \hat{\phi}_i &= \frac{b_i}{b_m}(Z-1)-\ln(Z-B^*)
         +\frac{A^*}{B^*\sqrt{u^2-4w}}\left(\frac{b_i}{b_m}-\delta_i  \right)\ln{\frac{2Z+B^*(u+\sqrt{u^2-4w})}{2Z+B^*(u-\sqrt{u^2-4w})}} \\
         \delta_i &= \frac{2a_i^{1/2}}{a_m}\sum_j y_j a_j^{1/2}(1-\bar{k}_{ij})
         \end{aligned}
@@ -347,15 +346,14 @@
     _Ωb = 0.08664
 
     def __init__(self,
                  Tc: Union[float, FloatVectorLike],
                  Pc: Union[float, FloatVectorLike],
                  k: Optional[FloatSquareMatrix] = None
                  ) -> None:
-        """Construct `RedlichKwong` with the given parameters."""
 
         super().__init__(Tc, Pc, np.zeros_like(Tc), k)
 
     def _alpha(self, T: float) -> FloatVector:
         return sqrt(self.Tc/T)
 
 
@@ -405,15 +403,14 @@
 
     def __init__(self,
                  Tc: Union[float, FloatVectorLike],
                  Pc: Union[float, FloatVectorLike],
                  w: Union[float, FloatVectorLike],
                  k: Optional[FloatSquareMatrix] = None
                  ) -> None:
-        """Construct `Soave` with the given parameters."""
 
         super().__init__(Tc, Pc, w, k)
 
     def _alpha(self, T: float) -> FloatVector:
         w = self.w
         Tr = T/self.Tc
         fw = 0.48 + 1.574*w - 0.176*w**2
@@ -466,15 +463,14 @@
 
     def __init__(self,
                  Tc: Union[float, FloatVectorLike],
                  Pc: Union[float, FloatVectorLike],
                  w: Union[float, FloatVectorLike],
                  k: Optional[FloatSquareMatrix] = None
                  ) -> None:
-        """Construct `PengRobinson` with the given parameters."""
 
         super().__init__(Tc, Pc, w, k)
 
     def _alpha(self, T: float) -> FloatVector:
         w = self.w
         Tr = T/self.Tc
         fw = 0.37464 + 1.54226*w - 0.26992*w**2
```

### Comparing `polykin-0.5.0/src/polykin/thermo/eos/virial.py` & `polykin-0.5.1/src/polykin/thermo/eos/virial.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 
     def __init__(self,
                  Tc: Union[float, FloatVectorLike],
                  Pc: Union[float, FloatVectorLike],
                  Zc: Union[float, FloatVectorLike],
                  w: Union[float, FloatVectorLike]
                  ) -> None:
-        """Construct `Virial` with the given parameters."""
 
         Tc, Pc, Zc, w = \
             convert_FloatOrVectorLike_to_FloatVector([Tc, Pc, Zc, w])
 
         self.Tc = Tc
         self.Pc = Pc
         self.Zc = Zc
@@ -182,30 +181,30 @@
         -------
         FloatSquareMatrix
             Matrix of interaction virial coefficients, $B_{ij}$.
             Unit = m³/mol.
         """
         return B_mixture(T, self.Tc, self.Pc, self.Zc, self.w)
 
-    def phi(self,
-            T: float,
-            P: float,
-            y: FloatVector
-            ) -> FloatVector:
-        r"""Calculate the fugacity coefficients of all components in the gas
+    def phiV(self,
+             T: float,
+             P: float,
+             y: FloatVector
+             ) -> FloatVector:
+        r"""Calculate the fugacity coefficients of all components in the vapor
         phase.
 
         $$
         \ln \hat{\phi}_i = \left(2\sum_j {y_jB_{ij}} -B_m \right)\frac{P}{RT}
         $$
 
-        where $\phi_i$ is the fugacity coefficient, $P$ is the pressure, $T$
-        is the temperature, $B_{ij}$ is the matrix of interaction virial
+        where $\hat{\phi}_i$ is the fugacity coefficient, $P$ is the pressure,
+        $T$ is the temperature, $B_{ij}$ is the matrix of interaction virial
         coefficients, $B_m$ is the second virial coefficient of the mixture,
-        and $y_i$ is the mole fraction in the gas phase.
+        and $y_i$ is the mole fraction in the vapor phase.
 
         **References**
 
         *   RC Reid, JM Prausniz, and BE Poling. The properties of gases &
             liquids 4th edition, 1986, p. 145.
 
         Parameters
@@ -223,18 +222,18 @@
             Fugacity coefficients of all components.
         """
         B = self.Bij(T)
         Bm = self.Bm(T, y)
         return exp((2*dot(B, y) - Bm)*P/(R*T))
 
     def DA(self, T, V, n, v0):
-        nt = n.sum()
-        y = n/nt
+        nT = n.sum()
+        y = n/nT
         Bm = self.Bm(T, y)
-        return -nt*R*T*log((V - nt*Bm)/(nt*v0))
+        return -nT*R*T*log((V - nT*Bm)/(nT*v0))
 
 # %% Second virial coefficient
 
 
 def B_pure(T: Union[float, FloatArray],
            Tc: float,
            Pc: float,
```

### Comparing `polykin-0.5.0/src/polykin/utils/math.py` & `polykin-0.5.1/src/polykin/utils/math.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/utils/tools.py` & `polykin-0.5.1/src/polykin/utils/tools.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/src/polykin/utils/types.py` & `polykin-0.5.1/src/polykin/utils/types.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.0/PKG-INFO` & `polykin-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: polykin
-Version: 0.5.0
+Version: 0.5.1
 Summary: A polymerization kinetics library.
 Home-page: https://hugomvale.github.io/polykin/
 License: MIT
 Keywords: polymer,polymerization,kinetics,reaction
 Author: HugoMVale
 Author-email: 57530119+HugoMVale@users.noreply.github.com
-Requires-Python: >=3.9,<3.13
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -34,20 +34,20 @@
 [![codecov](https://codecov.io/gh/HugoMVale/polykin/branch/main/graph/badge.svg?token=QfqQLX2rHx)](https://codecov.io/gh/HugoMVale/polykin)
 [![Latest Commit](https://img.shields.io/github/last-commit/HugoMVale/polykin)](https://img.shields.io/github/last-commit/HugoMVale/polykin)
 
 PolyKin is an open-source polymerization kinetics library for Python. It is still at an early
 development stage, but the following modules can already be used:
 
 - Activity coefficient models
-  - [50%] Cubic (Redlich-Kwong, Soave, Peng-Robinson)
   - [x] Ideal solution
   - [x] Flory-Huggins
   - [x] NRTL
   - [ ] Poly-NRTL
   - [x] UNIQUAC
+  - [x] Wilson
 - Copolymerization
   - [x] Implicit penultimate model
   - [x] Penultimate model
   - [x] Terminal model
   - [x] Mayo-Lewis equation (binary, ternary and multicomponent)
   - [x] Monomer dift equation (multicomponent)
   - [ ] Fitting methods
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: polykin Version: 0.5.0 Summary: A polymerization
+Metadata-Version: 2.1 Name: polykin Version: 0.5.1 Summary: A polymerization
 kinetics library. Home-page: https://hugomvale.github.io/polykin/ License: MIT
 Keywords: polymer,polymerization,kinetics,reaction Author: HugoMVale Author-
-email: 57530119+HugoMVale@users.noreply.github.com Requires-Python: >=3.9,<3.13
+email: 57530119+HugoMVale@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Chemistry Requires-
 Dist: matplotlib (>=3.7.1,<4.0.0) Requires-Dist: mpmath (>=1.3.0,<2.0.0)
@@ -17,36 +17,35 @@
 (https://github.com/HugoMVale/polykin/actions/workflows/test.yml/badge.svg)]
 (https://github.com/HugoMVale/polykin/actions) [![codecov](https://codecov.io/
 gh/HugoMVale/polykin/branch/main/graph/badge.svg?token=QfqQLX2rHx)](https://
 codecov.io/gh/HugoMVale/polykin) [![Latest Commit](https://img.shields.io/
 github/last-commit/HugoMVale/polykin)](https://img.shields.io/github/last-
 commit/HugoMVale/polykin) PolyKin is an open-source polymerization kinetics
 library for Python. It is still at an early development stage, but the
-following modules can already be used: - Activity coefficient models - [50%]
-Cubic (Redlich-Kwong, Soave, Peng-Robinson) - [x] Ideal solution - [x] Flory-
-Huggins - [x] NRTL - [ ] Poly-NRTL - [x] UNIQUAC - Copolymerization - [x]
-Implicit penultimate model - [x] Penultimate model - [x] Terminal model - [x]
-Mayo-Lewis equation (binary, ternary and multicomponent) - [x] Monomer dift
-equation (multicomponent) - [ ] Fitting methods - Equations of state - [50%]
-Cubic (Redlich-Kwong, Soave, Peng-Robinson) - [x] Ideal gas - [ ] Sanchez-
-Lacombe - [x] Virial equation - [ ] Database - Distributions - [x] Flory - [ ]
-Gold - [x] Log-normal - [x] Poison - [x] Schulz-Zimm - Kinetics - [x] Arrhenius
-- [x] Eyring - [x] Propagation half-length - [x] Termination composite model -
-Math - [x] Joint confidence regions - [ ] Models - Physical property
-correlations - [x] Antoine - [x] DIPPR - [x] Wagner - [x] Yaws - Step-growth
-polymerization - [x] Analytical solutions for $M_n$ and $M_w$ - Transport
-properties (estimation methods, mixing rules, etc.) - Diffusivity - [x] Binary
-gas mixtures - [x] Binary liquid mixtures - [x] Binary polymer solutions - [ ]
-Multicomponent polymer solutions - Thermal conductivity - [x] Gases - [x]
-Liquids - [ ] Polymer solutions - Viscosity - [x] Gases - [x] Liquids - [ ]
-Polymer solutions ## Documentation Please refer to the package [homepage]
-(https://hugomvale.github.io/polykin/). ## Tutorials The main features of
-PolyKin are explained and illustrated through a series of [tutorials](https://
-hugomvale.github.io/polykin/tutorials/) based on Jupyter [notebooks](https://
-github.com/HugoMVale/polykin/tree/main/docs/tutorials), which can be launched
-online via Binder.
+following modules can already be used: - Activity coefficient models - [x]
+Ideal solution - [x] Flory-Huggins - [x] NRTL - [ ] Poly-NRTL - [x] UNIQUAC -
+[x] Wilson - Copolymerization - [x] Implicit penultimate model - [x]
+Penultimate model - [x] Terminal model - [x] Mayo-Lewis equation (binary,
+ternary and multicomponent) - [x] Monomer dift equation (multicomponent) - [ ]
+Fitting methods - Equations of state - [50%] Cubic (Redlich-Kwong, Soave, Peng-
+Robinson) - [x] Ideal gas - [ ] Sanchez-Lacombe - [x] Virial equation - [ ]
+Database - Distributions - [x] Flory - [ ] Gold - [x] Log-normal - [x] Poison -
+[x] Schulz-Zimm - Kinetics - [x] Arrhenius - [x] Eyring - [x] Propagation half-
+length - [x] Termination composite model - Math - [x] Joint confidence regions
+- [ ] Models - Physical property correlations - [x] Antoine - [x] DIPPR - [x]
+Wagner - [x] Yaws - Step-growth polymerization - [x] Analytical solutions for
+$M_n$ and $M_w$ - Transport properties (estimation methods, mixing rules, etc.)
+- Diffusivity - [x] Binary gas mixtures - [x] Binary liquid mixtures - [x]
+Binary polymer solutions - [ ] Multicomponent polymer solutions - Thermal
+conductivity - [x] Gases - [x] Liquids - [ ] Polymer solutions - Viscosity -
+[x] Gases - [x] Liquids - [ ] Polymer solutions ## Documentation Please refer
+to the package [homepage](https://hugomvale.github.io/polykin/). ## Tutorials
+The main features of PolyKin are explained and illustrated through a series of
+[tutorials](https://hugomvale.github.io/polykin/tutorials/) based on Jupyter
+[notebooks](https://github.com/HugoMVale/polykin/tree/main/docs/tutorials),
+which can be launched online via Binder.
                            _[_M_W_D_ _o_f_ _a_ _p_o_l_y_m_e_r_ _b_l_e_n_d_]
 ## Installation PolyKin currently runs on Python 3.9+. You can install it from
 PyPI via `pip` (or `poetry`): ```console pip install polykin # poetry add
 polykin ``` Alternatively, you may install it directly from the source code
 repository: ```console git clone https://github.com/HugoMVale/polykin.git cd
 polykin pip install . # poetry install ```
```

