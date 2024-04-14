# Comparing `tmp/limoon-0.0.4.tar.gz` & `tmp/limoon-0.0.5.tar.gz`

## Comparing `limoon-0.0.4.tar` & `limoon-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 limoon-0.0.4/DOCUMENTATION.md
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 limoon-0.0.4/README.md
--rw-r--r--   0        0        0    31396 2020-02-02 00:00:00.000000 limoon-0.0.4/limoon-logo.png
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 limoon-0.0.4/.github/workflows/doc.yml
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 limoon-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 limoon-0.0.4/.github/workflows/test.yml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 limoon-0.0.4/src/limoon/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 limoon-0.0.4/src/limoon/constant.py
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 limoon-0.0.4/src/limoon/core.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 limoon-0.0.4/src/limoon/exception.py
--rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 limoon-0.0.4/src/limoon/model.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 limoon-0.0.4/src/limoon/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 limoon-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 limoon-0.0.4/tests/test.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 limoon-0.0.4/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 limoon-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 limoon-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 limoon-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     5554 2020-02-02 00:00:00.000000 limoon-0.0.5/DOCUMENTATION.md
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 limoon-0.0.5/README.md
+-rw-r--r--   0        0        0    31396 2020-02-02 00:00:00.000000 limoon-0.0.5/limoon-logo.png
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 limoon-0.0.5/.github/workflows/doc.yml
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 limoon-0.0.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 limoon-0.0.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 limoon-0.0.5/src/limoon/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 limoon-0.0.5/src/limoon/constant.py
+-rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 limoon-0.0.5/src/limoon/core.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 limoon-0.0.5/src/limoon/exception.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 limoon-0.0.5/src/limoon/model.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 limoon-0.0.5/src/limoon/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 limoon-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 limoon-0.0.5/tests/test.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 limoon-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 limoon-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 limoon-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 limoon-0.0.5/PKG-INFO
```

### Comparing `limoon-0.0.4/DOCUMENTATION.md` & `limoon-0.0.5/DOCUMENTATION.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,16 @@
   * [TopicNotFound](#limoon.exception.TopicNotFound)
   * [EntryNotFound](#limoon.exception.EntryNotFound)
   * [AuthorNotFound](#limoon.exception.AuthorNotFound)
 * [limoon.core](#limoon.core)
   * [get\_topic](#limoon.core.get_topic)
   * [get\_entry](#limoon.core.get_entry)
   * [get\_author](#limoon.core.get_author)
+  * [get\_author\_rank](#limoon.core.get_author_rank)
+  * [get\_author\_topic](#limoon.core.get_author_topic)
   * [get\_agenda](#limoon.core.get_agenda)
   * [get\_debe](#limoon.core.get_debe)
 * [limoon.model](#limoon.model)
   * [Rank](#limoon.model.Rank)
   * [Entry](#limoon.model.Entry)
   * [Topic](#limoon.model.Topic)
   * [Author](#limoon.model.Author)
@@ -116,14 +118,53 @@
 - `nickname` _str_ - Unique author nickname.
   
 
 **Returns**:
 
 - `model.Author` _class_ - Author data class.
 
+<a id="limoon.core.get_author_rank"></a>
+
+#### get\_author\_rank
+
+```python
+def get_author_rank(nickname: Nickname) -> model.Rank
+```
+
+This function get Ekşi Sözlük author rank.
+
+**Arguments**:
+
+- `nickname` _str_ - Unique author nickname.
+  
+
+**Returns**:
+
+- `model.Rank` _class_ - Rank data class.
+
+<a id="limoon.core.get_author_topic"></a>
+
+#### get\_author\_topic
+
+```python
+def get_author_topic(nickname: Nickname, max_entry: int = None) -> model.Topic
+```
+
+This function get Ekşi Sözlük author topic.
+
+**Arguments**:
+
+- `nickname` _str_ - Unique author nickname.
+- `max_entry` _int=None_ - Maximum number of entrys to be get from page.
+  
+
+**Returns**:
+
+- `model.Topic` _class_ - Topic data class.
+
 <a id="limoon.core.get_agenda"></a>
 
 #### get\_agenda
 
 ```python
 def get_agenda(max_topic: int = None,
                max_entry: int = None) -> Iterator[model.Topic]
@@ -214,15 +255,15 @@
 
 **Arguments**:
 
 - `id` _int_ - Unique topic identity.
 - `title` _str_ - Topic title.
 - `path` _str_ - Unique topic path.
 - `entrys` _class_ - Entrys written for topic.
-- `page_count` _int_ - Topic total page count.
+- `page_count` _int|None_ - Topic total page count.
 - `url` _str_ - Topic HTTP link.
 
 <a id="limoon.model.Author"></a>
 
 ## Author Objects
 
 ```python
```

### Comparing `limoon-0.0.4/README.md` & `limoon-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `limoon-0.0.4/limoon-logo.png` & `limoon-0.0.5/limoon-logo.png`

 * *Files identical despite different names*

### Comparing `limoon-0.0.4/.github/workflows/doc.yml` & `limoon-0.0.5/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `limoon-0.0.4/.github/workflows/publish.yml` & `limoon-0.0.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `limoon-0.0.4/.github/workflows/test.yml` & `limoon-0.0.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `limoon-0.0.4/src/limoon/core.py` & `limoon-0.0.5/src/limoon/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,22 +35,22 @@
     r = request(constant.TOPIC_ROUTE.format(topic_keywords))
 
     if r.status_code == HTTPStatus.NOT_FOUND:
         raise exception.TopicNotFound()
 
     h1 = r.html.find("h1#title", first=True)
     path = h1.find("a", first=True).attrs["href"]
-    page_count = r.html.find("div.pager", first=True).attrs["data-pagecount"]
+    page_count = r.html.find("div.pager", first=True)
 
     return model.Topic(
         int(h1.attrs["data-id"]),
         h1.attrs["data-title"],
         path[1:],
         utils.entry_parser(r.html, max_entry),
-        int(page_count),
+        int(page_count.attrs["data-pagecount"]) if page_count else page_count,
     )
 
 
 def get_entry(entry_id: EntryID) -> model.Entry:
     """This function get Ekşi Sözlük entry.
 
     Arguments:
@@ -103,21 +103,43 @@
         int(follower_count.text),
         int(following_count.text),
         avatar_url.attrs["src"],
         rank,
     )
 
 
-def get_author_rank():
-    pass
+def get_author_rank(nickname: Nickname) -> model.Rank:
+    """This function get Ekşi Sözlük author rank.
 
+    Arguments:
+    nickname (str): Unique author nickname. 
+
+    Returns:
+    model.Rank (class): Rank data class.
+    """
+
+    author = get_author(nickname)
+
+    return model.Rank(name=author.rank.name, karma=author.rank.karma)
 
-def get_author_topic():
-    pass
 
+def get_author_topic(nickname: Nickname, max_entry: int = None) -> model.Topic:
+    """This function get Ekşi Sözlük author topic.
+
+    Arguments:
+    nickname (str): Unique author nickname.
+    max_entry (int=None): Maximum number of entrys to be get from page.
+
+    Returns:
+    model.Topic (class): Topic data class.
+    """
+
+    r = request(constant.AUTHOR_TOPIC_ROUTE.format(nickname))
+    
+    return get_topic(urlparse(r.url).path[1:], max_entry=max_entry)
 
 def get_agenda(max_topic: int = None, max_entry: int = None) -> Iterator[model.Topic]:
     """This function get Ekşi Sözlük agenda (gündem) page.
 
     Arguments:
     max_topic (int=None): Maximum number of topics to be get from agenda.
     max_entry (int=None): Maximum number of entrys to be get from topic.
@@ -160,8 +182,8 @@
     for topic in topic_list[:max_entry]:
         yield get_entry(
             urlparse(topic.attrs["href"]).path.split("/")[-1],
         )
 
 
 def search_topic(search_keywords: SearchKeywords):
-    pass
+    raise NotImplementedError
```

### Comparing `limoon-0.0.4/src/limoon/model.py` & `limoon-0.0.5/src/limoon/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,23 +67,23 @@
     """Topic data class.
 
     Arguments:
     id (int): Unique topic identity.
     title (str): Topic title.
     path (str): Unique topic path.
     entrys (class): Entrys written for topic.
-    page_count (int): Topic total page count.
+    page_count (int|None): Topic total page count.
     url (str): Topic HTTP link.
     """
 
     id: int
     title: str
     path: str
     entrys: Iterator[Entry]
-    page_count: int
+    page_count: Union[int, None]
     url: URL = field(init=False)
 
     def __repr__(self):
         return f"Topic({self.id})"
 
     def __post_init__(self):
         self.url = constant.BASE_URL + constant.TOPIC_ROUTE.format(self.path)
```

### Comparing `limoon-0.0.4/src/limoon/utils.py` & `limoon-0.0.5/src/limoon/utils.py`

 * *Files identical despite different names*

### Comparing `limoon-0.0.4/tests/test.py` & `limoon-0.0.5/tests/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,14 +40,34 @@
         assert author.following_count > 1
         assert "https://img.ekstat.com" in author.avatar_url
         assert type(author.rank) is limoon.Rank
         assert type(author.rank.name) is str
         assert type(author.rank.karma) is int
         assert author.url == "https://eksisozluk.com/biri/ssg"
 
+    def test_get_author_rank(self):
+        author_rank = limoon.get_author_rank("ssg")
+
+        assert type(author_rank) is limoon.Rank
+        assert type(author_rank.name) is str
+        assert type(author_rank.karma) is int
+        assert author_rank.karma > 1 
+
+    def test_get_author_topic(self):
+        author_topic = limoon.get_author_topic("ssg")
+
+        assert type(author_topic) is limoon.Topic
+        assert author_topic.id == 31795
+        assert author_topic.title == "ssg"
+        assert author_topic.path == "ssg--31795"
+        assert len(list(author_topic.entrys)) > 1
+        assert type(list(author_topic.entrys)) is list
+        assert author_topic.page_count > 1
+        assert author_topic.url == "https://eksisozluk.com/ssg--31795"
+
 
 class TestException:
     def test_topic_not_found(self):
         with pytest.raises(exception.TopicNotFound):
             limoon.get_topic("böylebirbaslikyok")
 
     def test_entry_not_found(self):
```

### Comparing `limoon-0.0.4/.gitignore` & `limoon-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `limoon-0.0.4/LICENSE.txt` & `limoon-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `limoon-0.0.4/pyproject.toml` & `limoon-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `limoon-0.0.4/PKG-INFO` & `limoon-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: limoon
-Version: 0.0.4
+Version: 0.0.5
 Summary: Web scraper base Pythonic API for Ekşi Sözlük
 Project-URL: Source, https://github.com/beucismis/limoon
 Project-URL: Issues, https://github.com/beucismis/limoon/issues
 Project-URL: Documentation, https://github.com/beucismis/limoon/DOCUMENTATION.md
 Author-email: beucismis <beucismis@tutamail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

