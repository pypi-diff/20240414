# Comparing `tmp/hawkmoth-0.8.0.tar.gz` & `tmp/hawkmoth-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hawkmoth-0.8.0.tar", last modified: Thu May 20 21:22:37 2021, max compression
+gzip compressed data, was "hawkmoth-0.9.0.tar", last modified: Thu Sep 30 13:24:08 2021, max compression
```

## Comparing `hawkmoth-0.8.0.tar` & `hawkmoth-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 jani      (1000) jani      (1000)        0 2021-05-20 21:22:37.801227 hawkmoth-0.8.0/
--rw-r--r--   0 jani      (1000) jani      (1000)     1316 2017-08-15 19:45:04.000000 hawkmoth-0.8.0/LICENSE
--rw-r--r--   0 jani      (1000) jani      (1000)     5365 2021-05-20 21:22:37.801227 hawkmoth-0.8.0/PKG-INFO
--rw-r--r--   0 jani      (1000) jani      (1000)     3521 2021-04-30 09:35:10.000000 hawkmoth-0.8.0/README.rst
-drwxr-xr-x   0 jani      (1000) jani      (1000)        0 2021-05-20 21:22:37.801227 hawkmoth-0.8.0/hawkmoth/
--rw-r--r--   0 jani      (1000) jani      (1000)        6 2021-05-20 21:20:55.000000 hawkmoth-0.8.0/hawkmoth/VERSION
--rw-r--r--   0 jani      (1000) jani      (1000)     6179 2021-05-20 21:02:40.000000 hawkmoth-0.8.0/hawkmoth/__init__.py
--rw-r--r--   0 jani      (1000) jani      (1000)     1897 2021-05-15 11:11:15.000000 hawkmoth-0.8.0/hawkmoth/__main__.py
--rw-r--r--   0 jani      (1000) jani      (1000)    12156 2021-05-13 10:34:31.000000 hawkmoth-0.8.0/hawkmoth/parser.py
-drwxr-xr-x   0 jani      (1000) jani      (1000)        0 2021-05-20 21:22:37.801227 hawkmoth-0.8.0/hawkmoth/util/
--rw-r--r--   0 jani      (1000) jani      (1000)        0 2019-01-26 16:10:12.000000 hawkmoth-0.8.0/hawkmoth/util/__init__.py
--rw-r--r--   0 jani      (1000) jani      (1000)     1492 2021-05-15 11:08:50.000000 hawkmoth-0.8.0/hawkmoth/util/compiler.py
--rw-r--r--   0 jani      (1000) jani      (1000)     2590 2021-05-20 21:02:40.000000 hawkmoth-0.8.0/hawkmoth/util/doccompat.py
--rw-r--r--   0 jani      (1000) jani      (1000)     3694 2021-05-20 21:02:40.000000 hawkmoth-0.8.0/hawkmoth/util/docstr.py
--rw-r--r--   0 jani      (1000) jani      (1000)      857 2021-01-29 20:33:58.000000 hawkmoth-0.8.0/hawkmoth/util/readthedocs.py
--rw-r--r--   0 jani      (1000) jani      (1000)      305 2021-05-13 10:33:57.000000 hawkmoth-0.8.0/hawkmoth/util/strutil.py
-drwxr-xr-x   0 jani      (1000) jani      (1000)        0 2021-05-20 21:22:37.801227 hawkmoth-0.8.0/hawkmoth.egg-info/
--rw-r--r--   0 jani      (1000) jani      (1000)     5365 2021-05-20 21:22:37.000000 hawkmoth-0.8.0/hawkmoth.egg-info/PKG-INFO
--rw-r--r--   0 jani      (1000) jani      (1000)      497 2021-05-20 21:22:37.000000 hawkmoth-0.8.0/hawkmoth.egg-info/SOURCES.txt
--rw-r--r--   0 jani      (1000) jani      (1000)        1 2021-05-20 21:22:37.000000 hawkmoth-0.8.0/hawkmoth.egg-info/dependency_links.txt
--rw-r--r--   0 jani      (1000) jani      (1000)       39 2021-05-20 21:22:37.000000 hawkmoth-0.8.0/hawkmoth.egg-info/requires.txt
--rw-r--r--   0 jani      (1000) jani      (1000)        9 2021-05-20 21:22:37.000000 hawkmoth-0.8.0/hawkmoth.egg-info/top_level.txt
--rw-r--r--   0 jani      (1000) jani      (1000)      104 2021-04-30 09:18:27.000000 hawkmoth-0.8.0/pyproject.toml
--rw-r--r--   0 jani      (1000) jani      (1000)     1067 2021-05-20 21:22:37.801227 hawkmoth-0.8.0/setup.cfg
-drwxr-xr-x   0 jani      (1000) jani      (1000)        0 2021-05-20 21:22:37.801227 hawkmoth-0.8.0/test/
--rwxr-xr-x   0 jani      (1000) jani      (1000)     1497 2021-05-20 21:02:40.000000 hawkmoth-0.8.0/test/test_cautodoc.py
--rwxr-xr-x   0 jani      (1000) jani      (1000)     1351 2021-05-20 21:02:40.000000 hawkmoth-0.8.0/test/test_hawkmoth.py
--rw-r--r--   0 jani      (1000) jani      (1000)     2217 2021-05-20 21:02:40.000000 hawkmoth-0.8.0/test/testenv.py
+drwxr-xr-x   0 jani      (1000) jani      (1000)        0 2021-09-30 13:24:08.118065 hawkmoth-0.9.0/
+-rw-r--r--   0 jani      (1000) jani      (1000)     1316 2017-08-15 19:45:04.000000 hawkmoth-0.9.0/LICENSE
+-rw-r--r--   0 jani      (1000) jani      (1000)     5455 2021-09-30 13:24:08.118065 hawkmoth-0.9.0/PKG-INFO
+-rw-r--r--   0 jani      (1000) jani      (1000)     4552 2021-09-26 15:38:43.000000 hawkmoth-0.9.0/README.rst
+drwxr-xr-x   0 jani      (1000) jani      (1000)        0 2021-09-30 13:24:08.118065 hawkmoth-0.9.0/hawkmoth/
+-rw-r--r--   0 jani      (1000) jani      (1000)        6 2021-09-30 13:18:41.000000 hawkmoth-0.9.0/hawkmoth/VERSION
+-rw-r--r--   0 jani      (1000) jani      (1000)     9406 2021-09-30 12:50:41.000000 hawkmoth-0.9.0/hawkmoth/__init__.py
+-rw-r--r--   0 jani      (1000) jani      (1000)     1976 2021-09-26 15:38:43.000000 hawkmoth-0.9.0/hawkmoth/__main__.py
+-rw-r--r--   0 jani      (1000) jani      (1000)     6136 2021-09-30 12:52:55.000000 hawkmoth-0.9.0/hawkmoth/docstring.py
+-rw-r--r--   0 jani      (1000) jani      (1000)    11135 2021-09-30 12:50:41.000000 hawkmoth-0.9.0/hawkmoth/parser.py
+drwxr-xr-x   0 jani      (1000) jani      (1000)        0 2021-09-30 13:24:08.118065 hawkmoth-0.9.0/hawkmoth/util/
+-rw-r--r--   0 jani      (1000) jani      (1000)        0 2019-01-26 16:10:12.000000 hawkmoth-0.9.0/hawkmoth/util/__init__.py
+-rw-r--r--   0 jani      (1000) jani      (1000)     1492 2021-09-26 12:15:51.000000 hawkmoth-0.9.0/hawkmoth/util/compiler.py
+-rw-r--r--   0 jani      (1000) jani      (1000)     2590 2021-09-10 10:58:08.000000 hawkmoth-0.9.0/hawkmoth/util/doccompat.py
+-rw-r--r--   0 jani      (1000) jani      (1000)      857 2021-01-29 20:33:58.000000 hawkmoth-0.9.0/hawkmoth/util/readthedocs.py
+-rw-r--r--   0 jani      (1000) jani      (1000)      267 2021-09-26 15:38:43.000000 hawkmoth-0.9.0/hawkmoth/util/strutil.py
+drwxr-xr-x   0 jani      (1000) jani      (1000)        0 2021-09-30 13:24:08.118065 hawkmoth-0.9.0/hawkmoth.egg-info/
+-rw-r--r--   0 jani      (1000) jani      (1000)     5455 2021-09-30 13:24:08.000000 hawkmoth-0.9.0/hawkmoth.egg-info/PKG-INFO
+-rw-r--r--   0 jani      (1000) jani      (1000)      510 2021-09-30 13:24:08.000000 hawkmoth-0.9.0/hawkmoth.egg-info/SOURCES.txt
+-rw-r--r--   0 jani      (1000) jani      (1000)        1 2021-09-30 13:24:08.000000 hawkmoth-0.9.0/hawkmoth.egg-info/dependency_links.txt
+-rw-r--r--   0 jani      (1000) jani      (1000)       50 2021-09-30 13:24:08.000000 hawkmoth-0.9.0/hawkmoth.egg-info/requires.txt
+-rw-r--r--   0 jani      (1000) jani      (1000)        9 2021-09-30 13:24:08.000000 hawkmoth-0.9.0/hawkmoth.egg-info/top_level.txt
+-rw-r--r--   0 jani      (1000) jani      (1000)      104 2021-04-30 09:18:27.000000 hawkmoth-0.9.0/pyproject.toml
+-rw-r--r--   0 jani      (1000) jani      (1000)     1079 2021-09-30 13:24:08.118065 hawkmoth-0.9.0/setup.cfg
+drwxr-xr-x   0 jani      (1000) jani      (1000)        0 2021-09-30 13:24:08.118065 hawkmoth-0.9.0/test/
+-rwxr-xr-x   0 jani      (1000) jani      (1000)     2617 2021-09-26 15:38:43.000000 hawkmoth-0.9.0/test/test_cautodoc.py
+-rw-r--r--   0 jani      (1000) jani      (1000)     2444 2021-09-26 15:38:43.000000 hawkmoth-0.9.0/test/test_cli.py
+-rwxr-xr-x   0 jani      (1000) jani      (1000)     1640 2021-09-30 12:50:41.000000 hawkmoth-0.9.0/test/test_parser.py
+-rw-r--r--   0 jani      (1000) jani      (1000)     3190 2021-09-30 12:52:04.000000 hawkmoth-0.9.0/test/testenv.py
```

### Comparing `hawkmoth-0.8.0/LICENSE` & `hawkmoth-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hawkmoth-0.8.0/README.rst` & `hawkmoth-0.9.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+
+|badge-tag| |badge-license| |badge-rtd| |badge-pypi|
+
+.. |badge-tag| image:: https://img.shields.io/github/v/tag/jnikula/hawkmoth
+		       :target: https://github.com/jnikula/hawkmoth/blob/master/CHANGELOG.rst
+		       :alt: GitHub tag (latest SemVer)
+
+.. |badge-license| image:: https://img.shields.io/github/license/jnikula/hawkmoth
+			   :target: https://opensource.org/licenses/BSD-2-Clause
+			   :alt: BSD-2-Clause
+
+.. |badge-rtd| image:: https://img.shields.io/readthedocs/hawkmoth
+		       :target: https://hawkmoth.readthedocs.io/en/latest/
+		       :alt: Read the Docs
+
+.. |badge-pypi| image:: https://img.shields.io/pypi/dm/hawkmoth
+			:target: https://pypi.org/project/hawkmoth/
+			:alt: PyPI Downloads
+
 Hawkmoth - Sphinx Autodoc for C
 ===============================
 
 Hawkmoth is a minimalistic Sphinx_ `C Domain`_ autodoc directive extension to
 incorporate formatted C source code comments written in reStructuredText_ into
 Sphinx based documentation. It uses Clang Python Bindings for parsing, and
 generates C Domain directives for C API documentation, and more. In short,
@@ -61,32 +80,40 @@
 your distro's package manager; they are not available via PyPI. For further
 details, see the documentation.
 
 Alternatively, installation packages are available for:
 
 * `Arch Linux`_
 
+There are also Docker images `jnikula/hawkmoth`_ and
+`jnikula/hawkmoth-latexpdf`_ at Docker Hub.
+
 In Sphinx ``conf.py``, add ``hawkmoth`` to ``extensions``, and point
 ``cautodoc_root`` at the source tree. See the extension documentation for
 details.
 
 .. _PyPI: https://pypi.org/project/hawkmoth/
 
 .. _Arch Linux: https://aur.archlinux.org/packages/?K=hawkmoth
 
+.. _jnikula/hawkmoth-latexpdf: https://hub.docker.com/repository/docker/jnikula/hawkmoth-latexpdf
+
+.. _jnikula/hawkmoth: https://hub.docker.com/repository/docker/jnikula/hawkmoth
+
 Development and Contributing
 ----------------------------
 
 Hawkmoth source code is available on GitHub_. The development version can be
 checked out via ``git`` using this command::
 
   git clone https://github.com/jnikula/hawkmoth.git
 
 Please file bugs and feature requests as GitHub issues. Contributions are
-welcome both as emailed patches to the mailing list and as pull requests.
+welcome both as GitHub pull requests (preferred) and as emailed patches to the
+mailing list.
 
 .. _GitHub: https://github.com/jnikula/hawkmoth
 
 Dependencies
 ------------
 
 - Python 3.6
@@ -105,15 +132,15 @@
 Hawkmoth is free software, released under the `2-Clause BSD License`_.
 
 .. _2-Clause BSD License: https://opensource.org/licenses/BSD-2-Clause
 
 Contact
 -------
 
-IRC channel ``#hawkmoth`` on freenode_.
+IRC channel ``#hawkmoth`` on `OFTC IRC network`_.
 
 Mailing list hawkmoth@freelists.org. Subscription information at the `list home
 page`_.
 
-.. _freenode: https://freenode.net/
+.. _OFTC IRC network: https://www.oftc.net/
 
 .. _list home page: https://www.freelists.org/list/hawkmoth
```

### Comparing `hawkmoth-0.8.0/hawkmoth/__main__.py` & `hawkmoth-0.9.0/hawkmoth/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,22 +30,23 @@
                         help='Argument to pass to Clang. May be specified multiple times. See cautodoc_clang.')
     parser.add_argument('--verbose', dest='verbose', action='store_true',
                         help='Verbose output.')
     args = parser.parse_args()
 
     transform = lambda comment: doccompat.convert(comment, transform=args.compat)
 
-    docs, errors = parse(args.file, transform=transform, clang=args.clang)
+    comments, errors = parse(args.file, clang_args=args.clang)
 
-    for (doc, meta) in docs:
+    for comment in comments.walk():
         if args.verbose:
-            print(f'# {meta}')
-        print(doc)
+            print(f'# {comment.get_meta()}')
+        print(comment.get_docstring(transform=transform))
 
     for (severity, filename, lineno, msg) in errors:
         if filename:
-            print('f{severity.name}: {filename}:{lineno}: {msg}',
+            print(f'{severity.name}: {filename}:{lineno}: {msg}',
                   file=sys.stderr)
         else:
             print(f'{severity.name}: {msg}', file=sys.stderr)
 
-main()
+if __name__ == '__main__':
+    main()
```

### Comparing `hawkmoth-0.8.0/hawkmoth/parser.py` & `hawkmoth-0.9.0/hawkmoth/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,59 @@
 # Copyright (c) 2016-2017 Jani Nikula <jani@nikula.org>
 # Copyright (c) 2018-2020 Bruno Santos <brunomanuelsantos@tecnico.ulisboa.pt>
 # Licensed under the terms of BSD 2-Clause, see LICENSE for details.
 """
 Documentation comment extractor
 ===============================
 
-This module extracts relevant documentation comments, optionally reformatting
-them in reST syntax.
+This module extracts relevant documentation comments.
 
 This is the part that uses Clang Python Bindings to extract documentation
 comments from C source code. This module does not depend on Sphinx.
 
 There are two passes:
 
 #. Pass over the tokens to find all the comments, including ones that aren't
    attached to cursors.
 
 #. Pass over the cursors to document them.
 
 There is minimal syntax parsing or input conversion:
 
-* Identification of documentation comment blocks, and stripping the comment
-  delimiters (``/**`` and ``*/``) and continuation line prefixes (e.g. ``␣*␣``).
+* Identification of documentation comment blocks, i.e. comments that start
+  with ``/**``.
 
 * Identification of function-like macros.
 
-* Indentation for reST C Domain directive blocks.
+* Identification of array and function pointer variables, members and
+  arguments, and conversion to a format suitable for Sphinx C Domain.
 
-* An optional external filter may be invoked to support different syntaxes.
-  These filters are expected to translate the comment into the reST format.
-
-Otherwise, documentation comments are passed through verbatim.
+The documentation comments are returned verbatim in a tree of Docstring objects.
 """
 
 import enum
 import re
 import sys
 
-from clang.cindex import CursorKind, TypeKind
+from clang.cindex import TokenKind, CursorKind, TypeKind
 from clang.cindex import Index, TranslationUnit
-from clang.cindex import SourceLocation, SourceRange
-from clang.cindex import TokenKind, TokenGroup
 
-from hawkmoth.util import docstr, doccompat, strutil
+from hawkmoth.docstring import *
 
 class ErrorLevel(enum.Enum):
     """
     Supported error levels in inverse numerical order of severity. The values
     are chosen so that they map directly to a 'verbosity level'.
     """
     ERROR = 0
     WARNING = 1
     INFO = 2
     DEBUG = 3
 
-def comment_extract(tu):
+def _comment_extract(tu):
 
     # FIXME: How to handle top level comments above a cursor that it does *not*
     # describe? Parsing @file or @doc at this stage would not be a clean design.
     # One idea is to use '/***' to denote them, but that might throw off editor
     # highlighting. The workaround is to follow the top level comment with an
     # empty '/**/' comment that gets attached to the cursor.
 
@@ -66,15 +61,15 @@
     comments = {}
     cursor = None
     current_comment = None
     for token in tu.get_tokens(extent=tu.cursor.extent):
         # handle all comments we come across
         if token.kind == TokenKind.COMMENT:
             # if we already have a comment, it wasn't related to a cursor
-            if current_comment and docstr.is_doc(current_comment.spelling):
+            if current_comment and Docstring.is_doc(current_comment.spelling):
                 top_level_comments.append(current_comment)
             current_comment = token
             continue
 
         # Store off the token's cursor for a slight performance improvement
         # instead of accessing the `cursor` property multiple times.
         token_cursor = token.cursor
@@ -89,43 +84,32 @@
 
         if cursor is not None and token_cursor == cursor:
             continue
 
         cursor = token_cursor
 
         # Note: current_comment may be None
-        if current_comment != None and docstr.is_doc(current_comment.spelling):
+        if current_comment != None and Docstring.is_doc(current_comment.spelling):
             comments[cursor.hash] = current_comment
         current_comment = None
 
     # comment at the end of file
-    if current_comment and docstr.is_doc(current_comment.spelling):
+    if current_comment and Docstring.is_doc(current_comment.spelling):
         top_level_comments.append(current_comment)
 
     return top_level_comments, comments
 
-def _result(comment, cursor=None, fmt=docstr.Type.TEXT, nest=0,
-            name=None, ttype=None, args=None, transform=None):
-
-    # FIXME: docstr.generate changes the number of lines in output. This impacts
-    # the error reporting via meta['line']. Adjust meta to take this into
-    # account.
-
-    doc = docstr.generate(text=comment.spelling, fmt=fmt,
-                          name=name, ttype=ttype, args=args, transform=transform)
-
-    doc = docstr.nest(doc, nest)
-
+def _get_meta(comment, cursor=None):
     meta = {'line': comment.extent.start.line}
     if cursor:
-        meta['cursor.kind']        = cursor.kind,
-        meta['cursor.displayname'] = cursor.displayname,
-        meta['cursor.spelling']    = cursor.spelling
+        meta['cursor.kind'] = cursor.kind
+        meta['cursor.displayname'] = cursor.displayname
+        meta['cursor.spelling'] = cursor.spelling
 
-    return [(doc, meta)]
+    return meta
 
 # Return None for simple macros, a potentially empty list of arguments for
 # function-like macros
 def _get_macro_args(cursor):
     if cursor.kind != CursorKind.MACRO_DEFINITION:
         return None
 
@@ -150,22 +134,26 @@
         elif token.spelling == '...':
             args.append(token.spelling)
         else:
             break
 
     return None
 
+# If this is an array, the dimensions should be applied to the name, not
+# the type.
 def _array_fixup(ttype, name):
     dims = ttype.rsplit(' ', 1)[-1]
     if dims.startswith('[') and dims.endswith(']'):
         ttype = ttype.rsplit(' ', 1)[0]
         name = name + dims
 
     return ttype, name
 
+# If this is a function pointer, or an array of function pointers, the
+# name should be within the parenthesis as in (*name) or (*name[N]).
 def _function_pointer_fixup(ttype, name):
     mo = re.match(r'(?P<begin>.+)\((?P<stars>\*+)(?P<qual>[a-zA-Z_ ]+)?(?P<brackets>\[[^]]*\])?\)(?P<end>.+)', ttype)
     if mo is None:
         return ttype, name
 
     begin = mo.group('begin')
     stars = mo.group('stars')
@@ -174,50 +162,56 @@
     end = mo.group('end')
 
     name = f'{begin}({stars}{qual}{name}{brackets}){end}'
     ttype = ''
 
     return ttype, name
 
-def _recursive_parse(comments, cursor, nest, transform):
+def _decl_fixup(ttype, name):
+    ttype, name = _array_fixup(ttype, name)
+
+    ttype, name = _function_pointer_fixup(ttype, name)
+
+    return ttype, name
+
+def _recursive_parse(comments, cursor, nest):
     comment = comments[cursor.hash]
     name = cursor.spelling
     ttype = cursor.type.spelling
+    text = comment.spelling
+    meta = _get_meta(comment, cursor)
 
     if cursor.kind == CursorKind.MACRO_DEFINITION:
         # FIXME: check args against comment
         args = _get_macro_args(cursor)
-        fmt = docstr.Type.MACRO if args is None else docstr.Type.MACRO_FUNC
 
-        return _result(comment, cursor=cursor, fmt=fmt,
-                       nest=nest, name=name, args=args, transform=transform)
+        if args is None:
+            ds = MacroDocstring(text=text, nest=nest, name=name, meta=meta)
+        else:
+            ds = MacroFunctionDocstring(text=text, nest=nest, name=name, args=args, meta=meta)
+
+        return [ds]
 
     elif cursor.kind in [CursorKind.VAR_DECL, CursorKind.FIELD_DECL]:
+        # Note: Preserve original name
+        ttype, decl_name = _decl_fixup(ttype, name)
+
         if cursor.kind == CursorKind.VAR_DECL:
-            fmt = docstr.Type.VAR
+            ds = VarDocstring(text=text, nest=nest, name=name, decl_name=decl_name, ttype=ttype, meta=meta)
         else:
-            fmt = docstr.Type.MEMBER
+            ds = MemberDocstring(text=text, nest=nest, name=name, decl_name=decl_name, ttype=ttype, meta=meta)
 
-        # If this is an array, the dimensions should be applied to the name, not
-        # the type.
-        ttype, name = _array_fixup(ttype, name)
-
-        # If this is a function pointer, or an array of function pointers, the
-        # name should be within the parenthesis as in (*name) or (*name[N]).
-        ttype, name = _function_pointer_fixup(ttype, name)
-
-        return _result(comment, cursor=cursor, fmt=fmt,
-                       nest=nest, name=name, ttype=ttype, transform=transform)
+        return [ds]
 
     elif cursor.kind == CursorKind.TYPEDEF_DECL:
         # FIXME: function pointers typedefs.
-        fmt = docstr.Type.TYPE
 
-        return _result(comment, cursor=cursor, fmt=fmt,
-                       nest=nest, name=ttype, transform=transform)
+        ds = TypeDocstring(text=text, nest=nest, name=ttype, meta=meta)
+
+        return [ds]
 
     elif cursor.kind in [CursorKind.STRUCT_DECL, CursorKind.UNION_DECL,
                          CursorKind.ENUM_DECL]:
 
         # FIXME:
         # Handle cases where variables are instantiated on type declaration,
         # including anonymous cases. Idea is that if there is a variable
@@ -225,116 +219,104 @@
         # the structure is anonymous or to the type otherwise.
         #
         # Due to the new recursiveness of the parser, fixing this here, _should_
         # handle all cases (struct, union, enum).
 
         # FIXME: Handle anonymous enumerators.
 
-        fmts = {CursorKind.STRUCT_DECL: docstr.Type.STRUCT,
-                CursorKind.UNION_DECL: docstr.Type.UNION,
-                CursorKind.ENUM_DECL: docstr.Type.ENUM}
-
-        fmt = fmts[cursor.kind]
-
         # name may be empty for typedefs
-        result = _result(comment, cursor=cursor, fmt=fmt,
-                         nest=nest, name=name if name else ttype, transform=transform)
+        name = name if name else ttype
+
+        if cursor.kind == CursorKind.STRUCT_DECL:
+            ds = StructDocstring(text=text, nest=nest, name=name, meta=meta)
+        elif cursor.kind == CursorKind.UNION_DECL:
+            ds = UnionDocstring(text=text, nest=nest, name=name, meta=meta)
+        else:
+            ds = EnumDocstring(text=text, nest=nest, name=name, meta=meta)
 
-        nest += 1
         for c in cursor.get_children():
             if c.hash in comments:
-                result.extend(_recursive_parse(comments, c, nest, transform))
+                ds.add_children(_recursive_parse(comments, c, nest + 1))
 
-        return result
+        return [ds]
 
     elif cursor.kind == CursorKind.ENUM_CONSTANT_DECL:
-        fmt = docstr.Type.ENUM_VAL
+        ds = EnumeratorDocstring(text=text, nest=nest, name=name, meta=meta)
 
-        return _result(comment, cursor=cursor, fmt=fmt,
-                       nest=nest, name=name, transform=transform)
+        return [ds]
 
     elif cursor.kind == CursorKind.FUNCTION_DECL:
         # FIXME: check args against comment
         # FIXME: children may contain extra stuff if the return type is a
         # typedef, for example
         args = []
 
         # Only fully prototyped functions will have argument lists to process.
         if cursor.type.kind == TypeKind.FUNCTIONPROTO:
             for c in cursor.get_children():
                 if c.kind == CursorKind.PARM_DECL:
-                    arg_ttype, arg_name = _array_fixup(c.type.spelling, c.spelling)
-                    arg_ttype, arg_name = _function_pointer_fixup(arg_ttype, arg_name)
+                    arg_ttype, arg_name = _decl_fixup(c.type.spelling, c.spelling)
 
                     args.append(f'{arg_ttype} {arg_name}')
 
             if cursor.type.is_function_variadic():
                 args.append('...')
 
-        fmt = docstr.Type.FUNC
         ttype = cursor.result_type.spelling
 
-        return _result(comment, cursor=cursor, fmt=fmt, nest=nest,
-                       name=name, ttype=ttype, args=args, transform=transform)
+        ds = FunctionDocstring(text=text, nest=nest, name=name, ttype=ttype, args=args,
+                               meta=meta)
+        return [ds]
 
     # FIXME: If we reach here, nothing matched. This is a warning or even error
     # and it should be logged, but it should also return an empty list so that
     # it doesn't break. I.e. the parser needs to pass warnings and errors to the
     # Sphinx extension instead of polluting the generated output.
-    fmt = docstr.Type.TEXT
     kind = str(cursor.kind)
     text = f'warning: unhandled cursor {kind} {cursor.spelling}\n'
+    meta = _get_meta(comment, cursor)
 
-    doc = docstr.generate(text=text, fmt=fmt)
+    ds = TextDocstring(text=text, meta=meta)
 
-    meta = {
-        'line':               comment.extent.start.line,
-        'cursor.kind':        cursor.kind,
-        'cursor.displayname': cursor.displayname,
-        'cursor.spelling':    cursor.spelling
-    }
+    return [ds]
 
-    return [(doc, meta)]
-
-def clang_diagnostics(errors, diagnostics):
+def _clang_diagnostics(diagnostics):
+    errors = []
     sev = {0: ErrorLevel.DEBUG,
            1: ErrorLevel.DEBUG,
            2: ErrorLevel.WARNING,
            3: ErrorLevel.ERROR,
            4: ErrorLevel.ERROR}
 
     for diag in diagnostics:
         filename = diag.location.file.name if diag.location.file else None
         errors.extend([(sev[diag.severity], filename,
                         diag.location.line, diag.spelling)])
 
-# return a list of (comment, metadata) tuples
-# options - dictionary with directive options
-def parse(filename, **options):
-
-    errors = []
-    args = strutil.args_as_list(options.get('clang'))
+    return errors
 
+# Parse a file and return a tree of Docstring objects.
+def parse(filename, clang_args=None):
     index = Index.create()
 
-    tu = index.parse(filename, args=args, options=
+    tu = index.parse(filename, args=clang_args, options=
                      TranslationUnit.PARSE_DETAILED_PROCESSING_RECORD |
                      TranslationUnit.PARSE_SKIP_FUNCTION_BODIES)
 
-    clang_diagnostics(errors, tu.diagnostics)
+    errors = _clang_diagnostics(tu.diagnostics)
 
-    top_level_comments, comments = comment_extract(tu)
+    top_level_comments, comments = _comment_extract(tu)
 
-    result = []
-    transform = options.get('transform')
+    # Empty comment with just children
+    result = Docstring()
 
     for comment in top_level_comments:
-        result.extend(_result(comment, transform=transform))
+        text = comment.spelling
+        meta = _get_meta(comment)
+        ds = TextDocstring(text=text, meta=meta)
+        result.add_child(ds)
 
     for cursor in tu.cursor.get_children():
         if cursor.hash in comments:
-            result.extend(_recursive_parse(comments, cursor, 0, transform))
-
-    # Sort all elements by order of appearance.
-    result.sort(key=lambda r: r[1]['line'])
+            result.add_children(_recursive_parse(comments, cursor, 0))
 
     return result, errors
```

### Comparing `hawkmoth-0.8.0/hawkmoth/util/compiler.py` & `hawkmoth-0.9.0/hawkmoth/util/compiler.py`

 * *Files identical despite different names*

### Comparing `hawkmoth-0.8.0/hawkmoth/util/doccompat.py` & `hawkmoth-0.9.0/hawkmoth/util/doccompat.py`

 * *Files identical despite different names*

### Comparing `hawkmoth-0.8.0/hawkmoth/util/readthedocs.py` & `hawkmoth-0.9.0/hawkmoth/util/readthedocs.py`

 * *Files identical despite different names*

### Comparing `hawkmoth-0.8.0/setup.cfg` & `hawkmoth-0.9.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 	hawkmoth
 	hawkmoth.util
 
 [options.extras_require]
 dev = 
 	pytest
 	sphinx-testing
+	strictyaml
 
 [options.package_data]
 hawkmoth = 
 	VERSION
 
 [egg_info]
 tag_build =
```

### Comparing `hawkmoth-0.8.0/test/test_hawkmoth.py` & `hawkmoth-0.9.0/test/test_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,29 +10,38 @@
 from hawkmoth.util import doccompat
 from test import conf, testenv
 
 def _get_output(input_filename, **options):
     docs_str = ''
     errors_str = ''
 
-    transform = options.pop('compat', None)
-    if transform is not None:
-        options['transform'] = lambda comment: doccompat.convert(comment, transform=transform)
+    directive = options.get('directive')
+    if directive:
+        pytest.skip(f'{directive} directive test')
+
+    options = options.get('directive-options', {})
+
+    clang_args = options.get('clang')
+    comments, errors = parse(input_filename, clang_args=clang_args)
+
+    tropt = options.pop('compat', None)
+    if tropt is not None:
+        transform = lambda comment: doccompat.convert(comment, transform=tropt)
     else:
-        transform = options.pop('transform', None)
-        if transform is not None:
-            options['transform'] = conf.cautodoc_transformations[transform]
+        tropt = options.pop('transform', None)
+        if tropt is not None:
+            transform = conf.cautodoc_transformations[tropt]
+        else:
+            transform = None
 
-    docs, errors = parse(input_filename, **options)
-
-    for (doc, meta) in docs:
-        docs_str += doc + '\n'
+    for comment in comments.walk():
+        docs_str += comment.get_docstring(transform=transform) + '\n'
 
     for (severity, filename, lineno, msg) in errors:
-        errors_str += f'{severity.name}: {lineno}: {msg}\n'
+        errors_str += f'{severity.name}: {os.path.basename(filename)}:{lineno}: {msg}\n'
 
     return docs_str, errors_str
 
 def _get_expected(input_filename, **options):
     return testenv.read_file(input_filename, ext='rst'), \
         testenv.read_file(input_filename, ext='stderr')
```

