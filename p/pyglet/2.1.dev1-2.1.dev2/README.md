# Comparing `tmp/pyglet-2.1.dev1.tar.gz` & `tmp/pyglet-2.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglet-2.1.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyglet-2.1.dev2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyglet-2.1.dev1.tar` & `pyglet-2.1.dev2.tar`

### file list

```diff
@@ -1,214 +1,775 @@
--rw-r--r--   0        0        0     1546 2024-02-28 05:05:21.210710 pyglet-2.1.dev1/LICENSE
--rw-r--r--   0        0        0     7520 2024-02-29 01:38:03.790142 pyglet-2.1.dev1/README.md
--rw-r--r--   0        0        0    12126 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/__init__.py
--rw-r--r--   0        0        0      507 2024-04-02 05:14:53.599283 pyglet-2.1.dev1/pyglet/__init__.pyi
--rw-r--r--   0        0        0     2875 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/app/__init__.py
--rw-r--r--   0        0        0    11064 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/app/base.py
--rw-r--r--   0        0        0     9228 2024-03-08 00:58:25.028785 pyglet-2.1.dev1/pyglet/app/cocoa.py
--rw-r--r--   0        0        0     4325 2024-02-28 05:05:21.230711 pyglet-2.1.dev1/pyglet/app/win32.py
--rw-r--r--   0        0        0     2543 2024-02-28 05:05:21.230711 pyglet-2.1.dev1/pyglet/app/xlib.py
--rw-r--r--   0        0        0    21640 2024-02-28 05:05:21.230711 pyglet-2.1.dev1/pyglet/clock.py
--rw-r--r--   0        0        0      606 2024-04-02 05:14:53.599283 pyglet-2.1.dev1/pyglet/customtypes.py
--rwxr-xr-x   0        0        0     3093 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/display/__init__.py
--rwxr-xr-x   0        0        0    10500 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/display/base.py
--rw-r--r--   0        0        0     5559 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/display/cocoa.py
--rw-r--r--   0        0        0     2152 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/display/headless.py
--rwxr-xr-x   0        0        0     4774 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/display/win32.py
--rw-r--r--   0        0        0     9210 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/display/xlib.py
--rw-r--r--   0        0        0     5654 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/display/xlib_vidmoderestore.py
--rw-r--r--   0        0        0    17272 2024-02-28 05:05:21.230711 pyglet-2.1.dev1/pyglet/event.py
--rw-r--r--   0        0        0      221 2024-02-28 05:05:21.230711 pyglet-2.1.dev1/pyglet/experimental/README.md
--rw-r--r--   0        0        0    24495 2024-02-28 05:05:21.230711 pyglet-2.1.dev1/pyglet/experimental/geoshader_sprite.py
--rw-r--r--   0        0        0     6260 2024-02-28 05:05:21.230711 pyglet-2.1.dev1/pyglet/experimental/hidraw.py
--rw-r--r--   0        0        0     7680 2024-02-28 05:05:21.230711 pyglet-2.1.dev1/pyglet/experimental/net.py
--rw-r--r--   0        0        0      128 2024-02-28 05:05:21.234044 pyglet-2.1.dev1/pyglet/extlibs/__init__.py
--rw-r--r--   0        0        0    81404 2024-02-28 05:05:21.234044 pyglet-2.1.dev1/pyglet/extlibs/png.py
--rw-r--r--   0        0        0     8373 2024-04-02 05:14:53.599283 pyglet-2.1.dev1/pyglet/font/__init__.py
--rw-r--r--   0        0        0    13521 2024-02-28 05:05:21.234044 pyglet-2.1.dev1/pyglet/font/base.py
--rw-r--r--   0        0        0    95230 2024-02-28 05:05:21.234044 pyglet-2.1.dev1/pyglet/font/directwrite.py
--rw-r--r--   0        0        0     9763 2024-02-28 05:05:21.234044 pyglet-2.1.dev1/pyglet/font/fontconfig.py
--rw-r--r--   0        0        0    12212 2024-02-28 05:05:21.234044 pyglet-2.1.dev1/pyglet/font/freetype.py
--rw-r--r--   0        0        0    15642 2024-02-28 05:05:21.234044 pyglet-2.1.dev1/pyglet/font/freetype_lib.py
--rw-r--r--   0        0        0    12533 2024-02-28 05:05:21.234044 pyglet-2.1.dev1/pyglet/font/quartz.py
--rw-r--r--   0        0        0    23839 2024-02-28 05:05:21.234044 pyglet-2.1.dev1/pyglet/font/ttf.py
--rw-r--r--   0        0        0     6569 2024-03-08 00:58:25.028785 pyglet-2.1.dev1/pyglet/font/user.py
--rw-r--r--   0        0        0    16227 2024-03-08 00:58:25.028785 pyglet-2.1.dev1/pyglet/font/win32.py
--rw-r--r--   0        0        0     5407 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/gl/__init__.py
--rw-r--r--   0        0        0    26670 2024-02-28 05:05:21.234044 pyglet-2.1.dev1/pyglet/gl/agl.py
--rwxr-xr-x   0        0        0    17746 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/gl/base.py
--rw-r--r--   0        0        0    10601 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/gl/cocoa.py
--rw-r--r--   0        0        0   212567 2024-02-28 05:05:21.234044 pyglet-2.1.dev1/pyglet/gl/gl.py
--rw-r--r--   0        0        0   277237 2024-02-28 05:05:21.234044 pyglet-2.1.dev1/pyglet/gl/gl_compat.py
--rw-r--r--   0        0        0     6513 2024-02-28 05:05:21.234044 pyglet-2.1.dev1/pyglet/gl/gl_info.py
--rw-r--r--   0        0        0    29235 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/gl/glx.py
--rw-r--r--   0        0        0     3565 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/gl/glx_info.py
--rw-r--r--   0        0        0    50608 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/gl/glxext_arb.py
--rw-r--r--   0        0        0      261 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/gl/glxext_mesa.py
--rw-r--r--   0        0        0    41435 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/gl/glxext_nv.py
--rw-r--r--   0        0        0     5224 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/gl/headless.py
--rw-r--r--   0        0        0     3405 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/gl/lib.py
--rw-r--r--   0        0        0      902 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/gl/lib_agl.py
--rw-r--r--   0        0        0     1408 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/gl/lib_glx.py
--rw-r--r--   0        0        0     2910 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/gl/lib_wgl.py
--rwxr-xr-x   0        0        0    16109 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/gl/wgl.py
--rwxr-xr-x   0        0        0      954 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/gl/wgl_info.py
--rw-r--r--   0        0        0    70293 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/gl/wglext_arb.py
--rw-r--r--   0        0        0    69927 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/gl/wglext_nv.py
--rwxr-xr-x   0        0        0     9223 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/gl/win32.py
--rw-r--r--   0        0        0     8652 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/gl/xlib.py
--rw-r--r--   0        0        0    20565 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/graphics/__init__.py
--rw-r--r--   0        0        0    12604 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/graphics/allocation.py
--rw-r--r--   0        0        0    44701 2024-04-02 05:14:53.599283 pyglet-2.1.dev1/pyglet/graphics/shader.py
--rw-r--r--   0        0        0     1105 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/graphics/vertexarray.py
--rw-r--r--   0        0        0    12807 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/graphics/vertexbuffer.py
--rw-r--r--   0        0        0    19779 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/graphics/vertexdomain.py
--rw-r--r--   0        0        0       44 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/gui/__init__.py
--rw-r--r--   0        0        0     6862 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/gui/frame.py
--rw-r--r--   0        0        0    18674 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/gui/widgets.py
--rw-r--r--   0        0        0    76136 2024-04-02 05:14:53.599283 pyglet-2.1.dev1/pyglet/image/__init__.py
--rw-r--r--   0        0        0     6413 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/image/animation.py
--rw-r--r--   0        0        0    10284 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/image/atlas.py
--rw-r--r--   0        0        0     8488 2024-04-02 05:14:53.599283 pyglet-2.1.dev1/pyglet/image/buffer.py
--rw-r--r--   0        0        0     6498 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/image/codecs/__init__.py
--rw-r--r--   0        0        0    10642 2024-02-28 05:05:21.237378 pyglet-2.1.dev1/pyglet/image/codecs/bmp.py
--rw-r--r--   0        0        0     5668 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/image/codecs/dds.py
--rw-r--r--   0        0        0    11012 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/image/codecs/gdiplus.py
--rw-r--r--   0        0        0     8939 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/image/codecs/gdkpixbuf2.py
--rw-r--r--   0        0        0     3571 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/image/codecs/gif.py
--rw-r--r--   0        0        0     2592 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/image/codecs/pil.py
--rw-r--r--   0        0        0     2081 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/image/codecs/png.py
--rw-r--r--   0        0        0     4708 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/image/codecs/quartz.py
--rw-r--r--   0        0        0    12392 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/image/codecs/s3tc.py
--rw-r--r--   0        0        0    22368 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/image/codecs/wic.py
--rw-r--r--   0        0        0     5835 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/info.py
--rw-r--r--   0        0        0     6252 2024-04-02 05:16:19.531061 pyglet-2.1.dev1/pyglet/input/__init__.py
--rw-r--r--   0        0        0    41133 2024-04-02 05:16:19.534395 pyglet-2.1.dev1/pyglet/input/base.py
--rw-r--r--   0        0        0     5623 2024-04-02 05:16:19.534395 pyglet-2.1.dev1/pyglet/input/controller.py
--rw-r--r--   0        0        0   217906 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/input/controller_db.py
--rw-r--r--   0        0        0      391 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/input/linux/__init__.py
--rw-r--r--   0        0        0    19502 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/input/linux/evdev.py
--rw-r--r--   0        0        0     9789 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/input/linux/evdev_constants.py
--rw-r--r--   0        0        0    10993 2024-04-02 05:16:19.534395 pyglet-2.1.dev1/pyglet/input/linux/x11_xinput.py
--rw-r--r--   0        0        0     3007 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/input/linux/x11_xinput_tablet.py
--rw-r--r--   0        0        0      348 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/input/macos/__init__.py
--rw-r--r--   0        0        0    24468 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/input/macos/darwin_hid.py
--rw-r--r--   0        0        0     4222 2024-03-08 00:58:25.028785 pyglet-2.1.dev1/pyglet/input/win32/__init__.py
--rw-r--r--   0        0        0    16928 2024-04-02 05:16:19.534395 pyglet-2.1.dev1/pyglet/input/win32/directinput.py
--rw-r--r--   0        0        0    14512 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/input/win32/wintab.py
--rw-r--r--   0        0        0    21397 2024-04-02 05:16:19.534395 pyglet-2.1.dev1/pyglet/input/win32/xinput.py
--rw-r--r--   0        0        0    10952 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/lib.py
--rw-r--r--   0        0        0        1 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/libs/__init__.py
--rw-r--r--   0        0        0       23 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/libs/darwin/__init__.py
--rw-r--r--   0        0        0     1798 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/libs/darwin/cocoapy/__init__.py
--rw-r--r--   0        0        0    23244 2024-04-02 05:16:19.534395 pyglet-2.1.dev1/pyglet/libs/darwin/cocoapy/cocoalibs.py
--rw-r--r--   0        0        0     2629 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/libs/darwin/cocoapy/cocoatypes.py
--rw-r--r--   0        0        0    56271 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/libs/darwin/cocoapy/runtime.py
--rw-r--r--   0        0        0     6964 2024-02-28 05:05:21.240711 pyglet-2.1.dev1/pyglet/libs/darwin/coreaudio.py
--rw-r--r--   0        0        0     5179 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/darwin/quartzkey.py
--rw-r--r--   0        0        0        0 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/egl/__init__.py
--rw-r--r--   0        0        0    29920 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/egl/egl.py
--rw-r--r--   0        0        0      859 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/egl/eglext.py
--rw-r--r--   0        0        0      893 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/egl/lib.py
--rw-r--r--   0        0        0        0 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/wayland/__init__.py
--rw-r--r--   0        0        0    13388 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/wayland/gbm.py
--rw-r--r--   0        0        0    20657 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/wayland/xkbcommon.py
--rwxr-xr-x   0        0        0    14234 2024-04-02 05:16:19.534395 pyglet-2.1.dev1/pyglet/libs/win32/__init__.py
--rw-r--r--   0        0        0    15463 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/win32/com.py
--rw-r--r--   0        0        0   121260 2024-04-02 05:16:19.534395 pyglet-2.1.dev1/pyglet/libs/win32/constants.py
--rw-r--r--   0        0        0     1433 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/win32/context_managers.py
--rwxr-xr-x   0        0        0    10968 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/win32/dinput.py
--rwxr-xr-x   0        0        0    10901 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/win32/libwintab.py
--rw-r--r--   0        0        0    14851 2024-04-02 05:16:19.534395 pyglet-2.1.dev1/pyglet/libs/win32/types.py
--rw-r--r--   0        0        0     4667 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/win32/winkey.py
--rw-r--r--   0        0        0        1 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/x11/__init__.py
--rw-r--r--   0        0        0     1451 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/x11/cursorfont.py
--rw-r--r--   0        0        0    13531 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/x11/xf86vmode.py
--rw-r--r--   0        0        0     2182 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/x11/xinerama.py
--rw-r--r--   0        0        0    54556 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/x11/xinput.py
--rw-r--r--   0        0        0   183778 2024-04-02 05:16:19.534395 pyglet-2.1.dev1/pyglet/libs/x11/xlib.py
--rw-r--r--   0        0        0    15202 2024-02-28 05:05:21.244044 pyglet-2.1.dev1/pyglet/libs/x11/xsync.py
--rw-r--r--   0        0        0    34525 2024-04-02 05:16:19.534395 pyglet-2.1.dev1/pyglet/math.py
--rw-r--r--   0        0        0     3208 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/__init__.py
--rw-r--r--   0        0        0     1025 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/buffered_logger.py
--rw-r--r--   0        0        0     3308 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/codecs/__init__.py
--rw-r--r--   0        0        0    25186 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/codecs/base.py
--rw-r--r--   0        0        0     6805 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/codecs/coreaudio.py
--rw-r--r--   0        0        0    40899 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/codecs/ffmpeg.py
--rw-r--r--   0        0        0      201 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/codecs/ffmpeg_lib/__init__.py
--rw-r--r--   0        0        0     3314 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/codecs/ffmpeg_lib/compat.py
--rw-r--r--   0        0        0    15663 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/codecs/ffmpeg_lib/libavcodec.py
--rw-r--r--   0        0        0    10160 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/codecs/ffmpeg_lib/libavformat.py
--rw-r--r--   0        0        0     7169 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/codecs/ffmpeg_lib/libavutil.py
--rw-r--r--   0        0        0     1688 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/codecs/ffmpeg_lib/libswresample.py
--rw-r--r--   0        0        0     1501 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/codecs/ffmpeg_lib/libswscale.py
--rw-r--r--   0        0        0     9250 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/codecs/gstreamer.py
--rw-r--r--   0        0        0    17727 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/codecs/pyogg.py
--rw-r--r--   0        0        0     3566 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/codecs/wave.py
--rw-r--r--   0        0        0    33706 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/codecs/wmf.py
--rw-r--r--   0        0        0      773 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/devices/__init__.py
--rw-r--r--   0        0        0     3218 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/devices/base.py
--rw-r--r--   0        0        0    12409 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/devices/win32.py
--rw-r--r--   0        0        0     2463 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/drivers/__init__.py
--rw-r--r--   0        0        0    15352 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/drivers/base.py
--rw-r--r--   0        0        0      251 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/drivers/directsound/__init__.py
--rw-r--r--   0        0        0    12133 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/drivers/directsound/adaptation.py
--rw-r--r--   0        0        0      325 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/drivers/directsound/exceptions.py
--rw-r--r--   0        0        0    12655 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/drivers/directsound/interface.py
--rw-r--r--   0        0        0    12705 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/drivers/directsound/lib_dsound.py
--rw-r--r--   0        0        0     2438 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/drivers/listener.py
--rw-r--r--   0        0        0      324 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/drivers/openal/__init__.py
--rw-r--r--   0        0        0     9226 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/drivers/openal/adaptation.py
--rw-r--r--   0        0        0    16582 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/drivers/openal/interface.py
--rw-r--r--   0        0        0    10833 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/drivers/openal/lib_alc.py
--rw-r--r--   0        0        0    26707 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/drivers/openal/lib_openal.py
--rw-r--r--   0        0        0      244 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/drivers/pulse/__init__.py
--rw-r--r--   0        0        0    14112 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/drivers/pulse/adaptation.py
--rw-r--r--   0        0        0    26864 2024-02-28 05:05:21.247378 pyglet-2.1.dev1/pyglet/media/drivers/pulse/interface.py
--rw-r--r--   0        0        0   125621 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/media/drivers/pulse/lib_pulseaudio.py
--rw-r--r--   0        0        0      127 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/media/drivers/silent/__init__.py
--rw-r--r--   0        0        0     4080 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/media/drivers/silent/adaptation.py
--rw-r--r--   0        0        0      128 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/media/drivers/xaudio2/__init__.py
--rw-r--r--   0        0        0    12769 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/media/drivers/xaudio2/adaptation.py
--rw-r--r--   0        0        0    25003 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/media/drivers/xaudio2/interface.py
--rw-r--r--   0        0        0    27709 2024-04-02 05:14:53.599283 pyglet-2.1.dev1/pyglet/media/drivers/xaudio2/lib_xaudio2.py
--rw-r--r--   0        0        0      152 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/media/exceptions.py
--rw-r--r--   0        0        0    10798 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/media/instrumentation.py
--rw-r--r--   0        0        0    23852 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/media/player.py
--rw-r--r--   0        0        0     3768 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/media/player_worker_thread.py
--rw-r--r--   0        0        0    11814 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/media/synthesis.py
--rw-r--r--   0        0        0     9359 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/model/__init__.py
--rw-r--r--   0        0        0     1502 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/model/codecs/__init__.py
--rw-r--r--   0        0        0     7303 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/model/codecs/gltf.py
--rw-r--r--   0        0        0     7683 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/model/codecs/obj.py
--rw-r--r--   0        0        0    30029 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/resource.py
--rw-r--r--   0        0        0    73958 2024-04-02 05:16:19.537728 pyglet-2.1.dev1/pyglet/shapes.py
--rw-r--r--   0        0        0    26390 2024-04-02 05:16:19.537728 pyglet-2.1.dev1/pyglet/sprite.py
--rw-r--r--   0        0        0    17920 2024-04-02 05:16:19.537728 pyglet-2.1.dev1/pyglet/text/__init__.py
--rw-r--r--   0        0        0    22076 2024-04-02 05:14:53.602617 pyglet-2.1.dev1/pyglet/text/caret.py
--rw-r--r--   0        0        0    24041 2024-04-02 05:14:53.602617 pyglet-2.1.dev1/pyglet/text/document.py
--rw-r--r--   0        0        0       48 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/text/formats/__init__.py
--rw-r--r--   0        0        0     2679 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/text/formats/attributed.py
--rw-r--r--   0        0        0    11551 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/text/formats/html.py
--rw-r--r--   0        0        0      264 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/text/formats/plaintext.py
--rw-r--r--   0        0        0    10726 2024-04-02 05:14:53.602617 pyglet-2.1.dev1/pyglet/text/formats/structured.py
--rw-r--r--   0        0        0     6142 2024-04-02 05:14:53.602617 pyglet-2.1.dev1/pyglet/text/layout/__init__.py
--rw-r--r--   0        0        0    74183 2024-04-02 05:16:19.537728 pyglet-2.1.dev1/pyglet/text/layout/base.py
--rw-r--r--   0        0        0    35365 2024-04-02 05:16:19.537728 pyglet-2.1.dev1/pyglet/text/layout/incremental.py
--rw-r--r--   0        0        0     9310 2024-04-02 05:16:19.537728 pyglet-2.1.dev1/pyglet/text/layout/scrolling.py
--rw-r--r--   0        0        0    12514 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/text/runlist.py
--rw-r--r--   0        0        0     8646 2024-02-28 05:05:21.250711 pyglet-2.1.dev1/pyglet/util.py
--rw-r--r--   0        0        0    68026 2024-04-02 05:16:19.537728 pyglet-2.1.dev1/pyglet/window/__init__.py
--rw-r--r--   0        0        0    26197 2024-04-02 05:16:19.537728 pyglet-2.1.dev1/pyglet/window/cocoa/__init__.py
--rw-r--r--   0        0        0     5866 2024-04-02 05:16:19.537728 pyglet-2.1.dev1/pyglet/window/cocoa/pyglet_delegate.py
--rw-r--r--   0        0        0     6677 2024-03-08 00:58:25.028785 pyglet-2.1.dev1/pyglet/window/cocoa/pyglet_textview.py
--rw-r--r--   0        0        0    14775 2024-02-28 05:05:21.254045 pyglet-2.1.dev1/pyglet/window/cocoa/pyglet_view.py
--rw-r--r--   0        0        0     3284 2024-02-28 05:05:21.254045 pyglet-2.1.dev1/pyglet/window/cocoa/pyglet_window.py
--rw-r--r--   0        0        0      691 2024-02-28 05:05:21.254045 pyglet-2.1.dev1/pyglet/window/cocoa/systemcursor.py
--rw-r--r--   0        0        0     3830 2024-02-28 05:05:21.254045 pyglet-2.1.dev1/pyglet/window/event.py
--rw-r--r--   0        0        0     2776 2024-04-02 05:16:19.537728 pyglet-2.1.dev1/pyglet/window/headless/__init__.py
--rw-r--r--   0        0        0     9566 2024-02-28 05:05:21.254045 pyglet-2.1.dev1/pyglet/window/key.py
--rw-r--r--   0        0        0     2324 2024-02-28 05:05:21.254045 pyglet-2.1.dev1/pyglet/window/mouse.py
--rw-r--r--   0        0        0    50394 2024-04-02 05:16:19.537728 pyglet-2.1.dev1/pyglet/window/win32/__init__.py
--rw-r--r--   0        0        0    66785 2024-04-02 05:16:19.537728 pyglet-2.1.dev1/pyglet/window/xlib/__init__.py
--rw-r--r--   0        0        0      355 2024-02-28 05:05:21.254045 pyglet-2.1.dev1/pyproject.toml
--rw-r--r--   0        0        0     7809 1970-01-01 00:00:00.000000 pyglet-2.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0      166 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/.coveragerc
+-rw-r--r--   0        0        0      716 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      482 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0       95 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/.github/ISSUE_TEMPLATE/questions--or-other.md
+-rw-r--r--   0        0        0      837 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1977 2024-03-08 00:58:25.025452 pyglet-2.1.dev2/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0      594 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/.gitignore
+-rw-r--r--   0        0        0      266 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/.readthedocs.yml
+-rw-r--r--   0        0        0     1546 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/LICENSE
+-rw-r--r--   0        0        0      370 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/MANIFEST.in
+-rw-r--r--   0        0        0     7520 2024-02-29 01:38:03.790142 pyglet-2.1.dev2/README.md
+-rw-r--r--   0        0        0    43634 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/RELEASE_NOTES
+-rw-r--r--   0        0        0      516 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/contrib/aseprite_codec/README
+-rw-r--r--   0        0        0      571 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/contrib/aseprite_codec/asedemo.py
+-rw-r--r--   0        0        0    12536 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/contrib/aseprite_codec/aseprite.py
+-rw-r--r--   0        0        0     1570 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/contrib/aseprite_codec/running.ase
+-rw-r--r--   0        0        0    55873 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/contrib/logo3d/logo3d.jpg
+-rw-r--r--   0        0        0    88069 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/contrib/logo3d/logo3d.obj.zip
+-rw-r--r--   0        0        0   117880 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/contrib/logo3d/logo3d.wings
+-rw-r--r--   0        0        0    27940 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/contrib/qt_sprite_preview.py
+-rw-r--r--   0        0        0     3051 2024-04-13 23:03:26.295974 pyglet-2.1.dev2/contrib/scenemanager.py
+-rw-r--r--   0        0        0     2869 2024-04-13 23:03:26.295974 pyglet-2.1.dev2/contrib/toys/follow_mouse.py
+-rw-r--r--   0        0        0     5773 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/doc/Makefile
+-rw-r--r--   0        0        0     1629 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/doc/README.md
+-rw-r--r--   0        0        0     1150 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/doc/_static/favicon.ico
+-rw-r--r--   0        0        0    10844 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/doc/_static/logo.png
+-rw-r--r--   0        0        0    24723 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/doc/_static/logo5.svg
+-rw-r--r--   0        0        0     1500 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/doc/_static/relatedlogo.png
+-rw-r--r--   0        0        0    12042 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/doc/conf.py
+-rw-r--r--   0        0        0     1041 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/doc/external_resources.rst
+-rw-r--r--   0        0        0     3547 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/doc/index.rst
+-rw-r--r--   0        0        0     2516 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/doc/internal/contributing.rst
+-rwxr-xr-x   0        0        0     1100 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/doc/internal/dist.rst
+-rw-r--r--   0        0        0     7416 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/doc/internal/doc.rst
+-rw-r--r--   0        0        0     5027 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/doc/internal/generated.rst
+-rw-r--r--   0        0        0     2065 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/doc/internal/gl.rst
+-rw-r--r--   0        0        0    20027 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/doc/internal/media_logging_manual.rst
+-rw-r--r--   0        0        0    14652 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/doc/internal/media_manual.rst
+-rw-r--r--   0        0        0     5121 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/doc/internal/testing.rst
+-rw-r--r--   0        0        0     4235 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/doc/internal/virtualenv.rst
+-rw-r--r--   0        0        0    59510 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/doc/internal/wraptypes-class.svg
+-rw-r--r--   0        0        0    14208 2024-02-28 05:05:21.210710 pyglet-2.1.dev2/doc/internal/wraptypes.rst
+-rw-r--r--   0        0        0     5402 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/make.bat
+-rw-r--r--   0        0        0      766 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/app.rst
+-rw-r--r--   0        0        0      249 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/canvas.rst
+-rw-r--r--   0        0        0       86 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/clock.rst
+-rw-r--r--   0        0        0       86 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/event.rst
+-rw-r--r--   0        0        0       83 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/font.rst
+-rw-r--r--   0        0        0      381 2024-04-13 23:03:26.295974 pyglet-2.1.dev2/doc/modules/gl.rst
+-rw-r--r--   0        0        0      128 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/graphics/allocation.rst
+-rw-r--r--   0        0        0      227 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/graphics/index.rst
+-rw-r--r--   0        0        0      115 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/graphics/shader.rst
+-rw-r--r--   0        0        0      134 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/graphics/vertexbuffer.rst
+-rw-r--r--   0        0        0      134 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/graphics/vertexdomain.rst
+-rw-r--r--   0        0        0      563 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/gui.rst
+-rw-r--r--   0        0        0      116 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/image/animation.rst
+-rw-r--r--   0        0        0      104 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/image/atlas.rst
+-rw-r--r--   0        0        0      107 2024-04-02 05:14:53.599283 pyglet-2.1.dev2/doc/modules/image/buffer.rst
+-rw-r--r--   0        0        0     2279 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/doc/modules/image/index.rst
+-rw-r--r--   0        0        0       83 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/info.rst
+-rw-r--r--   0        0        0     2142 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/input.rst
+-rw-r--r--   0        0        0       83 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/math.rst
+-rw-r--r--   0        0        0     2073 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/media.rst
+-rw-r--r--   0        0        0      116 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/media_synthesis.rst
+-rw-r--r--   0        0        0       62 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/pyglet.rst
+-rw-r--r--   0        0        0      788 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/resource.rst
+-rw-r--r--   0        0        0     1960 2024-03-08 00:58:25.028785 pyglet-2.1.dev2/doc/modules/shapes.rst
+-rw-r--r--   0        0        0      734 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/sprite.rst
+-rw-r--r--   0        0        0      101 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/text/caret.rst
+-rw-r--r--   0        0        0      110 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/text/document.rst
+-rw-r--r--   0        0        0      190 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/text/index.rst
+-rw-r--r--   0        0        0      104 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/text/layout.rst
+-rw-r--r--   0        0        0     4040 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/window.rst
+-rw-r--r--   0        0        0     5317 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/window_key.rst
+-rw-r--r--   0        0        0       91 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/modules/window_mouse.rst
+-rw-r--r--   0        0        0    19018 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/context.rst
+-rw-r--r--   0        0        0     5411 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/debug.rst
+-rw-r--r--   0        0        0     6167 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/eventloop.rst
+-rw-r--r--   0        0        0    11616 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/events.rst
+-rw-r--r--   0        0        0    45717 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/examplegame.rst
+-rw-r--r--   0        0        0     7662 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/gl.rst
+-rw-r--r--   0        0        0     6127 2024-04-02 05:14:53.599283 pyglet-2.1.dev2/doc/programming_guide/gui.rst
+-rw-r--r--   0        0        0    36633 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/doc/programming_guide/image.rst
+-rw-r--r--   0        0        0    16047 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/abstract_image.png
+-rw-r--r--   0        0        0    14389 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/abstract_image.svg
+-rw-r--r--   0        0        0    12844 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/buffer_image.png
+-rw-r--r--   0        0        0    10123 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/buffer_image.svg
+-rw-r--r--   0        0        0    37719 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/context_flow.png
+-rw-r--r--   0        0        0    23812 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/context_flow.svg
+-rw-r--r--   0        0        0      293 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_mac_crosshair.png
+-rw-r--r--   0        0        0      284 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_mac_default.png
+-rw-r--r--   0        0        0      574 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_mac_hand.png
+-rw-r--r--   0        0        0     1095 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_mac_no.png
+-rw-r--r--   0        0        0      231 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_mac_size_down.png
+-rw-r--r--   0        0        0      204 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_mac_size_left.png
+-rw-r--r--   0        0        0      257 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_mac_size_left_right.png
+-rw-r--r--   0        0        0      212 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_mac_size_right.png
+-rw-r--r--   0        0        0      232 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_mac_size_up.png
+-rw-r--r--   0        0        0      269 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_mac_size_up_down.png
+-rw-r--r--   0        0        0      337 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_mac_text.png
+-rw-r--r--   0        0        0      171 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_mac_wait.png
+-rw-r--r--   0        0        0      204 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_win_crosshair.png
+-rw-r--r--   0        0        0      279 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_win_default.png
+-rw-r--r--   0        0        0      285 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_win_hand.png
+-rw-r--r--   0        0        0      314 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_win_help.png
+-rw-r--r--   0        0        0      286 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_win_no.png
+-rw-r--r--   0        0        0      277 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_win_size.png
+-rw-r--r--   0        0        0      224 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_win_size_left_right.png
+-rw-r--r--   0        0        0      240 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_win_size_nesw.png
+-rw-r--r--   0        0        0      243 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_win_size_nwse.png
+-rw-r--r--   0        0        0      223 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_win_size_up_down.png
+-rw-r--r--   0        0        0      203 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_win_text.png
+-rw-r--r--   0        0        0      293 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_win_wait.png
+-rw-r--r--   0        0        0      354 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/cursor_win_wait_arrow.png
+-rw-r--r--   0        0        0     2797 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/explosion.png
+-rw-r--r--   0        0        0     7784 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/font_metrics.png
+-rw-r--r--   0        0        0     5744 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/font_metrics.svg
+-rw-r--r--   0        0        0    87562 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/image_classes.png
+-rw-r--r--   0        0        0    44024 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/image_classes.svg
+-rw-r--r--   0        0        0    21889 2024-02-28 05:05:21.214044 pyglet-2.1.dev2/doc/programming_guide/img/image_grid.png
+-rw-r--r--   0        0        0    25732 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/image_grid.svg
+-rw-r--r--   0        0        0    16277 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/image_sequence.png
+-rw-r--r--   0        0        0    11720 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/image_sequence.svg
+-rw-r--r--   0        0        0     4333 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/mouse_coordinates.png
+-rw-r--r--   0        0        0     8773 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/mouse_coordinates.svg
+-rw-r--r--   0        0        0    11699 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/screens.png
+-rw-r--r--   0        0        0    12266 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/screens.svg
+-rw-r--r--   0        0        0    16487 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/text_classes.png
+-rw-r--r--   0        0        0    13736 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/text_classes.svg
+-rw-r--r--   0        0        0     9298 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/window_location.png
+-rw-r--r--   0        0        0    10096 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/window_location.svg
+-rw-r--r--   0        0        0     4251 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/window_osx_borderless.png
+-rw-r--r--   0        0        0     8984 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/window_osx_default.png
+-rw-r--r--   0        0        0     8722 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/window_osx_dialog.png
+-rw-r--r--   0        0        0     7877 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/window_osx_tool.png
+-rw-r--r--   0        0        0     6607 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/window_xp_default.png
+-rw-r--r--   0        0        0     5797 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/window_xp_dialog.png
+-rw-r--r--   0        0        0    34485 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/window_xp_overlay.png
+-rw-r--r--   0        0        0     3817 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/window_xp_tool.png
+-rw-r--r--   0        0        0    35777 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/img/window_xp_transparent.png
+-rw-r--r--   0        0        0    16254 2024-04-13 23:03:26.295974 pyglet-2.1.dev2/doc/programming_guide/input.rst
+-rw-r--r--   0        0        0     1363 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/installation.rst
+-rw-r--r--   0        0        0    15078 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/keyboard.rst
+-rw-r--r--   0        0        0     2698 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/math.rst
+-rw-r--r--   0        0        0    28682 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/media.rst
+-rw-r--r--   0        0        0     6087 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/doc/programming_guide/migration.rst
+-rw-r--r--   0        0        0    11293 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/mouse.rst
+-rw-r--r--   0        0        0      844 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/options.rst
+-rw-r--r--   0        0        0     8244 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/quickstart.rst
+-rw-r--r--   0        0        0    22709 2024-04-02 05:14:53.599283 pyglet-2.1.dev2/doc/programming_guide/rendering.rst
+-rw-r--r--   0        0        0     9954 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/resources.rst
+-rw-r--r--   0        0        0     2747 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/shapes.rst
+-rw-r--r--   0        0        0    31438 2024-03-08 00:58:25.028785 pyglet-2.1.dev2/doc/programming_guide/text.rst
+-rw-r--r--   0        0        0     6313 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/time.rst
+-rw-r--r--   0        0        0    16288 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/programming_guide/windowing.rst
+-rw-r--r--   0        0        0       77 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/doc/requirements.txt
+-rw-r--r--   0        0        0      501 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/examples/clipboard.py
+-rw-r--r--   0        0        0     1224 2024-04-13 23:03:26.295974 pyglet-2.1.dev2/examples/dpi_scaled_window.py
+-rw-r--r--   0        0        0      696 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/events/events_key_state_handler.py
+-rw-r--r--   0        0        0     1169 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/events/register_event_type.py
+-rwxr-xr-x   0        0        0      357 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/events/window_events.py
+-rwxr-xr-x   0        0        0     1460 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/events/window_platform_event.py
+-rw-r--r--   0        0        0     6397 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/file_dialog.py
+-rw-r--r--   0        0        0     5321 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/resources/asteroid.png
+-rw-r--r--   0        0        0      327 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/resources/bullet.png
+-rw-r--r--   0        0        0    12680 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/resources/bullet.wav
+-rw-r--r--   0        0        0      662 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/resources/engine_flame.png
+-rw-r--r--   0        0        0     1435 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/resources/player.png
+-rw-r--r--   0        0        0      823 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/version1/asteroid.py
+-rw-r--r--   0        0        0       30 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/version1/game/__init__.py
+-rw-r--r--   0        0        0      936 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/version1/game/load.py
+-rw-r--r--   0        0        0      584 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/version1/game/resources.py
+-rw-r--r--   0        0        0     1249 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/version2/asteroid.py
+-rw-r--r--   0        0        0       38 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/version2/game/__init__.py
+-rw-r--r--   0        0        0     1563 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/version2/game/load.py
+-rw-r--r--   0        0        0     1102 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/version2/game/physicalobject.py
+-rw-r--r--   0        0        0     1555 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/version2/game/player.py
+-rw-r--r--   0        0        0      584 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/version2/game/resources.py
+-rw-r--r--   0        0        0     2120 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/version3/asteroid.py
+-rw-r--r--   0        0        0       38 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/version3/game/__init__.py
+-rw-r--r--   0        0        0     1390 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/version3/game/load.py
+-rw-r--r--   0        0        0     1772 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/version3/game/physicalobject.py
+-rw-r--r--   0        0        0     1865 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/version3/game/player.py
+-rw-r--r--   0        0        0      916 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/version3/game/resources.py
+-rw-r--r--   0        0        0      196 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/version3/game/util.py
+-rw-r--r--   0        0        0     2519 2024-02-28 05:05:21.217377 pyglet-2.1.dev2/examples/game/version4/asteroid.py
+-rw-r--r--   0        0        0       38 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/game/version4/game/__init__.py
+-rw-r--r--   0        0        0     1223 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/game/version4/game/asteroid.py
+-rw-r--r--   0        0        0      466 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/game/version4/game/bullet.py
+-rw-r--r--   0        0        0     1236 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/game/version4/game/load.py
+-rw-r--r--   0        0        0     2394 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/game/version4/game/physicalobject.py
+-rw-r--r--   0        0        0     3155 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/game/version4/game/player.py
+-rw-r--r--   0        0        0     1072 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/game/version4/game/resources.py
+-rw-r--r--   0        0        0      351 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/game/version4/game/util.py
+-rw-r--r--   0        0        0     4697 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/game/version5/asteroid.py
+-rw-r--r--   0        0        0       38 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/game/version5/game/__init__.py
+-rw-r--r--   0        0        0     1223 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/game/version5/game/asteroid.py
+-rw-r--r--   0        0        0      466 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/game/version5/game/bullet.py
+-rw-r--r--   0        0        0     1236 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/game/version5/game/load.py
+-rw-r--r--   0        0        0     2463 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/game/version5/game/physicalobject.py
+-rw-r--r--   0        0        0     3155 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/game/version5/game/player.py
+-rw-r--r--   0        0        0     1072 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/game/version5/game/resources.py
+-rw-r--r--   0        0        0      351 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/game/version5/game/util.py
+-rwxr-xr-x   0        0        0      767 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/graphics/image_convert.py
+-rwxr-xr-x   0        0        0     1077 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/graphics/image_display.py
+-rw-r--r--   0        0        0      222 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/gui/bar.png
+-rw-r--r--   0        0        0     3105 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/gui/button_hover.png
+-rw-r--r--   0        0        0     2953 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/examples/gui/button_pressed.png
+-rw-r--r--   0        0        0     2888 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/examples/gui/button_unpressed.png
+-rw-r--r--   0        0        0      449 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/gui/knob.png
+-rw-r--r--   0        0        0     2796 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/examples/gui/widgets.py
+-rw-r--r--   0        0        0      401 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/hello_world.py
+-rwxr-xr-x   0        0        0     1187 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/input/apple_remote.py
+-rw-r--r--   0        0        0     4892 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/examples/input/controller.py
+-rwxr-xr-x   0        0        0     1044 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/input/input.py
+-rwxr-xr-x   0        0        0     2062 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/input/joystick.py
+-rwxr-xr-x   0        0        0     1926 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/examples/input/tablet.py
+-rwxr-xr-x   0        0        0     2554 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/media/media_info.py
+-rwxr-xr-x   0        0        0    13853 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/media/media_player.py
+-rw-r--r--   0        0        0      366 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/media/noisy/README
+-rw-r--r--   0        0        0      996 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/media/noisy/ball.png
+-rw-r--r--   0        0        0     9424 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/media/noisy/ball.wav
+-rwxr-xr-x   0        0        0     2187 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/media/noisy/noisy.py
+-rw-r--r--   0        0        0     1157 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/media/soundspace/README
+-rw-r--r--   0        0        0     4523 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/media/soundspace/reader.py
+-rw-r--r--   0        0        0    96720 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/media/soundspace/res/bass.wav
+-rw-r--r--   0        0        0    48062 2024-02-28 05:05:21.220711 pyglet-2.1.dev2/examples/media/soundspace/res/drums.wav
+-rw-r--r--   0        0        0   139946 2024-02-28 05:05:21.224044 pyglet-2.1.dev2/examples/media/soundspace/res/guitar.wav
+-rw-r--r--   0        0        0   139946 2024-02-28 05:05:21.224044 pyglet-2.1.dev2/examples/media/soundspace/res/piano.wav
+-rw-r--r--   0        0        0      482 2024-02-28 05:05:21.224044 pyglet-2.1.dev2/examples/media/soundspace/res/space.txt
+-rw-r--r--   0        0        0    21717 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/examples/media/soundspace/soundspace.py
+-rw-r--r--   0        0        0     2671 2024-02-28 05:05:21.224044 pyglet-2.1.dev2/examples/media/synthesizer.py
+-rwxr-xr-x   0        0        0      704 2024-02-28 05:05:21.224044 pyglet-2.1.dev2/examples/media/video.py
+-rw-r--r--   0        0        0      251 2024-02-28 05:05:21.224044 pyglet-2.1.dev2/examples/model/box.mtl
+-rw-r--r--   0        0        0     1010 2024-02-28 05:05:21.224044 pyglet-2.1.dev2/examples/model/box.obj
+-rw-r--r--   0        0        0     5820 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/examples/model/fpscamera.py
+-rw-r--r--   0        0        0      199 2024-02-28 05:05:21.224044 pyglet-2.1.dev2/examples/model/logo3d.mtl
+-rw-r--r--   0        0        0   539412 2024-02-28 05:05:21.227377 pyglet-2.1.dev2/examples/model/logo3d.obj
+-rw-r--r--   0        0        0     1528 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/examples/model/model.py
+-rw-r--r--   0        0        0    17967 2024-02-28 05:05:21.227377 pyglet-2.1.dev2/examples/model/pyglet.png
+-rw-r--r--   0        0        0     1468 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/examples/opengl/compute_shader.py
+-rw-r--r--   0        0        0     2935 2024-02-28 05:05:21.227377 pyglet-2.1.dev2/examples/opengl/egl_context.py
+-rw-r--r--   0        0        0     4663 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/examples/opengl/minimal_shader.py
+-rwxr-xr-x   0        0        0     1066 2024-02-28 05:05:21.227377 pyglet-2.1.dev2/examples/opengl/opengl_context.py
+-rw-r--r--   0        0        0     3421 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/examples/opengl/opengl_core.py
+-rw-r--r--   0        0        0     2876 2024-02-28 05:05:21.227377 pyglet-2.1.dev2/examples/opengl/opengl_scissor.py
+-rw-r--r--   0        0        0     6575 2024-02-28 05:05:21.227377 pyglet-2.1.dev2/examples/opengl/pyglet.png
+-rwxr-xr-x   0        0        0     3986 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/examples/opengl/torus.py
+-rwxr-xr-x   0        0        0     1027 2024-02-28 05:05:21.227377 pyglet-2.1.dev2/examples/programming_guide/animation.py
+-rw-r--r--   0        0        0     7002 2024-02-28 05:05:21.227377 pyglet-2.1.dev2/examples/programming_guide/dinosaur.gif
+-rwxr-xr-x   0        0        0      718 2024-02-28 05:05:21.227377 pyglet-2.1.dev2/examples/programming_guide/events.py
+-rwxr-xr-x   0        0        0      401 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/examples/programming_guide/hello_world.py
+-rwxr-xr-x   0        0        0      269 2024-02-28 05:05:21.227377 pyglet-2.1.dev2/examples/programming_guide/image_viewer.py
+-rw-r--r--   0        0        0    43950 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/examples/programming_guide/kitten.jpg
+-rwxr-xr-x   0        0        0      573 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/examples/programming_guide/window_subclass.py
+-rw-r--r--   0        0        0    43950 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/examples/resources/kitten.jpg
+-rw-r--r--   0        0        0     6575 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/examples/resources/pyglet.png
+-rw-r--r--   0        0        0     3202 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/examples/shapes.py
+-rw-r--r--   0        0        0     2811 2024-04-02 05:14:53.599283 pyglet-2.1.dev2/examples/sprite/depth_sprite.py
+-rw-r--r--   0        0        0      809 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/examples/sprite/display_sprite.py
+-rw-r--r--   0        0        0     6088 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/examples/sprite/multi_texture_sprite.py
+-rw-r--r--   0        0        0     1511 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/examples/sprite/sprite_batching.py
+-rw-r--r--   0        0        0     2356 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/examples/text/advanced_font.py
+-rwxr-xr-x   0        0        0     1142 2024-04-02 05:14:53.599283 pyglet-2.1.dev2/examples/text/html_label.py
+-rw-r--r--   0        0        0     6575 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/examples/text/pyglet.png
+-rwxr-xr-x   0        0        0     4408 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/examples/text/text_input.py
+-rwxr-xr-x   0        0        0     1643 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/examples/timer.py
+-rw-r--r--   0        0        0     5012 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/examples/window/camera.py
+-rw-r--r--   0        0        0     5155 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/examples/window/camera_group.py
+-rwxr-xr-x   0        0        0     3970 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/examples/window/fixed_resolution.py
+-rw-r--r--   0        0        0     1134 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/examples/window/fps_change.py
+-rw-r--r--   0        0        0      656 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/examples/window/multiple_windows.py
+-rw-r--r--   0        0        0      436 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/examples/window/overlay_window.py
+-rw-r--r--   0        0        0      444 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/examples/window/transparent_window.py
+-rw-r--r--   0        0        0     1171 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/experimental/dist_field/README
+-rw-r--r--   0        0        0     3313 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/experimental/dist_field/genfield.py
+-rw-r--r--   0        0        0     1300 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/experimental/dist_field/py.df.png
+-rw-r--r--   0        0        0     5495 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/experimental/dist_field/py.png
+-rw-r--r--   0        0        0     8481 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/experimental/dist_field/renderfield.py
+-rw-r--r--   0        0        0    12986 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/experimental/flaccodec.py
+-rw-r--r--   0        0        0     6058 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/experimental/hello_world.svg
+-rw-r--r--   0        0        0     1128 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/experimental/spritebenchmark.py
+-rw-r--r--   0        0        0    14149 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/experimental/svg_test.py
+-rw-r--r--   0        0        0     2178 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/experimental/wayland/gbm_egl_context.py
+-rw-r--r--   0        0        0     1906 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/experimental/win32priority.py
+-rwxr-xr-x   0        0        0     2399 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/make.py
+-rw-r--r--   0        0        0    12126 2024-04-13 23:03:31.923029 pyglet-2.1.dev2/pyglet/__init__.py
+-rw-r--r--   0        0        0      543 2024-04-13 23:03:31.926343 pyglet-2.1.dev2/pyglet/__init__.pyi
+-rw-r--r--   0        0        0     2875 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/app/__init__.py
+-rw-r--r--   0        0        0    11064 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/app/base.py
+-rw-r--r--   0        0        0     9228 2024-03-08 00:58:25.028785 pyglet-2.1.dev2/pyglet/app/cocoa.py
+-rw-r--r--   0        0        0     4325 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/pyglet/app/win32.py
+-rw-r--r--   0        0        0     2543 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/pyglet/app/xlib.py
+-rw-r--r--   0        0        0    21640 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/pyglet/clock.py
+-rw-r--r--   0        0        0      606 2024-04-02 05:14:53.599283 pyglet-2.1.dev2/pyglet/customtypes.py
+-rwxr-xr-x   0        0        0     3093 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/display/__init__.py
+-rwxr-xr-x   0        0        0    10500 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/display/base.py
+-rw-r--r--   0        0        0     5559 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/display/cocoa.py
+-rw-r--r--   0        0        0     2152 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/display/headless.py
+-rwxr-xr-x   0        0        0     4774 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/display/win32.py
+-rw-r--r--   0        0        0     9210 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/display/xlib.py
+-rw-r--r--   0        0        0     5654 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/display/xlib_vidmoderestore.py
+-rw-r--r--   0        0        0    17272 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/pyglet/event.py
+-rw-r--r--   0        0        0      221 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/pyglet/experimental/README.md
+-rw-r--r--   0        0        0    24495 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/pyglet/experimental/geoshader_sprite.py
+-rw-r--r--   0        0        0     6260 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/pyglet/experimental/hidraw.py
+-rw-r--r--   0        0        0     7680 2024-02-28 05:05:21.230711 pyglet-2.1.dev2/pyglet/experimental/net.py
+-rw-r--r--   0        0        0      128 2024-02-28 05:05:21.234044 pyglet-2.1.dev2/pyglet/extlibs/__init__.py
+-rw-r--r--   0        0        0    81404 2024-02-28 05:05:21.234044 pyglet-2.1.dev2/pyglet/extlibs/png.py
+-rw-r--r--   0        0        0     8373 2024-04-02 05:14:53.599283 pyglet-2.1.dev2/pyglet/font/__init__.py
+-rw-r--r--   0        0        0    13521 2024-02-28 05:05:21.234044 pyglet-2.1.dev2/pyglet/font/base.py
+-rw-r--r--   0        0        0    95230 2024-02-28 05:05:21.234044 pyglet-2.1.dev2/pyglet/font/directwrite.py
+-rw-r--r--   0        0        0     9763 2024-02-28 05:05:21.234044 pyglet-2.1.dev2/pyglet/font/fontconfig.py
+-rw-r--r--   0        0        0    12212 2024-02-28 05:05:21.234044 pyglet-2.1.dev2/pyglet/font/freetype.py
+-rw-r--r--   0        0        0    15642 2024-02-28 05:05:21.234044 pyglet-2.1.dev2/pyglet/font/freetype_lib.py
+-rw-r--r--   0        0        0    12533 2024-02-28 05:05:21.234044 pyglet-2.1.dev2/pyglet/font/quartz.py
+-rw-r--r--   0        0        0    23839 2024-02-28 05:05:21.234044 pyglet-2.1.dev2/pyglet/font/ttf.py
+-rw-r--r--   0        0        0     6569 2024-03-08 00:58:25.028785 pyglet-2.1.dev2/pyglet/font/user.py
+-rw-r--r--   0        0        0    16227 2024-03-08 00:58:25.028785 pyglet-2.1.dev2/pyglet/font/win32.py
+-rw-r--r--   0        0        0     5407 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/gl/__init__.py
+-rw-r--r--   0        0        0    26670 2024-02-28 05:05:21.234044 pyglet-2.1.dev2/pyglet/gl/agl.py
+-rwxr-xr-x   0        0        0    17746 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/gl/base.py
+-rw-r--r--   0        0        0    10601 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/gl/cocoa.py
+-rw-r--r--   0        0        0   212567 2024-02-28 05:05:21.234044 pyglet-2.1.dev2/pyglet/gl/gl.py
+-rw-r--r--   0        0        0   277237 2024-02-28 05:05:21.234044 pyglet-2.1.dev2/pyglet/gl/gl_compat.py
+-rw-r--r--   0        0        0     6513 2024-02-28 05:05:21.234044 pyglet-2.1.dev2/pyglet/gl/gl_info.py
+-rw-r--r--   0        0        0    29235 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/gl/glx.py
+-rw-r--r--   0        0        0     3565 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/gl/glx_info.py
+-rw-r--r--   0        0        0    50608 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/gl/glxext_arb.py
+-rw-r--r--   0        0        0      261 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/gl/glxext_mesa.py
+-rw-r--r--   0        0        0    41435 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/gl/glxext_nv.py
+-rw-r--r--   0        0        0     5224 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/gl/headless.py
+-rw-r--r--   0        0        0     3405 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/gl/lib.py
+-rw-r--r--   0        0        0      902 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/gl/lib_agl.py
+-rw-r--r--   0        0        0     1408 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/gl/lib_glx.py
+-rw-r--r--   0        0        0     2910 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/gl/lib_wgl.py
+-rwxr-xr-x   0        0        0    16109 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/gl/wgl.py
+-rwxr-xr-x   0        0        0      954 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/gl/wgl_info.py
+-rw-r--r--   0        0        0    70293 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/gl/wglext_arb.py
+-rw-r--r--   0        0        0    69927 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/gl/wglext_nv.py
+-rwxr-xr-x   0        0        0     9223 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/gl/win32.py
+-rw-r--r--   0        0        0     8652 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/gl/xlib.py
+-rw-r--r--   0        0        0    20565 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/graphics/__init__.py
+-rw-r--r--   0        0        0    12604 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/graphics/allocation.py
+-rw-r--r--   0        0        0    44701 2024-04-02 05:14:53.599283 pyglet-2.1.dev2/pyglet/graphics/shader.py
+-rw-r--r--   0        0        0     1105 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/graphics/vertexarray.py
+-rw-r--r--   0        0        0    12807 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/graphics/vertexbuffer.py
+-rw-r--r--   0        0        0    19779 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/graphics/vertexdomain.py
+-rw-r--r--   0        0        0       44 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/gui/__init__.py
+-rw-r--r--   0        0        0     6862 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/gui/frame.py
+-rw-r--r--   0        0        0    18793 2024-04-13 23:03:31.926343 pyglet-2.1.dev2/pyglet/gui/widgets.py
+-rw-r--r--   0        0        0    76136 2024-04-02 05:14:53.599283 pyglet-2.1.dev2/pyglet/image/__init__.py
+-rw-r--r--   0        0        0     6413 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/image/animation.py
+-rw-r--r--   0        0        0    10284 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/image/atlas.py
+-rw-r--r--   0        0        0     8488 2024-04-02 05:14:53.599283 pyglet-2.1.dev2/pyglet/image/buffer.py
+-rw-r--r--   0        0        0     6498 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/image/codecs/__init__.py
+-rw-r--r--   0        0        0    10642 2024-02-28 05:05:21.237378 pyglet-2.1.dev2/pyglet/image/codecs/bmp.py
+-rw-r--r--   0        0        0     5668 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/image/codecs/dds.py
+-rw-r--r--   0        0        0    11012 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/image/codecs/gdiplus.py
+-rw-r--r--   0        0        0     8939 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/image/codecs/gdkpixbuf2.py
+-rw-r--r--   0        0        0     3571 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/image/codecs/gif.py
+-rw-r--r--   0        0        0     2592 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/image/codecs/pil.py
+-rw-r--r--   0        0        0     2081 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/image/codecs/png.py
+-rw-r--r--   0        0        0     4708 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/image/codecs/quartz.py
+-rw-r--r--   0        0        0    12392 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/image/codecs/s3tc.py
+-rw-r--r--   0        0        0    22368 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/image/codecs/wic.py
+-rw-r--r--   0        0        0     5835 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/info.py
+-rw-r--r--   0        0        0     6252 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/input/__init__.py
+-rw-r--r--   0        0        0    41133 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/input/base.py
+-rw-r--r--   0        0        0     5623 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/input/controller.py
+-rw-r--r--   0        0        0   193972 2024-04-13 23:03:31.926343 pyglet-2.1.dev2/pyglet/input/controller_db.py
+-rw-r--r--   0        0        0      391 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/input/linux/__init__.py
+-rw-r--r--   0        0        0    19502 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/input/linux/evdev.py
+-rw-r--r--   0        0        0     9789 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/input/linux/evdev_constants.py
+-rw-r--r--   0        0        0    10993 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/input/linux/x11_xinput.py
+-rw-r--r--   0        0        0     3007 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/input/linux/x11_xinput_tablet.py
+-rw-r--r--   0        0        0      348 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/input/macos/__init__.py
+-rw-r--r--   0        0        0    24468 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/input/macos/darwin_hid.py
+-rw-r--r--   0        0        0     4222 2024-03-08 00:58:25.028785 pyglet-2.1.dev2/pyglet/input/win32/__init__.py
+-rw-r--r--   0        0        0    16928 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/input/win32/directinput.py
+-rw-r--r--   0        0        0    14512 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/input/win32/wintab.py
+-rw-r--r--   0        0        0    21397 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/input/win32/xinput.py
+-rw-r--r--   0        0        0    10952 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/lib.py
+-rw-r--r--   0        0        0        1 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/libs/__init__.py
+-rw-r--r--   0        0        0       23 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/libs/darwin/__init__.py
+-rw-r--r--   0        0        0     1798 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/libs/darwin/cocoapy/__init__.py
+-rw-r--r--   0        0        0    23244 2024-04-13 23:03:26.299270 pyglet-2.1.dev2/pyglet/libs/darwin/cocoapy/cocoalibs.py
+-rw-r--r--   0        0        0     2629 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/libs/darwin/cocoapy/cocoatypes.py
+-rw-r--r--   0        0        0    56271 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/libs/darwin/cocoapy/runtime.py
+-rw-r--r--   0        0        0     6964 2024-02-28 05:05:21.240711 pyglet-2.1.dev2/pyglet/libs/darwin/coreaudio.py
+-rw-r--r--   0        0        0     5179 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/darwin/quartzkey.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/egl/__init__.py
+-rw-r--r--   0        0        0    29920 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/egl/egl.py
+-rw-r--r--   0        0        0      859 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/egl/eglext.py
+-rw-r--r--   0        0        0      893 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/egl/lib.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/wayland/__init__.py
+-rw-r--r--   0        0        0    13388 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/wayland/gbm.py
+-rw-r--r--   0        0        0    20657 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/wayland/xkbcommon.py
+-rwxr-xr-x   0        0        0    14234 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/pyglet/libs/win32/__init__.py
+-rw-r--r--   0        0        0    15463 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/win32/com.py
+-rw-r--r--   0        0        0   121260 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/pyglet/libs/win32/constants.py
+-rw-r--r--   0        0        0     1433 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/win32/context_managers.py
+-rwxr-xr-x   0        0        0    10968 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/win32/dinput.py
+-rwxr-xr-x   0        0        0    10901 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/win32/libwintab.py
+-rw-r--r--   0        0        0    14851 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/pyglet/libs/win32/types.py
+-rw-r--r--   0        0        0     4667 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/win32/winkey.py
+-rw-r--r--   0        0        0        1 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/x11/__init__.py
+-rw-r--r--   0        0        0     1451 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/x11/cursorfont.py
+-rw-r--r--   0        0        0    13531 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/x11/xf86vmode.py
+-rw-r--r--   0        0        0     2182 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/x11/xinerama.py
+-rw-r--r--   0        0        0    54556 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/x11/xinput.py
+-rw-r--r--   0        0        0   183778 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/pyglet/libs/x11/xlib.py
+-rw-r--r--   0        0        0    15202 2024-02-28 05:05:21.244044 pyglet-2.1.dev2/pyglet/libs/x11/xsync.py
+-rw-r--r--   0        0        0    35523 2024-04-13 23:03:31.926343 pyglet-2.1.dev2/pyglet/math.py
+-rw-r--r--   0        0        0     3208 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/__init__.py
+-rw-r--r--   0        0        0     1025 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/buffered_logger.py
+-rw-r--r--   0        0        0     3308 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/codecs/__init__.py
+-rw-r--r--   0        0        0    25186 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/codecs/base.py
+-rw-r--r--   0        0        0     6805 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/codecs/coreaudio.py
+-rw-r--r--   0        0        0    40899 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/codecs/ffmpeg.py
+-rw-r--r--   0        0        0      201 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/codecs/ffmpeg_lib/__init__.py
+-rw-r--r--   0        0        0     3314 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/codecs/ffmpeg_lib/compat.py
+-rw-r--r--   0        0        0    15663 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/codecs/ffmpeg_lib/libavcodec.py
+-rw-r--r--   0        0        0    10160 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/codecs/ffmpeg_lib/libavformat.py
+-rw-r--r--   0        0        0     7169 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/codecs/ffmpeg_lib/libavutil.py
+-rw-r--r--   0        0        0     1688 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/codecs/ffmpeg_lib/libswresample.py
+-rw-r--r--   0        0        0     1501 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/codecs/ffmpeg_lib/libswscale.py
+-rw-r--r--   0        0        0     9250 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/codecs/gstreamer.py
+-rw-r--r--   0        0        0    17727 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/codecs/pyogg.py
+-rw-r--r--   0        0        0     3566 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/codecs/wave.py
+-rw-r--r--   0        0        0    33706 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/codecs/wmf.py
+-rw-r--r--   0        0        0      773 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/devices/__init__.py
+-rw-r--r--   0        0        0     3218 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/devices/base.py
+-rw-r--r--   0        0        0    12409 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/devices/win32.py
+-rw-r--r--   0        0        0     2463 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/drivers/__init__.py
+-rw-r--r--   0        0        0    15352 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/drivers/base.py
+-rw-r--r--   0        0        0      251 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/drivers/directsound/__init__.py
+-rw-r--r--   0        0        0    12133 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/drivers/directsound/adaptation.py
+-rw-r--r--   0        0        0      325 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/drivers/directsound/exceptions.py
+-rw-r--r--   0        0        0    12655 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/drivers/directsound/interface.py
+-rw-r--r--   0        0        0    12705 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/drivers/directsound/lib_dsound.py
+-rw-r--r--   0        0        0     2438 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/drivers/listener.py
+-rw-r--r--   0        0        0      324 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/drivers/openal/__init__.py
+-rw-r--r--   0        0        0     9226 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/drivers/openal/adaptation.py
+-rw-r--r--   0        0        0    16582 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/drivers/openal/interface.py
+-rw-r--r--   0        0        0    10833 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/drivers/openal/lib_alc.py
+-rw-r--r--   0        0        0    26707 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/drivers/openal/lib_openal.py
+-rw-r--r--   0        0        0      244 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/drivers/pulse/__init__.py
+-rw-r--r--   0        0        0    14112 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/drivers/pulse/adaptation.py
+-rw-r--r--   0        0        0    26864 2024-02-28 05:05:21.247378 pyglet-2.1.dev2/pyglet/media/drivers/pulse/interface.py
+-rw-r--r--   0        0        0   125621 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/media/drivers/pulse/lib_pulseaudio.py
+-rw-r--r--   0        0        0      127 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/media/drivers/silent/__init__.py
+-rw-r--r--   0        0        0     4080 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/media/drivers/silent/adaptation.py
+-rw-r--r--   0        0        0      128 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/media/drivers/xaudio2/__init__.py
+-rw-r--r--   0        0        0    12769 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/media/drivers/xaudio2/adaptation.py
+-rw-r--r--   0        0        0    25003 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/media/drivers/xaudio2/interface.py
+-rw-r--r--   0        0        0    27709 2024-04-02 05:14:53.599283 pyglet-2.1.dev2/pyglet/media/drivers/xaudio2/lib_xaudio2.py
+-rw-r--r--   0        0        0      152 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/media/exceptions.py
+-rw-r--r--   0        0        0    10798 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/media/instrumentation.py
+-rw-r--r--   0        0        0    23852 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/media/player.py
+-rw-r--r--   0        0        0     3768 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/media/player_worker_thread.py
+-rw-r--r--   0        0        0    11814 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/media/synthesis.py
+-rw-r--r--   0        0        0    12946 2024-04-13 23:03:31.926343 pyglet-2.1.dev2/pyglet/model/__init__.py
+-rw-r--r--   0        0        0     1502 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/model/codecs/__init__.py
+-rw-r--r--   0        0        0     7303 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/model/codecs/gltf.py
+-rw-r--r--   0        0        0     7683 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/model/codecs/obj.py
+-rw-r--r--   0        0        0    30029 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/resource.py
+-rw-r--r--   0        0        0    73958 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/pyglet/shapes.py
+-rw-r--r--   0        0        0    26390 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/pyglet/sprite.py
+-rw-r--r--   0        0        0    17920 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/pyglet/text/__init__.py
+-rw-r--r--   0        0        0    22076 2024-04-02 05:14:53.602617 pyglet-2.1.dev2/pyglet/text/caret.py
+-rw-r--r--   0        0        0    24041 2024-04-02 05:14:53.602617 pyglet-2.1.dev2/pyglet/text/document.py
+-rw-r--r--   0        0        0       48 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/text/formats/__init__.py
+-rw-r--r--   0        0        0     2679 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/text/formats/attributed.py
+-rw-r--r--   0        0        0    11551 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/text/formats/html.py
+-rw-r--r--   0        0        0      264 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/text/formats/plaintext.py
+-rw-r--r--   0        0        0    10726 2024-04-02 05:14:53.602617 pyglet-2.1.dev2/pyglet/text/formats/structured.py
+-rw-r--r--   0        0        0     6142 2024-04-02 05:14:53.602617 pyglet-2.1.dev2/pyglet/text/layout/__init__.py
+-rw-r--r--   0        0        0    74183 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/pyglet/text/layout/base.py
+-rw-r--r--   0        0        0    35365 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/pyglet/text/layout/incremental.py
+-rw-r--r--   0        0        0     9310 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/pyglet/text/layout/scrolling.py
+-rw-r--r--   0        0        0    12514 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/text/runlist.py
+-rw-r--r--   0        0        0     8646 2024-02-28 05:05:21.250711 pyglet-2.1.dev2/pyglet/util.py
+-rw-r--r--   0        0        0    68027 2024-04-13 23:03:31.926343 pyglet-2.1.dev2/pyglet/window/__init__.py
+-rw-r--r--   0        0        0    26197 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/pyglet/window/cocoa/__init__.py
+-rw-r--r--   0        0        0     5866 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/pyglet/window/cocoa/pyglet_delegate.py
+-rw-r--r--   0        0        0     6677 2024-03-08 00:58:25.028785 pyglet-2.1.dev2/pyglet/window/cocoa/pyglet_textview.py
+-rw-r--r--   0        0        0    14775 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/pyglet/window/cocoa/pyglet_view.py
+-rw-r--r--   0        0        0     3284 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/pyglet/window/cocoa/pyglet_window.py
+-rw-r--r--   0        0        0      691 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/pyglet/window/cocoa/systemcursor.py
+-rw-r--r--   0        0        0     3830 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/pyglet/window/event.py
+-rw-r--r--   0        0        0     2776 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/pyglet/window/headless/__init__.py
+-rw-r--r--   0        0        0     9566 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/pyglet/window/key.py
+-rw-r--r--   0        0        0     2324 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/pyglet/window/mouse.py
+-rw-r--r--   0        0        0    50394 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/pyglet/window/win32/__init__.py
+-rw-r--r--   0        0        0    66785 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/pyglet/window/xlib/__init__.py
+-rw-r--r--   0        0        0      355 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/pyproject.toml
+-rw-r--r--   0        0        0      569 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/pytest.ini
+-rw-r--r--   0        0        0     1961 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/setup.py
+-rw-r--r--   0        0        0       97 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/tests/__init__.py
+-rw-r--r--   0        0        0     2251 2024-03-08 00:58:25.028785 pyglet-2.1.dev2/tests/annotations.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/tests/base/__init__.py
+-rw-r--r--   0        0        0     1153 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/tests/base/data.py
+-rw-r--r--   0        0        0     5311 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/tests/base/event_loop.py
+-rw-r--r--   0        0        0    11528 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/tests/base/interactive.py
+-rw-r--r--   0        0        0      497 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/tests/base/performance.py
+-rw-r--r--   0        0        0      818 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/tests/conftest.py
+-rw-r--r--   0        0        0      175 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/tests/data/fonts/README
+-rw-r--r--   0        0        0    49408 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/tests/data/fonts/action_man.ttf
+-rw-r--r--   0        0        0    48976 2024-02-28 05:05:21.254045 pyglet-2.1.dev2/tests/data/fonts/action_man_bold.ttf
+-rw-r--r--   0        0        0    49008 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/fonts/action_man_bold_italic.ttf
+-rw-r--r--   0        0        0    49424 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/fonts/action_man_italic.ttf
+-rw-r--r--   0        0        0    13756 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/fonts/courR12-ISO8859-1.pcf
+-rw-r--r--   0        0        0    17335 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/images/8bpp.gif
+-rw-r--r--   0        0        0     2452 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/images/cursor.png
+-rw-r--r--   0        0        0     7002 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/images/dinosaur.gif
+-rw-r--r--   0        0        0      624 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/images/gdk_close.png
+-rw-r--r--   0        0        0     5449 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/images/grey_background.png
+-rw-r--r--   0        0        0     2350 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/images/icon1.png
+-rw-r--r--   0        0        0      275 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/images/icon_size1.png
+-rw-r--r--   0        0        0      508 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/images/icon_size2.png
+-rw-r--r--   0        0        0      898 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/images/icon_size3.png
+-rw-r--r--   0        0        0      831 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/images/icon_size4.png
+-rw-r--r--   0        0        0     1609 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/images/icon_size5.png
+-rw-r--r--   0        0        0    18720 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/images/l.png
+-rw-r--r--   0        0        0    18324 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/images/la.png
+-rw-r--r--   0        0        0      437 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/images/multitexture.png
+-rwxr-xr-x   0        0        0    53639 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/images/rgb.png
+-rw-r--r--   0        0        0   121374 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/images/rgb_16bpp.bmp
+-rw-r--r--   0        0        0     8286 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/images/rgb_1bpp.bmp
+-rw-r--r--   0        0        0   182010 2024-02-28 05:05:21.257378 pyglet-2.1.dev2/tests/data/images/rgb_24bpp.bmp
+-rw-r--r--   0        0        0   241650 2024-02-28 05:05:21.260712 pyglet-2.1.dev2/tests/data/images/rgb_32bpp.bmp
+-rw-r--r--   0        0        0    30958 2024-02-28 05:05:21.260712 pyglet-2.1.dev2/tests/data/images/rgb_4bpp.bmp
+-rw-r--r--   0        0        0    61730 2024-02-28 05:05:21.260712 pyglet-2.1.dev2/tests/data/images/rgb_8bpp.bmp
+-rw-r--r--   0        0        0    11956 2024-02-28 05:05:21.260712 pyglet-2.1.dev2/tests/data/images/rgb_8bpp.png
+-rw-r--r--   0        0        0    10169 2024-02-28 05:05:21.260712 pyglet-2.1.dev2/tests/data/images/rgb_8bpp_trans.png
+-rw-r--r--   0        0        0    32896 2024-02-28 05:05:21.260712 pyglet-2.1.dev2/tests/data/images/rgb_dxt1.dds
+-rwxr-xr-x   0        0        0    83645 2024-02-28 05:05:21.260712 pyglet-2.1.dev2/tests/data/images/rgba.png
+-rw-r--r--   0        0        0   241634 2024-02-28 05:05:21.260712 pyglet-2.1.dev2/tests/data/images/rgba_32bpp.bmp
+-rw-r--r--   0        0        0    32896 2024-02-28 05:05:21.260712 pyglet-2.1.dev2/tests/data/images/rgba_dxt1.dds
+-rw-r--r--   0        0        0    65664 2024-02-28 05:05:21.260712 pyglet-2.1.dev2/tests/data/images/rgba_dxt3.dds
+-rw-r--r--   0        0        0    65664 2024-02-28 05:05:21.264045 pyglet-2.1.dev2/tests/data/images/rgba_dxt5.dds
+-rw-r--r--   0        0        0      590 2024-02-28 05:05:21.264045 pyglet-2.1.dev2/tests/data/images/tests.interactive.test_interactive_test_base._Test.test_1.001.png
+-rw-r--r--   0        0        0       51 2024-02-28 05:05:21.264045 pyglet-2.1.dev2/tests/data/media/README
+-rw-r--r--   0        0        0    23314 2024-02-28 05:05:21.264045 pyglet-2.1.dev2/tests/data/media/alert.wav
+-rw-r--r--   0        0        0   192412 2024-02-28 05:05:21.264045 pyglet-2.1.dev2/tests/data/media/login.wav
+-rw-r--r--   0        0        0   155888 2024-02-28 05:05:21.264045 pyglet-2.1.dev2/tests/data/media/logout.wav
+-rw-r--r--   0        0        0    55008 2024-02-28 05:05:21.264045 pyglet-2.1.dev2/tests/data/media/receive.wav
+-rw-r--r--   0        0        0    57440 2024-02-28 05:05:21.264045 pyglet-2.1.dev2/tests/data/media/send.wav
+-rw-r--r--   0        0        0    22094 2024-02-28 05:05:21.264045 pyglet-2.1.dev2/tests/data/media/synthesis_sawtooth_16_11025_1ch.wav
+-rw-r--r--   0        0        0    89644 2024-02-28 05:05:21.264045 pyglet-2.1.dev2/tests/data/media/synthesis_sawtooth_16_44800_1ch.wav
+-rw-r--r--   0        0        0    22094 2024-02-28 05:05:21.264045 pyglet-2.1.dev2/tests/data/media/synthesis_silence_16_11025_1ch.wav
+-rw-r--r--   0        0        0    89644 2024-02-28 05:05:21.264045 pyglet-2.1.dev2/tests/data/media/synthesis_silence_16_44800_1ch.wav
+-rw-r--r--   0        0        0    22094 2024-02-28 05:05:21.264045 pyglet-2.1.dev2/tests/data/media/synthesis_simplefm_16_11025_1ch.wav
+-rw-r--r--   0        0        0    89644 2024-02-28 05:05:21.264045 pyglet-2.1.dev2/tests/data/media/synthesis_simplefm_16_44800_1ch.wav
+-rw-r--r--   0        0        0    22094 2024-02-28 05:05:21.264045 pyglet-2.1.dev2/tests/data/media/synthesis_sine_16_11025_1ch.wav
+-rw-r--r--   0        0        0    89644 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/data/media/synthesis_sine_16_44800_1ch.wav
+-rw-r--r--   0        0        0    22094 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/data/media/synthesis_square_16_11025_1ch.wav
+-rw-r--r--   0        0        0    89644 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/data/media/synthesis_square_16_44800_1ch.wav
+-rw-r--r--   0        0        0    22094 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/data/media/synthesis_triangle_16_11025_1ch.wav
+-rw-r--r--   0        0        0    89644 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/data/media/synthesis_triangle_16_44800_1ch.wav
+-rw-r--r--   0        0        0      209 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/data/models/logo3d.mtl
+-rw-r--r--   0        0        0   553330 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/data/models/logo3d.obj
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/app/__init__.py
+-rw-r--r--   0        0        0     1660 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/app/test_eventloop.py
+-rw-r--r--   0        0        0      378 2024-03-08 00:58:25.028785 pyglet-2.1.dev2/tests/integration/font/test_fontconfig.py
+-rw-r--r--   0        0        0     4093 2024-03-08 00:58:25.028785 pyglet-2.1.dev2/tests/integration/font/test_freetype_face.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/graphics/__init__.py
+-rwxr-xr-x   0        0        0    12662 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/graphics/test_allocation.py
+-rw-r--r--   0        0        0      654 2024-03-08 00:58:25.028785 pyglet-2.1.dev2/tests/integration/graphics/test_batch_migration.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/image/__init__.py
+-rw-r--r--   0        0        0     2552 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/image/test_gdkpixbuf2.py
+-rw-r--r--   0        0        0     3176 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/image/test_imagegrid.py
+-rw-r--r--   0        0        0     3887 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/image/test_texture3d.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/media/__init__.py
+-rw-r--r--   0        0        0     2617 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/media/mock_player.py
+-rw-r--r--   0        0        0     7282 2024-04-02 05:14:53.602617 pyglet-2.1.dev2/tests/integration/media/test_directsound.py
+-rw-r--r--   0        0        0     4615 2024-04-02 05:14:53.602617 pyglet-2.1.dev2/tests/integration/media/test_driver.py
+-rw-r--r--   0        0        0    11912 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/media/test_openal.py
+-rw-r--r--   0        0        0     2205 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/media/test_player.py
+-rw-r--r--   0        0        0     8161 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/media/test_pulse.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/model/__init__.py
+-rw-r--r--   0        0        0     1644 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/model/test_loading.py
+-rw-r--r--   0        0        0       83 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/platform/__init__.py
+-rw-r--r--   0        0        0     3871 2024-03-08 00:58:25.028785 pyglet-2.1.dev2/tests/integration/platform/test_win_context_managers.py
+-rw-r--r--   0        0        0     1210 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/platform/test_win_multicore_clock.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/resource/__init__.py
+-rw-r--r--   0        0        0        3 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/resource/dir1/dir1/f3.txt
+-rw-r--r--   0        0        0        3 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/resource/dir1/f2.txt
+-rw-r--r--   0        0        0      749 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/resource/dir1/res.zip
+-rw-r--r--   0        0        0        3 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/resource/dir2/f6.txt
+-rw-r--r--   0        0        0        3 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/resource/f1.txt
+-rwxr-xr-x   0        0        0      170 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/resource/rgbm.png
+-rwxr-xr-x   0        0        0     2130 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/resource/test_resource_image_loading.py
+-rw-r--r--   0        0        0     2575 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/resource/test_resource_loading.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/text/__init__.py
+-rw-r--r--   0        0        0     1261 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/tests/integration/text/test_empty_document.py
+-rw-r--r--   0        0        0     1070 2024-03-08 04:38:06.094148 pyglet-2.1.dev2/tests/integration/text/test_label_creation.py
+-rw-r--r--   0        0        0     1453 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/tests/integration/text/test_layout_creation.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/window/__init__.py
+-rw-r--r--   0        0        0     1476 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/tests/integration/window/test_context_share.py
+-rw-r--r--   0        0        0     5844 2024-04-02 05:14:53.602617 pyglet-2.1.dev2/tests/integration/window/test_event_sequence.py
+-rw-r--r--   0        0        0      833 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/integration/window/test_window_caption.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/interactive/__init__.py
+-rw-r--r--   0        0        0     2757 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/interactive/conftest.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/interactive/image/__init__.py
+-rw-r--r--   0        0        0    11804 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/interactive/image/test_image.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/interactive/media/__init__.py
+-rw-r--r--   0        0        0     4436 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/interactive/media/test_player.py
+-rw-r--r--   0        0        0       75 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/interactive/screenshots/committed/README
+-rw-r--r--   0        0        0       80 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/interactive/screenshots/session/README
+-rw-r--r--   0        0        0     5805 2024-03-08 00:58:25.028785 pyglet-2.1.dev2/tests/interactive/shapes/test_shapes.py
+-rw-r--r--   0        0        0    14904 2024-03-08 00:58:25.028785 pyglet-2.1.dev2/tests/interactive/test_interactive_test_base.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/interactive/text/__init__.py
+-rw-r--r--   0        0        0     4382 2024-04-02 05:14:53.602617 pyglet-2.1.dev2/tests/interactive/text/test_caret_color.py
+-rw-r--r--   0        0        0     5999 2024-04-02 05:14:53.602617 pyglet-2.1.dev2/tests/interactive/text/test_content_valign.py
+-rw-r--r--   0        0        0     8054 2024-04-02 05:14:53.602617 pyglet-2.1.dev2/tests/interactive/text/test_html.py
+-rw-r--r--   0        0        0     8309 2024-04-02 05:14:53.602617 pyglet-2.1.dev2/tests/interactive/text/test_inline_elements.py
+-rw-r--r--   0        0        0     5686 2024-04-02 05:14:53.602617 pyglet-2.1.dev2/tests/interactive/text/test_inline_elements_style_change.py
+-rw-r--r--   0        0        0     4826 2024-04-02 05:14:53.602617 pyglet-2.1.dev2/tests/interactive/text/test_multiline_wrap.py
+-rw-r--r--   0        0        0     5015 2024-04-02 05:14:53.602617 pyglet-2.1.dev2/tests/interactive/text/test_plain.py
+-rw-r--r--   0        0        0    11612 2024-04-02 05:14:53.602617 pyglet-2.1.dev2/tests/interactive/text/test_style.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.267378 pyglet-2.1.dev2/tests/interactive/window/__init__.py
+-rw-r--r--   0        0        0    25342 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/interactive/window/test_window_events.py
+-rw-r--r--   0        0        0     5390 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/interactive/window/test_window_fullscreen.py
+-rw-r--r--   0        0        0     4301 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/interactive/window/test_window_modes.py
+-rwxr-xr-x   0        0        0     4683 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/interactive/window/test_window_multisample.py
+-rw-r--r--   0        0        0     1487 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/interactive/window/test_window_open.py
+-rw-r--r--   0        0        0    20880 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/interactive/window/test_window_settings.py
+-rw-r--r--   0        0        0     1131 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/interactive/window/test_window_styles.py
+-rwxr-xr-x   0        0        0      647 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/interactive/window/window_util.py
+-rw-r--r--   0        0        0     2232 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/interactive/windowed_test_base.py
+-rw-r--r--   0        0        0       25 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/requirements.txt
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/unit/__init__.py
+-rw-r--r--   0        0        0     2985 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/tests/unit/conftest.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/unit/media/__init__.py
+-rw-r--r--   0        0        0     2157 2024-03-08 00:58:25.028785 pyglet-2.1.dev2/tests/unit/media/test_listener.py
+-rw-r--r--   0        0        0    33518 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/unit/media/test_player.py
+-rw-r--r--   0        0        0    14145 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/unit/media/test_sources.py
+-rw-r--r--   0        0        0     2283 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/unit/media/test_synthesis.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/unit/shapes/__init__.py
+-rw-r--r--   0        0        0      283 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/unit/shapes/conftest.py
+-rw-r--r--   0        0        0     3528 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/unit/shapes/test_bordered_rectangle.py
+-rw-r--r--   0        0        0     3493 2024-03-08 00:58:25.028785 pyglet-2.1.dev2/tests/unit/shapes/test_shapes.py
+-rw-r--r--   0        0        0     2596 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/unit/test_atlas.py
+-rw-r--r--   0        0        0    14135 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/unit/test_clock.py
+-rw-r--r--   0        0        0     2125 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/unit/test_clock_freq.py
+-rw-r--r--   0        0        0     6828 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/unit/test_events.py
+-rw-r--r--   0        0        0      594 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/unit/test_font.py
+-rw-r--r--   0        0        0      293 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/unit/test_input.py
+-rw-r--r--   0        0        0     3993 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/unit/test_math.py
+-rw-r--r--   0        0        0     4686 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/unit/test_resource_path.py
+-rw-r--r--   0        0        0     3880 2024-04-13 23:03:26.302566 pyglet-2.1.dev2/tests/unit/test_sprite.py
+-rw-r--r--   0        0        0    11559 2024-04-13 23:03:26.305862 pyglet-2.1.dev2/tests/unit/test_text.py
+-rw-r--r--   0        0        0        0 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/unit/text/__init__.py
+-rw-r--r--   0        0        0     3300 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tests/unit/text/test_caret.py
+-rw-r--r--   0        0        0      950 2024-04-02 05:14:53.602617 pyglet-2.1.dev2/tests/unit/text/test_layout.py
+-rw-r--r--   0        0        0     2112 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tools/al_info.py
+-rw-r--r--   0        0        0     4404 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tools/ffmpeg/bokeh_timeline.py
+-rw-r--r--   0        0        0     2707 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tools/ffmpeg/compare.py
+-rw-r--r--   0        0        0     7684 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tools/ffmpeg/configure.py
+-rw-r--r--   0        0        0     6650 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tools/ffmpeg/extractors.py
+-rw-r--r--   0        0        0    12661 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tools/ffmpeg/fs.py
+-rw-r--r--   0        0        0       86 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tools/ffmpeg/mp.py
+-rw-r--r--   0        0        0     1311 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tools/ffmpeg/mpexceptions.py
+-rw-r--r--   0        0        0     3362 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tools/ffmpeg/playmany.py
+-rw-r--r--   0        0        0     1425 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tools/ffmpeg/readme_ffmpeg_debbuging_branch.txt
+-rw-r--r--   0        0        0     3201 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tools/ffmpeg/readme_run_tests.txt
+-rw-r--r--   0        0        0     1652 2024-02-28 05:05:21.270712 pyglet-2.1.dev2/tools/ffmpeg/report.py
+-rw-r--r--   0        0        0     6831 2024-02-28 05:05:21.274045 pyglet-2.1.dev2/tools/ffmpeg/reports.py
+-rw-r--r--   0        0        0     3392 2024-02-28 05:05:21.274045 pyglet-2.1.dev2/tools/ffmpeg/retry_crashed.py
+-rw-r--r--   0        0        0     2870 2024-02-28 05:05:21.274045 pyglet-2.1.dev2/tools/ffmpeg/run_test_suite.py
+-rw-r--r--   0        0        0     5060 2024-02-28 05:05:21.274045 pyglet-2.1.dev2/tools/ffmpeg/summarize.py
+-rw-r--r--   0        0        0     1345 2024-02-28 05:05:21.274045 pyglet-2.1.dev2/tools/ffmpeg/test_instrumentation.py
+-rw-r--r--   0        0        0     2699 2024-02-28 05:05:21.274045 pyglet-2.1.dev2/tools/ffmpeg/timeline.py
+-rwxr-xr-x   0        0        0     2703 2024-04-13 23:03:31.926343 pyglet-2.1.dev2/tools/gencontrollerdb.py
+-rw-r--r--   0        0        0     7237 2024-02-28 05:05:21.274045 pyglet-2.1.dev2/tools/gengl.py
+-rw-r--r--   0        0        0     4141 2024-02-28 05:05:21.274045 pyglet-2.1.dev2/tools/genwrappers.py
+-rw-r--r--   0        0        0      409 2024-02-28 05:05:21.274045 pyglet-2.1.dev2/tools/gl.template
+-rw-r--r--   0        0        0  2940792 2024-02-28 05:05:21.277378 pyglet-2.1.dev2/tools/gl.xml
+-rw-r--r--   0        0        0     2552 2024-04-13 23:03:26.305862 pyglet-2.1.dev2/tools/gl_info.py
+-rwxr-xr-x   0        0        0      766 2024-02-28 05:05:21.277378 pyglet-2.1.dev2/tools/inspect_font.py
+-rw-r--r--   0        0        0       21 2024-02-28 05:05:21.277378 pyglet-2.1.dev2/tools/requirements.txt
+-rwxr-xr-x   0        0        0     6624 2024-02-28 05:05:21.277378 pyglet-2.1.dev2/tools/wgl.h
+-rw-r--r--   0        0        0      355 2024-02-28 05:05:21.277378 pyglet-2.1.dev2/tools/wraptypes/__init__.py
+-rw-r--r--   0        0        0    45676 2024-02-28 05:05:21.277378 pyglet-2.1.dev2/tools/wraptypes/cparser.py
+-rw-r--r--   0        0        0    10431 2024-02-28 05:05:21.277378 pyglet-2.1.dev2/tools/wraptypes/ctypesparser.py
+-rw-r--r--   0        0        0    33992 2024-02-28 05:05:21.277378 pyglet-2.1.dev2/tools/wraptypes/lex.py
+-rw-r--r--   0        0        0    49188 2024-02-28 05:05:21.277378 pyglet-2.1.dev2/tools/wraptypes/preprocessor.py
+-rw-r--r--   0        0        0     9718 2024-02-28 05:05:21.277378 pyglet-2.1.dev2/tools/wraptypes/wrap.py
+-rw-r--r--   0        0        0    82261 2024-02-28 05:05:21.277378 pyglet-2.1.dev2/tools/wraptypes/yacc.py
+-rw-r--r--   0        0        0    20139 2024-02-28 05:05:21.277378 pyglet-2.1.dev2/website/LICENSE.txt
+-rw-r--r--   0        0        0      635 2024-02-28 05:05:21.277378 pyglet-2.1.dev2/website/README.rst
+-rw-r--r--   0        0        0     4286 2024-02-28 05:05:21.277378 pyglet-2.1.dev2/website/assets/favicon.ico
+-rw-r--r--   0        0        0      255 2024-02-28 05:05:21.277378 pyglet-2.1.dev2/website/assets/static/css/example-custom-styles.css
+-rw-r--r--   0        0        0     6575 2024-02-28 05:05:21.277378 pyglet-2.1.dev2/website/assets/static/images/pyglet.png
+-rw-r--r--   0        0        0      251 2024-02-28 05:05:21.277378 pyglet-2.1.dev2/website/content/404.html/contents.lr
+-rw-r--r--   0        0        0   229646 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/content/404.html/ngc-5793.jpg
+-rw-r--r--   0        0        0       37 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/content/authors/benjamin/contents.lr
+-rw-r--r--   0        0        0     6575 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/content/authors/benjamin/pyglet.png
+-rw-r--r--   0        0        0       41 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/content/authors/contents.lr
+-rw-r--r--   0        0        0      130 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/content/blog/contents.lr
+-rw-r--r--   0        0        0     1329 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/content/blog/welcome-blog/contents.lr
+-rw-r--r--   0        0        0     3861 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/content/contents.lr
+-rw-r--r--   0        0        0   531187 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/content/eclipse.jpg
+-rw-r--r--   0        0        0      825 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/pyglet.lektorproject
+-rw-r--r--   0        0        0      796 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/themes/lektor-icon/AUTHORS.txt
+-rw-r--r--   0        0        0     2843 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/themes/lektor-icon/CHANGELOG.md
+-rw-r--r--   0        0        0     8777 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/themes/lektor-icon/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1804 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/themes/lektor-icon/LICENSE.txt
+-rw-r--r--   0        0        0    52017 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/themes/lektor-icon/NOTICE.txt
+-rwxr-xr-x   0        0        0    33220 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/themes/lektor-icon/README.md
+-rw-r--r--   0        0        0   148797 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/css/bootstrap.css
+-rw-r--r--   0        0        0    37059 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/css/icomoon.css
+-rw-r--r--   0        0        0     7443 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/css/magnific-popup.css
+-rw-r--r--   0        0        0    43490 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/css/style.css
+-rw-r--r--   0        0        0    45404 2024-02-28 05:05:21.280712 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/fonts/bootstrap/glyphicons-halflings-regular.ttf
+-rw-r--r--   0        0        0    23424 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/fonts/bootstrap/glyphicons-halflings-regular.woff
+-rw-r--r--   0        0        0    18028 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/fonts/bootstrap/glyphicons-halflings-regular.woff2
+-rw-r--r--   0        0        0   200464 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/fonts/icomoon/icomoon.ttf
+-rw-r--r--   0        0        0   200540 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/fonts/icomoon/icomoon.woff
+-rw-r--r--   0        0        0    15382 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/images/Preloader_2.gif
+-rw-r--r--   0        0        0     1017 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/images/placeholder_person.png
+-rw-r--r--   0        0        0    86927 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/js/jquery-3.3.1.min.js
+-rw-r--r--   0        0        0     2302 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/js/jquery.easing.min.js
+-rw-r--r--   0        0        0    20235 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/js/jquery.magnific-popup.min.js
+-rw-r--r--   0        0        0    23302 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/js/jquery.stellar.js
+-rw-r--r--   0        0        0    12600 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/js/jquery.stellar.min.js
+-rw-r--r--   0        0        0     9029 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/js/jquery.waypoints.min.js
+-rw-r--r--   0        0        0      665 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/js/magnific-popup-options.js
+-rw-r--r--   0        0        0     7020 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/js/main-singlelayout.js
+-rw-r--r--   0        0        0     3484 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/assets/static/js/main.js
+-rw-r--r--   0        0        0     1873 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/flowblocks/content.ini
+-rw-r--r--   0        0        0     1390 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/flowblocks/gallery.ini
+-rw-r--r--   0        0        0     1070 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/flowblocks/gallery_item.ini
+-rw-r--r--   0        0        0     1396 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/flowblocks/member.ini
+-rw-r--r--   0        0        0     1611 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/flowblocks/mission.ini
+-rw-r--r--   0        0        0      954 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/flowblocks/mission_tab.ini
+-rw-r--r--   0        0        0      530 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/flowblocks/service.ini
+-rw-r--r--   0        0        0     1319 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/flowblocks/services.ini
+-rw-r--r--   0        0        0     1069 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/flowblocks/team.ini
+-rw-r--r--   0        0        0    23927 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/images/blog-index.png
+-rw-r--r--   0        0        0    35843 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/images/full-blog.png
+-rw-r--r--   0        0        0    58159 2024-02-28 05:05:21.284045 pyglet-2.1.dev2/website/themes/lektor-icon/images/full-page.png
+-rw-r--r--   0        0        0   614932 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/images/gallery-404.png
+-rw-r--r--   0        0        0   220108 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/images/gallery-singlepage.png
+-rw-r--r--   0        0        0   294590 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/images/mainpage-screenshots.png
+-rw-r--r--   0        0        0   281441 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/images/responsive-layout.png
+-rw-r--r--   0        0        0      880 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/models/404.ini
+-rw-r--r--   0        0        0      393 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/models/author.ini
+-rw-r--r--   0        0        0      148 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/models/authors.ini
+-rw-r--r--   0        0        0     1778 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/models/blog-post.ini
+-rw-r--r--   0        0        0      705 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/models/blog.ini
+-rw-r--r--   0        0        0      570 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/models/page.ini
+-rw-r--r--   0        0        0     1281 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/models/single-layout.ini
+-rw-r--r--   0        0        0     1309 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/templates/404.html
+-rw-r--r--   0        0        0       71 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/templates/author.html
+-rw-r--r--   0        0        0       26 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/templates/authors.html
+-rw-r--r--   0        0        0      624 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/templates/blocks/content.html
+-rw-r--r--   0        0        0     1422 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/templates/blocks/gallery.html
+-rw-r--r--   0        0        0     1783 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/templates/blocks/mission.html
+-rw-r--r--   0        0        0     1294 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/templates/blocks/services.html
+-rw-r--r--   0        0        0     2407 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/templates/blocks/team.html
+-rw-r--r--   0        0        0      594 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/templates/blog-layout.html
+-rw-r--r--   0        0        0      479 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/templates/blog-post.html
+-rw-r--r--   0        0        0      577 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/templates/blog.html
+-rw-r--r--   0        0        0    12658 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/templates/layout.html
+-rw-r--r--   0        0        0     1446 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/templates/macros/blog.html
+-rw-r--r--   0        0        0      813 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/templates/macros/pagination.html
+-rw-r--r--   0        0        0        1 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/templates/none.html
+-rw-r--r--   0        0        0      592 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/templates/page.html
+-rw-r--r--   0        0        0     4286 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/templates/single-layout.html
+-rw-r--r--   0        0        0     1450 2024-02-28 05:05:21.287379 pyglet-2.1.dev2/website/themes/lektor-icon/theme.ini
+-rw-r--r--   0        0        0     7809 1970-01-01 00:00:00.000000 pyglet-2.1.dev2/PKG-INFO
```

### Comparing `pyglet-2.1.dev1/LICENSE` & `pyglet-2.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/README.md` & `pyglet-2.1.dev2/README.md`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/__init__.py` & `pyglet-2.1.dev2/pyglet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import os
 import sys
 
 from typing import TYPE_CHECKING, Dict
 
 #: The release version
-version = '2.1.dev1'
+version = '2.1.dev2'
 __version__ = version
 
 MIN_PYTHON_VERSION = 3, 8
 MIN_PYTHON_VERSION_STR = '.'.join([str(v) for v in MIN_PYTHON_VERSION])
 
 if sys.version_info < MIN_PYTHON_VERSION:
     raise Exception(f"pyglet {version} requires Python {MIN_PYTHON_VERSION_STR} or newer.")
```

### Comparing `pyglet-2.1.dev1/pyglet/app/__init__.py` & `pyglet-2.1.dev2/pyglet/app/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/app/base.py` & `pyglet-2.1.dev2/pyglet/app/base.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/app/cocoa.py` & `pyglet-2.1.dev2/pyglet/app/cocoa.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/app/win32.py` & `pyglet-2.1.dev2/pyglet/app/win32.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/app/xlib.py` & `pyglet-2.1.dev2/pyglet/app/xlib.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/clock.py` & `pyglet-2.1.dev2/pyglet/clock.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/customtypes.py` & `pyglet-2.1.dev2/pyglet/customtypes.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/display/__init__.py` & `pyglet-2.1.dev2/pyglet/display/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/display/base.py` & `pyglet-2.1.dev2/pyglet/display/base.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/display/cocoa.py` & `pyglet-2.1.dev2/pyglet/display/cocoa.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/display/headless.py` & `pyglet-2.1.dev2/pyglet/display/headless.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/display/win32.py` & `pyglet-2.1.dev2/pyglet/display/win32.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/display/xlib.py` & `pyglet-2.1.dev2/pyglet/display/xlib.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/display/xlib_vidmoderestore.py` & `pyglet-2.1.dev2/pyglet/display/xlib_vidmoderestore.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/event.py` & `pyglet-2.1.dev2/pyglet/event.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/experimental/geoshader_sprite.py` & `pyglet-2.1.dev2/pyglet/experimental/geoshader_sprite.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/experimental/hidraw.py` & `pyglet-2.1.dev2/pyglet/experimental/hidraw.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/experimental/net.py` & `pyglet-2.1.dev2/pyglet/experimental/net.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/extlibs/png.py` & `pyglet-2.1.dev2/pyglet/extlibs/png.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/font/__init__.py` & `pyglet-2.1.dev2/pyglet/font/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/font/base.py` & `pyglet-2.1.dev2/pyglet/font/base.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/font/directwrite.py` & `pyglet-2.1.dev2/pyglet/font/directwrite.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/font/fontconfig.py` & `pyglet-2.1.dev2/pyglet/font/fontconfig.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/font/freetype.py` & `pyglet-2.1.dev2/pyglet/font/freetype.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/font/freetype_lib.py` & `pyglet-2.1.dev2/pyglet/font/freetype_lib.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/font/quartz.py` & `pyglet-2.1.dev2/pyglet/font/quartz.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/font/ttf.py` & `pyglet-2.1.dev2/pyglet/font/ttf.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/font/user.py` & `pyglet-2.1.dev2/pyglet/font/user.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/font/win32.py` & `pyglet-2.1.dev2/pyglet/font/win32.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/__init__.py` & `pyglet-2.1.dev2/pyglet/gl/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/agl.py` & `pyglet-2.1.dev2/pyglet/gl/agl.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/base.py` & `pyglet-2.1.dev2/pyglet/gl/base.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/cocoa.py` & `pyglet-2.1.dev2/pyglet/gl/cocoa.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/gl.py` & `pyglet-2.1.dev2/pyglet/gl/gl.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/gl_compat.py` & `pyglet-2.1.dev2/pyglet/gl/gl_compat.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/gl_info.py` & `pyglet-2.1.dev2/pyglet/gl/gl_info.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/glx.py` & `pyglet-2.1.dev2/pyglet/gl/glx.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/glx_info.py` & `pyglet-2.1.dev2/pyglet/gl/glx_info.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/glxext_arb.py` & `pyglet-2.1.dev2/pyglet/gl/glxext_arb.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/glxext_nv.py` & `pyglet-2.1.dev2/pyglet/gl/glxext_nv.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/headless.py` & `pyglet-2.1.dev2/pyglet/gl/headless.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/lib.py` & `pyglet-2.1.dev2/pyglet/gl/lib.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/lib_agl.py` & `pyglet-2.1.dev2/pyglet/gl/lib_agl.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/lib_glx.py` & `pyglet-2.1.dev2/pyglet/gl/lib_glx.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/lib_wgl.py` & `pyglet-2.1.dev2/pyglet/gl/lib_wgl.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/wgl.py` & `pyglet-2.1.dev2/pyglet/gl/wgl.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/wgl_info.py` & `pyglet-2.1.dev2/pyglet/gl/wgl_info.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/wglext_arb.py` & `pyglet-2.1.dev2/pyglet/gl/wglext_arb.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/wglext_nv.py` & `pyglet-2.1.dev2/pyglet/gl/wglext_nv.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/win32.py` & `pyglet-2.1.dev2/pyglet/gl/win32.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gl/xlib.py` & `pyglet-2.1.dev2/pyglet/gl/xlib.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/graphics/__init__.py` & `pyglet-2.1.dev2/pyglet/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/graphics/allocation.py` & `pyglet-2.1.dev2/pyglet/graphics/allocation.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/graphics/shader.py` & `pyglet-2.1.dev2/pyglet/graphics/shader.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/graphics/vertexarray.py` & `pyglet-2.1.dev2/pyglet/graphics/vertexarray.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/graphics/vertexbuffer.py` & `pyglet-2.1.dev2/pyglet/graphics/vertexbuffer.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/graphics/vertexdomain.py` & `pyglet-2.1.dev2/pyglet/graphics/vertexdomain.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gui/frame.py` & `pyglet-2.1.dev2/pyglet/gui/frame.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/gui/widgets.py` & `pyglet-2.1.dev2/pyglet/gui/widgets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Display different types of interactive widgets.
 """
 
 from __future__ import annotations
 
+from typing import Tuple
+
 import pyglet
 
 from pyglet.event import EventDispatcher
 from pyglet.graphics import Group
 from pyglet.text.caret import Caret
 from pyglet.text.layout import IncrementalTextLayout
 
 
 class WidgetBase(EventDispatcher):
 
-    def __init__(self, x, y, width, height):
+    def __init__(self, x: float, y: float, width: float, height: float) -> None:
         self._x = x
         self._y = y
         self._width = width
         self._height = height
         self._parent = None
         self._bg_group = None
         self._fg_group = None
@@ -53,37 +55,31 @@
         self._enabled = new_enabled
         self._set_enabled(new_enabled)
 
     def update_groups(self, order):
         pass
 
     @property
-    def x(self):
-        """X coordinate of the widget.
-
-        :type: int
-        """
+    def x(self) -> float:
+        """X coordinate of the widget."""
         return self._x
 
     @x.setter
-    def x(self, value):
+    def x(self, value: float):
         self._x = value
         self._update_position()
         self.dispatch_event("on_reposition", self)
 
     @property
-    def y(self):
-        """Y coordinate of the widget.
-
-        :type: int
-        """
+    def y(self) -> float:
+        """Y coordinate of the widget."""
         return self._y
 
     @y.setter
-    def y(self, value):
+    def y(self, value: float):
         self._y = value
         self._update_position()
         self.dispatch_event("on_reposition", self)
 
     @property
     def parent(self):
         """The frame this widget belongs to.
@@ -93,50 +89,43 @@
         return self._parent
 
     @parent.setter
     def parent(self, value):
         self._parent = value
 
     @property
-    def position(self):
+    def position(self) -> Tuple[float, float]:
         """The x, y coordinate of the widget as a tuple.
 
         :type: tuple(int, int)
         """
         return self._x, self._y
 
     @position.setter
-    def position(self, values):
+    def position(self, values: Tuple[float, float]):
         self._x, self._y = values
         self._update_position()
         self.dispatch_event("on_reposition", self)
 
     @property
-    def width(self):
-        """Width of the widget.
-
-        :type: int
-        """
+    def width(self) -> float:
+        """Width of the widget."""
         return self._width
 
     @property
-    def height(self):
-        """Height of the widget.
-
-        :type: int
-        """
+    def height(self) -> float:
+        """Height of the widget."""
         return self._height
 
     @property
-    def aabb(self):
+    def aabb(self) -> Tuple[float, float, float, float]:
         """Bounding box of the widget.
 
-        Expressed as (x, y, x + width, y + height)
-
-        :type: (int, int, int, int)
+        Expressed as (x, y, x + width, y + height),
+        also referred to as (left, bottom, right, top).
         """
         return self._x, self._y, self._x + self._width, self._y + self._height
 
     @property
     def value(self):
         """Query or set the Widget's value.
 
@@ -148,15 +137,15 @@
         """
         raise NotImplementedError("Value depends on control type!")
 
     @value.setter
     def value(self, value):
         raise NotImplementedError("Value depends on control type!")
 
-    def _check_hit(self, x, y):
+    def _check_hit(self, x: float, y: float) -> bool:
         return self._x < x < self._x + self._width and self._y < y < self._y + self._height
 
     def _update_position(self):
         raise NotImplementedError("Unable to reposition this Widget")
 
     def on_key_press(self, symbol, modifiers):
         pass
@@ -195,42 +184,42 @@
 class PushButton(WidgetBase):
     """Instance of a push button.
 
     Triggers the event 'on_press' when it is clicked by the mouse.
     Triggers the event 'on_release' when the mouse is released.
     """
 
-    def __init__(self, x, y, pressed, depressed, hover=None, batch=None, group=None):
+    def __init__(self, x, y, pressed, unpressed, hover=None, batch=None, group=None):
         """Create a push button.
 
         :Parameters:
             `x` : int
                 X coordinate of the push button.
             `y` : int
                 Y coordinate of the push button.
             `pressed` : `~pyglet.image.AbstractImage`
                 Image to display when the button is pressed.
-            `depresseed` : `~pyglet.image.AbstractImage`
-                Image to display when the button isn't pressed.
+            `unpressed` : `~pyglet.image.AbstractImage`
+                Image to display when the button is not pressed.
             `hover` : `~pyglet.image.AbstractImage`
                 Image to display when the button is being hovered over.
             `batch` : `~pyglet.graphics.Batch`
                 Optional batch to add the push button to.
             `group` : `~pyglet.graphics.Group`
                 Optional parent group of the push button.
         """
-        super().__init__(x, y, depressed.width, depressed.height)
+        super().__init__(x, y, unpressed.width, unpressed.height)
         self._pressed_img = pressed
-        self._depressed_img = depressed
-        self._hover_img = hover or depressed
+        self._unpressed_img = unpressed
+        self._hover_img = hover or unpressed
 
         self._batch = batch or pyglet.graphics.Batch()
         self._user_group = group
         bg_group = Group(order=0, parent=group)
-        self._sprite = pyglet.sprite.Sprite(self._depressed_img, x, y, batch=batch, group=bg_group)
+        self._sprite = pyglet.sprite.Sprite(self._unpressed_img, x, y, batch=batch, group=bg_group)
 
         self._pressed = False
 
     def _update_position(self):
         self._sprite.position = self._x, self._y, 0
 
     @property
@@ -238,42 +227,42 @@
         """Whether the button is pressed or not."""
         return self._pressed
 
     @value.setter
     def value(self, value):
         assert type(value) is bool, "This Widget's value must be True or False."
         self._pressed = value
-        self._sprite.image = self._pressed_img if self._pressed else self._depressed_img
+        self._sprite.image = self._pressed_img if self._pressed else self._unpressed_img
 
     def update_groups(self, order):
         self._sprite.group = Group(order=order + 1, parent=self._user_group)
 
     def on_mouse_press(self, x, y, buttons, modifiers):
         if not self.enabled or not self._check_hit(x, y):
             return
         self._sprite.image = self._pressed_img
         self._pressed = True
         self.dispatch_event('on_press', self)
 
     def on_mouse_release(self, x, y, buttons, modifiers):
         if not self.enabled or not self._pressed:
             return
-        self._sprite.image = self._hover_img if self._check_hit(x, y) else self._depressed_img
+        self._sprite.image = self._hover_img if self._check_hit(x, y) else self._unpressed_img
         self._pressed = False
         self.dispatch_event('on_release', self)
 
     def on_mouse_motion(self, x, y, dx, dy):
         if not self.enabled or self._pressed:
             return
-        self._sprite.image = self._hover_img if self._check_hit(x, y) else self._depressed_img
+        self._sprite.image = self._hover_img if self._check_hit(x, y) else self._unpressed_img
 
     def on_mouse_drag(self, x, y, dx, dy, buttons, modifiers):
         if not self.enabled or self._pressed:
             return
-        self._sprite.image = self._hover_img if self._check_hit(x, y) else self._depressed_img
+        self._sprite.image = self._hover_img if self._check_hit(x, y) else self._unpressed_img
 
     def on_press(self, widget: PushButton):
         """Event: Dispatched when the button is clicked."""
 
     def on_release(self, widget: PushButton):
         """Event: Dispatched when the button is released."""
 
@@ -285,15 +274,15 @@
 class ToggleButton(PushButton):
     """Instance of a toggle button.
 
     Triggers the event 'on_toggle' when the mouse is pressed or released.
     """
 
     def _get_release_image(self, x, y):
-        return self._hover_img if self._check_hit(x, y) else self._depressed_img
+        return self._hover_img if self._check_hit(x, y) else self._unpressed_img
 
     def on_mouse_press(self, x, y, buttons, modifiers):
         if not self.enabled or not self._check_hit(x, y):
             return
         self._pressed = not self._pressed
         self._sprite.image = self._pressed_img if self._pressed else self._get_release_image(x, y)
         self.dispatch_event('on_toggle', self, self._pressed)
```

### Comparing `pyglet-2.1.dev1/pyglet/image/__init__.py` & `pyglet-2.1.dev2/pyglet/image/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/image/animation.py` & `pyglet-2.1.dev2/pyglet/image/animation.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/image/atlas.py` & `pyglet-2.1.dev2/pyglet/image/atlas.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/image/buffer.py` & `pyglet-2.1.dev2/pyglet/image/buffer.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/image/codecs/__init__.py` & `pyglet-2.1.dev2/pyglet/image/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/image/codecs/bmp.py` & `pyglet-2.1.dev2/pyglet/image/codecs/bmp.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/image/codecs/dds.py` & `pyglet-2.1.dev2/pyglet/image/codecs/dds.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/image/codecs/gdiplus.py` & `pyglet-2.1.dev2/pyglet/image/codecs/gdiplus.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/image/codecs/gdkpixbuf2.py` & `pyglet-2.1.dev2/pyglet/image/codecs/gdkpixbuf2.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/image/codecs/gif.py` & `pyglet-2.1.dev2/pyglet/image/codecs/gif.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/image/codecs/pil.py` & `pyglet-2.1.dev2/pyglet/image/codecs/pil.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/image/codecs/png.py` & `pyglet-2.1.dev2/pyglet/image/codecs/png.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/image/codecs/quartz.py` & `pyglet-2.1.dev2/pyglet/image/codecs/quartz.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/image/codecs/s3tc.py` & `pyglet-2.1.dev2/pyglet/image/codecs/s3tc.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/image/codecs/wic.py` & `pyglet-2.1.dev2/pyglet/image/codecs/wic.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/info.py` & `pyglet-2.1.dev2/pyglet/info.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/input/__init__.py` & `pyglet-2.1.dev2/pyglet/input/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/input/base.py` & `pyglet-2.1.dev2/pyglet/input/base.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/input/controller.py` & `pyglet-2.1.dev2/pyglet/input/controller.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/input/controller_db.py` & `pyglet-2.1.dev2/pyglet/input/controller_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,45 @@
 from pyglet import compat_platform
 
 
 # This file is automatically generated by 'pyglet/tools/gen_controller_db.py'
-# Generated on: Wed Aug 30 15:53:55 2023
+# Generated on: Wed Apr  3 09:38:16 2024
 
 if compat_platform.startswith("linux"):
     mapping_list = [
-"03000000c82d00000090000011010000,8BitDo FC30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a5,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000090000011010000,8BitDo FC30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a5,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"05000000c82d00001038000000010000,8BitDo FC30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "05000000c82d00001038000000010000,8BitDo FC30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00000650000011010000,8BitDo M30 Gamepad,a:b0,b:b1,back:b10,guide:b2,leftshoulder:b6,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b7,righttrigger:a5,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "05000000c82d00005106000000010000,8BitDo M30 Gamepad,a:b1,b:b0,back:b10,guide:b2,leftshoulder:b6,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,righttrigger:a4,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00001590000011010000,8BitDo N30 Pro 2,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a5,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00001590000011010000,8BitDo N30 Pro 2,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a5,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"05000000c82d00006528000000010000,8BitDo N30 Pro 2,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "05000000c82d00006528000000010000,8BitDo N30 Pro 2,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"030000003512000012ab000010010000,8BitDo NES30 Gamepad,a:b0,b:b1,back:b10,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b6,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "030000003512000012ab000010010000,8BitDo NES30 Gamepad,a:b1,b:b0,back:b10,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b6,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000022000000090000011010000,8BitDo NES30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000022000000090000011010000,8BitDo NES30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00000190000011010000,8BitDo NES30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a5,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000190000011010000,8BitDo NES30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a5,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"05000000203800000900000000010000,8BitDo NES30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "05000000203800000900000000010000,8BitDo NES30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"05000000c82d00002038000000010000,8BitDo NES30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "05000000c82d00002038000000010000,8BitDo NES30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000020000000000000,8BitDo Pro 2 Wired Controller for Xbox,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "06000000c82d00000020000006010000,8BitDo Pro 2 Wired Controller for Xbox,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
-"03000000c82d00000660000011010000,8BitDo Pro 2,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000660000011010000,8BitDo Pro 2,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"05000000c82d00000660000000010000,8BitDo Pro 2,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "05000000c82d00000660000000010000,8BitDo Pro 2,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"05000000c82d00000061000000010000,8BitDo SF30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "05000000c82d00000061000000010000,8BitDo SF30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"05000000102800000900000000010000,8BitDo SFC30 Gamepad,a:b0,b:b1,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "05000000102800000900000000010000,8BitDo SFC30 Gamepad,a:b1,b:b0,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"05000000c82d00003028000000010000,8BitDo SFC30 Gamepad,a:b0,b:b1,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "05000000c82d00003028000000010000,8BitDo SFC30 Gamepad,a:b1,b:b0,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00000260000011010000,8BitDo SN30 Pro+,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000260000011010000,8BitDo SN30 Pro+,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"05000000c82d00000261000000010000,8BitDo SN30 Pro+,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "05000000c82d00000261000000010000,8BitDo SN30 Pro+,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00000160000011010000,8BitDo SN30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a5,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000160000011010000,8BitDo SN30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a5,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"030000003512000020ab000010010000,8BitDo SNES30 Gamepad,a:b0,b:b1,back:b10,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b6,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "030000003512000020ab000010010000,8BitDo SNES30 Gamepad,a:b1,b:b0,back:b10,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b6,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"05000000202800000900000000010000,8BitDo SNES30 Gamepad,a:b0,b:b1,back:b10,dpdown:b122,dpleft:b119,dpright:b120,dpup:b117,leftshoulder:b6,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "05000000202800000900000000010000,8BitDo SNES30 Gamepad,a:b1,b:b0,back:b10,dpdown:b122,dpleft:b119,dpright:b120,dpup:b117,leftshoulder:b6,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00001130000011010000,8BitDo Ultimate Wired Controller,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,misc1:b26,paddle1:b24,paddle2:b25,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,",
 "03000000c82d00001330000011010000,8BitDo Ultimate Wireless Controller,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,misc1:b26,paddle1:b23,paddle2:b19,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,",
-"03000000c82d00001890000011010000,8BitDo Zero 2,a:b0,b:b1,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00001890000011010000,8BitDo Zero 2,a:b1,b:b0,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"05000000c82d00003032000000010000,8BitDo Zero 2,a:b0,b:b1,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "05000000c82d00003032000000010000,8BitDo Zero 2,a:b1,b:b0,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"05000000a00500003232000001000000,8BitDo Zero Gamepad,a:b0,b:b1,back:b10,dpdown:b122,dpleft:b119,dpright:b120,dpup:b117,leftshoulder:b6,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "05000000a00500003232000001000000,8BitDo Zero Gamepad,a:b1,b:b0,back:b10,dpdown:b122,dpleft:b119,dpright:b120,dpup:b117,leftshoulder:b6,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"05000000a00500003232000008010000,8BitDo Zero Gamepad,a:b0,b:b1,back:b10,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b6,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "05000000a00500003232000008010000,8BitDo Zero Gamepad,a:b1,b:b0,back:b10,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b6,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000031000011010000,8Bitdo Receiver,a:b1,b:b0,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b4,y:b3,",
-"03000000c82d00001290000011010000,8Bitdo SN30 Gamepad,a:b0,b:b1,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00001290000011010000,8Bitdo SN30 Gamepad,a:b1,b:b0,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"05000000c82d00006228000000010000,8Bitdo SN30 Gamepad,a:b0,b:b1,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "05000000c82d00006228000000010000,8Bitdo SN30 Gamepad,a:b1,b:b0,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "05000000050b00000045000031000000,ASUS Gamepad,a:b0,b:b1,back:b9,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b6,leftshoulder:b4,leftstick:b7,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b8,righttrigger:a4,rightx:a2,righty:a3,start:b10,x:b2,y:b3,",
 "05000000050b00000045000040000000,ASUS Gamepad,a:b0,b:b1,back:b9,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b6,leftshoulder:b4,leftstick:b7,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b8,righttrigger:a4,rightx:a2,righty:a3,start:b10,x:b2,y:b3,",
 "03000000050b00000579000011010000,ASUS ROG Kunai 3 Gamepad,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,misc1:b36,paddle1:b52,paddle2:b53,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,",
 "05000000050b00000679000000010000,ASUS ROG Kunai 3 Gamepad,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,misc1:b21,paddle1:b22,paddle2:b23,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,",
 "030000006f0e00003901000020060000,Afterglow Controller for Xbox One,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "030000006f0e00003901000000430000,Afterglow Prismatic Controller,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
@@ -75,14 +49,15 @@
 "03000000491900001904000011010000,Amazon Luna Controller,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,misc1:b9,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b7,x:b2,y:b3,",
 "05000000710100001904000000010000,Amazon Luna Controller,a:b0,b:b1,back:b9,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b10,leftshoulder:b4,leftstick:b7,lefttrigger:a5,leftx:a0,lefty:a1,misc1:b11,rightshoulder:b5,rightstick:b8,righttrigger:a4,rightx:a2,righty:a3,start:b6,x:b2,y:b3,",
 "03000000790000003018000011010000,Arcade Fightstick F300,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,righttrigger:b7,start:b9,x:b0,y:b3,",
 "03000000503200000110000000000000,Atari Classic Controller,a:b0,back:b2,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b4,start:b3,x:b1,",
 "05000000503200000110000000000000,Atari Classic Controller,a:b0,back:b2,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b4,start:b3,x:b1,",
 "03000000503200000210000000000000,Atari Game Controller,a:b0,b:b1,back:b9,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b10,leftshoulder:b4,leftstick:b6,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b7,righttrigger:a4,rightx:a2,righty:a3,start:b8,x:b2,y:b3,",
 "05000000503200000210000000000000,Atari Game Controller,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b3,y:b2,",
+"05000000503200000210000000000000128804098,Atari Game Controller,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b3,y:b2,",
 "030000005e0400008e02000047010000,Atari Xbox 360 Game Controller,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "03000000c62400001b89000011010000,BDA MOGA XP5-X Plus,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,",
 "03000000d62000002a79000011010000,BDA PS4 Fightpad,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "03000000120c0000f70e000011010000,Brook Universal Fighting Board,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:,lefty:,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:,righty:,start:b9,x:b0,y:b3,",
 "03000000b40400000a01000000010000,CYPRESS USB Gamepad,a:b0,b:b1,back:b5,guide:b2,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b8,x:b3,y:b4,",
 "03000000ffff0000ffff000000010000,Chinese-made Xbox Controller,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b5,leftstick:b8,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b2,rightstick:b9,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b3,y:b4,",
 "03000000e82000006058000001010000,Cideko AK08b,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b0,",
@@ -114,15 +89,15 @@
 "030000000d0f00006a00000011010000,HORI CO. LTD. Real Arcade Pro.4,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "030000000d0f00006b00000011010000,HORI CO. LTD. Real Arcade Pro.4,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "030000000d0f00005001000009040000,HORI Fighting Commander OCTA,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "030000000d0f00008400000011010000,HORI Fighting Commander,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "030000000d0f00008500000010010000,HORI Fighting Commander,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "030000000d0f00008800000011010000,HORI Fighting Stick mini 4 (PS3),a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,rightshoulder:b5,rightstick:b11,righttrigger:b7,start:b9,x:b0,y:b3,",
 "030000000d0f00008700000011010000,HORI Fighting Stick mini 4 (PS4),a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,rightshoulder:b5,rightstick:b11,righttrigger:a4,start:b9,x:b0,y:b3,",
-"030000000d0f0000d800000072056800,HORI Real Arcade Pro S,a:b0,b:b1,back:b4,dpdown:b12,dpleft:b13,dpright:b14,dpup:b11,guide:b5,leftshoulder:b9,leftstick:b7,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b10,rightstick:b8,righttrigger:a5,rightx:a2,righty:a3,start:b6,x:b2,y:b3,",
+"030000000d0f0000d800000072056800,HORI Real Arcade Pro S,a:b0,b:b1,back:b4,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b5,leftshoulder:b9,leftstick:b7,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b10,rightstick:b8,righttrigger:a5,rightx:a2,righty:a3,start:b6,x:b2,y:b3,",
 "030000000d0f0000aa00000011010000,HORI Real Arcade Pro,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b0,",
 "030000000d0f00006e00000011010000,HORIPAD 4 (PS3),a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "030000000d0f00006600000011010000,HORIPAD 4 (PS4),a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "030000000d0f00006700000001010000,HORIPAD ONE,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "06000000adde0000efbe000002010000,Hidromancer Game Controller,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "03000000d81400000862000011010000,HitBox (PS3/PC) Analog Mode,a:b1,b:b2,back:b8,guide:b9,leftshoulder:b4,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,righttrigger:b7,start:b12,x:b0,y:b3,",
 "030000000d0f00005f00000011010000,Hori Fighting Commander 4 (PS3),a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
@@ -178,40 +153,26 @@
 "05000000d6200000ad0d000001000000,Moga Pro,a:b0,b:b1,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b7,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b8,righttrigger:a4,rightx:a2,righty:a3,start:b6,x:b2,y:b3,",
 "030000006b140000010c000010010000,NACON GC-400ES,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b2,y:b3,",
 "030000001008000001e5000010010000,NEXT SNES Controller,a:b2,b:b1,back:b8,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b4,rightshoulder:b6,start:b9,x:b3,y:b0,",
 "03000000550900001472000011010000,NVIDIA Controller v01.04,a:b0,b:b1,back:b14,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b17,leftshoulder:b4,leftstick:b7,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b8,righttrigger:a4,rightx:a2,righty:a5,start:b6,x:b2,y:b3,",
 "03000000550900001072000011010000,NVIDIA Controller,a:b0,b:b1,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b13,leftshoulder:b4,leftstick:b8,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b9,righttrigger:a4,rightx:a2,righty:a3,start:b7,x:b2,y:b3,",
 "030000004b120000014d000000010000,NYKO AIRFLO EX,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b10,leftshoulder:b4,leftstick:b11,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b12,righttrigger:b7,rightx:a3,righty:a2,start:b9,x:b2,y:b3,",
 "03000000451300000830000010010000,NYKO CORE,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
-"03000000790000004318000010010000,Nintendo GameCube Controller,a:b1,b:b2,dpdown:b14,dpleft:b15,dpright:b13,dpup:b12,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b7,righttrigger:a4,rightx:a5,righty:a2,start:b9,x:b0,y:b3,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000790000004318000010010000,Nintendo GameCube Controller,a:b1,b:b0,dpdown:b14,dpleft:b15,dpright:b13,dpup:b12,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b7,righttrigger:a4,rightx:a5,righty:a2,start:b9,x:b2,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"030000007e0500003703000000016800,Nintendo GameCube Controller,a:b0,b:b2,dpdown:b6,dpleft:b4,dpright:b5,dpup:b7,lefttrigger:a4,leftx:a0,lefty:a1~,rightshoulder:b9,righttrigger:a5,rightx:a2,righty:a3~,start:b8,x:b1,y:b3,",
-"050000007e0500000620000001800000,Nintendo Switch Joy-Con (L),a:b15,b:b16,guide:b4,leftshoulder:b6,leftstick:b12,leftx:a1,lefty:a0~,rightshoulder:b8,start:b9,x:b17,y:b14,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "050000007e0500000620000001800000,Nintendo Switch Joy-Con (L),a:b16,b:b15,guide:b4,leftshoulder:b6,leftstick:b12,leftx:a1,lefty:a0~,rightshoulder:b8,start:b9,x:b14,y:b17,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"060000007e0500000620000000000000,Nintendo Switch Joy-Con (L/R),a:b1,b:b0,back:b9,dpdown:b15,dpleft:b16,dpright:b17,dpup:b14,leftshoulder:b5,leftstick:b12,lefttrigger:b7,leftx:a0,lefty:a1,rightshoulder:b6,rightstick:b13,righttrigger:b8,rightx:a2,righty:a3,start:b10,x:b2,y:b3,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "060000007e0500000620000000000000,Nintendo Switch Joy-Con (L/R),a:b0,b:b1,back:b9,dpdown:b15,dpleft:b16,dpright:b17,dpup:b14,leftshoulder:b5,leftstick:b12,lefttrigger:b7,leftx:a0,lefty:a1,rightshoulder:b6,rightstick:b13,righttrigger:b8,rightx:a2,righty:a3,start:b10,x:b3,y:b2,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"060000007e0500000820000000000000,Nintendo Switch Joy-Con (L/R),a:b1,b:b0,back:b9,dpdown:b15,dpleft:b16,dpright:b17,dpup:b14,guide:b11,leftshoulder:b5,leftstick:b12,lefttrigger:b7,leftx:a0,lefty:a1,rightshoulder:b6,rightstick:b13,righttrigger:b8,rightx:a2,righty:a3,start:b10,x:b2,y:b3,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "060000007e0500000820000000000000,Nintendo Switch Joy-Con (L/R),a:b0,b:b1,back:b9,dpdown:b15,dpleft:b16,dpright:b17,dpup:b14,guide:b11,leftshoulder:b5,leftstick:b12,lefttrigger:b7,leftx:a0,lefty:a1,rightshoulder:b6,rightstick:b13,righttrigger:b8,rightx:a2,righty:a3,start:b10,x:b3,y:b2,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"050000007e0500000720000001800000,Nintendo Switch Joy-Con (R),a:b2,b:b1,guide:b9,leftshoulder:b4,leftstick:b10,leftx:a1~,lefty:a0,rightshoulder:b6,start:b8,x:b3,y:b0,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "050000007e0500000720000001800000,Nintendo Switch Joy-Con (R),a:b1,b:b2,guide:b9,leftshoulder:b4,leftstick:b10,leftx:a1~,lefty:a0,rightshoulder:b6,start:b8,x:b0,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000d620000013a7000011010000,Nintendo Switch PowerA Controller,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b0,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000d620000013a7000011010000,Nintendo Switch PowerA Controller,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000d620000011a7000011010000,Nintendo Switch PowerA Core Plus Controller,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b0,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000d620000011a7000011010000,Nintendo Switch PowerA Core Plus Controller,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"030000007e0500000920000011810000,Nintendo Switch Pro Controller,a:b1,b:b0,back:b9,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b11,leftshoulder:b5,leftstick:b12,lefttrigger:b7,leftx:a0,lefty:a1,misc1:b4,rightshoulder:b6,rightstick:b13,righttrigger:b8,rightx:a2,righty:a3,start:b10,x:b2,y:b3,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "030000007e0500000920000011810000,Nintendo Switch Pro Controller,a:b0,b:b1,back:b9,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b11,leftshoulder:b5,leftstick:b12,lefttrigger:b7,leftx:a0,lefty:a1,misc1:b4,rightshoulder:b6,rightstick:b13,righttrigger:b8,rightx:a2,righty:a3,start:b10,x:b3,y:b2,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"050000004c69632050726f20436f6e00,Nintendo Switch Pro Controller,crc:15b7,a:b1,b:b0,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,misc1:b13,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b2,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "050000004c69632050726f20436f6e00,Nintendo Switch Pro Controller,crc:15b7,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,misc1:b13,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b2,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"050000007e0500000920000001000000,Nintendo Switch Pro Controller,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b2,y:b3,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "050000007e0500000920000001000000,Nintendo Switch Pro Controller,a:b1,b:b0,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b2,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"050000007e0500000920000001800000,Nintendo Switch Pro Controller,a:b1,b:b0,back:b9,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b11,leftshoulder:b5,leftstick:b12,lefttrigger:b7,leftx:a0,lefty:a1,rightshoulder:b6,rightstick:b13,righttrigger:b8,rightx:a2,righty:a3,start:b10,x:b2,y:b3,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "050000007e0500000920000001800000,Nintendo Switch Pro Controller,a:b0,b:b1,back:b9,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b11,leftshoulder:b5,leftstick:b12,lefttrigger:b7,leftx:a0,lefty:a1,rightshoulder:b6,rightstick:b13,righttrigger:b8,rightx:a2,righty:a3,start:b10,x:b3,y:b2,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"050000007e0500000603000000060000,Nintendo Wii Remote Classic Controller,crc:0d8a,a:b0,b:b1,back:b10,dpdown:b14,dpleft:b12,dpright:b13,dpup:b11,guide:b8,leftshoulder:b4,lefttrigger:b6,leftx:a0,lefty:a1~,rightshoulder:b5,righttrigger:b7,rightx:a2,righty:a3~,start:b9,x:b2,y:b3,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "050000007e0500000603000000060000,Nintendo Wii Remote Classic Controller,crc:0d8a,a:b1,b:b0,back:b10,dpdown:b14,dpleft:b12,dpright:b13,dpup:b11,guide:b8,leftshoulder:b4,lefttrigger:b6,leftx:a0,lefty:a1~,rightshoulder:b5,righttrigger:b7,rightx:a2,righty:a3~,start:b9,x:b3,y:b2,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"050000007e0500003003000001000000,Nintendo Wii Remote Pro Controller,a:b1,b:b0,back:b8,dpdown:b14,dpleft:b15,dpright:b16,dpup:b13,guide:b10,leftshoulder:b4,leftstick:b11,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b12,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b2,y:b3,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "050000007e0500003003000001000000,Nintendo Wii Remote Pro Controller,a:b0,b:b1,back:b8,dpdown:b14,dpleft:b15,dpright:b16,dpup:b13,guide:b10,leftshoulder:b4,leftstick:b11,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b12,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b2,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "050000007e0500000603000000060000,Nintendo Wii Remote,crc:60be,a:b1,b:b0,back:b4,dpdown:b8,dpleft:b6,dpright:b7,dpup:b5,guide:b2,start:b3,x:b9,y:b10,",
 "05000000010000000100000003000000,Nintendo Wiimote,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b10,leftshoulder:b4,leftstick:b11,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b12,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b2,y:b3,",
 "030000000d0500000308000010010000,Nostromo n45 Dual Analog Gamepad,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b9,leftshoulder:b4,leftstick:b12,lefttrigger:b5,leftx:a0,lefty:a1,rightshoulder:b6,rightstick:b11,righttrigger:b7,rightx:a3,righty:a2,start:b10,x:b2,y:b3,",
 "05000000362800000100000002010000,OUYA Game Controller,a:b0,b:b3,dpdown:b9,dpleft:b10,dpright:b11,dpup:b8,guide:b14,leftshoulder:b4,leftstick:b6,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b7,righttrigger:a5,rightx:a3,righty:a4,x:b1,y:b2,",
 "05000000362800000100000003010000,OUYA Game Controller,a:b0,b:b3,dpdown:b9,dpleft:b10,dpright:b11,dpup:b8,guide:b14,leftshoulder:b4,leftstick:b6,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b7,righttrigger:a5,rightx:a3,righty:a4,x:b1,y:b2,",
 "030000005e0400000202000000010000,Old Xbox pad,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b5,leftstick:b8,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b2,rightstick:b9,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b3,y:b4,",
@@ -266,15 +227,14 @@
 "030000008916000000fe000024010000,Razer Sabertooth,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "03000000c6240000045d000024010000,Razer Sabertooth,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "03000000c6240000045d000025010000,Razer Sabertooth,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "03000000321500000009000011010000,Razer Serval,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a4,rightx:a2,righty:a3,start:b7,x:b2,y:b3,",
 "050000003215000000090000163a0000,Razer Serval,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a4,rightx:a2,righty:a3,start:b7,x:b2,y:b3,",
 "0300000032150000030a000001010000,Razer Wildcat,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "0300000000f000000300000000010000,RetroPad,a:b1,b:b5,back:b2,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b3,x:b0,y:b4,",
-"03000000790000001100000010010000,Retrolink SNES Controller,a:b1,b:b2,back:b8,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b4,rightshoulder:b5,start:b9,x:b0,y:b3,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000790000001100000010010000,Retrolink SNES Controller,a:b2,b:b1,back:b8,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b4,rightshoulder:b5,start:b9,x:b3,y:b0,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "030000006b140000130d000011010000,Revolution Pro Controller 3,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "030000006b140000010d000011010000,Revolution Pro Controller,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "030000006f0e00001e01000011010000,Rock Candy PS3 Controller,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "030000006f0e00004601000001010000,Rock Candy Xbox One Controller,a:b0,b:b1,back:b6,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "030000006f0e00001f01000000010000,Rock Candy,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "03000000632500007505000010010000,SHANWAN PS3/PC Gamepad,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b0,",
@@ -298,14 +258,15 @@
 "03000000de2800000211000011010000,Steam Controller,a:b2,b:b3,back:b10,dpdown:+a5,dpleft:-a4,dpright:+a4,dpup:-a5,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:a7,leftx:a0,lefty:a1,paddle1:b15,paddle2:b16,rightshoulder:b7,rightstick:b14,righttrigger:a6,rightx:a2,righty:a3,start:b11,x:b4,y:b5,",
 "03000000de2800004211000001000000,Steam Controller,a:b0,b:b1,back:b6,dpdown:b14,dpleft:b15,dpright:b13,dpup:b12,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,paddle1:b11,paddle2:b10,rightshoulder:b5,righttrigger:a3,start:b7,x:b2,y:b3,",
 "03000000de2800004211000011010000,Steam Controller,a:b2,b:b3,back:b10,dpdown:+a5,dpleft:-a4,dpright:+a4,dpup:-a5,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:a7,leftx:a0,lefty:a1,paddle1:b15,paddle2:b16,rightshoulder:b7,rightstick:b14,righttrigger:a6,rightx:a2,righty:a3,start:b11,x:b4,y:b5,",
 "03000000de280000fc11000001000000,Steam Controller,a:b0,b:b1,back:b6,dpdown:b14,dpleft:b15,dpright:b13,dpup:b12,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "05000000de2800000212000001000000,Steam Controller,a:b0,b:b1,back:b6,dpdown:b14,dpleft:b15,dpright:b13,dpup:b12,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,paddle1:b11,paddle2:b10,rightshoulder:b5,righttrigger:a3,start:b7,x:b2,y:b3,",
 "05000000de2800000511000001000000,Steam Controller,a:b0,b:b1,back:b6,dpdown:b14,dpleft:b15,dpright:b13,dpup:b12,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,paddle1:b11,paddle2:b10,rightshoulder:b5,righttrigger:a3,start:b7,x:b2,y:b3,",
 "05000000de2800000611000001000000,Steam Controller,a:b0,b:b1,back:b6,dpdown:b14,dpleft:b15,dpright:b13,dpup:b12,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,paddle1:b11,paddle2:b10,rightshoulder:b5,righttrigger:a3,start:b7,x:b2,y:b3,",
+"03000000de2800000512000000016800,Steam Deck,a:b0,b:b1,back:b4,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b5,leftshoulder:b9,leftstick:b7,lefttrigger:a4,leftx:a0,lefty:a1,misc1:b11,paddle1:b12,paddle2:b13,paddle3:b14,paddle4:b15,rightshoulder:b10,rightstick:b8,righttrigger:a5,rightx:a2,righty:a3,start:b6,x:b2,y:b3,",
 "03000000de2800000512000011010000,Steam Deck,a:b3,b:b4,back:b11,dpdown:b17,dpleft:b18,dpright:b19,dpup:b16,guide:b13,leftshoulder:b7,leftstick:b14,lefttrigger:a9,leftx:a0,lefty:a1,misc1:b2,paddle1:b21,paddle2:b20,paddle3:b23,paddle4:b22,rightshoulder:b8,rightstick:b15,righttrigger:a8,rightx:a2,righty:a3,start:b12,x:b5,y:b6,",
 "03000000de280000ff11000001000000,Steam Virtual Gamepad,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "0500000011010000311400001b010000,SteelSeries Stratus Duo,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b32,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,",
 "05000000110100001914000009010000,SteelSeries Stratus XL,a:b0,b:b1,back:b17,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b18,leftshoulder:b6,leftstick:b13,lefttrigger:+a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:+a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,",
 "03000000ad1b000038f0000090040000,Street Fighter IV FightStick TE,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "03000000666600000488000000010000,Super Joy Box 5 Pro,a:b2,b:b1,back:b9,dpdown:b14,dpleft:b15,dpright:b13,dpup:b12,leftshoulder:b6,leftstick:b10,lefttrigger:b4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b11,righttrigger:b5,rightx:a2,righty:a3,start:b8,x:b3,y:b0,",
 "0300000000f00000f100000000010000,Super RetroPort,a:b1,b:b5,back:b2,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b3,x:b0,y:b4,",
@@ -338,63 +299,42 @@
 "050000005e040000e002000003090000,Xbox One Wireless Controller,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b10,leftshoulder:b4,leftstick:b8,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b9,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "050000005e040000fd02000003090000,Xbox One Wireless Controller,a:b0,b:b1,back:b15,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,guide:b16,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,",
 "05000000172700004431000029010000,XiaoMi Game Controller,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b20,leftshoulder:b6,leftstick:b13,lefttrigger:a7,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a6,rightx:a2,righty:a5,start:b11,x:b3,y:b4,",
 "03000000c0160000e105000010010000,Xin-Mo Dual Arcade,crc:82d5,a:b1,b:b2,back:b9,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,rightshoulder:b4,righttrigger:b5,start:b8,x:b0,y:b3,",
 "03000000120c0000100e000011010000,ZEROPLUS P4 Gamepad,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "03000000120c0000101e000011010000,ZEROPLUS P4 Wired Gamepad,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "03000000666600006706000000010000,boom PSX to PC Converter,a:b2,b:b1,back:b8,dpdown:b14,dpleft:b15,dpright:b13,dpup:b12,leftshoulder:b6,leftstick:b9,lefttrigger:b4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b10,righttrigger:b5,rightx:a2,righty:a3,start:b11,x:b3,y:b0,",
-"030000000d0f00000d00000000010000,hori,a:b0,b:b6,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b10,leftshoulder:b3,leftx:b4,lefty:b5,rightshoulder:b7,start:b9,x:b1,y:b2,",
-"03000000830500006020000010010000,iBuffalo SNES Controller,a:b0,b:b1,back:b6,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b4,rightshoulder:b5,start:b7,x:b2,y:b3,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000830500006020000010010000,iBuffalo SNES Controller,a:b1,b:b0,back:b6,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b4,rightshoulder:b5,start:b7,x:b3,y:b2,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "050000006964726f69643a636f6e0000,idroid:con,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "03000000b50700001503000010010000,impact,a:b2,b:b3,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b5,leftx:a0,lefty:a1,rightshoulder:b6,rightstick:b11,righttrigger:b7,rightx:a3,righty:a2,start:b9,x:b0,y:b1,",
 "030000009b2800008000000020020000,raphnet technologies 1-player WUSBMote v2.2,a:b1,b:b4,back:b2,dpdown:b13,dpleft:b14,dpright:b15,dpup:b12,leftshoulder:b6,rightshoulder:b7,start:b3,x:b0,y:b5,",
 "030000009b2800000300000001010000,raphnet.net 4nes4snes v1.5,a:b0,b:b4,back:b2,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b3,x:b1,y:b5,",
 ]
 elif compat_platform.startswith("darwin"):
     mapping_list = [
-"03000000c82d00000090000001000000,8BitDo FC30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a5,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000090000001000000,8BitDo FC30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a5,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00001038000000010000,8BitDo FC30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00001038000000010000,8BitDo FC30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00000650000001000000,8BitDo M30 Gamepad,a:b0,b:b1,back:b10,guide:b2,leftshoulder:b6,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b7,righttrigger:a5,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000650000001000000,8BitDo M30 Gamepad,a:b1,b:b0,back:b10,guide:b2,leftshoulder:b6,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b7,righttrigger:a5,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00005106000000010000,8BitDo M30 Gamepad,a:b0,b:b1,back:b10,guide:b2,leftshoulder:b6,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,righttrigger:a4,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00005106000000010000,8BitDo M30 Gamepad,a:b1,b:b0,back:b10,guide:b2,leftshoulder:b6,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,righttrigger:a4,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00001590000001000000,8BitDo N30 Pro 2,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a5,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00001590000001000000,8BitDo N30 Pro 2,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a5,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00006528000000010000,8BitDo N30 Pro 2,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00006528000000010000,8BitDo N30 Pro 2,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"030000003512000012ab000001000000,8BitDo NES30 Gamepad,a:b0,b:b1,back:b10,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b6,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "030000003512000012ab000001000000,8BitDo NES30 Gamepad,a:b1,b:b0,back:b10,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b6,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000022000000090000001000000,8BitDo NES30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000022000000090000001000000,8BitDo NES30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000203800000900000000010000,8BitDo NES30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000203800000900000000010000,8BitDo NES30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00000660000000020000,8BitDo Pro 2,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000660000000020000,8BitDo Pro 2,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000102800000900000000000000,8BitDo SFC30 Gamepad,a:b0,b:b1,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000102800000900000000000000,8BitDo SFC30 Gamepad,a:b1,b:b0,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00001290000001000000,8BitDo SN30 Gamepad,a:b0,b:b1,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00001290000001000000,8BitDo SN30 Gamepad,a:b1,b:b0,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00000260000001000000,8BitDo SN30 Pro+,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000260000001000000,8BitDo SN30 Pro+,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00000261000000010000,8BitDo SN30 Pro+,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000261000000010000,8BitDo SN30 Pro+,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00000160000001000000,8BitDo SN30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a5,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000160000001000000,8BitDo SN30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:a4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a5,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00001130000000020000,8BitDo Ultimate Wired Controller,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,misc1:b26,paddle1:b24,paddle2:b25,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,",
 "03000000c82d00001330000000020000,8BitDo Ultimate Wireless Controller,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,misc1:b26,paddle1:b23,paddle2:b19,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,",
-"03000000c82d00001890000001000000,8BitDo Zero 2,a:b0,b:b1,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00001890000001000000,8BitDo Zero 2,a:b1,b:b0,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00003032000000010000,8BitDo Zero 2,a:b0,b:b1,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00003032000000010000,8BitDo Zero 2,a:b1,b:b0,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000a00500003232000008010000,8BitDo Zero Gamepad,a:b0,b:b1,back:b10,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b6,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000a00500003232000008010000,8BitDo Zero Gamepad,a:b1,b:b2,back:b10,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b6,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000a00500003232000009010000,8BitDo Zero Gamepad,a:b0,b:b1,back:b10,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b6,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000a00500003232000009010000,8BitDo Zero Gamepad,a:b1,b:b0,back:b10,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b6,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000050b00000579000000010000,ASUS ROG Kunai 3 Gamepad,a:b0,b:b1,back:b12,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b14,leftshoulder:b6,leftstick:b15,lefttrigger:a5,leftx:a0,lefty:a1,misc1:b42,paddle1:b9,paddle2:b11,rightshoulder:b7,rightstick:b16,righttrigger:a4,rightx:a2,righty:a3,start:b13,x:b3,y:b4,",
 "03000000050b00000679000000010000,ASUS ROG Kunai 3 Gamepad,a:b0,b:b1,back:b12,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b14,leftshoulder:b6,leftstick:b15,lefttrigger:a5,leftx:a0,lefty:a1,misc1:b23,rightshoulder:b7,rightstick:b16,righttrigger:a4,rightx:a2,righty:a3,start:b13,x:b3,y:b4,",
 "03000000491900001904000001010000,Amazon Luna Controller,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,misc1:b9,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b7,x:b2,y:b3,",
 "03000000710100001904000000010000,Amazon Luna Controller,a:b0,b:b1,back:b11,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b10,leftshoulder:b4,leftstick:b7,lefttrigger:a5,leftx:a0,lefty:a1,misc1:b9,rightshoulder:b5,rightstick:b8,righttrigger:a4,rightx:a2,righty:a3,start:b6,x:b2,y:b3,",
 "03000000c62400001a89000000010000,BDA MOGA XP5-X Plus,a:b0,b:b1,back:b12,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b14,leftshoulder:b6,leftstick:b15,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b16,righttrigger:a4,rightx:a2,righty:a3,start:b13,x:b3,y:b4,",
 "03000000c62400001b89000000010000,BDA MOGA XP5-X Plus,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,",
@@ -438,15 +378,14 @@
 "03000000790000004418000000010000,Mayflash GameCube Controller,a:b1,b:b2,dpdown:b14,dpleft:b15,dpright:b13,dpup:b12,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b7,righttrigger:a4,rightx:a5,righty:a2,start:b9,x:b0,y:b3,",
 "0300000025090000e803000000000000,Mayflash Wii Classic Controller,a:b1,b:b0,back:b8,dpdown:b13,dpleft:b12,dpright:b14,dpup:b11,guide:b10,leftshoulder:b4,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b2,",
 "03000000790000000018000000000000,Mayflash WiiU Pro Game Controller Adapter (DInput),a:b4,b:b8,back:b32,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b16,leftstick:b40,lefttrigger:b24,leftx:a0,lefty:a4,rightshoulder:b20,rightstick:b44,righttrigger:b28,rightx:a8,righty:a12,start:b36,x:b0,y:b12,",
 "030000001008000001e5000006010000,NEXT SNES Controller,a:b2,b:b1,back:b8,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b4,rightshoulder:b6,start:b9,x:b3,y:b0,",
 "03000000550900001472000025050000,NVIDIA Controller v01.04,a:b0,b:b1,back:b17,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b15,leftshoulder:b4,leftstick:b7,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b8,righttrigger:a4,rightx:a2,righty:a5,start:b6,x:b2,y:b3,",
 "030000004b120000014d000000010000,NYKO AIRFLO EX,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b10,leftshoulder:b4,leftstick:b11,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b12,righttrigger:b7,rightx:a3,righty:a2,start:b9,x:b2,y:b3,",
 "030000007e0500000920000000000000,Nintendo Switch Pro Controller,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b2,y:b3,",
-"050000007e05000009200000ff070000,Nintendo Switch Pro Controller,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b9,leftshoulder:b4,leftstick:b6,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b7,righttrigger:a5,rightx:a3,righty:a4,start:b10,x:b2,y:b3,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "050000007e05000009200000ff070000,Nintendo Switch Pro Controller,a:b1,b:b0,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b9,leftshoulder:b4,leftstick:b6,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b7,righttrigger:a5,rightx:a3,righty:a4,start:b10,x:b3,y:b2,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "030000006f0e00000901000002010000,PDP Versus Fighting Pad,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,lefttrigger:b6,rightshoulder:b5,righttrigger:b7,start:b9,x:b0,y:b3,",
 "030000004c0500006802000000000000,PS3 Controller,a:b14,b:b13,back:b0,dpdown:b6,dpleft:b7,dpright:b5,dpup:b4,guide:b16,leftshoulder:b10,leftstick:b1,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b11,rightstick:b2,righttrigger:b9,rightx:a2,righty:a3,start:b3,x:b15,y:b12,",
 "030000004c0500006802000000010000,PS3 Controller,a:b14,b:b13,back:b0,dpdown:b6,dpleft:b7,dpright:b5,dpup:b4,guide:b16,leftshoulder:b10,leftstick:b1,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b11,rightstick:b2,righttrigger:b9,rightx:a2,righty:a3,start:b3,x:b15,y:b12,",
 "030000004c050000a00b000000010000,PS4 Controller,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "030000004c050000c405000000000000,PS4 Controller,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "030000004c050000c405000000010000,PS4 Controller,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
@@ -459,15 +398,14 @@
 "03000000321500000104000000010000,Razer Panthera (PS4),a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "03000000321500000010000000010000,Razer RAIJU,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "03000000321500000507000001010000,Razer Raiju Mobile,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b21,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,",
 "03000000321500000011000000010000,Razer Raion Fightpad for PS4,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "03000000321500000009000000020000,Razer Serval,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b9,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b10,righttrigger:a4,rightx:a2,righty:a3,start:b7,x:b2,y:b3,",
 "0300000032150000030a000000000000,Razer Wildcat,a:b0,b:b1,back:b9,dpdown:b12,dpleft:b13,dpright:b14,dpup:b11,guide:b10,leftshoulder:b4,leftstick:b6,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b7,righttrigger:a5,rightx:a3,righty:a4,start:b8,x:b2,y:b3,",
 "03000000790000001100000000000000,Retrolink Classic Controller,a:b2,b:b1,back:b8,leftshoulder:b4,leftx:a3,lefty:a4,rightshoulder:b5,start:b9,x:b3,y:b0,",
-"03000000790000001100000006010000,Retrolink SNES Controller,a:b1,b:b2,back:b8,dpdown:+a4,dpleft:-a3,dpright:+a3,dpup:-a4,leftshoulder:b4,rightshoulder:b5,start:b9,x:b0,y:b3,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000790000001100000006010000,Retrolink SNES Controller,a:b2,b:b1,back:b8,dpdown:+a4,dpleft:-a3,dpright:+a3,dpup:-a4,leftshoulder:b4,rightshoulder:b5,start:b9,x:b3,y:b0,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "030000006b140000130d000000010000,Revolution Pro Controller 3,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "030000006b140000010d000000010000,Revolution Pro Controller,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "030000003512000021ab000000000000,SFC30 Joystick,a:b1,b:b0,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b4,y:b3,",
 "03000000457500002211000000010000,SZMY-POWER PC Gamepad,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "03000000b40400000a01000000000000,Sega Saturn USB Gamepad,a:b0,b:b1,back:b5,guide:b2,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b8,x:b3,y:b4,",
 "03000000811700007e05000000000000,Sega Saturn,a:b2,b:b4,dpdown:b16,dpleft:b15,dpright:b14,dpup:b17,leftshoulder:b8,lefttrigger:a5,leftx:a0,lefty:a2,rightshoulder:b9,righttrigger:a4,start:b13,x:b0,y:b6,",
@@ -501,68 +439,44 @@
 "030000005e040000e002000003090000,Xbox Wireless Controller,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b10,leftshoulder:b4,leftstick:b8,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b9,righttrigger:a5,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "030000005e040000ea02000000000000,Xbox Wireless Controller,a:b0,b:b1,back:b9,dpdown:b12,dpleft:b13,dpright:b14,dpup:b11,guide:b10,leftshoulder:b4,leftstick:b6,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b7,righttrigger:a5,rightx:a3,righty:a4,start:b8,x:b2,y:b3,",
 "030000005e040000fd02000003090000,Xbox Wireless Controller,a:b0,b:b1,back:b16,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b15,leftshoulder:b6,leftstick:b13,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a4,rightx:a2,righty:a3,start:b11,x:b3,y:b4,",
 "03000000172700004431000029010000,XiaoMi Game Controller,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b15,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a6,rightx:a2,righty:a5,start:b11,x:b3,y:b4,",
 "03000000c0160000e105000000040000,Xin-Mo Dual Arcade,crc:82d5,a:b2,b:b4,back:b18,dpdown:+a2,dpleft:-a0,dpright:+a0,dpup:-a2,rightshoulder:b8,righttrigger:b10,start:b16,x:b0,y:b6,",
 "03000000120c0000100e000000010000,ZEROPLUS P4 Gamepad,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "03000000120c0000101e000000010000,ZEROPLUS P4 Wired Gamepad,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
-"03000000830500006020000000010000,iBuffalo SNES Controller,a:b0,b:b1,back:b6,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b4,rightshoulder:b5,start:b7,x:b2,y:b3,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000830500006020000000010000,iBuffalo SNES Controller,a:b1,b:b0,back:b6,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b4,rightshoulder:b5,start:b7,x:b3,y:b2,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000830500006020000000000000,iBuffalo USB 2-axis 8-button Gamepad,a:b1,b:b0,back:b6,leftshoulder:b4,leftx:a0,lefty:a1,rightshoulder:b5,start:b7,x:b3,y:b2,",
 ]
 elif compat_platform.startswith("win"):
     mapping_list = [
 "03000000fa2d00000100000000000000,3DRUDDER,leftx:a0,lefty:a1,rightx:a5,righty:a2,",
-"03000000c82d00000090000000000000,8BitDo FC30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000090000000000000,8BitDo FC30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00001038000000000000,8BitDo FC30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00001038000000000000,8BitDo FC30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00000650000000000000,8BitDo M30 Gamepad,a:b0,b:b1,back:b10,guide:b2,leftshoulder:b6,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,righttrigger:b9,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000650000000000000,8BitDo M30 Gamepad,a:b1,b:b0,back:b10,guide:b2,leftshoulder:b6,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,righttrigger:b9,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00005106000000000000,8BitDo M30 Gamepad,a:b0,b:b1,back:b10,guide:b2,leftshoulder:b6,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,righttrigger:b9,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00005106000000000000,8BitDo M30 Gamepad,a:b1,b:b0,back:b10,guide:b2,leftshoulder:b6,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,righttrigger:b9,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00001590000000000000,8BitDo N30 Pro 2,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00001590000000000000,8BitDo N30 Pro 2,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00006528000000000000,8BitDo N30 Pro 2,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00006528000000000000,8BitDo N30 Pro 2,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"030000003512000012ab000000000000,8BitDo NES30 Gamepad,a:b0,b:b1,back:b10,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b6,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "030000003512000012ab000000000000,8BitDo NES30 Gamepad,a:b1,b:b0,back:b10,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b6,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000022000000090000000000000,8BitDo NES30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000022000000090000000000000,8BitDo NES30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000203800000900000000000000,8BitDo NES30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000203800000900000000000000,8BitDo NES30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00002038000000000000,8BitDo NES30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00002038000000000000,8BitDo NES30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00000660000000000000,8BitDo Pro 2,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000660000000000000,8BitDo Pro 2,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00000060000000000000,8BitDo SF30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000060000000000000,8BitDo SF30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00000061000000000000,8BitDo SF30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000061000000000000,8BitDo SF30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000102800000900000000000000,8BitDo SFC30 Gamepad,a:b0,b:b1,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000102800000900000000000000,8BitDo SFC30 Gamepad,a:b1,b:b0,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00001290000000000000,8BitDo SN30 Gamepad,a:b0,b:b1,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00001290000000000000,8BitDo SN30 Gamepad,a:b1,b:b0,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00006228000000000000,8BitDo SN30 Gamepad,a:b0,b:b1,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00006228000000000000,8BitDo SN30 Gamepad,a:b1,b:b0,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00000260000000000000,8BitDo SN30 Pro+,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000260000000000000,8BitDo SN30 Pro+,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00000261000000000000,8BitDo SN30 Pro+,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000261000000000000,8BitDo SN30 Pro+,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b2,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a2,righty:a3,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00000160000000000000,8BitDo SN30 Pro,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00000160000000000000,8BitDo SN30 Pro,a:b1,b:b0,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"030000003512000020ab000000000000,8BitDo SNES30 Gamepad,a:b0,b:b1,back:b10,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b6,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "030000003512000020ab000000000000,8BitDo SNES30 Gamepad,a:b1,b:b0,back:b10,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b6,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00001130000000000000,8BitDo Ultimate Wired Controller,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,misc1:b26,paddle1:b24,paddle2:b25,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,",
 "03000000c82d00001330000000000000,8BitDo Ultimate Wireless Controller,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,misc1:b26,paddle1:b23,paddle2:b19,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,",
-"03000000c82d00001890000000000000,8BitDo Zero 2,a:b0,b:b1,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00001890000000000000,8BitDo Zero 2,a:b1,b:b0,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000c82d00003032000000000000,8BitDo Zero 2,a:b0,b:b1,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000c82d00003032000000000000,8BitDo Zero 2,a:b1,b:b0,back:b10,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
-"03000000a00500003232000000000000,8BitDo Zero Gamepad,a:b0,b:b1,back:b10,dpdown:+a2,dpleft:-a0,dpright:+a0,dpup:-a2,leftshoulder:b6,rightshoulder:b7,start:b11,x:b3,y:b4,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000a00500003232000000000000,8BitDo Zero Gamepad,a:b1,b:b0,back:b10,dpdown:+a2,dpleft:-a0,dpright:+a0,dpup:-a2,leftshoulder:b6,rightshoulder:b7,start:b11,x:b4,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000050b00000579000000000000,ASUS ROG Kunai 3 Gamepad,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,",
 "03000000050b00000679000000000000,ASUS ROG Kunai 3 Gamepad,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,misc1:b15,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,",
 "030000008f0e00001200000000000000,Acme GA-02,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b5,leftx:a0,lefty:a1,rightshoulder:b6,rightstick:b11,righttrigger:b7,rightx:a3,righty:a2,start:b9,x:b2,y:b3,",
 "03000000fa190000f0ff000000000000,Acteck AGJ-3200,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b0,",
 "03000000341a00003608000000000000,Afterglow PS3 Controller,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "030000006f0e00000263000000000000,Afterglow PS3 Controller,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
@@ -589,24 +503,24 @@
 "030000006b1400000055000000000000,Bigben PS3 Controller,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b2,y:b3,",
 "030000006b1400000103000000000000,Bigben PS3 Controller,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b2,",
 "0300000066f700000500000000000000,BrutalLegendTest,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a3,righty:a2,start:b9,x:b0,y:b3,",
 "03000000e82000006058000000000000,Cideko AK08b,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b0,",
 "03000000260900008888000000000000,Cyber Gadget GameCube Controller,a:b0,b:b1,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,lefttrigger:a5,leftx:a0,lefty:a1,rightshoulder:b6,righttrigger:a4,rightx:a2,righty:a3~,start:b7,x:b2,y:b3,",
 "03000000a306000022f6000000000000,Cyborg V.3 Rumble Pad,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:+a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:-a3,rightx:a2,righty:a4,start:b9,x:b0,y:b3,",
 "03000000451300000830000000000000,Defender Game Racer X7,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b2,y:b3,",
+"03000000790000000600000000000000,Defender Joystick Cobra R4,crc:c77a,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2~,righty:a3~,start:b9,x:b3,y:b0,",
 "03000000791d00000103000000000000,Dual Box WII,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b10,leftshoulder:b6,lefttrigger:b4,leftx:a0,lefty:a1,rightshoulder:b7,righttrigger:b5,rightx:a2,righty:a3,start:b9,x:b3,y:b0,",
 "03000000bd12000002e0000000000000,Dual USB Vibration Joystick,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b9,lefttrigger:b4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b10,righttrigger:b5,rightx:a3,righty:a2,start:b11,x:b3,y:b0,",
 "030000006f0e00003001000000000000,EA SPORTS PS3 Controller,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "03000000341a00000108000000000000,EXEQ RF USB Gamepad 8206,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b8,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b7,rightx:a2,righty:a3,start:b9,x:b2,y:b3,",
 "030000008f0e00000f31000000000000,EXEQ,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b2,",
 "03000000b80500000410000000000000,Elecom Gamepad,a:b2,b:b3,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b1,",
 "03000000b80500000610000000000000,Elecom Gamepad,a:b2,b:b3,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b1,",
 "03000000852100000201000000000000,FF-GP1,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "030000000d0f00002700000000000000,FIGHTING STICK V3,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,lefttrigger:b6,rightshoulder:b5,righttrigger:b7,start:b9,x:b0,y:b3,",
-"03000000790000000600000000000000,G-Shark GS-GP702,crc:8e4f,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b0,",
 "030000008f0e00000d31000000000000,GAMEPAD 3 TURBO,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "03000000300f00000b01000000000000,GGE909 Recoil Pad,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a3,righty:a2,start:b9,x:b3,y:b0,",
 "03000000790000002201000000000000,Game Controller for PC,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b0,",
 "0300000066f700000100000000000000,Game VIB Joystick,a:b2,b:b3,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b8,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b9,righttrigger:b7,rightx:a3,righty:a2,start:b11,x:b0,y:b1,",
 "03000000491900000204000000000000,GameSir T4 Pro,crc:1aa4,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,",
 "03000000ac0500003d03000000000000,GameSir,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,",
 "03000000ac0500004d04000000000000,GameSir,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,",
@@ -688,18 +602,16 @@
 "03000000790000000018000000000000,Mayflash WiiU Pro Game Controller Adapter (DInput),a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "03000000efbe0000edfe000000000000,Monect Virtual Controller,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a5,rightx:a3,righty:a4,start:b9,x:b3,y:b0,",
 "030000006b140000010c000000000000,NACON GC-400ES,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b2,y:b3,",
 "030000001008000001e5000000000000,NEXT SNES Controller,a:b2,b:b1,back:b8,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b4,rightshoulder:b6,start:b9,x:b3,y:b0,",
 "03000000152000000182000000000000,NGDS,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a3,righty:a4,start:b9,x:b3,y:b0,",
 "030000005509000000b4000000000000,NVIDIA Virtual Gamepad,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b8,lefttrigger:+a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b9,righttrigger:-a2,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "030000004b120000014d000000000000,NYKO AIRFLO EX,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b10,leftshoulder:b4,leftstick:b11,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b12,righttrigger:b7,rightx:a3,righty:a2,start:b9,x:b2,y:b3,",
-"03000000790000004318000000000000,Nintendo GameCube Controller,a:b1,b:b2,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b7,righttrigger:a4,rightx:a5,righty:a2,start:b9,x:b0,y:b3,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000790000004318000000000000,Nintendo GameCube Controller,a:b1,b:b0,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b7,righttrigger:a4,rightx:a5,righty:a2,start:b9,x:b2,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000bd12000015d0000000000000,Nintendo Retrolink USB Super SNES Classic Controller,a:b2,b:b1,back:b8,leftshoulder:b4,leftx:a0,lefty:a1,rightshoulder:b5,start:b9,x:b3,y:b0,",
-"030000007e0500000920000000000000,Nintendo Switch Pro Controller,a:b1,b:b0,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b2,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "030000007e0500000920000000000000,Nintendo Switch Pro Controller,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b2,y:b3,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "030000000d0500000308000000000000,Nostromo N45,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b9,leftshoulder:b4,leftstick:b12,lefttrigger:b5,leftx:a0,lefty:a1,rightshoulder:b6,rightstick:b11,righttrigger:b7,rightx:a3,righty:a2,start:b10,x:b2,y:b3,",
 "03000000d62000006d57000000000000,OPP PS3 Controller,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "03000000362800000100000000000000,OUYA Game Controller,a:b0,b:b3,dpdown:b9,dpleft:b10,dpright:b11,dpup:b8,guide:b14,leftshoulder:b4,leftstick:b6,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b7,righttrigger:b13,rightx:a3,righty:a4,x:b1,y:b2,",
 "03000000782300000a10000000000000,Onlive Wireless Controller,a:b15,b:b14,back:b7,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b5,leftshoulder:b11,leftstick:b9,lefttrigger:a2,leftx:a0,lefty:a1,rightshoulder:b10,rightstick:b8,righttrigger:a5,rightx:a3,righty:a4,start:b6,x:b13,y:b12,",
 "030000006b14000001a1000000000000,Orange Controller,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b10,leftshoulder:b4,leftstick:b6,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b7,righttrigger:a4,rightx:a5,righty:a2,start:b9,x:b2,y:b3,",
 "03000000120c0000f60e000000000000,P4 Wired Gamepad,a:b1,b:b2,back:b12,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b5,lefttrigger:b7,rightshoulder:b4,righttrigger:b6,start:b9,x:b0,y:b3,",
@@ -742,14 +654,15 @@
 "030000000d0f00002200000000000000,REAL ARCADE Pro.V3,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "03000000050b00005819000000000000,ROG Chakram Core,a:b1,b:b0,leftx:a0,lefty:a1,x:b2,y:b3,",
 "03000000050b0000181a000000000000,ROG Chakram X,a:b1,b:b0,leftx:a0,lefty:a1,x:b2,y:b3,",
 "03000000050b00001a1a000000000000,ROG Chakram X,a:b1,b:b0,leftx:a0,lefty:a1,x:b2,y:b3,",
 "03000000050b00001c1a000000000000,ROG Chakram X,a:b1,b:b0,leftx:a0,lefty:a1,x:b2,y:b3,",
 "03000000050b0000e318000000000000,ROG Chakram,a:b1,b:b0,leftx:a0,lefty:a1,x:b2,y:b3,",
 "03000000050b0000e518000000000000,ROG Chakram,a:b1,b:b0,leftx:a0,lefty:a1,x:b2,y:b3,",
+"030000000d0f0000ad00000000000000,RX Gamepad,a:b0,b:b4,back:b11,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b3,rightshoulder:b6,start:b9,x:b2,y:b1,",
 "03000000321500000003000000000000,Razer Hydra,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b8,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b9,righttrigger:a2,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "03000000321500000204000000000000,Razer Panthera (PS3),a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "03000000321500000104000000000000,Razer Panthera (PS4),a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "03000000321500000507000000000000,Razer Raiju Mobile,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,",
 "03000000321500000707000000000000,Razer Raiju Mobile,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,",
 "03000000321500000011000000000000,Razer Raion Fightpad for PS4,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "03000000321500000009000000000000,Razer Serval,+lefty:+a2,-lefty:-a1,a:b0,b:b1,back:b12,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b10,leftshoulder:b4,leftstick:b8,leftx:a0,rightshoulder:b5,rightstick:b9,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
@@ -757,15 +670,14 @@
 "030000000d0f00006b00000000000000,Real Arcade Pro.4,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "030000000d0f00008a00000000000000,Real Arcade Pro.4,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "030000000d0f00008b00000000000000,Real Arcade Pro.4,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "030000000d0f00005b00000000000000,Real Arcade Pro.V4,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "030000000d0f00005c00000000000000,Real Arcade Pro.V4,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "0300000000f000000300000000000000,RetroUSB.com RetroPad,a:b1,b:b5,back:b2,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b3,x:b0,y:b4,",
 "0300000000f00000f100000000000000,RetroUSB.com Super RetroPort,a:b1,b:b5,back:b2,leftshoulder:b6,leftx:a0,lefty:a1,rightshoulder:b7,start:b3,x:b0,y:b4,",
-"03000000790000001100000000000000,Retrolink SNES Controller,a:b1,b:b2,back:b8,dpdown:+a4,dpleft:-a3,dpright:+a3,dpup:-a4,leftshoulder:b4,rightshoulder:b5,start:b9,x:b0,y:b3,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000790000001100000000000000,Retrolink SNES Controller,a:b2,b:b1,back:b8,dpdown:+a4,dpleft:-a3,dpright:+a3,dpup:-a4,leftshoulder:b4,rightshoulder:b5,start:b9,x:b3,y:b0,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "030000006b140000130d000000000000,Revolution Pro Controller 3,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "030000006b140000010d000000000000,Revolution Pro Controller,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "030000006f0e00001e01000000000000,Rock Candy PS3 Controller,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "030000006f0e00002801000000000000,Rock Candy PS3 Controller,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "030000006f0e00002f01000000000000,Rock Candy PS3 Controller,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b0,y:b3,",
 "03000000341a00000208000000000000,SL-6555-SBK,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b8,lefttrigger:-a4,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b9,righttrigger:a4,rightx:a3,righty:a2,start:b7,x:b2,y:b3,",
@@ -780,14 +692,15 @@
 "03000000a30600000c04000000000000,Saitek P2900,a:b1,b:b2,back:b12,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a3,righty:a2,start:b9,x:b0,y:b3,",
 "03000000300f00001001000000000000,Saitek P480 Rumble Pad,a:b2,b:b3,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b5,leftx:a0,lefty:a1,rightshoulder:b6,rightstick:b11,righttrigger:b7,rightx:a3,righty:a2,start:b9,x:b0,y:b1,",
 "03000000a30600000b04000000010000,Saitek P990 Dual Analog Pad,a:b1,b:b2,back:b9,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a3,righty:a2,start:b8,x:b0,y:b3,",
 "03000000a30600000b04000000000000,Saitek P990,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a3,righty:a2,start:b9,x:b0,y:b3,",
 "03000000a30600002106000000000000,Saitek PS1000,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a4,start:b9,x:b0,y:b3,",
 "03000000a306000020f6000000000000,Saitek PS2700,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a4,start:b9,x:b0,y:b3,",
 "03000000300f00001101000000000000,Saitek Rumble Pad,a:b2,b:b3,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b8,leftshoulder:b4,leftstick:b10,lefttrigger:b5,leftx:a0,lefty:a1,rightshoulder:b6,rightstick:b11,righttrigger:b7,rightx:a3,righty:a2,start:b9,x:b0,y:b1,",
+"03000000790000000600000000000000,Sanwa Supply JY-P76USV,crc:20f0,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a4,start:b9,x:b2,y:b3,",
 "0300000000050000289b000000000000,Saturn_Adapter_2.0,a:b1,b:b2,leftshoulder:b6,lefttrigger:b4,leftx:a0,lefty:a1,rightshoulder:b7,righttrigger:b5,start:b9,x:b0,y:b3,",
 "030000009b2800000500000000000000,Saturn_Adapter_2.0,a:b1,b:b2,leftshoulder:b6,lefttrigger:b4,leftx:a0,lefty:a1,rightshoulder:b7,righttrigger:b5,start:b9,x:b0,y:b3,",
 "030000008f0e00000800000000000000,SpeedLink Strike FX,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b0,",
 "03000000c01100000591000000000000,Speedlink Torid,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b0,",
 "03000000de280000ff11000000000000,Steam Virtual Gamepad,a:b0,b:b1,back:b6,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b8,lefttrigger:+a2,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b9,righttrigger:-a2,rightx:a3,righty:a4,start:b7,x:b2,y:b3,",
 "03000000110100003114000000000000,SteelSeries Stratus Duo,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,",
 "03000000381000001814000000000000,SteelSeries Stratus XL,a:b0,b:b1,back:b18,dpdown:b13,dpleft:b14,dpright:b15,dpup:b12,guide:b19,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b2,y:b3,",
@@ -820,14 +733,13 @@
 "03000000341a00000608000000000000,Xeox,a:b0,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b2,y:b3,",
 "03000000172700004431000000000000,XiaoMi Game Controller,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b20,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:a7,rightx:a2,righty:a5,start:b11,x:b3,y:b4,",
 "03000000c0160000e105000000000000,Xin-Mo Dual Arcade,crc:2246,a:b1,b:b2,back:b9,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,rightshoulder:b4,righttrigger:b5,start:b8,x:b0,y:b3,",
 "03000000790000004f18000000000000,ZD-T Android,a:b0,b:b1,back:b10,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b6,leftstick:b13,lefttrigger:b8,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b14,righttrigger:b9,rightx:a3,righty:a4,start:b11,x:b3,y:b4,",
 "03000000120c0000101e000000000000,ZEROPLUS P4 Wired Gamepad,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b12,leftshoulder:b4,leftstick:b10,lefttrigger:a3,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:a4,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "03000000d81d00000f00000000000000,iBUFFALO BSGP1204 Series,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b10,lefttrigger:b4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b11,righttrigger:b5,rightx:a2,righty:a3,start:b9,x:b3,y:b0,",
 "03000000d81d00001000000000000000,iBUFFALO BSGP1204P Series,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b6,leftstick:b10,lefttrigger:b4,leftx:a0,lefty:a1,rightshoulder:b7,rightstick:b11,righttrigger:b5,rightx:a2,righty:a3,start:b9,x:b3,y:b0,",
-"03000000830500006020000000000000,iBuffalo SNES Controller,a:b0,b:b1,back:b6,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b4,rightshoulder:b5,start:b7,x:b2,y:b3,hint:SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "03000000830500006020000000000000,iBuffalo SNES Controller,a:b1,b:b0,back:b6,dpdown:+a1,dpleft:-a0,dpright:+a0,dpup:-a1,leftshoulder:b4,rightshoulder:b5,start:b7,x:b3,y:b2,hint:!SDL_GAMECONTROLLER_USE_BUTTON_LABELS:=1,",
 "030000004f04000003d0000000000000,run'n'drive,a:b1,b:b2,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,guide:b7,leftshoulder:a3,leftstick:b10,lefttrigger:b4,leftx:a0,lefty:a1,rightshoulder:a4,rightstick:b11,righttrigger:b5,rightx:a2,righty:a5,start:b9,x:b0,y:b3,",
 "03000000101c0000171c000000000000,uRage Gamepad,a:b2,b:b1,back:b8,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,dpup:h0.1,leftshoulder:b4,leftstick:b10,lefttrigger:b6,leftx:a0,lefty:a1,rightshoulder:b5,rightstick:b11,righttrigger:b7,rightx:a2,righty:a3,start:b9,x:b3,y:b0,",
 ]
 else:
     mapping_list = []
```

### Comparing `pyglet-2.1.dev1/pyglet/input/linux/evdev.py` & `pyglet-2.1.dev2/pyglet/input/linux/evdev.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/input/linux/evdev_constants.py` & `pyglet-2.1.dev2/pyglet/input/linux/evdev_constants.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/input/linux/x11_xinput.py` & `pyglet-2.1.dev2/pyglet/input/linux/x11_xinput.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/input/linux/x11_xinput_tablet.py` & `pyglet-2.1.dev2/pyglet/input/linux/x11_xinput_tablet.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/input/macos/darwin_hid.py` & `pyglet-2.1.dev2/pyglet/input/macos/darwin_hid.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/input/win32/__init__.py` & `pyglet-2.1.dev2/pyglet/input/win32/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/input/win32/directinput.py` & `pyglet-2.1.dev2/pyglet/input/win32/directinput.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/input/win32/wintab.py` & `pyglet-2.1.dev2/pyglet/input/win32/wintab.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/input/win32/xinput.py` & `pyglet-2.1.dev2/pyglet/input/win32/xinput.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/lib.py` & `pyglet-2.1.dev2/pyglet/lib.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/darwin/cocoapy/__init__.py` & `pyglet-2.1.dev2/pyglet/libs/darwin/cocoapy/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/darwin/cocoapy/cocoalibs.py` & `pyglet-2.1.dev2/pyglet/libs/darwin/cocoapy/cocoalibs.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/darwin/cocoapy/cocoatypes.py` & `pyglet-2.1.dev2/pyglet/libs/darwin/cocoapy/cocoatypes.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/darwin/cocoapy/runtime.py` & `pyglet-2.1.dev2/pyglet/libs/darwin/cocoapy/runtime.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/darwin/coreaudio.py` & `pyglet-2.1.dev2/pyglet/libs/darwin/coreaudio.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/darwin/quartzkey.py` & `pyglet-2.1.dev2/pyglet/libs/darwin/quartzkey.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/egl/egl.py` & `pyglet-2.1.dev2/pyglet/libs/egl/egl.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/egl/eglext.py` & `pyglet-2.1.dev2/pyglet/libs/egl/eglext.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/egl/lib.py` & `pyglet-2.1.dev2/pyglet/libs/egl/lib.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/wayland/gbm.py` & `pyglet-2.1.dev2/pyglet/libs/wayland/gbm.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/wayland/xkbcommon.py` & `pyglet-2.1.dev2/pyglet/libs/wayland/xkbcommon.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/win32/__init__.py` & `pyglet-2.1.dev2/pyglet/libs/win32/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/win32/com.py` & `pyglet-2.1.dev2/pyglet/libs/win32/com.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/win32/constants.py` & `pyglet-2.1.dev2/pyglet/libs/win32/constants.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/win32/context_managers.py` & `pyglet-2.1.dev2/pyglet/libs/win32/context_managers.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/win32/dinput.py` & `pyglet-2.1.dev2/pyglet/libs/win32/dinput.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/win32/libwintab.py` & `pyglet-2.1.dev2/pyglet/libs/win32/libwintab.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/win32/types.py` & `pyglet-2.1.dev2/pyglet/libs/win32/types.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/win32/winkey.py` & `pyglet-2.1.dev2/pyglet/libs/win32/winkey.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/x11/cursorfont.py` & `pyglet-2.1.dev2/pyglet/libs/x11/cursorfont.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/x11/xf86vmode.py` & `pyglet-2.1.dev2/pyglet/libs/x11/xf86vmode.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/x11/xinerama.py` & `pyglet-2.1.dev2/pyglet/libs/x11/xinerama.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/x11/xinput.py` & `pyglet-2.1.dev2/pyglet/libs/x11/xinput.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/x11/xlib.py` & `pyglet-2.1.dev2/pyglet/libs/x11/xlib.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/libs/x11/xsync.py` & `pyglet-2.1.dev2/pyglet/libs/x11/xsync.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/math.py` & `pyglet-2.1.dev2/pyglet/math.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 
 Mat3T = _typing.TypeVar("Mat3T", bound="Mat3")
 Mat4T = _typing.TypeVar("Mat4T", bound="Mat4")
 
 
 def clamp(num: float, min_val: float, max_val: float) -> float:
+    """Clamp a value between a minimum and maximum limit."""
     return max(min(num, max_val), min_val)
 
 
 class Vec2(_typing.NamedTuple):
     """A two-dimensional vector represented as an X Y coordinate pair.
 
     `Vec2` is an immutable 2D Vector, including most common
@@ -96,81 +97,86 @@
     def __ne__(self, other: object) -> bool:
         return not isinstance(other, Vec2) or self.x != other.x or self.y != other.y
 
     @staticmethod
     def from_polar(mag: float, angle: float) -> Vec2:
         """Create a new vector from the given polar coordinates.
 
-        :parameters:
-            `mag`   : int or float :
-                The magnitude of the vector.
-            `angle` : int or float :
-                The angle of the vector in radians.
+        Args:
+          mag: The desired magnitude.
+          angle: The angle, in radians.
         """
         return Vec2(mag * _math.cos(angle), mag * _math.sin(angle))
 
     def from_magnitude(self, magnitude: float) -> Vec2:
-        """Create a new Vector of the given magnitude by normalizing,
-        then scaling the vector. The heading remains unchanged.
+        """Create a new vector of the given magnitude
 
-        :parameters:
-            `magnitude` : int or float :
-                The magnitude of the new vector.
+        The new vector will be created by first normalizing,
+        then scaling the vector. The heading remains unchanged.
         """
         return self.normalize() * magnitude
 
     def from_heading(self, heading: float) -> Vec2:
-        """Create a new vector of the same magnitude with the given heading. I.e. Rotate the vector to the heading.
+        """Create a new vector of the same magnitude with the given heading.
+
+         In effect, the vector rotated to the new heading.
+
+        Args:
+          heading: The desired heading, in radians.
 
-        :parameters:
-            `heading` : int or float :
-                The angle of the new vector in radians.
         """
         mag = self.__abs__()
         return Vec2(mag * _math.cos(heading), mag * _math.sin(heading))
 
     @property
     def heading(self) -> float:
         """The angle of the vector in radians."""
         return _math.atan2(self.y, self.x)
 
     @property
     def mag(self) -> float:
-        """The magnitude, or length of the vector. The distance between the coordinates and the origin.
+        """The magnitude, or length of the vector.
 
-        Alias of abs(self).
+        The distance between the coordinates and the origin.
+        Alias of abs(vec2_instance).
         """
         return self.__abs__()
 
     def limit(self, maximum: float) -> Vec2:
         """Limit the magnitude of the vector to passed maximum value."""
         if self.x ** 2 + self.y ** 2 > maximum * maximum:
             return self.from_magnitude(maximum)
         return self
 
     def lerp(self, other: Vec2, alpha: float) -> Vec2:
         """Create a new Vec2 linearly interpolated between this vector and another Vec2.
 
-        :parameters:
-            `other`  : Vec2 :
-                The vector to linearly interpolate with.
-            `alpha` : float or int :
-                The amount of interpolation.
-                Some value between 0.0 (this vector) and 1.0 (other vector).
-                0.5 is halfway inbetween.
+        Args:
+          other: Another Vec2 instance.
+          alpha: The amount of interpolation between this vector, and the other
+                 vector. This should be a value between 0.0 and 1.0. For example:
+                 0.5 is the midway point between both vectors.
         """
         return Vec2(self.x + (alpha * (other.x - self.x)),
                     self.y + (alpha * (other.y - self.y)))
 
-    def reflect(self, normal: Vec2) -> Vec2:
-        """Create a new Vec2 reflected (ricochet) from the given normal."""
-        return self - normal * 2 * normal.dot(self)
+    def reflect(self, vector: Vec2) -> Vec2:
+        """Create a new Vec2 reflected (ricochet) from the given normalized vector.
+
+        Args:
+          vector: A normalized vector.
+        """
+        return self - vector * 2 * vector.dot(self)
 
     def rotate(self, angle: float) -> Vec2:
-        """Create a new Vector rotated by the angle. The magnitude remains unchanged."""
+        """Create a new vector rotated by the angle. The magnitude remains unchanged.
+
+        Args:
+          angle: The desired angle, in radians.
+        """
         s = _math.sin(angle)
         c = _math.cos(angle)
         return Vec2(c * self.x - s * self.y, s * self.x + c * self.y)
 
     def distance(self, other: Vec2) -> float:
         """Calculate the distance between this vector and another 2D vector."""
         return _math.sqrt(((other.x - self.x) ** 2) + ((other.y - self.y) ** 2))
@@ -215,19 +221,18 @@
     """
     x: float = 0.0
     y: float = 0.0
     z: float = 0.0
 
     @property
     def mag(self) -> float:
-        """The magnitude, or length of the vector. The distance between the coordinates and the origin.
-
-        Alias of abs(self).
+        """The magnitude, or length of the vector.
 
-        :type: float
+        The distance between the coordinates and the origin.
+        Alias of abs(vector_instance).
         """
         return self.__abs__()
 
     def __add__(self, other: Vec3) -> Vec3:
         return Vec3(self.x + other.x, self.y + other.y, self.z + other.z)
 
     def __sub__(self, other: Vec3) -> Vec3:
@@ -270,21 +275,23 @@
     def __eq__(self, other: object) -> bool:
         return isinstance(other, Vec3) and self.x == other.x and self.y == other.y and self.z == other.z
 
     def __ne__(self, other: object) -> bool:
         return not isinstance(other, Vec3) or self.x != other.x or self.y != other.y or self.z != other.z
 
     def from_magnitude(self, magnitude: float) -> Vec3:
-        """Create a new Vector of the given magnitude by normalizing,
-        then scaling the vector. The rotation remains unchanged.
+        """Create a new vector of the given magnitude
+
+        The new vector will be created by first normalizing,
+        then scaling the vector. The heading remains unchanged.
         """
         return self.normalize() * magnitude
 
     def limit(self, maximum: float) -> Vec3:
-        """Limit the magnitude of the vector to the passed maximum value."""
+        """Limit the magnitude of the vector to passed maximum value."""
         if self.x ** 2 + self.y ** 2 + self.z ** 2 > maximum * maximum * maximum:
             return self.from_magnitude(maximum)
         return self
 
     def cross(self, other: Vec3) -> Vec3:
         """Calculate the cross product of this vector and another 3D vector."""
         return Vec3((self.y * other.z) - (self.z * other.y),
@@ -294,17 +301,19 @@
     def dot(self, other: Vec3) -> float:
         """Calculate the dot product of this vector and another 3D vector."""
         return self.x * other.x + self.y * other.y + self.z * other.z
 
     def lerp(self, other: Vec3, alpha: float) -> Vec3:
         """Create a new Vec3 linearly interpolated between this vector and another Vec3.
 
-        The `alpha` parameter dictates the amount of interpolation.
-        This should be a value between 0.0 (this vector) and 1.0 (other vector).
-        For example; 0.5 is the midway point between both vectors.
+        Args:
+          other: Another Vec3 instance.
+          alpha: The amount of interpolation between this vector, and the other
+                 vector. This should be a value between 0.0 and 1.0. For example:
+                 0.5 is the midway point between both vectors.
         """
         return Vec3(self.x + (alpha * (other.x - self.x)),
                     self.y + (alpha * (other.y - self.y)),
                     self.z + (alpha * (other.z - self.z)))
 
     def distance(self, other: Vec3) -> float:
         """Get the distance between this vector and another 3D vector."""
@@ -410,19 +419,21 @@
                 or self.x != other.x
                 or self.y != other.y
                 or self.z != other.z
                 or self.w != other.w
         )
 
     def lerp(self, other: Vec4, alpha: float) -> Vec4:
-        """Create a new Vec4 linearly interpolated between this one and another Vec4.
+        """Create a new Vec4 linearly interpolated between this vector and another Vec4.
 
-        The `alpha` parameter dictates the amount of interpolation.
-        This should be a value between 0.0 (this vector) and 1.0 (other vector).
-        For example; 0.5 is the midway point between both vectors.
+        Args:
+          other: Another Vec4 instance.
+          alpha: The amount of interpolation between this vector, and the other
+                 vector. This should be a value between 0.0 and 1.0. For example:
+                 0.5 is the midway point between both vectors.
         """
         return Vec4(self.x + (alpha * (other.x - self.x)),
                     self.y + (alpha * (other.y - self.y)),
                     self.z + (alpha * (other.z - self.z)),
                     self.w + (alpha * (other.w - self.w)))
 
     def distance(self, other: Vec4) -> float:
@@ -624,15 +635,20 @@
         return cls((w, 0, 0, 0,
                     0, h, 0, 0,
                     0, 0, q, -1,
                     0, 0, qn, 0))
 
     @classmethod
     def from_rotation(cls, angle: float, vector: Vec3) -> Mat4:
-        """Create a rotation matrix from an angle and Vec3."""
+        """Create a rotation matrix from an angle and Vec3.
+
+        Args:
+          angle: The desired angle, in radians.
+          vector: A Vec3 indicating the direction.
+        """
         return cls().rotate(angle, vector)
 
     @classmethod
     def from_scale(cls: type[Mat4T], vector: Vec3) -> Mat4T:
         """Create a scale matrix from a Vec3."""
         return cls((vector[0], 0.0, 0.0, 0.0,
                     0.0, vector[1], 0.0, 0.0,
@@ -645,14 +661,26 @@
         return cls((1.0, 0.0, 0.0, 0.0,
                     0.0, 1.0, 0.0, 0.0,
                     0.0, 0.0, 1.0, 0.0,
                     vector[0], vector[1], vector[2], 1.0))
 
     @classmethod
     def look_at(cls: type[Mat4T], position: Vec3, target: Vec3, up: Vec3):
+        """Create a viewing matrix that points toward a target.
+
+        This method takes three Vec3s, describing the viewer's position,
+        where they are looking, and the upward axis (typically positive
+        on the Y axis). The resulting Mat4 can be used as the projection
+        matrix.
+
+        Args:
+          position: The location of the viewer in the scene.
+          target: The point that the viewer is looking towards.
+          up: A vector pointing "up" in the scene, typically `Vec3(0.0, 1.0, 0.0)`.
+        """
         f = (target - position).normalize()
         u = up.normalize()
         s = f.cross(u).normalize()
         u = s.cross(f)
 
         return cls([s.x, u.x, -f.x, 0.0,
                     s.y, u.y, -f.y, 0.0,
@@ -888,14 +916,19 @@
         # i, j, k, -
         # -, -, -, -
 
         return Mat3((a, b, c, e, f, g, i, j, k))
 
     @property
     def mag(self) -> float:
+        """The magnitude, or length, of the Quaternion.
+
+        The distance between the coordinates and the origin.
+        Alias of abs(quaternion_instance).
+        """
         return self.__abs__()
 
     def conjugate(self) -> Quaternion:
         return Quaternion(self.w, -self.x, -self.y, -self.z)
 
     def dot(self, other: Quaternion) -> float:
         a, b, c, d = self
```

### Comparing `pyglet-2.1.dev1/pyglet/media/__init__.py` & `pyglet-2.1.dev2/pyglet/media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/buffered_logger.py` & `pyglet-2.1.dev2/pyglet/media/buffered_logger.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/codecs/__init__.py` & `pyglet-2.1.dev2/pyglet/media/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/codecs/base.py` & `pyglet-2.1.dev2/pyglet/media/codecs/base.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/codecs/coreaudio.py` & `pyglet-2.1.dev2/pyglet/media/codecs/coreaudio.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/codecs/ffmpeg.py` & `pyglet-2.1.dev2/pyglet/media/codecs/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/codecs/ffmpeg_lib/compat.py` & `pyglet-2.1.dev2/pyglet/media/codecs/ffmpeg_lib/compat.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/codecs/ffmpeg_lib/libavcodec.py` & `pyglet-2.1.dev2/pyglet/media/codecs/ffmpeg_lib/libavcodec.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/codecs/ffmpeg_lib/libavformat.py` & `pyglet-2.1.dev2/pyglet/media/codecs/ffmpeg_lib/libavformat.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/codecs/ffmpeg_lib/libavutil.py` & `pyglet-2.1.dev2/pyglet/media/codecs/ffmpeg_lib/libavutil.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/codecs/ffmpeg_lib/libswresample.py` & `pyglet-2.1.dev2/pyglet/media/codecs/ffmpeg_lib/libswresample.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/codecs/ffmpeg_lib/libswscale.py` & `pyglet-2.1.dev2/pyglet/media/codecs/ffmpeg_lib/libswscale.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/codecs/gstreamer.py` & `pyglet-2.1.dev2/pyglet/media/codecs/gstreamer.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/codecs/pyogg.py` & `pyglet-2.1.dev2/pyglet/media/codecs/pyogg.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/codecs/wave.py` & `pyglet-2.1.dev2/pyglet/media/codecs/wave.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/codecs/wmf.py` & `pyglet-2.1.dev2/pyglet/media/codecs/wmf.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/devices/__init__.py` & `pyglet-2.1.dev2/pyglet/media/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/devices/base.py` & `pyglet-2.1.dev2/pyglet/media/devices/base.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/devices/win32.py` & `pyglet-2.1.dev2/pyglet/media/devices/win32.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/drivers/__init__.py` & `pyglet-2.1.dev2/pyglet/media/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/drivers/base.py` & `pyglet-2.1.dev2/pyglet/media/drivers/base.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/drivers/directsound/adaptation.py` & `pyglet-2.1.dev2/pyglet/media/drivers/directsound/adaptation.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/drivers/directsound/interface.py` & `pyglet-2.1.dev2/pyglet/media/drivers/directsound/interface.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/drivers/directsound/lib_dsound.py` & `pyglet-2.1.dev2/pyglet/media/drivers/directsound/lib_dsound.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/drivers/listener.py` & `pyglet-2.1.dev2/pyglet/media/drivers/listener.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/drivers/openal/adaptation.py` & `pyglet-2.1.dev2/pyglet/media/drivers/openal/adaptation.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/drivers/openal/interface.py` & `pyglet-2.1.dev2/pyglet/media/drivers/openal/interface.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/drivers/openal/lib_alc.py` & `pyglet-2.1.dev2/pyglet/media/drivers/openal/lib_alc.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/drivers/openal/lib_openal.py` & `pyglet-2.1.dev2/pyglet/media/drivers/openal/lib_openal.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/drivers/pulse/adaptation.py` & `pyglet-2.1.dev2/pyglet/media/drivers/pulse/adaptation.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/drivers/pulse/interface.py` & `pyglet-2.1.dev2/pyglet/media/drivers/pulse/interface.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/drivers/pulse/lib_pulseaudio.py` & `pyglet-2.1.dev2/pyglet/media/drivers/pulse/lib_pulseaudio.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/drivers/silent/adaptation.py` & `pyglet-2.1.dev2/pyglet/media/drivers/silent/adaptation.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/drivers/xaudio2/adaptation.py` & `pyglet-2.1.dev2/pyglet/media/drivers/xaudio2/adaptation.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/drivers/xaudio2/interface.py` & `pyglet-2.1.dev2/pyglet/media/drivers/xaudio2/interface.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/drivers/xaudio2/lib_xaudio2.py` & `pyglet-2.1.dev2/pyglet/media/drivers/xaudio2/lib_xaudio2.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/instrumentation.py` & `pyglet-2.1.dev2/pyglet/media/instrumentation.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/player.py` & `pyglet-2.1.dev2/pyglet/media/player.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/player_worker_thread.py` & `pyglet-2.1.dev2/pyglet/media/player_worker_thread.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/media/synthesis.py` & `pyglet-2.1.dev2/pyglet/media/synthesis.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/model/__init__.py` & `pyglet-2.1.dev2/pyglet/model/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -44,21 +44,23 @@
 
     pyglet.app.run()
 
 
 .. versionadded:: 1.4
 """
 
+from __future__ import annotations
+
+from typing import Tuple
+
 import pyglet
 
 from pyglet import gl
 from pyglet import graphics
-from pyglet.gl import current_context
-from pyglet.math import Mat4, Vec3
-from pyglet.graphics import shader
+from pyglet.math import Mat4
 
 from .codecs import registry as _codec_registry
 from .codecs import add_default_codecs as _add_default_codecs
 
 
 def load(filename, file=None, decoder=None, batch=None, group=None):
     """Load a 3D model from a file.
@@ -86,14 +88,15 @@
         return _codec_registry.decode(filename, file, batch=batch, group=group)
 
 
 def get_default_shader():
     return pyglet.gl.current_context.create_program((MaterialGroup.default_vert_src, 'vertex'),
                                                     (MaterialGroup.default_frag_src, 'fragment'))
 
+
 def get_default_textured_shader():
     return pyglet.gl.current_context.create_program((TexturedMaterialGroup.default_vert_src, 'vertex'),
                                                     (TexturedMaterialGroup.default_frag_src, 'fragment'))
 
 
 class Model:
     """Instance of a 3D object.
@@ -166,32 +169,40 @@
         gl.current_context.window_block.bind(0)
         self._batch.draw_subset(self.vertex_lists)
 
 
 class Material:
     __slots__ = ("name", "diffuse", "ambient", "specular", "emission", "shininess", "texture_name")
 
-    def __init__(self, name, diffuse, ambient, specular, emission, shininess, texture_name=None):
+    def __init__(self, name: str = "default",
+                 diffuse: Tuple[float, float, float, float] = (0.8, 0.8, 0.8, 1.0),
+                 ambient: Tuple[float, float, float, float] = (0.2, 0.2, 0.2, 1.0),
+                 specular: Tuple[float, float, float, float] = (0.0, 0.0, 0.0, 1.0),
+                 emission: Tuple[float, float, float, float] = (0.0, 0.0, 0.0, 1.0),
+                 shininess: float = 20,
+                 texture_name: str = ""):
+
         self.name = name
         self.diffuse = diffuse
         self.ambient = ambient
         self.specular = specular
         self.emission = emission
         self.shininess = shininess
         self.texture_name = texture_name
 
-    def __eq__(self, other):
-        return (self.name == other.name and
-                self.diffuse == other.diffuse and
-                self.ambient == other.ambient and
-                self.specular == other.specular and
-                self.emission == other.emission and
-                self.shininess == other.shininess and
+    def __eq__(self, other: Material) -> bool:
+        return (self.name == other.name and self.diffuse == other.diffuse and
+                self.ambient == other.ambient and self.specular == other.specular and
+                self.emission == other.emission and self.shininess == other.shininess and
                 self.texture_name == other.texture_name)
 
+    def __hash__(self) -> int:
+        return hash((self.name, self.texture_name, tuple(self.diffuse), tuple(self.specular),
+                     tuple(self.ambient), tuple(self.emission), self.shininess, self.texture_name))
+
 
 class BaseMaterialGroup(graphics.Group):
     default_vert_src = None
     default_frag_src = None
     matrix = Mat4()
 
     def __init__(self, material, program, order=0, parent=None):
@@ -313,9 +324,80 @@
     }
     """
 
     def set_state(self):
         self.program.use()
         self.program['model'] = self.matrix
 
+    def __hash__(self):
+        return hash((self.material, self.program, self.order, self.parent))
+
+    def __eq__(self, other):
+        return (self.__class__ is other.__class__ and
+                self.material == other.material and
+                self.program == other.program and
+                self.order == other.order and
+                self.parent == other.parent)
+
+
+class Cube(Model):
+
+    def __init__(self, width=1.0, height=1.0, depth=1.0, color=(1.0, 1.0, 1.0, 1.0), material=None,
+                 batch=None, group=None, program=None):
+        self._width = width
+        self._height = height
+        self._depth = depth
+        self._color = color
+        self._scale = 1.0
+
+        self._batch = batch
+        self._program = program if program else get_default_shader()
+
+        # Create a Material and Group for the Model
+        self._material = material if material else pyglet.model.Material(name="cube")
+        self._group = pyglet.model.MaterialGroup(material=self._material, program=self._program, parent=group)
+
+        self._vlist = self._create_vertexlist()
+
+        super().__init__([self._vlist], [self._group], self._batch)
+
+    def _create_vertexlist(self):
+        w = self._width / 2
+        h = self._height / 2
+        d = self._depth / 2
+        s = self._scale
+
+        vertices = (-w, -h, -d,   # front, bottom-left    0
+                    w, -h, -d,    # front, bottom-right   1
+                    w, h, -d,     # front, top-right      2
+                    -w, h, -d,    # front, top-left       3
+                    -w, -h, d,    # back, bottom-left     4
+                    w, -h, d,     # back, bottom-right    5
+                    w, h, d,      # back, top-right       6
+                    -w, h, d)     # back, top-left        7
+
+        vertices = tuple(v * s for v in vertices)
+
+        normals = (-0.5, -0.5, -1.0,    # back, bottom-left
+                   0.5, -0.5, -1.0,     # back, buttom-right
+                   0.5,  0.5, -1.0,     # back, top-right
+                   -0.5, 0.5, -1.0,     # back, top-left
+                   -0.5, -0.5, 0.0,     # front, bottom-left
+                   0.5, -0.5, 0.0,      # front, bottom-right
+                   0.5, 0.5, 0.0,       # front, top-right
+                   -0.5, 0.5, 0.0)      # front, top-left
+
+        indices = (0, 3, 2, 0, 2, 1,    # front
+                   4, 5, 6, 4, 6, 7,    # back
+                   4, 7, 3, 4, 3, 0,    # left
+                   1, 2, 6, 1, 6, 5,    # right
+                   3, 7, 6, 3, 6, 2,    # top
+                   0, 1, 5, 0, 5, 4)    # bottom
+
+        return self._program.vertex_list_indexed(len(vertices) // 3, pyglet.gl.GL_TRIANGLES, indices,
+                                                 batch=self._batch, group=self._group,
+                                                 position=('f', vertices),
+                                                 normals=('f', normals),
+                                                 colors=('f', self._color * (len(vertices) // 3)))
+
 
 _add_default_codecs()
```

### Comparing `pyglet-2.1.dev1/pyglet/model/codecs/__init__.py` & `pyglet-2.1.dev2/pyglet/model/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/model/codecs/gltf.py` & `pyglet-2.1.dev2/pyglet/model/codecs/gltf.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/model/codecs/obj.py` & `pyglet-2.1.dev2/pyglet/model/codecs/obj.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/resource.py` & `pyglet-2.1.dev2/pyglet/resource.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/shapes.py` & `pyglet-2.1.dev2/pyglet/shapes.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/sprite.py` & `pyglet-2.1.dev2/pyglet/sprite.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/text/__init__.py` & `pyglet-2.1.dev2/pyglet/text/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/text/caret.py` & `pyglet-2.1.dev2/pyglet/text/caret.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/text/document.py` & `pyglet-2.1.dev2/pyglet/text/document.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/text/formats/attributed.py` & `pyglet-2.1.dev2/pyglet/text/formats/attributed.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/text/formats/html.py` & `pyglet-2.1.dev2/pyglet/text/formats/html.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/text/formats/structured.py` & `pyglet-2.1.dev2/pyglet/text/formats/structured.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/text/layout/__init__.py` & `pyglet-2.1.dev2/pyglet/text/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/text/layout/base.py` & `pyglet-2.1.dev2/pyglet/text/layout/base.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/text/layout/incremental.py` & `pyglet-2.1.dev2/pyglet/text/layout/incremental.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/text/layout/scrolling.py` & `pyglet-2.1.dev2/pyglet/text/layout/scrolling.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/text/runlist.py` & `pyglet-2.1.dev2/pyglet/text/runlist.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/util.py` & `pyglet-2.1.dev2/pyglet/util.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/window/__init__.py` & `pyglet-2.1.dev2/pyglet/window/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,16 +404,16 @@
     _mouse_in_window = False
 
     _event_queue = None
     _enable_event_queue = True     # overridden by EventLoop.
     _allow_dispatch_event = False  # controlled by dispatch_events stack frame
 
     # Class attributes
-    _default_width = 960
-    _default_height = 540
+    _default_width = 1280
+    _default_height = 720
 
     # Create a default ShaderProgram, so the Window instance can
     # update the `WindowBlock` UBO shared by all default shaders.
     _default_vertex_source = """#version 150 core
         in vec4 position;
 
         uniform WindowBlock
```

### Comparing `pyglet-2.1.dev1/pyglet/window/cocoa/__init__.py` & `pyglet-2.1.dev2/pyglet/window/cocoa/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/window/cocoa/pyglet_delegate.py` & `pyglet-2.1.dev2/pyglet/window/cocoa/pyglet_delegate.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/window/cocoa/pyglet_textview.py` & `pyglet-2.1.dev2/pyglet/window/cocoa/pyglet_textview.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/window/cocoa/pyglet_view.py` & `pyglet-2.1.dev2/pyglet/window/cocoa/pyglet_view.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/window/cocoa/pyglet_window.py` & `pyglet-2.1.dev2/pyglet/window/cocoa/pyglet_window.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/window/cocoa/systemcursor.py` & `pyglet-2.1.dev2/pyglet/window/cocoa/systemcursor.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/window/event.py` & `pyglet-2.1.dev2/pyglet/window/event.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/window/headless/__init__.py` & `pyglet-2.1.dev2/pyglet/window/headless/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/window/key.py` & `pyglet-2.1.dev2/pyglet/window/key.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/window/mouse.py` & `pyglet-2.1.dev2/pyglet/window/mouse.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/window/win32/__init__.py` & `pyglet-2.1.dev2/pyglet/window/win32/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/pyglet/window/xlib/__init__.py` & `pyglet-2.1.dev2/pyglet/window/xlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglet-2.1.dev1/PKG-INFO` & `pyglet-2.1.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglet
-Version: 2.1.dev1
+Version: 2.1.dev2
 Summary: pyglet is a cross-platform games and multimedia package.
 Author-email: Alex Holkner & contributors <Alex.Holkner@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Project-URL: Home, https://pyglet.org
 
 [![pypi](https://badge.fury.io/py/pyglet.svg)](https://pypi.python.org/pypi/pyglet) [![rtd](https://readthedocs.org/projects/pyglet/badge/?version=latest)](https://pyglet.readthedocs.io) [![PyTest](https://github.com/pyglet/pyglet/actions/workflows/unittests.yml/badge.svg)](https://github.com/pyglet/pyglet/actions/workflows/unittests.yml)
```

