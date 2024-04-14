# Comparing `tmp/bulletroulette-1.0.tar.gz` & `tmp/bulletroulette-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulletroulette-1.0.tar", last modified: Sat Apr 13 12:16:04 2024, max compression
+gzip compressed data, was "bulletroulette-1.0.2.tar", last modified: Sun Apr 14 03:08:16 2024, max compression
```

## Comparing `bulletroulette-1.0.tar` & `bulletroulette-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-13 12:16:04.843536 bulletroulette-1.0/
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     1070 2024-04-13 02:31:44.000000 bulletroulette-1.0/LICENSE
--rw-r--r--   0 gqx       (1000) gqx       (1000)     1942 2024-04-13 12:16:04.839536 bulletroulette-1.0/PKG-INFO
--rw-rw-r--   0 gqx       (1000) gqx       (1000)      934 2024-04-13 11:46:05.000000 bulletroulette-1.0/README.md
-drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-13 12:16:04.839536 bulletroulette-1.0/bulletroulette/
--rw-rw-r--   0 gqx       (1000) gqx       (1000)        0 2024-04-13 12:01:24.000000 bulletroulette-1.0/bulletroulette/__init__.py
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     1241 2024-04-13 01:51:20.000000 bulletroulette-1.0/bulletroulette/data.py
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     3199 2024-04-09 13:27:21.000000 bulletroulette-1.0/bulletroulette/roles.py
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    12703 2024-04-13 12:01:29.000000 bulletroulette-1.0/bulletroulette/run.py
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     1042 2024-04-09 13:27:21.000000 bulletroulette-1.0/bulletroulette/sprites.py
-drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-13 12:16:04.839536 bulletroulette-1.0/bulletroulette.egg-info/
--rw-r--r--   0 gqx       (1000) gqx       (1000)     1942 2024-04-13 12:16:04.000000 bulletroulette-1.0/bulletroulette.egg-info/PKG-INFO
--rw-rw-r--   0 gqx       (1000) gqx       (1000)      337 2024-04-13 12:16:04.000000 bulletroulette-1.0/bulletroulette.egg-info/SOURCES.txt
--rw-rw-r--   0 gqx       (1000) gqx       (1000)        1 2024-04-13 12:16:04.000000 bulletroulette-1.0/bulletroulette.egg-info/dependency_links.txt
--rw-rw-r--   0 gqx       (1000) gqx       (1000)       14 2024-04-13 12:16:04.000000 bulletroulette-1.0/bulletroulette.egg-info/requires.txt
--rw-rw-r--   0 gqx       (1000) gqx       (1000)       15 2024-04-13 12:16:04.000000 bulletroulette-1.0/bulletroulette.egg-info/top_level.txt
--rw-rw-r--   0 gqx       (1000) gqx       (1000)       38 2024-04-13 12:16:04.843536 bulletroulette-1.0/setup.cfg
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     1473 2024-04-13 12:15:27.000000 bulletroulette-1.0/setup.py
+drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-14 03:08:16.835646 bulletroulette-1.0.2/
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     1070 2024-04-13 02:31:44.000000 bulletroulette-1.0.2/LICENSE
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       68 2024-04-14 03:04:23.000000 bulletroulette-1.0.2/MANIFEST.in
+-rw-r--r--   0 gqx       (1000) gqx       (1000)     1944 2024-04-14 03:08:16.835646 bulletroulette-1.0.2/PKG-INFO
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)      934 2024-04-13 11:46:05.000000 bulletroulette-1.0.2/README.md
+drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-14 03:08:16.831646 bulletroulette-1.0.2/bulletroulette/
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       98 2024-04-14 00:21:35.000000 bulletroulette-1.0.2/bulletroulette/__init__.py
+drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-14 03:08:16.835646 bulletroulette-1.0.2/bulletroulette/assets/
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)      208 2024-04-13 02:21:31.000000 bulletroulette-1.0.2/bulletroulette/assets/__init__.py
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     1143 2024-04-14 02:40:49.000000 bulletroulette-1.0.2/bulletroulette/data.py
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     3187 2024-04-14 02:40:51.000000 bulletroulette-1.0.2/bulletroulette/roles.py
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    13727 2024-04-14 02:40:53.000000 bulletroulette-1.0.2/bulletroulette/run.py
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     1009 2024-04-14 02:41:24.000000 bulletroulette-1.0.2/bulletroulette/sprites.py
+drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-14 03:08:16.835646 bulletroulette-1.0.2/bulletroulette.egg-info/
+-rw-r--r--   0 gqx       (1000) gqx       (1000)     1944 2024-04-14 03:08:16.000000 bulletroulette-1.0.2/bulletroulette.egg-info/PKG-INFO
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)      383 2024-04-14 03:08:16.000000 bulletroulette-1.0.2/bulletroulette.egg-info/SOURCES.txt
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)        1 2024-04-14 03:08:16.000000 bulletroulette-1.0.2/bulletroulette.egg-info/dependency_links.txt
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       14 2024-04-14 03:08:16.000000 bulletroulette-1.0.2/bulletroulette.egg-info/requires.txt
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       15 2024-04-14 03:08:16.000000 bulletroulette-1.0.2/bulletroulette.egg-info/top_level.txt
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       38 2024-04-14 03:08:16.835646 bulletroulette-1.0.2/setup.cfg
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     1475 2024-04-14 03:08:01.000000 bulletroulette-1.0.2/setup.py
```

### Comparing `bulletroulette-1.0/LICENSE` & `bulletroulette-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0/PKG-INFO` & `bulletroulette-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulletroulette
-Version: 1.0
+Version: 1.0.2
 Summary: 模仿steam游戏“恶魔轮盘”，目前没有提供开发接口（只能单纯玩）
 Home-page: https://github.com/BinaryGuo/Buckshot_Roulette
 Author: GQX
 Author-email: kill114514251@outlook.com
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries :: pygame
```

### Comparing `bulletroulette-1.0/README.md` & `bulletroulette-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0/bulletroulette/data.py` & `bulletroulette-1.0.2/bulletroulette/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-# 此文件用于定义各种常量（必须）各种改动可在这里进行（比如路径）
+# 此文件用于定义各种常量，各种改动可在这里进行（比如路径）
 
 ASSESTS    = "assets/" # 修改为存放图片背景音乐等素材的目录
-DIR        = "/home/gqx/codelab/Buckshot_Roulette/" #修改为此程序存放的路径  
 RED        = (255,  0,  0)
 WHITE      = (255,255,255)
 BACKGROUND = f"{ASSESTS}bg.png"
 BGM        = f"{ASSESTS}bgmsc.ogg"
 FONT       = f"{ASSESTS}Simhei.ttf"
 LETTERS    = ("A","B","C","D","E","F","G","H","I","J","K","L","M","N","O","P","Q","R","S","T","U","V","W","X","Y","Z")
 DELETE     = f"{ASSESTS}DELETE.png"
```

### Comparing `bulletroulette-1.0/bulletroulette/roles.py` & `bulletroulette-1.0.2/bulletroulette/roles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 此文件用于定义角色类（必须）
+# 此文件用于定义角色类
 from random import random
 
 class Dealer: # 恶魔
     def __init__(self,health,prop = []) -> None: # 初始化
         self.__tophealth = health
         self.__health = health
         self.__prop = prop
```

### Comparing `bulletroulette-1.0/bulletroulette/run.py` & `bulletroulette-1.0.2/bulletroulette/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 __version__ = "1.0" # 版本说明（没什么用）
 
 # 外部导入
 cannotuseGUI = False
 from random import shuffle
 from time import sleep
 import pygame
-from traceback import print_exc
 from os import chdir
+from traceback import print_exc
 # 模块导入
-from roles import *
-from data import *
-try:
-    from sprites import Button
-except:
-    print("警告！无法导入sprites.py，无法使用窗口模式！")
-    cannotuseGUI = True
+from bulletroulette.roles import *
+from bulletroulette.data import *
+from bulletroulette.sprites import *
 # 以下是主程序
-chdir(DIR)
+file = __file__
+while file[-1] != "/":
+    file = file[:-1]
+chdir(file)
 health = [2,4,6]
 buckshots = [ # 子弹（1代表实，0代表空）
         [
             [1,0,0],
             [1,1,0,0]
         ],
         [
@@ -33,264 +32,265 @@
         [
             [1,1,1,1,1,0,0,0],
             [1,1,1,1,0,0,0,0],
             [1,1,1,0],
             [1,1,1,1,0,0,0,0]
         ]
     ]
-try:
-    if cannotuseGUI:
-        mode = 2
-    else:
-        mode = int(input("请选择模式（壳程序按0（更为稳定）,窗口按1（游戏体验更好））:"))
-    if mode:
-        FPS = int(input("请设置帧率（如果设的太高您的计算机可能运行不了，区间：1～200）："))
-        assert FPS >= 1 and FPS <= 200,"FPS out of range"
-        pygame.init()
-        # 以下是一些关于pygame的一些常量声明
-        # 以下是初始化
-        clock = pygame.time.Clock() # 初始化时钟
-        screen = pygame.display.set_mode((1400,850)) # 屏幕（窗口）初始化
-        pygame.display.set_caption("Buckshot Roulette") # 设置标题
-        background = pygame.image.load(BACKGROUND) # 加载背景图
-        gunimage = pygame.image.load(GUN) # 加载霰弹枪图片
-        charge = pygame.image.load(CHARGE) # 加载血量图片
-        blank = pygame.image.load(BLANK) # 加载空弹图片
-        liveround = pygame.image.load(LIVEROUND) # 加载实弹图片
-        dealershootself = pygame.image.load(SHOOTSELF) # 加载恶魔射击自己时的图片
-        dealershootplayer = pygame.image.load(SHOOTPLAYER) # 加载恶魔射击玩家时的图片
-        buckshotlocation = blank.get_rect() # 获取子弹显示位置
-        shootlocation = dealershootself.get_rect() # 获取恶魔射击时的位置
-        chargelocation = charge.get_rect() # 获取血量显示位置
-        gunimage.set_alpha(0) # 完全透明（此图是为了绘制边框）
-        gun = Button(675,300,gunimage,1) # 加载按钮（Button类的定义在sprites.py)
-        pygame.mixer.music.load(BGM) # 加载背景音乐（BGM）
-        liveplayermusic = pygame.mixer.Sound(LIVEPLAYER) # 玩家被击中时的音效
-        livedealermusic = pygame.mixer.Sound(LIVEDEALER) # 恶魔被击中时的音效
-        blankmusic = pygame.mixer.Sound(BLANKMUSIC) # 空弹发射时的音效
-        shootlocation.center = (700,300) # 设置恶魔射击时的位置
-        text = pygame.font.Font(FONT,75) # 设定字体
-        nametext = text.render("Enter name:",False,WHITE) # 用字体生成文字
-        playerlose = text.render("dealer win!",False,WHITE) # 用字体生成文字
-        loseorwinlocation = playerlose.get_rect()
-        loseorwinlocation.center = (700,425)
-        nametextlocation = nametext.get_rect()
-        nametextlocation.center = (700,100)
-        shootdealer = Button(700,75,text.render("DEALER",False,WHITE),1)
-        dealerturntext = text.render("dealer's turn",False,WHITE)
-        buttons = []
-        name = ""
-        for i in range(26):buttons.append(Button(50*(i+1),700,pygame.image.load(f"assets/{LETTERS[i]}.png")))
-        delete = Button(350,760,pygame.image.load(DELETE))
-        enter = Button(800,760,pygame.image.load(ENTER))
-        # 以下是一些控制变量
-        naming = True # 正在命名
-        playerturn = False # 玩家回合
-        dealerturn = False # 恶魔回合
-        choosing = False
-        drawingbuckshots = False
-        wasd = int(0)
-        turn = [0,0]
-        dealer = Dealer(2)
-        player = Player(2,name)
-        # 以下是游戏主循环
-        pygame.mixer.music.play(-1)
-        while True:
-            for event in pygame.event.get():
-                if event.type == pygame.QUIT:
-                    raise SystemExit
-            screen.blit(background,(0,0))
-            if not player.gethealth():
-                screen.blit(playerlose,loseorwinlocation)
-                pygame.display.update()
-                sleep(3)
-                raise SystemExit
-            if not dealer.gethealth():
-                turn[1] = 0
-                turn[0] += 1
-                del buckshot
-                screen.blit(playerwin,loseorwinlocation)
-                pygame.display.update()
-                sleep(3)
-                if turn[0] == 3:
+def run():
+    try:
+        if cannotuseGUI:
+            mode = 2
+        else:
+            mode = int(input("请选择模式（壳程序按0（更为稳定）,窗口按1（游戏体验更好））:"))
+        if mode:
+            FPS = int(input("请设置帧率（如果设的太高您的计算机可能运行不了，区间：1～200）："))
+            assert FPS >= 1 and FPS <= 200,"FPS out of range"
+            pygame.init()
+            # 以下是一些关于pygame的一些常量声明
+            # 以下是初始化
+            clock = pygame.time.Clock() # 初始化时钟
+            screen = pygame.display.set_mode((1400,850)) # 屏幕（窗口）初始化
+            pygame.display.set_caption("Buckshot Roulette") # 设置标题
+            background = pygame.image.load(BACKGROUND) # 加载背景图
+            gunimage = pygame.image.load(GUN) # 加载霰弹枪图片
+            charge = pygame.image.load(CHARGE) # 加载血量图片
+            blank = pygame.image.load(BLANK) # 加载空弹图片
+            liveround = pygame.image.load(LIVEROUND) # 加载实弹图片
+            dealershootself = pygame.image.load(SHOOTSELF) # 加载恶魔射击自己时的图片
+            dealershootplayer = pygame.image.load(SHOOTPLAYER) # 加载恶魔射击玩家时的图片
+            buckshotlocation = blank.get_rect() # 获取子弹显示位置
+            shootlocation = dealershootself.get_rect() # 获取恶魔射击时的位置
+            chargelocation = charge.get_rect() # 获取血量显示位置
+            gunimage.set_alpha(0) # 完全透明（此图是为了绘制边框）
+            gun = Button(675,300,gunimage,1) # 加载按钮（Button类的定义在sprites.py)
+            pygame.mixer.music.load(BGM) # 加载背景音乐（BGM）
+            liveplayermusic = pygame.mixer.Sound(LIVEPLAYER) # 玩家被击中时的音效
+            livedealermusic = pygame.mixer.Sound(LIVEDEALER) # 恶魔被击中时的音效
+            blankmusic = pygame.mixer.Sound(BLANKMUSIC) # 空弹发射时的音效
+            shootlocation.center = (700,300) # 设置恶魔射击时的位置
+            text = pygame.font.Font(FONT,75) # 设定字体
+            nametext = text.render("Enter name:",False,WHITE) # 用字体生成文字
+            playerlose = text.render("dealer win!",False,WHITE) # 用字体生成文字
+            loseorwinlocation = playerlose.get_rect()
+            loseorwinlocation.center = (700,425)
+            nametextlocation = nametext.get_rect()
+            nametextlocation.center = (700,100)
+            shootdealer = Button(700,75,text.render("DEALER",False,WHITE),1)
+            dealerturntext = text.render("dealer's turn",False,WHITE)
+            buttons = []
+            name = ""
+            for i in range(26):buttons.append(Button(50*(i+1),700,pygame.image.load(f"assets/{LETTERS[i]}.png")))
+            delete = Button(350,760,pygame.image.load(DELETE))
+            enter = Button(800,760,pygame.image.load(ENTER))
+            # 以下是一些控制变量
+            naming = True # 正在命名
+            playerturn = False # 玩家回合
+            dealerturn = False # 恶魔回合
+            choosing = False
+            drawingbuckshots = False
+            wasd = int(0)
+            turn = [0,0]
+            dealer = Dealer(2)
+            player = Player(2,name)
+            # 以下是游戏主循环
+            pygame.mixer.music.play(-1)
+            while True:
+                for event in pygame.event.get():
+                    if event.type == pygame.QUIT:
+                        raise SystemExit
+                screen.blit(background,(0,0))
+                if not player.gethealth():
+                    screen.blit(playerlose,loseorwinlocation)
+                    pygame.display.update()
+                    sleep(3)
                     raise SystemExit
-                else:
-                    dealer = Dealer(health[turn[0]])
-                    player = Player(health[turn[0]],name)
-            try:buckshot[0]
-            except:
-                if turn[0] < 3:
-                    buckshot = buckshots[turn[0]][turn[1]]
-                    turn[1] += 1
-                if not naming:
-                    playerturn = dealerturn = False
-                    drawingbuckshots = True
-            if naming:
-                screen.blit(nametext,nametextlocation)
-                for i in buttons: 
-                    if i.run(screen):
-                        name += (LETTERS[buttons.index(i)])
-                if delete.run(screen):
-                    name = name[:-1]
-                if enter.run(screen):
-                    naming = False
-                    drawingbuckshots = True
-                    shootyou = Button(700,700,text.render(name,False,WHITE),1)
-                    playerwin = text.render(f"{name} win!",False,WHITE)
-                    player.setname(name)
-                tmpnametext = text.render(name,False,WHITE)
-                tmpnametextlocation = tmpnametext.get_rect()
-                tmpnametextlocation.center = (700,400)
-                screen.blit(tmpnametext,tmpnametextlocation)
-            elif playerturn:
-                for i in range(player.gethealth()):
-                    chargelocation.bottomleft = (0,850-50*i)
-                    screen.blit(charge,chargelocation)
-                for i in range(dealer.gethealth()):
-                    chargelocation.topleft = (0,0+50*i)
-                    screen.blit(charge,chargelocation)
-                if gun.run(screen):
-                    playerturn = False
-                    choosing = True
-            elif dealerturn:
-                screen.blit(dealerturntext,nametextlocation)
-                for i in range(player.gethealth()):
-                    chargelocation.bottomleft = (0,850-50*i)
-                    screen.blit(charge,chargelocation)
-                for i in range(dealer.gethealth()):
-                    chargelocation.topleft = (0,0+50*i)
-                    screen.blit(charge,chargelocation)
-                if dealer.shoot() == 0:
-                    print("dealer shooting himself!")
-                    screen.blit(dealershootself,shootlocation)
-                    if buckshot[0]:
-                        livedealermusic.play()
-                        dealer.hurt()
-                        dealerturn = False
-                        playerturn = True
+                if not dealer.gethealth():
+                    turn[1] = 0
+                    turn[0] += 1
+                    del buckshot
+                    screen.blit(playerwin,loseorwinlocation)
+                    pygame.display.update()
+                    sleep(3)
+                    if turn[0] == 3:
+                        raise SystemExit
                     else:
-                        blankmusic.play()
-                else:
-                    print(f"dealer shooting {name}")
-                    screen.blit(dealershootplayer,shootlocation)
-                    if buckshot[0]:
-                        liveplayermusic.play()
-                        player.hurt()
-                    else:
-                        blankmusic.play()
-                    dealerturn = False
-                    playerturn = True
-                del buckshot[0]
-                pygame.display.update()
-                sleep(2)
-            elif choosing:
-                for i in range(player.gethealth()):
-                    chargelocation.bottomleft = (0,850-50*i)
-                    screen.blit(charge,chargelocation)
-                for i in range(dealer.gethealth()):
-                    chargelocation.topleft = (0,0+50*i)
-                    screen.blit(charge,chargelocation)
-                if shootdealer.run(screen):
-                    print(f"{name} shooting dealer!")
-                    choosing = False
-                    dealerturn = True
-                    if buckshot[0] == 0:
-                        blankmusic.play()
+                        dealer = Dealer(health[turn[0]])
+                        player = Player(health[turn[0]],name)
+                try:buckshot[0]
+                except:
+                    if turn[0] < 3:
+                        buckshot = buckshots[turn[0]][turn[1]]
+                        turn[1] += 1
+                    if not naming:
+                        playerturn = dealerturn = False
+                        drawingbuckshots = True
+                if naming:
+                    screen.blit(nametext,nametextlocation)
+                    for i in buttons: 
+                        if i.run(screen):
+                            name += (LETTERS[buttons.index(i)])
+                    if delete.run(screen):
+                        name = name[:-1]
+                    if enter.run(screen):
+                        naming = False
+                        drawingbuckshots = True
+                        shootyou = Button(700,700,text.render(name,False,WHITE),1)
+                        playerwin = text.render(f"{name} win!",False,WHITE)
+                        player.setname(name)
+                    tmpnametext = text.render(name,False,WHITE)
+                    tmpnametextlocation = tmpnametext.get_rect()
+                    tmpnametextlocation.center = (700,400)
+                    screen.blit(tmpnametext,tmpnametextlocation)
+                elif playerturn:
+                    for i in range(player.gethealth()):
+                        chargelocation.bottomleft = (0,850-50*i)
+                        screen.blit(charge,chargelocation)
+                    for i in range(dealer.gethealth()):
+                        chargelocation.topleft = (0,0+50*i)
+                        screen.blit(charge,chargelocation)
+                    if gun.run(screen):
+                        playerturn = False
+                        choosing = True
+                elif dealerturn:
+                    screen.blit(dealerturntext,nametextlocation)
+                    for i in range(player.gethealth()):
+                        chargelocation.bottomleft = (0,850-50*i)
+                        screen.blit(charge,chargelocation)
+                    for i in range(dealer.gethealth()):
+                        chargelocation.topleft = (0,0+50*i)
+                        screen.blit(charge,chargelocation)
+                    if dealer.shoot() == 0:
+                        print("dealer shooting himself!")
+                        screen.blit(dealershootself,shootlocation)
+                        if buckshot[0]:
+                            livedealermusic.play()
+                            dealer.hurt()
+                            dealerturn = False
+                            playerturn = True
+                        else:
+                            blankmusic.play()
                     else:
-                        livedealermusic.play()
-                        dealer.hurt()
+                        print(f"dealer shooting {name}")
+                        screen.blit(dealershootplayer,shootlocation)
+                        if buckshot[0]:
+                            liveplayermusic.play()
+                            player.hurt()
+                        else:
+                            blankmusic.play()
+                        dealerturn = False
+                        playerturn = True
                     del buckshot[0]
+                    pygame.display.update()
                     sleep(2)
-                elif shootyou.run(screen):
-                    print(f"{name} shooting himself!")
-                    choosing = False
-                    if buckshot[0] == 0:
-                        blankmusic.play()
-                        playerturn = True
-                    else:
-                        liveplayermusic.play()
-                        player.hurt()
+                elif choosing:
+                    for i in range(player.gethealth()):
+                        chargelocation.bottomleft = (0,850-50*i)
+                        screen.blit(charge,chargelocation)
+                    for i in range(dealer.gethealth()):
+                        chargelocation.topleft = (0,0+50*i)
+                        screen.blit(charge,chargelocation)
+                    if shootdealer.run(screen):
+                        print(f"{name} shooting dealer!")
+                        choosing = False
                         dealerturn = True
-                    del buckshot[0]
+                        if buckshot[0] == 0:
+                            blankmusic.play()
+                        else:
+                            livedealermusic.play()
+                            dealer.hurt()
+                        del buckshot[0]
+                        sleep(2)
+                    elif shootyou.run(screen):
+                        print(f"{name} shooting himself!")
+                        choosing = False
+                        if buckshot[0] == 0:
+                            blankmusic.play()
+                            playerturn = True
+                        else:
+                            liveplayermusic.play()
+                            player.hurt()
+                            dealerturn = True
+                        del buckshot[0]
+                        sleep(2)
+                elif drawingbuckshots:
+                    for en,b in enumerate(buckshot):
+                        buckshotlocation.topleft = (400+80 * en,400)
+                        if b:
+                            screen.blit(liveround,buckshotlocation)
+                        else:
+                            screen.blit(blank,buckshotlocation)
+                    pygame.display.update()
                     sleep(2)
-            elif drawingbuckshots:
-                for en,b in enumerate(buckshot):
-                    buckshotlocation.topleft = (400+80 * en,400)
-                    if b:
-                        screen.blit(liveround,buckshotlocation)
-                    else:
-                        screen.blit(blank,buckshotlocation)
+                    drawingbuckshots = False
+                    playerturn = True
+                    shuffle(buckshot)
+                else:
+                    raise TypeError("Nothing is Running!!!")
                 pygame.display.update()
-                sleep(2)
-                drawingbuckshots = False
-                playerturn = True
-                shuffle(buckshot)
-            else:
-                raise TypeError("Nothing is Running!!!")
-            pygame.display.update()
-            clock.tick(FPS)
-    else:
-        name = input("你的名字：") # 输入名字
-        for j in range(3): # 三个回合
-            dealer = Dealer(health[j]) # 恶魔初始化
-            player = Player(health[j],name) # 玩家初始化
-            for i in range(len(buckshots[j])): # 每一小轮
-                buckshot = buckshots[j][i] # 初始化本轮子弹
-                buckshotcount = [0,0] #子弹计数
-                for k in buckshot: # 实弹
-                    if k:buckshotcount[0]+=1
-                for k in buckshot: # 空弹
-                    if k == 0:buckshotcount[1]+=1
-                next = 0 # 下一轮
-                shuffle(buckshot) # 打乱子弹顺序
-                print(f"{buckshotcount[0]}发实弹，{buckshotcount[1]}发空弹") # 打印子弹提示
-                for i in range(len(buckshot)): #
-                    print(f"恶魔血量:{dealer.gethealth()} {name}的血量:{player.gethealth()}")
-                    if next == 0:
-                        if player.shoot():
-                            if buckshot[i]:
-                                print("砰！！！")
-                                dealer.hurt() # 受伤
-                            else:
-                                print("咔......")
-                            next = 1
-                        else:
-                            if buckshot[i]:
-                                print("砰！！！")
-                                player.hurt()
+                clock.tick(FPS)
+        else:
+            name = input("你的名字：") # 输入名字
+            for j in range(3): # 三个回合
+                dealer = Dealer(health[j]) # 恶魔初始化
+                player = Player(health[j],name) # 玩家初始化
+                for i in range(len(buckshots[j])): # 每一小轮
+                    buckshot = buckshots[j][i] # 初始化本轮子弹
+                    buckshotcount = [0,0] #子弹计数
+                    for k in buckshot: # 实弹
+                        if k:buckshotcount[0]+=1
+                    for k in buckshot: # 空弹
+                        if k == 0:buckshotcount[1]+=1
+                    next = 0 # 下一轮
+                    shuffle(buckshot) # 打乱子弹顺序
+                    print(f"{buckshotcount[0]}发实弹，{buckshotcount[1]}发空弹") # 打印子弹提示
+                    for i in range(len(buckshot)): #
+                        print(f"恶魔血量:{dealer.gethealth()} {name}的血量:{player.gethealth()}")
+                        if next == 0:
+                            if player.shoot():
+                                if buckshot[i]:
+                                    print("砰！！！")
+                                    dealer.hurt() # 受伤
+                                else:
+                                    print("咔......")
                                 next = 1
                             else:
-                                print("咔......")
-                    else:
-                        if dealer.shoot():
-                            print(f"恶魔选择向{name}开枪！！！")
-                            if buckshot[i]:
-                                print("砰！！！")
-                                player.hurt()
-                            else:
-                                print("咔......")
-                            next = 0
+                                if buckshot[i]:
+                                    print("砰！！！")
+                                    player.hurt()
+                                    next = 1
+                                else:
+                                    print("咔......")
                         else:
-                            print("恶魔选择向自己开枪......")
-                            if buckshot[i]:
-                                print("砰！！！")
-                                dealer.hurt()
+                            if dealer.shoot():
+                                print(f"恶魔选择向{name}开枪！！！")
+                                if buckshot[i]:
+                                    print("砰！！！")
+                                    player.hurt()
+                                else:
+                                    print("咔......")
                                 next = 0
                             else:
-                                print("咔......")
-                    if dealer.gethealth() == 0 or player.gethealth() == 0:exit()
-                    sleep(1.5)
-            del dealer
-            del player
-except KeyboardInterrupt:
-    print("\n检测到^C")
-    exit()
-except SystemExit:pass
-except:
-    print("抱歉，我们检测到了一个错误，这可能不是您造成的，但您无法继续进行游戏了")
-    print("错误信息：")
-    print_exc()
-print("游戏结束!")
-print("感谢您的游玩!")
-print("名称:Buckshot Roulette（恶魔轮盘赌）")
-print("版本：1.0")
-print("LevoLet Inc.")
+                                print("恶魔选择向自己开枪......")
+                                if buckshot[i]:
+                                    print("砰！！！")
+                                    dealer.hurt()
+                                    next = 0
+                                else:
+                                    print("咔......")
+                        if dealer.gethealth() == 0 or player.gethealth() == 0:exit()
+                        sleep(1.5)
+                del dealer
+                del player
+    except KeyboardInterrupt:
+        print("\n检测到^C")
+        exit()
+    except SystemExit:pass
+    except:
+        print("抱歉，我们检测到了一个错误，这可能不是您造成的，但您无法继续进行游戏了")
+        print("错误信息：")
+        print_exc()
+    print("游戏结束!")
+    print("感谢您的游玩!")
+    print("名称:Buckshot Roulette（恶魔轮盘赌）")
+    print("版本：1.0")
+    print("LevoLet Inc.")
```

### Comparing `bulletroulette-1.0/bulletroulette/sprites.py` & `bulletroulette-1.0.2/bulletroulette/sprites.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# 此文件用于声明用于pygame的类（不必须，但使用窗口模式时需要）
+# 此文件用于声明用于pygame的类
 import pygame
-from data import *
+from bulletroulette.data import *
 
 class Button:
     def __init__(self,x,y,image,mode = 0):
         self.image = image
         self.location = self.image.get_rect()
         if mode == 0:
             self.location.topleft = (x,y)
```

### Comparing `bulletroulette-1.0/bulletroulette.egg-info/PKG-INFO` & `bulletroulette-1.0.2/bulletroulette.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulletroulette
-Version: 1.0
+Version: 1.0.2
 Summary: 模仿steam游戏“恶魔轮盘”，目前没有提供开发接口（只能单纯玩）
 Home-page: https://github.com/BinaryGuo/Buckshot_Roulette
 Author: GQX
 Author-email: kill114514251@outlook.com
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries :: pygame
```

### Comparing `bulletroulette-1.0/setup.py` & `bulletroulette-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="bulletroulette",  # 模块名称
-    version="1.0",  # 当前版本
+    version="1.0.2",  # 当前版本
     author="GQX",  # 作者
     author_email="kill114514251@outlook.com",  # 作者邮箱
     description="模仿steam游戏“恶魔轮盘”，目前没有提供开发接口（只能单纯玩）",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     url="https://github.com/BinaryGuo/Buckshot_Roulette",  # 模块github地址
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
```

