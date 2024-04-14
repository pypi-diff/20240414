# Comparing `tmp/cortix-1.1.8.tar.gz` & `tmp/cortix-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cortix-1.1.8.tar", last modified: Mon Jul  6 07:23:23 2020, max compression
+gzip compressed data, was "dist/cortix-1.1.9.tar", last modified: Sun Nov 15 19:58:00 2020, max compression
```

## Comparing `cortix-1.1.8.tar` & `cortix-1.1.9.tar`

### file list

```diff
@@ -1,153 +1,157 @@
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      208 2020-01-15 04:55:02.000000 cortix-1.1.8/.coveragerc
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      394 2020-01-15 04:55:02.000000 cortix-1.1.8/.gitignore
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      318 2020-01-15 04:55:02.000000 cortix-1.1.8/.travis.yml
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     1225 2020-01-15 04:55:02.000000 cortix-1.1.8/LICENSE.txt
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      210 2020-01-15 04:55:02.000000 cortix-1.1.8/MANIFEST.in
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     4562 2020-07-06 07:23:23.000000 cortix-1.1.8/PKG-INFO
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     2990 2020-01-15 04:55:02.000000 cortix-1.1.8/README.md
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      360 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/__init__.py
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/docs/
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      604 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/Makefile
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/docs/_templates/
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     1954 2020-02-07 17:47:21.000000 cortix-1.1.8/cortix/docs/_templates/globaltoc.html
--rwx------   0 dealmeida  (1000) dealmeida  (1000)     1023 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/build_docs.sh
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     7836 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/conf.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      158 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/contents.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)   276517 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/cortix-cover.png
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/docs/examples_rst/
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/docs/examples_rst/city_justice_rst/
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      127 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/examples_rst/city_justice_rst/adjudication.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      115 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/examples_rst/city_justice_rst/arrested.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      118 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/examples_rst/city_justice_rst/community.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      103 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/examples_rst/city_justice_rst/jail.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      159 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/examples_rst/city_justice_rst/modules.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      109 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/examples_rst/city_justice_rst/parole.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      109 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/examples_rst/city_justice_rst/prison.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      118 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/examples_rst/city_justice_rst/probation.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      143 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/examples_rst/city_justice_rst/run_city_justice.rst
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/docs/examples_rst/droplet_swirl_rst/
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      112 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/examples_rst/droplet_swirl_rst/droplet.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      101 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/examples_rst/droplet_swirl_rst/modules.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      146 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/examples_rst/droplet_swirl_rst/run_droplet_swirl.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      109 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/examples_rst/droplet_swirl_rst/vortex.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      150 2020-02-07 17:47:21.000000 cortix-1.1.8/cortix/docs/examples_rst/examples.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      173 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/examples_rst/modules.rst
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/docs/examples_rst/nbody_rst/
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      103 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/examples_rst/nbody_rst/body.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)       66 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/examples_rst/nbody_rst/modules.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      126 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/examples_rst/nbody_rst/run_planets.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     1704 2020-02-07 17:47:21.000000 cortix-1.1.8/cortix/docs/index.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     1837 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/install.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     1290 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/license.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)    50130 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/logo-old.jpg
--rw-------   0 dealmeida  (1000) dealmeida  (1000)    42015 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/logo.jpg
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/docs/src_rst/
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      112 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/src_rst/cortix_main.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      109 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/src_rst/module.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)       91 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/src_rst/modules.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      112 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/src_rst/network.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      103 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/src_rst/node.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      103 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/src_rst/port.rst
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/docs/support_rst/
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      152 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/support_rst/modules.rst
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/docs/support_rst/nuclear_rst/
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      106 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/support_rst/nuclear_rst/actor.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      126 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/support_rst/nuclear_rst/fuel_bucket.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      126 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/support_rst/nuclear_rst/fuel_bundle.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      150 2020-02-07 17:47:00.000000 cortix-1.1.8/cortix/docs/support_rst/nuclear_rst/fuel_segment.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      145 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/support_rst/nuclear_rst/fuelsegmentsgroups.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      115 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/support_rst/nuclear_rst/fuelslug.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      148 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/support_rst/nuclear_rst/modules.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      115 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/support_rst/nuclear_rst/nuclides.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      130 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/support_rst/periodictable.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      106 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/support_rst/phase.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      120 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/support_rst/phase_new.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      129 2020-02-07 17:47:21.000000 cortix-1.1.8/cortix/docs/support_rst/phase_newest.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      115 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/support_rst/quantity.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      109 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/support_rst/specie.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      112 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/support_rst/species.rst
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      109 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/docs/support_rst/stream.rst
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/examples/
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      810 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/examples/__init__.py
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/examples/bwr/
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)    14785 2020-07-04 20:47:04.000000 cortix-1.1.8/cortix/examples/bwr/condenser.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)    21869 2020-02-07 17:47:00.000000 cortix-1.1.8/cortix/examples/bwr/heater.py
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     5320 2020-07-05 21:46:52.000000 cortix-1.1.8/cortix/examples/bwr/params.py
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)    20569 2020-07-05 23:48:16.000000 cortix-1.1.8/cortix/examples/bwr/reactor.py
--rwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)     7206 2020-07-05 23:47:35.000000 cortix-1.1.8/cortix/examples/bwr/run_plant.py
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     8813 2020-07-04 20:47:04.000000 cortix-1.1.8/cortix/examples/bwr/turbine.py
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/examples/city_justice/
--rw-------   0 dealmeida  (1000) dealmeida  (1000)    10045 2020-02-07 17:47:21.000000 cortix-1.1.8/cortix/examples/city_justice/adjudication.py
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     9676 2020-07-04 21:01:29.000000 cortix-1.1.8/cortix/examples/city_justice/arrested.py
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)    12816 2020-07-04 21:01:29.000000 cortix-1.1.8/cortix/examples/city_justice/community.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     8677 2020-02-07 17:47:21.000000 cortix-1.1.8/cortix/examples/city_justice/jail.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     6965 2020-02-07 17:47:21.000000 cortix-1.1.8/cortix/examples/city_justice/parole.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     8355 2020-02-07 17:47:21.000000 cortix-1.1.8/cortix/examples/city_justice/prison.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     8062 2020-02-07 17:47:21.000000 cortix-1.1.8/cortix/examples/city_justice/probation.py
--rwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)     5744 2020-07-03 17:21:15.000000 cortix-1.1.8/cortix/examples/city_justice/run_city_justice.py
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/examples/droplet_swirl/
--rw-------   0 dealmeida  (1000) dealmeida  (1000)    10804 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/examples/droplet_swirl/droplet.py
--rwx------   0 dealmeida  (1000) dealmeida  (1000)     4815 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/examples/droplet_swirl/run_droplet_swirl.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     6148 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/examples/droplet_swirl/vortex.py
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/examples/ideal_gas/
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     7422 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/examples/ideal_gas/particle.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     2777 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/examples/ideal_gas/particle_handler.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     3900 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/examples/ideal_gas/particle_plotting.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     3093 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/examples/ideal_gas/run_particle.py
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/examples/nbody/
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     2028 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/examples/nbody/body.py
--rwx------   0 dealmeida  (1000) dealmeida  (1000)     3327 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/examples/nbody/run_planets.py
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/examples/umlrr/
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)    30154 2020-07-04 21:01:29.000000 cortix-1.1.8/cortix/examples/umlrr/code.py
--rwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)     3385 2020-07-04 21:01:29.000000 cortix-1.1.8/cortix/examples/umlrr/run_umlrr.py
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)    20752 2020-07-04 21:01:29.000000 cortix-1.1.8/cortix/examples/umlrr/umlrr.py
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/src/
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     8381 2020-07-04 21:01:29.000000 cortix-1.1.8/cortix/src/cortix_main.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     7176 2020-02-07 17:47:21.000000 cortix-1.1.8/cortix/src/module.py
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)    10554 2020-07-04 21:01:29.000000 cortix-1.1.8/cortix/src/network.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)      490 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/src/node.py
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     3888 2020-07-04 21:01:29.000000 cortix-1.1.8/cortix/src/port.py
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/support/
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/support/nuclear/
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     2963 2020-02-07 17:47:00.000000 cortix-1.1.8/cortix/support/nuclear/actor.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)    21754 2020-02-07 17:47:00.000000 cortix-1.1.8/cortix/support/nuclear/fuel_bucket.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)    13092 2020-02-07 17:47:00.000000 cortix-1.1.8/cortix/support/nuclear/fuel_bundle.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)    17107 2020-02-07 17:47:00.000000 cortix-1.1.8/cortix/support/nuclear/fuel_segment.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)    11393 2020-02-07 17:47:00.000000 cortix-1.1.8/cortix/support/nuclear/fuelsegmentsgroups.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)    31443 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/support/nuclear/fuelslug.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)    13599 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/support/nuclear/nuclides.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)   130180 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/support/periodictable.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)    25263 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/support/phase.py
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)    37356 2020-07-04 21:01:29.000000 cortix-1.1.8/cortix/support/phase_new.py
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)    37615 2020-07-04 21:01:29.000000 cortix-1.1.8/cortix/support/phase_newest.py
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     7725 2020-07-04 21:01:29.000000 cortix-1.1.8/cortix/support/quantity.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)    23802 2020-02-07 17:47:00.000000 cortix-1.1.8/cortix/support/specie.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     9488 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/support/species.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     8141 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/support/stream.py
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix/tests/
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     3119 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/tests/dataplot.py
--rw-------   0 dealmeida  (1000) dealmeida  (1000)     1037 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/tests/dummy_module.py
--rwx------   0 dealmeida  (1000) dealmeida  (1000)      544 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/tests/mpi_test_send_recv.py
--rwx------   0 dealmeida  (1000) dealmeida  (1000)      882 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/tests/test_cortix_add_module.py
--rwx------   0 dealmeida  (1000) dealmeida  (1000)     1161 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/tests/test_data_plot.py
--rwx------   0 dealmeida  (1000) dealmeida  (1000)     5036 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/tests/test_droplet.py
--rwx------   0 dealmeida  (1000) dealmeida  (1000)      357 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/tests/test_module_init.py
--rwx------   0 dealmeida  (1000) dealmeida  (1000)      193 2020-01-15 04:55:02.000000 cortix-1.1.8/cortix/tests/test_send_recv.py
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix.egg-info/
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     4562 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix.egg-info/PKG-INFO
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     4417 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix.egg-info/SOURCES.txt
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)        1 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix.egg-info/dependency_links.txt
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)       46 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix.egg-info/requires.txt
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)       15 2020-07-06 07:23:23.000000 cortix-1.1.8/cortix.egg-info/top_level.txt
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)       46 2020-07-04 05:23:41.000000 cortix-1.1.8/requirements.txt
-drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-07-06 07:23:23.000000 cortix-1.1.8/scripts/
--rwx------   0 dealmeida  (1000) dealmeida  (1000)      600 2020-01-15 04:55:02.000000 cortix-1.1.8/scripts/format-all.sh
--rwx------   0 dealmeida  (1000) dealmeida  (1000)      606 2020-01-15 04:55:02.000000 cortix-1.1.8/scripts/format-code.sh
--rwx------   0 dealmeida  (1000) dealmeida  (1000)      659 2020-01-15 04:55:02.000000 cortix-1.1.8/scripts/install_sundials.sh
--rwx------   0 dealmeida  (1000) dealmeida  (1000)      528 2020-01-15 04:55:02.000000 cortix-1.1.8/scripts/pylint-src.sh
--rwx------   0 dealmeida  (1000) dealmeida  (1000)      217 2020-01-15 04:55:02.000000 cortix-1.1.8/scripts/pypi_upload.sh
--rwx------   0 dealmeida  (1000) dealmeida  (1000)      999 2020-01-15 04:55:02.000000 cortix-1.1.8/scripts/recordcortixsession
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)       38 2020-07-06 07:23:23.000000 cortix-1.1.8/setup.cfg
--rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     1215 2020-07-06 07:21:57.000000 cortix-1.1.8/setup.py
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      208 2020-01-15 04:55:02.000000 cortix-1.1.9/.coveragerc
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      394 2020-01-15 04:55:02.000000 cortix-1.1.9/.gitignore
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      318 2020-01-15 04:55:02.000000 cortix-1.1.9/.travis.yml
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     1225 2020-01-15 04:55:02.000000 cortix-1.1.9/LICENSE.txt
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      210 2020-01-15 04:55:02.000000 cortix-1.1.9/MANIFEST.in
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     4590 2020-11-15 19:58:00.000000 cortix-1.1.9/PKG-INFO
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     2990 2020-01-15 04:55:02.000000 cortix-1.1.9/README.md
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      360 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/__init__.py
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/docs/
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      604 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/Makefile
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/docs/_templates/
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     1954 2020-02-07 17:47:21.000000 cortix-1.1.9/cortix/docs/_templates/globaltoc.html
+-rwx------   0 dealmeida  (1000) dealmeida  (1000)     1023 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/build_docs.sh
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     7836 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/conf.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      158 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/contents.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)   276517 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/cortix-cover.png
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/docs/examples_rst/
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/docs/examples_rst/city_justice_rst/
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      127 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/examples_rst/city_justice_rst/adjudication.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      115 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/examples_rst/city_justice_rst/arrested.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      118 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/examples_rst/city_justice_rst/community.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      103 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/examples_rst/city_justice_rst/jail.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      159 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/examples_rst/city_justice_rst/modules.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      109 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/examples_rst/city_justice_rst/parole.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      109 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/examples_rst/city_justice_rst/prison.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      118 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/examples_rst/city_justice_rst/probation.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      143 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/examples_rst/city_justice_rst/run_city_justice.rst
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/docs/examples_rst/droplet_swirl_rst/
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      112 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/examples_rst/droplet_swirl_rst/droplet.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      101 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/examples_rst/droplet_swirl_rst/modules.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      146 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/examples_rst/droplet_swirl_rst/run_droplet_swirl.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      109 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/examples_rst/droplet_swirl_rst/vortex.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      150 2020-02-07 17:47:21.000000 cortix-1.1.9/cortix/docs/examples_rst/examples.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      173 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/examples_rst/modules.rst
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/docs/examples_rst/nbody_rst/
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      103 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/examples_rst/nbody_rst/body.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)       66 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/examples_rst/nbody_rst/modules.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      126 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/examples_rst/nbody_rst/run_planets.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     1704 2020-02-07 17:47:21.000000 cortix-1.1.9/cortix/docs/index.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     1837 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/install.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     1290 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/license.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)    50130 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/logo-old.jpg
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)    42015 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/logo.jpg
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/docs/src_rst/
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      112 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/src_rst/cortix_main.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      109 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/src_rst/module.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)       91 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/src_rst/modules.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      112 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/src_rst/network.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      103 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/src_rst/node.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      103 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/src_rst/port.rst
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/docs/support_rst/
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      152 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/support_rst/modules.rst
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/docs/support_rst/nuclear_rst/
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      106 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/support_rst/nuclear_rst/actor.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      126 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/support_rst/nuclear_rst/fuel_bucket.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      126 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/support_rst/nuclear_rst/fuel_bundle.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      150 2020-02-07 17:47:00.000000 cortix-1.1.9/cortix/docs/support_rst/nuclear_rst/fuel_segment.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      145 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/support_rst/nuclear_rst/fuelsegmentsgroups.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      115 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/support_rst/nuclear_rst/fuelslug.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      148 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/support_rst/nuclear_rst/modules.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      115 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/support_rst/nuclear_rst/nuclides.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      130 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/support_rst/periodictable.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      106 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/support_rst/phase.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      120 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/support_rst/phase_new.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      129 2020-02-07 17:47:21.000000 cortix-1.1.9/cortix/docs/support_rst/phase_newest.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      115 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/support_rst/quantity.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      109 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/support_rst/specie.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      112 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/support_rst/species.rst
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      109 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/docs/support_rst/stream.rst
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/examples/
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      810 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/examples/__init__.py
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/examples/bwr/
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)    20973 2020-11-15 19:45:05.000000 cortix-1.1.9/cortix/examples/bwr/condenser.py
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)      217 2020-09-05 03:52:22.000000 cortix-1.1.9/cortix/examples/bwr/condenser_tester.py
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     5031 2020-11-15 19:45:05.000000 cortix-1.1.9/cortix/examples/bwr/cooler.py
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     1086 2020-11-15 19:45:05.000000 cortix-1.1.9/cortix/examples/bwr/params.py
+-rwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)     5838 2020-09-05 03:52:22.000000 cortix-1.1.9/cortix/examples/bwr/plant_test.py
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)    20147 2020-07-31 20:27:39.000000 cortix-1.1.9/cortix/examples/bwr/reactor-old.py
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)    28904 2020-11-15 19:45:05.000000 cortix-1.1.9/cortix/examples/bwr/reactor.py
+-rwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)    18017 2020-11-15 19:45:05.000000 cortix-1.1.9/cortix/examples/bwr/run_plant.py
+-rwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)     2973 2020-09-05 03:52:22.000000 cortix-1.1.9/cortix/examples/bwr/run_reactor.py
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)    10406 2020-11-15 19:45:05.000000 cortix-1.1.9/cortix/examples/bwr/turbine.py
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/examples/city_justice/
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)    10045 2020-02-07 17:47:21.000000 cortix-1.1.9/cortix/examples/city_justice/adjudication.py
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     9676 2020-07-21 21:29:01.000000 cortix-1.1.9/cortix/examples/city_justice/arrested.py
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)    12663 2020-11-15 19:49:21.000000 cortix-1.1.9/cortix/examples/city_justice/community.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     8677 2020-02-07 17:47:21.000000 cortix-1.1.9/cortix/examples/city_justice/jail.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     6965 2020-02-07 17:47:21.000000 cortix-1.1.9/cortix/examples/city_justice/parole.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     8355 2020-02-07 17:47:21.000000 cortix-1.1.9/cortix/examples/city_justice/prison.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     8062 2020-02-07 17:47:21.000000 cortix-1.1.9/cortix/examples/city_justice/probation.py
+-rwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)     5759 2020-11-15 19:45:05.000000 cortix-1.1.9/cortix/examples/city_justice/run_city_justice.py
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/examples/droplet_swirl/
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)    10804 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/examples/droplet_swirl/droplet.py
+-rwx------   0 dealmeida  (1000) dealmeida  (1000)     4815 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/examples/droplet_swirl/run_droplet_swirl.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     6148 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/examples/droplet_swirl/vortex.py
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/examples/ideal_gas/
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     7422 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/examples/ideal_gas/particle.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     2777 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/examples/ideal_gas/particle_handler.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     3900 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/examples/ideal_gas/particle_plotting.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     3093 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/examples/ideal_gas/run_particle.py
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/examples/nbody/
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     2028 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/examples/nbody/body.py
+-rwx------   0 dealmeida  (1000) dealmeida  (1000)     3327 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/examples/nbody/run_planets.py
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/examples/umlrr/
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)    30154 2020-07-21 21:29:01.000000 cortix-1.1.9/cortix/examples/umlrr/code.py
+-rwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)     3385 2020-07-21 21:29:01.000000 cortix-1.1.9/cortix/examples/umlrr/run_umlrr.py
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)    20779 2020-11-15 19:45:05.000000 cortix-1.1.9/cortix/examples/umlrr/umlrr.py
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/src/
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     8381 2020-07-21 21:29:02.000000 cortix-1.1.9/cortix/src/cortix_main.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     7176 2020-02-07 17:47:21.000000 cortix-1.1.9/cortix/src/module.py
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)    10554 2020-07-21 21:29:02.000000 cortix-1.1.9/cortix/src/network.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)      490 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/src/node.py
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     3888 2020-07-21 21:29:02.000000 cortix-1.1.9/cortix/src/port.py
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/support/
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/support/nuclear/
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     2963 2020-02-07 17:47:00.000000 cortix-1.1.9/cortix/support/nuclear/actor.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)    21754 2020-02-07 17:47:00.000000 cortix-1.1.9/cortix/support/nuclear/fuel_bucket.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)    13092 2020-02-07 17:47:00.000000 cortix-1.1.9/cortix/support/nuclear/fuel_bundle.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)    17107 2020-02-07 17:47:00.000000 cortix-1.1.9/cortix/support/nuclear/fuel_segment.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)    11393 2020-02-07 17:47:00.000000 cortix-1.1.9/cortix/support/nuclear/fuelsegmentsgroups.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)    31443 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/support/nuclear/fuelslug.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)    13599 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/support/nuclear/nuclides.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)   130180 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/support/periodictable.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)    25263 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/support/phase.py
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)    37365 2020-11-15 19:45:05.000000 cortix-1.1.9/cortix/support/phase_new.py
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)    37615 2020-07-21 21:29:02.000000 cortix-1.1.9/cortix/support/phase_newest.py
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     8019 2020-07-31 20:27:39.000000 cortix-1.1.9/cortix/support/quantity.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)    23802 2020-02-07 17:47:00.000000 cortix-1.1.9/cortix/support/specie.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     9488 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/support/species.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     8141 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/support/stream.py
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix/tests/
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     3119 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/tests/dataplot.py
+-rw-------   0 dealmeida  (1000) dealmeida  (1000)     1037 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/tests/dummy_module.py
+-rwx------   0 dealmeida  (1000) dealmeida  (1000)      544 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/tests/mpi_test_send_recv.py
+-rwx------   0 dealmeida  (1000) dealmeida  (1000)      882 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/tests/test_cortix_add_module.py
+-rwx------   0 dealmeida  (1000) dealmeida  (1000)     1161 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/tests/test_data_plot.py
+-rwx------   0 dealmeida  (1000) dealmeida  (1000)     5036 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/tests/test_droplet.py
+-rwx------   0 dealmeida  (1000) dealmeida  (1000)      357 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/tests/test_module_init.py
+-rwx------   0 dealmeida  (1000) dealmeida  (1000)      193 2020-01-15 04:55:02.000000 cortix-1.1.9/cortix/tests/test_send_recv.py
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix.egg-info/
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     4590 2020-11-15 19:57:59.000000 cortix-1.1.9/cortix.egg-info/PKG-INFO
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     4561 2020-11-15 19:58:00.000000 cortix-1.1.9/cortix.egg-info/SOURCES.txt
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)        1 2020-11-15 19:57:59.000000 cortix-1.1.9/cortix.egg-info/dependency_links.txt
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)       46 2020-11-15 19:57:59.000000 cortix-1.1.9/cortix.egg-info/requires.txt
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)       15 2020-11-15 19:57:59.000000 cortix-1.1.9/cortix.egg-info/top_level.txt
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)       46 2020-07-17 21:30:20.000000 cortix-1.1.9/requirements.txt
+drwxr-xr-x   0 dealmeida  (1000) dealmeida  (1000)        0 2020-11-15 19:58:00.000000 cortix-1.1.9/scripts/
+-rwx------   0 dealmeida  (1000) dealmeida  (1000)      600 2020-01-15 04:55:02.000000 cortix-1.1.9/scripts/format-all.sh
+-rwx------   0 dealmeida  (1000) dealmeida  (1000)      606 2020-01-15 04:55:02.000000 cortix-1.1.9/scripts/format-code.sh
+-rwx------   0 dealmeida  (1000) dealmeida  (1000)      659 2020-01-15 04:55:02.000000 cortix-1.1.9/scripts/install_sundials.sh
+-rwx------   0 dealmeida  (1000) dealmeida  (1000)      528 2020-01-15 04:55:02.000000 cortix-1.1.9/scripts/pylint-src.sh
+-rwx------   0 dealmeida  (1000) dealmeida  (1000)      216 2020-11-15 19:57:52.000000 cortix-1.1.9/scripts/pypi_upload.sh
+-rwx------   0 dealmeida  (1000) dealmeida  (1000)      999 2020-01-15 04:55:02.000000 cortix-1.1.9/scripts/recordcortixsession
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)       38 2020-11-15 19:58:00.000000 cortix-1.1.9/setup.cfg
+-rw-r--r--   0 dealmeida  (1000) dealmeida  (1000)     1517 2020-11-15 19:57:14.000000 cortix-1.1.9/setup.py
```

### Comparing `cortix-1.1.8/LICENSE.txt` & `cortix-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/PKG-INFO` & `cortix-1.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cortix
-Version: 1.1.8
+Version: 1.1.9
 Summary: Cortix is a Python library for network dynamics            modeling and HPC simulation.
 Home-page: https://cortix.org
 Author: Cortix Computing
-Author-email: tazzaoui@cs.uml.edu
+Author-email: valmor_dealmeida@uml.edu
 License: UNKNOWN
 Description: # Cortix
         A Python library for network dynamics modeling and HPC simulation.
           + [Cortix on Jupyter notebook examples](https://github.com/dpploy/cortix-nb)
           + [Documentation on the web](https://cortix.org)
         
         ![Website](https://img.shields.io/website/https/github.com/dpploy/cortix.svg)
@@ -105,8 +105,9 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Topic :: Education
 Classifier: Topic :: Utilities
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cortix-1.1.8/README.md` & `cortix-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/docs/Makefile` & `cortix-1.1.9/cortix/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/docs/_templates/globaltoc.html` & `cortix-1.1.9/cortix/docs/_templates/globaltoc.html`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/docs/build_docs.sh` & `cortix-1.1.9/cortix/docs/build_docs.sh`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/docs/conf.py` & `cortix-1.1.9/cortix/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/docs/cortix-cover.png` & `cortix-1.1.9/cortix/docs/cortix-cover.png`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/docs/index.rst` & `cortix-1.1.9/cortix/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/docs/install.rst` & `cortix-1.1.9/cortix/docs/install.rst`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/docs/license.rst` & `cortix-1.1.9/cortix/docs/license.rst`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/docs/logo-old.jpg` & `cortix-1.1.9/cortix/docs/logo-old.jpg`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/docs/logo.jpg` & `cortix-1.1.9/cortix/docs/logo.jpg`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/__init__.py` & `cortix-1.1.9/cortix/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/bwr/condenser.py` & `cortix-1.1.9/cortix/examples/bwr/condenser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,352 +1,496 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # This file is part of the Cortix toolkit environment.
 # https://cortix.org
+'''
+Models a condenser with steam flowing perpendicular to several horizontal tubes.
+Returns the runoff temperature of steam from the condenser.
+'''
 
 import logging
-
+import math
 import numpy as np
-import scipy.constants as const
-import scipy.constants as sc
+import matplotlib.pyplot as pyplot
+
+import scipy.constants as unit
 import iapws.iapws97 as steam_table
-import math
-from scipy.integrate import odeint
 
 from cortix import Module
 from cortix.support.phase_new import PhaseNew as Phase
 from cortix import Quantity
 
 class Condenser(Module):
-    '''
-    Boiling water reactor single-point reactor.
+    """Boiling water reactor single-point reactor.
 
     Notes
     -----
     These are the `port` names available in this module to connect to respective
     modules: `turbine`, and `pump`.
     See instance attribute `port_names_expected`.
+    """
+
+    # Class units
+    meter = unit.meter = 1.0
+    second = unit.second = 1.0
+
+    m_per_s = unit.meter/unit.second
+    kg_per_s = unit.kilo*unit.gram/unit.second
 
-    '''
+    def __init__(self):
+        """Constructor.
 
-    def __init__(self, ode_params):
-        '''
         Parameters
         ----------
-        params: dict
-            All parameters for the module in the form of a dictionary.
+        None
 
-        '''
+        Notes
+        -----
+
+        VFdA: as of now both turbines are supposed to send the same information
+              to the condenser. This is to be changed in the future to handle
+              different turbine steam conditions outflow.
+
+        Ports:
+
+         + `inflow-1`: individual inflow from a turbine module.
+         + `inflow-2`: individual inflow from a turbine module.
+         + `outflow`: combined outflow from condenser.
+
+        Attributes:
+
+         + inflow_state: dict
+            ['quality']: 0-1 quality of steam; 1 dew point steam;
+                         >1 super heated; 0 bubble boint; <0 subcooled liquid.
+            ['temp']: Runoff temperature from the turbine. Indicates how much
+                      superheat must be removed before condensation can begin.
+            ['pressure']: Not used.
+            ['flowrate']: Half the amount of liquid (kg/s) that the condenser
+                          must process each second.
+            ['time']:     Current simulation time in seconds.
+
+        """
 
         super().__init__()
 
         self.port_names_expected = ['inflow-1', 'inflow-2', 'outflow']
 
-        quantities      = list()
-        self.ode_params = dict()
-        self.params = ode_params
-        self.initial_time = 0.0
-        self.end_time     = 4.0 * const.hour
-        self.show_time    = (False,10.0)
+        # Units
+        self.meter = Condenser.meter
+        self.second = Condenser.second
+        self.m_per_s = Condenser.m_per_s
+        self.kg_per_s = Condenser.kg_per_s
+
+        # General attributes
+        self.initial_time = 0.0*self.second
+        self.end_time = 0.0*self.second
+
+        self.show_time = (False, 10.0)
         self.time_step = 10.0
         self.log = logging.getLogger('cortix')
 
-        # Condenser outflow phase history
+        # Domain attributes
+        self.inflow_state = None
+        self.pipe_diameter = 0.1*self.meter
+        self.liquid_velocity = 10.0*self.m_per_s
+        self.cooling_water_flowrate = 100000.0*self.kg_per_s
+        self.heat_transfer_area = 10200.0 # m2, or 500 4m long, 0.1m diameter pipes
+        self.condensation_ht_coeff = 5000.0 # w/m-k
+        self.subcooling_ht_coeff = 1000.0 # w/m-k
+        self.ss_temp = 287.15 # Initial and ending temperature of the condenser
+        self.inlet_pressure = 0.005 #MPa, the runoff pressure from the LPT
+        self.coolant_inflow_temp = 287.15 #K, condenser coolant inflow temp
+        # Outflow phase history
         quantities = list()
 
         flowrate = Quantity(name='condenser-runoff-flowrate',
-                   formal_name='Condenser Runoff Flowrate', unit='kg/s', value=0.0,
-                   info='Condenser Outflow Flowrate', latex_name='$Q$')
+                            formal_name='Condenser Runoff Flowrate',
+                            unit='kg/s', value=0.0,
+                            info='Condenser Outflow Flowrate',
+                            latex_name=r'$Q$')
 
         quantities.append(flowrate)
 
-        temp = Quantity(name='temp', formal_name='Condenser Runoff Temp.', unit='K',
-                value=273.15, info='Condenser Outflow Temperature', latex_name='$T_o$')
+        temp = Quantity(name='temp',
+                        formal_name='Condenser Runoff Temp.',
+                        unit='K',
+                        value=0.0,
+                        info='Condenser Outflow Temperature',
+                        latex_name=r'$T_o$')
 
         quantities.append(temp)
 
-        self.outflow_phase = Phase(self.initial_time, time_unit='s',
-                quantities=quantities)
-
-        return
+        self.outflow_phase = Phase(time_stamp=self.initial_time, time_unit='s',
+                                   quantities=quantities)
 
     def run(self, *args):
 
-       # self.__zero_ode_parameters()
-
         time = self.initial_time
         end_time = self.end_time
 
-        while time <  end_time + self.time_step:
+        while time < end_time + self.time_step:
 
-            if self.show_time[0] and abs(time%self.show_time[1]-0.0)<=1.e-1:
-                self.log.info('time = '+str(round(time/const.minute,1)))
+            if self.show_time[0] and abs(time%self.show_time[1]-0.0) <= 1.e-1:
+
+                msg = 'time = '+str(round(time/unit.minute, 1))
+                self.log.info(msg)
 
             # Communicate information
             #------------------------
             self.__call_ports(time)
 
             # Evolve one time step
             #---------------------
-            time = self.__step( time )
+            time = self.__step(time)
 
+    def tester(self):
+        """Passes a string of test data (temperature, chi) to the condenser.
+           Debug the model itself.
+        """
+        x = 0
+        #start with a basic temperature scale
+        print(x, '\n', 'TESTING TEMPERATURE', '\n', x)
+        temp = np.linspace(300, 500, 200)
+        test_chi = 0
+        output_vector = []
+        for i in temp:
+            output = self.__condenser(0, i, test_chi)
+            print('temp is ', i, ' and outflow temp is ', output)
+            output_vector.append(output)
+
+        #test how the system responds to different chi's
+        print(x, '\n', 'TESTING CHI', '\n', x)
+        chi = np.linspace(0, 0.98, 100)
+        test_temperature = steam_table._TSat_P(0.005)
+        output_vector_2 = []
+        for i in chi:
+            output = self.__condenser(0, test_temperature, i)
+            print('chi is ', i, ' and outflow temp is ', output)
+            output_vector_2.append(output)
+
+        #graph the results
+        pyplot.plot(temp, output_vector)
+        pyplot.title('inflow temperature vs outflow temperature')
+        pyplot.savefig('condenser-inflow-temp-vs-outflow-temp.png')
+        pyplot.close()
+        pyplot.plot(chi, output_vector_2)
+        pyplot.title('inflow quality vs outflow temperature')
+        pyplot.savefig('inflow-quality-vs-outflow-temp.png')
         return
 
     def __call_ports(self, time):
 
         # Interactions in the inflow port
         #----------------------------------------
         # one way "from" inflow-1
 
         # from
-        self.send( time, 'inflow-1' )
-        (check_time, inflow_state) = self.recv('inflow-1')
-        assert abs(check_time-time) <= 1e-6
+        if self.get_port('inflow-1').connected_port:
+            self.send(time, 'inflow-1')
+            (check_time, inflow_state) = self.recv('inflow-1')
+            assert abs(check_time-time) <= 1e-6
 
-        self.inflow_state = inflow_state
-        self.inflow_state['time'] = time
+            self.inflow_state = inflow_state
+            self.inflow_state['time'] = time
 
         # Interactions in the inflow port
         #----------------------------------------
         # one way "from" inflow-2
 
         # from
-        self.send( time, 'inflow-2' )
-        (check_time, inflow_state) = self.recv('inflow-2')
-        assert abs(check_time-time) <= 1e-6
+        if self.get_port('inflow-2').connected_port:
+            self.send(time, 'inflow-2')
+            (check_time, inflow_state) = self.recv('inflow-2')
+            assert abs(check_time-time) <= 1e-6
 
-        self.inflow_state = inflow_state
-        self.inflow_state['time'] = time
+            self.inflow_state = inflow_state
+            self.inflow_state['time'] = time
 
         # Interactions in the outflow port
         #-----------------------------------------
         # one way "to" outflow
 
-        # to 
-        message_time = self.recv('outflow')
-        outflow_state = dict()
-        outflow_cool_temp = self.outflow_phase.get_value('temp', time)
-        condenser_runoff = dict()
-        condenser_runoff['outflow-temp'] = outflow_cool_temp
-        self.send( (message_time, outflow_cool_temp), 'outflow' )
-
-        return
+        if self.get_port('outflow').connected_port:
+            message_time = self.recv('outflow')
+            outflow_cool_temp = self.outflow_phase.get_value('temp', time)
+            self.send((message_time, outflow_cool_temp), 'outflow')
 
     def __step(self, time):
 
-        import iapws.iapws97 as steam
-
-        assert abs( time-self.inflow_state['time'] ) <= 1e-6
+        assert abs(time-self.inflow_state['time']) <= 1e-6
 
         temp_in = self.inflow_state['temp']
-        chi_in    = self.inflow_state['quality']
+        chi_in = self.inflow_state['quality']
+        flowrate = self.inflow_state['flowrate']
 
-        t_out = self.__condenser(time, temp_in, chi_in, self.params)
+        t_out = self.__condenser(temp_in, chi_in, flowrate)
 
         condenser_runoff = self.outflow_phase.get_row(time)
 
         time = time + self.time_step
 
         self.outflow_phase.add_row(time, condenser_runoff)
         self.outflow_phase.set_value('temp', t_out)
 
         return time
 
-    def __condenser(self, time, temp_in, chi_in, params):
-        '''
-        Simple model to condense a vapor-liquid mixture and subcool it. Takes in either superheated steam or a two-phase water mixture, and calculates the amount of surface area within a simple condenser required to remove all degrees of superheat and condense the mixture.
-        '''
-
-        critical_temp    = steam_table._TSat_P(0.005)
-        condenser_runoff = 14 + 273.15
-
-        if chi_in == -1 and temp_in > critical_temp: #superheated vapor inlet; deprecated
-            return(293.15)
-            x = x_in
-
-            pressure = 0.005
-            h_steam = steam_table._Region2(temp_in, pressure)['h']
-            h_sat = steam_table._Region4(0.005, 1)['h']
-            q = params['steam flowrate'] * (h_steam - h_sat) * sc.kilo
+    def __condenser(self, temp_in, chi_in, flowrate):
+        """Simple model to condense a vapor-liquid mixture and subcool it.
+
+        Takes in either superheated steam or a two-phase water mixture, and
+        calculates the amount of surface area within a simple condenser required to
+        remove all degrees of superheat and condense the mixture.
+        """
+
+        if flowrate == 0:
+            # no flowrate, return initial simulation condition
+            return self.ss_temp
+
+        #temporary, basic model for condensation, until I can work out a more
+        #advanced model that gives realistic values.
+        pressure = self.inlet_pressure
+        t_coolant = self.coolant_inflow_temp
+        h_mixture = steam_table._Region4(pressure, chi_in)['h']
+        h_dewpt = steam_table._Region4(pressure, 0)['h']
+        heat_pwr = (h_mixture - h_dewpt) * unit.kilo * flowrate
+        area_required = heat_pwr/(self.condensation_ht_coeff * (temp_in - t_coolant))
+        area_remaining = self.heat_transfer_area - area_required
+
+        if area_remaining > 0:
+            initial_coolant_temp = self.coolant_inflow_temp
+            delta_t = heat_pwr/(self.cooling_water_flowrate * unit.kilo * 4.184)
+            final_coolant_temp = initial_coolant_temp + delta_t
+            subcooling_pwr = area_remaining * self.subcooling_ht_coeff *\
+                             (temp_in - final_coolant_temp)
+            delta_tb = subcooling_pwr/(flowrate * 4.184 * unit.kilo)
+            runoff_temp = temp_in - delta_tb
+
+            if runoff_temp < initial_coolant_temp:
+                runoff_temp = initial_coolant_temp
+
+            return runoff_temp
+
+        return self.ss_temp
+        #anything below this point is not currently in use; I need to figure
+        #out a more accurate condensation model, the current one calculates
+        #heat transfer coefficients in excess of 100k w/m2-k
+
+        #print(time, ' chi_in is ', chi_in)
+        critical_temp = steam_table._TSat_P(self.inlet_pressure)
+        condenser_runoff = self.coolant_inflow_temp
+        #if chi_in == -1 and temp_in > critical_temp: #superheated vapor inlet; deprecated
+            #return 293.15
+            #x = x_in
+            #pressure = 0.005
+            #h_steam = steam_table._Region2(temp_in, pressure)['h']
+            #h_sat = steam_table._Region4(0.005, 1)['h']
+            #q = params['steam flowrate'] * (h_steam - h_sat) * sc.kilo
 
             #log mean temperature difference
-            delta_Ta = temp_in - critical_temp
-            delta_Tb = 20-10
-            LMTD = (delta_Ta - delta_Tb) / (math.log(delta_Ta) - math.log(delta_Tb))
-
-            low = steam_table.IAPWS97(T=critical_temp+1, P=pressure)
-            high = steam_table.IAPWS97(T=temp_in, P=pressure)
-
-            low_conductivity = low.k
-            low_rho = low.rho
-            low_prandlt = low.Prandt
-            low_viscosity = low.mu
-            low_reynolds = (low_rho * 0.1 * 40)/low_viscosity
-            low_nusselt = (0.3 + 0.629 * (low_reynolds ** 0.5) * low_prandlt**(1/3))
-            low_nusselt = low_nusselt/(1+(0.4/low_prandlt)**(2/3))**(1/4)
-            low_nusselt = low_nusselt * (1 + (low_reynolds / 282000)**(5/6))**(4/4.5)       #nusselt number at the crtical temperature according to the churchill-bernsetin correlation
-            low_heat_transfer_coeff = low_nusselt * (low.k/0.1)
-
-            high_rho = high.rho
-            high_prandlt = high.Prandt
-            high_viscocity = high.mu
-            high_conductivity = high.k
-            high_viscosity = high.mu
-            high_reynolds = (high_rho * 0.1 * 40)/high_viscosity
-            high_nusselt = (0.3 + 0.629 * (high_reynolds ** 0.5) * high_prandlt**(1/3))
-            high_nusselt = high_nusselt/(1+(0.4/high_prandlt)**(2/3))**(1/4)
-            high_nusselt = high_nusselt * (1 + (high_reynolds / 282000)**(5/6))**(4/4.5)
-            high_heat_transfer_coeff = high_nusselt * (high_conductivity/0.1)
+            #delta_Ta = temp_in - critical_temp
+            #delta_Tb = 20-10
+            #LMTD = (delta_Ta - delta_Tb) / (math.log(delta_Ta) - math.log(delta_Tb))
+
+            #low = steam_table.IAPWS97(T=critical_temp+1, P=pressure)
+            #high = steam_table.IAPWS97(T=temp_in, P=pressure)
+
+            #low_conductivity = low.k
+            #low_rho = low.rho
+            #low_prandtl = low.Prandt
+            #low_viscosity = low.mu
+            #low_reynolds = (low_rho * 0.1 * 40)/low_viscosity
+            #low_nusselt = (0.3 + 0.629 * (low_reynolds ** 0.5) * low_prandtl**(1/3))
+            #low_nusselt = low_nusselt/(1+(0.4/low_prandtl)**(2/3))**(1/4)
+            #low_nusselt = low_nusselt * (1 + (low_reynolds / 282000)**(5/6))**(4/4.5)
+            #nusselt number at the crtical temperature according to the
+            #churchill-bernsetin correlation
+            #low_heat_transfer_coeff = low_nusselt * (low.k/0.1)
+
+            #high_rho = high.rho
+            #high_prandtl = high.Prandt
+            #high_viscocity = high.mu
+            #high_conductivity = high.k
+            #high_viscosity = high.mu
+            #high_reynolds = (high_rho * 0.1 * 40)/high_viscosity
+            #high_nusselt = (0.3 + 0.629 * (high_reynolds ** 0.5) * high_prandtl**(1/3))
+            #high_nusselt = high_nusselt/(1+(0.4/high_prandtl)**(2/3))**(1/4)
+            #high_nusselt = high_nusselt * (1 + (high_reynolds / 282000)**(5/6))**(4/4.5)
+            #high_heat_transfer_coeff = high_nusselt * (high_conductivity/0.1)
 
-            average_ht_transfer_coeff = (high_heat_transfer_coeff + low_heat_transfer_coeff)/2
+            #average_ht_transfer_coeff = (high_heat_transfer_coeff + low_heat_transfer_coeff)/2
 
         if chi_in > 0:
-            pressure = 0.005
+            pressure = self.inlet_pressure
             h_mixture = steam_table._Region4(pressure, chi_in)['h']
             h_dewpt = steam_table._Region4(pressure, 0)['h']
-            q = (h_mixture - h_dewpt) * sc.kilo * params['steam flowrate']
+            heat_pwr = (h_mixture - h_dewpt) * unit.kilo * flowrate
 
+            critical_temp = temp_in
             critical_temp = steam_table._TSat_P(pressure)
             sat_liquid = steam_table.IAPWS97(T=critical_temp - 1, P=pressure)
-            h_dew = steam_table._Region4(0.005, 1)['h']
-            h_bubl = steam_table._Region4(0.005, 0)['h']
-            water_cp = steam_table.IAPWS97(T=287.15, P=0.1013).cp
-            delta_Tb = q/(params['cooling water flowrate'] * water_cp * sc.kilo)
-            t_c_in = 14 + 273.15
-            t_c_out = 14 + 273.15 + delta_Tb
-
-            LMTD = (t_c_out - t_c_in)/(math.log(critical_temp - t_c_in))/(critical_temp - t_c_out)
-
-            pipe_diameter = params['pipe_diameter']
-            liquid_velocity = params['liquid_velocity']
-
-            #calculate the convective heat transfer coefficient on a liquid basis from the Churchill-Bernstein correlation
-            liquid_conductivity = sat_liquid.k
-            liquid_rho = sat_liquid.rho
-            liquid_prandlt = sat_liquid.Prandt
-            liquid_viscosity = sat_liquid.mu
-            liquid_reynolds = (liquid_rho * pipe_diameter * liquid_velocity)/liquid_viscosity
-
-            liquid_nusselt = (0.3 + 0.629 * (liquid_reynolds ** 0.5) * liquid_prandlt**(1/3))
-            liquid_nusselt = liquid_nusselt/(1+(0.4/liquid_prandlt)**(2/3))**(1/4)
-            liquid_nusselt = liquid_nusselt * (1 + (liquid_reynolds / 282000)**(5/6))**(4/4.5) #nusselt number at the crtical temperature according to the churchill-bernsetin correlation
-            liquid_heat_transfer_coeff = liquid_nusselt * (liquid_conductivity/pipe_diameter) #overall convective heat transfer coefficient
+            water_cp = steam_table.IAPWS97(T=287.15, P=0.1013).Liquid.cp
+            delta_tb = heat_pwr/(self.cooling_water_flowrate * \
+                    water_cp * unit.kilo)
+            t_c_in = self.coolant_inflow_temp
+            t_c_out = t_c_in + delta_tb
+
+            lmtd = (t_c_out - t_c_in)/(math.log(critical_temp - t_c_in))/\
+                    (critical_temp - t_c_out)
+
+            pipe_diameter = self.pipe_diameter
+            liquid_velocity = self.liquid_velocity
+
+            #calculate the convective heat transfer coefficient on a liquid basis
+            #from the Churchill-Bernstein correlation
+            liquid_conductivity = sat_liquid.Liquid.k
+            liquid_rho = sat_liquid.Liquid.rho
+            liquid_prandtl = sat_liquid.Liquid.Prandt
+            liquid_viscosity = sat_liquid.Liquid.mu
+            liquid_reynolds = (liquid_rho * pipe_diameter * liquid_velocity)/\
+                    liquid_viscosity
+
+            liquid_nusselt = (0.3 + 0.629 * (liquid_reynolds ** 0.5) * \
+                    liquid_prandtl**(1/3))
+            liquid_nusselt = liquid_nusselt/(1+(0.4/liquid_prandtl)**(2/3))**(1/4)
+            #nusselt number at the critical temperature according to the
+            #churchill-bernstein correlation
+            liquid_nusselt = liquid_nusselt * (1 + (liquid_reynolds / 282000)**(5/6))**(4/4.5)
+            #overall convective heat transfer coefficient
+            liquid_heat_transfer_coeff = liquid_nusselt * (liquid_conductivity/pipe_diameter)
 
             #determine the Martinelli paremeter
             steam = steam_table.IAPWS97(T=critical_temp+1, P=pressure)
-            steam_rho = steam.rho
-            steam_viscosity = steam.mu
+            steam_rho = steam.Vapor.rho
+            steam_viscosity = steam.Vapor.mu
 
             #print(chi_in)
 
-            xtt = ((1 -chi_in)/chi_in)**1.8 * (steam_rho/liquid_rho) * (liquid_viscosity/steam_viscosity)**0.5
+            xtt = (((1 -chi_in)/chi_in)**1.8 * (steam_rho/liquid_rho) * (liquid_viscosity/
+                                                                         steam_viscosity)**0.5)
             xtt = math.sqrt(xtt)
 
-            #determine the overall heat transfer coefficient from the McNaught expression
+            #determine the overall heat transfer coefficient from the McNaught
+            #expression
             alpha_sh = liquid_heat_transfer_coeff * (1/xtt)**0.78
+            print(alpha_sh, 'alpha_sh')
+
+            #determine how far the two-phase mixture gets in the condenser
+            #before being fully condensed
+            condensation_area = (heat_pwr/(alpha_sh * lmtd))
 
-            #determine how far the two-phase mixture gets in the condenser before being fully condensed
-            condensation_area = (q/(alpha_sh * LMTD))
-            remaining_area = params['heat transfer area'] - condensation_area
+            remaining_area = self.heat_transfer_area - condensation_area
             condenser_runoff = critical_temp
-            #print(remaining_area)
-            if time > params['malfunction start'] and time < params['malfunction end']:
-                condenser_runoff = 14 + 273.15
+            print(remaining_area)
+            #if time > params['malfunction start'] and time < params['malfunction end']:
+                #condenser_runoff = 14 + 273.15
 
             if remaining_area < 0:
-                condenser_runoff = 14 + 273.15
+                condenser_runoff = critical_temp
 
             elif remaining_area > 0:
             #subcool the remaining liquid
             #iterative method
-            #0. guess an ending value for the coolant and 
+            #0. guess an ending value for the coolant and
             #1. calculate high nusselt number
             #2. guess a value for low temperature
             #3. calculate low nusselt number
-            #4. calculate LMTD and average heat transfer coefficient
+            #4. calculate lmtd and average heat transfer coefficient
             #5. calculate q
-            #6. use q to calculate a new ending temperature for the water and the vapor
+            #6. use q to calculate a new ending temperature for the water and the
+            #   vapor
             #7. rinse and repeat
 
-                final_coolant_temperature_guess = steam_table._TSat_P(0.005) - 10 # initial guess
+                # initial guess
+                final_coolant_temperature_guess = steam_table._TSat_P(self.inlet_pressure) - 10
                 final_runoff_temperature_guess = 300 # initial guess
                 final_runoff_temperature = 0 #iteration variable
 
                 # Loop until convergeance, +- 1 degree kelvin
                 # Compute the runoff temperature (subcooled liquid)
                 while abs((final_runoff_temperature_guess -
                            final_runoff_temperature)) > 1:
 
-                    runoff_in = steam_table._TSat_P(0.005)
-                    coolant_in = 14 + 273.15 #k
+                    runoff_in = steam_table._TSat_P(self.inlet_pressure)
+                    coolant_in = self.coolant_inflow_temp #k
                     #assert(final_coolant_temperature_guess < final_runoff_temperature_guess)
                     #assert(final_coolant_temperature_guess > coolant_in)
 
                     final_runoff_temperature = final_runoff_temperature_guess
 
                     #guess the LMTD
-
-                    LMTD = ((runoff_in - final_coolant_temperature_guess) - (final_runoff_temperature - coolant_in))\
-                /math.log((runoff_in -  final_coolant_temperature_guess)/(final_runoff_temperature - coolant_in))
+                    lmtd = ((runoff_in - final_coolant_temperature_guess) - (final_runoff_temperature - coolant_in)) / math.log(((runoff_in -  final_coolant_temperature_guess) / (final_runoff_temperature - coolant_in)))
 
                     #average wall temperatures
                     upper_wall_temp = (coolant_in + runoff_in)/2
-                    lower_wall_temp = (final_runoff_temperature + final_coolant_temperature_guess)/2
+                    lower_wall_temp = (final_runoff_temperature + \
+                            final_coolant_temperature_guess)/2
 
                     #high temperature heat transfer coefficient calculation
-                    high_properties = steam_table.IAPWS97(T=upper_wall_temp, P=pressure)
-                    high_conductivity = high_properties.k
-                    high_rho = high_properties.rho
-                    high_prandlt = high_properties.Prandt
-                    high_viscosity = high_properties.mu
-                    high_reynolds = (high_rho * pipe_diameter * liquid_velocity)/high_viscosity
-
-                    high_nusselt = (0.3 + 0.629 * (high_reynolds ** 0.5) * high_prandlt**(1/3))
-                    high_nusselt = high_nusselt/(1+(0.4/high_prandlt)**(2/3))**(1/4)
+                    high_properties = steam_table.IAPWS97(T=upper_wall_temp,
+                                                          P=pressure)
+                    high_conductivity = high_properties.Liquid.k
+                    high_rho = high_properties.Liquid.rho
+                    high_prandtl = high_properties.Liquid.Prandt
+                    high_viscosity = high_properties.Liquid.mu
+                    high_reynolds = (high_rho * pipe_diameter * liquid_velocity)/\
+                            high_viscosity
+
+                    high_nusselt = (0.3 + 0.629 * (high_reynolds ** 0.5) * \
+                            high_prandtl**(1/3))
+                    high_nusselt = high_nusselt/(1+(0.4/high_prandtl)**(2/3))**(1/4)
                     high_nusselt = high_nusselt * (1 + (high_reynolds / 282000)**(5/6))**(4/4.5)
-                    high_heat_transfer_coeff = high_nusselt * (high_conductivity/pipe_diameter) #overall convective heat transfer coefficient
+                    #overall convective heat transfer coefficient
+                    high_heat_transfer_coeff = high_nusselt * (high_conductivity/pipe_diameter)
 
-                #   low temperature heat transfer coefficient calculation
+                    #   low temperature heat transfer coefficient calculation
                     low_properties = steam_table.IAPWS97(T=lower_wall_temp, P=pressure)
-                    low_conductivity = low_properties.k
-                    low_rho = low_properties.rho
-                    low_prandlt = low_properties.Prandt
-                    low_viscosity = low_properties.mu
-                    low_reynolds = (low_rho * pipe_diameter * liquid_velocity)/low_viscosity
-
-                    low_nusselt = (0.3 + 0.629 * (low_reynolds ** 0.5) * low_prandlt**(1/3))
-                    low_nusselt = low_nusselt/(1+(0.4/low_prandlt)**(2/3))**(1/4)
+                    low_conductivity = low_properties.Liquid.k
+                    low_rho = low_properties.Liquid.rho
+                    low_prandtl = low_properties.Liquid.Prandt
+                    low_viscosity = low_properties.Liquid.mu
+                    low_reynolds = (low_rho * pipe_diameter * \
+                            liquid_velocity)/low_viscosity
+
+                    low_nusselt = 0.3 + 0.629 * (low_reynolds ** 0.5) * \
+                            low_prandtl**(1/3)
+                    low_nusselt = low_nusselt/(1+(0.4/low_prandtl)**(2/3))**(1/4)
                     low_nusselt = low_nusselt * (1 + (low_reynolds / 282000)**(5/6))**(4/4.5)
-                    low_heat_transfer_coeff = low_nusselt * (low_conductivity/pipe_diameter) #overall convective heat transfer coefficient
+                    #overall convective heat transfer coefficient
+                    low_heat_transfer_coeff = low_nusselt * (low_conductivity/pipe_diameter)
 
                     #average heat transfer coefficient
-                    average_heat_transfer_coeff = (high_heat_transfer_coeff + low_heat_transfer_coeff)/2
+                    average_heat_transfer_coeff = ((high_heat_transfer_coeff
+                                                    + low_heat_transfer_coeff)/2)
 
                     #calculate q = UAdeltaTlm
-                    q_1 = average_heat_transfer_coeff * remaining_area * LMTD/10
+                    q_1 = average_heat_transfer_coeff * remaining_area * lmtd/10
 
                     #calculate actual coolant and liquid water temperatures
 
-                    coolant_cp = steam_table.IAPWS97(T=coolant_in, P=0.005).cp
-                    iterated_coolant_final_temp = (q_1/(coolant_cp * params['cooling water flowrate'] * sc.kilo)) + coolant_in
-
-                    steam_cp = steam_table.IAPWS97(T=runoff_in, P=0.005).cp
-                    iterated_steam_final_temp = runoff_in - (q_1/(steam_cp * params['steam flowrate'] * sc.kilo))
-
-                    if ( iterated_steam_final_temp   < coolant_in or
-                         iterated_coolant_final_temp > runoff_in or
-                         iterated_steam_final_temp   < iterated_coolant_final_temp):
+                    coolant_cp = steam_table.IAPWS97(T=coolant_in, P=self.inlet_pressure).Liquid.cp
+                    iterated_coolant_final_temp = ((q_1/(coolant_cp *
+                                                         self.cooling_water_flowrate
+                                                         * unit.kilo)) + coolant_in)
+
+                    steam_cp = steam_table.IAPWS97(T=runoff_in, P=self.inlet_pressure).Vapor.cp
+                    iterated_steam_final_temp = (runoff_in - (q_1/(steam_cp *
+                                                                   flowrate *
+                                                                   unit.kilo)))
+
+                    if (iterated_steam_final_temp < coolant_in or
+                            iterated_coolant_final_temp > runoff_in or
+                            iterated_steam_final_temp < iterated_coolant_final_temp):
 
                         final_runoff_temperature_guess = coolant_in
-                        final_coolant_runoff_guess = runoff_in
+                        #final_coolant_runoff_guess = runoff_in use for later implementation
                         break
 
                     final_runoff_temperature_guess = iterated_steam_final_temp
                     final_coolant_temperature_guess = iterated_coolant_final_temp
 
                 # end of: Loop until convergeance, +- 1 degree kelvin
                 condenser_runoff = final_runoff_temperature_guess
 
         else:
-            condenser_runoff = 14 + 273.15
+            condenser_runoff = self.ss_temp
 
         return condenser_runoff
```

### Comparing `cortix-1.1.8/cortix/examples/bwr/heater.py` & `cortix-1.1.9/cortix/examples/bwr/reactor-old.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 # -*- coding: utf-8 -*-
 # This file is part of the Cortix toolkit environment.
 # https://cortix.org
 
 import logging
 
 import numpy as np
-import scipy.constants as const
+import scipy.constants as unit
 from scipy.integrate import odeint
+import math
 
 from cortix import Module
 from cortix.support.phase_new import PhaseNew as Phase
 from cortix import Quantity
 
 class BWR(Module):
     '''
@@ -30,165 +31,181 @@
         Parameters
         ----------
         params: dict
             All parameters for the module in the form of a dictionary.
 
         '''
 
-        super().__init__(ode_params, self):
+        super().__init__()
 
-        self.port_names_expected = ['coolant-inflow','coolant-outflow']
+        self.port_names_expected = ['coolant-inflow', 'coolant-outflow',
+                                     'signal-out', 'signal-in']
 
-        quantities      = list()
-        self.ode_params = dict()
+        self.params = params
 
-        self.initial_time = 0.0 * const.day
-        self.end_time     = 4 * const.hour
-        self.time_step    = 10 * const.second
-        self.show_time    = (False,10*const.second)
+        self.initial_time = 0.0 * unit.day
+        self.end_time     = 4 * unit.hour
+        self.time_step    = 10.0
 
-        self.log = logging.getLogger('cortix')
-
-        # Coolant inflow phase history
-        quantities = list()
-
-        flowrate = Quantitiy(name='inflow-cool-flowrate',
-                   formalName='Inflow Cool. Flowrate',
-                   unit='kg/s', value=0.0)
-        quantities.append(flowrate)
-
-        temp = Quantitiy(name='inflow-cool-temp', formalName='Inflow Cool. Temperature',
-               unit='K', value=0.0)
-        quantities.append(temp)
+        self.show_time    = (False,10.0)
 
-        press = Quantitiy(name='inflow-cool-press',formalName='Inflow Cool. Pressure',
-                unit='Pa', value=0.0)
-        quantities.append(press)
-
-        self.coolant_inflow_phase = Phase(self.initial_time, time_unit='s',
-                quantities=quantities)
+        self.log = logging.getLogger('cortix')
 
         # Coolant outflow phase history
         quantities = list()
 
-        flowrate = Quantitiy(name='outflow-cool-flowrate',
-                   formalName='Outflow Cool. Flowrate',
-                   unit='kg/s', value=0.0)
+        flowrate = Quantity(name='flowrate', formal_name='q_c', unit='kg/s', value=0.0,
+                info='Reactor Outflow Coolant Flowrate' ,latex_name='$q_c$')
+
         quantities.append(flowrate)
 
-        temp = Quantitiy(name='outflow-cool-temp',
-                   formalName='Outflow Cool. Temperature',
-                   unit='K', value=0.0)
+        temp = Quantity(name='temp', formal_name='T_c', unit='K', value=273.15,
+                info='Reactor Outflow Coolant Temperature', latex_name='$T_c$')
+
         quantities.append(temp)
 
-        press = Quantitiy(name='outflow-cool-press',formalName='Outflow Cool. Pressure',
-                   unit='Pa', value=0.0)
+        press = Quantity(name='pressure', formal_name='P_c', unit='Pa', value=0.0,
+                info='Reactor Outflow Coolant Pressure', latex_name='$P_c$')
+
         quantities.append(press)
 
-        quality = Quantitiy(name='steam-quality',formalName='Steam Quality',
-                   unit='', value=0.0)
+        quality = Quantity(name='steam-quality', formal_name='chi_s', unit='', value=0.0,
+                info='Reactor STeam Quality', latex_name='$\chi$')
+
         quantities.append(quality)
 
         self.coolant_outflow_phase = Phase(self.initial_time, time_unit='s',
                 quantities=quantities)
 
         # Neutron phase history
         quantities = list()
 
-        neutron_dens = Quantitiy(name='neutron-dens',
-                   formalName='Neutron Dens.',
-                   unit='1/m^3', value=0.0)
+        neutron_dens = Quantity(name='neutron-dens', formal_name='n', unit='1/m^3',
+                value=0.0, info='Rel. Reactor Neutron Density', latex_name='$n$')
+
         quantities.append(neutron_dens)
 
         delayed_neutrons_0 = np.zeros(6)
 
-        delayed_neutron_cc = Quantitiy(name='delayed-neutrons-cc',
-                   formalName='Delayed Neutrons',
-                   unit='1/m^3', value=delayed_neutrons_0)
+        delayed_neutron_cc = Quantity(name='delayed-neutrons-cc', formal_name='c_i',
+                unit='1/m^3 ', value=delayed_neutrons_0,
+                info='Rel. Delayed Neutron Precursors', latex_name='$c_i$')
+
         quantities.append(delayed_neutron_cc)
 
         self.neutron_phase = Phase(self.initial_time, time_unit='s',
                 quantities=quantities)
 
-        #self.population_phase.SetValue('f0g', f0g_0, self.initial_time)
-
         #reactor paramaters
         quantities = list()
 
-        fuel_temp = Quantity(name='fuel-temp', formalName='Fuel Temp.', unit='k', value=273.15)
+        fuel_temp = Quantity( name='fuel-temp', formalName='T_f', unit='k',
+                value=273.15, info='Reactor Nuclear Fuel Temperature',
+                latex_name='$T_f$')
 
         quantities.append(fuel_temp)
 
-        reg_rod_position = Quantity(name='reg-rod-position', formalName='Regulating Rod Position', unit='m', value=0.0)
+        reg_rod_position = Quantity(name='reg-rod-position',
+                formal_name = 'reg rod position', unit='m', value=0.0,
+                info='Reactor Regulating Rod Position', latex_name='$x_p$')
 
         quantities.append(reg_rod_position)
 
-        self.reactor_phase = Phase(self.initial_time, time_unit='s', quantities=quantities)
-
-        self.ode_params = ode_params
+        self.reactor_phase = Phase(self.initial_time, time_unit='s',
+                quantities=quantities)
 
-        # Initialize inflows to zero
-        #self.ode_params['prison-inflow-rates']       = np.zeros(self.n_groups)
-        #self.ode_params['parole-inflow-rates']       = np.zeros(self.n_groups)
-        #self.ode_params['arrested-inflow-rates']     = np.zeros(self.n_groups)
-        #self.ode_params['jail-inflow-rates']         = np.zeros(self.n_groups)
-        #self.ode_params['adjudication-inflow-rates'] = np.zeros(self.n_groups)
-        #self.ode_params['probation-inflow-rates']    = np.zeros(self.n_groups)
+        # Initialize inflow
+        self.params['inflow-cool-temp'] = 273.15
 
         return
 
     def run(self, *args):
 
-       # self.__zero_ode_parameters()
+        # Some logic for logging time stamps
+        if self.initial_time + self.time_step > self.end_time:
+            self.end_time = self.initial_time + self.time_step
 
         time = self.initial_time
+        print_time = self.initial_time
+        print_time_step = self.show_time[1]
+        if print_time_step < self.time_step:
+            print_time_step = self.time_step
+
+        while time <= self.end_time:
 
-        while time < self.end_time:
+            last_time_stamp = time - self.time_step
 
-            if self.show_time[0] and abs(time%self.show_time[1]-0.0)<=1.e-1:
-                self.log.info('time = '+str(round(time/const.minute,1)))
+            if self.show_time[0] and time>=print_time and \
+                    time<print_time+print_time_step:
+
+                self.log.info( self.name+'::run():time[m]='+
+                        str(round(time/unit.minute,1)))
+
+                self.__logit = True
+                print_time += self.show_time[1]
+
+            else:
+                self.__logit = False
 
             # Communicate information
             #------------------------
-
             self.__call_ports(time)
 
             # Evolve one time step
             #---------------------
 
             time = self.__step( time )
 
-    def __call_input_ports(self, time):
+    def __call_ports(self, time):
+
+        # Interactions in the coolant-outflow port
+        #-----------------------------------------
+        # one way "to" coolant-outflow
+
+        # send to 
+        if self.get_port('coolant-outflow').connected_port:
+
+            message_time = self.recv('coolant-outflow')
+
+            coolant_outflow = self.__get_coolant_outflow( message_time )
+            outflow_params = dict()
+            self.send( (message_time, coolant_outflow), 'coolant-outflow' )
 
         # Interactions in the coolant-inflow port
         #----------------------------------------
         # one way "from" coolant-inflow
 
-        # from
-        self.send( time, 'coolant-inflow' )
-        (check_time, inflow_state) = self.recv('coolant-inflow')
-        assert abs(check_time-time) <= 1e-6
-
-        inflow = self.coolant_inlet_phase.GetRow(time)
-        self.coolant_inlet_phase.AddRow(time, inflow)
-        self.coolant_inlet_phase.SetValue('inflow-cool-temp', inflow_state['inflow-cool-temp'], time)
+        #self.send( time, 'coolant-inflow' )
 
-    def __call_output_ports(self, time):
-        # Interactions in the coolant-outflow port
+        # receive from
+        if self.get_port('coolant-inflow').connected_port:
+
+            self.send( time, 'coolant-inflow' )
+            (check_time, inflow_cool_temp) = self.recv('coolant-inflow')
+
+            assert abs(check_time-time) <= 1e-6
+            self.params['inflow-cool-temp'] = inflow_cool_temp
+
+        # Interactions in the signal-out port
         #-----------------------------------------
-        # one way "to" coolant-outflow
+        # one way "to" signal-out 
+
+        # send to 
+        if self.get_port('signal-out').connected_port:
+
+            message_time = self.recv('signal-out')
+
+            signal_out = self.__get_signal_out(time)
+
+            self.send( (message_time, signal_out), 'signal-out' )
+
+    def __get_coolant_outflow(message_time):
 
-        # to be, or not to be?
-        message_time = self.recv('coolant-outflow')
-        outflow_state = dict()
-        outflow_cool_temp = self.coolant_outflow_phase.GetValue('outflow-cool-temp', time)
-
-        outflow_state['outflow-cool-temp'] = outflow_cool_temp
-        self.send( (message_time, outflow_state), 'coolant-outflow' )
-        self.send( (message_time, outflow_state), 'coolant-inflow')
+        outflow = self.params['coolant-outflow']
+        return(outflow)
 
     def __step(self, time=0.0):
         r'''
         ODE IVP problem:
         Given the initial data at :math:`t=0`,
         :math:`u = (u_1(0),u_2(0),\ldots)`
         solve :math:`\frac{\text{d}u}{\text{d}t} = f(u)` in the interval
@@ -205,145 +222,158 @@
 
         '''
         import iapws.iapws97 as steam
 
         # Get state values
         u_0 = self.__get_state_vector( time )
 
-        t_interval_sec = np.linspace(0.0, self.time_step, num=2)
+        t_interval_sec = np.linspace(time, time+self.time_step, num=2)
 
         (u_vec_hist, info_dict) = odeint( self.__f_vec,
                                           u_0, t_interval_sec,
                                           args=( self.params, ),
                                           rtol=1e-4, atol=1e-8, mxstep=200,
                                           full_output=True )
 
         assert info_dict['message'] =='Integration successful.', info_dict['message']
 
         u_vec = u_vec_hist[1,:]  # solution vector at final time step
 
-        n_dens = u_vec[0]
-        c_vec = u_vec[1:5]
-        fuel_temp = u_vec[6]
-        cool_temp = u_vec[7]
-
-        time += self.time_step
+        n_dens    = u_vec[0]
+        c_vec     = u_vec[1:7]
+        fuel_temp = u_vec[7]
+        cool_temp = u_vec[8]
 
         #update state variables
-        outflow = self.coolant_outflow_phase.GetRow(time)
-        neutrons = self.neutron_phase.GetRow(time)
-        reactor = self.reactor_phase.GetRow(time)
-
+        outflow  = self.coolant_outflow_phase.get_row(time)
+        neutrons = self.neutron_phase.get_row(time)
+        reactor  = self.reactor_phase.get_row(time)
+        self.params['outflow temp'] = cool_temp
         time += self.time_step
 
-        self.coolant_outflow_phase.AddRow(time, outflow)
-        self.neutron_phase.AddRow(time, neutrons)
-        self.reactor_phase.AddRow(time, reactor)
-
-        self.coolant_outflow_phase.SetValue('outflow-cool-temp', cool_temp, time)
-        self.neutron_phase.SetValue('neutron-dens', n_dens, time)
-        self.neutron_phase.SetValue('delayed-neutrons-cc', c_vec, time)
-        self.reactor_phase.SetValue('fuel-temp', fuel_temp, time)
+        self.coolant_outflow_phase.add_row(time, outflow)
+        self.neutron_phase.add_row(time, neutrons)
+        self.reactor_phase.add_row(time, reactor)
+
+        self.coolant_outflow_phase.set_value('temp', cool_temp, time)
+        self.neutron_phase.set_value('neutron-dens', n_dens, time)
+        self.neutron_phase.set_value('delayed-neutrons-cc', c_vec, time)
+        self.reactor_phase.set_value('fuel-temp', fuel_temp, time)
 
         return time
 
+    def __signal_out(self, time=0.0):
+        '''
+        Send reactor signals to anyone requesting it.
+
+        Parameters
+        ----------
+        time: float
+            Time in SI unit.
+
+        Returns
+        -------
+        None
+
+        '''
+
+        signals = dict()
+
+        return signals
+
+    def __get_coolant_outflow(self, time=0.0):
+        '''
+        Get the coolant outflow stream.
+
+        Parameters
+        ----------
+        time: float
+            Time in SI unit.
+
+        Returns
+        -------
+        None
+
+        '''
+
+        coolant_outflow_stream = dict()
+
+        outflow_cool_temp = self.coolant_outflow_phase.get_value('temp', time)
+
+        coolant_outflow_stream['temp'] = outflow_cool_temp
+        coolant_outflow_stream['quality'] = 0.7
+        return coolant_outflow_stream
+
     def __get_state_vector(self, time):
         '''
         Return a numpy array of all unknowns ordered as below:
             neutron density (1), delayed neutron emmiter concentrations (6),
             termperature of fuel (1), temperature of coolant (1).
         '''
 
-        u_list = list()
-
         u_vec = np.empty(0,dtype=np.float64)
 
-        neutron_dens = self.neutron_phase.get_value('neutron-dens',time)/(const.centi)**3
+        neutron_dens = self.neutron_phase.get_value('neutron-dens',time)
         u_vec = np.append( u_vec, neutron_dens )
 
-        delayed_neutrons_cc = self.neutron_phase.get_value('delayed-neutrons-cc',time)/(const.centi)**3
-        u_vec = np.append( u_vec, delayed_neutrons_cc )
+        delayed_neutrons_cc = self.neutron_phase.get_value('delayed-neutrons-cc',time)
+        u_vec = np.append(u_vec, delayed_neutrons_cc)
 
-        fuel_temp = self.reactor_phase.GetValue('fuel-temp',time)
+        fuel_temp = self.reactor_phase.get_value('fuel-temp',time)
         u_vec = np.append( u_vec, fuel_temp)
 
-
-       # for spc in self.aqueous_phase.species:
-            #mass_cc = self.aqueous_phase.get_species_concentration(spc.name,time)
-           # mass_cc = self.aqueous_phase.get_species_concentration(spc.name)
-           # assert mass_cc is not None
-           # u_list.append( mass_cc )
-           # spc.flag = idx # the global id of the species
-           # idx += 1
-
-       # for spc in self.organic_phase.species:
-            #mass_cc = self.organic_phase.get_species_concentration(spc.name,time)
-           # mass_cc = self.organic_phase.get_species_concentration(spc.name)
-           # assert mass_cc is not None
-           # u_list.append( mass_cc )
-          #  spc.flag = idx # the global id of the species
-         #   idx += 1
-
-       # for spc in self.vapor_phase.species:
-            #mass_cc = self.vapor_phase.get_species_concentration(spc.name,time)
-           # mass_cc = self.vapor_phase.get_species_concentration(spc.name)
-           # assert mass_cc is not None
-           # u_list.append( mass_cc )
-           # spc.flag = idx # the global id of the species
-           # idx += 1
-
-        u_vec = np.array( u_list, dtype=np.float64 )
+        temp = self.coolant_outflow_phase.get_value('temp',time)
+        u_vec = np.append(u_vec, temp)
 
         # sanity check
-        assert not u_vec[u_vec<0.0],'%r'%u_vec
 
         return u_vec
 
-    def __alpha_tn_func(temp, params, self):
+    def __alpha_tn_func(self, temp, params):
         import math
         import scipy.misc as diff
-        import scipy.constants as sc
+        import scipy.constants as unit
         import iapws.iapws97 as steam
         import iapws.iapws95 as steam2
 
         pressure = steam._PSat_T(temp)
 
         d_rho = steam2.IAPWS95(P=pressure, T=temp-1).drhodT_P
 
         #d_rho2 = diff.derivative(derivative_helper, temp) # dRho/dTm
 
         rho = 1 / steam._Region4(pressure, 0)['v'] # mass density, kg/m3
 
-        Nm = ((rho * sc.kilo)/params['mod molar mass']) * sc.N_A * (sc.centi)**3 # number density of the moderator
-        d_Nm =  ((d_rho * sc.kilo)/params['mod molar mass']) * sc.N_A * (sc.centi)**3 #dNm/dTm
-        d_Nm = d_Nm * sc.zepto * sc.milli
+        Nm = ((rho * unit.kilo)/params['mod molar mass']) * unit.N_A * (unit.centi)**3 # number density of the moderator
+        d_Nm =  ((d_rho * unit.kilo)/params['mod molar mass']) * unit.N_A * (unit.centi)**3 #dNm/dTm
+        d_Nm = d_Nm * unit.zepto * unit.milli
 
         mod_macro_a = params['mod micro a'] * Nm # macroscopic absorption cross section of the moderator
         mod_macro_s = params['mod micro s'] * Nm # macroscopic scattering cross section of the moderator
 
         F = params['fuel macro a']/(params['fuel macro a'] + mod_macro_a) # thermal utilization, F
     #dF/dTm
         d_F = -1*(params['fuel macro a'] * params['mod micro a'] * d_Nm)/(params['fuel macro a'] + mod_macro_a)**2
 
         # Resonance escape integral, P
         P = math.exp((-1 * params['n fuel'] * (params['fuel_volume']) * params['I'])/(mod_macro_s * 3000))
         #dP/dTm
-        d_P = P * (-1 * params['n fuel'] * params['fuel_volume'] * sc.centi**3 * params['mod micro s'] * d_Nm)/(mod_macro_s * 3000 * sc.centi**3)**2
+        d_P = P * (-1 * params['n fuel'] * params['fuel_volume'] * unit.centi**3 * params['mod micro s'] * d_Nm)/(mod_macro_s * 3000 * unit.centi**3)**2
 
         Eth = 0.0862 * temp # convert temperature to energy in MeV
         E1 = mod_macro_s/math.log(params['E0']/Eth) # neutron thermalization macroscopic cross section
 
         Df = 1/(3 * mod_macro_s * (1 - params['mod mu0'])) # neutron diffusion coefficient
         tau = Df/E1 # fermi age, tau
         #dTau/dTm
         d_tau = (((0.0862 * (Eth/params['E0'])) * 3 * Nm) - math.log(params['E0']/Eth) * (params['mod micro s'] * d_Nm))/((3 * Nm)**2 * (1 - params['mod mu0']))
 
         L = math.sqrt(1/(3 * mod_macro_s * mod_macro_a * (1 - params['mod mu0']))) # diffusion length L
         # dL/dTm
-        d_L = 1/(2 * math.sqrt((-2 * d_Nm * sc.zepto * sc.milli)/(3 * params['mod micro s'] * params['mod micro a'] * (Nm * sc.zepto * sc.milli)**3 * (1 - params['mod mu0']))))
+        d_L = 1/(2 * math.sqrt((-2 * d_Nm * unit.zepto * unit.milli)/(3 * params['mod micro s'] * params['mod micro a'] * (Nm * unit.zepto * unit.milli)**3 * (1 - params['mod mu0']))))
 
         # left term of the numerator of the moderator temperature feedback coefficient, alpha
         left_1st_term = d_tau * (params['buckling']**2 + L**2 * params['buckling']**4) #holding L as constant
         left_2nd_term = d_L * (2 * L * params['buckling']**2 + 2 * L * tau * params['buckling']**4) # holding tau as constant
         left_term = (P * F) * (left_1st_term + left_2nd_term) # combining with P and F held as constant
 
         # right term of the numerator of the moderator temperature feedback coefficient, alpha
@@ -359,15 +389,15 @@
 
         alpha_tn = numerator/denominator
 
 
         alpha_tn = alpha_tn/3
         return alpha_tn
 
-    def __rho_func( t, n_dens, temp, params, self ):
+    def __rho_func(self, time, n_dens, temp, params, ):
         '''
         Reactivity function.
 
         Parameters
         ----------
         t: float, required
             Time.
@@ -381,51 +411,51 @@
         rho_t: float
             Value of reactivity.
 
         Examples
         --------
         '''
 
-        rho_0  = params['rho_0']
+        rho_0    = params['rho_0']
         temp_ref = params['temp_0']
         n_dens_ss_operation = params['n_dens_ss_operation']
-        alpha_n = params['alpha_n']
+        alpha_n  = params['alpha_n']
 
         if temp < 293.15: # if temperature is less than the starting temperature then moderator feedback is zero
             alpha_tn = 0
 
         else:
             alpha_tn = self.__alpha_tn_func(temp , self.params) #alpha_tn_func(temp, params)
 
-        if t > params['malfunction start'] and t < params['malfunction end']: # reg rod held in position; only mod temp reactivity varies with time during malfunction
+        if time > params['malfunction start'] and time < params['malfunction end']: # reg rod held in position; only mod temp reactivity varies with time during malfunction
             alpha_n = params['alpha_n_malfunction']
             rho_t = rho_0 + alpha_n + alpha_tn * (temp - temp_ref)
 
-        elif t > params['shutdown time']: # effectively the inverse of startup; gradually reduce reactivity and neutron density.
-            rho_0 = -1 * n_dens * rho_0
+        elif time > params['shutdown time']: # effectively the inverse of startup; gradually reduce reactivity and neutron density.
+            rho_0 = -1 * rho_0
             alpha_n = rho_0 - (alpha_tn * (temp - temp_ref))
             rho_t = rho_0
 
         elif n_dens < 1e-5: #controlled startup w/ blade; gradually increase neutron density to SS value.
             #rho_current = (1 - n_dens) * rho_0
             #alpha_n = rho_current - rho_0 - alpha_tn * (temp - temp_ref)
             #rho_t = rho_current
             #params['alpha_n_malfunction'] = alpha_n
             rho_t = rho_0
 
         else:
             rho_current = (1 - n_dens) * rho_0
-            alpha_n = rho_current - rho_0 - alpha_tn * (temp - temp_ref)
+            alphh_n = rho_current - rho_0 - alpha_tn * (temp - temp_ref)
             rho_t = rho_current
             params['alpha_n_malfunction'] = alpha_n
         #print(n_dens)
 
         return (rho_t, alpha_n, alpha_tn * (temp - temp_ref))
 
-    def __q_source( t, params, self ):
+    def __q_source(self, time, params):
         '''
         Neutron source delta function.
 
         Parameters
         ----------
         t: float, required
             Time.
@@ -438,32 +468,31 @@
             Value of source.
 
         Examples
         --------
         '''
         q_0 = params['q_0']
 
-        if t <= 1e-5: # small time value
+        if time <= 1500: # small time value
             q = q_0
         else:
             q = 0.0
             params['q_source_status'] = 'out'
 
         return q
 
-    def __sigma_fis_func( temp, params, self ):
+    def __sigma_fis_func(self, temp, params):
         '''
         Place holder for implementation
         '''
-
         sigma_f = params['sigma_f_o']  * math.sqrt(298/temp) * math.sqrt(math.pi) * 0.5
 
         return(sigma_f)
 
-    def __nuclear_pwr_dens_func( time, temp, n_dens, params, self ):
+    def __nuclear_pwr_dens_func(self, time, temp, n_dens, params ):
         '''
         Place holder for implementation
         '''
         n_dens = n_dens + self.__q_source(time, self.params) # include the neutrons from the initial source
 
         rxn_heat = params['fis_energy'] # get fission reaction energy J per reaction
 
@@ -471,47 +500,47 @@
 
         fis_nuclide_num_dens = params['fis_nuclide_num_dens_fake'] #  #/m3
 
         Sigma_fis = sigma_f * fis_nuclide_num_dens # macroscopic cross section
 
         v_o = params['thermal_neutron_velo'] # m/s
 
-        neutron_flux = n_dens * 4.5e14 * v_o
+        neutron_flux = n_dens * 0.95E15 * v_o * sigma_f/params['sigma_f_o']*0.7
 
          #reaction rate density
         rxn_rate_dens = Sigma_fis * neutron_flux
 
         # nuclear power source
-        q3prime = - rxn_heat * rxn_rate_dens # exothermic reaction W/m3
+        q3prime = - rxn_heat * rxn_rate_dens # exothermic reaction W/m3)
         #q3prime = - n_dens * 3323E6
         #print("q3prime")
         #print(q3prime)
 
         return q3prime
 
-    def __heat_sink_rate( time, temp_f, temp_c, params, self):
+    def __heat_sink_rate(self, time, temp_f, temp_c, params):
 
         ht_coeff = params['ht_coeff']
 
         q_f = - ht_coeff * (temp_f - temp_c)
         #print(q_f)
         return q_f
 
-    def __f_vec(time, u_vec, params, self):
-
+    def __f_vec(self, u_vec, time, params):
         num_negatives = u_vec[u_vec < 0]
+
         if num_negatives.any() < 0:
             assert np.max(abs(u_vec[u_vec < 0])) <= 1e-8, 'u_vec = %r'%u_vec
-        #assert np.all(u_vec >= 0.0), 'u_vec = %r'%u_vec
 
-        q_source_t = self__.q_source(time, self.params)
+        #assert np.all(u_vec >= 0.0), 'u_vec = %r'%u_vec
+        q_source_t = self.__q_source(time, self.params)
 
         n_dens = u_vec[0] # get neutron dens
 
-        c_vec = u_vec[1:-2] # get delayed neutron emitter concentration
+        c_vec  = u_vec[1:-2] # get delayed neutron emitter concentration
 
         temp_f = u_vec[-2] # get temperature of fuel
 
         temp_c = u_vec[-1] # get temperature of coolant
 
         # initialize f_vec to zero 
         species_decay = params['species_decay']
@@ -524,100 +553,64 @@
         # neutron balance
         #----------------
         rho_t = self.__rho_func(time, n_dens, temp_c, self.params)[0]
 
         beta = params['beta']
         gen_time = params['gen_time']
 
-        species_rel_yield = params['species_rel_yield']
-        beta_vec = np.array(species_rel_yield) * beta
-
-        assert len(lambda_vec)==len(beta_vec)
+        assert len(lambda_vec)==len(c_vec)
 
         f_tmp[0] = (rho_t - beta)/gen_time * n_dens + lambda_vec @ c_vec + q_source_t
-        #if f_tmp[0] < 0 and time < params['shutdown time'] and n_dens < 1:
-            #f_tmp[0] = 0
 
         #-----------------------------------
         # n species balances (implicit loop)
         #-----------------------------------
-        f_tmp[1:-2] = beta_vec/gen_time * n_dens - lambda_vec * c_vec
+
+        species_rel_yield = params['species_rel_yield']
+        beta_vec = np.array(species_rel_yield) * beta
+
+        assert len(lambda_vec)==len(c_vec)
+        assert len(beta_vec)==len(c_vec)
+        #species are in RELATIVE yield, not actual; multiply by delayed neutron
+        #yield fraction of 0.0065 to get the actual delayed neutron
+        #concentration
+
+        f_tmp[1:-2] = beta_vec / gen_time * n_dens - lambda_vec * c_vec
+
 
         #--------------------
         # fuel energy balance
         #--------------------
-        rho_f = params['fuel_dens']
-        cp_f = params['cp_fuel']
+        rho_f    = params['fuel_dens']
+        cp_f     = params['cp_fuel']
         vol_fuel = params['fuel_volume']
 
-        pwr_dens = self.__nuclear_pwr_dens_func( time, (temp_f+temp_c)/2, n_dens, self.params)
+        pwr_dens  = self.__nuclear_pwr_dens_func( time, (temp_f+temp_c)/2, n_dens, self.params)
 
         heat_sink = self.__heat_sink_rate( time, temp_f, temp_c, self.params)
 
         #assert heat_sink <= 0.0,'heat_sink = %r'%heat_sink
 
         f_tmp[-2] =  -1/rho_f/cp_f * ( pwr_dens - heat_sink/vol_fuel )
+
         #-----------------------
         # coolant energy balance
         #-----------------------
         rho_c    = params['coolant_dens']
         cp_c     = params['cp_coolant']
         vol_cool = params['coolant_volume']
 
         # subcooled liquid
-        turbine_calcs = turbine(time, temp_c,  params)
-        t_runoff = turbine_calcs[0]
-        x_runoff = turbine_calcs[2] #run the turbine, take the runoff and pass to condenser
-        condenser_out = condenser(time, t_runoff, x_runoff, temp_c, params) #run the condenser, pass runoff to the pump
-        pump_out = pump(time, condenser_out, temp_c, params) #run the pump, runoff returns to reactor as temp_in
-        #print("time is ", time, "and inlet temperature is", temp_in, "\n")
+        pump_out = params['inflow-cool-temp']
 
         tau = params['tau_fake']
 
         heat_source = heat_sink
         temp_in = pump_out
 
         f_tmp[-1] = - 1/tau * (temp_c - temp_in) - 1./rho_c/cp_c/vol_cool * heat_source
 
         # pressure calculations
 
         #print(time)
         #print(u_vec)
         return f_tmp
-
-    def __compute_outflow_rates(self, time, name):
-
-        f0g = self.population_phase.GetValue('f0g',time)
-
-        if name == 'arrested':
-
-            c0rg = self.ode_params['commit-to-arrested-coeff-grps']
-            m0rg = self.ode_params['commit-to-arrested-coeff-mod-grps']
-
-            c00g = self.ode_params['general-commit-to-arrested-coeff-grps']
-            m00g = self.ode_params['general-commit-to-arrested-coeff-mod-grps']
-
-            f0 = self.ode_params['non-offender-adult-population']
-
-            # Recidivism
-            outflow_rates = c0rg * m0rg * np.abs(f0g) + c00g * m00g * f0
-
-        return outflow_rates
-
-    def __zero_ode_parameters(self):
-        '''
-        If ports are not connected the corresponding outflows must be zero.
-
-        '''
-
-        zeros = np.zeros(self.n_groups)
-
-        p_names = [p.name for p in self.ports]
-
-        if 'arrested' not in p_names:
-            self.ode_params['commit-to-arrested-coeff-grps']     = zeros
-            self.ode_params['commit-to-arrested-coeff-mod-grps'] = zeros
-
-            self.ode_params['general-commit-to-arrested-coeff-grps']     = zeros
-            self.ode_params['general-commit-to-arrested-coeff-mod-grps'] = zeros
-
-        return
```

### Comparing `cortix-1.1.8/cortix/examples/bwr/reactor.py` & `cortix-1.1.9/cortix/examples/bwr/reactor.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,409 +6,590 @@
 import logging
 
 import math
 from scipy.integrate import odeint
 import scipy.constants as unit
 import numpy as np
 
+import iapws.iapws97 as steam
+import iapws.iapws95 as steam2
+
 from cortix import Module
 from cortix.support.phase_new import PhaseNew as Phase
 from cortix import Quantity
 
 class BWR(Module):
-    '''
-    Boiling water reactor single-point reactor.
+    """Boiling water reactor single-point reactor.
 
     Notes
     -----
     These are the `port` names available in this module to connect to respective
     modules: `turbine`, and `pump`.
     See instance attribute `port_names_expected`.
 
-    '''
+    """
 
     def __init__(self, params):
-        '''
+        """Constructor.
+
         Parameters
         ----------
         params: dict
             All parameters for the module in the form of a dictionary.
 
-        '''
+        """
 
         super().__init__()
 
         self.port_names_expected = ['coolant-inflow', 'coolant-outflow',
-                                    'signal-out', 'signal-in']
+                                    'RCIS-inflow', 'RCIS-outflow']
 
         self.params = params
 
-        self.initial_time = 0.0 * unit.day
-        self.end_time = 4 * unit.hour
+        self.initial_time = params['start-time']
+        self.end_time = params['end-time']
         self.time_step = 10.0
 
         self.show_time = (False, 10.0)
 
         self.log = logging.getLogger('cortix')
         self.__logit = False
 
+        #Data pertaining to one-group energy neutron balance
+        self.gen_time = 1.0e-4  # s
+        self.beta = 6.5e-3  # params['k_infty'] = 1.3447
+        # geometric buckling; B = (pi/R)^2 + (2.405/H)^2
+        self.buckling = (math.pi/237.5)**2.0 + (2.405/410)**2.0
+        self.q_0 = 5000
+        # fuel macroscopic absorption cross section, cm^-1
+        self.fuel_macro_a = 1.34226126162
+        # moderator microscopic absorption cross section, cm^2
+        self.mod_micro_a = 0.332 * unit.zepto * unit.milli
+        #number density of the fuel, atoms/cm^3
+        self.n_fuel = 1.9577906e+21
+        #resonance integral, I (dimensionless)
+        self.I = 40.9870483 * unit.zepto * unit.milli
+        # moderator microscopic scattering cross section, cm^2
+        self.mod_micro_s = 20 * unit.zepto * unit.milli
+        self.xi = 1 # average logarithmic energy decrement for light water
+        # energy of a neutron produced by fissioning, in electron volts
+        self.E0 = 2 * unit.mega
+        self.mod_mu0 = 0.71 # migration and diffusion area constants
+        self.eta = 1.03 # fast fission factor
+        self.epsilon = 2.05 # neutron multiplecation factor
+        self.mod_molar_mass = 18 # g/mol
+        
+        # Delayed neutron emission
+        self.species_decay = [0.0124, 0.0305, 0.111, 0.301, 1.14, 3.01] # 1/sec
+        self.species_rel_yield = [0.033, 0.219, 0.196, 0.395, 0.115, 0.042]
+
+        # Data pertaining to two-temperature heat balances
+        self.fis_energy = 180 * 1.602e-13 # J/fission
+        self.enrich = 4.3/100.
+        self.fuel_mat_mass_dens = 10.5 # g/cc
+        #params['moderator_fuel_ratio'] = 387 # atomic number concentration ratio
+        self.sigma_f_o = 586.2 * 100 * 1e-30 # m2
+        self.temp_o = 20 + 273.15 # K
+        self.thermal_neutron_velo = 2200 # m/s
+
+        self.fis_nuclide_num_dens = 9.84e26 # (fissile nuclei)/m3
+
+        self.q_c = 303 # volumetric flow rate
+
+        self.fuel_dens = 10500 # kg/m3
+        self.cp_fuel = 175 # J/(kg K)
+        self.fuel_volume = 7.25  # m3
+
+        self.steam_flowrate = 1820 # kg/s
+        self.coolant_dens = 1000 #  kg/m3
+        self.cp_coolant = 3500# J/(mol K) - > J/(kg K)
+        self.coolant_volume = 7 #m3
+
+        self.ht_coeff = 45000000
+
+        # J/(fission sec) 1.26 t^-1.2 (t in seconds)
+        self.fis_beta_energy = 1.26 * 1.602e-13
+        # J/(fission sec) 1.40 t^-1.2 (t in seconds)
+        self.fis_alpha_energy = 1.40 * 1.602e-13
+        # % subcooling based on the % subcooling that exists at steady state
+        self.subcooling_percent = 1 #(1 -(steam_table._Region4(7, 0)["h"]  - steam_table._Region1(493.15, 7)["h"])/(steam_table._Region4(7,0)["h"]))
+        self.shutdown_temp_reached = False
+        self.q_source_status = 'in' # is q_source inserted (in) or withdrawn (out)
+
+        gen_time = self.gen_time # retrieve neutron generation time
+        self.q_0 = 0.1
+
+        self.n_ss = 0 # neutronless steady state before start up
+
+        rho_0_over_beta = 0.25 # $
+        beta = self.beta
+
+        # control rod reactivity worth; enough to cancel out the negative
+        self.alpha_n = 0
+
+        self.reactivity = rho_0_over_beta * beta # "rho/beta = 10 cents"
+
+        self.temp_o = self.temp_o
+
+        self.tau = 1 # s
+        self.malfunction_subcooling = 0.75
+        self.alpha_n_malfunction = 0
+        n_species = len(self.species_decay)
+
+        assert len(self.species_rel_yield) == n_species
+
+        # initialize concentration vector
+        c_vec_0 = np.zeros(n_species, dtype=np.float64)
+        # retrieve list of decay constants
+        species_decay = self.species_decay
+        lambda_vec = np.array(species_decay) # create a numpy vector
+        beta = self.beta
+        species_rel_yield = self.species_rel_yield
+        # create the beta_i's vector
+        beta_vec = np.array(species_rel_yield) * beta
+        gen_time = self.gen_time # retrieve neutron generation time
+        n_ss = self.n_ss
+        # compute the steady state precursors number density
+        c_vec_ss = beta_vec/lambda_vec/gen_time * n_ss
+        self.c_vec_ss = c_vec_ss
+        # setup initial condition for variables
+        self.n_0 = n_ss
+        self.c_vec_0 = c_vec_ss
+        self.rho_0 = self.reactivity
+
+        self.RCIS = False
+
         # Coolant outflow phase history
         quantities = list()
 
-        flowrate = Quantity(name='flowrate', formal_name='q_c', unit='kg/s',
-                            value=0.0,
-                            info='Reactor Outflow Coolant Flowrate',
-                            latex_name='$q_c$')
+        flowrate = Quantity(name='flowrate', formal_name='q_c', unit='kg/s', value=0.0,
+                            info='Reactor Outflow Coolant Flowrate', latex_name=r'$q_c$')
 
         quantities.append(flowrate)
 
-        temp = Quantity(name='temp', formal_name='T_c', unit='K',
-                        value=273.15,
-                        info='Reactor Outflow Coolant Temperature',
-                        latex_name='$T_c$')
+        temp = Quantity(name='temp', formal_name='T_c', unit='K', value=params['coolant-temp'],
+                        info='Reactor Outflow Coolant Temperature', latex_name=r'$T_c$')
 
         quantities.append(temp)
 
-        press = Quantity(name='pressure', formal_name='P_c', unit='Pa',
-                         value=0.0,
-                         info='Reactor Outflow Coolant Pressure',
-                         latex_name='$P_c$')
+        press = Quantity(name='pressure', formal_name='P_c', unit='Pa', value=0.0,
+                         info='Reactor Outflow Coolant Pressure', latex_name=r'$P_c$')
 
         quantities.append(press)
 
-        quality = Quantity(name='steam-quality', formal_name='chi_s', unit='',
-                           value=0.0,
-                           info='Reactor STeam Quality', latex_name=r'$\chi$')
-
+        quality = Quantity(name='steam-quality', formal_name='chi_s', unit='', value=0.0,
+                           info='Reactor Steam Quality', latex_name=r'$\chi$')
         quantities.append(quality)
 
-        self.coolant_outflow_phase = Phase(self.initial_time, time_unit='s',
-                                           quantities=quantities)
+        self.coolant_outflow_phase = Phase(time_stamp=self.initial_time, time_unit='s', quantities=quantities)
 
         # Neutron phase history
         quantities = list()
 
         neutron_dens = Quantity(name='neutron-dens', formal_name='n', unit='1/m^3',
-                                value=0.0, info='Rel. Reactor Neutron Density',
-                                latex_name='$n$')
+                                value=params['n-dens'], info='Rel. Reactor Neutron Density', latex_name=r'$n$')
 
         quantities.append(neutron_dens)
 
-        delayed_neutrons_0 = np.zeros(6)
-
         delayed_neutron_cc = Quantity(name='delayed-neutrons-cc', formal_name='c_i',
-                                      unit='1/m^3 ',
-                                      value=delayed_neutrons_0,
-                                      info='Relative Delayed Neutron Precursors',
-                                      latex_name='$c_i$')
-
+                                      unit='1/m^3 ', value=params['delayed-neutron-cc'],
+                                      info='Rel. Delayed Neutron Precursors', latex_name=r'$c_i$')
         quantities.append(delayed_neutron_cc)
 
-        self.neutron_phase = Phase(self.initial_time, time_unit='s',
-                quantities=quantities)
+        self.neutron_phase = Phase(time_stamp=self.initial_time, time_unit='s',
+                                   quantities=quantities)
 
-        #reactor paramaters
+        # Reactor phase
         quantities = list()
 
-        fuel_temp = Quantity( name='fuel-temp', formalName='T_f', unit='k',
-                value=273.15, info='Reactor Nuclear Fuel Temperature',
-                latex_name='$T_f$')
+        fuel_temp = Quantity(name='fuel-temp', formalName='T_f', unit='K',
+                             value=params['fuel-temp'], info='Reactor Nuclear Fuel Temperature',
+                             latex_name=r'$T_f$')
 
         quantities.append(fuel_temp)
 
         reg_rod_position = Quantity(name='reg-rod-position',
-                formal_name = 'reg rod position', unit='m', value=0.0,
-                info='Reactor Regulating Rod Position', latex_name='$x_p$')
+                                    formal_name='reg rod position', unit='m', value=0.0,
+                                    info='Reactor Regulating Rod Position', latex_name=r'$x_p$')
 
         quantities.append(reg_rod_position)
 
-        self.reactor_phase = Phase(self.initial_time, time_unit='s',
-                quantities=quantities)
+        self.reactor_phase = Phase(time_stamp=self.initial_time, time_unit='s',
+                                   quantities=quantities)
 
         # Initialize inflow
-        self.params['inflow-cool-temp'] = 273.15
+        self.params['inflow-cool-temp'] = params['condenser-runoff-temp']
 
-    def run(self, *args):
+        self.params['decay-heat-0'] = 0
+        # Set up initial decay heat value
+        if self.params['shutdown-mode']:
+            temp = params['fuel-temp']
+            n_dens = params['n-dens']
+            decay_heat = self.__nuclear_pwr_dens_func(999, temp, n_dens, params)
+            decay_heat *= 0.0622 # assume decay heat at 6.5% total power
+            self.params['decay-heat-0'] = decay_heat
 
+    def run(self, *args):
         # Some logic for logging time stamps
         if self.initial_time + self.time_step > self.end_time:
             self.end_time = self.initial_time + self.time_step
 
         time = self.initial_time
         print_time = self.initial_time
         print_time_step = self.show_time[1]
         if print_time_step < self.time_step:
             print_time_step = self.time_step
 
         while time <= self.end_time:
 
-            last_time_stamp = time - self.time_step
+            #last_time_stamp = time - self.time_step
 
-            if self.show_time[0] and time>=print_time and \
-                    time<print_time+print_time_step:
+            #if self.show_time[0] and time >= print_time and \
+            #        time<print_time+print_time_step:
+            if self.show_time[0] and print_time <= time < print_time+print_time_step:
 
-                self.log.info( self.name+'::run():time[m]='+
-                        str(round(time/unit.minute,1)))
+                msg = self.name+'::run():time[m]='+ str(round(time/unit.minute, 1))
+                self.log.info(msg)
 
                 self.__logit = True
                 print_time += self.show_time[1]
 
             else:
                 self.__logit = False
 
             # Communicate information
             #------------------------
             self.__call_ports(time)
 
             # Evolve one time step
             #---------------------
 
-            time = self.__step( time )
+            time = self.__step(time)
 
     def __call_ports(self, time):
 
+        current_temp = self.__get_coolant_outflow(time)['temp']
+        if current_temp < 373.15:
+            if self.params['operating-mode'] == 'shutdown':
+                self.RCIS = True
+
+        if current_temp > 373.15:
+            if self.params['operating-mode'] == 'startup':
+                self.RCIS = False
+
         # Interactions in the coolant-outflow port
         #-----------------------------------------
         # one way "to" coolant-outflow
 
         # send to
         if self.get_port('coolant-outflow').connected_port:
-
             message_time = self.recv('coolant-outflow')
 
-            coolant_outflow = self.__get_coolant_outflow(message_time)
-            outflow_params = dict()
-            self.send((message_time, coolant_outflow), 'coolant-outflow')
+            if self.RCIS:
+                coolant_outflow = dict()
+                coolant_outflow['temp'] = 287.15
+                coolant_outflow['pressure'] = 0
+                coolant_outflow['quality'] = 0
+                coolant_outflow['flowrate'] = 0
+                self.send((message_time, coolant_outflow), 'coolant-outflow')
+            else:
+                coolant_outflow = self.__get_coolant_outflow(message_time)
+                #outflow_params = dict()
+                self.send((message_time, coolant_outflow), 'coolant-outflow')
+
+        # Interactions in the RCIS-outflow port
+        #-----------------------------------------
+        # one way "to" RCIS-outflow
+
+        # send to
+        if self.get_port('RCIS-outflow').connected_port:
+            message_time = self.recv('RCIS-outflow')
+
+            if self.RCIS:
+                coolant_outflow = self.__get_coolant_outflow(message_time)
+                coolant_outflow['flowrate'] = 5280 # kg/s
+                self.send((message_time, coolant_outflow), 'RCIS-outflow')
+            else:
+                coolant_outflow = self.__get_coolant_outflow(message_time)
+                coolant_outflow['flowrate'] = 0.0 # kg/s
+                self.send((message_time, coolant_outflow), 'RCIS-outflow')
 
         # Interactions in the coolant-inflow port
         #----------------------------------------
         # one way "from" coolant-inflow
 
-        #self.send( time, 'coolant-inflow' )
-
         # receive from
         if self.get_port('coolant-inflow').connected_port:
-
             self.send(time, 'coolant-inflow')
-            (check_time, inflow_cool_temp) = self.recv('coolant-inflow')
-
-            assert abs(check_time-time) <= 1e-6
-            self.params['inflow-cool-temp'] = inflow_cool_temp
-
-        # Interactions in the signal-out port
-        #-----------------------------------------
-        # one way "to" signal-out
-
-        # send to
-        if self.get_port('signal-out').connected_port:
 
-            message_time = self.recv('signal-out')
-
-            #signal_out = self.__get_signal_out(time)
+            if self.RCIS:
+                (check_time, _) = self.recv('coolant-inflow')
+                assert abs(check_time-time) <= 1e-6
+            else:
+                (check_time, inflow_cool_temp) = self.recv('coolant-inflow')
+                assert abs(check_time-time) <= 1e-6
+                self.params['inflow-cool-temp'] = inflow_cool_temp
 
-            #self.send( (message_time, signal_out), 'signal-out' )
+        # Interactions in the RCIS-inflow port
+        #----------------------------------------
+        # one way "from" RCIS-inflow
 
-    def __get_coolant_outflow(self, message_time):
+        # receive from
+        if self.get_port('RCIS-inflow').connected_port:
+            self.send(time, 'RCIS-inflow')
 
-        outflow = self.params['coolant-outflow']
-        return outflow
+            if self.RCIS:
+                (check_time, inflow_temp) = self.recv('RCIS-inflow')
+                assert abs(check_time-time) <= 1e-6
+                self.params['inflow-cool-temp'] = inflow_temp
+            else:
+                (check_time, _) = self.recv('RCIS-inflow')
+                assert abs(check_time-time) <= 1e-6
 
     def __step(self, time=0.0):
-        r'''
-        ODE IVP problem:
+        r"""ODE IVP problem.
         Given the initial data at :math:`t=0`,
         :math:`u = (u_1(0),u_2(0),\ldots)`
         solve :math:`\frac{\text{d}u}{\text{d}t} = f(u)` in the interval
         :math:`0\le t \le t_f`.
 
         Parameters
         ----------
         time: float
             Time in SI unit.
 
         Returns
         -------
         None
-
-        '''
-        import iapws.iapws97 as steam
+        """
+        #import iapws.iapws97 as steam
 
         # Get state values
-        u_0 = self.__get_state_vector( time )
+        u_0 = self.__get_state_vector(time)
 
         t_interval_sec = np.linspace(time, time+self.time_step, num=2)
 
-        (u_vec_hist, info_dict) = odeint( self.__f_vec,
-                                          u_0, t_interval_sec,
-                                          args=( self.params, ),
-                                          rtol=1e-4, atol=1e-8, mxstep=200,
-                                          full_output=True )
+        (u_vec_hist, info_dict) = odeint(self.__f_vec,
+                                         u_0, t_interval_sec,
+                                         args=(self.params,),
+                                         rtol=1e-4, atol=1e-8, mxstep=200,
+                                         full_output=True)
 
-        assert info_dict['message'] =='Integration successful.', info_dict['message']
+        assert info_dict['message'] == 'Integration successful.', info_dict['message']
 
-        u_vec = u_vec_hist[1,:]  # solution vector at final time step
+        u_vec = u_vec_hist[1, :]  # solution vector at final time step
 
-        n_dens    = u_vec[0]
-        c_vec     = u_vec[1:7]
+        n_dens = u_vec[0]
+        c_vec = u_vec[1:7]
         fuel_temp = u_vec[7]
         cool_temp = u_vec[8]
 
         #update state variables
-        outflow  = self.coolant_outflow_phase.get_row(time)
+        outflow = self.coolant_outflow_phase.get_row(time)
         neutrons = self.neutron_phase.get_row(time)
-        reactor  = self.reactor_phase.get_row(time)
+        reactor = self.reactor_phase.get_row(time)
         self.params['outflow temp'] = cool_temp
         time += self.time_step
 
         self.coolant_outflow_phase.add_row(time, outflow)
         self.neutron_phase.add_row(time, neutrons)
         self.reactor_phase.add_row(time, reactor)
 
         self.coolant_outflow_phase.set_value('temp', cool_temp, time)
         self.neutron_phase.set_value('neutron-dens', n_dens, time)
         self.neutron_phase.set_value('delayed-neutrons-cc', c_vec, time)
         self.reactor_phase.set_value('fuel-temp', fuel_temp, time)
 
         return time
 
-    def __signal_out(self, time=0.0):
-        '''
-        Send reactor signals to anyone requesting it.
+    def __get_signal_out(self, time):
+        """Determine whether the RCIS module should be on or off.
 
         Parameters
         ----------
         time: float
             Time in SI unit.
 
         Returns
         -------
-        None
-
-        '''
-
-        signals = dict()
+        signal: string
+            either 'online' or 'offline' to represent desired RCIS operation mode
+        """
+        if self.RCIS:
+            signal = 'online'
+            return(signal)
+        else:
+            signal = 'offline'
+            return(signal)
 
-        return signals
 
-    def __get_coolant_outflow(self, time=0.0):
-        '''
-        Get the coolant outflow stream.
+    def __get_coolant_outflow(self, time):
+        """Get the coolant outflow stream.
 
         Parameters
         ----------
         time: float
             Time in SI unit.
 
         Returns
         -------
         None
 
-        '''
+        """
 
         coolant_outflow_stream = dict()
-
+        
         outflow_cool_temp = self.coolant_outflow_phase.get_value('temp', time)
 
-        coolant_outflow_stream['temp'] = outflow_cool_temp
-        coolant_outflow_stream['quality'] = 0.7
+        if outflow_cool_temp <= 373.15:
+            coolant_outflow_stream['temp'] = outflow_cool_temp
+            coolant_outflow_stream['pressure'] = 0
+            coolant_outflow_stream['quality'] = 0
+            coolant_outflow_stream['flowrate'] = 0
+
+        else:
+
+            if self.params['valve_opened']:
+                pressure = steam._PSat_T(outflow_cool_temp)
+                base_temp = 373.15
+                base_pressure = steam._PSat_T(base_temp)
+                base_params = steam.IAPWS97(T=base_temp, x=0)
+                base_entropy = base_params.s
+                base_cp = base_params.cp
+                inlet_params = steam.IAPWS97(T=outflow_cool_temp, x=0)
+                inlet_cp = inlet_params.cp
+                average_cp = (base_cp + inlet_cp)/2
+
+                delta_s = average_cp * math.log(outflow_cool_temp/base_temp) - (unit.R/1000) * math.log(pressure/base_pressure)
+
+                inlet_entropy = (delta_s + base_entropy) * 1.25
+                bubl_entropy = inlet_params.s
+                bubl_enthalpy = inlet_params.h
+
+                inlet_params = steam.IAPWS97(T=base_temp, x=1)
+                dew_entropy = inlet_params.s
+                dew_enthalpy = inlet_params.h
+                quality = (inlet_entropy - bubl_entropy)/(dew_entropy - bubl_entropy)
+
+                delta_t = time - self.params['valve_opening_time']
+                mass_flowrate = 1820 * (1 - math.exp(-1 * delta_t/(3 * unit.minute)))
+
+                coolant_outflow_stream['temp'] = outflow_cool_temp
+                coolant_outflow_stream['pressure'] = pressure
+                coolant_outflow_stream['quality'] = quality
+                coolant_outflow_stream['flowrate'] = mass_flowrate
+
+            else:
+                self.params['valve_opened'] = True
+                self.params['valve_opening_time'] = time
+                coolant_outflow_stream['temp'] = 373.15
+                coolant_outflow_stream['pressure'] = 0
+                coolant_outflow_stream['quality'] = 0
+                coolant_outflow_stream['flowrate'] = 0
+
         return coolant_outflow_stream
 
     def __get_state_vector(self, time):
-        '''
-        Return a numpy array of all unknowns ordered as below:
+        """Return a numpy array of all unknowns ordered as below:
             neutron density (1), delayed neutron emmiter concentrations (6),
             termperature of fuel (1), temperature of coolant (1).
-        '''
+        """
 
-        u_vec = np.empty(0,dtype=np.float64)
+        u_vec = np.empty(0, dtype=np.float64)
 
-        neutron_dens = self.neutron_phase.get_value('neutron-dens',time)
-        u_vec = np.append( u_vec, neutron_dens )
+        neutron_dens = self.neutron_phase.get_value('neutron-dens', time)
+        u_vec = np.append(u_vec, neutron_dens)
 
-        delayed_neutrons_cc = self.neutron_phase.get_value('delayed-neutrons-cc',time)
+        delayed_neutrons_cc = self.neutron_phase.get_value('delayed-neutrons-cc', time)
         u_vec = np.append(u_vec, delayed_neutrons_cc)
 
-        fuel_temp = self.reactor_phase.get_value('fuel-temp',time)
-        u_vec = np.append( u_vec, fuel_temp)
+        fuel_temp = self.reactor_phase.get_value('fuel-temp', time)
+        u_vec = np.append(u_vec, fuel_temp)
 
-        temp = self.coolant_outflow_phase.get_value('temp',time)
+        temp = self.coolant_outflow_phase.get_value('temp', time)
         u_vec = np.append(u_vec, temp)
 
-        # sanity check
-
         return u_vec
 
     def __alpha_tn_func(self, temp, params):
-        import math
-        import scipy.misc as diff
-        import scipy.constants as unit
-        import iapws.iapws97 as steam
-        import iapws.iapws95 as steam2
-
-        pressure = steam._PSat_T(temp)
+        pressure = steam._PSat_T(temp) # vfda: why accessing protected method?
 
         d_rho = steam2.IAPWS95(P=pressure, T=temp-1).drhodT_P
 
-        #d_rho2 = diff.derivative(derivative_helper, temp) # dRho/dTm
-
         rho = 1 / steam._Region4(pressure, 0)['v'] # mass density, kg/m3
 
-        Nm = ((rho * unit.kilo)/params['mod molar mass']) * unit.N_A * (unit.centi)**3 # number density of the moderator
-        d_Nm =  ((d_rho * unit.kilo)/params['mod molar mass']) * unit.N_A * (unit.centi)**3 #dNm/dTm
-        d_Nm = d_Nm * unit.zepto * unit.milli
+        n_m = ((rho * unit.kilo)/self.mod_molar_mass) * unit.N_A * (unit.centi)**3
+        # number density of the moderator
+        d_nm = ((d_rho * unit.kilo)/self.mod_molar_mass) * unit.N_A * (unit.centi)**3 #dNm/dTm
+        d_nm = d_nm * unit.zepto * unit.milli
+
+        mod_macro_a = self.mod_micro_a * n_m
+        # macroscopic absorption cross section of the moderator
+        mod_macro_s = self.mod_micro_s * n_m
+        # macroscopic scattering cross section of the moderator
 
-        mod_macro_a = params['mod micro a'] * Nm # macroscopic absorption cross section of the moderator
-        mod_macro_s = params['mod micro s'] * Nm # macroscopic scattering cross section of the moderator
-
-        F = params['fuel macro a']/(params['fuel macro a'] + mod_macro_a) # thermal utilization, F
+        F = self.fuel_macro_a/(self.fuel_macro_a + mod_macro_a) # thermal utilization, F
     #dF/dTm
-        d_F = -1*(params['fuel macro a'] * params['mod micro a'] * d_Nm)/(params['fuel macro a'] + mod_macro_a)**2
+        d_f = -1*(self.fuel_macro_a * self.mod_micro_a * d_nm)/(
+            (self.fuel_macro_a + mod_macro_a)**2)
 
         # Resonance escape integral, P
-        P = math.exp((-1 * params['n fuel'] * (params['fuel_volume']) * params['I'])/(mod_macro_s * 3000))
+        P = math.exp((-1 * self.n_fuel * (self.fuel_volume) * self.I)/
+                     ((mod_macro_s * 3000)))
         #dP/dTm
-        d_P = P * (-1 * params['n fuel'] * params['fuel_volume'] * unit.centi**3 * params['mod micro s'] * d_Nm)/(mod_macro_s * 3000 * unit.centi**3)**2
+        d_p = P * (-1 * self.n_fuel * self.fuel_volume * unit.centi**3 *
+                   (self.mod_micro_s) * d_nm)/(mod_macro_s * 3000 * unit.centi**3)**2
 
-        Eth = 0.0862 * temp # convert temperature to energy in MeV
-        E1 = mod_macro_s/math.log(params['E0']/Eth) # neutron thermalization macroscopic cross section
+        e_th = 0.0862 * temp # convert temperature to energy in MeV
+        e_one = mod_macro_s/math.log(self.E0/e_th)
+        # neutron thermalization macroscopic cross section
 
-        Df = 1/(3 * mod_macro_s * (1 - params['mod mu0'])) # neutron diffusion coefficient
-        tau = Df/E1 # fermi age, tau
+        d_f = 1/(3 * mod_macro_s * (1 - self.mod_mu0)) # neutron diffusion coefficient
+        tau = d_f/e_one # fermi age, tau
         #dTau/dTm
-        d_tau = (((0.0862 * (Eth/params['E0'])) * 3 * Nm) - math.log(params['E0']/Eth) * (params['mod micro s'] * d_Nm))/((3 * Nm)**2 * (1 - params['mod mu0']))
+        d_tau = (((0.0862 * (e_th/self.E0)) * 3 * n_m) - math.log(self.E0/e_th) *
+                 ((self.mod_micro_s * d_nm))/((3 * n_m)**2 * (1 - self.mod_mu0)))
 
-        L = math.sqrt(1/(3 * mod_macro_s * mod_macro_a * (1 - params['mod mu0']))) # diffusion length L
+        L = math.sqrt(1/(3 * mod_macro_s * mod_macro_a * (1 - self.mod_mu0)))
+        # diffusion length L
         # dL/dTm
-        d_L = 1/(2 * math.sqrt((-2 * d_Nm * unit.zepto * unit.milli)/(3 * params['mod micro s'] * params['mod micro a'] * (Nm * unit.zepto * unit.milli)**3 * (1 - params['mod mu0']))))
+        d_l = 1/(2 * math.sqrt((-2 * d_nm * unit.zepto * unit.milli)/(3 * self.mod_micro_s * (self.mod_micro_a * (n_m * unit.zepto * unit.milli)**3 * ((1 - self.mod_mu0))))))
 
         # left term of the numerator of the moderator temperature feedback coefficient, alpha
-        left_1st_term = d_tau * (params['buckling']**2 + L**2 * params['buckling']**4) #holding L as constant
-        left_2nd_term = d_L * (2 * L * params['buckling']**2 + 2 * L * tau * params['buckling']**4) # holding tau as constant
-        left_term = (P * F) * (left_1st_term + left_2nd_term) # combining with P and F held as constant
-
-        # right term of the numerator of the moderator temperature feedback coefficient, alpha
-
-        right_1st_term = (-1) * (1 + ((tau + L**2) * params['buckling']**2) + tau * L**2 * params['buckling']**4) # num as const
-        right_2nd_term = F * d_P # holding thermal utilization as constant
-        right_3rd_term = P * d_F # holding resonance escpae as constant
-        right_term = right_1st_term * (right_2nd_term + right_3rd_term) # combining all three terms together
+        left_first_term = d_tau * (self.buckling**2 + L**2 * self.buckling**4)
+        #holding L as constant
+        left_second_term = d_l * (2 * L * self.buckling**2 + 2 * L *
+                                  (tau * self.buckling**4)) # holding tau as constant
+        left_term = (P * F) * (left_first_term + left_second_term)
+        # combining with P and F held as constant
+
+        right_1st_term = (-1) * (1 + ((tau + d_l**2) * self.buckling**2) + \
+                tau * d_l**2 * self.buckling**4) # num as const
+
+        right_first_term = (-1) * ((1 + ((tau + L**2) * self.buckling**2))
+                                   + tau * L**2 * self.buckling**4) # num as const
+        right_second_term = F * d_p # holding thermal utilization as constant
+        right_third_term = P * d_f # holding resonance escpae as constant
+        right_term = right_first_term * (right_second_term + right_third_term)
+        # combining all three terms together
 
         # numerator and denominator
         numerator = left_term + right_term
-        denominator = params['eta'] * params['epsilon'] * (F * P)**2
+        denominator = self.eta * self.epsilon * \
+                (F * P)**2
 
         alpha_tn = numerator/denominator
 
 
         alpha_tn = alpha_tn/3
+
         return alpha_tn
 
-    def __rho_func(self, time, n_dens, temp, params, ):
-        '''
-        Reactivity function.
+    def __rho_func(self, time, n_dens, temp, params):
+        """Reactivity function.
 
         Parameters
         ----------
         t: float, required
             Time.
         temp_f: float, required
             Temperature at time t.
@@ -418,55 +599,59 @@
         Returns
         -------
         rho_t: float
             Value of reactivity.
 
         Examples
         --------
-        '''
-
-        rho_0    = params['rho_0']
-        temp_ref = params['temp_0']
-        n_dens_ss_operation = params['n_dens_ss_operation']
-        alpha_n  = params['alpha_n']
+        """
 
-        if temp < 293.15: # if temperature is less than the starting temperature then moderator feedback is zero
+        rho_0 = self.rho_0
+        temp_ref = self.temp_o
+        #n_dens_ss_operation = params['n_dens_ss_operation']
+        alpha_n = self.alpha_n
+
+        if temp < 293.15:
+            # if temperature is less than the starting temperature then moderator
+            # feedback is zero
             alpha_tn = 0
 
         else:
-            alpha_tn = self.__alpha_tn_func(temp , self.params) #alpha_tn_func(temp, params)
+            alpha_tn = self.__alpha_tn_func(temp, self.params) #alpha_tn_func(temp, params)
 
-        if time > params['malfunction start'] and time < params['malfunction end']: # reg rod held in position; only mod temp reactivity varies with time during malfunction
-            alpha_n = params['alpha_n_malfunction']
+        if params['malfunction start'] < time < params['malfunction end']:
+            # reg rod held in position; only mod temp reactivity varies with time
+            # during malfunction
+            alpha_n = self.alpha_n_malfunction
             rho_t = rho_0 + alpha_n + alpha_tn * (temp - temp_ref)
 
-        elif time > params['shutdown time']: # effectively the inverse of startup; gradually reduce reactivity and neutron density.
+        elif time > params['shutdown time']:
+            # effectively the inverse of startup; gradually reduce reactivity and neutron density.
             rho_0 = -1 * rho_0
             alpha_n = rho_0 - (alpha_tn * (temp - temp_ref))
             rho_t = rho_0
 
-        elif n_dens < 1e-5: #controlled startup w/ blade; gradually increase neutron density to SS value.
+        elif n_dens < 1e-5:
+            #controlled startup w/ blade; gradually increase neutron density to SS value.
             #rho_current = (1 - n_dens) * rho_0
             #alpha_n = rho_current - rho_0 - alpha_tn * (temp - temp_ref)
             #rho_t = rho_current
-            #params['alpha_n_malfunction'] = alpha_n
+            #self.alpha_n_malfunction = alpha_n
             rho_t = rho_0
 
         else:
             rho_current = (1 - n_dens) * rho_0
-            alphh_n = rho_current - rho_0 - alpha_tn * (temp - temp_ref)
+            alpha_n = rho_current - rho_0 - alpha_tn * (temp - temp_ref)
             rho_t = rho_current
-            params['alpha_n_malfunction'] = alpha_n
-        #print(n_dens)
+            self.alpha_n_malfunction = alpha_n
 
         return (rho_t, alpha_n, alpha_tn * (temp - temp_ref))
 
     def __q_source(self, time, params):
-        '''
-        Neutron source delta function.
+        """Neutron source delta function.
 
         Parameters
         ----------
         t: float, required
             Time.
         params: dict, required
             Dictionary of quantities. It must have a `'q_0'` key/value pair.
@@ -474,152 +659,147 @@
         Returns
         -------
         q: float
             Value of source.
 
         Examples
         --------
-        '''
-        q_0 = params['q_0']
+        """
+        q_0 = self.q_0
 
-        if time <= 1500: # small time value
-            q = q_0
+        if time <= 30 and params['shutdown-mode'] == False: # small time value
+            q_source = q_0
         else:
-            q = 0.0
-            params['q_source_status'] = 'out'
+            q_source = 0.0
+            self.q_source_status = 'out'
 
-        return q
+        return q_source
 
     def __sigma_fis_func(self, temp, params):
-        '''
-        Place holder for implementation
-        '''
-        sigma_f = params['sigma_f_o']  * math.sqrt(298/temp) * math.sqrt(math.pi) * 0.5
+        """Place holder for implementation
+        """
+        sigma_f = self.sigma_f_o  * math.sqrt(298/temp) * math.sqrt(math.pi) * 0.5
 
-        return(sigma_f)
+        return sigma_f
 
-    def __nuclear_pwr_dens_func(self, time, temp, n_dens, params ):
-        '''
-        Place holder for implementation
-        '''
-        n_dens = n_dens + self.__q_source(time, self.params) # include the neutrons from the initial source
+    def __nuclear_pwr_dens_func(self, time, temp, n_dens, params):
+        """Place holder for implementation.
+        """
+        # include the neutrons from the initial source
 
-        rxn_heat = params['fis_energy'] # get fission reaction energy J per reaction
+        rxn_heat = self.fis_energy # get fission reaction energy J per reaction
 
-        sigma_f = self.__sigma_fis_func( temp, self.params ) # m2
+        sigma_f = self.__sigma_fis_func(temp, self.params) # m2
 
-        fis_nuclide_num_dens = params['fis_nuclide_num_dens_fake'] #  #/m3
+        fis_nuclide_num_dens = self.fis_nuclide_num_dens #  #/m3
 
-        Sigma_fis = sigma_f * fis_nuclide_num_dens # macroscopic cross section
+        sigma_fis = sigma_f * fis_nuclide_num_dens # macroscopic cross section
 
-        v_o = params['thermal_neutron_velo'] # m/s
+        v_o = self.thermal_neutron_velo # m/s
 
-        neutron_flux = n_dens * 0.95E15 * v_o * sigma_f/params['sigma_f_o']*0.7
+        neutron_flux = n_dens * 0.9E15 * v_o * sigma_f/self.sigma_f_o*0.7
 
          #reaction rate density
-        rxn_rate_dens = Sigma_fis * neutron_flux
+        rxn_rate_dens = sigma_fis * neutron_flux
 
         # nuclear power source
         q3prime = - rxn_heat * rxn_rate_dens # exothermic reaction W/m3)
-        #q3prime = - n_dens * 3323E6
-        #print("q3prime")
-        #print(q3prime)
 
+        # add decay heat
+        if self.params['shutdown-mode']:
+            t_0 = unit.hour * 24 # assume 24 hours of steady state operation before shutdown
+            p_0 = self.params['decay-heat-0']
+            p_t = p_0 * (((time + 1) ** -0.2) - (t_0 + time) ** -0.2)
+            q3prime += p_t
+        
         return q3prime
 
     def __heat_sink_rate(self, time, temp_f, temp_c, params):
 
-        ht_coeff = params['ht_coeff']
+        ht_coeff = self.ht_coeff
 
         q_f = - ht_coeff * (temp_f - temp_c)
-        #print(q_f)
         return q_f
 
     def __f_vec(self, u_vec, time, params):
         num_negatives = u_vec[u_vec < 0]
 
         if num_negatives.any() < 0:
             assert np.max(abs(u_vec[u_vec < 0])) <= 1e-8, 'u_vec = %r'%u_vec
 
         #assert np.all(u_vec >= 0.0), 'u_vec = %r'%u_vec
         q_source_t = self.__q_source(time, self.params)
 
         n_dens = u_vec[0] # get neutron dens
 
-        c_vec  = u_vec[1:-2] # get delayed neutron emitter concentration
+        c_vec = u_vec[1:-2] # get delayed neutron emitter concentration
 
         temp_f = u_vec[-2] # get temperature of fuel
 
         temp_c = u_vec[-1] # get temperature of coolant
 
-        # initialize f_vec to zero 
-        species_decay = params['species_decay']
+        # initialize f_vec to zero
+        species_decay = self.species_decay
         lambda_vec = np.array(species_decay)
-        n_species  = len(lambda_vec)
-
-        f_tmp = np.zeros(1+n_species+2,dtype=np.float64) # vector for f_vec return
+        n_species = len(lambda_vec)
 
+        f_tmp = np.zeros(1+n_species+2, dtype=np.float64) # vector for f_vec return
         #----------------
         # neutron balance
         #----------------
         rho_t = self.__rho_func(time, n_dens, temp_c, self.params)[0]
 
-        beta = params['beta']
-        gen_time = params['gen_time']
+        beta = self.beta
+        gen_time = self.gen_time
 
-        assert len(lambda_vec)==len(c_vec)
+        assert len(lambda_vec) == len(c_vec)
 
         f_tmp[0] = (rho_t - beta)/gen_time * n_dens + lambda_vec @ c_vec + q_source_t
 
         #-----------------------------------
         # n species balances (implicit loop)
         #-----------------------------------
 
-        species_rel_yield = params['species_rel_yield']
+        species_rel_yield = self.species_rel_yield
         beta_vec = np.array(species_rel_yield) * beta
 
-        assert len(lambda_vec)==len(c_vec)
-        assert len(beta_vec)==len(c_vec)
-        #species are in RELATIVE yield, not actual; multiply by delayed neutron
-        #yield fraction of 0.0065 to get the actual delayed neutron
-        #concentration
+        assert len(lambda_vec) == len(c_vec)
+        assert len(beta_vec) == len(c_vec)
 
         f_tmp[1:-2] = beta_vec / gen_time * n_dens - lambda_vec * c_vec
 
-
         #--------------------
         # fuel energy balance
         #--------------------
-        rho_f    = params['fuel_dens']
-        cp_f     = params['cp_fuel']
-        vol_fuel = params['fuel_volume']
+        rho_f = self.fuel_dens
+        cp_f = self.cp_fuel
+        vol_fuel = self.fuel_volume
 
-        pwr_dens  = self.__nuclear_pwr_dens_func( time, (temp_f+temp_c)/2, n_dens, self.params)
+        pwr_dens = self.__nuclear_pwr_dens_func(time, (temp_f+temp_c)/2,
+                                                n_dens, self.params)
 
-        heat_sink = self.__heat_sink_rate( time, temp_f, temp_c, self.params)
+        heat_sink = self.__heat_sink_rate(time, temp_f, temp_c, self.params)
 
         #assert heat_sink <= 0.0,'heat_sink = %r'%heat_sink
 
-        f_tmp[-2] =  -1/rho_f/cp_f * ( pwr_dens - heat_sink/vol_fuel )
+        f_tmp[-2] = -1/rho_f/cp_f * (pwr_dens - heat_sink/vol_fuel)
 
         #-----------------------
         # coolant energy balance
         #-----------------------
-        rho_c    = params['coolant_dens']
-        cp_c     = params['cp_coolant']
-        vol_cool = params['coolant_volume']
+        rho_c = self.coolant_dens
+        cp_c = self.cp_coolant
+        vol_cool = self.coolant_volume
 
         # subcooled liquid
         pump_out = params['inflow-cool-temp']
 
-        tau = params['tau_fake']
+        tau = self.tau
 
         heat_source = heat_sink
         temp_in = pump_out
 
         f_tmp[-1] = - 1/tau * (temp_c - temp_in) - 1./rho_c/cp_c/vol_cool * heat_source
+        
+        f_tmp[:] = [0 if np.isnan(x) else x for x in f_tmp] #nifty conditional mutator
 
-        # pressure calculations
-
-        #print(time)
-        #print(u_vec)
         return f_tmp
```

### Comparing `cortix-1.1.8/cortix/examples/bwr/turbine.py` & `cortix-1.1.9/cortix/examples/bwr/turbine.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,285 +1,316 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # This file is part of the Cortix toolkit environment.
 # https://cortix.org
+"""
+Cortix Example Module
+"""
 
 import logging
 from copy import deepcopy
 
-import numpy as np
-import scipy.constants as const
-from scipy.integrate import odeint
-import scipy.constants as sc
+import scipy.constants as unit
+import numpy as math
 
 import iapws.iapws97 as steam_table
 
 from cortix import Module
 from cortix.support.phase_new import PhaseNew as Phase
 from cortix import Quantity
 
 class Turbine(Module):
-    '''
-    Boiling water reactor single-point reactor.
+    """Boiling water single-point reactor.
 
     Notes
     -----
     These are the `port` names available in this module to connect to respective
     modules: `turbine`, and `pump`.
     See instance attribute `port_names_expected`.
 
-    '''
+    """
 
     def __init__(self, params):
-        '''
+        """Constructor.
+
         Parameters
         ----------
         params: dict
             All parameters for the module in the form of a dictionary.
 
-        '''
+        """
 
         super().__init__()
 
         self.params = deepcopy(params)
+        self.params['entropy'] = 4.5 # Kj/Kg-K
+
+        self.port_names_expected = ['inflow', 'outflow-1', 'outflow-2']
 
-        self.port_names_expected = ['inflow','outflow-1','outflow-2']
+        self.initial_time = params['start-time']
+        self.end_time = params['end-time']
 
-        self.initial_time = 0.0 * const.day
-        self.end_time     = 4 * const.hour
-        self.time_step    = 10.0
-        self.show_time    = (False,10.0)
+        self.time_step = 10.0
+        self.show_time = (False, 10.0)
 
         self.log = logging.getLogger('cortix')
+        self.efficiency = 0.8
 
         # Inflow phase history
         quantities = list()
 
-        temp = Quantity(name='temp', formal_name = 'T_in', unit='k', value=273.15,
-                info='Turbine Steam Inflow Temperature', latex_name='$T_i$')
+        temp = Quantity(name='temp', formal_name='T_in', unit='K', value=params['coolant-temp'],
+                        info='Turbine Steam Inflow Temperature', latex_name=r'$T_i$')
 
         quantities.append(temp)
 
-        self.inflow_phase = Phase(self.initial_time, time_unit = 's',
-                quantities = quantities)
+        self.inflow_phase = Phase(time_stamp=self.initial_time, time_unit='s',
+                                  quantities=quantities)
 
         # Outflow phase history
         quantities = list()
 
-        temp = Quantity(name='temp', formal_name='T_o', unit='k', value=273.15,
-                info='Turbine Steam Outflow Temperature', latex_name='$T_o$')
+        temp = Quantity(name='temp', formal_name='T_o', unit='K', value=params['turbine-outflow-temp'],
+                        info='Turbine Steam Outflow Temperature', latex_name=r'$T_o$')
 
         quantities.append(temp)
 
-        press = Quantity(name='pressure', formal_name='P_t', unit = 'Pa',
-                value=params['runoff-pressure'],
-                info='Turbine Steam Outflow Pressure', latex_name='$P_t$')
+        press = Quantity(name='pressure', formal_name='P_t', unit='Pa',
+                         value=params['runoff-pressure'],
+                         info='Turbine Steam Outflow Pressure', latex_name=r'$P_t$')
 
         quantities.append(press)
 
-        x = Quantity(name='quality', formal_name='chi_t', unit='%', value=0.0,
-                info='Turbine Steam Outflow Quality', latex_name='$\chi_t$')
+        x = Quantity(name='quality', formal_name='chi_t', unit='%', value=params['turbine-chi'],
+                     info='Turbine Steam Outflow Quality', latex_name=r'$\chi_t$')
 
         quantities.append(x)
 
-        work = Quantity(name='power', formal_name='P_t', unit='W', value=0.0,
-                info='Turbine Power', latex_name='$W_t$')
+        work = Quantity(name='power', formal_name='P_t', unit='W', value=params['turbine-work'],
+                        info='Turbine Power', latex_name=r'$W_t$')
 
         quantities.append(work)
 
-        self.outflow_phase = Phase(self.initial_time, time_unit = 's',
-                quantities = quantities)
+        flowrate = Quantity(name='flowrate', formal_name='m', unit='kg/s', value=params['initial-flowrate'], info='Mass Flowrate', latex_name=r'$/dot m$')
 
-        return
+        quantities.append(flowrate)
+
+        self.outflow_phase = Phase(time_stamp=self.initial_time, time_unit='s',
+                                   quantities=quantities)
 
     def run(self, *args):
 
         time = self.initial_time
 
         while time < self.end_time + self.time_step:
 
-            if self.show_time[0] and abs(time%self.show_time[1]-0.0)<=1.e-1:
-                self.log.info('time = '+str(round(time/const.minute,1)))
+            if self.show_time[0] and abs(time%self.show_time[1]-0.0) <= 1.e-1:
+                msg = 'time = '+str(round(time/unit.minute, 1))
+                self.log.info(msg)
 
             # Communicate information
             #------------------------
             self.__call_ports(time)
 
             # Evolve one time step
             #---------------------
 
-            time = self.__step( time )
+            time = self.__step(time)
 
+    def module_tester(self):
         return
 
     def __call_ports(self, time):
 
         # Interactions in the steam-outflow-1 port
         #-----------------------------------------
         # one way "to" outflow-1
 
-        # to 
+        # to
         if self.get_port('outflow-1').connected_port:
-
+            print(self.params['high_pressure_turbine'])
             message_time = self.recv('outflow-1')
 
             outflow_state = dict()
 
             steam_temp = self.outflow_phase.get_value('temp', time)
             steam_quality = self.outflow_phase.get_value('quality', time)
-            steam_press = self.outflow_phase.get_value('pressure', time)
+            steam_press = self.params['turbine_inlet_pressure']
+            steam_flowrate = self.outflow_phase.get_value('flowrate', time)
+
 
             outflow_state['temp'] = steam_temp
             outflow_state['quality'] = steam_quality
-            outflow_state['press'] = steam_press
+            outflow_state['pressure'] = steam_press
+            outflow_state['flowrate'] = steam_flowrate
 
-            self.send( (message_time, outflow_state), 'outflow-1' )
+            if self.params['high_pressure_turbine'] == False:
+                outflow_state['flowrate'] *= 2
+
+            else:
+                outflow_state['flowrate'] *= 0.5
+
+            self.send((message_time, outflow_state), 'outflow-1')
 
         # Interactions in the steam-outflow-2 port
         #-----------------------------------------
         # one way "to" outflow-2
 
-        # to 
+        # to
         if self.get_port('outflow-2').connected_port:
 
             message_time = self.recv('outflow-2')
 
             outflow_state = dict()
 
             steam_temp = self.outflow_phase.get_value('temp', time)
             steam_quality = self.outflow_phase.get_value('quality', time)
-            steam_press = self.outflow_phase.get_value('pressure', time)
+            steam_press = self.params['turbine_outlet_pressure']
+            steam_flowrate = self.outflow_phase.get_value('flowrate', time)
 
             outflow_state['temp'] = steam_temp
             outflow_state['quality'] = steam_quality
-            outflow_state['press'] = steam_press
+            outflow_state['pressure'] = steam_press
+            outflow_state['flowrate'] = steam_flowrate
+
+            if self.params['high_pressure_turbine'] == False:
+                outflow_state['flowrate'] *= 2
 
-            self.send( (message_time, outflow_state), 'outflow-2' )
+            else:
+                outflow_state['flowrate'] *= 0.5
+
+            self.send((message_time, outflow_state), 'outflow-2')
 
         # Interactions in the steam-inflow port
         #----------------------------------------
         # one way "from" inflow
 
         # from
         if self.get_port('inflow').connected_port:
 
-            self.send( time, 'inflow' )
+            self.send(time, 'inflow')
 
             (check_time, inflow_state) = self.recv('inflow')
             assert abs(check_time-time) <= 1e-6
 
             self.temp = inflow_state['temp']
-            self.chi  = inflow_state['quality']
+            self.chi = inflow_state['quality']
+            self.pressure = inflow_state['pressure']
+            self.flowrate = inflow_state['flowrate']
 
-        return
+            if self.params['high_pressure_turbine'] == False:
+                self.flowrate = self.flowrate * 0.5
 
     def __step(self, time=0.0):
-        r'''
+        r"""
         Advance the state of the turbine.
 
         Parameters
         ----------
         time: float
             Time in SI unit.
 
         Returns
         -------
         None
-
-        '''
-        import iapws.iapws97 as steam
-
-        output = self.__turbine(time, self.temp, self.chi, self.params)
+        """
+        output = self.__turbine(time, self.temp, self.chi, self.pressure, self.flowrate, self.params)
 
         tmp = self.outflow_phase.get_row(time)
 
         time += self.time_step
 
         self.outflow_phase.add_row(time, tmp)
 
         t_runoff = output[0]
 
         x_runoff = output[2]
-        if x_runoff < 0 and x_runoff != -1:
-            x_runoff = 0
+
+        m_runoff = output[3]
+
+        #if x_runoff < 0 and x_runoff != -1:
+            #x_runoff = 0
 
         w_turbine = output[1]
 
         self.outflow_phase.set_value('power', w_turbine, time)
         self.outflow_phase.set_value('quality', x_runoff, time)
         self.outflow_phase.set_value('temp', t_runoff, time)
+        self.outflow_phase.set_value('flowrate', m_runoff, time)
 
         return time
 
-    def __turbine(self, time, temp_in, x,  params):
-        #expand the entering steam from whatever temperature and pressure it enters at to 0.035 kpa, with 80% efficiency.
-        #pressure of steam when it enters the turbine equals the current reactor operating pressure
-        if self.params['high_pressure_turbine'] == True:
-            p_in = steam_table._PSat_T(temp_in)
-            #print('not evaluated')
-        else:
-            #print('evaluated')
-            p_in = self.params['turbine_inlet_pressure']
+    def __turbine(self, time, temp_in, chi_in, p_in, flowrate, params):
+        # Expand the entering steam from whatever temperature and pressure it enters
+        # at to 0.035 kpa, with 80% efficiency.
 
-        p_out = self.params['turbine_outlet_pressure']
- 
-        if temp_in <= 273.15 or p_in <= p_out: # if temp is below this the turbine will not work
-            t_runoff = temp_in
-            w_real = 0
-            x = 0
-            return (t_runoff, w_real, x)
+        if flowrate == 0:
+            return(293.15, 0, 0, 0)
 
-        if temp_in < 373.15:
-            t_runoff = steam_table._TSat_P(p_out)
+        if temp_in < steam_table._TSat_P(0.5) and self.params['high_pressure_turbine'] == False:
+            t_runoff = steam_table._TSat_P(0.5)
             w_real = 0
-            x = -3
-            return (t_runoff, w_real, x)
-
-        #properties of the inlet steam
+            runoff_quality = 0
+            return(t_runoff, w_real, runoff_quality)
 
-        inlet_parameters = steam_table._Region4(p_in, x)
+        # vfda: access of a protected member?
+        inlet_parameters = steam_table._Region4(p_in, chi_in)
         inlet_entropy = inlet_parameters['s']
         inlet_enthalpy = inlet_parameters['h']
 
+        p_out = self.params['turbine_outlet_pressure']
+
         #bubble and dewpoint properties at turbine outlet
+        # vfda: access of a protected member?
         bubl = steam_table._Region4(p_out, 0)
+        # vfda: access of a protected member?
         dew = steam_table._Region4(p_out, 1)
         bubl_entropy = bubl['s']
         dew_entropy = dew['s']
         bubl_enthalpy = bubl['h']
         dew_enthalpy = dew['h']
+        #print(bubl_entropy, inlet_entropy, dew_entropy, self.params['high_pressure_turbine'])
 
         #if the ideal runoff is two-phase mixture:
-        if inlet_entropy < dew_entropy and inlet_entropy > bubl_entropy:
+        #if inlet_entropy < dew_entropy and inlet_entropy > bubl_entropy:
+        if  bubl_entropy < inlet_entropy < dew_entropy:
             x_ideal = (inlet_entropy - bubl_entropy)/(dew_entropy - bubl_entropy)
+            # vfda: access of a protected member?
             h_ideal = steam_table._Region4(p_out, x_ideal)['h']
 
         #if the ideal runoff is a superheated steam
-        elif inlet_entropy > dew_entropy:
-            t_ideal = steam_table._Backward2_T_Ps(p_out, inlet_entropy)
-            h_ideal = steam_table._Region2(t_ideal, p_out)['h']
+        #elif inlet_entropy > dew_entropy:
+            # vfda: access of a protected member?
+            #t_ideal = steam_table._Backward2_T_Ps(p_out, inlet_entropy)
+            # vfda: access of a protected member?
+            #h_ideal = steam_table._Region2(t_ideal, p_out)['h']
 
         #calculate the real runoff enthalpy
         w_ideal = inlet_enthalpy - h_ideal #on a per mass basis
         #assert(w_ideal > 0)
-        w_real = w_ideal * params['turbine efficiency']
+        w_real = w_ideal * self.efficiency
         h_real = inlet_enthalpy - w_ideal
-        assert(h_real > 0)
+        assert h_real > 0
+        if w_real < 0:
+            w_real = 0
 
         # if the real runoff is a superheated steam
         if h_real > dew_enthalpy:
+            # vfda: access of a protected member?
             t_runoff = steam_table._Backward2_T_Ph(p_out, h_real)
             x_runoff = -1 # superheated steam
 
         #if the real runoff is a subcooled liquid
         elif h_real < bubl_enthalpy:
+            # vfda: access of a protected member?
             t_runoff = steam_table._Backward1_T_Ph(p_out, h_real)
             x_runoff = 2 # subcooled liquid
 
-        #if the real runoff is a two-phase mixture    
+        #if the real runoff is a two-phase mixture
         else:
-            x_runoff = (h_real - bubl_enthalpy)/(dew_enthalpy - bubl_enthalpy) # saturated vapor
+            # saturated vapor
+            x_runoff = (h_real - bubl_enthalpy)/(dew_enthalpy - bubl_enthalpy)
+            # vfda: access of a protected member?
             t_runoff = steam_table._TSat_P(p_out)
+        w_real = w_real * flowrate * unit.kilo
 
-        w_real = w_real * params['steam flowrate'] * sc.kilo
-        #w_real = heat_removed
-        return (t_runoff, w_real, x_runoff)
+        return (t_runoff, w_real, x_runoff, flowrate)
```

### Comparing `cortix-1.1.8/cortix/examples/city_justice/adjudication.py` & `cortix-1.1.9/cortix/examples/city_justice/adjudication.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/city_justice/arrested.py` & `cortix-1.1.9/cortix/examples/city_justice/arrested.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/city_justice/community.py` & `cortix-1.1.9/cortix/examples/city_justice/community.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,102 +1,112 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # This file is part of the Cortix toolkit environment.
-# https://cortix.org
-
 import logging
 
 import numpy as np
 import scipy.constants as unit
 from scipy.integrate import odeint
 
 from cortix import Module
 from cortix import Phase
 from cortix import Quantity
 
 class Community(Module):
-    '''
-    Community Cortix module used to model criminal group population in a
-    community system.  Community here is the system at large with all possible
-    adult individuals included in a society.
+    """Community model with criminal group population.
+
+    Community here is the system at large with all possible
+    adult individuals included in any given society.
 
     Notes
     -----
     These are the `port` names available in this module to connect to respective
-    modules: `probation`, `adjudication`, `jail`, `prison`, `arrested`, and `parole`.
+    modules:
+
+     + `probation`,
+     + `adjudication`,
+     + `jail`, `prison`,
+     + `arrested`, and
+     + `parole`.
+
     See instance attribute `port_names_expected`.
 
-    '''
+    """
 
-    def __init__(self, n_groups=1, non_offender_adult_population=100, 
+    def __init__(self, n_groups=1, non_offender_adult_population=100,
                  offender_pool_size=0.0, free_offender_pool_size=0.0):
-        '''
+        """Constructor.
+
         Parameters
         ----------
         n_groups: int
             Number of groups in the population.
         non_offender_adult_population: float
             Pool of individuals reaching the adult age (SI) unit. Default: 100.
         offender_pool_size: float
             Upperbound on the range of the existing population groups. A random value
             from 0 to the upperbound value will be assigned to each group. This is
             typically a small number, say a fraction of a percent.
 
-        '''
+        """
 
         super().__init__()
 
-        self.port_names_expected = ['probation','adjudication','jail','prison',
+        self.port_names_expected = ['probation', 'adjudication', 'jail', 'prison',
                                     'arrested', 'parole']
 
-        quantities      = list()
+        quantities = list()
         self.ode_params = dict()
 
         self.initial_time = 0.0 * unit.day
-        self.end_time     = 100 * unit.day
-        self.time_step    = 0.5 * unit.day
-        self.show_time    = (False,10*unit.day)
+        self.end_time = 100 * unit.day
+        self.time_step = 0.5 * unit.day
+        self.show_time = (False, 10*unit.day)
         self.log = logging.getLogger('cortix')
 
         unit.percent = 1/100
 
         # Population groups
         self.n_groups = n_groups
 
         # Community non-offender population
         n0_0 = np.array([float(non_offender_adult_population)])
-        n0   = Quantity(name='n0', formal_name='non-offender-adult-pop',
-                latex_name = '$n_0$',
-                unit='# adults', value=n0_0, info='Non-Offender Adult Population')
+        n0 = Quantity(name='n0', formal_name='non-offender-adult-pop',
+                      latex_name='$n_0$',
+                      unit='# adults', value=n0_0,
+                      info='Non-Offender Adult Population')
         quantities.append(n0)
 
-        # Community free-offender population groups 
+        # Community free-offender population groups
         f0g_0 = np.random.random(self.n_groups) * offender_pool_size
         f0g = Quantity(name='f0g', formal_name='free-offender-pop-grps',
-                latex_name = '$n_0^{(g)}$',
-                unit='# offenders', value=f0g_0, info='Free-Offender Population Groups')
+                       latex_name='$n_0^{(g)}$',
+                       unit='# offenders', value=f0g_0,
+                       info='Free-Offender Population Groups')
         quantities.append(f0g)
 
         # Model parameters: commitment coefficients
 
         # Community non-offenders to offenders (arrested)
         a = 0.6*unit.percent/unit.year * np.ones(self.n_groups)
         b = 0.8*unit.percent/unit.year * np.ones(self.n_groups)
         c00g_0 = (a + (b-a)*np.random.random(self.n_groups)) / self.n_groups
-        c00g = Quantity(name='c00g', formal_name='non-offenders-commit-arrested-coeff-grps',
-               unit='1/s', value=c00g_0)
+        c00g = Quantity(name='c00g',
+                        formal_name='non-offenders-commit-arrested-coeff-grps',
+                        unit='1/s', value=c00g_0)
         self.ode_params['non-offenders-commit-to-arrested-coeff-grps'] = c00g_0
         quantities.append(c00g)
 
         # Community free-offenders to arrested (recidivism)
         a = 0.8*unit.percent/unit.year * np.ones(self.n_groups)
         b = 0.9*unit.percent/unit.year * np.ones(self.n_groups)
         c0rg_0 = (a + (b-a)*np.random.random(self.n_groups)) / self.n_groups
-        c0rg = Quantity(name='c0rg', formal_name='free-offenders-commit-arrested-coeff-grps',
-               unit='1/s', value=c0rg_0)
+        c0rg = Quantity(name='c0rg',
+                        formal_name='free-offenders-commit-arrested-coeff-grps',
+                        value=c0rg_0, unit='1/s')
         self.ode_params['free-offenders-commit-to-arrested-coeff-grps'] = c0rg_0
         quantities.append(c0rg)
 
         # Death term for community offenders
         a = 0.8*unit.percent/unit.year * np.ones(self.n_groups)
         b = 1.0*unit.percent/unit.year * np.ones(self.n_groups)
         d0g_0 = (a + (b-a)*np.random.random(self.n_groups)) / self.n_groups
@@ -113,108 +123,106 @@
         b = 2.5*unit.percent/unit.year
         s0_0 = a + (b-a)*np.random.random()
         self.ode_params['non-offenders-maturity-rate-coeff'] = s0_0
         self.ode_params['non_offender_adult_population'] = non_offender_adult_population
 
         # Phase state
         self.population_phase = Phase(self.initial_time, time_unit='s',
-                quantities=quantities)
+                                      quantities=quantities)
 
         self.population_phase.SetValue('n0', n0_0, self.initial_time)
         self.population_phase.SetValue('f0g', f0g_0, self.initial_time)
 
         # Initialize inflows to zero
-        self.ode_params['prison-inflow-rates']       = np.zeros(self.n_groups)
-        self.ode_params['parole-inflow-rates']       = np.zeros(self.n_groups)
-        self.ode_params['arrested-inflow-rates']     = np.zeros(self.n_groups)
-        self.ode_params['jail-inflow-rates']         = np.zeros(self.n_groups)
+        self.ode_params['prison-inflow-rates'] = np.zeros(self.n_groups)
+        self.ode_params['parole-inflow-rates'] = np.zeros(self.n_groups)
+        self.ode_params['arrested-inflow-rates'] = np.zeros(self.n_groups)
+        self.ode_params['jail-inflow-rates'] = np.zeros(self.n_groups)
         self.ode_params['adjudication-inflow-rates'] = np.zeros(self.n_groups)
-        self.ode_params['probation-inflow-rates']    = np.zeros(self.n_groups)
-
-        return
+        self.ode_params['probation-inflow-rates'] = np.zeros(self.n_groups)
 
     def run(self, *args):
 
         self.__zero_ode_parameters()
 
         time = self.initial_time
 
         while time <= self.end_time:
 
-            if self.show_time[0] and abs(time%self.show_time[1]-0.0)<=1.e-1:
-                self.log.info('Community::time[d] = '+str(round(time/unit.day,1)))
+            if self.show_time[0] and abs(time%self.show_time[1]-0.0) <= 1.e-1:
+                self.log.info('Community::time[d] = '+str(round(time/unit.day, 1)))
 
             self.__call_ports(time)
 
             # Evolve offenders group population to the next time stamp
             #---------------------------------------------------------
 
-            time = self.__step( time )
+            time = self.__step(time)
 
     def __call_ports(self, time):
 
-            # Interactions in the jail port
-            #--------------------------------
-            # one way "from" jail
-
-            self.send( time, 'jail' )
-            (check_time, inflow_rates) = self.recv('jail')
-            assert abs(check_time-time) <= 1e-6
-            self.ode_params['jail-inflow-rates'] = inflow_rates
-
-            # Interactions in the adjudication port
-            #--------------------------------------
-            # one way "from" adjudication
-
-            self.send( time, 'adjudication' )
-            (check_time, inflow_rates) = self.recv('adjudication')
-            assert abs(check_time-time) <= 1e-6
-            self.ode_params['adjudication-inflow-rates'] = inflow_rates
-
-            # Interactions in the probation port
-            #--------------------------------
-            # one way "from" probation
-
-            self.send( time, 'probation' )
-            (check_time, inflow_rates) = self.recv('probation')
-            assert abs(check_time-time) <= 1e-6
-            self.ode_params['probation-inflow-rates'] = inflow_rates
-
-            # Interactions in the prison port
-            #--------------------------------
-            # one way "from" prison
-
-            self.send( time, 'prison' )
-            (check_time, inflow_rates) = self.recv('prison')
-            assert abs(check_time-time) <= 1e-6
-            self.ode_params['prison-inflow-rates'] = inflow_rates
-
-            # Interactions in the parole port
-            #--------------------------------
-            # one way "from" parole
-
-            self.send( time, 'parole' )
-            (check_time, inflow_rates) = self.recv('parole')
-            assert abs(check_time-time) <= 1e-6
-            self.ode_params['parole-inflow-rates'] = inflow_rates
-
-            # Interactions in the arrested port
-            #--------------------------------
-            # two way "to" and "from" arrested
-
-            # to
-            message_time = self.recv('arrested')
-            outflow_rates = self.__compute_outflow_rates( message_time, 'arrested' )
-            self.send( (message_time, outflow_rates), 'arrested' )
-
-            # from
-            self.send( time, 'arrested' )
-            (check_time, inflow_rates) = self.recv('arrested')
-            assert abs(check_time-time) <= 1e-6
-            self.ode_params['arrested-inflow-rates'] = inflow_rates
+        # Interactions in the jail port
+        #--------------------------------
+        # one way "from" jail
+
+        self.send(time, 'jail')
+        (check_time, inflow_rates) = self.recv('jail')
+        assert abs(check_time-time) <= 1e-6
+        self.ode_params['jail-inflow-rates'] = inflow_rates
+
+        # Interactions in the adjudication port
+        #--------------------------------------
+        # one way "from" adjudication
+
+        self.send(time, 'adjudication')
+        (check_time, inflow_rates) = self.recv('adjudication')
+        assert abs(check_time-time) <= 1e-6
+        self.ode_params['adjudication-inflow-rates'] = inflow_rates
+
+        # Interactions in the probation port
+        #--------------------------------
+        # one way "from" probation
+
+        self.send(time, 'probation')
+        (check_time, inflow_rates) = self.recv('probation')
+        assert abs(check_time-time) <= 1e-6
+        self.ode_params['probation-inflow-rates'] = inflow_rates
+
+        # Interactions in the prison port
+        #--------------------------------
+        # one way "from" prison
+
+        self.send(time, 'prison')
+        (check_time, inflow_rates) = self.recv('prison')
+        assert abs(check_time-time) <= 1e-6
+        self.ode_params['prison-inflow-rates'] = inflow_rates
+
+        # Interactions in the parole port
+        #--------------------------------
+        # one way "from" parole
+
+        self.send(time, 'parole')
+        (check_time, inflow_rates) = self.recv('parole')
+        assert abs(check_time-time) <= 1e-6
+        self.ode_params['parole-inflow-rates'] = inflow_rates
+
+        # Interactions in the arrested port
+        #--------------------------------
+        # two way "to" and "from" arrested
+
+        # to
+        message_time = self.recv('arrested')
+        outflow_rates = self.__compute_outflow_rates(message_time, 'arrested')
+        self.send((message_time, outflow_rates), 'arrested')
+
+        # from
+        self.send(time, 'arrested')
+        (check_time, inflow_rates) = self.recv('arrested')
+        assert abs(check_time-time) <= 1e-6
+        self.ode_params['arrested-inflow-rates'] = inflow_rates
 
     def __step(self, time=0.0):
         r'''
         ODE IVP problem:
         Given the initial data at :math:`t=0`,
         :math:`u = (u_1(0),u_2(0),\ldots)`
         solve :math:`\frac{\text{d}u}{\text{d}t} = f(u)` in the interval
@@ -231,43 +239,43 @@
 
         '''
 
         # Get state values
         a_vec = self.population_phase.GetValue('n0', time)
         b_vec = self.population_phase.GetValue('f0g', time)
 
-        u_0 = np.concatenate( (a_vec,b_vec) )
+        u_0 = np.concatenate((a_vec, b_vec))
 
         t_interval_sec = np.linspace(0.0, self.time_step, num=2)
 
-        (u_vec_hist, info_dict) = odeint( self.__rhs_fn,
-                                          u_0, t_interval_sec,
-                                          args=( self.ode_params, ),
-                                          rtol=1e-4, atol=1e-8, mxstep=200,
-                                          full_output=True )
+        (u_vec_hist, info_dict) = odeint(self.__rhs_fn,
+                                         u_0, t_interval_sec,
+                                         args=(self.ode_params, ),
+                                         rtol=1e-4, atol=1e-8, mxstep=200,
+                                         full_output=True)
 
         assert info_dict['message'] =='Integration successful.', info_dict['message']
 
-        u_vec = u_vec_hist[1,:]  # solution vector at final time step
+        u_vec = u_vec_hist[1, :]  # solution vector at final time step
 
 
         time += self.time_step
 
         # Update state variables
         values = self.population_phase.GetRow() # values existing values
         self.population_phase.AddRow(time, values) # copy on new time for convenience
 
-        self.population_phase.SetValue('n0',  u_vec[:1], time) # insert new values
+        self.population_phase.SetValue('n0', u_vec[:1], time) # insert new values
         self.population_phase.SetValue('f0g', u_vec[1:], time) # insert new values
 
         return time
 
     def __rhs_fn(self, u_vec, t, params):
 
-        n0  = u_vec[:1]   # non-offender population
+        n0 = u_vec[:1]   # non-offender population
 
         # source of non-offenders
         s0_coeff = params['non-offenders-maturity-rate-coeff']
         n0_0 = params['non_offender_adult_population']
         s0 = s0_coeff * n0_0
 
         # outflow rate to Arrested
@@ -277,55 +285,55 @@
         # death rate
         death_rate_coeff = params['non-offenders-death-rate-coeff']
         death_rate = death_rate_coeff * n0
 
         dt_n0 = s0 - outflow_rate - death_rate
 
 
-        f0g = u_vec[1:]  # free-offender population groups 
+        f0g = u_vec[1:]  # free-offender population groups
 
-        prison_inflow_rates       = params['prison-inflow-rates']
-        parole_inflow_rates       = params['parole-inflow-rates']
-        arrested_inflow_rates     = params['arrested-inflow-rates']
-        jail_inflow_rates         = params['jail-inflow-rates']
+        prison_inflow_rates = params['prison-inflow-rates']
+        parole_inflow_rates = params['parole-inflow-rates']
+        arrested_inflow_rates = params['arrested-inflow-rates']
+        jail_inflow_rates = params['jail-inflow-rates']
         adjudication_inflow_rates = params['adjudication-inflow-rates']
-        probation_inflow_rates    = params['probation-inflow-rates']
+        probation_inflow_rates = params['probation-inflow-rates']
 
         # free-offenders inflows
         inflow_rates = prison_inflow_rates + parole_inflow_rates +\
                        arrested_inflow_rates + jail_inflow_rates +\
                        adjudication_inflow_rates + probation_inflow_rates
 
-        assert np.all(inflow_rates>=0.0), 'values: %r'%inflow_rates
+        assert np.all(inflow_rates >= 0.0), 'values: %r'%inflow_rates
 
         c0rg = params['free-offenders-commit-to-arrested-coeff-grps']
 
 
         # free-offenders outflow (recidivism)
         outflow_rates = c0rg * f0g
 
-        assert np.all(outflow_rates>=0.0), 'values: %r'%outflow_rates
+        assert np.all(outflow_rates >= 0.0), 'values: %r'%outflow_rates
 
         death_rates_coeff = params['free-offenders-death-rates-coeff']
 
         death_rates = death_rates_coeff * f0g
 
-        assert np.all(death_rates>=0.0), 'values: %r'%death_rates
+        assert np.all(death_rates >= 0.0), 'values: %r'%death_rates
 
         dt_f0g = inflow_rates - outflow_rates - death_rates
 
 
-        dt_u = np.concatenate( (dt_n0,dt_f0g) )
+        dt_u = np.concatenate((dt_n0, dt_f0g))
 
         return dt_u
 
     def __compute_outflow_rates(self, time, name):
 
-        n0  = self.population_phase.GetValue('n0',time)
-        f0g = self.population_phase.GetValue('f0g',time)
+        n0 = self.population_phase.GetValue('n0', time)
+        f0g = self.population_phase.GetValue('f0g', time)
 
         if name == 'arrested':
 
             c0rg = self.ode_params['free-offenders-commit-to-arrested-coeff-grps']
 
             c00g = self.ode_params['non-offenders-commit-to-arrested-coeff-grps']
 
@@ -341,12 +349,12 @@
         '''
 
         zeros = np.zeros(self.n_groups)
 
         p_names = [p.name for p in self.ports]
 
         if 'arrested' not in p_names:
-            self.ode_params['commit-to-arrested-coeff-grps']     = zeros
+            self.ode_params['commit-to-arrested-coeff-grps'] = zeros
 
-            self.ode_params['general-commit-to-arrested-coeff-grps']     = zeros
+            self.ode_params['general-commit-to-arrested-coeff-grps'] = zeros
 
         return
```

### Comparing `cortix-1.1.8/cortix/examples/city_justice/jail.py` & `cortix-1.1.9/cortix/examples/city_justice/jail.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/city_justice/parole.py` & `cortix-1.1.9/cortix/examples/city_justice/parole.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/city_justice/prison.py` & `cortix-1.1.9/cortix/examples/city_justice/prison.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/city_justice/probation.py` & `cortix-1.1.9/cortix/examples/city_justice/probation.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/city_justice/run_city_justice.py` & `cortix-1.1.9/cortix/examples/city_justice/run_city_justice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # This file is part of the Cortix toolkit environment
 # https://cortix.org
-'''
-Crimninal justice network dynamics modeling.
+"""Crimninal justice network dynamics modeling.
 
 This example uses 7 modules:
     - Community
     - Arrested
     - Adjudication
     - Jail
     - Prison
@@ -30,15 +29,15 @@
 
     `run_city_justice.py`
 
 To profile this run do:
 
      python -m cProfile -s time run_city_justice.py > lixo
 
-'''
+"""
 
 import scipy.constants as unit
 import matplotlib.pyplot as plt
 
 from cortix import Cortix
 from cortix import Network
 
@@ -75,22 +74,22 @@
     use_mpi = False  # True for MPI; False for Python multiprocessing
 
     city = Cortix(use_mpi=use_mpi, splash=True)
 
     city.network = Network()
 
     community = Community(n_groups=n_groups, non_offender_adult_population=100000,
-            offender_pool_size=0)
+                          offender_pool_size=0)
     city.network.module(community)
     community.end_time = end_time
     community.time_step = time_step
-    community.show_time = (True,30*unit.day)
+    community.show_time = (True, 30*unit.day)
     community.save = True
 
-    prison = Prison(n_groups=n_groups,pool_size=0.0)
+    prison = Prison(n_groups=n_groups, pool_size=0.0)
     city.network.module(prison)
     prison.end_time = end_time
     prison.time_step = time_step
     prison.save = True
 
     parole = Parole(n_groups=n_groups)
     city.network.module(parole)
```

### Comparing `cortix-1.1.8/cortix/examples/droplet_swirl/droplet.py` & `cortix-1.1.9/cortix/examples/droplet_swirl/droplet.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/droplet_swirl/run_droplet_swirl.py` & `cortix-1.1.9/cortix/examples/droplet_swirl/run_droplet_swirl.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/droplet_swirl/vortex.py` & `cortix-1.1.9/cortix/examples/droplet_swirl/vortex.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/ideal_gas/particle.py` & `cortix-1.1.9/cortix/examples/ideal_gas/particle.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/ideal_gas/particle_handler.py` & `cortix-1.1.9/cortix/examples/ideal_gas/particle_handler.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/ideal_gas/particle_plotting.py` & `cortix-1.1.9/cortix/examples/ideal_gas/particle_plotting.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/ideal_gas/run_particle.py` & `cortix-1.1.9/cortix/examples/ideal_gas/run_particle.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/nbody/body.py` & `cortix-1.1.9/cortix/examples/nbody/body.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/nbody/run_planets.py` & `cortix-1.1.9/cortix/examples/nbody/run_planets.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/umlrr/code.py` & `cortix-1.1.9/cortix/examples/umlrr/code.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/umlrr/run_umlrr.py` & `cortix-1.1.9/cortix/examples/umlrr/run_umlrr.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/examples/umlrr/umlrr.py` & `cortix-1.1.9/cortix/examples/umlrr/umlrr.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,24 +42,26 @@
 
         self.port_names_expected = ['coolant-inflow', 'coolant-outflow',
                                     'signal-out', 'signal-in']
 
         unit.kg     = unit.kilo*unit.gram
         unit.meter  = 1.0
         unit.second = 1.0
+        unit.pascal = 1.0
         unit.joule  = 1.0
         unit.kj     = unit.kilo*unit.joule
         unit.kelvin = 1.0
         unit.watt   = 1.0
         unit.barn   = 1.0e-28 * unit.meter**2
 
         self.initial_time = 0.0 * unit.day
         self.end_time     = 4 * unit.hour
         self.time_step    = 10.0 * unit.second
         self.show_time    = (False,10.0)
+
         self.log = logging.getLogger('cortix')
 
         self.params = dict()
 
         # General parameters
 
         #self.params['gen-time'] = 1.0e-4  # s
```

### Comparing `cortix-1.1.8/cortix/src/cortix_main.py` & `cortix-1.1.9/cortix/src/cortix_main.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/src/module.py` & `cortix-1.1.9/cortix/src/module.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/src/network.py` & `cortix-1.1.9/cortix/src/network.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/src/port.py` & `cortix-1.1.9/cortix/src/port.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/support/nuclear/actor.py` & `cortix-1.1.9/cortix/support/nuclear/actor.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/support/nuclear/fuel_bucket.py` & `cortix-1.1.9/cortix/support/nuclear/fuel_bucket.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/support/nuclear/fuel_bundle.py` & `cortix-1.1.9/cortix/support/nuclear/fuel_bundle.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/support/nuclear/fuel_segment.py` & `cortix-1.1.9/cortix/support/nuclear/fuel_segment.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/support/nuclear/fuelsegmentsgroups.py` & `cortix-1.1.9/cortix/support/nuclear/fuelsegmentsgroups.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/support/nuclear/fuelslug.py` & `cortix-1.1.9/cortix/support/nuclear/fuelslug.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/support/nuclear/nuclides.py` & `cortix-1.1.9/cortix/support/nuclear/nuclides.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/support/periodictable.py` & `cortix-1.1.9/cortix/support/periodictable.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/support/phase.py` & `cortix-1.1.9/cortix/support/phase.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/support/phase_new.py` & `cortix-1.1.9/cortix/support/phase_new.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import time
 import datetime
 
 import numpy as np
 import pandas
 
 import matplotlib
-matplotlib.use('Agg', warn=False)
+#needed? matplotlib.use('Agg', warn=False)
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gridspec
 from matplotlib.ticker import MultipleLocator
 from matplotlib.ticker import ScalarFormatter
 
 from cortix.support.species   import Species
 from cortix.support.quantity import Quantity
```

### Comparing `cortix-1.1.8/cortix/support/phase_newest.py` & `cortix-1.1.9/cortix/support/phase_newest.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/support/quantity.py` & `cortix-1.1.9/cortix/support/quantity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # This file is part of the Cortix toolkit environment
 # https://cortix.org
 import pandas
-import matplotlib
-matplotlib.use('Agg', warn=False)
+#import matplotlib
+#matplotlib.use('Agg', warn=False)
 import matplotlib.pyplot as plt
 
 class Quantity:
-    '''
+    """
     todo: this probably should not have a "value" for the same reason as Species.
           this needs some thinking.
     well not so fast. This can be used to build a quantity with anything as a
     value. For instance a history of the quantity as a time series.
 
-    '''
+    """
     def __init__(self,
-                 name        = 'null-quantity-name',
-                 formalName  = 'null-quantity-formal-name', # deprecated
+                 name = 'null-quantity-name',
+                 formalName = 'null-quantity-formal-name', # deprecated
                  formal_name = 'null-quantity-formal-name',
-                 latex_name  = 'null-quantity-latex-name',
-                 value      = float(0.0),      # this can be any type
-                 unit       = 'null-quantity-unit',
-                 info       = 'null-quantity-info'
+                 latex_name = 'null-quantity-latex-name',
+                 value = float(0.0),      # this can be any type
+                 unit = 'null-quantity-unit',
+                 info = 'null-quantity-info'
                 ):
 
         assert isinstance(name, str), 'not a string.'
         self.__name = name
 
         assert isinstance(formalName, str), 'not a string.'
         self.__formalName = formalName  # deprecated
@@ -212,15 +212,22 @@
             return
         if len(self.__value) == 1:
             return
 
         if not title:
             title = self.info
         if not y_label:
-            y_label = self.name
+            if self.latex_name != 'null-quantity-latex-name':
+                y_label = self.latex_name
+            elif self.formal_name != 'null-quantity-formal-name':
+                y_label = self.formal_name
+            elif self.name != 'null-quantity-name':
+                y_label = self.name
+            else:
+                assert False
 
         if isinstance(self.__value[0],float) or isinstance(self.__value[0],int) \
                 or isinstance(self.__value[0],bool):
             n_dim = 1
             # Turn series of values into a series of a list of one value to allow for
             # the indexing below
             for i in range (len(self.__value[:])):
@@ -246,15 +253,16 @@
             plt.ylabel(y_label)
 
             plt.title(title)
 
             plt.plot(x, y)
 
             if not same_axis and file_name:
-                plt.savefig(file_name+str(i)+'.png',dpi=dpi)
+                plt.savefig(file_name+str(i)+'.png', dpi=dpi)
+
         if same_axis and file_name:
             plt.savefig(file_name+'.png',dpi=dpi)
 
         return
 
     def __str__(self):
         '''
```

### Comparing `cortix-1.1.8/cortix/support/specie.py` & `cortix-1.1.9/cortix/support/specie.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/support/species.py` & `cortix-1.1.9/cortix/support/species.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/support/stream.py` & `cortix-1.1.9/cortix/support/stream.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/tests/dataplot.py` & `cortix-1.1.9/cortix/tests/dataplot.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/tests/dummy_module.py` & `cortix-1.1.9/cortix/tests/dummy_module.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/tests/mpi_test_send_recv.py` & `cortix-1.1.9/cortix/tests/mpi_test_send_recv.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/tests/test_cortix_add_module.py` & `cortix-1.1.9/cortix/tests/test_cortix_add_module.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/tests/test_data_plot.py` & `cortix-1.1.9/cortix/tests/test_data_plot.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix/tests/test_droplet.py` & `cortix-1.1.9/cortix/tests/test_droplet.py`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/cortix.egg-info/PKG-INFO` & `cortix-1.1.9/cortix.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cortix
-Version: 1.1.8
+Version: 1.1.9
 Summary: Cortix is a Python library for network dynamics            modeling and HPC simulation.
 Home-page: https://cortix.org
 Author: Cortix Computing
-Author-email: tazzaoui@cs.uml.edu
+Author-email: valmor_dealmeida@uml.edu
 License: UNKNOWN
 Description: # Cortix
         A Python library for network dynamics modeling and HPC simulation.
           + [Cortix on Jupyter notebook examples](https://github.com/dpploy/cortix-nb)
           + [Documentation on the web](https://cortix.org)
         
         ![Website](https://img.shields.io/website/https/github.com/dpploy/cortix.svg)
@@ -105,8 +105,9 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Topic :: Education
 Classifier: Topic :: Utilities
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cortix-1.1.8/cortix.egg-info/SOURCES.txt` & `cortix-1.1.9/cortix.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,22 @@
 cortix/docs/support_rst/nuclear_rst/fuel_segment.rst
 cortix/docs/support_rst/nuclear_rst/fuelsegmentsgroups.rst
 cortix/docs/support_rst/nuclear_rst/fuelslug.rst
 cortix/docs/support_rst/nuclear_rst/modules.rst
 cortix/docs/support_rst/nuclear_rst/nuclides.rst
 cortix/examples/__init__.py
 cortix/examples/bwr/condenser.py
-cortix/examples/bwr/heater.py
+cortix/examples/bwr/condenser_tester.py
+cortix/examples/bwr/cooler.py
 cortix/examples/bwr/params.py
+cortix/examples/bwr/plant_test.py
+cortix/examples/bwr/reactor-old.py
 cortix/examples/bwr/reactor.py
 cortix/examples/bwr/run_plant.py
+cortix/examples/bwr/run_reactor.py
 cortix/examples/bwr/turbine.py
 cortix/examples/city_justice/adjudication.py
 cortix/examples/city_justice/arrested.py
 cortix/examples/city_justice/community.py
 cortix/examples/city_justice/jail.py
 cortix/examples/city_justice/parole.py
 cortix/examples/city_justice/prison.py
```

### Comparing `cortix-1.1.8/scripts/format-all.sh` & `cortix-1.1.9/scripts/format-all.sh`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/scripts/format-code.sh` & `cortix-1.1.9/scripts/format-code.sh`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/scripts/install_sundials.sh` & `cortix-1.1.9/scripts/install_sundials.sh`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/scripts/pylint-src.sh` & `cortix-1.1.9/scripts/pylint-src.sh`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/scripts/recordcortixsession` & `cortix-1.1.9/scripts/recordcortixsession`

 * *Files identical despite different names*

### Comparing `cortix-1.1.8/setup.py` & `cortix-1.1.9/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,37 @@
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# This file is part of the Cortix toolkit environment
+# https://cortix.org
+
+# Read contents of README file.
+from os import path
+
 import setuptools
 
-with open("README.md", "r") as fh:
-    long_description = fh.read()
+THIS_DIRECTORY = path.abspath(path.dirname(__file__))
 
-with open("requirements.txt", "r") as fh:
-    req = fh.readlines()
+with open(path.join(THIS_DIRECTORY, 'README.md'), encoding='utf-8') as f:
+    LONG_DESCRIPTION = f.read()
+
+with open('requirements.txt', 'r') as fh:
+    REQ = fh.readlines()
 
 setuptools.setup(
-    name="cortix",
-    version="1.1.8",
+    name='cortix',
+    version='1.1.9',
     author="Cortix Computing",
-    author_email="tazzaoui@cs.uml.edu",
-    description="Cortix is a Python library for network dynamics\
-            modeling and HPC simulation.",
-    long_description=long_description,
+    author_email="valmor_dealmeida@uml.edu",
+    description='Cortix is a Python library for network dynamics\
+            modeling and HPC simulation.',
+    long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     setup_requires=['wheel'],
     include_package_data=True,
-    install_requires=req,
+    install_requires=REQ,
     url="https://cortix.org",
     packages=setuptools.find_namespace_packages(),
     keywords = ['simulation', 'math'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         'Topic :: Scientific/Engineering :: Mathematics',
@@ -30,8 +40,10 @@
         'Intended Audience :: End Users/Desktop',
         'Intended Audience :: Science/Research',
         'Operating System :: MacOS',
         'Operating System :: Unix',
         'Topic :: Education',
         'Topic :: Utilities'
     ],
+    python_requires='>=3.7'
 )
+
```

