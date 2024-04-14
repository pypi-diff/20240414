# Comparing `tmp/whishow-1.3.3-py2.py3-none-any.whl.zip` & `tmp/whishow-1.3.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9816495 bytes, number of entries: 12
+Zip file size: 9816735 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat 16574124 b- defN 24-Apr-09 14:00 whishow/NotoSansCJKsc-Regular.ttf
 -rw-rw-rw-  2.0 fat      107 b- defN 24-Apr-13 20:05 whishow/__init__.py
 -rw-rw-rw-  2.0 fat       66 b- defN 24-Apr-13 20:38 whishow/__main__.py
--rw-rw-rw-  2.0 fat     1557 b- defN 24-Apr-13 21:01 whishow/easyplayer.py
--rw-rw-rw-  2.0 fat     7263 b- defN 24-Apr-13 20:59 whishow/stream.py
+-rw-rw-rw-  2.0 fat     1529 b- defN 24-Apr-14 05:48 whishow/easyplayer.py
+-rw-rw-rw-  2.0 fat     7284 b- defN 24-Apr-14 05:46 whishow/stream.py
 -rw-rw-rw-  2.0 fat     4093 b- defN 24-Apr-13 18:10 whishow/utils.py
--rw-rw-rw-  2.0 fat     8521 b- defN 24-Apr-13 20:59 whishow/whishow.py
--rw-rw-rw-  2.0 fat    35821 b- defN 24-Apr-13 21:04 whishow-1.3.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      886 b- defN 24-Apr-13 21:04 whishow-1.3.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 24-Apr-13 21:04 whishow-1.3.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-13 21:04 whishow-1.3.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      929 b- defN 24-Apr-13 21:04 whishow-1.3.3.dist-info/RECORD
-12 files, 16633485 bytes uncompressed, 9814957 bytes compressed:  41.0%
+-rw-rw-rw-  2.0 fat     6957 b- defN 24-Apr-14 05:39 whishow/whishow.py
+-rw-rw-rw-  2.0 fat    35821 b- defN 24-Apr-14 05:50 whishow-1.3.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2791 b- defN 24-Apr-14 05:50 whishow-1.3.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 24-Apr-14 05:50 whishow-1.3.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-14 05:50 whishow-1.3.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      930 b- defN 24-Apr-14 05:50 whishow-1.3.4.dist-info/RECORD
+12 files, 16633820 bytes uncompressed, 9815197 bytes compressed:  41.0%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: whishow/utils.py
 Comment: 
 
 Filename: whishow/whishow.py
 Comment: 
 
-Filename: whishow-1.3.3.dist-info/LICENSE
+Filename: whishow-1.3.4.dist-info/LICENSE
 Comment: 
 
-Filename: whishow-1.3.3.dist-info/METADATA
+Filename: whishow-1.3.4.dist-info/METADATA
 Comment: 
 
-Filename: whishow-1.3.3.dist-info/WHEEL
+Filename: whishow-1.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: whishow-1.3.3.dist-info/top_level.txt
+Filename: whishow-1.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: whishow-1.3.3.dist-info/RECORD
+Filename: whishow-1.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## whishow/easyplayer.py

```diff
@@ -5,25 +5,25 @@
 
 def player(url,video_dst_frame_size=[640,320]):
     print("ESC for exit ..")
     
     # init the stream reader, named stm.
     stm = STREAM()
     stm.init_state(url=url,
-                    cache_size=10*60)
+                    cache_size=10*60,
+                    video_frame_quality=50)
     # init the whishow player, and connect the audio/video stream of stm.
     ply = PLAY()
-    ply.init_state(start=0,
-                    chunk_size=1,
-                    video_frame_shift=20,
-                    audio_fps=stm.AUDIO_FPS,
-                    video_fps=stm.VIDEO_FPS,
-                    Q_audio_play=stm.Q_audio_play,
-                    Q_video_play=stm.Q_video_play,
-                    asr_results=[])
+    ply.init_state(chunk_size=1,
+                video_frame_shift=20,
+                audio_fps=stm.AUDIO_FPS,
+                video_fps=stm.VIDEO_FPS,
+                Q_audio_play=stm.Q_audio_play,
+                Q_video_play=stm.Q_video_play,
+                asr_results=[])
 
     # esc for exit
     def engine():
         while 1:
             if keyboard.is_pressed('esc'):
                 print("exit ..")
                 break
@@ -35,15 +35,15 @@
     def stream():
         stm.read(video_dst_frame_size=video_dst_frame_size,
                 is_play=True,
                 is_asr=False)
 
     # stream palyer
     def play():
-        ply.run(show_subtitle=False)
+        ply.run()
 
     p0 = threading.Thread(target=engine,args=())
     p1 = threading.Thread(target=stream,args=())
     p2 = threading.Thread(target=play,args=())
 
     p0.start()
     p1.start()
```

## whishow/stream.py

```diff
@@ -15,24 +15,26 @@
 
     def P(self,text):
         printc("%s: %s"%(self.__class__.__name__,text),self.pcolor)
 
     def init_state(self,
                    url:str="",
                    cache_size:int=5*60,
-                   AUDIO_FPS = 16000,
-                   VIDEO_FPS = 30):
+                   video_frame_quality:int=90,
+                   AUDIO_FPS:int = 16000,
+                   VIDEO_FPS:int = 30):
         """
         url: the video address to play
         cache_size: the buffer size to build audio/video cache (seconds) 
-
+        video_frame_quality: Lower picture quality means a smaller buffer
         """
         self.running = True
         self.start_start = False
         self.stream_end = False
+        self.video_frame_quality = video_frame_quality
         self.AUDIO_FPS = AUDIO_FPS
         self.VIDEO_FPS = VIDEO_FPS
         self.init_container(url)
         self.Q_audio_asr = queue.Queue(cache_size*self.AUDIO_FPS)
         self.Q_audio_play = queue.Queue(cache_size*self.AUDIO_FPS)
         self.Q_video_play = queue.Queue(cache_size*self.VIDEO_FPS)
         self.P("Finished to init the state ..")
@@ -132,15 +134,15 @@
                     wt = frame.time
                     if self.start_start:
                         video_count += 1
                         frame = frame.to_image()
                         frame = np.asarray(frame)
                         frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
                         frame = cv2.resize(frame,video_mdf_frame_size)
-                        frame= cv2.imencode('.jpg', frame,[cv2.IMWRITE_JPEG_QUALITY, 90])[1]
+                        frame= cv2.imencode('.jpg', frame,[cv2.IMWRITE_JPEG_QUALITY, self.video_frame_quality])[1]
                         if is_play:
                             self.Q_video_play.put(frame)
 
             pcount += 1
 
             if at>0 :
                 self.start_start = True
@@ -162,12 +164,8 @@
         # 关闭容器和输出文件
         self.container.close()
         self.P("Stop to read stream ..")
         
 
 if __name__ == "__main__":
 
-    # url = "rtmp://mobliestream.c3tv.com:554/live/goodtv.sdp"
-    url = "test.mp4"
-    stm = STREAM()
-    stm.init_state(url=url,cache_size=10*60)
-    stm.read(video_dst_frame_size=[-1,-1])
+    pass
```

## whishow/whishow.py

```diff
@@ -21,25 +21,23 @@
         self.pcolor = "green"
         pass
 
     def P(self,text):
         printc("%s: %s"%(self.__class__.__name__,text),self.pcolor)
 
     def init_state(self,
-                   start:int=0,
                    chunk_size:int=1,
                    video_frame_shift=20,
                    audio_fps:int=16000,
                    video_fps:int=30,
                    Q_audio_play:Queue=None,
                    Q_video_play:Queue=None,
                    asr_results:list=[],
                    font_file:str=""):
         """
-        start: Select the start play time (Seconds)
         chunk_size: The size of each block read on the buffer
         video_frame_shift: If processing per frame is too slow, this parameter can be reduced to improve fps (ms)
         audio_fps: Audio frame per second, offered by whishow.STREAM
         video_fps: Video frame per second, offered by whishow.STREAM
         Q_audio_play: Audio input queue, offered by whishow.STREAM
         Q_Video_play: Video input queue, offered by whishow.STREAM
         asr_results: Will play a role in title generation, format:[[start_second,end_second,asr_content],...]
@@ -49,16 +47,16 @@
         self.running = True
         self.AUDIO_FPS = audio_fps
         self.VIDEO_FPS = video_fps
         self.video_frame_shift = video_frame_shift
         self.Q_audio_play = Q_audio_play
         self.Q_video_play = Q_video_play
         self.asr_results = asr_results
-        self.seek_a = int(start * self.AUDIO_FPS)
-        self.seek_v = int(start * self.VIDEO_FPS)
+        self.seek_a = 0
+        self.seek_v = 0
         self.step_a = int(chunk_size * self.AUDIO_FPS)
         self.step_v = int(chunk_size * self.VIDEO_FPS)
         self.init_audio_driver()
         self.init_video_driver()
         self.fid = 0
         self.aid = 0
         self.vid = 0
@@ -126,105 +124,59 @@
                     seek_asr = self.seek_v/self.VIDEO_FPS
                     for frame in self.video_data:
                         seek_asr += 1/self.VIDEO_FPS
                         text = self.search_subtitle(seek_asr)
                         # frame 处理
                         frame = cv2.imdecode(np.frombuffer(frame, dtype=np.uint8),cv2.IMREAD_COLOR)
                         frame = self.rewrite_video_frame(frame,text)
-                        #
+                        # 播放
                         cv2.imshow(self.win_name, frame)
                         key = cv2.waitKey(self.video_frame_shift)
-                        
-                        
                     self.P(f"listen_video -> frame[{self.vid}] -> cost:{time.time()-s}")
                     self.video_data = []
                     self.vid += 1
             time.sleep(0.001)
         self.P("Stop to play video ..")
 
     
 
-    def run(self,show_subtitle=False):
-        """
-        show_suntitle: Whether to generate subtitles for the video. If yes, the video will be played after the recognition result appears
-        """
+    def run(self):
         
         pa = threading.Thread(target=self.listen_audio,args=())
         pv = threading.Thread(target=self.listen_video,args=())
         pa.start()
         pv.start()
         self.asr_index = 0
         while 1:
             time.sleep(0.1)
             if not self.running:
                 break
-            if show_subtitle and not self.asr_results:continue
+            # if show_subtitle and not self.asr_results:continue
             if self.Q_audio_play.qsize()>=self.step_a and self.Q_video_play.qsize()>=self.step_v and\
                self.fid==self.aid==self.vid:
-                
-                # 播放
+
+                # 取数据
                 chunk_a = [self.Q_audio_play.get() for _ in range(self.step_a)]
                 chunk_v = [self.Q_video_play.get() for _ in range(self.step_v)]
                 chunk_a = np.array(chunk_a,dtype="int16")
                 # chunk_v = np.array(chunk_v,dtype="uint8")
-
+                
+                # 播放
                 self.audio_data = chunk_a
                 self.video_data = chunk_v
                 self.P("Send the %s block data .."%self.fid)
 
                 self.seek_a+=self.step_a
                 self.seek_v+=self.step_v
                 self.fid += 1
                 self.P("seek(play):%s "%(format_timestamp(self.seek_v/self.VIDEO_FPS)))
-            # time.sleep(0.01)
+
         pa.join()
         pv.join()
         self.P("========== PLAY END ==================")
         
 
 
 
 
 if __name__ == "__main__":
-    from whishow.stream import STREAM
-
-    url = "rtmp://mobliestream.c3tv.com:554/live/goodtv.sdp"
-    
-    # init the stream reader, named stm.
-    stm = STREAM()
-    stm.init_state(url=url,
-                  cache_size=10*60)
-    ply = PLAY()
-    ply.init_state(start=0,
-                    step=1,
-                    audio_fps=stm.AUDIO_FPS,
-                    video_fps=stm.VIDEO_FPS,
-                    Q_audio_play=stm.Q_audio_play,
-                    Q_video_play=stm.Q_video_play,
-                    asr_results=[])
-
-    # esc退出播放
-    def engine():
-        global stm,ply
-        import keyboard
-        while 1:
-            if keyboard.is_pressed('esc'):
-                print("exit ..")
-                break
-            time.sleep(0.1)
-        stm.running = False
-        ply.running = False
-
-    def stream():
-        global stm 
-        stm.read(is_play=True,is_asr=False)
-
-    def play():
-        global ply
-        ply.run(show_subtitle=False)
-
-    p0 = threading.Thread(target=engine,args=())
-    p1 = threading.Thread(target=stream,args=())
-    p2 = threading.Thread(target=play,args=())
-    p0.start()
-    p1.start()
-    p2.start()
+    pass
```

## Comparing `whishow-1.3.3.dist-info/LICENSE` & `whishow-1.3.4.dist-info/LICENSE`

 * *Files identical despite different names*

