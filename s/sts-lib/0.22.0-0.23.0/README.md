# Comparing `tmp/sts-lib-0.22.0.tar.gz` & `tmp/sts_lib-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sts-lib-0.22.0.tar", last modified: Fri Apr 12 08:50:37 2024, max compression
+gzip compressed data, was "sts_lib-0.23.0.tar", last modified: Sun Apr 14 08:56:06 2024, max compression
```

## Comparing `sts-lib-0.22.0.tar` & `sts_lib-0.23.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 08:50:37.906263 sts-lib-0.22.0/
--rw-rw-rw-   0        0        0    11358 2020-07-10 16:04:12.000000 sts-lib-0.22.0/LICENSE
--rw-rw-rw-   0        0        0       13 2024-04-08 13:49:48.000000 sts-lib-0.22.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6931 2024-04-12 08:50:37.906263 sts-lib-0.22.0/PKG-INFO
--rw-rw-rw-   0        0        0     5589 2024-04-11 14:01:20.000000 sts-lib-0.22.0/README.md
--rw-rw-rw-   0        0        0     1687 2024-04-12 08:50:37.910259 sts-lib-0.22.0/setup.cfg
--rw-rw-rw-   0        0        0       65 2024-04-08 13:49:48.000000 sts-lib-0.22.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:50:37.844327 sts-lib-0.22.0/sts/
--rw-rw-rw-   0        0        0    40155 2024-04-12 08:47:37.000000 sts-lib-0.22.0/sts/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-08 13:49:45.000000 sts-lib-0.22.0/sts/__main__.py
--rw-rw-rw-   0        0        0     7721 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:50:37.846324 sts-lib-0.22.0/sts/data/
-drwxrwxrwx   0        0        0        0 2024-04-12 08:50:37.865306 sts-lib-0.22.0/sts/data/config/
--rw-rw-rw-   0        0        0      653 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/config/_default.json
--rw-rw-rw-   0        0        0      369 2020-08-12 18:29:24.000000 sts-lib-0.22.0/sts/data/config/hk2s.json
--rw-rw-rw-   0        0        0      275 2020-07-12 06:22:39.000000 sts-lib-0.22.0/sts/data/config/hk2t.json
--rw-rw-rw-   0        0        0      323 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/config/jp2t.json
--rw-rw-rw-   0        0        0      289 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/config/s2hk.json
--rw-rw-rw-   0        0        0      201 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/config/s2t.json
--rw-rw-rw-   0        0        0      287 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/config/s2tw.json
--rw-rw-rw-   0        0        0      369 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/config/s2twp.json
--rw-rw-rw-   0        0        0      197 2020-07-12 06:22:39.000000 sts-lib-0.22.0/sts/data/config/t2hk.json
--rw-rw-rw-   0        0        0      211 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/config/t2jp.json
--rw-rw-rw-   0        0        0      201 2020-07-16 15:29:01.000000 sts-lib-0.22.0/sts/data/config/t2s.json
--rw-rw-rw-   0        0        0      195 2020-07-12 06:22:39.000000 sts-lib-0.22.0/sts/data/config/t2tw.json
--rw-rw-rw-   0        0        0      367 2020-07-12 06:22:39.000000 sts-lib-0.22.0/sts/data/config/tw2s.json
--rw-rw-rw-   0        0        0      413 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/config/tw2sp.json
--rw-rw-rw-   0        0        0      273 2020-07-12 06:22:39.000000 sts-lib-0.22.0/sts/data/config/tw2t.json
-drwxrwxrwx   0        0        0        0 2024-04-12 08:50:37.887283 sts-lib-0.22.0/sts/data/dictionary/
--rw-rw-rw-   0        0        0      595 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/dictionary/HKVariants.txt
--rw-rw-rw-   0        0        0     2865 2020-07-10 16:04:12.000000 sts-lib-0.22.0/sts/data/dictionary/HKVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0      103 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/dictionary/JPShinjitaiCharacters.txt
--rw-rw-rw-   0        0        0     2720 2020-07-10 16:04:12.000000 sts-lib-0.22.0/sts/data/dictionary/JPShinjitaiPhrases.txt
--rw-rw-rw-   0        0        0     3307 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/dictionary/JPVariants.txt
--rw-rw-rw-   0        0        0    38333 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/dictionary/STCharacters.txt
--rw-rw-rw-   0        0        0  1053351 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/dictionary/STPhrases.txt
--rw-rw-rw-   0        0        0    38740 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/dictionary/TSCharacters.txt
--rw-rw-rw-   0        0        0     5438 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/dictionary/TSPhrases.txt
--rw-rw-rw-   0        0        0     8014 2024-04-12 08:47:58.000000 sts-lib-0.22.0/sts/data/dictionary/TWPhrasesIT.txt
--rw-rw-rw-   0        0        0     2205 2020-07-10 16:04:12.000000 sts-lib-0.22.0/sts/data/dictionary/TWPhrasesName.txt
--rw-rw-rw-   0        0        0      608 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/dictionary/TWPhrasesOther.txt
--rw-rw-rw-   0        0        0      351 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/dictionary/TWVariants.txt
--rw-rw-rw-   0        0        0     1143 2020-07-12 14:58:22.000000 sts-lib-0.22.0/sts/data/dictionary/TWVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0    14070 2024-04-12 08:47:37.000000 sts-lib-0.22.0/sts/data/htmlpage.tpl.html
-drwxrwxrwx   0        0        0        0 2024-04-12 08:50:37.891278 sts-lib-0.22.0/sts/data/scheme/
--rw-rw-rw-   0        0        0    21633 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/scheme/st_multi.txt
--rw-rw-rw-   0        0        0      436 2024-04-12 08:49:25.000000 sts-lib-0.22.0/sts/data/scheme/ts_multi.txt
--rw-rw-rw-   0        0        0     2108 2020-07-10 16:04:12.000000 sts-lib-0.22.0/sts/data/scheme/variant.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 08:50:37.902267 sts-lib-0.22.0/sts_lib.egg-info/
--rw-rw-rw-   0        0        0     6931 2024-04-12 08:50:37.000000 sts-lib-0.22.0/sts_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1325 2024-04-12 08:50:37.000000 sts-lib-0.22.0/sts_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 08:50:37.000000 sts-lib-0.22.0/sts_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-12 08:50:37.000000 sts-lib-0.22.0/sts_lib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      170 2024-04-12 08:50:37.000000 sts-lib-0.22.0/sts_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-12 08:50:37.000000 sts-lib-0.22.0/sts_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 08:56:06.574401 sts_lib-0.23.0/
+-rw-rw-rw-   0        0        0    11358 2020-07-10 16:04:12.000000 sts_lib-0.23.0/LICENSE
+-rw-rw-rw-   0        0        0       13 2024-04-08 13:49:48.000000 sts_lib-0.23.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7172 2024-04-14 08:56:06.574401 sts_lib-0.23.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5830 2024-04-14 08:53:14.000000 sts_lib-0.23.0/README.md
+-rw-rw-rw-   0        0        0     1687 2024-04-14 08:56:06.575400 sts_lib-0.23.0/setup.cfg
+-rw-rw-rw-   0        0        0       65 2024-04-08 13:49:48.000000 sts_lib-0.23.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 08:56:06.522474 sts_lib-0.23.0/sts/
+-rw-rw-rw-   0        0        0    41481 2024-04-14 08:53:14.000000 sts_lib-0.23.0/sts/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-08 13:49:45.000000 sts_lib-0.23.0/sts/__main__.py
+-rw-rw-rw-   0        0        0     7754 2024-04-14 08:53:14.000000 sts_lib-0.23.0/sts/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-14 08:56:06.524455 sts_lib-0.23.0/sts/data/
+drwxrwxrwx   0        0        0        0 2024-04-14 08:56:06.540436 sts_lib-0.23.0/sts/data/config/
+-rw-rw-rw-   0        0        0      653 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/config/_default.json
+-rw-rw-rw-   0        0        0      369 2020-08-12 18:29:24.000000 sts_lib-0.23.0/sts/data/config/hk2s.json
+-rw-rw-rw-   0        0        0      275 2020-07-12 06:22:39.000000 sts_lib-0.23.0/sts/data/config/hk2t.json
+-rw-rw-rw-   0        0        0      323 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/config/jp2t.json
+-rw-rw-rw-   0        0        0      289 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/config/s2hk.json
+-rw-rw-rw-   0        0        0      201 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/config/s2t.json
+-rw-rw-rw-   0        0        0      287 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/config/s2tw.json
+-rw-rw-rw-   0        0        0      369 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/config/s2twp.json
+-rw-rw-rw-   0        0        0      197 2020-07-12 06:22:39.000000 sts_lib-0.23.0/sts/data/config/t2hk.json
+-rw-rw-rw-   0        0        0      211 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/config/t2jp.json
+-rw-rw-rw-   0        0        0      201 2020-07-16 15:29:01.000000 sts_lib-0.23.0/sts/data/config/t2s.json
+-rw-rw-rw-   0        0        0      195 2020-07-12 06:22:39.000000 sts_lib-0.23.0/sts/data/config/t2tw.json
+-rw-rw-rw-   0        0        0      367 2020-07-12 06:22:39.000000 sts_lib-0.23.0/sts/data/config/tw2s.json
+-rw-rw-rw-   0        0        0      413 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/config/tw2sp.json
+-rw-rw-rw-   0        0        0      273 2020-07-12 06:22:39.000000 sts_lib-0.23.0/sts/data/config/tw2t.json
+drwxrwxrwx   0        0        0        0 2024-04-14 08:56:06.559417 sts_lib-0.23.0/sts/data/dictionary/
+-rw-rw-rw-   0        0        0      595 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/dictionary/HKVariants.txt
+-rw-rw-rw-   0        0        0     2865 2020-07-10 16:04:12.000000 sts_lib-0.23.0/sts/data/dictionary/HKVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0      103 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/dictionary/JPShinjitaiCharacters.txt
+-rw-rw-rw-   0        0        0     2720 2020-07-10 16:04:12.000000 sts_lib-0.23.0/sts/data/dictionary/JPShinjitaiPhrases.txt
+-rw-rw-rw-   0        0        0     3307 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/dictionary/JPVariants.txt
+-rw-rw-rw-   0        0        0    38333 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/dictionary/STCharacters.txt
+-rw-rw-rw-   0        0        0  1053351 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/dictionary/STPhrases.txt
+-rw-rw-rw-   0        0        0    38740 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/dictionary/TSCharacters.txt
+-rw-rw-rw-   0        0        0     5438 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/dictionary/TSPhrases.txt
+-rw-rw-rw-   0        0        0     8014 2024-04-14 07:55:14.000000 sts_lib-0.23.0/sts/data/dictionary/TWPhrasesIT.txt
+-rw-rw-rw-   0        0        0     2205 2020-07-10 16:04:12.000000 sts_lib-0.23.0/sts/data/dictionary/TWPhrasesName.txt
+-rw-rw-rw-   0        0        0      608 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/dictionary/TWPhrasesOther.txt
+-rw-rw-rw-   0        0        0      351 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/dictionary/TWVariants.txt
+-rw-rw-rw-   0        0        0     1143 2020-07-12 14:58:22.000000 sts_lib-0.23.0/sts/data/dictionary/TWVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0    21012 2024-04-14 08:53:14.000000 sts_lib-0.23.0/sts/data/htmlpage.tpl.html
+drwxrwxrwx   0        0        0        0 2024-04-14 08:56:06.563415 sts_lib-0.23.0/sts/data/scheme/
+-rw-rw-rw-   0        0        0    21633 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/scheme/st_multi.txt
+-rw-rw-rw-   0        0        0      436 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/scheme/ts_multi.txt
+-rw-rw-rw-   0        0        0     2108 2020-07-10 16:04:12.000000 sts_lib-0.23.0/sts/data/scheme/variant.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 08:56:06.571405 sts_lib-0.23.0/sts_lib.egg-info/
+-rw-rw-rw-   0        0        0     7172 2024-04-14 08:56:06.000000 sts_lib-0.23.0/sts_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1325 2024-04-14 08:56:06.000000 sts_lib-0.23.0/sts_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 08:56:06.000000 sts_lib-0.23.0/sts_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-14 08:56:06.000000 sts_lib-0.23.0/sts_lib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      170 2024-04-14 08:56:06.000000 sts_lib-0.23.0/sts_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-14 08:56:06.000000 sts_lib-0.23.0/sts_lib.egg-info/top_level.txt
```

### Comparing `sts-lib-0.22.0/LICENSE` & `sts_lib-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sts-lib-0.22.0/PKG-INFO` & `sts_lib-0.23.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.22.0
+Version: 0.23.0
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -62,15 +62,15 @@
   * `-c CONFIG` 指定配置檔，可為內建配置檔名稱或自製 JSON 配置檔的路徑。可用的內建配置檔詳見 [sts/data/config](https://github.com/danny0838/sts-lib/tree/master/sts/data/config) 目錄，可簡寫，例如輸入 `s2t` 代表使用 `sts/data/config/s2t.json`。
   * `-f FORMAT` 指定輸出格式，可用格式如下：
     * `txt`：純文字，適合一般使用。
     * `txtm`：純文字加轉換標示。
     * `html`：加上 HTML 標記的文本，可嵌入至網頁應用程式做互動式校對。
     * `htmlpage`：加入 HTML 樣式的網頁，可直接開啟做互動式校對。
     * `json`：以 JSON 格式表示轉換輸出，可用其他程式進一步解析處理。
-  * `--exclude PATTERN` 指定用於忽略簡繁轉換的正規表示式。有指定 `return` 子群組時會取代為子群組的值。
+  * `--exclude PATTERN` 指定用於忽略簡繁轉換的正規表示式。有指定 `return`（或 `return1`, `return2`, ... 等）子群組時會取代為子群組的值。
     * 例如 `sts convert -c s2twp --exclude "「.*?」"` 會把 `「程序」正义` 轉換為 `「程序」正義`。
     * 例如 `sts convert -c s2twp --exclude "-{(?P<return>.*?)}-"` 會把 `-{程序}-正义` 轉換為 `程序正義`。
   * `--in-enc ENCODING` 指定輸入編碼。可用編碼參見[這裡](https://docs.python.org/3/library/codecs.html#standard-encodings)。
   * `--out-enc ENCODING` 指定輸出編碼。可用編碼參見[這裡](https://docs.python.org/3/library/codecs.html#standard-encodings)。
   * `-o OUTPUT` 可重覆多次，指定對應輸入檔案轉換結果的輸出路徑。（無對應者輸出至原檔）
   * `--stdout` 將所有轉換結果輸出至標準輸出 STDOUT。
 
@@ -117,19 +117,23 @@
  *     (or the directory of this config file). Each should be a .tlist
  *     (compiled trie), .jlist (compiled table), or .list (plain text table).
  * @property {string} mode - the mode to handle the loaded source files: "load"
  *     to simply merge the loaded keys and values; "swap" to reverse the
  *     dictionary (i.e. use the values as keys and the keys as values); "join"
  *     to build from a chain of dictionaries (in which case src must be an
  *     array of subarrays of strings)
- * @property {boolean} [sort] - true to sort the keys of the output dictionary
  * @property {Array.<(string|string[])>} src - the source files. Each as an
  *     absolute path, or a path relative to the directory of this config file,
  *     or the basename of a built-in dictionary file. Each should be a .txt or
  *     .list dictionary file.
+ * @property {boolean} [sort] - true to sort the keys of the output dictionary.
+ * @property {string} [include] - a regex filter that discards non-matched
+ *     conversion values.
+ * @property {string} [exclude] - a regex filter that discards matched
+ *     conversion values.
  */
 ```
 
 ## License 許可協議
 
 本專案以 Apache License 2.0 協議授權使用。
```

### Comparing `sts-lib-0.22.0/README.md` & `sts_lib-0.23.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   * `-c CONFIG` 指定配置檔，可為內建配置檔名稱或自製 JSON 配置檔的路徑。可用的內建配置檔詳見 [sts/data/config](https://github.com/danny0838/sts-lib/tree/master/sts/data/config) 目錄，可簡寫，例如輸入 `s2t` 代表使用 `sts/data/config/s2t.json`。
   * `-f FORMAT` 指定輸出格式，可用格式如下：
     * `txt`：純文字，適合一般使用。
     * `txtm`：純文字加轉換標示。
     * `html`：加上 HTML 標記的文本，可嵌入至網頁應用程式做互動式校對。
     * `htmlpage`：加入 HTML 樣式的網頁，可直接開啟做互動式校對。
     * `json`：以 JSON 格式表示轉換輸出，可用其他程式進一步解析處理。
-  * `--exclude PATTERN` 指定用於忽略簡繁轉換的正規表示式。有指定 `return` 子群組時會取代為子群組的值。
+  * `--exclude PATTERN` 指定用於忽略簡繁轉換的正規表示式。有指定 `return`（或 `return1`, `return2`, ... 等）子群組時會取代為子群組的值。
     * 例如 `sts convert -c s2twp --exclude "「.*?」"` 會把 `「程序」正义` 轉換為 `「程序」正義`。
     * 例如 `sts convert -c s2twp --exclude "-{(?P<return>.*?)}-"` 會把 `-{程序}-正义` 轉換為 `程序正義`。
   * `--in-enc ENCODING` 指定輸入編碼。可用編碼參見[這裡](https://docs.python.org/3/library/codecs.html#standard-encodings)。
   * `--out-enc ENCODING` 指定輸出編碼。可用編碼參見[這裡](https://docs.python.org/3/library/codecs.html#standard-encodings)。
   * `-o OUTPUT` 可重覆多次，指定對應輸入檔案轉換結果的輸出路徑。（無對應者輸出至原檔）
   * `--stdout` 將所有轉換結果輸出至標準輸出 STDOUT。
 
@@ -85,19 +85,23 @@
  *     (or the directory of this config file). Each should be a .tlist
  *     (compiled trie), .jlist (compiled table), or .list (plain text table).
  * @property {string} mode - the mode to handle the loaded source files: "load"
  *     to simply merge the loaded keys and values; "swap" to reverse the
  *     dictionary (i.e. use the values as keys and the keys as values); "join"
  *     to build from a chain of dictionaries (in which case src must be an
  *     array of subarrays of strings)
- * @property {boolean} [sort] - true to sort the keys of the output dictionary
  * @property {Array.<(string|string[])>} src - the source files. Each as an
  *     absolute path, or a path relative to the directory of this config file,
  *     or the basename of a built-in dictionary file. Each should be a .txt or
  *     .list dictionary file.
+ * @property {boolean} [sort] - true to sort the keys of the output dictionary.
+ * @property {string} [include] - a regex filter that discards non-matched
+ *     conversion values.
+ * @property {string} [exclude] - a regex filter that discards matched
+ *     conversion values.
  */
 ```
 
 ## License 許可協議
 
 本專案以 Apache License 2.0 協議授權使用。
```

### Comparing `sts-lib-0.22.0/setup.cfg` & `sts_lib-0.23.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sts-lib-0.22.0/sts/__init__.py` & `sts_lib-0.23.0/sts/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import html
 import json
 import math
 import os
 import re
 import sys
-from collections import OrderedDict, namedtuple
+from collections import namedtuple
 from contextlib import nullcontext
 
 try:
     from functools import cached_property
 except ImportError:
     # polyfill for Python < 3.8
     def cached_property(fn):
@@ -43,15 +43,15 @@
         @_lazyprop.setter
         def _lazyprop(self, value):
             setattr(self, attr_name, value)
 
         return _lazyprop
 
 
-__version__ = '0.22.0'
+__version__ = '0.23.0'
 
 StsDictMatch = namedtuple('StsDictMatch', ['conv', 'start', 'end'])
 StsDictConv = namedtuple('StsDictConv', ['key', 'values'])
 
 
 class StreamList(list):
     """Convert an iterable into a serializable "list".
@@ -611,27 +611,27 @@
             a list of possible conversions.
         """
         text = parts
         parts = self._split(parts)
 
         stack = [(parts, 0, 0)]
         substack = []
-        results = OrderedDict()
-        while len(stack):
+        results = {}
+        while stack:
             (parts, matched, nextindex) = data = stack.pop()
             if nextindex < len(parts):
                 self._apply_enum_sub(substack, data, include_short=include_short, include_self=include_self)
-                while len(substack):
+                while substack:
                     stack.append(substack.pop())
             elif matched > 0:
                 results[''.join(parts)] = True
 
         results = list(results)
 
-        if len(results) == 0:
+        if not results:
             results.append(text if isinstance(text, str) else ''.join(text))
 
         return results
 
     def _apply_enum_sub(self, stack, data, include_short=False, include_self=False):
         """Helper function of apply_enum
         """
@@ -924,19 +924,33 @@
                 self.make(cf, base_dir=config_dir, output_dir=output_dir, skip_requires=skip_requires, quiet=quiet)
 
         # make the requested dicts
         for dict_ in config['dicts']:
             dest = os.path.join(output_dir or config_dir, dict_['file'])
             format = os.path.splitext(dest)[1][1:].lower()
             mode = dict_['mode']
-            sort = dict_.get('sort', False)
             files = [self.get_stsdict_file(f, base_dir=config_dir)
                      if isinstance(f, str)
                      else [self.get_stsdict_file(i, base_dir=config_dir) for i in f]
                      for f in dict_['src']]
+            sort = dict_.get('sort', False)
+            include = dict_.get('include', None)
+            exclude = dict_.get('exclude', None)
+
+            if include is not None:
+                try:
+                    include = re.compile(include)
+                except re.error as exc:
+                    raise ValueError(f'regex syntax error of the include filter: {exc}')
+
+            if exclude is not None:
+                try:
+                    exclude = re.compile(exclude)
+                except re.error as exc:
+                    raise ValueError(f'regex syntax error of the exclude filter: {exc}')
 
             if not skip_check and not self.check_update(dest, files):
                 if not quiet:
                     print(f'skip making (up-to-date): {dest}')
                 continue
 
             if not quiet:
@@ -947,14 +961,24 @@
             elif mode == 'swap':
                 table = Table().load(*files).swap()
             elif mode == 'join':
                 table = Table().load_filegroups(files)
             else:
                 raise ValueError(f'Specified mode "{mode}" is not supported.')
 
+            if include is not None or exclude is not None:
+                _table = table
+                table = Table()
+                for key, values in _table.items():
+                    values = [v for v in values
+                              if (include is None or include.search(v))
+                              and (exclude is None or not exclude.search(v))]
+                    if values:
+                        table.add(key, values)
+
             os.makedirs(os.path.dirname(dest), exist_ok=True)
 
             if format == 'tlist':
                 Trie(table).dumpjson(dest, sort=sort)
             elif format == 'jlist':
                 table.dumpjson(dest, sort=sort)
             else:  # default: list
@@ -974,19 +998,19 @@
             return config
 
         relative_config = os.path.join(base_dir, config) if base_dir is not None else config
         if os.path.isfile(relative_config):
             return relative_config
 
         if os.path.basename(config) == config:
-            search_file = os.path.join(self.default_config_dir, config)
+            search_file = os.path.join(self.config_dir, config)
             if os.path.isfile(search_file):
                 return search_file
             if not config.lower().endswith('.json'):
-                search_file = os.path.join(self.default_config_dir, config + '.json')
+                search_file = os.path.join(self.config_dir, config + '.json')
                 if os.path.isfile(search_file):
                     return search_file
 
         return relative_config
 
     def get_stsdict_file(self, stsdict, base_dir=None):
         """Calculate the path of a dictionary file.
@@ -1000,15 +1024,15 @@
             return stsdict
 
         relative_stsdict = os.path.join(base_dir, stsdict) if base_dir is not None else stsdict
         if os.path.isfile(relative_stsdict):
             return relative_stsdict
 
         if os.path.basename(stsdict) == stsdict:
-            search_file = os.path.join(self.default_dictionary_dir, stsdict)
+            search_file = os.path.join(self.dictionary_dir, stsdict)
             if os.path.isfile(search_file):
                 return search_file
 
         return relative_stsdict
 
     def check_update(self, output, filegroups):
         """Check if the output file needs update.
@@ -1021,16 +1045,16 @@
                 files = [files]
             for file in files:
                 if os.path.getmtime(file) > os.path.getmtime(output):
                     return True
 
         return False
 
-    default_config_dir = os.path.join(os.path.dirname(__file__), 'data', 'config')
-    default_dictionary_dir = os.path.join(os.path.dirname(__file__), 'data', 'dictionary')
+    config_dir = os.path.join(os.path.dirname(__file__), 'data', 'config')
+    dictionary_dir = os.path.join(os.path.dirname(__file__), 'data', 'dictionary')
 
 
 class StsConverter():
     """Convert a text using an stsdict.
     """
     def __init__(self, stsdict):
         """Initialize a converter.
@@ -1057,37 +1081,39 @@
             the next converted part as an StsDictConv, or an unmatched part as
             a str.
         """
         if exclude is None:
             yield from self.table.apply(text)
             return
 
-        def convert_with_regex(text, regex):
-            index = 0
-            for m in regex.finditer(text):
-                start, end = m.span(0)
-
-                t = text[index:start]
-                if t:
-                    yield from self.table.apply(t)
-
-                try:
-                    t = m.group('return')
-                except IndexError:
-                    t = m.group(0)
-                if t:
-                    yield t
+        yield from self._convert_with_filter(text, exclude)
 
-                index = end
+    def _convert_with_filter(self, text, exclude):
+        index = 0
+        for m in exclude.finditer(text):
+            start, end = m.span(0)
 
-            t = text[index:]
+            t = text[index:start]
             if t:
                 yield from self.table.apply(t)
 
-        yield from convert_with_regex(text, exclude)
+            for k, v in m.groupdict().items():
+                if self.exclude_return_group_pattern.search(k) and v is not None:
+                    t = v
+                    break
+            else:
+                t = m.group(0)
+            if t:
+                yield t
+
+            index = end
+
+        t = text[index:]
+        if t:
+            yield from self.table.apply(t)
 
     def convert_formatted(self, text, format=None, exclude=None):
         """Convert a text and yield each formatted part.
         """
         conv = self.convert(text, exclude=exclude)
         format = format if format is not None else 'txt'
         formatter = getattr(self, f'_convert_formatted_{format}')
@@ -1125,25 +1151,34 @@
                 for i, v in enumerate(news):
                     hidden = '' if i == 0 else ' hidden'
                     content += f'<ins{hidden}>{html.escape(v)}</ins>'
 
                 part = f"""<a>{content}</a>"""
                 yield part
 
-    def _convert_formatted_htmlpage(self, parts):
-        with open(self.default_htmlpage_template,
-                  encoding='UTF-8', newline='') as fh:
+    def _convert_formatted_htmlpage(self, parts, template=None):
+        if template is None:
+            template = self.htmlpage_template
+
+        try:
+            fh = open(template, encoding='UTF-8', newline='')
+        except TypeError:
+            fh = nullcontext(template)
+
+        with fh as fh:
             html = fh.read()
 
         pos = 0
-        for m in self.regex_template.finditer(html):
+        for m in self.template_placeholder_pattern.finditer(html):
             yield html[pos:m.start(0)]
 
             key = m.group(1)
-            if key == 'CONTENT':
+            if key == '':
+                yield '%'
+            elif key == 'CONTENT':
                 yield from self._convert_formatted_html(parts)
             elif key == 'VERSION':
                 yield __version__
 
             pos = m.end(0)
 
         yield html[pos:]
@@ -1187,10 +1222,10 @@
             open(output, 'w', encoding=output_encoding, newline='')
             if output
             else nullcontext(sys.stdout)
         ) as fh:
             for part in conv:
                 fh.write(part)
 
-    default_htmlpage_template = os.path.join(os.path.dirname(__file__), 'data', 'htmlpage.tpl.html')
-
-    regex_template = re.compile(r'%(\w+)%')
+    exclude_return_group_pattern = re.compile(r'^return\d*$')
+    template_placeholder_pattern = re.compile(r'%(\w*)%')
+    htmlpage_template = os.path.join(os.path.dirname(__file__), 'data', 'htmlpage.tpl.html')
```

### Comparing `sts-lib-0.22.0/sts/cli.py` & `sts_lib-0.23.0/sts/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,16 @@
                                 help="""the config to use, either a built-in config name or a path to a custom JSON file
 (built-in configs: s2t|t2s|s2tw|tw2s|s2twp|tw2sp|s2hk|hk2s|t2tw|tw2t|t2hk|hk2t|t2jp|jp2t)
 (default: %(default)s)""")
     parser_convert.add_argument('-f', '--format', default='txt',
                                 choices=['txt', 'txtm', 'html', 'htmlpage', 'json'], metavar='FORMAT',
                                 help="""output format (txt|txtm|html|htmlpage|json) (default: %(default)s)""")
     parser_convert.add_argument('--exclude', type=regex,
-                                help="""exclude text matching given regex from conversion, and replace it with the "return" subgroup value if exists""")
+                                help="""exclude text matching given regex from conversion, and replace it with the
+"return" (or "return1", "return2", etc.) subgroup value if exists""")
     parser_convert.add_argument('--in-enc', default='UTF-8', metavar='ENCODING',
                                 help="""encoding for input (default: %(default)s)""")
     parser_convert.add_argument('--out-enc', default='UTF-8', metavar='ENCODING',
                                 help="""encoding for output (default: %(default)s)""")
     parser_convert.add_argument('-o', '--output', default=[], action='append',
                                 help="""path to output (for the corresponding input) (default: to input)""")
     parser_convert.add_argument('--stdout', default=False, action='store_true',
```

### Comparing `sts-lib-0.22.0/sts/data/config/_default.json` & `sts_lib-0.23.0/sts/data/config/_default.json`

 * *Files identical despite different names*

### Comparing `sts-lib-0.22.0/sts/data/dictionary/HKVariants.txt` & `sts_lib-0.23.0/sts/data/dictionary/HKVariants.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.22.0/sts/data/dictionary/HKVariantsRevPhrases.txt` & `sts_lib-0.23.0/sts/data/dictionary/HKVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.22.0/sts/data/dictionary/JPShinjitaiPhrases.txt` & `sts_lib-0.23.0/sts/data/dictionary/JPShinjitaiPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.22.0/sts/data/dictionary/JPVariants.txt` & `sts_lib-0.23.0/sts/data/dictionary/JPVariants.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.22.0/sts/data/dictionary/STCharacters.txt` & `sts_lib-0.23.0/sts/data/dictionary/STCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.22.0/sts/data/dictionary/STPhrases.txt` & `sts_lib-0.23.0/sts/data/dictionary/STPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.22.0/sts/data/dictionary/TSCharacters.txt` & `sts_lib-0.23.0/sts/data/dictionary/TSCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.22.0/sts/data/dictionary/TSPhrases.txt` & `sts_lib-0.23.0/sts/data/dictionary/TSPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.22.0/sts/data/dictionary/TWPhrasesIT.txt` & `sts_lib-0.23.0/sts/data/dictionary/TWPhrasesIT.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.22.0/sts/data/dictionary/TWPhrasesName.txt` & `sts_lib-0.23.0/sts/data/dictionary/TWPhrasesName.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.22.0/sts/data/dictionary/TWPhrasesOther.txt` & `sts_lib-0.23.0/sts/data/dictionary/TWPhrasesOther.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.22.0/sts/data/dictionary/TWVariantsRevPhrases.txt` & `sts_lib-0.23.0/sts/data/dictionary/TWVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.22.0/sts/data/scheme/st_multi.txt` & `sts_lib-0.23.0/sts/data/scheme/st_multi.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.22.0/sts/data/scheme/variant.txt` & `sts_lib-0.23.0/sts/data/scheme/variant.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.22.0/sts_lib.egg-info/PKG-INFO` & `sts_lib-0.23.0/sts_lib.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.22.0
+Version: 0.23.0
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -62,15 +62,15 @@
   * `-c CONFIG` 指定配置檔，可為內建配置檔名稱或自製 JSON 配置檔的路徑。可用的內建配置檔詳見 [sts/data/config](https://github.com/danny0838/sts-lib/tree/master/sts/data/config) 目錄，可簡寫，例如輸入 `s2t` 代表使用 `sts/data/config/s2t.json`。
   * `-f FORMAT` 指定輸出格式，可用格式如下：
     * `txt`：純文字，適合一般使用。
     * `txtm`：純文字加轉換標示。
     * `html`：加上 HTML 標記的文本，可嵌入至網頁應用程式做互動式校對。
     * `htmlpage`：加入 HTML 樣式的網頁，可直接開啟做互動式校對。
     * `json`：以 JSON 格式表示轉換輸出，可用其他程式進一步解析處理。
-  * `--exclude PATTERN` 指定用於忽略簡繁轉換的正規表示式。有指定 `return` 子群組時會取代為子群組的值。
+  * `--exclude PATTERN` 指定用於忽略簡繁轉換的正規表示式。有指定 `return`（或 `return1`, `return2`, ... 等）子群組時會取代為子群組的值。
     * 例如 `sts convert -c s2twp --exclude "「.*?」"` 會把 `「程序」正义` 轉換為 `「程序」正義`。
     * 例如 `sts convert -c s2twp --exclude "-{(?P<return>.*?)}-"` 會把 `-{程序}-正义` 轉換為 `程序正義`。
   * `--in-enc ENCODING` 指定輸入編碼。可用編碼參見[這裡](https://docs.python.org/3/library/codecs.html#standard-encodings)。
   * `--out-enc ENCODING` 指定輸出編碼。可用編碼參見[這裡](https://docs.python.org/3/library/codecs.html#standard-encodings)。
   * `-o OUTPUT` 可重覆多次，指定對應輸入檔案轉換結果的輸出路徑。（無對應者輸出至原檔）
   * `--stdout` 將所有轉換結果輸出至標準輸出 STDOUT。
 
@@ -117,19 +117,23 @@
  *     (or the directory of this config file). Each should be a .tlist
  *     (compiled trie), .jlist (compiled table), or .list (plain text table).
  * @property {string} mode - the mode to handle the loaded source files: "load"
  *     to simply merge the loaded keys and values; "swap" to reverse the
  *     dictionary (i.e. use the values as keys and the keys as values); "join"
  *     to build from a chain of dictionaries (in which case src must be an
  *     array of subarrays of strings)
- * @property {boolean} [sort] - true to sort the keys of the output dictionary
  * @property {Array.<(string|string[])>} src - the source files. Each as an
  *     absolute path, or a path relative to the directory of this config file,
  *     or the basename of a built-in dictionary file. Each should be a .txt or
  *     .list dictionary file.
+ * @property {boolean} [sort] - true to sort the keys of the output dictionary.
+ * @property {string} [include] - a regex filter that discards non-matched
+ *     conversion values.
+ * @property {string} [exclude] - a regex filter that discards matched
+ *     conversion values.
  */
 ```
 
 ## License 許可協議
 
 本專案以 Apache License 2.0 協議授權使用。
```

### Comparing `sts-lib-0.22.0/sts_lib.egg-info/SOURCES.txt` & `sts_lib-0.23.0/sts_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

