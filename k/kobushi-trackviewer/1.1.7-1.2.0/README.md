# Comparing `tmp/kobushi_trackviewer-1.1.7-py3-none-any.whl.zip` & `tmp/kobushi_trackviewer-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,22 @@
-Zip file size: 42850 bytes, number of entries: 19
+Zip file size: 44362 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      634 b- defN 21-Aug-15 09:07 kobushi/__init__.py
 -rw-r--r--  2.0 unx      649 b- defN 21-Aug-14 12:53 kobushi/__main__.py
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-08 14:07 kobushi/_version.py
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-14 06:07 kobushi/_version.py
 -rw-r--r--  2.0 unx     3482 b- defN 21-Aug-20 14:15 kobushi/dialog_multifields.py
--rw-r--r--  2.0 unx    35123 b- defN 24-Apr-08 14:07 kobushi/gui_interface.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-Apr-14 06:07 kobushi/font_window.py
+-rw-r--r--  2.0 unx    35595 b- defN 24-Apr-14 06:07 kobushi/gui_interface.py
 -rw-r--r--  2.0 unx     2999 b- defN 21-Aug-14 12:53 kobushi/loadheader.py
 -rw-r--r--  2.0 unx      761 b- defN 22-Oct-15 12:32 kobushi/loadmapgrammer.py
 -rw-r--r--  2.0 unx     1781 b- defN 24-Apr-08 14:07 kobushi/map-grammer.lark
 -rw-r--r--  2.0 unx     9929 b- defN 23-Jul-22 03:03 kobushi/mapinterpreter.py
 -rw-r--r--  2.0 unx    11659 b- defN 23-Jul-22 03:03 kobushi/mapobj.py
 -rw-r--r--  2.0 unx    17464 b- defN 24-Apr-08 14:07 kobushi/mapplot.py
 -rw-r--r--  2.0 unx     6733 b- defN 24-Apr-08 14:07 kobushi/othertrack_window.py
 -rw-r--r--  2.0 unx    17540 b- defN 23-Mar-18 15:38 kobushi/trackcoordinate.py
 -rw-r--r--  2.0 unx    35622 b- defN 23-Jun-24 15:41 kobushi/trackgenerator.py
--rw-r--r--  2.0 unx     9724 b- defN 24-Apr-08 14:08 kobushi_trackviewer-1.1.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     2749 b- defN 24-Apr-08 14:08 kobushi_trackviewer-1.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 14:08 kobushi_trackviewer-1.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-08 14:08 kobushi_trackviewer-1.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1562 b- defN 24-Apr-08 14:08 kobushi_trackviewer-1.1.7.dist-info/RECORD
-19 files, 158533 bytes uncompressed, 40308 bytes compressed:  74.6%
+-rw-r--r--  2.0 unx     9724 b- defN 24-Apr-14 06:07 kobushi_trackviewer-1.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3300 b- defN 24-Apr-14 06:07 kobushi_trackviewer-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-14 06:07 kobushi_trackviewer-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-14 06:07 kobushi_trackviewer-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1641 b- defN 24-Apr-14 06:07 kobushi_trackviewer-1.2.0.dist-info/RECORD
+20 files, 162142 bytes uncompressed, 41700 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: kobushi/_version.py
 Comment: 
 
 Filename: kobushi/dialog_multifields.py
 Comment: 
 
+Filename: kobushi/font_window.py
+Comment: 
+
 Filename: kobushi/gui_interface.py
 Comment: 
 
 Filename: kobushi/loadheader.py
 Comment: 
 
 Filename: kobushi/loadmapgrammer.py
@@ -36,23 +39,23 @@
 
 Filename: kobushi/trackcoordinate.py
 Comment: 
 
 Filename: kobushi/trackgenerator.py
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.7.dist-info/LICENSE
+Filename: kobushi_trackviewer-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.7.dist-info/METADATA
+Filename: kobushi_trackviewer-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.7.dist-info/WHEEL
+Filename: kobushi_trackviewer-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.7.dist-info/top_level.txt
+Filename: kobushi_trackviewer-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.7.dist-info/RECORD
+Filename: kobushi_trackviewer-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kobushi/_version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.7'
+__version__ = '1.2.0'
```

## kobushi/gui_interface.py

```diff
@@ -25,25 +25,28 @@
 import tkinter.simpledialog as simpledialog
 import tkinter.font as font
 
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 from matplotlib import rcParams
 import matplotlib.gridspec
+import matplotlib.font_manager
 import numpy as np
 
 # https://qiita.com/yniji/items/3fac25c2ffa316990d0c matplotlibで日本語を使う
 rcParams['font.family'] = 'sans-serif'
 rcParams['font.sans-serif'] = ['Hiragino Sans', 'Yu Gothic', 'Meirio', 'Takao', 'IPAexGothic', 'IPAPGothic', 'VL PGothic', 'Noto Sans CJK JP']
 
+
 from ._version import __version__
 from . import mapinterpreter as interp
 from . import mapplot
 from . import dialog_multifields
 from . import othertrack_window
+from . import font_window
 
 # http://centerwave-callout.com/tkinter内で起きた例外をどうキャッチするか？/
 class Catcher: # tkinter内で起きた例外をキャッチする
     def __init__(self, func, subst, widget):
         self.func = func
         self.subst = subst
         self.widget = widget
@@ -57,29 +60,33 @@
             if not __debug__: # デバッグモード(-O)なら素通し。pdbが起動する
                 raise e
             else:
                 print(e) # 通常モードならダイアログ表示
                 tk.messagebox.showinfo(message=e)
 
 class mainwindow(ttk.Frame):
-    def __init__(self, master, parser, stepdist = 25):
+    def __init__(self, master, parser, stepdist = 25, font = ''):
         self.dmin = None
         self.dmax = None
         self.result = None
         self.profYlim = None
         self.default_track_interval = stepdist
         
         super().__init__(master, padding='3 3 3 3')
         self.master.title('Kobushi trackviewer')
         self.grid(column=0, row=0, sticky=(tk.N, tk.W, tk.E, tk.S))
         self.master.columnconfigure(0, weight=1)
         self.master.rowconfigure(0, weight=1)
         
         master.protocol('WM_DELETE_WINDOW', self.ask_quit)
         
+        self.fontctrl = font_window.FontControl(None,self)
+        if font != '':
+            self.fontctrl.set_fontname(font)
+        
         self.create_widgets()
         self.create_menubar()
         self.bind_keyevent()
         self.subwindow = othertrack_window.SubWindow(tk.Toplevel(master), self)
         
         self.parser = parser
 
@@ -261,14 +268,15 @@
         self.menu_file.add_command(label='軌道座標を保存...', command=self.save_trackdata)
         self.menu_file.add_separator()
         self.menu_file.add_command(label='終了', command=self.ask_quit, accelerator='Alt+F4')
         
         self.menu_option.add_command(label='座標制御点...', command=self.set_arbcpdist)
         self.menu_option.add_command(label='描画可能区間...', command=self.set_plotlimit)
         self.menu_option.add_command(label='断面図y軸範囲...', command=self.set_profYlimit)
+        self.menu_option.add_command(label='Font...', command=self.fontctrl.create_window)
         
         #self.menu_option.add_command(label='customdialog...', command=self.customdialog_test)
         
         self.menu_help.add_command(label='ヘルプ...', command=self.open_webdocument)
         self.menu_help.add_command(label='Kobushiについて...', command=self.aboutwindow)
         
         self.master['menu'] = self.menubar
@@ -478,14 +486,15 @@
             self.ydim_offset_entry['state']='normal'
             self.setdist_scale(0)
     def distset_entry(self, event=None):
         if self.result != None:
             self.distance_scale.set((self.setdist_entry_val.get()-self.distrange_min)/((self.distrange_max-self.dist_range_arb_val.get()) - self.distrange_min)*100)
     def plot_all(self):
         if(self.result != None):
+            rcParams['font.family'] = self.fontctrl.get_fontname()
             self.draw_planerplot()
             self.draw_profileplot()
     def ask_quit(self, event=None, ask=True):
         if ask:
             if tk.messagebox.askyesno(message='Kobushi Track Viewerを終了しますか？'):
                 self.quit()
         else:
@@ -617,16 +626,17 @@
         #import sys
         sys.excepthook = info
         print('Debug mode')
 
     argparser = argparse.ArgumentParser()
     argparser.add_argument('filepath', metavar='F', type=str, help='input mapfile', nargs='?')
     argparser.add_argument('-s', '--step', help='distance interval for track calculation', type=float, default=25)
+    argparser.add_argument('-f', '--font', help='Font', type=str, default = 'sans-serif')
     args = argparser.parse_args()
-    
+       
     tk.CallWrapper = Catcher
     root = tk.Tk()
-    app = mainwindow(master=root, parser = None, stepdist = args.step)
+    app = mainwindow(master=root, parser = None, stepdist = args.step, font=args.font)
 
     if args.filepath is not None:
         app.open_mapfile(inputdir=args.filepath)
     app.mainloop()
```

## Comparing `kobushi_trackviewer-1.1.7.dist-info/LICENSE` & `kobushi_trackviewer-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kobushi_trackviewer-1.1.7.dist-info/METADATA` & `kobushi_trackviewer-1.2.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: kobushi-trackviewer
-Version: 1.1.7
+Version: 1.2.0
 Summary: Trackviewer for BVE trainsim 5/6
 Home-page: https://github.com/konawasabi/kobushi-trackviewer/
 Author: Konawasabi
 Author-email: webmaster@konawasabi.riceball.jp
 License: Apache License 2.0
 Keywords: BVE trainsim
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: matplotlib
-Requires-Dist: ttkwidgets
-Requires-Dist: lark
+Requires-Dist: scipy >=1.13.0
+Requires-Dist: matplotlib >=3.8.4
+Requires-Dist: ttkwidgets >=0.13.0
+Requires-Dist: lark >=1.1.9
 
 # Kobushi trackviewer
 
 Bve trainsim 5/6向けのマップファイルから、線路平面図・縦断面図を生成するPythonスクリプトです。
 
 動作にはPython 3が必要です。
 
@@ -46,23 +45,37 @@
 Powershellで以下のコマンドを実行します。
 ```
 python -m kobushi
 ```
 
 `python -m kobushi hoge.txt`として、読み込みたいマップファイルを指定して起動することも可能です。
 
+### オプション引数
+
+- `-h, --help`
+  - ヘルプメッセージを表示して終了
+- `-s STEP, --step STEP`
+  - 軌道座標を計算する距離程間隔をSTEP [m]に設定
+  - Default: 25[m]
+- `-f FONT, --font FONT`
+  - 線路平面図・縦断面図で使用するフォントをFONTに設定
+  - フォント名にスペースが含まれる場合、ダブルクォーテーションで囲むこと
+  - Default: sans-serif
+
+
 ## リファレンス
 
 [こちら](reference.md)を参照
 
 ## おことわり
 
 バージョン1.10以前のマップファイルには対応していません。[マップコンバーター](https://bvets.net/jp/download/mapconv.html)でMap 2.00への変換が必要です。
 
-多バイト文字を変数名に使用しているマップには対応していません。変数名に利用できる文字は英字(A-Z, a-z), 数字(0-9), アンダーバー(_)です。
+~~多バイト文字を変数名に使用しているマップには対応していません。変数名に利用できる文字は英字(A-Z, a-z), 数字(0-9), アンダーバー(_)です。~~
+Version 1.1.7で多バイト文字を変数名に使用したマップに対応しました。
 
 その他、BVE本体では読み込み可能なマップファイルがKobushiでは正しく読み込めない場合があります。ご了承ください。
 
 ## License
 
 [Apache License, Version 2.0](LICENSE)
```

## Comparing `kobushi_trackviewer-1.1.7.dist-info/RECORD` & `kobushi_trackviewer-1.2.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 kobushi/__init__.py,sha256=_OBJRtuhwlJl97iwmsRFAjWTMcS1F7fivZjoumsd8qk,634
 kobushi/__main__.py,sha256=zrMhFiAoyKL6DprEbJWok4KNmlsu-fVIA7xT581287E,649
-kobushi/_version.py,sha256=-fuOquJHyQzJBvFtIu-3yyIDnUrOzpa5DnHRbCoQnE4,22
+kobushi/_version.py,sha256=U3f_Jgr3zpgiYG2kLcvcT05TQsVzN9Kktg_f3Q9OZFA,22
 kobushi/dialog_multifields.py,sha256=hWcMMg8KOFql3NC-jQueRrnNUJpQutSI9IOjLh6cleU,3482
-kobushi/gui_interface.py,sha256=T3P0TCy41nMZTvXteCh-raSzBTvIS3Zyvw4wTMP0iUs,35123
+kobushi/font_window.py,sha256=J1tSAxv4zvHcGZDcniATQmg_bnWNbdcIGht8qgyHCgc,2507
+kobushi/gui_interface.py,sha256=AUc02H-DV8PAIqcRYxKNprEvj2yODeeogm2J8ZM6-a8,35595
 kobushi/loadheader.py,sha256=rLutNKL6VAgZXNwyaLmkiz8j3I6VOs93XqqbxFD6Ods,2999
 kobushi/loadmapgrammer.py,sha256=f5OHCL2l483D0IkBLTulsfQZfLcDmyidutt7TDjSHbU,761
 kobushi/map-grammer.lark,sha256=FWXjldaUyp9T1XoLW5vQI3wRCowsbGmdbRqXDkOQalY,1781
 kobushi/mapinterpreter.py,sha256=-HlhhH6IjVVXl3nYu81oq7GCwzuIw6QxuMiNDRBpTU0,9929
 kobushi/mapobj.py,sha256=Gi_xxHAwcK5uIiPXjIr6_om-QvD16_-qFhAuU5q7PFc,11659
 kobushi/mapplot.py,sha256=SD534B5OiFCJD0-elBg5bOP6nz7QgHhfV_KithmZEvE,17464
 kobushi/othertrack_window.py,sha256=PM7iSj03NdBdipYK9P5QNlJKRrnp0mo6Ek9jsXMo1JY,6733
 kobushi/trackcoordinate.py,sha256=dwu44v5uvA8yUcJOs50eNLzktOFJJT28pUhccXGJRR8,17540
 kobushi/trackgenerator.py,sha256=9p_elvjclxYnqrxaLwMaFrZkw-exg5ocUijVihy5614,35622
-kobushi_trackviewer-1.1.7.dist-info/LICENSE,sha256=OURbRZ-GYhaD-XMftqfQcIGdw3mEDo71L2K7HGiUIpE,9724
-kobushi_trackviewer-1.1.7.dist-info/METADATA,sha256=pf5Xb5vjONrWWDpjUpkqDAhwOVQflEW831d4z-u7VmQ,2749
-kobushi_trackviewer-1.1.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-kobushi_trackviewer-1.1.7.dist-info/top_level.txt,sha256=g2m4m7gw1NgwbluSrxfBImA8GHjvuXwFnHgkagrMPB0,8
-kobushi_trackviewer-1.1.7.dist-info/RECORD,,
+kobushi_trackviewer-1.2.0.dist-info/LICENSE,sha256=OURbRZ-GYhaD-XMftqfQcIGdw3mEDo71L2K7HGiUIpE,9724
+kobushi_trackviewer-1.2.0.dist-info/METADATA,sha256=YFN9PUZKSca8KzYbe3RrgrONx_qYVMDPsbizvp1xjjw,3300
+kobushi_trackviewer-1.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+kobushi_trackviewer-1.2.0.dist-info/top_level.txt,sha256=g2m4m7gw1NgwbluSrxfBImA8GHjvuXwFnHgkagrMPB0,8
+kobushi_trackviewer-1.2.0.dist-info/RECORD,,
```

