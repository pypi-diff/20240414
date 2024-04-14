# Comparing `tmp/ansible_later-4.0.2.tar.gz` & `tmp/ansible_later-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_later-4.0.2.tar", max compression
+gzip compressed data, was "ansible_later-4.0.3.tar", max compression
```

## Comparing `ansible_later-4.0.2.tar` & `ansible_later-4.0.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1123 2024-03-02 13:54:41.863655 ansible_later-4.0.2/LICENSE
--rw-r--r--   0        0        0     2749 2024-03-02 13:54:41.863655 ansible_later-4.0.2/README.md
--rw-r--r--   0        0        0      120 2024-03-02 13:54:57.191169 ansible_later-4.0.2/ansiblelater/__init__.py
--rwxr-xr-x   0        0        0     2844 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/__main__.py
--rw-r--r--   0        0        0     7580 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/candidate.py
--rw-r--r--   0        0        0      666 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/exceptions.py
--rw-r--r--   0        0        0     5638 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/logger.py
--rw-r--r--   0        0        0    11809 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rule.py
--rw-r--r--   0        0        0      789 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckBecomeUser.py
--rw-r--r--   0        0        0     1599 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckBracesSpaces.py
--rw-r--r--   0        0        0     2527 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckChangedInWhen.py
--rw-r--r--   0        0        0     1081 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckCommandHasChanges.py
--rw-r--r--   0        0        0     2638 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckCommandInsteadOfArgument.py
--rw-r--r--   0        0        0     2043 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckCommandInsteadOfModule.py
--rw-r--r--   0        0        0     1186 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckCompareToEmptyString.py
--rw-r--r--   0        0        0     1189 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckCompareToLiteralBool.py
--rw-r--r--   0        0        0      915 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckDeprecated.py
--rw-r--r--   0        0        0     3785 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckDeprecatedBareVars.py
--rw-r--r--   0        0        0     4175 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckFQCNBuiltin.py
--rw-r--r--   0        0        0     3708 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckFilePermissionMissing.py
--rw-r--r--   0        0        0     3236 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckFilePermissionOctal.py
--rw-r--r--   0        0        0     1118 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckFilterSeparation.py
--rw-r--r--   0        0        0     1883 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckGitHasVersion.py
--rw-r--r--   0        0        0     1389 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckInstallUseLatest.py
--rw-r--r--   0        0        0     2530 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckKeyOrder.py
--rw-r--r--   0        0        0      903 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckLiteralBoolFormat.py
--rw-r--r--   0        0        0      697 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckLocalAction.py
--rw-r--r--   0        0        0     1144 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckMetaChangeFromDefault.py
--rw-r--r--   0        0        0     1159 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckMetaMain.py
--rw-r--r--   0        0        0      852 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckNameFormat.py
--rw-r--r--   0        0        0      859 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckNamedTask.py
--rw-r--r--   0        0        0     1644 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckNativeYaml.py
--rw-r--r--   0        0        0     2141 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckNestedJinja.py
--rw-r--r--   0        0        0     1197 2024-03-02 13:54:41.863655 ansible_later-4.0.2/ansiblelater/rules/CheckRelativeRolePaths.py
--rw-r--r--   0        0        0      768 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/rules/CheckScmInSrc.py
--rw-r--r--   0        0        0     1026 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/rules/CheckShellInsteadCommand.py
--rw-r--r--   0        0        0     1563 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/rules/CheckTaskSeparation.py
--rw-r--r--   0        0        0      864 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/rules/CheckUniqueNamedTask.py
--rw-r--r--   0        0        0      845 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/rules/CheckWhenFormat.py
--rw-r--r--   0        0        0      483 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/rules/CheckYamlColons.py
--rw-r--r--   0        0        0      494 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/rules/CheckYamlDocumentEnd.py
--rw-r--r--   0        0        0      502 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/rules/CheckYamlDocumentStart.py
--rw-r--r--   0        0        0      489 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/rules/CheckYamlEmptyLines.py
--rw-r--r--   0        0        0      649 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/rules/CheckYamlFile.py
--rw-r--r--   0        0        0      592 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/rules/CheckYamlHasContent.py
--rw-r--r--   0        0        0      486 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/rules/CheckYamlHyphens.py
--rw-r--r--   0        0        0      491 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/rules/CheckYamlIndent.py
--rw-r--r--   0        0        0      504 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/rules/CheckYamlOctalValues.py
--rw-r--r--   0        0        0     8046 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/settings.py
--rw-r--r--   0        0        0        0 2024-03-02 13:54:42.651616 ansible_later-4.0.2/ansiblelater/test/__init__.py
--rw-r--r--   0        0        0        0 2024-03-02 13:54:42.655616 ansible_later-4.0.2/ansiblelater/test/unit/__init__.py
--rw-r--r--   0        0        0     2337 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/test/unit/test_logger.py
--rw-r--r--   0        0        0      527 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/test/unit/test_settings.py
--rw-r--r--   0        0        0     3290 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/utils/__init__.py
--rw-r--r--   0        0        0    19946 2024-03-02 13:54:41.867655 ansible_later-4.0.2/ansiblelater/utils/yamlhelper.py
--rw-r--r--   0        0        0     3294 2024-03-02 13:54:57.191169 ansible_later-4.0.2/pyproject.toml
--rw-r--r--   0        0        0     4506 1970-01-01 00:00:00.000000 ansible_later-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1123 2024-04-14 09:47:16.651297 ansible_later-4.0.3/LICENSE
+-rw-r--r--   0        0        0     2749 2024-04-14 09:47:16.651297 ansible_later-4.0.3/README.md
+-rw-r--r--   0        0        0      120 2024-04-14 09:47:28.979625 ansible_later-4.0.3/ansiblelater/__init__.py
+-rwxr-xr-x   0        0        0     2844 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/__main__.py
+-rw-r--r--   0        0        0     7580 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/candidate.py
+-rw-r--r--   0        0        0      666 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/exceptions.py
+-rw-r--r--   0        0        0     5638 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/logger.py
+-rw-r--r--   0        0        0    11809 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rule.py
+-rw-r--r--   0        0        0      789 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckBecomeUser.py
+-rw-r--r--   0        0        0     1599 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckBracesSpaces.py
+-rw-r--r--   0        0        0     2527 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckChangedInWhen.py
+-rw-r--r--   0        0        0     1081 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckCommandHasChanges.py
+-rw-r--r--   0        0        0     2638 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckCommandInsteadOfArgument.py
+-rw-r--r--   0        0        0     2043 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckCommandInsteadOfModule.py
+-rw-r--r--   0        0        0     1186 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckCompareToEmptyString.py
+-rw-r--r--   0        0        0     1189 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckCompareToLiteralBool.py
+-rw-r--r--   0        0        0      915 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckDeprecated.py
+-rw-r--r--   0        0        0     3785 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckDeprecatedBareVars.py
+-rw-r--r--   0        0        0     4175 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckFQCNBuiltin.py
+-rw-r--r--   0        0        0     3708 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckFilePermissionMissing.py
+-rw-r--r--   0        0        0     3236 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckFilePermissionOctal.py
+-rw-r--r--   0        0        0     1118 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckFilterSeparation.py
+-rw-r--r--   0        0        0     1883 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckGitHasVersion.py
+-rw-r--r--   0        0        0     1389 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckInstallUseLatest.py
+-rw-r--r--   0        0        0     2530 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckKeyOrder.py
+-rw-r--r--   0        0        0      903 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckLiteralBoolFormat.py
+-rw-r--r--   0        0        0      697 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckLocalAction.py
+-rw-r--r--   0        0        0     1144 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckMetaChangeFromDefault.py
+-rw-r--r--   0        0        0     1159 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckMetaMain.py
+-rw-r--r--   0        0        0      852 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckNameFormat.py
+-rw-r--r--   0        0        0      859 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckNamedTask.py
+-rw-r--r--   0        0        0     1644 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckNativeYaml.py
+-rw-r--r--   0        0        0     2141 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckNestedJinja.py
+-rw-r--r--   0        0        0     1197 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckRelativeRolePaths.py
+-rw-r--r--   0        0        0      768 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckScmInSrc.py
+-rw-r--r--   0        0        0     1026 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckShellInsteadCommand.py
+-rw-r--r--   0        0        0     1563 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckTaskSeparation.py
+-rw-r--r--   0        0        0      864 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckUniqueNamedTask.py
+-rw-r--r--   0        0        0      845 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckWhenFormat.py
+-rw-r--r--   0        0        0      483 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckYamlColons.py
+-rw-r--r--   0        0        0      494 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckYamlDocumentEnd.py
+-rw-r--r--   0        0        0      502 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckYamlDocumentStart.py
+-rw-r--r--   0        0        0      489 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckYamlEmptyLines.py
+-rw-r--r--   0        0        0      649 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckYamlFile.py
+-rw-r--r--   0        0        0      592 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckYamlHasContent.py
+-rw-r--r--   0        0        0      486 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckYamlHyphens.py
+-rw-r--r--   0        0        0      491 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckYamlIndent.py
+-rw-r--r--   0        0        0      504 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/rules/CheckYamlOctalValues.py
+-rw-r--r--   0        0        0     8046 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/settings.py
+-rw-r--r--   0        0        0        0 2024-04-14 09:47:17.475322 ansible_later-4.0.3/ansiblelater/test/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 09:47:17.475322 ansible_later-4.0.3/ansiblelater/test/unit/__init__.py
+-rw-r--r--   0        0        0     2337 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/test/unit/test_logger.py
+-rw-r--r--   0        0        0      527 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/test/unit/test_settings.py
+-rw-r--r--   0        0        0     3290 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/utils/__init__.py
+-rw-r--r--   0        0        0    19946 2024-04-14 09:47:16.651297 ansible_later-4.0.3/ansiblelater/utils/yamlhelper.py
+-rw-r--r--   0        0        0     3294 2024-04-14 09:47:28.979625 ansible_later-4.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4506 1970-01-01 00:00:00.000000 ansible_later-4.0.3/PKG-INFO
```

### Comparing `ansible_later-4.0.2/LICENSE` & `ansible_later-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/README.md` & `ansible_later-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/__main__.py` & `ansible_later-4.0.3/ansiblelater/__main__.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/candidate.py` & `ansible_later-4.0.3/ansiblelater/candidate.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/exceptions.py` & `ansible_later-4.0.3/ansiblelater/exceptions.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/logger.py` & `ansible_later-4.0.3/ansiblelater/logger.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rule.py` & `ansible_later-4.0.3/ansiblelater/rule.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckBecomeUser.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckBecomeUser.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckBracesSpaces.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckBracesSpaces.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckChangedInWhen.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckChangedInWhen.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckCommandHasChanges.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckCommandHasChanges.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckCommandInsteadOfArgument.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckCommandInsteadOfArgument.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckCommandInsteadOfModule.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckCommandInsteadOfModule.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckCompareToEmptyString.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckCompareToEmptyString.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckCompareToLiteralBool.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckCompareToLiteralBool.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckDeprecated.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckDeprecated.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckDeprecatedBareVars.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckDeprecatedBareVars.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckFQCNBuiltin.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckFQCNBuiltin.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckFilePermissionMissing.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckFilePermissionMissing.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckFilePermissionOctal.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckFilePermissionOctal.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckFilterSeparation.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckFilterSeparation.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckGitHasVersion.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckGitHasVersion.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckInstallUseLatest.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckInstallUseLatest.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckKeyOrder.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckKeyOrder.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckLiteralBoolFormat.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckLiteralBoolFormat.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckLocalAction.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckLocalAction.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckMetaChangeFromDefault.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckMetaChangeFromDefault.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckMetaMain.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckMetaMain.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckNameFormat.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckNameFormat.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckNamedTask.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckNamedTask.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckNativeYaml.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckNativeYaml.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckNestedJinja.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckNestedJinja.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckRelativeRolePaths.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckRelativeRolePaths.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckScmInSrc.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckScmInSrc.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckShellInsteadCommand.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckShellInsteadCommand.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckTaskSeparation.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckTaskSeparation.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckUniqueNamedTask.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckUniqueNamedTask.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckWhenFormat.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckWhenFormat.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckYamlFile.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckYamlFile.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/rules/CheckYamlHasContent.py` & `ansible_later-4.0.3/ansiblelater/rules/CheckYamlHasContent.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/settings.py` & `ansible_later-4.0.3/ansiblelater/settings.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/test/unit/test_logger.py` & `ansible_later-4.0.3/ansiblelater/test/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/test/unit/test_settings.py` & `ansible_later-4.0.3/ansiblelater/test/unit/test_settings.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/utils/__init__.py` & `ansible_later-4.0.3/ansiblelater/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/ansiblelater/utils/yamlhelper.py` & `ansible_later-4.0.3/ansiblelater/utils/yamlhelper.py`

 * *Files identical despite different names*

### Comparing `ansible_later-4.0.2/pyproject.toml` & `ansible_later-4.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 include = ["LICENSE"]
 keywords = ["ansible", "code", "review"]
 license = "MIT"
 name = "ansible-later"
 packages = [{ include = "ansiblelater" }]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/ansible-later/"
-version = "4.0.2"
+version = "4.0.3"
 
 [tool.poetry.dependencies]
 PyYAML = "6.0.1"
-ansible-core = { version = "2.14.14", optional = true }
+ansible-core = { version = "2.14.15", optional = true }
 ansible = { version = "7.7.0", optional = true }
 anyconfig = "0.14.0"
 appdirs = "1.4.4"
 colorama = "0.4.6"
 jsonschema = "4.21.1"
 nested-lookup = "0.2.25"
 pathspec = "0.12.1"
@@ -49,18 +49,18 @@
 ansible = ["ansible"]
 ansible-core = ["ansible-core"]
 
 [tool.poetry.scripts]
 ansible-later = "ansiblelater.__main__:main"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "0.2.2"
-pytest = "8.0.2"
-pytest-mock = "3.12.0"
-pytest-cov = "4.1.0"
+ruff = "0.3.5"
+pytest = "8.1.1"
+pytest-mock = "3.14.0"
+pytest-cov = "5.0.0"
 toml = "0.10.2"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "semver"
 vcs = "git"
```

### Comparing `ansible_later-4.0.2/PKG-INFO` & `ansible_later-4.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-later
-Version: 4.0.2
+Version: 4.0.3
 Summary: Reviews ansible playbooks, roles and inventories and suggests improvements.
 Home-page: https://ansible-later.geekdocs.de/
 License: MIT
 Keywords: ansible,code,review
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.9.0,<4.0.0
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Provides-Extra: ansible
 Provides-Extra: ansible-core
 Requires-Dist: PyYAML (==6.0.1)
 Requires-Dist: ansible (==7.7.0) ; extra == "ansible"
-Requires-Dist: ansible-core (==2.14.14) ; extra == "ansible-core"
+Requires-Dist: ansible-core (==2.14.15) ; extra == "ansible-core"
 Requires-Dist: anyconfig (==0.14.0)
 Requires-Dist: appdirs (==1.4.4)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: jsonschema (==4.21.1)
 Requires-Dist: nested-lookup (==0.2.25)
 Requires-Dist: pathspec (==0.12.1)
 Requires-Dist: python-json-logger (==2.0.7)
```

