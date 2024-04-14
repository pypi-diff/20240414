# Comparing `tmp/provisioner_runtime-0.1.5-py3-none-any.whl.zip` & `tmp/provisioner_runtime-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 131180 bytes, number of entries: 152
+Zip file size: 131179 bytes, number of entries: 152
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 external/ansible_playbooks/__init__.py
 -rwxr-xr-x  2.0 unx      368 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/apt_update_upgrade.yaml
 -rwxr-xr-x  2.0 unx     5549 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/common/shell_lib.sh
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/group_vars/all
 -rwxr-xr-x  2.0 unx      678 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/reboot.yaml
 -rwxr-xr-x  2.0 unx      353 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/roles/anchor/defaults/main.yaml
 -rwxr-xr-x  2.0 unx    10424 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/roles/anchor/files/anchor_run.sh
@@ -142,13 +142,13 @@
 -rwxr-xr-x  2.0 unx     8629 b- defN 80-Jan-01 00:00 provisioner/utils/prompter.py
 -rwxr-xr-x  2.0 unx     2400 b- defN 80-Jan-01 00:00 provisioner/utils/prompter_fakes.py
 -rwxr-xr-x  2.0 unx     2165 b- defN 80-Jan-01 00:00 provisioner/utils/properties.py
 -rwxr-xr-x  2.0 unx     1310 b- defN 80-Jan-01 00:00 provisioner/utils/properties_fakes.py
 -rwxr-xr-x  2.0 unx     2080 b- defN 80-Jan-01 00:00 provisioner/utils/summary.py
 -rwxr-xr-x  2.0 unx     1401 b- defN 80-Jan-01 00:00 provisioner/utils/summary_fakes.py
 -rwxr-xr-x  2.0 unx     2598 b- defN 80-Jan-01 00:00 provisioner/utils/yaml_util.py
--rw-r--r--  2.0 unx     1071 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx      792 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.5.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    15772 b- defN 16-Jan-01 00:00 provisioner_runtime-0.1.5.dist-info/RECORD
-152 files, 339229 bytes uncompressed, 105038 bytes compressed:  69.0%
+-rw-r--r--  2.0 unx     1071 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx      792 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.6.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    15772 b- defN 16-Jan-01 00:00 provisioner_runtime-0.1.6.dist-info/RECORD
+152 files, 339229 bytes uncompressed, 105037 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -435,23 +435,23 @@
 
 Filename: provisioner/utils/summary_fakes.py
 Comment: 
 
 Filename: provisioner/utils/yaml_util.py
 Comment: 
 
-Filename: provisioner_runtime-0.1.5.dist-info/LICENSE
+Filename: provisioner_runtime-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: provisioner_runtime-0.1.5.dist-info/METADATA
+Filename: provisioner_runtime-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: provisioner_runtime-0.1.5.dist-info/WHEEL
+Filename: provisioner_runtime-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: provisioner_runtime-0.1.5.dist-info/entry_points.txt
+Filename: provisioner_runtime-0.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: provisioner_runtime-0.1.5.dist-info/RECORD
+Filename: provisioner_runtime-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## provisioner/resources/version.txt

```diff
@@ -1 +1 @@
-0.1.5
+0.1.6
```

## Comparing `provisioner_runtime-0.1.5.dist-info/LICENSE` & `provisioner_runtime-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `provisioner_runtime-0.1.5.dist-info/METADATA` & `provisioner_runtime-0.1.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: provisioner-runtime
-Version: 0.1.5
+Version: 0.1.6
 Summary: Provision Everything Anywhere
 Author: Zachi Nachshon
 Author-email: zachi.nachshon@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

## Comparing `provisioner_runtime-0.1.5.dist-info/RECORD` & `provisioner_runtime-0.1.6.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 provisioner/infra/context.py,sha256=XKhLaNFaBxCCJrPKCH__cGDK2lzMRSl7OSjvfMT2b40,2452
 provisioner/infra/evaluator.py,sha256=kEukOBHkFgqD9_ntkXRuodfiU9sLgZ4d5mWsyeD02Is,2682
 provisioner/infra/log.py,sha256=61ST3qmrIf-CZUZtJVnKRgZp49vGeViQpUMp0nkVaqI,4102
 provisioner/infra/remote_context.py,sha256=U-7juzMelcFbuWzUfmgylMxrj88CczOo7vZ6fRyGlTQ,962
 provisioner/main.py,sha256=xLg-poqJ_0yRT_1TuABTGTDBgi9q6xwyKRpUIYZZ9PU,1668
 provisioner/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/resources/config.yaml,sha256=loN-e5Ptp7nKPssrjJ867g5RHppCYzwvVLfm5NoaVRE,26
-provisioner/resources/version.txt,sha256=QXCYE8RmYkHVrHvVrvCJYMkGMqpOawbNrZOJ4WODczY,5
+provisioner/resources/version.txt,sha256=Us6-ekrSteRiwlfY-S3rQlmDLCZyBEVABgGI-6YEsGQ,5
 provisioner/runner/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/runner/ansible/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/runner/ansible/ansible_fakes.py,sha256=1fIDJ4v8X2B7BBfmo_Ge6_If6mTaNEPOE-Mrz7066rQ,1228
 provisioner/runner/ansible/ansible_runner.py,sha256=eMOczcQPhp9flK481wyq0eMBAfGLdKhPkOew9CXgPgw,16182
 provisioner/runner/ansible/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/runner/ansible/resources/ansible.cfg,sha256=SXL8xHPL8xT-g-DbOzqUlQzYRKEyHU6UfVGVE4ApCjo,1957
 provisioner/runner/ansible/resources/callback_plugins/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -141,12 +141,12 @@
 provisioner/utils/prompter.py,sha256=RWhDat_577wsM1die636ctuuhNB1-dZWJqlA9bobLJw,8629
 provisioner/utils/prompter_fakes.py,sha256=qqB7pikYvh8RIoArDFq1JYC1PaBdLleQFwC_Gp_ZbSY,2400
 provisioner/utils/properties.py,sha256=pPAV_NFRCfNvy6G87p_a2JpC7P5VRlviEFgORIiucBg,2165
 provisioner/utils/properties_fakes.py,sha256=1fsOQu9FTA12H2XH4I4Wn_H9Bg8hZqYVco-wn-pOHuk,1310
 provisioner/utils/summary.py,sha256=U9dYFFJe_Nodw-1y52K650HOO2d35IVQoCZNU8qPUD4,2080
 provisioner/utils/summary_fakes.py,sha256=YMm6sBiNw5MGCO-ILwnPx0u715_-vJOnyno1czLkeNM,1401
 provisioner/utils/yaml_util.py,sha256=-i1hIyh05hhJYa8bJBjreMfEaZdNkheU6zSvnhgVe-Y,2598
-provisioner_runtime-0.1.5.dist-info/LICENSE,sha256=rcr78KAutoVDcl3EaX33JjBsvfatzmlKWJ0-Ji3I7tk,1071
-provisioner_runtime-0.1.5.dist-info/METADATA,sha256=0u1-2jiHNjO9to1dYE4VcBoxuhanucO5wfVyhRB8hnU,792
-provisioner_runtime-0.1.5.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-provisioner_runtime-0.1.5.dist-info/entry_points.txt,sha256=YyXkOvQA01nCNiVumyuvhjPWhndn3ZwrvVGFQQ6O74k,53
-provisioner_runtime-0.1.5.dist-info/RECORD,,
+provisioner_runtime-0.1.6.dist-info/LICENSE,sha256=rcr78KAutoVDcl3EaX33JjBsvfatzmlKWJ0-Ji3I7tk,1071
+provisioner_runtime-0.1.6.dist-info/METADATA,sha256=qc4319Iaslab8GxOma0SNeLxZdpyG7-WEBNnBT_sK1Y,792
+provisioner_runtime-0.1.6.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+provisioner_runtime-0.1.6.dist-info/entry_points.txt,sha256=YyXkOvQA01nCNiVumyuvhjPWhndn3ZwrvVGFQQ6O74k,53
+provisioner_runtime-0.1.6.dist-info/RECORD,,
```

