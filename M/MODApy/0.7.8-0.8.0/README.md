# Comparing `tmp/MODApy-0.7.8.tar.gz` & `tmp/MODApy-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MODApy-0.7.8.tar", last modified: Tue Nov  1 21:16:06 2022, max compression
+gzip compressed data, was "MODApy-0.8.0.tar", last modified: Sun Apr 14 11:20:20 2024, max compression
```

## Comparing `MODApy-0.7.8.tar` & `MODApy-0.8.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 juanvazquez   (501) staff       (20)        0 2022-11-01 21:16:06.030914 MODApy-0.7.8/
--rwxr-xr-x   0 juanvazquez   (501) staff       (20)    35147 2021-06-18 01:46:18.000000 MODApy-0.7.8/LICENSE
-drwxr-xr-x   0 juanvazquez   (501) staff       (20)        0 2022-11-01 21:16:06.017922 MODApy-0.7.8/MODApy/
--rwxr-xr-x   0 juanvazquez   (501) staff       (20)       97 2022-11-01 19:48:51.000000 MODApy-0.7.8/MODApy/__init__.py
--rwxr-xr-x   0 juanvazquez   (501) staff       (20)     5563 2022-11-01 19:48:51.000000 MODApy-0.7.8/MODApy/cfg.py
--rwxr-xr-x   0 juanvazquez   (501) staff       (20)    25343 2022-11-01 19:48:51.000000 MODApy-0.7.8/MODApy/cmd_line.py
--rwxr-xr-x   0 juanvazquez   (501) staff       (20)     3609 2022-11-01 19:48:51.000000 MODApy-0.7.8/MODApy/coverage.py
--rwxr-xr-x   0 juanvazquez   (501) staff       (20)     7518 2022-11-01 19:48:51.000000 MODApy-0.7.8/MODApy/downloader.py
--rwxr-xr-x   0 juanvazquez   (501) staff       (20)     5179 2022-11-01 19:48:51.000000 MODApy-0.7.8/MODApy/modaapi.py
--rwxr-xr-x   0 juanvazquez   (501) staff       (20)    17320 2022-11-01 19:48:51.000000 MODApy-0.7.8/MODApy/pipeline.py
--rw-r--r--   0 juanvazquez   (501) staff       (20)      465 2022-11-01 19:48:51.000000 MODApy-0.7.8/MODApy/utils.py
--rwxr-xr-x   0 juanvazquez   (501) staff       (20)    18071 2022-11-01 19:48:51.000000 MODApy-0.7.8/MODApy/variantsdb.py
--rw-r--r--   0 juanvazquez   (501) staff       (20)     5243 2022-11-01 19:48:51.000000 MODApy-0.7.8/MODApy/vcfanalysis.py
--rwxr-xr-x   0 juanvazquez   (501) staff       (20)    30360 2022-11-01 19:48:51.000000 MODApy-0.7.8/MODApy/vcfmgr.py
--rwxr-xr-x   0 juanvazquez   (501) staff       (20)       22 2022-11-01 21:15:34.000000 MODApy-0.7.8/MODApy/version.py
-drwxr-xr-x   0 juanvazquez   (501) staff       (20)        0 2022-11-01 21:16:06.029111 MODApy-0.7.8/MODApy/www/
--rwxr-xr-x   0 juanvazquez   (501) staff       (20)    52660 2022-03-23 18:54:20.000000 MODApy-0.7.8/MODApy/www/wespipelinebam.png
--rwxr-xr-x   0 juanvazquez   (501) staff       (20)   113893 2022-03-23 18:54:20.000000 MODApy-0.7.8/MODApy/www/wespipelinefull.png
--rwxr-xr-x   0 juanvazquez   (501) staff       (20)    52084 2022-03-23 18:54:20.000000 MODApy-0.7.8/MODApy/www/wespipelinevcf.png
-drwxr-xr-x   0 juanvazquez   (501) staff       (20)        0 2022-11-01 21:16:06.024257 MODApy-0.7.8/MODApy.egg-info/
--rw-r--r--   0 juanvazquez   (501) staff       (20)     3354 2022-11-01 21:16:05.000000 MODApy-0.7.8/MODApy.egg-info/PKG-INFO
--rw-r--r--   0 juanvazquez   (501) staff       (20)      522 2022-11-01 21:16:05.000000 MODApy-0.7.8/MODApy.egg-info/SOURCES.txt
--rw-r--r--   0 juanvazquez   (501) staff       (20)        1 2022-11-01 21:16:05.000000 MODApy-0.7.8/MODApy.egg-info/dependency_links.txt
--rw-r--r--   0 juanvazquez   (501) staff       (20)       48 2022-11-01 21:16:05.000000 MODApy-0.7.8/MODApy.egg-info/entry_points.txt
--rw-r--r--   0 juanvazquez   (501) staff       (20)      165 2022-11-01 21:16:05.000000 MODApy-0.7.8/MODApy.egg-info/requires.txt
--rw-r--r--   0 juanvazquez   (501) staff       (20)        7 2022-11-01 21:16:05.000000 MODApy-0.7.8/MODApy.egg-info/top_level.txt
--rw-r--r--   0 juanvazquez   (501) staff       (20)     3354 2022-11-01 21:16:06.030391 MODApy-0.7.8/PKG-INFO
--rwxr-xr-x   0 juanvazquez   (501) staff       (20)     2640 2021-06-18 01:46:18.000000 MODApy-0.7.8/README.md
--rw-r--r--   0 juanvazquez   (501) staff       (20)       38 2022-11-01 21:16:06.031071 MODApy-0.7.8/setup.cfg
--rwxr-xr-x   0 juanvazquez   (501) staff       (20)     2105 2022-11-01 19:48:51.000000 MODApy-0.7.8/setup.py
+drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-14 11:20:20.060520 MODApy-0.8.0/
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    35147 2023-03-11 19:24:07.000000 MODApy-0.8.0/LICENSE
+drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-14 11:20:20.056244 MODApy-0.8.0/MODApy/
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)      297 2024-04-07 18:02:09.000000 MODApy-0.8.0/MODApy/__init__.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     6593 2024-04-07 18:02:09.000000 MODApy-0.8.0/MODApy/cfg.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    30224 2024-04-14 11:10:14.000000 MODApy-0.8.0/MODApy/cmd_line.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     3656 2024-04-07 18:02:09.000000 MODApy-0.8.0/MODApy/coverage.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     8208 2024-04-07 18:02:09.000000 MODApy-0.8.0/MODApy/downloader.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     7416 2024-04-07 18:02:09.000000 MODApy-0.8.0/MODApy/modaapi.py
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)     6342 2024-04-07 18:02:09.000000 MODApy-0.8.0/MODApy/parquetvardb.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    19642 2024-04-07 18:02:09.000000 MODApy-0.8.0/MODApy/pipeline.py
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)     1300 2024-04-03 22:26:23.000000 MODApy-0.8.0/MODApy/utils.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    21570 2024-04-14 11:10:14.000000 MODApy-0.8.0/MODApy/variantsdb.py
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)     5418 2024-04-07 18:02:09.000000 MODApy-0.8.0/MODApy/vcfanalysis.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    47643 2024-04-14 11:10:14.000000 MODApy-0.8.0/MODApy/vcfmgr.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)       22 2024-04-07 18:02:09.000000 MODApy-0.8.0/MODApy/version.py
+drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-14 11:20:20.059934 MODApy-0.8.0/MODApy/www/
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    52660 2023-03-11 19:24:07.000000 MODApy-0.8.0/MODApy/www/wespipelinebam.png
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)   113893 2023-03-11 19:24:07.000000 MODApy-0.8.0/MODApy/www/wespipelinefull.png
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    52084 2023-03-11 19:24:07.000000 MODApy-0.8.0/MODApy/www/wespipelinevcf.png
+drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-14 11:20:20.058640 MODApy-0.8.0/MODApy.egg-info/
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)     3354 2024-04-14 11:20:20.000000 MODApy-0.8.0/MODApy.egg-info/PKG-INFO
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)      560 2024-04-14 11:20:20.000000 MODApy-0.8.0/MODApy.egg-info/SOURCES.txt
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)        1 2024-04-14 11:20:20.000000 MODApy-0.8.0/MODApy.egg-info/dependency_links.txt
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)       48 2024-04-14 11:20:20.000000 MODApy-0.8.0/MODApy.egg-info/entry_points.txt
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)      172 2024-04-14 11:20:20.000000 MODApy-0.8.0/MODApy.egg-info/requires.txt
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)        7 2024-04-14 11:20:20.000000 MODApy-0.8.0/MODApy.egg-info/top_level.txt
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)     3354 2024-04-14 11:20:20.060330 MODApy-0.8.0/PKG-INFO
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     2640 2023-03-11 19:24:07.000000 MODApy-0.8.0/README.md
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)       84 2023-05-21 18:43:17.000000 MODApy-0.8.0/pyproject.toml
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)       38 2024-04-14 11:20:20.060577 MODApy-0.8.0/setup.cfg
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     2112 2023-05-14 18:54:50.000000 MODApy-0.8.0/setup.py
```

### Comparing `MODApy-0.7.8/LICENSE` & `MODApy-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MODApy-0.7.8/MODApy/cmd_line.py` & `MODApy-0.8.0/MODApy/cmd_line.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 #!/usr/bin/env python
 import argparse
+import glob
 import logging
 import os
 import shlex
 import subprocess
 from sys import argv
 
-import pandas as pd
-import uvicorn
-
-from MODApy import cfg, pipeline, vcfmgr, downloader, variantsdb, coverage, vcfanalysis
+from MODApy import (
+    coverage,
+    downloader,
+    parquetvardb,
+    pipeline,
+    variantsdb,
+    vcfanalysis,
+    vcfmgr,
+)
+from MODApy.cfg import configuration
 from MODApy.modaapi import app
 from MODApy.utils import checkFile
 from MODApy.version import __version__
 
+import pandas as pd
+
+import uvicorn
+
+
 logger = logging.getLogger(__name__)
 
 
 class Parser(object):
     """
     Main parser for command line arguments. Uses ArgParse
     """
@@ -26,34 +38,38 @@
         parser = argparse.ArgumentParser(
             description="Multi-Omics Data Analisis for Python",
             usage='''MODApy <command> [<args>]
 
         Commands:
         launcher        Run MoDAPy Web Interface
         variantsDB      Work with Variants Database
-        addPatient      Download Patient Data to Patients folder. Receives both url or xls/xlsx
+        addPatient      Download Patient Data to Patients folder. Receives
+                        both url or xls/xlsx
         pipeline        Run pipeline on FastQ file/s
         abs_pipeline    Run pipeline on FastQ file/s using absolute paths
-        parsevcf        Parse a VCF and write it's Raw Output to CSV.
+        parsevcf        Parse a VCF and write it's Raw Output to CSV or Parquet.
         diffvcf         Generate a Duos analysis on any given vcf
         single          Run study on a single patient
         abs_single      Run study on a single patient using absolute paths
         duos            Run Duos analysis on two selected patients
         trios           Run Trios analysis on three selected patients
         coverageStats   Generate coverages stats for bam file or list of files
         launchapi       Run Modapy Api Server
 
         For more info on any of these commands, use "cmd_line.py <command> -h
-        
+
         You can check the package version using -v or --version"''',
         )
 
         parser.add_argument("command", help="Select command to run")
         parser.add_argument(
-            "-v", "--version", action="version", version="MODApy " + __version__
+            "-v",
+            "--version",
+            action="version",
+            version="MODApy " + __version__,
         )
         # exclude all arguments but the first one
         args = parser.parse_args(argv[1:2])
         if not hasattr(self, args.command):
             logger.error("Unrecognized commands")
             parser.print_help()
             exit(1)
@@ -62,118 +78,217 @@
         getattr(self, args.command)()
 
     def launcher(self):
         try:
             logger.info("Launching Web Interface")
             cmd = (
                 'R -e shiny::runApp(\\"'
-                + cfg.rootDir
+                + configuration.rootDir
                 + '/MODApy-Shiny.R\\"\\,port=3838\\,host=\\"0.0.0.0\\")'
             )
             webapp = subprocess.Popen(
-                shlex.split(cmd), stderr=subprocess.STDOUT, stdout=subprocess.PIPE
+                shlex.split(cmd),
+                stderr=subprocess.STDOUT,
+                stdout=subprocess.PIPE,
             )
             webapp.wait()
             output, error = webapp.communicate()
             logger.debug(output)
             logger.debug(error)
             logger.info("Web Interface Closed")
         except Exception as err:
             logger.error("Webapp process failed")
             logger.debug(f"There was an error: {err}", exc_info=True)
 
     def coverageStats(self):
         parser = argparse.ArgumentParser(
-            description="Downloads Patient Data to Patients folder. Receives both url or xls/xlsx"
+            description="Downloads Patient Data to Patients folder. Receives both url \
+                or xls/xlsx"
         )
         parser.add_argument(
             "Gene_Exon_Bed_File",
-            help="A Gene and Exon Bed file, in the format CHROM START END GENE_EXON STRAND",
+            help="A Gene and Exon Bed file, in the format CHROM START END GENE_EXON \
+                STRAND",
         )
         parser.add_argument(
             "-Panel",
-            help="Filepath of a bed file containing a group of genes or exons of interest",
+            help="Filepath of a bed file containing a group of genes or exons of \
+                interest",
         )
         parser.add_argument(
             "Bam_files",
-            help="Bam files or list of files to calculate coverage stats (can use wildcard) Example: /home/bams/*.bam",
+            help="Bam files or list of files to calculate coverage stats (can use \
+                  wildcard) Example: /home/bams/*.bam",
             nargs="*",
         )
         try:
             args = parser.parse_args(argv[2:])
             Bam_files = list(args.Bam_files)
             bed_file = args.Gene_Exon_Bed_File
             panel_file = args.Panel
             coverage.main(Bam_files, bed_file, panel_file)
         except Exception as err:
             logger.error("Coverage process failed")
             logger.debug(f"There was an error: {err}", exc_info=True)
 
     def addPatient(self):
         parser = argparse.ArgumentParser(
-            description="Downloads Patient Data to Patients folder. Receives both url or xls/xlsx"
+            description="Downloads Patient Data to Patients folder. Receives both \
+                  url or xls/xlsx"
         )
         parser.add_argument(
             "FileorURL",
-            help="URL to download or filepath to xls or xlsx files containing urls",
+            help="URL to download or filepath to xls or xlsx files containing \
+                  urls",
         )
         try:
             args = parser.parse_args(argv[2:])
             fileorurl = args.FileorURL
             downloader.get_links(fileorurl)
         except Exception as err:
             logger.error("Download process failed")
             logger.debug(f"There was an error: {err}", exc_info=True)
 
     def parsevcf(self):
         parser = argparse.ArgumentParser(
-            description="Parses a VCF file using MODApy parser and exports output as a csv file with all fields tabulated."
+            description="Parses a VCF file using MODApy parser and exports output as \
+                  a csv or parquet file with all fields tabulated."
+        )
+        parser.add_argument("Path", help="Path to VCF file or folder to Parse")
+        parser.add_argument("Filetype", help="filetype to export to (csv or parquet)")
+        parser.add_argument(
+            "-nonprioritized",
+            action="store_false",
+            default=True,
+            help="""Prioritize variants (output will have one line per variant).
+                  Otherwise, output will have one line per per variant-annotation.""",
+        )
+        parser.add_argument(
+            "-recursive",
+            action="store_true",
+            default=False,
+            help="Parse all vcf files in recursive folders.",
+        )
+        parser.add_argument(
+            "-partition_cols",
+            default=None,
+            help="Partition columns for parquet file. Must be a list of columns",
         )
-        parser.add_argument("File", help="Path to VCF file to Parse")
         try:
             args = parser.parse_args(argv[2:])
-            file = args.File
-            vcfmgr.ParsedVCF.from_vcf(file).to_csv(
-                file.split(".vcf")[0] + ".csv", index=False
+            path = args.Path
+            filetype = args.Filetype
+            prioritized = args.nonprioritized
+            recursive = args.recursive
+            partition_cols = args.partition_cols
+            logger.info(
+                f"""Parsing VCF file/s in {path}, to: {filetype},
+                        prioritized: {prioritized}"""
             )
-            logger.info("Output file is in %s" % file.split(".vcf")[0])
+            if recursive:
+                file_list = glob.glob(path + "/**/*.vcf", recursive=True)
+            else:
+                file_list = [path]
+            for file in file_list:
+                df = vcfmgr.ParsedVCF.from_vcf(file, prioritized=prioritized)
+                if filetype == "csv":
+                    df.to_csv(file.split(".vcf")[0] + ".csv", index=False)
+                elif filetype == "parquet":
+                    df.vcf_to_parquet(
+                        file.split(".vcf")[0] + ".parquet", partition_cols
+                    )
+                else:
+                    logger.error("Filetype not recognized")
+                logger.info("Output file is in %s" % file.split(".vcf")[0])
+                del df
         except Exception as err:
             logger.error("Parsing process failed")
             logger.debug(f"There was an error: {err}", exc_info=True)
 
     def variantsDB(self):
         parser = argparse.ArgumentParser(description="Work with Variants DB")
         parser.add_argument(
             "-buildDB",
             action="store_true",
-            help="Build Variants DataBase with all patients that are not currently in it.",
+            help="Build Variants DataBase with all patients that are not currently \
+                in it.",
         )
         parser.add_argument(
             "-addPatientToDB",
             help="Adds a single patient to DB. Must supply path to vcf",
         )
         parser.add_argument(
             "-annotate",
-            help="Adds data from variantsdb to analysis done in modapy. Must supply path to excel output from modapy",
+            help="Adds data from variantsdb to analysis done in modapy. Must \
+                supply path to excel output from modapy",
+        )
+        parser.add_argument("Filetype", help="DB filetype (csv or parquet)")
+        parser.add_argument(
+            "-nonprioritized",
+            action="store_false",
+            default=True,
+            help="""Prioritize variants (output will have one line per variant).
+                  Otherwise, output will have one line per per variant-annotation.""",
         )
         try:
             args = parser.parse_args(argv[2:])
+            filetype = args.Filetype
+            prioritized = args.nonprioritized
+            if prioritized is True:
+                suffix = "-prioritized"
+            else:
+                suffix = "-nonprioritized"
+            dbpath = (
+                configuration.variantsDBPath.rsplit('/', maxsplit=1)[0]
+                + "/vardb"
+                + suffix
+                + ".parquet"
+            )
             if args.buildDB:
-                db = variantsdb.VariantsDB.buildDB()
-                db.to_VarDBCSV()
+                if filetype == 'csv':
+                    db = variantsdb.VariantsDB.buildDB()
+                    db.to_VarDBCSV()
+                elif filetype == 'parquet':
+                    if os.path.exists(dbpath):
+                        logger.info(f"Loading parquet db from {dbpath}")
+                        db = parquetvardb.ParquetVarDB.from_parquetdb(dbpath)
+                    else:
+                        logger.info(
+                            f"Parquet db not found in {dbpath}. Building from scratch"
+                        )
+                        db = None
+                    parquetvardb.ParquetVarDB.buildDB(
+                        db=db,
+                        patientPath=configuration.patientPath,
+                        dbpath=dbpath,
+                        filetype='vcf',
+                        prioritized=prioritized,
+                    )
             if args.addPatientToDB:
-                patient = cfg.patientPath + args.addPatientToDB
+                patient = configuration.patientPath + args.addPatientToDB
                 db = variantsdb.VariantsDB.from_csvdb(variantsdb.variantsDBPath)
                 db = db.addPatientToDB(patient)
                 db.to_VarDBCSV()
             if args.annotate:
                 fileName = args.annotate.rsplit("/", maxsplit=1)[1]
                 patient = pd.read_excel(args.annotate)
+                columns = [
+                    "CHROM",
+                    "POS",
+                    "REF",
+                    "ALT",
+                    "GENE_NAME",
+                    "HGVS.C",
+                    "HGVS.P",
+                    "FREQ",
+                    "ALLELE_FREQ",
+                ]
                 db = variantsdb.VariantsDB.from_csvdb(
-                    variantsdb.variantsDBPath.rsplit("/", maxsplit=1)[0]
+                    variantsdb.variantsDBPath.rsplit("/", maxsplit=1)[0],
+                    columns=columns,
                 )
                 patient = db.annotate_excel(patient, fileName)
         except Exception as err:
             logger.error("Add patient process failed")
             logger.debug(f"There was an error: {err}", exc_info=True)
 
     def launchapi(self):
@@ -191,15 +306,16 @@
             required=True,
             help="File name of the Pipeline inside Pipelines folder",
         )
         parser.add_argument(
             "-FQ",
             required=True,
             help="Patient FastQ1 File Path - It needs to match exactly "
-            "the filename found inside Patients folder. Only this one is needed for Single End."
+            "the filename found inside Patients folder. Only this one is needed \
+            for Single End."
             "Two FastQs will be needed for Paired End (usage: -FQ Fastq1 -FQ Fastq2",
             action="append",
         )
         parser.add_argument(
             "-keeptmp",
             action="store_true",
             default=False,
@@ -289,15 +405,16 @@
             required=True,
             help="File name of the Pipeline inside Pipelines folder",
         )
         parser.add_argument(
             "-FQ",
             required=True,
             help="Patient FastQ1 File Path - It needs to match exactly "
-            "the filename found inside Patients folder. Only this one is needed for Single End."
+            "the filename found inside Patients folder. Only this one is needed \
+              for Single End."
             "Two FastQs will be needed for Paired End (usage: -FQ Fastq1 -FQ Fastq2",
             action="append",
         )
         parser.add_argument(
             "-keeptmp",
             action="store_true",
             default=False,
@@ -314,30 +431,30 @@
             default=0,
             type=int,
             help="Defines step to start running pipeline.",
         )
 
         # ignore first argument
         args = parser.parse_args(argv[2:])
-        pipe = cfg.pipelinesPath + args.Pipeline
+        pipe = configuration.pipelinesPath + args.Pipeline
 
         checkFile(pipe, args.Pipeline.split(".")[-1])
 
         newpipe = pipeline.Pipeline.from_json(pipe)
 
         if len(args.FQ) > 2:
             logger.error(
                 "Only Two FASTQ files allowed. The Input for FastQ Files was: ",
                 str(args.FQ),
             )
             return exit(1)
 
         elif len(args.FQ) == 2:
-            fq1 = cfg.patientPath + args.FQ[0]
-            fq2 = cfg.patientPath + args.FQ[1]
+            fq1 = configuration.patientPath + args.FQ[0]
+            fq2 = configuration.patientPath + args.FQ[1]
             checkFile(fq1, "." + fq1.split(".")[-1])
             checkFile(fq2, "." + fq2.split(".")[-1])
             if args.keeptmp:
                 newpipe.runpipeline(
                     fq1,
                     fq2,
                     keeptmp=True,
@@ -346,20 +463,23 @@
                 )
             else:
                 newpipe.runpipeline(
                     fq1, fq2, startStep=args.startStep, endStep=args.endStep
                 )
             return 0
         else:
-            fq1 = cfg.patientPath + args.FQ[0]
+            fq1 = configuration.patientPath + args.FQ[0]
             fq2 = ""
             checkFile(fq1, "." + fq1.split(".")[-1])
             if args.keeptmp:
                 newpipe.runpipeline(
-                    fq1, keeptmp=True, startStep=args.startStep, endStep=args.endStep
+                    fq1,
+                    keeptmp=True,
+                    startStep=args.startStep,
+                    endStep=args.endStep,
                 )
             else:
                 newpipe.runpipeline(fq1, startStep=args.startStep, endStep=args.endStep)
             return 0
 
     def abs_single(self):
         parser = argparse.ArgumentParser(description="Run study on a single patient")
@@ -367,85 +487,103 @@
             "-Panel",
             required=True,
             help="File path to Panel filename of Panel inside Panels folder",
         )
         parser.add_argument(
             "-Patient",
             required=True,
-            help="Patient File Path - It needs to match exactly to the one found inside Patients folder",
+            help="Patient File Path - It needs to match exactly to the one found \
+            inside Patients folder",
         )
         try:
             args = parser.parse_args(argv[2:])
             patient = args.Patient
             panel = args.Panel
             vcfanalysis.single(patient, panel)
         except Exception as error:
             logger.info("There was an error in the Panel Process")
             logger.debug(f"Error was: {error}")
 
     def single(self):
         # Description for panel usage
         parser = argparse.ArgumentParser(description="Run study on a single patient")
         parser.add_argument(
-            "-Panel", required=True, help="File name of Panel inside Panels folder"
+            "-Panel",
+            required=True,
+            help="File name of Panel inside Panels folder",
         )
         parser.add_argument(
             "-Patient",
             required=True,
-            help="Patient File Path - It needs to match exactly to the one found inside Patients folder",
+            help="Patient File Path - It needs to match exactly to the one found \
+              inside Patients folder",
         )
         # ignore first argument
         try:
             args = parser.parse_args(argv[2:])
-            panel = cfg.panelsPath + args.Panel + ".xlsx"
-            patient = cfg.patientPath + args.Patient
-            ptCheck = checkFile(patient, ".vcf")
-            pnCheck = checkFile(panel, ".xlsx")
+            panel = configuration.panelsPath + args.Panel + ".xlsx"
+            patient = configuration.patientPath + args.Patient
+            checkFile(patient, ".vcf")
+            checkFile(panel, ".xlsx")
             logger.info(
                 "Running %s on patient %s" % (str(args.Panel), str(args.Patient))
             )
             result = vcfmgr.ParsedVCF.from_vcf(patient).panel(panel)
             outpath = (
-                cfg.patientPath
+                configuration.patientPath
                 + result.name
                 + "/Panels/"
                 + result.name
                 + "_"
                 + args.Panel
                 + ".xlsx"
             )
             os.makedirs(os.path.dirname(outpath), exist_ok=True)
             result.vcf_to_excel(outpath)
             logger.info("Annotating VARDB Freq")
             fileName = outpath.rsplit("/", maxsplit=1)[1]
             patient = pd.read_excel(outpath)
+            # columns = [
+            #    "CHROM",
+            #    "POS",
+            #    "REF",
+            #    "ALT",
+            #    "GENE_NAME",
+            #    "HGVS.C",
+            #    "HGVS.P",
+            #    "FREQ",
+            #    "ALLELE_FREQ",
+            # ]
             db = variantsdb.VariantsDB.from_csvdb(
-                variantsdb.variantsDBPath.rsplit("/", maxsplit=1)[0]
+                configuration.variantsDBPath.rsplit("/", maxsplit=1)[0],
+                #    columns=columns,
             )
             patient = db.annotate_excel(patient, fileName)
             logger.info("Single Analisis Complete")
             logger.info("File available at:%s" % outpath)
         except Exception as err:
             logger.info("Single Analisis Failed")
-            logger.debug(f"Error was: {err}")
+            logger.debug(f"Error was: {err}", exc_info=True)
 
         return 0
 
     def duos(self):
         # Description for duos usage
         parser = argparse.ArgumentParser(description="Run Duos Study on two patients")
         parser.add_argument(
             "-Patient1",
             required=True,
-            help="Patient 1 File Path - It needs to match exactly to the one found inside Patients folder",
+            help="Patient 1 File Path - It needs to match exactly to the one found \
+                  inside Patients folder",
         )
         parser.add_argument(
             "-Patient2",
             required=True,
-            help="Patient 2 File Path - It needs to match exactly to the one found inside Patients folder",
+            help="Patient 2 File Path - It needs to match exactly to the one found \
+                  inside Patients folder",
         )
         parser.add_argument(
             "--VennPlace",
             const=None,
             choices=["A", "B", "A:B"],
             nargs="?",
             help="Place in a Venn Diagram to obtain variants from",
@@ -453,56 +591,58 @@
         parser.add_argument(
             "--Panel", nargs="?", const=None, help="Panel to run on Duos study"
         )
         parser.add_argument(
             "--Filter",
             nargs="?",
             const=None,
-            help="Filter to apply. This function will filter out every row that includes the given text"
+            help="Filter to apply. This function will filter out every row that \
+                  includes the given text"
             " in the given column. For filtering Empty data, TEXT keyword is 'Empty'",
             metavar=("COLUMN TEXT"),
             action="append",
         )
         # ignore first argument
         try:
             args = parser.parse_args(argv[2:])
-            patient1 = cfg.patientPath + args.Patient1
-            patient2 = cfg.patientPath + args.Patient2
+            patient1 = configuration.patientPath + args.Patient1
+            patient2 = configuration.patientPath + args.Patient2
             # Checks file existence and type for patients
-            pt1Check = checkFile(patient1, ".vcf")
-            pt2Check = checkFile(patient2, ".vcf")
+            checkFile(patient1, ".vcf")
+            checkFile(patient2, ".vcf")
             logger.info(
                 "Running Duos Study on %s and %s"
                 % (str(args.Patient1), str(args.Patient2))
             )
             pvcfs = vcfmgr.ParsedVCF.mp_parser(patient1, patient2)
             result = pvcfs[0].duos(pvcfs[1], VENNPLACE=args.VennPlace)
             resultname = result.name
             outpath = (
-                cfg.resultsPath
+                configuration.resultsPath
                 + "Duos/"
                 + result.name.replace(":", "_")
                 + "/"
                 + result.name.replace(":", "_")
             )
             result.name = resultname
             if args.VennPlace is not None:
                 outpath = outpath + "_Venn" + args.VennPlace.replace(":", "_")
             if args.Panel is not None:
                 logger.info("Running panel {}".format(args.Panel))
-                panel = cfg.panelsPath + args.Panel + ".xlsx"
+                panel = configuration.panelsPath + args.Panel + ".xlsx"
                 checkFile(panel, ".xlsx")
                 result = result.panel(panel)
                 result.name = resultname
                 outpath = outpath + "_P" + args.Panel
             if args.Filter[0] is not None:
                 for x in args.Filter:
                     if (len(x.split())) != 2:
                         logger.error(
-                            "--Filter accepts only two arguments. Usage: --Filter COLUMN_NAME TEXT_TO_FILTER"
+                            "--Filter accepts only two arguments. \
+                            Usage: --Filter COLUMN_NAME TEXT_TO_FILTER"
                         )
                         exit(1)
                     else:
                         x = x.split()
                         if x[1] == "Empty":
                             result = result[result[x[0]] != ""]
                         else:
@@ -510,35 +650,36 @@
                     result.name = resultname
                     outpath = outpath + "_F" + str(x[0]) + str(x[1])
             outpath = outpath + ".xlsx"
             logger.info("Writing Result File")
             result.vcf_to_excel(outpath)
             logger.info("Duos Analisis Complete")
             logger.info("File available at:%s" % outpath)
-        except:
+        except Exception as err:
             logger.info("Duos Analisis Failed")
+            logger.debug(f"Error was: {err}")
         return 0
 
     def diffvcf(self):
         # Description for duos usage
         try:
             patient1 = argv[2]
             patient2 = argv[3]
             # Checks file existence and type for patients
-            pt1Check = checkFile(patient1, ".vcf")
-            pt2Check = checkFile(patient2, ".vcf")
+            checkFile(patient1, ".vcf")
+            checkFile(patient2, ".vcf")
             logger.info(
                 "Evaluating differences between %s and %s"
                 % (str(patient1), str(patient2))
             )
             pvcfs = vcfmgr.ParsedVCF.mp_parser(patient1, patient2)
             result = pvcfs[0].duos(pvcfs[1])
             resultname = result.name
             outpath = (
-                cfg.resultsPath
+                configuration.resultsPath
                 + "Diffs/"
                 + result.name.replace(":", "_")
                 + "/"
                 + result.name.replace(":", "_")
             )
             result.name = resultname
             outpath = outpath + ".xlsx"
@@ -552,34 +693,41 @@
         return 0
 
     def trios(self):
         parser = argparse.ArgumentParser(description="Run Trios Study on two patients")
         parser.add_argument(
             "-Patient1",
             required=True,
-            help="Patient 1 File Path - It needs to match exactly to the one found inside Patients folder",
+            help="Patient 1 File Path - It needs to match exactly to the \
+                one found inside Patients folder",
         )
         parser.add_argument(
             "-Patient2",
             required=True,
-            help="Patient 2 File Path - It needs to match exactly to the one found inside Patients folder",
+            help="Patient 2 File Path - It needs to match exactly to the \
+                one found inside Patients folder",
         )
         parser.add_argument(
             "-Patient3",
             required=True,
-            help="Patient 3 File Path - It needs to match exactly to the one found inside Patients folder",
+            help="Patient 3 File Path - It needs to match exactly to the \
+                one found inside Patients folder",
         )
         parser.add_argument(
-            "--Panel", nargs="?", const=None, help="Panel to run on Trios study"
+            "--Panel",
+            nargs="?",
+            const=None,
+            help="Panel to run on Trios study",
         )
         parser.add_argument(
             "--Filter",
             nargs="?",
             const=None,
-            help="Filter to apply. This function will filter out every row that includes the given text"
+            help="Filter to apply. This function will filter out every row \
+                that includes the given text"
             " in the given column. For filtering Empty data, TEXT keyword is 'Empty'",
             metavar=("COLUMN TEXT"),
             action="append",
         )
         parser.add_argument(
             "--VennPlace",
             default=None,
@@ -587,71 +735,74 @@
             nargs="?",
             choices=["A", "B", "C", "A:B", "A:C", "B:C", "A:B:C", "ALL"],
             help="Place in a Venn Diagram to obtain variants from",
         )
         try:
             # ignore first argument
             args = parser.parse_args(argv[2:])
-            patient1 = cfg.patientPath + args.Patient1
-            patient2 = cfg.patientPath + args.Patient2
-            patient3 = cfg.patientPath + args.Patient3
+            patient1 = configuration.patientPath + args.Patient1
+            patient2 = configuration.patientPath + args.Patient2
+            patient3 = configuration.patientPath + args.Patient3
             # Checks file existence and type for patients
-            pt1Check = checkFile(patient1, ".vcf")
-            pt2Check = checkFile(patient2, ".vcf")
-            pt3Check = checkFile(patient3, ".vcf")
+            checkFile(patient1, ".vcf")
+            checkFile(patient2, ".vcf")
+            checkFile(patient3, ".vcf")
             logger.info(
                 "Running Trios Study on %s, %s and %s"
                 % (str(args.Patient1), str(args.Patient2), str(args.Patient3))
             )
             pvcfs = vcfmgr.ParsedVCF.mp_parser(patient1, patient2, patient3)
             result = pvcfs[0].duos(pvcfs[1]).duos(pvcfs[2], VENNPLACE=args.VennPlace)
             resultname = result.name
             outpath = (
-                cfg.resultsPath
+                configuration.resultsPath
                 + "Trios/"
                 + result.name.replace(":", "_")
                 + "/"
                 + result.name.replace(":", "_")
             )
             result.name = resultname
             if args.VennPlace is not None:
                 outpath = outpath + "_Venn" + args.VennPlace.replace(":", "_")
             # check if there is a Panel Requested
             if args.Panel:
                 logger.info("Running panel {}".format(args.Panel))
-                panel = cfg.panelsPath + args.Panel + ".xlsx"
+                panel = configuration.panelsPath + args.Panel + ".xlsx"
                 checkFile(panel, ".xlsx")
                 result = result.panel(panel)
                 result.name = resultname
                 outpath = outpath + "_Panel" + args.Panel
             # check if there is a Filter Requested
             if args.Filter[0] is not None:
                 for x in args.Filter:
                     if (len(x.split())) != 2:
                         logger.error(
-                            "--Filter accepts only two arguments. Usage: --Filter COLUMN_NAME TEXT_TO_FILTER"
+                            "--Filter accepts only two arguments. \
+                                Usage: --Filter COLUMN_NAME TEXT_TO_FILTER"
                         )
                         exit(1)
                     else:
                         x = x.split()
                         if x[1] == "Empty":
                             result = result[result[x[0]] != ""]
                         else:
                             result = result[~result[x[0]].str.contains(x[1])]
                         result.name = resultname
                         outpath = outpath + "_Filter" + str(x[0]) + str(x[1])
             outpath = outpath + ".xlsx"
             result.vcf_to_excel(outpath)
             logger.info("Trios Analisis Complete")
             logger.info("File available at:%s" % outpath)
-        except:
+        except Exception as e:
             logger.info("Trios Analisis Failed")
+            logger.debug("Error: %s" % str(e))
         return 0
 
 
 def main():
-    cfg.setup_logging()
+
+    configuration.setup_logging()
     Parser()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `MODApy-0.7.8/MODApy/coverage.py` & `MODApy-0.8.0/MODApy/coverage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import multiprocessing as mp
 import subprocess
 import traceback
 
-import pandas as pd
+from MODApy.cfg import configuration
 
-from MODApy.cfg import cfg
+import pandas as pd
 
 logger = logging.getLogger(__name__)
 
 
 def generate_coverage(file):
     cmd = "bedtools"
     args = " genomecov -ibam {} -bga".format(file)
@@ -21,24 +21,26 @@
 
 
 def panel_intersect(file, panel_file):
     cmd = "bedtools"
     args = " intersect -a {} -b {}".format(file, panel_file)
     with open(
         "{}_{}.bed".format(
-            file.rsplit(".", maxsplit=1)[0], panel_file.rsplit(".", maxsplit=1)[0]
+            file.rsplit(".", maxsplit=1)[0],
+            panel_file.rsplit(".", maxsplit=1)[0],
         ),
         "w",
     ) as output:
         subprocess.Popen(cmd + args, stdout=output, stderr=output, shell=True)
 
 
 def annotate_genes(file, gene_file):
     cmd = "bedtools"
-    args = " intersect -a {} -b {} -wb | awk -v OFS='\t' '{{print $1,$2,$3,$4,$8}}'".format(
+    args = " intersect -a {} -b {} -wb | awk -v OFS='\t' \
+        '{{print $1,$2,$3,$4,$8}}'".format(
         file, gene_file
     )
     with open(
         "{}_with_genes.cov".format(file.rsplit(".", maxsplit=1)[0]), "w"
     ) as output:
         p2 = subprocess.Popen(cmd + args, stdout=output, stderr=output, shell=True)
         p2.wait()
@@ -54,15 +56,15 @@
     )
     csv.groupby(["EXON", "CHROM"]).DEPTH.describe().drop(columns="count").to_csv(
         file.rsplit(".", maxsplit=1)[0] + "_coverage_per_exon.csv"
     )
 
 
 def main(files, bedfile, panelfile=None):
-    pool = mp.Pool(processes=int(cfg["GENERAL"]["cores"]))
+    pool = mp.Pool(processes=int(configuration.cfg["GENERAL"]["cores"]))
     try:
         logger.info("Generating coverage on {}".format(files))
         r = pool.map_async(generate_coverage, files)
         r.wait()
         covfiles = [
             "{}_genomecov.bed".format(file.rsplit(".", maxsplit=1)[0]) for file in files
         ]
```

### Comparing `MODApy-0.7.8/MODApy/downloader.py` & `MODApy-0.8.0/MODApy/downloader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,46 @@
+# TODO: refactor this to modularize the code
+
 import hashlib
 import json
 import logging
 import os
 import re
 import tarfile
 
+from MODApy import configuration
+
 import openpyxl
+
 import pandas as pd
+
 import requests
-import xlrd
+
 from tqdm import tqdm
 
-from MODApy import cfg
+import xlrd
+
 
 logger = logging.getLogger(__name__)
-downlog = cfg.rootDir + "/logs/downloads.log"
+downlog = configuration.rootDir + "/logs/downloads.log"
 
 
 def get_links(filename):
     link_list = list()
     # If filename is an url
     if (
         filename.startswith("http://")
         or filename.startswith("https://")
         or filename.startswith("ftp://")
     ):
         logger.debug("URL to download")
         download(filename)
     elif filename.startswith("www"):
         logger.error("URLs must start with http:// or https:// or ftp://")
-        exit(1)
+        raise ValueError("URLs must start with http:// or https:// or ftp://")
     # If filename is an excel file
     elif os.path.exists(filename):
         if filename.rsplit(".")[-1] == "xlsx":
             logger.info("Parsing file to find URLs")
             wb = openpyxl.load_workbook(filename=filename)
             for ws in wb:
                 for row in ws.rows:
@@ -87,49 +94,50 @@
                 down_dict.update({x: "Pending" for x in linksdict})
             with open(downlog, "w") as dlog:
                 json.dump(down_dict, dlog, indent=4)
             for link in linksdict:
                 download(link, linksdict[link])
         else:
             logger.error("File extension must be xlsx or xls.")
-            exit(1)
+            raise ValueError("File extension must be xlsx or xls.")
     else:
         logger.error("File or URL provided is not valid")
-        exit(1)
+        raise ValueError("File or URL provided is not valid")
 
 
 def download(url, md5=None):
     """
     @param: url to download file
     """
-    outputdir = cfg.patientPath + url.rsplit("/")[-1].split(".")[0] + "/"
+    outputdir = configuration.patientPath + url.rsplit("/")[-1].split(".")[0] + "/"
     outputfile = url.rsplit("/")[-1]
     outpath = outputdir + outputfile
-    tmpdir = cfg.tmpDir
-    tmppath = cfg.tmpDir + outputfile
+    tmpdir = configuration.tmpDir
+    tmppath = configuration.tmpDir + outputfile
     os.makedirs(outputdir, exist_ok=True)
     os.makedirs(tmpdir, exist_ok=True)
     logger.info("Downloading %s to %s" % (url, outpath))
     try:
         response = requests.head(url)
-    except:
+    except Exception as e:
         logger.info("Connection Failed")
         logger.debug("Downloader Connection Failed", exc_info=True)
-        exit(1)
+        logger.debug(e)
+        raise ConnectionError("Connection Failed")
     else:
         if response.status_code == 200:
             if "Content-Length" in response.headers.keys():
                 file_size = int(response.headers["Content-Length"])
             else:
                 logger.info("Could not get file size")
                 file_size = 0
         else:
             logger.info("Connection Failed")
             logger.debug("Downloader Connection Failed", exc_info=True)
-            exit(1)
+            raise ConnectionError("Connection Failed")
     if os.path.exists(tmppath):
         first_byte = os.path.getsize(tmppath)
     else:
         first_byte = 0
     header = {"Range": "bytes=%s-%s" % (first_byte, file_size)}
     with open(downlog, "r") as dlog:
         down_dict = json.load(dlog)
@@ -141,15 +149,15 @@
         initial=first_byte,
         unit="B",
         unit_scale=True,
         desc=url.split("/")[-1],
     )
     try:
         req = requests.get(url, headers=header, stream=True)
-        with (open(tmppath, "ab")) as f:
+        with open(tmppath, "ab") as f:
             for chunk in req.iter_content(chunk_size=1024):
                 if chunk:
                     f.write(chunk)
                     pbar.update(1024)
         pbar.close()
         with open(downlog, "r") as dlog:
             down_dict = json.load(dlog)
@@ -170,31 +178,34 @@
                     logger.info("Moving file to destination folder")
                     os.rename(tmppath, outpath)
                     try:
                         logger.info("Extracting tar file")
                         tf = tarfile.open(outpath)
                         tf.extractall(outputdir)
                         logger.info("Extraction finished")
-                    except:
+                    except Exception as e:
                         logger.error("Extraction failed")
+                        logger.debug("Extraction failed, Error was str(%e)" % e)
                         logger.debug("", exc_info=True)
-                        exit(1)
+                        raise RuntimeError("Extraction failed, Error was str(%e)" % e)
                 else:
                     print(file_md5, md5)
                     logger.info("MD5 Verification Failed")
                     logger.error("Error with the download")
-                    exit(1)
+                    raise AssertionError("MD5 Verification Failed")
             try:
                 os.removedirs(tmpdir)
-            except:
+            except Exception as e:
                 logger.debug(tmpdir + " is not empty.")
+                logger.debug("Error was str(%e)" % e)
         with open(downlog, "w") as dlog:
             json.dump(down_dict, dlog, indent=4)
-    except:
+    except Exception as e:
         with open(downlog, "r") as dlog:
             down_dict = json.load(dlog)
             down_dict.update({url: "Download Error"})
             logger.error("Error with download")
+            logger.debug("Error was str(%e)" % e)
             logger.debug("", exc_info=True)
         with open(downlog, "w") as dlog:
             json.dump(down_dict, dlog, indent=4)
     return file_size
```

### Comparing `MODApy-0.7.8/MODApy/modaapi.py` & `MODApy-0.8.0/MODApy/modaapi.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import logging
+from typing import Optional
+
+from MODApy import configuration, pipeline, vcfanalysis
+from MODApy.utils import checkFile
+
 from fastapi import FastAPI, HTTPException, status
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import JSONResponse
-from typing import Optional
+
 from pydantic import BaseModel
-from MODApy import cfg, pipeline, vcfanalysis
-from MODApy.utils import checkFile
-import logging
 
 logger = logging.getLogger()
 app = FastAPI()
 
 origins = [
     "*",
 ]
@@ -20,72 +23,135 @@
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"],
 )
 
 
 class Pipeline(BaseModel):
+    """
+    Represents a pipeline.
+
+    Attributes:
+        Pipeline (str): The pipeline name.
+        FQ_1 (str): The first FastQ file.
+        FQ_2 (str, optional): The second FastQ file. Defaults to "".
+        startStep (int, optional): The starting step. Defaults to 0.
+        endStep (int, optional): The ending step. Defaults to 0.
+        keeptmp (bool, optional): Whether to keep temporary files. Defaults to False.
+    """
+
     Pipeline: str
     FQ_1: str
     FQ_2: Optional[str] = ""
     startStep: Optional[int] = 0
     endStep: Optional[int] = 0
     keeptmp: Optional[bool] = False
 
 
 class Single(BaseModel):
+    """
+    Represents single input data.
+
+    Attributes:
+        patient (str): The patient identifier.
+        panel (str): The panel identifier.
+    """
+
     patient: str
     panel: str
 
 
 class Duos(BaseModel):
+    """
+    Represents duos input data.
+
+    Attributes:
+        patient1 (str): The first patient identifier.
+        patient2 (str): The second patient identifier.
+        panel (str, optional): The panel identifier. Defaults to None.
+        vennPlace (str, optional): The vennPlace identifier. Defaults to None.
+        filter (str, optional): The filter identifier. Defaults to None.
+    """
+
     patient1: str
     patient2: str
     panel: Optional[str] = None
     vennPlace: Optional[str] = None
     filter: Optional[str] = None
 
 
 class Trios(BaseModel):
+    """
+    Represents trios input data.
+
+    Attributes:
+        patient1 (str): The first patient identifier.
+        patient2 (str): The second patient identifier.
+        patient3 (str): The third patient identifier.
+        panel (str, optional): The panel identifier. Defaults to None.
+        vennPlace (str, optional): The vennPlace identifier. Defaults to None.
+        filter (str, optional): The filter identifier. Defaults to None.
+    """
+
     patient1: str
     patient2: str
     patient3: str
     panel: Optional[str] = None
     vennPlace: Optional[str] = None
     filter: Optional[str] = None
 
 
 @app.post("/modaapi/single")
 async def single(data: Single):
+    """
+    Handles single input data.
+
+    Parameters:
+        data (Single): The single input data.
+
+    Returns:
+        JSONResponse: The response containing the job ID.
+    """
     data = data.dict()
     try:
         panel = data["panel"]
         patient = data["patient"]
-        job_id = cfg.short_queue.enqueue(vcfanalysis.single, args=[patient, panel])
+        job_id = configuration.short_queue.enqueue(
+            vcfanalysis.single, args=[patient, panel]
+        )
         job_id = job_id.id
         return JSONResponse(
             status_code=status.HTTP_202_ACCEPTED,
             content=f"Job Queued. Job id is {job_id}",
         )
     except Exception as err:
         logger.error("Api error on Single")
         logger.debug(f"Error was: {err}", exc_info=True)
         raise HTTPException(status_code=404, detail=str(err))
 
 
 @app.post("/modaapi/duos")
 async def duos(data: Duos):
+    """
+    Handles duos input data.
+
+    Parameters:
+        data (Duos): The duos input data.
+
+    Returns:
+        JSONResponse: The response containing the job ID.
+    """
     data = data.dict()
     try:
         patient1 = data["patient1"]
         patient2 = data["patient2"]
         VennPlace = data["vennPlace"]
         Panel = data["panel"]
         Filter = data["filter"]
-        job_id = cfg.short_queue.enqueue(
+        job_id = configuration.short_queue.enqueue(
             vcfanalysis.duos,
             args=[patient1, patient2],
             kwargs={"VennPlace": VennPlace, "Panel": Panel, "Filter": Filter},
         )
         job_id = job_id.id
         return JSONResponse(
             status_code=status.HTTP_202_ACCEPTED,
@@ -95,24 +161,33 @@
         logger.error("Api error on Duos")
         logger.debug(f"Error was: {err}", exc_info=True)
         raise HTTPException(status_code=404, detail=str(err))
 
 
 @app.post("/modaapi/trios")
 async def trios(data: Trios):
+    """
+    Handles trios input data.
+
+    Parameters:
+        data (Trios): The trios input data.
+
+    Returns:
+        JSONResponse: The response containing the job ID.
+    """
     data = data.dict()
     try:
         patient1 = data["patient1"]
         patient2 = data["patient2"]
         patient3 = data["patient3"]
         VennPlace = data["vennPlace"]
         Panel = data["panel"]
         Filter = data["filter"]
         # Checks file existence and type for patients
-        job_id = cfg.short_queue.enqueue(
+        job_id = configuration.short_queue.enqueue(
             vcfanalysis.trios,
             args=[patient1, patient2, patient3],
             kwargs={"VennPlace": VennPlace, "Panel": Panel, "Filter": Filter},
         )
         job_id = job_id.id
         return JSONResponse(
             status_code=status.HTTP_202_ACCEPTED,
@@ -122,29 +197,37 @@
         logger.error("Api error on Trios")
         logger.debug(f"Error was: {err}", exc_info=True)
         raise HTTPException(status_code=404, detail=str(err))
 
 
 @app.post("/modaapi/pipeline")
 async def run_pipeline(data: Pipeline):
+    """
+    Runs the pipeline.
+
+    Parameters:
+        data (Pipeline): The pipeline data.
+
+    Returns:
+        JSONResponse: The response containing the job ID.
+    """
     try:
         data = data.dict()
         pipe = data["Pipeline"]
 
         checkFile(pipe, data["Pipeline"].split(".")[-1])
 
         newpipe = pipeline.Pipeline.from_json(pipe)
         fq1 = data["FQ_1"]
         fq2 = data["FQ_2"]
 
         if fq2 != "":
-
             checkFile(fq1, "." + fq1.split(".")[-1])
             checkFile(fq2, "." + fq2.split(".")[-1])
-            job_id = cfg.long_queue.enqueue(
+            job_id = configuration.long_queue.enqueue(
                 newpipe.runpipeline,
                 args=[fq1, fq2],
                 kwargs={
                     "keeptmp": data["keeptmp"],
                     "startStep": data["startStep"],
                     "endStep": data["endStep"],
                 },
@@ -152,15 +235,15 @@
             job_id = job_id.id
             return JSONResponse(
                 status_code=status.HTTP_202_ACCEPTED,
                 content=f"Job Queued. Job id is {job_id}",
             )
         else:
             checkFile(fq1, "." + fq1.split(".")[-1])
-            job_id = cfg.long_queue.enqueue(
+            job_id = configuration.long_queue.enqueue(
                 newpipe.runpipeline,
                 args=[fq1],
                 kwargs={
                     "keeptmp": data["keeptmp"],
                     "startStep": data["startStep"],
                     "endStep": data["endStep"],
                 },
```

### Comparing `MODApy-0.7.8/MODApy/pipeline.py` & `MODApy-0.8.0/MODApy/pipeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import json
 import logging
 import os
 import shlex
 import shutil
 import subprocess
 
+from MODApy import configuration, vcfmgr
+
 import xmltodict
+
 import yaml
 
-from MODApy import cfg, vcfmgr
 
 logger = logging.getLogger(__name__)
 logger2 = logging.getLogger("Pipeline Module")
-os.makedirs(cfg.rootDir + '/logs', exist_ok=True)
-hdlr = logging.FileHandler(cfg.rootDir + "/logs/pipe_run.log")
+os.makedirs(configuration.rootDir + "/logs", exist_ok=True)
+hdlr = logging.FileHandler(configuration.rootDir + "/logs/pipe_run.log")
 formatter = logging.Formatter("%(asctime)s %(name)-25s %(levelname)-8s %(message)s")
 hdlr.setFormatter(formatter)
 logger2.addHandler(hdlr)
 logger2.setLevel(logging.DEBUG)
 
 
 # TODO: restructure pipeline, being less open, so less prone to errors
@@ -25,61 +27,132 @@
 
 class PipeStep(object):
     """
     Class defined for each step of the Pipeline
     """
 
     def __init__(self, name, command, subcommand, version, inputfile, outputfile, args):
+        """
+        Initializes a PipeStep object.
+
+        Parameters
+        ----------
+        name : str
+            Name of the step.
+        command : str
+            Command to be executed for the step.
+        subcommand : str
+            Subcommand to be executed for the step.
+        version : str
+            Version of the command.
+        inputfile : str or list
+            Path to the input file(s).
+        outputfile : str
+            Path to the output file.
+        args : str
+            Additional arguments for the command.
+        """
         self.name = name
         self.command = command
         self.subcommand = subcommand
         self.version = version
         self.inputfile = inputfile
         self.outputfile = outputfile
         self.args = args
 
     def __str__(self):
+        """
+        Returns the name of the step as a string.
+
+        Returns
+        -------
+        str
+            Name of the step.
+        """
         return self.name
 
     def __repr__(self):
+        """
+        Returns the name of the step as a string.
+
+        Returns
+        -------
+        str
+            Name of the step.
+        """
         return self.name
 
     def stepinfo(self):
-        print("Name:", self.name)
-        print("Command", self.command + self.version, self.subcommand, self.args)
-        print("Input File:", self.inputfile)
-        print("Output File:", self.outputfile)
+        """
+        Prints information about the step.
+        """
+        logger.info("Name:", self.name)
+        logger.info("Command", self.command + self.version, self.subcommand, self.args)
+        logger.info("Input File:", self.inputfile)
+        logger.info("Output File:", self.outputfile)
 
 
 class Pipeline(object):
     """
     General Class for Pipelines
     """
 
     def __init__(self, name, reference, url="", description=""):
+        """
+        Initializes a Pipeline object.
+
+        Parameters
+        ----------
+        name : str
+            Name of the pipeline.
+        reference : str
+            Reference for the pipeline.
+        url : str, optional
+            URL for the pipeline, by default "".
+        description : str, optional
+            Description of the pipeline, by default "".
+        """
         self.name = name
         self.url = url
         self.description = description
         self.reference = reference
         self.required_files = []
         self.steps = []
 
     def add_steps(self, step):
+        """
+        Adds a step to the pipeline.
+
+        Parameters
+        ----------
+        step : PipeStep
+            Step to be added to the pipeline.
+        """
         self.steps.append(step)
 
     def add_req_files(self, path):
+        """
+        Adds a required file to the pipeline.
+
+        Parameters
+        ----------
+        path : str
+            Path to the required file.
+        """
         self.required_files.append(path)
 
     @staticmethod
     def _buildpipe(pipedict):
         """
         Private Class Method to build pipeline from loaded json,xml or yaml
+
         Parameters
-        --------------------
-        pipefile File loaded by from_json, from_xml or from_yaml
+        ----------
+        pipedict : dict
+            Dictionary representing the pipeline.
         """
         name = pipedict["INFO"]["name"]
         url = pipedict["INFO"]["url"]
         description = pipedict["INFO"]["description"]
         reference = pipedict["INFO"]["reference"]
 
         newpipe = Pipeline(name, reference, url, description)
@@ -104,14 +177,15 @@
 
         return newpipe
 
     @classmethod
     def from_json(cls, jsonpath):
         """
         Class Method to read json and build the Pipeline
+
         Parameters
         ----------
         jsonpath
             Path to the json file used to create the Pipeline.
 
         Returns Pipeline object
         """
@@ -122,14 +196,15 @@
 
         return builtpipe
 
     @classmethod
     def from_yaml(cls, yamlpath):
         """
         Class Method to read yaml and build the Pipeline
+
         Parameters
         ----------
         jsonpath
             Path to the yaml file used to create the Pipeline.
 
         Returns Pipeline object
         """
@@ -139,14 +214,15 @@
 
         return builtpipe
 
     @classmethod
     def from_xml(cls, xmlpath):
         """
         Class Method to parse xml and build the Pipeline
+
         Parameters
         ----------
         xmlpath
             Path to the xml file used to create the Pipeline.
 
         Returns Pipeline object
         """
@@ -163,42 +239,51 @@
         keeptmp=False,
         startStep=0,
         endStep=0,
         patientPath=None,
     ):
         """
         Method to run the Pipeline
+
         Parameters
         ----------
         fastq1
             Path to the first fastq file.
         fastq2
             Path to the second fastq file, in case of paired reads.
         """
 
-        """
-        Method to run selected Pipeline on fastq files
-        """
         try:
             logger.info(self.steps)
             logger.info("Nro de Pasos: %s" % str(len(self.steps)))
             logger2.info(self.steps)
             logger2.info("Nro de Pasos: %s" % str(len(self.steps)))
-            patientname = fastq1.split("/")[-1].split(".")[0].split("_")[0]
-            ref = cfg.referencesPath + self.reference + "/" + self.reference + ".fa"
+            patientname = fastq1.split("/")[-1].split(".")[0].split("_1")[0]
+            ref = (
+                configuration.referencesPath
+                + self.reference
+                + "/"
+                + self.reference
+                + ".fa"
+            )
             pipedir = "".join(x for x in self.name if x.isalnum())
-            if patientPath == None:
-                patientPath = cfg.patientPath
-            if cfg.testFlag:
+            if patientPath is None:
+                patientPath = configuration.patientPath
+            if configuration.testFlag:
                 tmpdir = (
-                    cfg.testPath + "Pipelines/" + patientname + "/" + pipedir + "/tmp/"
+                    configuration.testPath
+                    + "Pipelines/"
+                    + patientname
+                    + "/"
+                    + pipedir
+                    + "/tmp/"
                 )
             else:
                 tmpdir = (
-                    cfg.resultsPath
+                    configuration.resultsPath
                     + "Pipelines/"
                     + patientname
                     + "/"
                     + pipedir
                     + "/tmp/"
                 )
 
@@ -214,59 +299,64 @@
             first = True
             if endStep == 0:
                 endStep = len(self.steps) + 1
             if startStep > 0:
                 first = False
             logger2.info(f"STARTSTEP {startStep}")
             for step in self.steps[startStep:endStep]:
-                if first == True:
+                if first is True:
                     logger2.debug("First Step")
                     first = False
-                    if type(step.inputfile) == list:
+                    if isinstance(step.inputfile, list):
                         if any(
                             x in y
                             for y in [fastq1, fastq2]
                             for x in [".fastq", ".fastq.gz", ".fq", ".fq.gz"]
                         ):
                             if (fastq1 is not None) & (fastq2 is not None):
                                 inputfile = fastq1 + " " + fastq2
                             else:
-                                print(
-                                    "WARNING: This pipeline was designed for Pair End and you are running it as Single End"
+                                logger.warn(
+                                    "WARNING: This pipeline was designed for Pair End \
+                                    and you are running it as Single End"
                                 )
                                 inputfile = fastq1
-                    elif type(step.inputfile) == str:
+                    elif isinstance(step.inputfile, str):
                         if any(
                             x in y
                             for y in [fastq1]
                             for x in [".fastq", ".fastq.gz", ".fq", ".fq.gz"]
                         ):
                             if (fastq1 is not None) & (fastq2 is not None):
-                                print(
-                                    "WARNING: This pipeline was designed for Single End and you are running it as Pair End"
+                                logger.warn(
+                                    "WARNING: This pipeline was designed for Single \
+                                        End and you are running it as Pair End"
                                 )
                                 inputfile = fastq1 + " " + fastq2
                         else:
                             inputfile = fastq1
-                # If it's not first step, input depends on output of previous step + patientname
+                # If it's not first step, input depends on output of previous
+                # step + patientname
                 else:
-                    if type(step.inputfile) == list:
+                    if isinstance(step.inputfile, str):
                         inputfile1 = step.inputfile[0].replace(
-                            "patientname", tmpdir + patientname + "/" + patientname
+                            "patientname",
+                            tmpdir + patientname + "/" + patientname,
                         )
                         inputfile2 = step.inputfile[1].replace(
-                            "patientname", tmpdir + patientname + "/" + patientname
+                            "patientname",
+                            tmpdir + patientname + "/" + patientname,
                         )
                         inputfile = inputfile1 + " " + inputfile2
-                    elif type(step.inputfile) == str:
+                    elif isinstance(step.inputfile, str):
                         inputfile = step.inputfile.replace(
                             "patientname", tmpdir + patientname
                         )
                 # replaces patient name in outputfiles
-                if type(step.outputfile) == str:
+                if isinstance(step.outputfile, str):
                     outputfile = step.outputfile.replace(
                         "patientname", tmpdir + patientname
                     )
                 else:
                     return "Error Parsing output file. It should be a string."
 
                 logger2.info(step.name)
@@ -276,45 +366,45 @@
                     .replace("samplename", samplename)
                 )
                 cmdver = step.version.replace(".", "_")
                 javacmds = ["GATK", "picard", "SnpSift", "snpEff"]
                 if any(javacmd in step.command for javacmd in javacmds):
                     cmd = (
                         "java -jar -Xmx12G -Djava.io.tmpdir=%s " % "~/.tmp"
-                        + cfg.binPath
+                        + configuration.binPath
                         + step.command
                         + "/"
                         + step.command
                         + "_"
                         + cmdver
                         + ".jar "
                         + step.subcommand
                     )
                 else:
                     cmd = (
-                        cfg.binPath
+                        configuration.binPath
                         + step.command
                         + "/"
                         + step.command
                         + "_"
                         + cmdver
                         + " "
                         + step.subcommand
                     )
                 if "HaplotypeCaller" in cmd:
                     cmdstr = cmd + " " + args + " " + inputfile + " " + outputfile
                 else:
                     cmdstr = cmd + " " + args + " " + " " + inputfile + " " + outputfile
-                    print(cmd)
+                    logger.info(f"Command is: {cmd}")
                 cmd = shlex.split(cmdstr)
 
                 logging.info("Subprocess: " + cmdstr)
                 logger2.info("Subprocess: " + cmdstr)
                 stdcmds = ["bwa", "bedtools", "snpEff", "SnpSift"]
-                print(cmd)
+                logger.info(f"Command is: {cmd}")
                 try:
                     if any(stdcmd in s for s in cmd for stdcmd in stdcmds):
                         output = cmd[-1]
                         del cmd[-1]
                         with open(output, "w+") as out:
                             cmdrun = subprocess.Popen(
                                 cmd,
@@ -351,52 +441,56 @@
 
                 except (OSError, subprocess.CalledProcessError) as exception:
                     logging.debug("Subprocess failed")
                     logging.debug("Exception ocurred: " + str(exception))
                     logger2.debug("Subprocess failed")
                     logger2.debug("Exception ocurred: " + str(exception))
                     logging.info(
-                        "There was an error when running the pipeline. Please check logs for more info"
+                        "There was an error when running the pipeline. Please \
+                            check logs for more info"
                     )
                     logger2.info(
-                        "There was an error when running the pipeline. Please check logs for more info"
+                        "There was an error when running the pipeline. Please \
+                            check logs for more info"
                     )
                     exit(1)
                 else:
                     logging.info("Subprocess finished")
                     logger2.info("Subprocess finished")
-            if cfg.testFlag:
+            if configuration.testFlag:
                 if os.path.exists(tmpdir + patientname + "_MODApy.final.vcf"):
                     file = (
-                        cfg.testPath
+                        configuration.testPath
                         + patientname
                         + "_MODApy/"
                         + patientname
                         + "_MODApy.final.vcf"
                     )
-                    os.makedirs(cfg.testPath + patientname + "_MODApy", exist_ok=True)
+                    os.makedirs(
+                        configuration.testPath + patientname + "_MODApy", exist_ok=True
+                    )
                     shutil.move(tmpdir + patientname + "_MODApy.final.vcf", file)
                     logger2.info("Parsing final VCF file")
                     logging.info("Parsing final VCF file")
                     vcfmgr.ParsedVCF.from_vcf(file).to_csv(
                         file.split(".vcf")[0] + ".csv", index=False
                     )
                 if os.path.exists(tmpdir + patientname + "_realigned_reads_recal.bam"):
                     shutil.move(
                         tmpdir + patientname + "_realigned_reads_recal.bam",
-                        cfg.testPath
+                        configuration.testPath
                         + patientname
                         + "_MODApy/"
                         + patientname
                         + "MODApy_realigned_reads_recal.bam",
                     )
                 if os.path.exists(tmpdir + patientname + "_realigned_reads_recal.bai"):
                     shutil.move(
                         tmpdir + patientname + "_realigned_reads_recal.bai",
-                        cfg.testPath
+                        configuration.testPath
                         + patientname
                         + "_MODApy/"
                         + patientname
                         + "MODApy_realigned_reads_recal.bai",
                     )
             else:
                 if os.path.exists(tmpdir + patientname + "_MODApy.final.vcf"):
@@ -442,13 +536,13 @@
             logger2.debug(f"Pipeline error: {error}", exc_info=True)
             logging.debug(f"Pipeline error: {error}", exc_info=True)
 
     def pipelineinfo(self):
         """
         Method to print Pipeline Info
         """
-        print("Name:", self.name)
-        print("Reference:", self.reference)
-        print("URL:", self.url)
-        print("Description:", self.description)
-        print("Additional Files Required:", self.required_files)
-        print("Steps:", self.steps)
+        logger.info("Name:", self.name)
+        logger.info("Reference:", self.reference)
+        logger.info("URL:", self.url)
+        logger.info("Description:", self.description)
+        logger.info("Additional Files Required:", self.required_files)
+        logger.info("Steps:", self.steps)
```

### Comparing `MODApy-0.7.8/MODApy/variantsdb.py` & `MODApy-0.8.0/MODApy/variantsdb.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import glob
 import logging
 import os
 
+from MODApy.cfg import configuration
+from MODApy.vcfmgr import ParsedVCF
+
 import cyvcf2
-import numpy as np
-import pandas as pd
 
-from functools import reduce
+import numpy as np
 
-from MODApy.cfg import variantsDBPath, patientPath, cfg, resultsPath
-from MODApy.vcfmgr import ParsedVCF
+import pandas as pd
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: FIND A MORE EFFICIENT WAY TO SUM EMPTY
 
 
@@ -22,44 +22,51 @@
     def _constructor(self):
         return VariantsDB
 
     @classmethod
     def from_exceldb(cls, excelpath):
         if os.path.exists(excelpath):
             try:
-                db = pd.read_excel(excelpath)
-
-            except:
-                logger.error("There was an error parsing excel File")
+                files = [f for f in glob.glob(excelpath + "/*.xls*")]
+                if len(files) == 0:
+                    return None
+                dfs = [pd.read_excel(x) for x in files]
+                db = pd.concat(dfs, sort=True)
+                del files
+                del dfs
+            except Exception as e:
+                logger.error("There was an error parsing Excel File")
                 logger.debug("", exc_info=True)
+                logger.debug(str(e))
                 exit(1)
         else:
-            logger.error("Path to excel file incorrect.")
+            logger.error("Path to Excel file incorrect.")
             exit(1)
         db.set_index(
             ["CHROM", "POS", "REF", "ALT", "GENE_NAME", "HGVS.C", "HGVS.P"],
             inplace=True,
         )
         db = db.pipe(VariantsDB)
         return db
 
     @classmethod
-    def from_csvdb(cls, csvpath):
+    def from_csvdb(cls, csvpath, columns=None):
         if os.path.exists(csvpath):
             try:
                 files = [f for f in glob.glob(csvpath + "/*.csv")]
                 if len(files) == 0:
                     return None
-                dfs = [pd.read_csv(x) for x in files]
+                dfs = [pd.read_csv(x, usecols=columns) for x in files]
                 db = pd.concat(dfs, sort=True)
                 del files
                 del dfs
-            except:
+            except Exception as e:
                 logger.error("There was an error parsing CSV File")
                 logger.debug("", exc_info=True)
+                logger.debug(str(e))
                 exit(1)
         else:
             logger.error("Path to CSV file incorrect.")
             exit(1)
         db.set_index(
             ["CHROM", "POS", "REF", "ALT", "GENE_NAME", "HGVS.C", "HGVS.P"],
             inplace=True,
@@ -67,15 +74,15 @@
         db = db.pipe(VariantsDB)
         return db
 
     @classmethod
     def buildDB(cls):
         def patientLister(db=None):
             vcfspath = []
-            for dirpath, dirnames, filenames in os.walk(patientPath):
+            for dirpath, dirnames, filenames in os.walk(configuration.patientPath):
                 for filename in [
                     f for f in filenames if f.lower().endswith("final.vcf")
                 ]:
                     vcfspath.append(os.path.join(dirpath, filename))
             final_list = []
             for idx in range(len(vcfspath)):
                 splitfn = vcfspath[idx].rsplit("/", maxsplit=1)[-1]
@@ -87,30 +94,42 @@
                         any(
                             splitfn.strip(".final.vcf") in string
                             for string in final_list
                         )
                     ):
                         final_list.append(vcfspath[idx])
             for x in final_list:
-                fn = x.rsplit("/",maxsplit=1)[-1]
-                if any(fn.strip(".final.vcf")+"_MODApy.final.vcf" in string for string in final_list):
+                fn = x.rsplit("/", maxsplit=1)[-1]
+                if any(
+                    fn.strip(".final.vcf") + "_MODApy.final.vcf" in string
+                    for string in final_list
+                ):
                     final_list.remove(x)
             vcfspath = final_list
             try:
                 vcfsnames = [cyvcf2.Reader(x).samples[0] for x in vcfspath]
-            except:
+            except Exception as e:
                 logger.info(
                     "No Sample name in one of the vcfs files. Using File Names Instead"
                 )
+                logger.debug(str(e))
                 vcfsnames = [
                     x.rsplit("/", maxsplit=1)[-1].strip(".final.vcf") for x in vcfspath
                 ]
 
             if db is not None:
-                addpatnames = [x for x in vcfsnames if x not in db.columns]
+                addpatnames = [
+                    x
+                    for x in vcfsnames
+                    if (
+                        x not in db.columns
+                        and x + "_MODApy" not in db.columns
+                        and x.replace("_MODApy", "") not in db.columns
+                    )
+                ]
                 if len(addpatnames) >= 1:
                     logger.info("Adding Patients: {}".format([x for x in addpatnames]))
                 else:
                     logger.error("No Patients to Add")
                     exit(1)
                 patientslist = [x for x in vcfspath for y in addpatnames if y in x]
             else:
@@ -148,15 +167,23 @@
             if db is not None:
                 db.drop(columns=["level_0", "index"], errors="ignore", inplace=True)
                 db = db.reset_index()
                 pvcfs.insert(0, db)
                 db.drop(columns=["level_0", "index"], inplace=True, errors="ignore")
             pvcfs = [
                 x.set_index(
-                    ["CHROM", "POS", "REF", "ALT", "GENE_NAME", "HGVS.C", "HGVS.P"]
+                    [
+                        "CHROM",
+                        "POS",
+                        "REF",
+                        "ALT",
+                        "GENE_NAME",
+                        "HGVS.C",
+                        "HGVS.P",
+                    ]
                 )
                 for x in pvcfs
             ]
             tempdb1 = pd.concat(pvcfs, axis=1, join="outer")
             tempdb1 = (
                 tempdb1.reset_index()
                 .groupby(["CHROM", "POS", "REF", "ALT"])
@@ -180,42 +207,50 @@
             del pvcfs
             colslist = ["GENE_NAME", "HGVS.C", "HGVS.P"]
             for col in colslist:
                 db[col] = db[col].apply(lambda x: " | ".join(set(x.split(" | "))))
             db = db.reset_index().set_index(
                 ["CHROM", "POS", "REF", "ALT", "GENE_NAME", "HGVS.C", "HGVS.P"]
             )
-            db.drop(columns=["index", "0", "level_0"], inplace=True, errors="ignore")
+            db.drop(
+                columns=["index", "0", "level_0"],
+                inplace=True,
+                errors="ignore",
+            )
             db.replace({".": np.nan}, inplace=True)
             db = db.pipe(VariantsDB)
             db = db.calcfreqs()
             return db
 
         try:
             logger.info("Checking DB File")
-            if variantsDBPath.rsplit(".")[-1].lower() == "xlsx":
-                db = VariantsDB.from_exceldb(variantsDBPath.rsplit("/", maxsplit=1)[0])
+            if configuration.variantsDBPath.rsplit(".")[-1].lower() == "xlsx":
+                db = VariantsDB.from_exceldb(
+                    configuration.variantsDBPath.rsplit("/", maxsplit=1)[0]
+                )
                 patientslist = patientLister(db)
-            elif variantsDBPath.rsplit(".")[-1].lower() == "csv":
-                db = VariantsDB.from_csvdb(variantsDBPath.rsplit("/", maxsplit=1)[0])
+            elif configuration.variantsDBPath.rsplit(".")[-1].lower() == "csv":
+                db = VariantsDB.from_csvdb(
+                    configuration.variantsDBPath.rsplit("/", maxsplit=1)[0]
+                )
                 patientslist = patientLister(db)
             else:
-                logger.error("VariantsDBPath must be a xlsx or csv file")
+                logger.error("configuration.variantsDBPath must be a xlsx or csv file")
                 exit(1)
-        except:
+        except Exception as e:
+            logger.debug(str(e))
             exit()
-            logger.info("No DB Found, Building new Variants DB")
-            patientslist = patientLister()
-            db = None
         sublists = [
-            patientslist[i : i + int(cfg["GENERAL"]["cores"])]
-            for i in range(0, len(patientslist), int(cfg["GENERAL"]["cores"]))
+            patientslist[i : i + int(configuration.cfg["GENERAL"]["cores"])]
+            for i in range(
+                0, len(patientslist), int(configuration.cfg["GENERAL"]["cores"])
+            )
         ]
-        for l in sublists:
-            db = dbbuilder(l, db)
+        for lista in sublists:
+            db = dbbuilder(lista, db)
             db.to_VarDBCSV()
         return db
 
     def addPatientToDB(self, patient):
         if patient.rsplit("/")[-1].strip(".final.vcf") in self.columns:
             logger.error("Patient already is in DB")
             exit(1)
@@ -224,15 +259,24 @@
         elif isinstance(patient, ParsedVCF):
             pvcf = patient
         else:
             logger.error("Patient must be either a path to vcf or a ParsedVCF object")
             logger.debug("", exc_info=True)
             exit(1)
         pvcf = pvcf[
-            ["CHROM", "POS", "REF", "ALT", "ZIGOSITY", "GENE_NAME", "HGVS.C", "HGVS.P"]
+            [
+                "CHROM",
+                "POS",
+                "REF",
+                "ALT",
+                "ZIGOSITY",
+                "GENE_NAME",
+                "HGVS.C",
+                "HGVS.P",
+            ]
         ]
         if "ZIGOSITY" not in pvcf.columns:
             pvcf["ZIGOSITY"] = "UNKWN"
         pvcf.rename(columns={"ZIGOSITY": pvcf.name}, inplace=True)
         pvcf.set_index(
             ["CHROM", "POS", "REF", "ALT", "GENE_NAME", "HGVS.C", "HGVS.P"],
             inplace=True,
@@ -243,17 +287,19 @@
         return db
 
     def to_VarDBXLS(self):
         logger.info("Writing DB to Excel")
         self.reset_index(inplace=True)
         self["POS"] = self["POS"].astype(int)
         self.sort_values(["CHROM", "POS"], inplace=True)
-        os.makedirs(variantsDBPath.rsplit("/", maxsplit=1)[0], exist_ok=True)
-        vdbpath = variantsDBPath.rsplit(".", maxsplit=1)[0]
-        output = pd.ExcelWriter(variantsDBPath)
+        os.makedirs(
+            configuration.variantsDBPath.rsplit("/", maxsplit=1)[0], exist_ok=True
+        )
+        vdbpath = configuration.variantsDBPath.rsplit(".", maxsplit=1)[0]
+        output = pd.ExcelWriter(configuration.variantsDBPath)
         workbook = output.book
         datasheet = workbook.add_worksheet("VariantSDB")
         output.sheets["VariantsDB"] = datasheet
         formatpos = workbook.add_format({"num_format": "###,###,###"})
         self["POS"] = self["POS"].astype(int)
         datasheet.set_column("B:B", 15, formatpos)
         for chrom in self["CHROM"].unique():
@@ -267,16 +313,18 @@
         logger.info("Xlsx DB construction complete")
 
     def to_VarDBCSV(self):
         logger.info("Writing DB to CSV")
         self.reset_index(inplace=True)
         self["POS"] = self["POS"].astype(int)
         self.sort_values(["CHROM", "POS"], inplace=True)
-        vdbpath = variantsDBPath.rsplit(".", maxsplit=1)[0]
-        os.makedirs(variantsDBPath.rsplit("/", maxsplit=1)[0], exist_ok=True)
+        vdbpath = configuration.variantsDBPath.rsplit(".", maxsplit=1)[0]
+        os.makedirs(
+            configuration.variantsDBPath.rsplit("/", maxsplit=1)[0], exist_ok=True
+        )
         for chrom in self["CHROM"].unique():
             self[self["CHROM"] == chrom].to_csv(
                 vdbpath + str(chrom) + ".csv", index=False, float_format="%.5f"
             )
         logger.info("DB construction complete")
 
     def calcfreqs(self):
@@ -297,39 +345,42 @@
         cols.remove("FREQ")
         cols.remove("ALLELE_FREQ")
         self = self[["ALLELE_FREQ", "FREQ"] + cols]
         self.replace({np.nan: "."}, inplace=True)
         self.pipe(VariantsDB)
         return self
 
-    def annotate_excel(self, df, fileName):
+    def annotate_excel(self, df, fileName, annotate_patients=True):
         logger.info("Annotating Excel file")
         cols_to_drop = ["FREQ", "ALLELE_FREQ", "VARDB_FREQ"]
         df.drop(columns=[x for x in cols_to_drop if x in df.columns], inplace=True)
         df = df.merge(
             self.reset_index()[["CHROM", "POS", "REF", "ALT", "FREQ", "ALLELE_FREQ"]],
             on=["CHROM", "POS", "REF", "ALT"],
             how="left",
         )
         df.rename(columns={"FREQ": "VARDB_FREQ"}, inplace=True)
         df["VARDB_FREQ"] = pd.to_numeric(df["VARDB_FREQ"], errors="coerce")
         df["VARDB_FREQ"].round(6)
         if "_MODApy" in fileName:
-            foldername = fileName.split("_MODApy")[0]
+            foldername = fileName.split("_MODApy")[0] + "_MODApy"
         elif "_" in fileName:
             foldername = fileName.split("_")[0]
         else:
             foldername = fileName.split(".")[0]
         outpath = (
-            patientPath
+            configuration.patientPath
             + foldername
             + "/"
             + fileName.rsplit(".", maxsplit=1)[0].replace(".annotated", "")
             + ".annotated.xlsx"
         )
+        if annotate_patients is True:
+            patdf = self.annotate_patients_with_variants(df)
+            df = df.merge(patdf, on=["CHROM", "POS", "REF", "ALT"], how="left")
         firstcols = [
             "GENE_NAME",
             "AMINOCHANGE",
             "HGVS.P",
             "HGVS.C",
             "RSID",
             "IMPACT",
@@ -353,15 +404,17 @@
         datasheet.set_column(
             df.columns.to_list().index("POS"),
             df.columns.to_list().index("POS"),
             15,
             formatpos,
         )
         datasheet.set_column(
-            df.columns.to_list().index("RSID"), df.columns.to_list().index("RSID"), 15
+            df.columns.to_list().index("RSID"),
+            df.columns.to_list().index("RSID"),
+            15,
         )
         # Light red fill with dark red text.
         highformat = workbook.add_format(
             {"bg_color": "#FFC7CE", "font_color": "#9C0006", "bold": True}
         )
         # Light yellow fill with dark yellow text.
         modformat = workbook.add_format(
@@ -421,33 +474,37 @@
                 "criteria": "containing",
                 "value": "LOW",
                 "format": lowformat,
             },
         )
         logger.info("Writing Excel File")
         df[firstcols + lastcols].to_excel(
-            output, sheet_name="DATA", merge_cells=False, index=False, header=True
+            output,
+            sheet_name="DATA",
+            merge_cells=False,
+            index=False,
+            header=True,
         )
 
         if df.reset_index().index.max() < 32150:
             logger.info("Redirecting IDs and GENEs to URLs")
             try:
                 colid = df.columns.to_list().index("RSID")
                 colgen = df.columns.to_list().index("GENE_NAME")
                 row = 2
                 for x in zip(df["RSID"], df["GENE_NAME"]):
-                    if type(x[0]) == str:
+                    if isinstance(x[0], str):
                         urlrs = "https://varsome.com/variant/hg19/%s"
                         rsvalue = (x[0].replace(";", ",").split(","))[0]
                         datasheet.write_url(
                             "%s%i" % (chr(colid + 65), (row)),
                             urlrs % rsvalue,
                             string=rsvalue,
                         )
-                    if type(x[1]) == str:
+                    if isinstance(x[1], str):
                         urlgen = "https://www.ncbi.nlm.nih.gov/omim/?term=%s"
                         datasheet.write_url(
                             "%s%i" % (chr(colgen + 65), (row)),
                             urlgen % x[1],
                             string=x[1],
                         )
                     row += 1
@@ -456,30 +513,81 @@
         stats = ParsedVCF.general_stats(df)
         stats.to_excel(output, sheet_name="STATISTICS")
         output.sheets["STATISTICS"] = statsheet
         try:
             stats.to_excel(output, sheet_name="STATISTICS")
         except Exception as e:
             logger.error(
-                "Could not print statistics. Error was {}".format(e), exc_info=True
+                "Could not print statistics. Error was {}".format(e),
+                exc_info=True,
             )
         try:
             statsheet.insert_image("H2", "./general.png")
         except Exception as e:
             logger.error(
-                "Could not print stats graphs. Error was {}".format(e), exc_info=True
+                "Could not print stats graphs. Error was {}".format(e),
+                exc_info=True,
             )
         if os.path.isfile("./venn.png"):
             statsheet.insert_image("H25", "./venn.png")
         output.save()
         try:
             os.remove("./general.png")
-        except:
+        except Exception as e:
             logger.debug("Could not remove general.png")
+            logger.debug(str(e))
         try:
             os.remove("./venn.png")
-        except:
+        except Exception as e:
             logger.debug("Could not remove venn.png")
+            logger.debug(str(e))
         datasheet.autofilter(0, 0, len(self), len(df.columns))
         output.save()
         logger.info("File saved to %s" % outpath)
         return outpath
+
+    def annotate_patients_with_variants(self, paneldf, columns=None):
+        if columns is None:
+            columns = ['CHROM', 'POS', 'REF', 'ALT']
+        logger.info("Annotating Patients with Variants")
+        patsdf = paneldf[columns].merge(
+            self.reset_index().drop(columns=['FREQ', 'ALLELE_FREQ']),
+            on=["CHROM", "POS", "REF", "ALT"],
+            how="left",
+        )
+        patsdf.drop(columns='index', inplace=True)
+        patsdf['PATS_WITH_VARIANTS'] = pd.Series(
+            list(
+                np.where(
+                    ~patsdf.drop(
+                        columns=[
+                            'CHROM',
+                            'POS',
+                            'REF',
+                            'ALT',
+                            'HGVS.C',
+                            'HGVS.P',
+                            'GENE_NAME',
+                        ]
+                    ).eq('.'),
+                    patsdf.drop(
+                        columns=[
+                            'CHROM',
+                            'POS',
+                            'REF',
+                            'ALT',
+                            'HGVS.C',
+                            'HGVS.P',
+                            'GENE_NAME',
+                        ]
+                    ).columns,
+                    'to_delete',
+                )
+            )
+        )
+        patsdf['PATS_WITH_VARIANTS'] = patsdf['PATS_WITH_VARIANTS'].apply(
+            lambda x: x.tolist()
+        )
+        patsdf['PATS_WITH_VARIANTS'] = patsdf['PATS_WITH_VARIANTS'].apply(
+            lambda row: [pat for pat in row if pat != 'to_delete']
+        )
+        return patsdf[columns + ['PATS_WITH_VARIANTS']]
```

### Comparing `MODApy-0.7.8/MODApy/vcfanalysis.py` & `MODApy-0.8.0/MODApy/vcfanalysis.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import logging
+import os
 
-from MODApy import vcfmgr, cfg
+from MODApy import configuration, vcfmgr
 from MODApy.utils import checkFile
-import os
+
 
 logger = logging.getLogger()
 
 
 def single(patient, panel):
     try:
         checkFile(patient, ".vcf")
         checkFile(panel, ".xlsx")
         logger.info("Running %s on patient %s" % (str(panel), str(patient)))
         result = vcfmgr.ParsedVCF.from_vcf(patient).panel(panel)
         outpath = (
-            cfg.patientPath
+            configuration.patientPath
             + result.name
             + "/Panels/"
             + result.name
             + "_"
             + panel
             + ".xlsx"
         )
@@ -26,27 +27,27 @@
         result.vcf_to_excel(outpath)
         logger.info("Single Analisis Complete")
         logger.info("File available at:%s" % outpath)
         return outpath
     except Exception as err:
         logger.error("Single analysis Failed")
         logger.debug(f"Error was: {err}", exc_info=True)
-        raise Exception
+        raise RuntimeError("Single analysis Failed")
 
 
-def duos(patient1, patient2, VennPlace=None, Panel=None, Filter=None):
+def duos(patient1, patient2, VennPlace=None, Panel=None, Filter=[None]):
     try:
         checkFile(patient1, ".vcf")
         checkFile(patient2, ".vcf")
         logger.info("Running Duos Study on %s and %s" % (str(patient1), str(patient2)))
         pvcfs = vcfmgr.ParsedVCF.mp_parser(patient1, patient2)
         result = pvcfs[0].duos(pvcfs[1], VENNPLACE=VennPlace)
         resultname = result.name
         outpath = (
-            cfg.resultsPath
+            configuration.resultsPath
             + "Duos/"
             + result.name.replace(":", "_")
             + "/"
             + result.name.replace(":", "_")
         )
         result.name = resultname
         if VennPlace is not None:
@@ -75,34 +76,35 @@
                 result.name = resultname
                 outpath = outpath + "_F" + str(x[0]) + str(x[1])
         outpath = outpath + ".xlsx"
         logger.info("Writing Result File")
         result.vcf_to_excel(outpath)
         logger.info("Duos Analisis Complete")
         logger.info("File available at:%s" % outpath)
+        return outpath
     except Exception as err:
         logger.error("Duos Analisis Failed")
         logger.debug(f"Error was: {err}", exc_info=True)
-        raise Exception
+        raise RuntimeError("Duos Analisis Failed")
 
 
-def trios(patient1, patient2, patient3, VennPlace=None, Filter=None, Panel=None):
+def trios(patient1, patient2, patient3, VennPlace=None, Filter=[None], Panel=None):
     try:
         checkFile(patient1, ".vcf")
         checkFile(patient2, ".vcf")
         checkFile(patient3, ".vcf")
         logger.info(
             "Running Trios Study on %s, %s and %s"
             % (str(patient1), str(patient2), str(patient3))
         )
         pvcfs = vcfmgr.ParsedVCF.mp_parser(patient1, patient2, patient3)
         result = pvcfs[0].duos(pvcfs[1]).duos(pvcfs[2], VENNPLACE=VennPlace)
         resultname = result.name
         outpath = (
-            cfg.resultsPath
+            configuration.resultsPath
             + "Trios/"
             + result.name.replace(":", "_")
             + "/"
             + result.name.replace(":", "_")
         )
         result.name = resultname
         if VennPlace is not None:
@@ -132,11 +134,12 @@
                         result = result[~result[x[0]].str.contains(x[1])]
                     result.name = resultname
                     outpath = outpath + "_Filter" + str(x[0]) + str(x[1])
         outpath = outpath + ".xlsx"
         result.vcf_to_excel(outpath)
         logger.info("Trios Analisis Complete")
         logger.info("File available at:%s" % outpath)
+        return outpath
     except Exception as err:
         logger.error("Trios Analisis Failed")
         logger.debug(f"Error was: {err}", exc_info=True)
-        raise Exception
+        raise RuntimeError("Trios Analisis Failed")
```

### Comparing `MODApy-0.7.8/MODApy/www/wespipelinebam.png` & `MODApy-0.8.0/MODApy/www/wespipelinebam.png`

 * *Files identical despite different names*

### Comparing `MODApy-0.7.8/MODApy/www/wespipelinefull.png` & `MODApy-0.8.0/MODApy/www/wespipelinefull.png`

 * *Files identical despite different names*

### Comparing `MODApy-0.7.8/MODApy/www/wespipelinevcf.png` & `MODApy-0.8.0/MODApy/www/wespipelinevcf.png`

 * *Files identical despite different names*

### Comparing `MODApy-0.7.8/MODApy.egg-info/PKG-INFO` & `MODApy-0.8.0/MODApy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MODApy
-Version: 0.7.8
+Version: 0.8.0
 Summary: Package to perform several analysis on Multi-Omics Data
 Home-page: https://github.com/juancgvazquez/MODApy
 Author: Juan Carlos Vázquez, Elmer A. Fernández
 Author-email: juancgvazquez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `MODApy-0.7.8/MODApy.egg-info/SOURCES.txt` & `MODApy-0.8.0/MODApy.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
 MODApy/__init__.py
 MODApy/cfg.py
 MODApy/cmd_line.py
 MODApy/coverage.py
 MODApy/downloader.py
 MODApy/modaapi.py
+MODApy/parquetvardb.py
 MODApy/pipeline.py
 MODApy/utils.py
 MODApy/variantsdb.py
 MODApy/vcfanalysis.py
 MODApy/vcfmgr.py
 MODApy/version.py
 MODApy.egg-info/PKG-INFO
```

### Comparing `MODApy-0.7.8/PKG-INFO` & `MODApy-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MODApy
-Version: 0.7.8
+Version: 0.8.0
 Summary: Package to perform several analysis on Multi-Omics Data
 Home-page: https://github.com/juancgvazquez/MODApy
 Author: Juan Carlos Vázquez, Elmer A. Fernández
 Author-email: juancgvazquez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `MODApy-0.7.8/README.md` & `MODApy-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `MODApy-0.7.8/setup.py` & `MODApy-0.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     description="Package to perform several analysis on Multi-Omics Data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/juancgvazquez/MODApy",
     packages=setuptools.find_packages(),
     package_data={"MODApy": ["www/*"]},
     install_requires=[
-        "pandas>=1.3.0",
+        "pandas>=1.3.0,<2.0.0",
         "numpy",
         "configparser",
         "argparse",
         "Cython",
         "cyvcf2==0.9.0",
         "xlrd",
         "openpyxl",
```

