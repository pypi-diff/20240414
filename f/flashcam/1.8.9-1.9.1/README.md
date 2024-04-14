# Comparing `tmp/flashcam-1.8.9.tar.gz` & `tmp/flashcam-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashcam-1.8.9.tar", last modified: Tue Apr  2 12:30:20 2024, max compression
+gzip compressed data, was "flashcam-1.9.1.tar", last modified: Sun Apr 14 18:40:55 2024, max compression
```

## Comparing `flashcam-1.8.9.tar` & `flashcam-1.9.1.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:30:20.153960 flashcam-1.8.9/
--rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-02 12:30:20.153960 flashcam-1.8.9/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      901 2024-04-02 12:30:17.000000 flashcam-1.8.9/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:30:20.141960 flashcam-1.8.9/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    29232 2024-03-17 02:07:58.000000 flashcam-1.8.9/bin/flashcam
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-11-02 08:34:00.000000 flashcam-1.8.9/bin/flashcam_join
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3406 2023-11-02 08:34:00.000000 flashcam-1.8.9/bin/flashcam_org
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      865 2023-11-02 08:34:00.000000 flashcam-1.8.9/bin/flashcam_rep
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      679 2024-02-27 15:50:11.000000 flashcam-1.8.9/bin/flashcamg
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:30:20.145959 flashcam-1.8.9/flashcam/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5401 2024-03-11 10:00:57.000000 flashcam-1.8.9/flashcam/base_camera2.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8850 2024-03-08 14:33:40.000000 flashcam-1.8.9/flashcam/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:30:20.153960 flashcam-1.8.9/flashcam/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/BEAM_OFF.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/BEAM_ON_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/DET_NRDY.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/DET_RDY_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/digital-7.mono.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34360 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/digital-7.regular.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/monoskop.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     7865 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/pattern_acircles.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    22255 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/pattern_chessboard.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    12496 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/small_pixel.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/win_rain.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/win_skull.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/win_storm.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/win_winter.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/windows.jpg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/direct.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/izmq_receiver.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4635 2024-03-08 14:33:40.000000 flashcam-1.8.9/flashcam/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    50217 2024-04-02 12:28:54.000000 flashcam-1.8.9/flashcam/real_camera.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    43977 2024-04-02 04:35:37.000000 flashcam-1.8.9/flashcam/stream_enhancer.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)   114843 2024-03-22 13:59:53.000000 flashcam-1.8.9/flashcam/uniwrec.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13650 2024-04-02 12:14:08.000000 flashcam-1.8.9/flashcam/usbcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    36471 2023-11-02 08:59:16.000000 flashcam-1.8.9/flashcam/v4lc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2024-04-02 12:30:19.000000 flashcam-1.8.9/flashcam/version.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    40773 2024-04-02 12:27:03.000000 flashcam-1.8.9/flashcam/web.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:30:20.153960 flashcam-1.8.9/flashcam.egg-info/
--rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-02 12:30:19.000000 flashcam-1.8.9/flashcam.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      975 2024-04-02 12:30:20.000000 flashcam-1.8.9/flashcam.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-02 12:30:19.000000 flashcam-1.8.9/flashcam.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      165 2024-04-02 12:30:19.000000 flashcam-1.8.9/flashcam.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2024-04-02 12:30:19.000000 flashcam-1.8.9/flashcam.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-02 12:30:20.153960 flashcam-1.8.9/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2275 2023-11-02 08:34:00.000000 flashcam-1.8.9/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-14 18:40:55.015771 flashcam-1.9.1/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-14 18:40:55.015771 flashcam-1.9.1/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      901 2024-04-14 18:40:48.000000 flashcam-1.9.1/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-14 18:40:55.003771 flashcam-1.9.1/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    28426 2024-04-14 18:40:50.000000 flashcam-1.9.1/bin/flashcam
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-11-02 08:34:00.000000 flashcam-1.9.1/bin/flashcam_join
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3406 2023-11-02 08:34:00.000000 flashcam-1.9.1/bin/flashcam_org
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      865 2023-11-02 08:34:00.000000 flashcam-1.9.1/bin/flashcam_rep
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      679 2024-02-27 15:50:11.000000 flashcam-1.9.1/bin/flashcamg
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-14 18:40:55.007771 flashcam-1.9.1/flashcam/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-11-02 08:34:00.000000 flashcam-1.9.1/flashcam/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5401 2024-03-11 10:00:57.000000 flashcam-1.9.1/flashcam/base_camera2.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8850 2024-03-08 14:33:40.000000 flashcam-1.9.1/flashcam/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-14 18:40:55.011772 flashcam-1.9.1/flashcam/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-11-02 08:34:00.000000 flashcam-1.9.1/flashcam/data/BEAM_OFF.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-11-02 08:34:00.000000 flashcam-1.9.1/flashcam/data/BEAM_ON_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-11-02 08:34:00.000000 flashcam-1.9.1/flashcam/data/DET_NRDY.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-11-02 08:34:00.000000 flashcam-1.9.1/flashcam/data/DET_RDY_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-11-02 08:34:00.000000 flashcam-1.9.1/flashcam/data/digital-7.mono.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34360 2023-11-02 08:34:00.000000 flashcam-1.9.1/flashcam/data/digital-7.regular.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-11-02 08:34:00.000000 flashcam-1.9.1/flashcam/data/monoskop.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     7865 2023-11-02 08:34:00.000000 flashcam-1.9.1/flashcam/data/pattern_acircles.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    22255 2023-11-02 08:34:00.000000 flashcam-1.9.1/flashcam/data/pattern_chessboard.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    12496 2023-11-02 08:34:00.000000 flashcam-1.9.1/flashcam/data/small_pixel.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-11-02 08:34:00.000000 flashcam-1.9.1/flashcam/data/win_rain.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-11-02 08:34:00.000000 flashcam-1.9.1/flashcam/data/win_skull.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-11-02 08:34:00.000000 flashcam-1.9.1/flashcam/data/win_storm.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-11-02 08:34:00.000000 flashcam-1.9.1/flashcam/data/win_winter.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-11-02 08:34:00.000000 flashcam-1.9.1/flashcam/data/windows.jpg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-11-02 08:34:00.000000 flashcam-1.9.1/flashcam/direct.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-11-02 08:34:00.000000 flashcam-1.9.1/flashcam/izmq_receiver.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4635 2024-03-08 14:33:40.000000 flashcam-1.9.1/flashcam/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    50705 2024-04-02 14:16:21.000000 flashcam-1.9.1/flashcam/real_camera.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    43977 2024-04-02 04:35:37.000000 flashcam-1.9.1/flashcam/stream_enhancer.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    86593 2024-04-02 23:52:20.000000 flashcam-1.9.1/flashcam/uniwrec.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5092 2024-04-02 23:14:00.000000 flashcam-1.9.1/flashcam/uniwrec_io.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5142 2024-04-02 22:19:28.000000 flashcam-1.9.1/flashcam/uniwrec_keys.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    16073 2024-04-02 23:42:21.000000 flashcam-1.9.1/flashcam/uniwrec_manip.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13894 2024-04-02 19:22:46.000000 flashcam-1.9.1/flashcam/usbcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    36471 2023-11-02 08:59:16.000000 flashcam-1.9.1/flashcam/v4lc.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2024-04-14 18:40:54.000000 flashcam-1.9.1/flashcam/version.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    41957 2024-04-14 18:40:33.000000 flashcam-1.9.1/flashcam/web.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-14 18:40:55.011772 flashcam-1.9.1/flashcam.egg-info/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-14 18:40:54.000000 flashcam-1.9.1/flashcam.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1049 2024-04-14 18:40:54.000000 flashcam-1.9.1/flashcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-14 18:40:54.000000 flashcam-1.9.1/flashcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      165 2024-04-14 18:40:54.000000 flashcam-1.9.1/flashcam.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2024-04-14 18:40:54.000000 flashcam-1.9.1/flashcam.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-14 18:40:55.015771 flashcam-1.9.1/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2275 2023-11-02 08:34:00.000000 flashcam-1.9.1/setup.py
```

### Comparing `flashcam-1.8.9/PKG-INFO` & `flashcam-1.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.8.9
+Version: 1.9.1
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 Requires-Dist: fire
```

### Comparing `flashcam-1.8.9/README.md` & `flashcam-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/bin/flashcam` & `flashcam-1.9.1/bin/flashcam`

 * *Files 5% similar despite different names*

```diff
@@ -326,28 +326,28 @@
 | -X | XY                                        |     |
 | -y | speed of translation for astrophotography |  18 |
 | -z | zoom                                      |  20 |
 |    | n   u                                     |     |
 | -h | help                                      |     |
     """
 
-    all_commands = ["usage","savecfg","save","flask5000","5000",
-                    "flask", "show", "ls" , "getres" ,
+    all_commands = ["usage","savecfg","save","flask","ask",
+                    "show", "ls" , "getres" ,
                     "v4l", "uni","zmq","zmqv","zmqs",
                     "test"]
 
     if help is not None:
         print(helptext)
         print("COMMANDS:", all_commands)
         print("""
         ls        ... see available cameras, IDPath (use in -p)
         getres    ... show resolutions available for product
         show      ... direct show
-        flask5000 ... start flask on port 5000, consider -w; also 'flask'
-        flask     ... prepare to start gunicorn!!! flashcamg; initialization'
+        flask     ... start flask on port -n xxx (or config value), consider -w; also 'flask'
+        ask       ... wget ... prepare to start gunicorn!!!=flashcamg;
         savecfg   ... save commandline parameters to config
         v4l       ...
         uni       ... uninteruptible stream: uni http://192.168.0.91:8000/video
         zmqv      ... wait imagezmq receive + display + avi
         zmqs      ... wait imagezmq receive silent avi
         """)
         sys.exit(0)
@@ -519,15 +519,15 @@
         print(''' ... usage:
     flashcam command [options]
 _____________________________________________________
     commands:
         ls        ... see available cameras, IDPath (use in -p)
         getres    ... show resolutions available for product
         show      ... direct show
-        flask5000 ... start flask on port 5000, consider -w; also 'flask'
+        flask     ... start flask on port -n xxx, consider -w; also 'flask'
         savecfg   ... save commandline parameters to config
         v4l       ...
         uni       ... uninteruptible stream: uni http://192.168.0.91:8000/video
         zmqv      ... wait imagezmq receive + display + avi
         zmqs      ... wait imagezmq receive silent avi
 _____________________________________________________
     options:                         EXAMPLE:
@@ -538,15 +538,15 @@
         -b ... blur* : blur the frame  | -b 3
         -t ... threshold for motiondet | -t 100
         -f ... frame kind (direct,delta*,detect*,histo)
         -F ... FOURCC codec laps       | -F DIVX,IYUV
         -P ... PIXELFORMAT             | -P YUYV, MJPG
         -H ... show a mean histo value | -H
         -l ... save timelaps [seconds] | -l 3600
-        -w ... open web (for flask5000)| -w
+        -w ... open web (for flask    )| -w
         -e ... exposure (0-1;auto)     | -e 0.02
         -g ... gain     (0-1; default) | -g 0.1
         -m ... gamma    (0-1;default)  | -m 0.1
         -q ... passfile for UNI        | -q ~/.pycamfw_userpass
         -x ... move image in x ( -y)   | -x 0.01
            ... <1 is speed/s >1 fixed  | -x -200 -y 100
         -o ... rotate by N degrees     | -o 180
@@ -770,15 +770,15 @@
         recomvid = usbcheck.recommend_video( product )
         print(f"i... checking resolution for video {recomvid[0]}")
         # should be v4lc.
         resolutions = usbcheck.get_resolutions( recomvid[0] )
         print(resolutions)
         sys.exit(0)
     # ------------------------------------------------------------------------------
-    elif cmd == "flask":
+    elif cmd == "ask":
         print("i... NOT STARTING flask NOT STARTING GUNICORN")
 
         CMD="gunicorn --threads 5  -w 1 -b 0.0.0.0:8000  --timeout 15 web:app"
         print(CMD)
         print(CMD)
         print(CMD)
         print("i... now i ONLY try to initiate the port 8000 and I quit")
@@ -801,37 +801,15 @@
 
     elif cmd == "zmq":
         print("\ni... for receiver of imagezmq use zmqv or zmqs")
         sys.exit(0)
 
 
     # ------------------------------------------------------------------------------
-    elif cmd == "flask5000" or cmd=="5000":
-
-        # [x] why I am saving ? because it is the way to tune real flask 8000?
-        #     - i can only pass to real_cam by saving CONFIG !
-
-
-        # config.CONFIG[''] =
-
-        # NOW i dont want to save during flask5000!
-        #if saveme:
-        #    config.save_config()
-
-        #OR     - i must save it to config, because else config if only x y====
-        #EITHER - I must remove x,y from  cfg.json  file
-        #CHECK WHERE IS THE PROBLEM
-
-        #print(config.CONFIG)
-        #print(config.CONFIG["histogram"]) # here it is true BUT
-
-        #print("===================")
-        #if config.CONFIG['netport']==8000:
-        #    config.CONFIG['netport']=5000
-        #    print(fg.green,"W... FORCED THE PORT == NETPORT == TO 5000 (from previous 8000)  ", fg.default)
+    elif cmd == "flask" :
 
         print(f"i... flask starting on port {config.CONFIG['netport']} - multiprocessing with target=API")
         p = multiprocessing.Process(target=API) # it keeps the config???/ it shuld...
         p.start()
         if web5000:
             webbrowser.open(f"http://localhost:{config.CONFIG['netport']}")
         else:
```

### Comparing `flashcam-1.8.9/bin/flashcam_org` & `flashcam-1.9.1/bin/flashcam_org`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/bin/flashcam_rep` & `flashcam-1.9.1/bin/flashcam_rep`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/bin/flashcamg` & `flashcam-1.9.1/bin/flashcamg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/base_camera2.py` & `flashcam-1.9.1/flashcam/base_camera2.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/config.py` & `flashcam-1.9.1/flashcam/config.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/data/BEAM_OFF.jpg` & `flashcam-1.9.1/flashcam/data/BEAM_OFF.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/data/BEAM_ON_.jpg` & `flashcam-1.9.1/flashcam/data/BEAM_ON_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/data/DET_NRDY.jpg` & `flashcam-1.9.1/flashcam/data/DET_NRDY.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/data/DET_RDY_.jpg` & `flashcam-1.9.1/flashcam/data/DET_RDY_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/data/digital-7.mono.ttf` & `flashcam-1.9.1/flashcam/data/digital-7.mono.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/data/digital-7.regular.ttf` & `flashcam-1.9.1/flashcam/data/digital-7.regular.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/data/monoskop.jpg` & `flashcam-1.9.1/flashcam/data/monoskop.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/data/pattern_acircles.png` & `flashcam-1.9.1/flashcam/data/pattern_acircles.png`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/data/pattern_chessboard.png` & `flashcam-1.9.1/flashcam/data/pattern_chessboard.png`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/data/small_pixel.ttf` & `flashcam-1.9.1/flashcam/data/small_pixel.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/data/win_rain.jpg` & `flashcam-1.9.1/flashcam/data/win_rain.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/data/win_skull.jpg` & `flashcam-1.9.1/flashcam/data/win_skull.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/data/win_storm.jpg` & `flashcam-1.9.1/flashcam/data/win_storm.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/data/win_winter.jpg` & `flashcam-1.9.1/flashcam/data/win_winter.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/data/windows.jpg` & `flashcam-1.9.1/flashcam/data/windows.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/direct.py` & `flashcam-1.9.1/flashcam/direct.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/izmq_receiver.py` & `flashcam-1.9.1/flashcam/izmq_receiver.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/mmapwr.py` & `flashcam-1.9.1/flashcam/mmapwr.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/real_camera.py` & `flashcam-1.9.1/flashcam/real_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,17 +174,24 @@
         #
 
         if len(vids)>0:
             if vids[0]==-1:
                 return config.CONFIG["product"] , -1, None
 
             vidnum = vids[0]
-            print("D... asking VideoCapture", vidnum )
+            print("D... asking VideoCapture", vidnum, dt.datetime.now() )
+            #
+            #  00.0-usb-0:1.3:1.0   00.0-usb-0:1.1:1.0
+            #  00.0-usb-0:1.4:1.0   00.0-usb-0:1.2:1.0
+            #
+            #
             cap = cv2.VideoCapture(vidnum,  cv2.CAP_V4L2)
-            print("D... got    VideoCapture", vidnum )
+            #cap = cv2.VideoCapture(vidnum )
+            ### cap = cv2.VideoCapture(vidnum,  cv2.CAP_DSHOW) ## ??? ## https://stackoverflow.com/questions/59371075/opencv-error-cant-open-camera-through-video-capture#61817613
+            print("D... got    VideoCapture", vidnum , dt.datetime.now())
 
             # config.CONFIG["camera_on"] = True
 
             # - with C270 - it showed corrupt jpeg
             # - it allowed to use try: except: and not stuck@!!!
             #cap = cv2.VideoCapture(vidnum)
             #   70% stucks even with timeout
@@ -606,14 +613,15 @@
             # very stupid camera    ZC0303 Webcam
             if "exposure" in capa:
                 exposure = cc.get_exposure()
                 exposuredef = cc.getdef_exposure()
                 #?????
                 #auto_exposuredef = cc.getdef_exposure()
                 print(f"i... EXPOAUTO (top) == {exposure} vs def={exposuredef}; ")
+                # it seems I lost autoexposure in one RPI4 imx  camera...
 
 
 
 
             nfrm = 0
             # if config.CONFIG["product"]:
             #     wname = "none "
```

### Comparing `flashcam-1.8.9/flashcam/stream_enhancer.py` & `flashcam-1.9.1/flashcam/stream_enhancer.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/uniwrec.py` & `flashcam-1.9.1/flashcam/uniwrec.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,62 @@
 #!/usr/bin/env python3
 
-# there is tuning of the size------
-
-# import the necessary packages
-
-# -----this is some repair of avi?
-#  ls zen_192.168.0.91_20211105_* |
-# while read line; do echo file \'$line\'; done |
-# ffmpeg -protocol_whitelist file,pipe -f
-# concat -i - -c copy zen_192.168.0.91_20211105_.avi
-#
 #
-
+# import pyautogui
 from flashcam.version import __version__
 from console import fg,bg
 # from imutils.video import VideoStream
 import socket
 import time
 import signal
 from contextlib import contextmanager
-
 # import argparse
 
 import cv2
 import datetime
 
-# import datetime as dt
-
 import os
 
-
 from fire import Fire
 
-# import imutils
-
-import urllib.request
+#import urllib.request
 import numpy as np
 
 # user pass
-import base64
-
-import getpass
+#import base64
+#import getpass
 
 import sys
 
 from flashcam.stream_enhancer import Stream_Enhancer
 import webbrowser
 
 import math
 
 import requests  # crosson=CROSSON
 from PIL import ImageFont, ImageDraw, Image
 
+from uniwrec_keys import remap_keys
+from uniwrec_manip import disp_mutext, rotate_image, adjust_gamma, make_measurements, matrix_undistort
+from uniwrec_io import setupsave, get_stream, get_FILE_REDCROSS
+
 # ------------------problem with SHIFT
 # from pynput.keyboard import Key, Listener
 
 
 global SHIFT, CTRL
 SHIFT = CTRL = False
 
 global centerX1, centerY1
-global FILE_USERPASS
-global FILE_REDCROSS
+# global FILE_USERPASS
+#global FILE_REDCROSS
 # ---------- files:
-FILE_USERPASS = "~/.config/flashcam/.flashcam_upw"  # will extend
-FILE_REDCROSS0 = "~/.config/flashcam/crossred"  # will extend
-FILE_REDCROSS = "~/.config/flashcam/crossred"  # will extend
+#FILE_USERPASS = "~/.config/flashcam/.flashcam_upw"  # will extend
+#FILE_REDCROSS0 = "~/.config/flashcam/crossred"  # will extend
+#FILE_REDCROSS = "~/.config/flashcam/crossred"  # will extend
 
 
 global local_gamma, integrate
 local_gamma = 1  # adjust_gamma
 integrate = 1  # call accum
 
 # automatic tuning histogram
@@ -120,331 +107,16 @@
  i/I* ... accumulate images
 
  w ... open web browser
  q ... quit           ? ... HELP
 ctl: t=kompr  h=histo  j=direct  k=detect
        * with remote flashcam server """
 
-
-
-
-
-def rotate_image(image, angle):
-    if angle is None:     return image
-    if abs(angle)<0.1:     return image
-    image_center = tuple(np.array(image.shape[1::-1]) / 2)
-    # print( "rotate", image_center, angle )
-    rot_mat = cv2.getRotationMatrix2D(image_center, angle, 1.0)
-    #print(rot_mat)
-    result = cv2.warpAffine(image, rot_mat, image.shape[1::-1], flags=cv2.INTER_LINEAR)
-    #print("rotated by ", angle)
-    return result
-
-
-
-# NOT IN UBUNTU22
-def kb_on_press(key):
-    global SHIFT, CTRL
-    print("                                              =v=")
-    try:
-        a = key.char
-        # print('alphanumeric key {0} pressed'.format( key.char))
-        # CTRL  = False
-    except AttributeError:
-        print('special key {0} pressed'.format(  key))
-    if key == Key.alt:
-        CTRL = True
-    if key == Key.shift:
-        SHIFT = True
-    return
-
-# NOT ON UBUNTU22
-def kb_on_release(key):
-    global SHIFT, CTRL
-    print("                                              =^=")
-    if key == Key.alt:
-        CTRL = False
-    if key == Key.shift:
-        SHIFT = False
-    print('{0} released'.format( key))
-    if key == Key.esc:
-        # Stop listener
-        return False
-
-
-def remap_keys(key):
-    """
-    Problem - THIS TABLE WORKS ON  gigajm
-        , while zen : 65505
-    """
-    global CTRL
-    CTRL=False
-    print(f" ... remap_keys()  KEY==/{key}/", CTRL)
-    if key>=262241 and key<=262266:CTRL=True  # zen
-    if key>=1310817 and key<=1310842:CTRL=True # zaba
-
-    print(f" ... remap_keys()  KEY==/{key}/ ", CTRL)
-    table = {
-        262241: "a", # zen ctrl
-        262242: "b", # zen ctrl
-        262243: "c", # zen ctrl
-        262244: "d", # zen ctrl
-        262245: "e", # zen ctrl
-        262246: "f", # zen ctrl
-        262247: "g", # zen ctrl
-        262248: "h", # zen ctrl
-        262249: "i", # zen ctrl
-        262250: "j", # zen ctrl
-        262251: "k", # zen ctrl
-        262252: "l", # zen ctrl
-        262253: "m", # zen ctrl
-        262254: "n", # zen ctrl
-        262255: "o", # zen ctrl
-        262256: "p", # zen ctrl
-        262257: "q", # zen ctrl
-        262258: "r", # zen ctrl
-        262259: "s", # zen ctrl
-        262260: "t", # zen ctrl
-        262261: "u", # zen ctrl
-        262262: "v", # zen ctrl
-        262263: "w", # zen ctrl
-        262264: "x", # zen ctrl
-        262265: "y", # zen ctrl
-        262266: "z", # zen ctrl
-
-
-        1310817: "a", #ctrl zaba
-        1310818: "b", #ctrl zaba
-        1310819: "c", #ctrl zaba
-        1310820: "d", #ctrl
-        1310821: "e", #ctrl
-        1310822: "f", #ctrl zaba
-        1310823: "g", #ctrl zaba
-        1310824: "h", #ctrl zaba
-        1310825: "i", #ctrl zaba
-        1310826: "j", #ctrl zaba
-        1310827: "k", #ctrl zaba
-        1310828: "l", #ctrl zaba
-        1310829: "m", #ctrl zaba
-        1310830: "n", #ctrl zaba
-        1310831: "o", #ctrl zaba
-        1310832: "p", #ctrl zaba
-        1310833: "q", #ctrl zaba
-        1310834: "r", #ctrl zaba
-        1310835: "s", #ctrl zaba
-        1310836: "t", # ctrl
-        1310837: "u", # ctrl
-        1310838: "v", # ctrl
-        1310839: "w", # ctrl
-        1310840: "x", # ctrl
-        1310841: "y", # ctrl
-        1310842: "z", # ctrl
-
-        1114175: "?", # zaba
-        65599: "?", # zen
-
-        1048673: "a",
-        1048674: "b",
-        1048675: "c",
-        1048676: "d",
-        1048677: "e",
-        1048678: "f",
-        1048679: "g",
-        1048680: "h",
-        1048681: "i",
-        1048682: "j",
-        1048683: "k",
-        1048684: "l",
-        1048685: "m",
-        1048686: "n",
-        1048687: "o",
-        1048688: "p",
-        1048689: "q",
-        1048690: "r",
-        1048691: "s",
-        1048692: "t",
-        1048693: "u",
-        1048694: "v",
-        1048695: "w",
-        1048696: "x",
-        1048697: "y",
-        1310841: "y", #ctrl
-        1048698: "z",
-        1114177: "A",
-        1114178: "B",
-        1114179: "C",
-        1114180: "D",
-        1114181: "E",
-        1114182: "F",
-
-        65601: "A", # zen
-        65602: "B", #zen
-        65603: "C", # zen
-        65604: "D",
-        65605: "E",
-        65606: "F", # zen
-        65607: "G",
-        65608: "H",
-        65609: "I",
-        65610: "J",
-        65611: "K",
-        65612: "L",
-        65613: "M",
-        65614: "N",
-        65615: "O",
-        65616: "P",
-        65617: "Q",
-        65618: "R",
-        65619: "S",
-        65620: "T",
-        65621: "U",
-        65622: "V",
-        65623: "W",
-        65624: "X",
-        65625: "Y",
-        65626: "Z",
-
-        1114183: "G",
-        1114184: "H",
-        1114185: "I",
-        1114186: "J",
-        1114187: "K",
-        1114188: "L",
-        1114189: "M",
-        1114190: "N",
-        1114191: "O",
-        1114192: "P",
-        1114193: "Q",
-        1114194: "R",
-        1114195: "S",
-        1114196: "T",
-        1114197: "U",
-        1114198: "V",
-        1114199: "W",
-        1114200: "X",
-        1114201: "Y",
-        1114202: "Z",
-    }
-    # 1.  I deactivate ALL above keys to avoid duplicity for arrows etc...
-    #
-    #
-    # 2. I use these ctrl-
-    # ctrle     1310821:''
-    # (key == 1310823): # ctrlg
-    #         1310841): #ctrly
-    # ctrla
-
-    # ####return table[key]
-    if key in table:
-        key = ord(table[key])
-        # keynew = table[key]
-        # #print(f"in remaping {key} - {keynew}")
-        # #return keynew
-    return key
-
-
-# -------------------- DISPLAY MULTITEXT ---------------------
-def disp_mutext(lena, wrapped_text_o):
-    lena = np.array(lena)  # I turn to np.array
-    lena = lena / 255
-
-    size = lena.shape
-    wrapped_text = wrapped_text_o.split("\n")
-
-    img = np.zeros(size, dtype="uint8")
-    img = img + 0.0  # +0.9 # whitish
-    # print("npzero",img.shape, img)
-
-    height, width, channel = img.shape
-
-    # never used text_img = np.ones((height, width))
-    # print(text_img.shape)
-    font = cv2.FONT_HERSHEY_SIMPLEX
-
-    x, y = 10, 40
-    font_size = 0.4
-    font_thickness = 1
-
-    i = 0
-
-    textsize1 = 1
-    textsize0 = 1
-
-    for line in wrapped_text:
-        textsize = cv2.getTextSize(line, font, font_size, font_thickness)[0]
-        if textsize[0] > textsize0:
-            textsize0 = textsize[0]
-        if textsize[1] > textsize1:
-            textsize1 = textsize[1]
-
-    #    wrapped_text.append( " "*textsize1+"[OK]" )
-    # print(    wrapped_text )
-
-    for line in wrapped_text:
-        textsize = cv2.getTextSize(line, font, font_size, font_thickness)[0]
-        if textsize[0] > textsize0:
-            textsize0 = textsize[0]
-        if textsize[1] > textsize1:
-            textsize1 = textsize[1]
-    # ----- after finding the text sizes; define gap
-
-    gap = textsize1 + 6
-
-    nlines = len(wrapped_text)
-    offx = 0 + int((img.shape[1] - textsize0) / 2)
-    offy = 0 + int((img.shape[0] - gap * (nlines - 1)) / 2)
-
-    pad = 10
-    start_point = (offx - pad, offy - pad - textsize1)
-    start_point2 = (offx - pad, offy - pad - textsize1 + int(pad / 2))
-    end_point = (pad + offx + textsize0, offy + gap * len(wrapped_text))
-    end_point2 = (pad + offx + textsize0, offy + gap * len(wrapped_text) - int(pad / 2))
-
-    img = cv2.rectangle(img, start_point, end_point, (0.2, 0.2, 0.2), -1)
-
-    img = cv2.rectangle(img, start_point, end_point, (-1, -1, -1), 1)  # trick
-    img = cv2.rectangle(img, start_point2, end_point2, (-1, -1, -1), 1)
-
-    for line in wrapped_text:
-        textsize = cv2.getTextSize(line, font, font_size, font_thickness)[0]
-        # print(textsize)
-        # gap = textsize[1] + 5
-        # gap = textsize1 # gap define earlier
-
-        y = int((img.shape[0] + textsize[1]) / 2) + i * gap
-        x = 10  # for center alignment => int((img.shape[1] - textsize[0]) / 2)
-        x = offx
-        y = offy + i * gap
-
-        cv2.putText(
-            img,
-            line,
-            (x, y),
-            font,
-            font_size,
-            #                (255,255,255),
-            (-1, -1, -1),  # BIG TRICK
-            font_thickness,
-            lineType=cv2.LINE_AA,
-        )
-        i += 1
-
-    # -------------------- howto merge with frame........
-    img = lena - img
-
-    # print("min", img.min()  , "max=",img.max()  )
-    img = np.clip(img, 0.0, 1.0, None)  # for dark img values, clip to 0
-    # img = img / img.max()
-    # print("min", img.min()  , "max=",img.max()  )
-
-    img = img * 255  # i dont know how to make int
-    img = img.astype(np.uint8)  # this makes negative to positive
-    # print(img)
-    return img
-
+####  rotate_image was here
+####  disp_mutex was here ==================================
 
 @contextmanager
 def timeout(atime):
     # register a function to raise a TimeoutError on the signal
     signal.signal(signal.SIGALRM, raise_timeout)
     # schedule the signal to be sent after 'time'
     signal.alarm(atime)
@@ -462,32 +134,16 @@
         signal.signal(signal.SIGALRM, signal.SIG_IGN)
 
 
 def raise_timeout(signum, frame):
     raise TimeoutError
 
 
-def adjust_gamma(image, gamma=1.0):
-    # build a lookup table mapping the pixel values [0, 255] to
-    # their adjusted gamma values
-    invGamma = 1.0 / gamma
-    table = np.array(
-        [((i / 255.0) ** invGamma) * 255 for i in np.arange(0, 256)]
-    ).astype("uint8")
-    # apply gamma correction using the lookup table
-    return cv2.LUT(image, table)
-
-
-def img_estim(img, thrshld=127):
-    res = np.mean(img)
-    return res
-    is_light = res > thrshld
-    return "light" if is_light else "dark"
-    # 40 -> 2.2
-
+# adjust_gamma was here ===============================
+# img_estim was here
 
 # ------------------------------------------------------------------------ 3
 # ================================================================================================
 
 # ================================================================================================
 
 
@@ -505,15 +161,15 @@
 
     sme = socket.gethostname()
     # frame = None  #  gigavg a vaio have strange behaviour
 
     global jpgkompr1, jpgkompr2
     global CTRL, SHIFT
     global centerX1, centerY1, clicked
-    global FILE_USERPASS, FILE_REDCROSS, FILE_REDCROSS0
+    #global FILE_USERPASS, FILE_REDCROSS, FILE_REDCROSS0
     global show_help
     global allow_tracker, allow_tracker_demand
     global local_gamma, integrate
     global countdown_gain
     centerX1, centerY1, clicked = 0, 0, True  # center zoom ion start
 
     filesource = False
@@ -559,139 +215,28 @@
 – middle/similar: MP42, mp4v
 
 Recommendation:
 – use avi or mkv for best compatibility across all codecs for the maximum flexibility
 – use mp4 (avc1, mp4v) for compatibility across players with most/reasonable compression
 
 """
+    # =============setupsave was here ================
 
-    def setupsave(resolution=(640, 480)):
-        sname = "rec"
-        sname = videodev
-        sname = sname.replace("http", "")
-        sname = sname.replace("//", "")
-        sname = sname.replace(":", "")
-        sname = sname.replace("5000/video", "")
-        sname = sname.replace("8000/video", "")
-
-        sfilenamea = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
-        sme = socket.gethostname()
-        sfilenamea = f"{sme}_{sname}_{sfilenamea}"
-        #
-        # DEFINE EXTENSION : avi+xvid     mov  mp4 mpg
-        #   avi+x264
-        #
-        # sfilenamea = f"{sfilenamea}.mp4"
-        # sfilenamea = f"{sfilenamea}.mp4"
-        sfilenamea = f"{sfilenamea}.mkv"
-
-        # XVID-works     LAGS   X264    MP4V? mp4v-new,ubu22    IYUV-huge
-        CODEC = "mp4v"
-
-        dir2create = os.path.expanduser("~/DATA/")
-        if not os.path.isdir(os.path.expanduser(dir2create)):
-            print(f"D... trying to create directory {dir2create} for saving")
-            # result = False
-            os.mkdir(os.path.expanduser(dir2create))
-
-        sfilenamea = os.path.expanduser("~/DATA/" + sfilenamea)
-        # codec
-        # sfourcc = cv2.VideoWriter_fourcc(*'XVID')
-        # ### sfourcc = cv2.VideoWriter_fourcc(*'LAGS') # lossless NOT mkv,avi
-        # sfourcc = cv2.VideoWriter_fourcc(*'X264') # +avi small NOTubu22
-        # sfourcc = cv2.VideoWriter_fourcc(*'mp4v') # works on UBU22 clean inst
-        # ####sfourcc = cv2.VideoWriter_fourcc(*'MP4V')
-        # ####sfourcc = cv2.VideoWriter_fourcc(*'IYUV') # huge + avi
-
-        sfourcc = cv2.VideoWriter_fourcc(*f"{CODEC}")  #
-
-        #  25 FPS
-        saviout = cv2.VideoWriter(sfilenamea, sfourcc, 25.0, resolution)
-        for i in range(4):
-            print(f"SAVE={sfilenamea} ---  FOURCC={CODEC}")
-        return sfilenamea, saviout
-
-    def get_stream():
-        global CTRL, SHIFT
-        # localuser
-        global FILE_USERPASS, FILE_REDCROSS,FILE_REDCROSS0
-        stream = None  # i return
-        u, p = getpass.getuser(), "a"
-
-        # this is bug.... never find passfile
-        if "passfile" in locals():
-            if passfile is None:
-                print(f"i... nO passfile...trying {videodev} , {passfile}")
-                passfile = videodev.strip("http://")
-                print("i... TRYING", passfile)
-        else:
-            passfile = videodev.strip("http://")
-            passfile = passfile.strip("/video")
-            passfile = passfile.split(":")[0]
-
-            # WITH A HACK  -  I REDEFINE REDCROSS too
-            FILE_REDCROSS = f"{FILE_REDCROSS0}_{passfile}.txt"
-
-            passfile = f"{FILE_USERPASS}_{passfile}"
-            print(f"i... TRYING {videodev} PASS: {passfile}")
-
-        try:
-            with open(os.path.expanduser(passfile)) as f:
-                print("YES---> PASSWORD FILE  ", passfile)
-                w1 = f.readlines()
-                u = w1[0].strip()
-                p = w1[1].strip()
-        except:
-            print("NO PASSWORD FILE (gs) ")
-
-        print("D... capturing from: /{}/".format(videodev))
-        # cam = cv2.VideoCapture( videodev )
-        # stream = urllib.request.urlopen( videodev )
-
-        request = urllib.request.Request(videodev)
-        print("D... USER/PASS", u, p)
-        base64string = base64.b64encode(bytes("%s:%s" % (u, p), "ascii"))
-        print("D... stream ok1", base64string)
-        request.add_header("Authorization", "Basic %s" % base64string.decode("utf-8"))
-
-        # request.add_header("Authorization", "Basic %s" % base64string)
-        print("D... stream ok2 - request.urlopen (disp)")
-        ok = False
-        try:
-            stream = urllib.request.urlopen(
-                request, timeout=3
-            )  # timeout to 7 from 5 sec.
-            ok = True
-            filesource = True
-            print("D... stream ok3")
-        except urllib.error.HTTPError as e:
-            print("Server Offline1? ", e)
-            print(videodev)
-            # do stuff here
-        except urllib.error.URLError as e:
-            print("Server Offline2? ", e)
-            print(videodev)
-            # do stuff here
-        except:
-            ok = False
-            stream = None
-            print("X.... Timeouted on URLOPEN")
-
-        return stream, u, p
+    # ==================getstream was here ==============
 
     # ********************************************************** main loop
     io_none = 0  # to reset stream
     sfilename = ""  # move up to limi # of AVI files.... tst?
     sfilenamea = ""
 
     stream_length = 1024 * 50  # i had 50k all the time from 1st working versn
     stream_length = 1024 * 15  #
 
     if save:
-        sfilenamea, saviout = setupsave()
+        sfilenamea, saviout = setupsave( resolution=(640,480) , videodev=videodev )
     while True:  # ==================== MAIN LOOP =================
         mjpg = False
 
         # #===================== OPENCV START CAPTURE==========================
 
         bytex = b""  # stream
         rpi_name = videodev
@@ -725,15 +270,15 @@
                                 (111, 111, 111),
                                 thickness=line_thickness,
                             )
                         cv2.imshow(rpi_name, gray)  # 1 window for each RPi
                         key = cv2.waitKey(1)
 
                 time.sleep(1)
-                stream, u, p = get_stream()
+                stream, u, p = get_stream( videodev=videodev)
         else:
             print("X... use http:// address")
             print("i... or this may be a file?...")
             # sys.exit(0)
 
         if (str(videodev).find("http://") == 0) or (
             str(videodev).find("https://") == 0
@@ -892,14 +437,22 @@
         # -see the values sent from the webpy - i can use in track,
         #   but not in savejpg,saveavi!
         webframen = ""  # frame number from web.py()
         webframetime = ""
 
         save_decor = False # save with decor or original... save is def in call...
 
+# =================================================================================
+# =================================================================================
+# =================================================================================
+#                CONNECTION HERE =========================
+# =================================================================================
+# =================================================================================
+# =================================================================================
+
         while connection_ok:  # ===============================================
             # read the frame from the camera and send it to the server
             # time.sleep(0.05)
 
             # while True:
             if (str(videodev).find("http://") == 0) or (
                 str(videodev).find("https://") == 0
@@ -1075,84 +628,73 @@
                 # -------- i tried all---no help for csrt tracking-------
                 # frame = cv2.bilateralFilter(frame,5,100,20) # preserve edges
                 # frame = cv2.cvtColor(frame,cv2.COLOR_BGR2GRAY)
                 # (T,frame) = cv2.threshold(frame,  100, 255,
                 #                          cv2.THRESH_BINARY | cv2.THRESH_OTSU)
                 # frame = cv2.blur( frame, (6,6) ) # doesnt help
 
+
+# ============================================================================================
+# ============================================================================================
+# ============================================================================================
+#
+#            Window refreshed/resized ------ something..... From now - real things
+#
+# ============================================================================================
+# ============================================================================================
+# ============================================================================================
+#
+#        RUNNING TRACKERS -=-----------------------------
+#
                 # ======================== track before zoom
                 if (tracker1 is not None) and (not pause):
                     # print("tracking",tracker1)
                     ok, bbox = tracker1.update(frame)
                     if not ok:
                         continue
                     bbox = [round(i * 10) / 10 for i in bbox]
                     (x, y, w, h) = [v for v in bbox]
                     cx, cy = round(10 * (x + w / 2)) / 10, round(10 * (y + h / 2)) / 10
                     # print("tracking",ok,bbox," ->", cx,cy)
                     with open(tracker1_fname, "a") as f:
                         f.write(f"{webframetime} {webframen} {cx} {cy}\n")
                         #   f.write( f"{webframetime[11:]} {webframen} {cx} {cy}\n" )
 
-                    # there is time sent from server... by a trick
-                    #
+                    # there is time sent from server... by a trick  ************ NICE TRICK **********
                     # if from file(or elsewhere) it is int or nothing...
                     #
+                    #print( "WEBFRAMEN...",type(webframen), f"/{webframen}/")
                     if (type(webframen) == int) or (webframen.strip(" ") == ""):
                         # no acq timestamp info from server
                         webframen = frame_num
                         ttime = int(webframen)
-                    else:
+                    elif type(webframen)==str and len(webframen.strip())>9 and webframen!="0000000":
                         # better this, fractions are kept...
                         ttime = datetime.datetime.strptime(
                             # THIS IS A PROBLEM _ WITH NEW WEBTAG_ NEW TTIME NEEDED
                             webframetime, "%H:%M:%S.%f"
-#                            webframetime, "%Y-%m-%d %H:%M:%S.%f"
+                            #                            webframetime, "%Y-%m-%d %H:%M:%S.%f"
                         )
+                    else:
+                        ttime = datetime.datetime.now()
+
 
                     tracker_list.append((round(cx), round(cy), ttime))
                     colmax = 255
                     colmaxb = 0
                     for i in reversed(tracker_list):
                         x2, y2, ttime = i
                         frame[y2, x2] = (colmaxb, 255 - colmax - colmaxb, 255)
                         if colmax > 1:
                             colmax -= 1
                         elif (colmaxb < 255) and (colmaxb > 1):
                             colmaxb += 1
 
                     # ------------ play on cropping -- may further stabilize
                     cropped = frame[round(y) : round(y + h), round(x) : round(x + w)]
-                    # normalize region-   problems/crashes on pause
-                    # resu = np.zeros((640,480))
-                    # cropped = cv2.normalize(cropped, resu,0,255,cv2.NORM_MINMAX)
-                    #    gray
-                    # #cropped = cv2.cvtColor(cropped,cv2.COLOR_BGR2GRAY)
-                    # #cropped = cv2.blur( cropped, (2,2) )
-                    # #(T,cropped) = cv2.threshold(cropped,  100, 255,  cv2.THRESH_BINARY | cv2.THRESH_OTSU)
-                    # merge back to BGR
-                    # #cropped = cv2.merge([cropped,cropped,cropped] )
-
-                    # # return cropped to main image -------------- problem on pause+normalize
-                    # frame[round(y):round(y+h), round(x):round(x+w)] = cropped
-
-                    # ---ORB feature matching...
-                    # cropped = frame[round(y):round(y+h), round(x):round(x+w)]
-                    # kp,des = orb.detectAndCompute(cropped,None)
-                    # frame[round(y):round(y+h), round(x):round(x+w)] = cv2.drawKeypoints(cropped,kp,None)
-
-                    # --- ups
-                    # if not( (x<0)or(y<0)or(x+w>=frame.shape[1])or(y+h>=frame.shape[0]) ):
-                    # print("rect")
-
-                    # # - the other part HSV histo ---- HISTO TRACKING
-                    # hsv = cv2.cvtColor(frame, cv2.COLOR_BGR2HSV)
-                    # dst = cv2.calcBackProject([hsv],[0],roi_hist,[0,180],1)
-                    # ret, track_window = cv2.meanShift(dst,track_window, term_crit)
-                    # xh,yh,wh,hh = track_window
 
                     cv2.rectangle(
                         frame,
                         (round(x), round(y)),
                         (round(x + w), round(y + h)),
                         (0, 255, 0),
                         1,
@@ -1254,15 +796,15 @@
 
                 # I just need to put local gamma before avisave...
                 # else astroimage shows nothing..
                 if local_gamma != 1:
                     frame = adjust_gamma(frame, local_gamma)
 
                 if savepngcont:
-                    sfilename = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
+                    sfilename = datetim<e.datetime.now().strftime("%Y%m%d_%H%M%S")
                     sname = "snapshot"
                     sfilename = f"{sme}_{sfilename}_{sname}.png"
                     sfilename = os.path.expanduser("~/DATA/" + sfilename)
                     print(f"i... PNGcontinuous {sfilename}")
 
                     cv2.imwrite(sfilename, frame)
                     if senh.add_frame(frame):
@@ -1292,378 +834,40 @@
                         senh.setbox("PNG", senh.jpg)
                         frame = senh.get_frame()
 
                 if show_help:
                     # show_help = True
                     frame = disp_mutext(frame, HELPTEXT)
 
+
                 if (allow_tracker_demand) and not (allow_tracker):
                     TRACKERHELP = """
 u ... return back
 
 t ... use tracker1
 T ... use tracker2
   ...  ENTER or SPACE to accept region
   ...  c cancel
 """
                     frame = disp_mutext(frame, TRACKERHELP)
 
-                # MEASUREMENT ==================================
-
-                if measure > 0:
-                    h, w = frame.shape[0], frame.shape[1]
-                    # measure_fov = 110.5 # notebook
-
-                    # approximative, not precise... 5%
-                    radians_per_pixel = (measure_fov / 180 * math.pi) / w
 
-                    # rad per pix * unit distance * better
-                    # worked with zoom cameras????
-                    radians_per_pixel2 = math.tan(measure_fov / 180 * math.pi / 2 / w)
-
-                    # works with my 101deg camera---------------- and 55deg builtin ntbcam
-                    #           ..... for 0.5 tan and alpha have 10% diff (tan vs. atan)
-                    # measure_fov is TOTAL ANGLE
-                    # radians_per_pixel2 =  math.atan(measure_fov /180*math.pi/(2*w) )*2
-                    radians_per_pixel2 = math.atan(measure_fov / 180 * math.pi / w)
-                    # print( radians_per_pixel2 ) # GOOD .... 0.00275
-
-                    # radians_per_pixel2 =
-
-                    radians_per_pixel2 /= zoomme  # process with zoom
-
-                    # print(f"RPPX {radians_per_pixel}  {radians_per_pixel2} ")
-
-                    # now arbitrarily define 1 meter..like.. 100px =>
-                    # alpha = 100*radians_per_pixel
-                    # b = 1m / math.tan( alpha )
-
-                    def get_order(dist=1.7):  # determine order that fits
-                        # list of marks on the ruler
-                        wide = 0.001
-                        notfulrng = 1.0 # notfulrng==0.8; I want full range now..
-                        while True:
-                            wide *= 10
-                            pixwid = math.atan(wide / dist) / radians_per_pixel2
-                            alpha = pixwid * radians_per_pixel2
-                            if pixwid > w / 2 * notfulrng:  # not full rANGE
-                                wide /= 10
-                                pixwid = math.atan(wide / dist) / radians_per_pixel2
-                                alpha = pixwid * radians_per_pixel2
-                                break
-                        order = wide
-
-                        row = []
-
-                        while True:
-                            wide += order
-                            pixwid = math.atan(wide / dist) / radians_per_pixel2
-                            alpha = pixwid * radians_per_pixel2
-                            if pixwid > w / 2 * notfulrng:  # not full rANGE:
-                                wide -= order
-                                pixwid = math.atan(wide / dist) / radians_per_pixel2
-                                # neverused alpha = pixwid * radians_per_pixel2
-                                break
-                            else:
-                                row.append(wide)
-                        # -----
-                        # -----
-                        row.append(order)
-                        row = sorted(row)
-                        row = row[::-1]  # revert - we want Big to small
-                        # print( "TICKS... max:", row[0]  )
-
-                        base = 10**math.floor( math.log10( row[0]) )
-                        if row[0]/base<4:
-                            base = 10**math.floor( math.log10( row[0]/4) )
-
-                        minors = np.arange( base, row[0], base)
-                        minors = minors[::-1]
-                        #print(minors)
-                        if len(row) <= 2:
-                            in0 = row[0] / 2
-                            row.append(in0)
-                            in1 =  row[0] / 4
-                            row.append(in1)
-                        #     in2 = row[0] / 4 *3
-                        #     in3 = row[0] / 5
-                        #     #in2 = row[-1]/10
-                        #     row.append(in2)
-                        #     # row.append( in2 )
-                            # print("   > ",row)
-                        return row,minors  # Big to small
-
-
-                    def one_mark(dist=1.7, wide=[1, 2], speed=0, dispnumb = True):
-                        #  wide ...  # Big to small
-                        # h,w = frame.shape[0], frame.shape[1]
-                        # pixel distance of halfwidth
-
-                        # alpha = pixwid * radians_per_pixel2
-                        # dist = wide/math.tan( alpha)
-                        # I need to calculate 1m
-                        level = 0
-                        # print("XXXXX",wide)
-                        for iwide in wide:
-
-                            # multiply and round to one digit..before pixel calc
-                            for ix in range(4):
-                                if iwide*10**ix > 1:
-                                    iwide = round( iwide* 10**ix)/10**ix
-                                    break
-
-                            pixwid = math.atan(iwide / dist) / radians_per_pixel2
-                            # neverused alpha = pixwid * radians_per_pixel2
-
-                            # print(f" {radians_per_pixel}radpp {pixwid}   {wide}m <- {dist} ")
-                            step = 0
-                            mX, mY = int(w / 2), int(h / 2)
-                            if not (cross is None):
-                                mX += cross[0]
-                                mY += cross[1]
-                            # here I addd the red cross position
-
-                            mY = mY + level * step
-
-                            yA, yB = mY, mY
-
-                            xA = mX
-                            xB = mX + int(pixwid)
-
-                            yC = mY - int(pixwid) # up
-
-                            color = (0, 255, 0)  # BGR
-                            color = (55, 0, 255)  # BGR same as the red cross
-                            colos = (255, 0, 55)  # BGR same as the red cross
-                            if level == 0:
-                                # line - horiznotal
-                                cv2.line(
-                                    frame,
-                                    (int(xA), int(yA)),
-                                    (int(xB), int(yB)),
-                                    color,
-                                    1,
-                                )
-                                cv2.line( # left
-                                    frame,
-                                    (int(xA), int(yA)),
-                                    (int(2*xA-xB), int(yB)),
-                                    color,
-                                    1,
-                                )
-
-
-                                cv2.line( # probably central  mark
-                                    frame,
-                                    (int(xA), int(yA + 8)),
-                                    (int(xA), int(yA - 8)),
-                                    color,
-                                    1,
-                                )
-
-                            # vert bars on horiz axis
-                            cv2.line(  # ticks right
-                                frame,
-                                (int(xB), int(yB + 3)),
-                                (int(xB), int(yB - 3)),
-                                color,
-                                1,
-                            )
-                            cv2.line( # ticks left
-                                frame,
-                                (int(2*xA-xB), int(yB + 3)),
-                                (int(2*xA-xB), int(yB - 3)),
-                                color,
-                                1,
-                            )
-
-                            if yC>0:
-                                # horz bars on vertic axis
-                                cv2.line( # up
-                                    frame,
-                                    (int(xA), int(yA)),
-                                    (int(xA), int(yC)),
-                                    color,
-                                    1,
-                                )
-                                cv2.line(
-                                    frame,
-                                    (int(xA-3), int(yC )),
-                                    (int(xA+3), int(yC )),
-                                    color,
-                                    1,
-                                )
-
-                            unit = "m"
-                            # --- check the biggest to set the unit [0] is biggest
-                            if wide[0] <= 0.001:
-                                iwide = round(iwide * 1000 * 1000) / 1000
-                                unit = "mm"
-                            elif wide[0] <= 0.01:
-                                iwide = round(iwide * 100 * 1000) / 1000
-                                unit = "cm"
-                            elif wide[0] <= 0.1:
-                                iwide = round(iwide * 100 * 100) / 100
-                                unit = "cm"
-                            elif wide[0] < 1:
-                                iwide = round(iwide * 10 *100) / 100
-                                unit = "dm"
-                            else:
-                                iwide = round(iwide * 10) / 10
-
-                            # only properly round whatever unit
-                            if iwide <= 0.001:
-                                iwide = round(iwide * 10000) / 10000
-                            elif iwide <= 0.01:
-                                iwide = round(iwide * 1000) / 1000
-                            elif iwide <= 0.1:
-                                iwide = round(iwide * 100) / 100
-                            elif iwide < 1:
-                                iwide = round(iwide * 10) / 10
-                            else:
-                                iwide = round(iwide)
-
-
-                            if level > 0:
-                                unit = ""  # no unit during the scale
-                            unit2 = "m"
-
-                            if str(iwide)[:2] == "0.":
-                                iwide = str(iwide)[1:]
-
-                            if dispnumb:
-                                # width on scale - scale values
-                                cv2.putText(
-                                    frame,
-                                    f"{iwide}",
-                                    (int(xB - 10), int(mY - 7)),  # little rightx a bit up y
-                                    cv2.FONT_HERSHEY_SIMPLEX,
-                                    0.35,
-                                    color,
-                                    1,
-                                )
-                                cv2.putText(
-                                    frame,
-                                    f"{iwide}",
-                                    (int(2*xA-xB - 10), int(mY - 7)),  # little rightx a bit up y
-                                    cv2.FONT_HERSHEY_SIMPLEX,
-                                    0.35,
-                                    color,
-                                    1,
-                                )
-
-                                cv2.putText(  # up
-                                    frame,
-                                    f"{iwide}{unit}",
-                                    (int(xA + 10), int(yC)),  # little rightx a bit up y
-                                    cv2.FONT_HERSHEY_SIMPLEX,
-                                    0.35,
-                                    color,
-                                    1,
-                                )
-
-
-
-                                if level==0 and unit!="":
-                                    cv2.putText(
-                                        frame,
-                                        f"  unit ... {unit}",
-                                        (
-                                            int(xA - 130),
-                                            int(mY - 5 -40),
-                                        ),  # little rightx a bit up y
-                                        cv2.FONT_HERSHEY_SIMPLEX,
-                                        0.35,
-                                        color,
-                                        1,
-                                    )
+                    #======================
+                    #
+                    #  first big mess
+                    #
+                    #=====================
 
 
-                            if level >= 0:
-                                # distance - only at first mark
-                                cv2.putText(
-                                    frame,
-                                    f"  at {dist} {unit2}",
-                                    (
-                                        int(xA - 130),
-                                        int(mY + 5 -40),
-                                    ),  # little rightx a bit up y
-                                    cv2.FONT_HERSHEY_SIMPLEX,
-                                    0.35,
-                                    color,
-                                    1,
-                                )
-                                cv2.putText(
-                                    frame,
-                                    f"  FOV {measure_fov:.1f}deg",
-                                    (
-                                        int(xA - 130),
-                                        int(mY + 15 -40),
-                                    ),  # little rightx a bit up y
-                                    cv2.FONT_HERSHEY_SIMPLEX,
-                                    0.35,
-                                    color,
-                                    1,
-                                )
-                                # I add velocity
-                                if (level == 0) and not (tracker1 is None):
-                                    cv2.putText(
-                                        frame,
-                                        f"speed {speed:6.2f}m/s",
-                                        (
-                                            int(xB - 50),
-                                            int(mY + 15),
-                                        ),  # little rightx a bit up y
-                                        cv2.FONT_HERSHEY_SIMPLEX,
-                                        0.35,
-                                        color,
-                                        1,
-                                    )
-                            level += 1
+                # MEASUREMENT ==================================
 
-                    # main part of the ruler making---------------
+                if measure > 0:
+                    frame = make_measurements(frame, measure_fov, zoomme, measure, tracker1, tracker_list, cross)
 
-                    order,minorticks = get_order(dist=measure)
-                    # print(minorticks)
 
-                    # speed computation
-                    if not (tracker1 is None) and len(tracker_list) > 2:
-                        b = tracker_list[-1]
-                        try:
-                            v_from = -2
-                            a = tracker_list[v_from]
-                            while True:
-                                dt = (b[2] - a[2]).total_seconds()
-                                if dt > 1.0:
-                                    break
-                                else:
-                                    v_from -= 1
-                                if len(tracker_list) < abs(v_from):
-                                    break
-                                a = tracker_list[v_from]
-                        except:
-                            dt = 100000  # velocity 0
-                        c = ((b[0] - a[0]) ** 2 + (b[1] - a[1]) ** 2) ** 0.5
-                        v = c / dt * radians_per_pixel2
-                        v = round(100 * math.tan(v) * measure) / 100
-                        # print(f"i... speed = {v} m/s  {dt:.2}==dt " )
-                    else:
-                        v = 0
-                    # plot ruler
-                    one_mark(dist=measure, wide=minorticks, speed=v, dispnumb = False)
-                    one_mark(dist=measure, wide=order, speed=v)
-
-                    # ----------- THERE IS A MISTAKE countdown_s not known here
-                #                 if "countdown" in locals() and len(countdown) > 0:
-                #                     now = datetime.datetime.now()
-                #                     delta = now - datetime.datetime(1970, 1, 1)
-                #                     if delta < countdown_s:
-                #                         TEXT = """scanning exposure
-                # in progress"""
-                #                         frame = disp_mutext(frame, TEXT)
 
                 # ANY chnges to imge BEFORE IMSHOW!!
                 if cross is not None:
                     overtext = f"({cross[0]},{cross[1]})"
                     fontpath = os.path.expanduser("~/.config/flashcam/small_pixel.ttf")
                     #fontpath = os.path.expanduser("~/.config/flashcam/digital-7.mono.ttf")
                     position = ( 320+15+cross[0],240-40+cross[1] ) # 480 on x
@@ -1688,36 +892,21 @@
                 # ======================================================== IMSHOW
                 # ======================================================== IMSHOW
 
 
                 apply_distortion = False
                 if apply_distortion:
                     # Assuming no distortion
-                    #dist = np.zeros((5,1))
-                    dist = np.array([[ -8e-7, 4e-11, 0.0, 0.0, 0.0]])
-
-                    #mtx = np.eye(3)
-                    scale = 1.0
-                    mtx = np.array([[scale, 0, h/2], [0, scale, w/2], [0, 0, 1]])
-
-                    h, w = frame.shape[:2]
-
-                    newcameramtx, roi = cv2.getOptimalNewCameraMatrix(mtx, dist, (w,h), 1, (w,h))
-                    # undistort
-                    dst = cv2.undistort(frame, mtx, dist, None, newcameramtx)
-                    ## crop the image
-                    #x, y, w, h = roi
-                    frame = dst#[y:y+h, x:x+w]
+                    frame = matrix_undistort(frame)
 
 
-
-                # IMSHOW #############
-                # IMSHOW #############
-                # IMSHOW #############
-                # IMSHOW #############
+                # IMSHOW #############==================================================================
+                # IMSHOW #############==================================================================
+                # IMSHOW #############==================================================================
+                # IMSHOW #############==================================================================
                 cv2.imshow(rpi_name, frame)  # 1 window for each RPi
                 ##########cv2.moveWindow(rpi_name, int(xy1), int(xy2))
                # ======================================================== IMSHOW
                 if save_decor:
                     saviout.write(frame)
                 # ======================================================== IMSHOW
                 # ======================================================== IMSHOW
@@ -1759,21 +948,18 @@
                 # print(f" {c} x {s} ...      ", end = "       \n")
 
                 #
                 # UBUNTU 22 - ctrl and alt give 227 and 233 resp
                 #
                 if key != -1:
                     print(f" *key== {key}   /{chr(0xFF&key)}/  .. {c} : {s}  >>>.      ")
-                    key = remap_keys(key) # make compatible with waitKey()
+                    key, CTRL = remap_keys(key, CTRL ) # make compatible with waitKey()
                     print(f" ... --------------------------------------------- remapped {key}")
                     # if SHIFT: key = ord(chr(key).upper())
 
-                # i will not use the translation,,
-                # key = remap_keys(key) # make compatible with waitKey()
-                # print(f"remapped {key}")
 
                 # print(f"{centerX1} {centerY1}")
                 if (cross is None) and not greencross:
                     if (frame is not None) and (rpi_name != "") and (key == ord("?") and not CTRL):
                         print("h PRESSED! - ")
                         show_help = not (show_help)
                         print(HELPTEXT)
@@ -1885,15 +1071,15 @@
                     else:
                         print("a PRESSED! - saving AVI WITHOUT DECOR (mkv)")
                         save = True
                         save_decor = False
 
                         height, width, channel = frame.shape
 
-                        sfilenamea, saviout = setupsave((width, height))
+                        sfilenamea, saviout = setupsave((width, height) , videodev=videodev )
                         print(">>>", sfilenamea)
 
 
 
                 if (frame is not None) and \
                    (rpi_name != "") and \
                    (key == ord("A") and not CTRL):  # not with ctl
@@ -1904,15 +1090,15 @@
                         save = False
                     else:
                         print("A PRESSED! - WITH DECOR saving AVI (mkv)")
                         save = True
                         save_decor = True
                         height, width, channel = frame.shape
 
-                        sfilenamea, saviout = setupsave((width, height))
+                        sfilenamea, saviout = setupsave((width, height), videodev=videodev)
                         print(">>>", sfilenamea)
 
 
 
                 if ( (frame is not None) and \
                      (rpi_name != "") and \
                      (key == ord("a"))  and (CTRL) ):  # (key == 1310817):
@@ -1969,30 +1155,33 @@
                         print("Image is successfully saved as file.", sfilename)
 
 
                 # ------------------------- measure and cross -------------------------------
 
                 if (frame is not None) and (rpi_name != ""):
                     if key == ord("C"):
+                        FILE_REDCROSS = get_FILE_REDCROSS( videodev )
                         print(
                             f"c PRESSED! - cross = {cross} OFF; saving {FILE_REDCROSS}"
                         )
                         if (cross is None) or (len(cross) != 2):
                             break
                         with open(os.path.expanduser(FILE_REDCROSS), "w") as f:
                             f.write(f"{cross[0]}\n{cross[1]}\n")
                             cross = None
                     if key == ord("c"):
                         if cross is None:
+                            FILE_REDCROSS = get_FILE_REDCROSS( videodev )
                             cross = [0, 0]
                             if os.path.exists(os.path.expanduser(FILE_REDCROSS)):
                                 try:
                                     with open(os.path.expanduser(FILE_REDCROSS)) as f:
                                         cr = f.readlines()
                                         cross = [int(cr[0]), int(cr[1])]
+                                        print(f"i... redcross loaded {FILE_REDCROSS}")
                                 except:
                                     print(f"X... problem to open {FILE_REDCROSS}")
                             print(f"c PRESSED! - cross = {cross} ON")
 
                 # --------- redcross manip
                 if not (cross is None):
                     if (
@@ -2111,14 +1300,21 @@
                         measure_fov = round(measure_fov * 10) / 10
 
                     if measure_fov < 0.3:
                         measure_fov = 0.3
 
                 # ---------------- trackers--------------- t T u---------------
 
+                # ==========================================================================
+                # ==========================================================================
+                # ==========================================================================
+                #  TRACKER THING
+                # ==========================================================================
+                # ==========================================================================
+                # ==========================================================================
                 # ------if ALLOWED - first - to have no display help
                 # elif to skip one loop
                 if (
                     (allow_tracker)
                     and (frame is not None)
                     and (rpi_name != "")
                     # and allow_tracker1
@@ -2148,14 +1344,15 @@
                         # mask = cv2.inRange(hsv_roi, np.array((0., 60.,32.)), np.array((180.,255.,255.)))
                         # roi_hist = cv2.calcHist([hsv_roi],[0],mask,[180],[0,180])
                         # cv2.normalize(roi_hist,roi_hist,0,255,cv2.NORM_MINMAX)
                         # term_crit = ( cv2.TERM_CRITERIA_EPS | cv2.TERM_CRITERIA_COUNT, 200, 0.1 ) #iters, eps
 
                         # orb = cv2.ORB_create() # I dont use now
 
+
                 if (
                     (allow_tracker)
                     and (frame is not None)
                     and (rpi_name != "")
                     #                    and allow_tracker2
                 ):
                     # and (key == ord('T')):
@@ -2212,14 +1409,23 @@
                     print("u PRESSED! - UNtrack")
                     tracker1 = None
                     tracker2 = None
                     tracker_date = None
                     allow_tracker_demand = False
                     allow_tracker = False
 
+
+                    # ==================================================
+                    # ==================================================
+                    # ==================================================
+                    # END OF TRACKERS
+                    # ==================================================
+                    # ==================================================
+                    # ==================================================
+
                 if (frame is not None) and (rpi_name != "") and (key == ord("v")):
                     print("v PRESSED! - green crosson")
                     greencross = True
                     post_addr = videodev.replace("/video", "/cross")
                     post_data = {"crosson": "CROSSON"}
                     post_response = requests.post(url=post_addr, data=post_data)
```

### Comparing `flashcam-1.8.9/flashcam/usbcheck.py` & `flashcam-1.9.1/flashcam/usbcheck.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,18 @@
 
     0     001 006 2.0 	0458:708c 	 Genius WideCam F100 	 14.0-usb-0:9:1.0 	 12e
     ./usbcheck.py "Genius W"
     rpi with 2 cams...very tedious process - hack slow_track = False
     """
     usb_hubs = usbroot()
 
-    if not(prefname is None) and ( prefname.find(".jpg")>=0  or prefname.find("clock")==0   ):
+    if type(prefname) == int:
+        prefname = f"/dev/video{prefname}"
+        print("D... prefname became", prefname)
+    if (prefname is not None) and ( prefname.find(".jpg")>=0  or prefname.find("clock")==0   ):
         return [-1] # if image is required
 
     # ====================== nice BUT NOT NEEDED HERE
     # devices=serial.tools.list_ports.comports()
     # print("____________________serial  devices _______"+"_"*37)
     # for i in devices:
     #     print(i)
@@ -389,26 +392,27 @@
                     bus,dev,name = lsusbv(f"{vendor}:{model}")
                     #print(usb_hubs)
                     vidid = int(vid[vid.find('/dev/video')+10:])
                     pref = " "
                     if prefname is None:
                         recomvid.append( vidid )
                     else:
-                        if (name.find(str(prefname))>=0) or (id_path.find(str(prefname))>=0):
+                        # vend:mod:rev ;  idpath(usb)    devvideo
+                        if (name.find(str(prefname))>=0) or (id_path.find(str(prefname))>=0) or (vid.find(str(prefname))>=0):
                             recomvid.append( vidid)
                             pref = "*"
                         #if self.verbose:print("     ",vendor, model, vname)
                     print(f"{vidid:2d}   {bus:4s} {dev:4s} {usb_hubs[bus]:6s} {vendor:4s}:{model:4s}:{revision:4s}  {name:20s}  {id_path:16s}  {len(capa)}{GE}   {pref}" )
                     # verify_resolutions( vidid, resolutions )
             # print(prefname, recomvid)
     print(f"{bg.cyan}"+"|"*80,f"{bg.default}")
-    if not prefname is None:
+    if prefname is not None:
         if len(recomvid)==0:
-            print("X... config WANTS the camera",prefname)
-            print("X... NOT FOUND")
+            print("X... no VID recommendation, config WANTS the camera",prefname)
+            #print("X... NOT FOUND")
     if len(recomvid)>0:
         print("i... recommending video#:",recomvid[0], " ... full list:", recomvid)
 
     #resolutions = get_resolutions( recomvid[0] )
     # show_cam( recomvid[0], resolutions[-1] )
 
     return recomvid
```

### Comparing `flashcam-1.8.9/flashcam/v4lc.py` & `flashcam-1.9.1/flashcam/v4lc.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.9/flashcam/web.py` & `flashcam-1.9.1/flashcam/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -1054,46 +1054,77 @@
 def ptz_windowsxp():
     mx = request.args.get('movex')
     my = request.args.get('movey')
     src = request.args.get('src')
     zoom = request.args.get('zoom')
     print(f"i... {fg.yellow}  DX={mx}   DY={my}  SRC={src}  ZOOM={zoom}  {fg.default}")
 
-    if my is not None:
-        if int(my)<0:
-            print("TILT ^")
-            if (pantilthat.get_tilt()-1)>=-85:
-                pantilthat.tilt( pantilthat.get_tilt()-1 )
-        else:
-            print("TILT ^")
-            if (pantilthat.get_tilt()+1)<=-32:
-                pantilthat.tilt( pantilthat.get_tilt()+1 )
-
-    if mx is not None:
-        if int(mx)<0:
-            print("PAN <-")
-            if (pantilthat.get_pan()+1)<=90:
-                pantilthat.pan( pantilthat.get_pan()+1 )
-        else:
-            print("PAN ->")
-            if (pantilthat.get_pan()-1)>=-90:
-                pantilthat.pan( pantilthat.get_pan()-1 )
+    ptz_ok = False
+    try:
+        pantilthat.get_tilt()
+        ptz_ok = True
+    except:
+        print("D... pt-hat not installed")
+
+    if ptz_ok:
+        if my is not None:
+            if int(my)<0:
+                print("TILT ^ - /ptz")
+                if (pantilthat.get_tilt()-1)>=-85:
+                    pantilthat.tilt( pantilthat.get_tilt()-1 )
+            else:
+                print("TILT v - /ptz")
+                if (pantilthat.get_tilt()+1)<=-32:
+                    pantilthat.tilt( pantilthat.get_tilt()+1 )
+
+        if mx is not None:
+            if int(mx)<0:
+                print("PAN <- - /ptz")
+                if (pantilthat.get_pan()+1)<=90:
+                    pantilthat.pan( pantilthat.get_pan()+1 )
+            else:
+                print("PAN -> - /ptz")
+                if (pantilthat.get_pan()-1)>=-90:
+                    pantilthat.pan( pantilthat.get_pan()-1 )
+    else:
+        print("i... experim: dx=-1=no laps; laps 1s, 15s 60s")
+        timelaps = 0
+        try:
+            if mx is not None and int(mx) == -1: timelaps = 0
+            if my is not None and int(my) ==  1: timelaps = 1
+            if mx is not None and int(mx) ==  1: timelaps = 15
+            if my is not None and int(my) == -1: timelaps = 60
+        except:
+            pass
+        if mx is not None or my is not None: mmwrite(f"timelaps {timelaps}" )
+
+        switchzoom = 0
+        try:
+            if zoom is not None and int(zoom) == -1: switchzoom = -1
+            if zoom is not None and int(zoom) == 1: switchzoom = 1
+        except:
+            pass
+        if zoom>0: mmwrite(f"switch_re_on SWITCH_RES_ON" )
+        if zoom<0: mmwrite(f"switch_re_off SWITCH_RES_OFF" )
 
     return "ok", 200
 
 #==================== IN FACT == THIS IS THE START OF THE CAMERA =====
 # with asking Camera()    I create an "instance" (static!) of the class
 # and call init_cam
 #
 # windows  webcamxp ...   jpg  only
 ##### @app.route('/cam_5.cgi')
 @app.route('/video')
+# widows / windowsXP /channel dependent
 @app.route('/cam_5.jpg')
+#@app.route('/cam_<int(cam_id):[0-9]{1,2}.jpg>')
+@app.route('/cam_<regex("[0-9]+"):uid>.jpg')
 @auth.login_required
-def video():
+def video(uid=1):
     remote_ip=request.environ.get('HTTP_X_REAL_IP', request.remote_addr)
     now = dt.datetime.now().strftime("%m/%d %H:%M:%S")
     print(f"W... {now} web is asking VIDEO",request.remote_addr, "(",remote_ip,")", end="\r")
     logthis( " /video remote      = "+request.remote_addr )
     logthis( " /video remote xreal= "+remote_ip )
     # i return JPG TO AXIS CAMERA....
     #---------------this is MJPEG-------------------------
```

### Comparing `flashcam-1.8.9/flashcam.egg-info/PKG-INFO` & `flashcam-1.9.1/flashcam.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.8.9
+Version: 1.9.1
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 Requires-Dist: fire
```

### Comparing `flashcam-1.8.9/flashcam.egg-info/SOURCES.txt` & `flashcam-1.9.1/flashcam.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 flashcam/config.py
 flashcam/direct.py
 flashcam/izmq_receiver.py
 flashcam/mmapwr.py
 flashcam/real_camera.py
 flashcam/stream_enhancer.py
 flashcam/uniwrec.py
+flashcam/uniwrec_io.py
+flashcam/uniwrec_keys.py
+flashcam/uniwrec_manip.py
 flashcam/usbcheck.py
 flashcam/v4lc.py
 flashcam/version.py
 flashcam/web.py
 flashcam.egg-info/PKG-INFO
 flashcam.egg-info/SOURCES.txt
 flashcam.egg-info/dependency_links.txt
```

### Comparing `flashcam-1.8.9/setup.py` & `flashcam-1.9.1/setup.py`

 * *Files identical despite different names*

