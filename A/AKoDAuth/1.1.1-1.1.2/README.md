# Comparing `tmp/AKoDAuth-1.1.1.tar.gz` & `tmp/AKoDAuth-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AKoDAuth-1.1.1.tar", last modified: Sat Mar 23 18:40:28 2024, max compression
+gzip compressed data, was "AKoDAuth-1.1.2.tar", last modified: Sun Apr 14 04:24:22 2024, max compression
```

## Comparing `AKoDAuth-1.1.1.tar` & `AKoDAuth-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-23 18:40:28.785694 AKoDAuth-1.1.1/
-drwxrwxrwx   0        0        0        0 2024-03-23 18:40:28.772729 AKoDAuth-1.1.1/AKoDAuth/
--rw-rw-rw-   0        0        0     1710 2024-03-23 18:39:58.000000 AKoDAuth-1.1.1/AKoDAuth/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 18:40:28.784696 AKoDAuth-1.1.1/AKoDAuth.egg-info/
--rw-rw-rw-   0        0        0      281 2024-03-23 18:40:28.000000 AKoDAuth-1.1.1/AKoDAuth.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2024-03-23 18:40:28.000000 AKoDAuth-1.1.1/AKoDAuth.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-23 18:40:28.000000 AKoDAuth-1.1.1/AKoDAuth.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-03-23 18:40:28.000000 AKoDAuth-1.1.1/AKoDAuth.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-23 18:40:28.000000 AKoDAuth-1.1.1/AKoDAuth.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1080 2024-03-23 17:29:31.000000 AKoDAuth-1.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2024-03-20 01:03:08.000000 AKoDAuth-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      281 2024-03-23 18:40:28.784696 AKoDAuth-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1740 2024-03-23 18:34:20.000000 AKoDAuth-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-03-23 18:40:28.785694 AKoDAuth-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      336 2024-03-23 18:33:54.000000 AKoDAuth-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 04:24:22.008768 AKoDAuth-1.1.2/
+drwxrwxrwx   0        0        0        0 2024-04-14 04:24:22.000745 AKoDAuth-1.1.2/AKoDAuth/
+-rw-rw-rw-   0        0        0     2527 2024-04-14 04:23:05.000000 AKoDAuth-1.1.2/AKoDAuth/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 04:24:22.006249 AKoDAuth-1.1.2/AKoDAuth.egg-info/
+-rw-rw-rw-   0        0        0      227 2024-04-14 04:24:21.000000 AKoDAuth-1.1.2/AKoDAuth.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-04-14 04:24:21.000000 AKoDAuth-1.1.2/AKoDAuth.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 04:24:21.000000 AKoDAuth-1.1.2/AKoDAuth.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-14 04:24:21.000000 AKoDAuth-1.1.2/AKoDAuth.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-14 04:24:21.000000 AKoDAuth-1.1.2/AKoDAuth.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1080 2024-03-23 17:29:31.000000 AKoDAuth-1.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2024-03-20 01:03:08.000000 AKoDAuth-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      227 2024-04-14 04:24:22.008768 AKoDAuth-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1755 2024-03-25 04:45:00.000000 AKoDAuth-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-14 04:24:22.008768 AKoDAuth-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      336 2024-04-14 04:23:29.000000 AKoDAuth-1.1.2/setup.py
```

### Comparing `AKoDAuth-1.1.1/LICENSE.txt` & `AKoDAuth-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `AKoDAuth-1.1.1/README.md` & `AKoDAuth-1.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <div align="center">
     </a>
     <br />
     
    [tagoWorks](https://tago.works/) - [AKoD](https://github.com/tagoworks/akod)
    
 
-  Activating Keys on Discord Validating Package is coded to simplify the process of checking keys in your Python projects. Instead of taking up extra lines it handling decryption and key checking, AKoDAuth provides simple functions. You can use the validate function, passing in your email and key variables. AKoDAuth handles all the decryption and checking behind the scenes, allowing you to focus on your main code. For example, you can use `if akodauth.isValid(emailvar, licensekeyvar) == False:` to quickly check if a key is valid, without worrying about the details of the validation process. To use AKoDAuth in your code and key your software please visit https://github.com/t-a-g-o/vlod. View AKoDAuth's PyPi page at https://pypi.org/project/akodauth
+  Activating Keys on Discord Validating Package is coded to simplify the process of checking keys in your Python projects. Instead of taking up extra lines it handling decryption and key checking, AKoDAuth provides simple functions. You can use the validate function, passing in your email and key variables. AKoDAuth handles all the decryption and checking behind the scenes, allowing you to focus on your main code. For example, you can use `if akodauth.isValid(username, activationkey) == False:` to quickly check if a key is valid, without worrying about the details of the validation process. To use AKoDAuth in your code and key your software please visit https://github.com/t-a-g-o/vlod. View AKoDAuth's PyPi page at https://pypi.org/project/akodauth
 
 </div>
 
 # How to use AKoDAuth
 
 1. Install AKoDAuth
 
@@ -27,12 +27,13 @@
    * To set your private key use `AKoDAuth.privatekey('hehSUUXf3m33ns9Hwenj')`
    * To set your authentication webserver link use `AKoDAuth.publicserverkey('jweikAAAA-jemef-efj-_eneiebeufu_38h')`
 
 3. Implement a way to get user input for email and key
 
 4. Check if the account and key is valid using AKoDAuth.isValid()
    ```py
-   if AKoDAuth.isValid(usernamevar, keyvar) == False:
-      print("Invalid email or key")
+   if AKoDAuth.isValid(username, activationkey) == False:
+      print("Invalid user or key")
+      exit
    else:
       # Run your main code here
    ```
```

