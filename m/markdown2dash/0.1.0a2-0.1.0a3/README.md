# Comparing `tmp/markdown2dash-0.1.0a2.tar.gz` & `tmp/markdown2dash-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown2dash-0.1.0a2.tar", max compression
+gzip compressed data, was "markdown2dash-0.1.0a3.tar", max compression
```

## Comparing `markdown2dash-0.1.0a2.tar` & `markdown2dash-0.1.0a3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-08-09 17:04:50.363457 markdown2dash-0.1.0a2/LICENSE
--rw-r--r--   0        0        0     6794 2023-08-12 04:36:44.578122 markdown2dash-0.1.0a2/README.md
--rw-r--r--   0        0        0       51 2023-08-09 15:36:00.121838 markdown2dash-0.1.0a2/markdown2dash/__init__.py
--rw-r--r--   0        0        0      303 2023-08-09 15:37:50.871333 markdown2dash-0.1.0a2/markdown2dash/src/decorators.py
--rw-r--r--   0        0        0      992 2023-08-09 15:37:18.306584 markdown2dash-0.1.0a2/markdown2dash/src/directives/admonition.py
--rw-r--r--   0        0        0     1328 2023-08-11 14:56:48.852264 markdown2dash-0.1.0a2/markdown2dash/src/directives/exec.py
--rw-r--r--   0        0        0      574 2023-08-09 15:37:30.831355 markdown2dash-0.1.0a2/markdown2dash/src/directives/image.py
--rw-r--r--   0        0        0     1138 2023-08-09 15:37:33.285761 markdown2dash-0.1.0a2/markdown2dash/src/directives/kwargs.py
--rw-r--r--   0        0        0     1875 2023-08-11 14:10:16.951219 markdown2dash-0.1.0a2/markdown2dash/src/directives/toc.py
--rw-r--r--   0        0        0     1034 2023-08-12 04:35:33.701149 markdown2dash-0.1.0a2/markdown2dash/src/parser.py
--rw-r--r--   0        0        0     3138 2023-08-09 15:38:05.931584 markdown2dash-0.1.0a2/markdown2dash/src/renderer.py
--rw-r--r--   0        0        0      147 2023-08-09 12:46:54.785400 markdown2dash-0.1.0a2/markdown2dash/src/utils.py
--rw-r--r--   0        0        0     1735 2023-08-12 04:33:24.177177 markdown2dash-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     7932 2023-08-12 04:43:15.869509 markdown2dash-0.1.0a2/setup.py
--rw-r--r--   0        0        0     8596 2023-08-12 04:43:15.870096 markdown2dash-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-09 17:04:50.363457 markdown2dash-0.1.0a3/LICENSE
+-rw-r--r--   0        0        0     5850 2023-08-16 14:21:51.549569 markdown2dash-0.1.0a3/README.md
+-rw-r--r--   0        0        0      434 2023-08-18 02:24:44.861413 markdown2dash-0.1.0a3/markdown2dash/__init__.py
+-rw-r--r--   0        0        0      367 2023-08-16 10:00:21.280058 markdown2dash-0.1.0a3/markdown2dash/src/decorators.py
+-rw-r--r--   0        0        0      410 2023-08-16 10:01:43.165098 markdown2dash-0.1.0a3/markdown2dash/src/directives/admonition.py
+-rw-r--r--   0        0        0     1101 2023-08-16 10:00:42.384225 markdown2dash-0.1.0a3/markdown2dash/src/directives/base.py
+-rw-r--r--   0        0        0      834 2023-08-16 10:01:53.791751 markdown2dash-0.1.0a3/markdown2dash/src/directives/exec.py
+-rw-r--r--   0        0        0      304 2023-08-16 10:01:57.695655 markdown2dash-0.1.0a3/markdown2dash/src/directives/image.py
+-rw-r--r--   0        0        0     1444 2023-08-16 10:31:38.867216 markdown2dash-0.1.0a3/markdown2dash/src/directives/kwargs.py
+-rw-r--r--   0        0        0     1880 2023-08-17 18:09:34.062119 markdown2dash-0.1.0a3/markdown2dash/src/directives/toc.py
+-rw-r--r--   0        0        0      808 2023-08-16 06:35:05.068396 markdown2dash-0.1.0a3/markdown2dash/src/parser.py
+-rw-r--r--   0        0        0     3197 2023-08-18 02:24:37.705572 markdown2dash-0.1.0a3/markdown2dash/src/renderer.py
+-rw-r--r--   0        0        0      729 2023-08-16 09:53:13.580520 markdown2dash-0.1.0a3/markdown2dash/src/utils.py
+-rw-r--r--   0        0        0     1735 2023-09-10 11:52:53.669136 markdown2dash-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0     6949 2023-09-10 11:55:53.383152 markdown2dash-0.1.0a3/setup.py
+-rw-r--r--   0        0        0     7652 2023-09-10 11:55:53.383736 markdown2dash-0.1.0a3/PKG-INFO
```

### Comparing `markdown2dash-0.1.0a2/LICENSE` & `markdown2dash-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown2dash-0.1.0a2/README.md` & `markdown2dash-0.1.0a3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,237 +1,34 @@
-## Markdown-2-Dash
+# -*- coding: utf-8 -*-
+from setuptools import setup
 
-.. toc::
-    :min_level: 3
+packages = \
+['markdown2dash', 'markdown2dash.src', 'markdown2dash.src.directives']
 
-Markdown-2-Dash or m2d is a standalone package forked out of the [official documentation for dash-mantine-components](https://www.dash-mantine-components.com).
-Some form of m2d has existed since the inception of the documentation, but I figured more people can make use of this to document their dash
-apps or component libraries.
-
-Have a look [here](https://github.com/snehilvj/markdown2dash/tree/main/preview) to see how this README would look after parsing with m2d.
-
-### Installation
-
-```bash
-pip install markdown2dash
-```
-
-```bash
-poetry add markdown2dash
-```
-
-### Quickstart
-
-Just parse the contents of your markdown file with m2d parser, and voilà! You have a layout ready.
-
-```python
-import dash_mantine_components as dmc
-from dash import Dash, html
-
-from markdown2dash import parse
-
-with open("../README.md") as f:
-    md = f.read()
-
-
-def render_toc(self, toc):
-    paddings = {3: 0, 5: 40}
-    links = [
-        html.A(
-            dmc.Text(text, color="dimmed", size="sm"),
-            href="#" + hid,
-            style={
-                "textTransform": "capitalize",
-                "textDecoration": "none",
-                "paddingLeft": paddings[level],
-            },
-        )
-        for level, text, hid in toc
-    ]
-    heading = dmc.Text("Table of Contents", mb=10, weight=500) if links else None
-    return dmc.Stack([heading, *links], spacing=4, mt=20, mb=30)
-
-
-layout = parse(md, toc_renderer=render_toc)
-
-app = Dash(__name__)
-
-app.layout = dmc.MantineProvider(
-    dmc.Container(layout, size="lg", p=20),
-    withGlobalStyles=True,
-    withNormalizeCSS=True,
-    theme={
-        "primaryColor": "indigo",
-        "colorScheme": "light",
-        "fontFamily": "'Inter', sans-serif",
-        "components": {
-            "Table": {"defaultProps": {"striped": True, "withBorder": True}},
-            "Alert": {"styles": {"title": {"fontWeight": 500}}},
-        },
-    },
-)
-
-if __name__ == "__main__":
-    app.run(debug=True)
-```
-
-There's now styling by default, so you'll have to provide your own css. You can do that in two ways:
-1. Wrap your layout in a MantineProvider and use it to style your page
-2. Create CSS files. You can get started with the one provided in this repository: [styles.css]()
-
-##### Example App
-
-You can also just run the example app included in this project locally.
-
-```bash
-python example/app.py
-``` 
-
-### Available tokens and class names
-
-m2d can render following types of tokens:
-
-| Token               | Class Name          |
-|---------------------|---------------------|
-| Links               | .m2d-link           |
-| Paragraph           | .m2d-paragraph      |
-| Emphasis            | .m2d-emphasis       |
-| Strong              | .m2d-strong         |
-| Code Span           | .m2d-code span      |
-| Heading             | .m2d-heading        |
-| Thematic Break      | .m2d-thematic-break |
-| Block Code          | .m2d-block-code     |
-| Block Quote         | .m2d-block-quote    |
-| List Item           | .m2d-list-item      |
-| List                | .m2d-list           |
-| Strikethrough       | .m2d-strikethrough  |
-| Mark                | .m2d-mark           |
-| Table               | .m2d-table          |
-| Table Head          | .m2d-table-head     |
-| Table Body          | .m2d-table-body     |
-| Table Row           | .m2d-table-row      |
-| Table Cell          | .m2d-table-cell     |
-| Admonition          | .m2d-admonition     |
-| Image               | .m2d-image          |
-| Executable Block    | .m2d-block-exec     |
-| Dash Component Docs | .m2d-kwargs         |
-| Table of Contents   | << user defined >>  |
-
-### Special Directives
-
-m2d includes some special directives enabling you to do a lot more than just rendering static markdown into a dash layout. 
-
-##### Executable Block
-
-You can use the `exec` directive to embed the output of a python script as well as its source code. This directive expects that 
-you have stored the output layout in the variable called `component`.
-
-```markdown
-.. exec::example.component
-```
-
-Here's the output if you are viewing this in a dash app:
-
-.. exec::example.component
-
-You can hide the source code using the `code` argument, and the border using `border`.
-
-```markdown
-.. exec::markdown2dash.example.component
-    :code: false
-    :border: false
-```
-
-##### Admonition
-
-You can use `admonition` directive to add dmc.Alert components in your page.
-Admonition directive uses [DashIconify]() to render icons as well.
-
-```markdown
-.. admonition::Alert Title
-    :icon: radix-icons:github-logo
-    
-    This is to show that now you can render alerts directly from the markdown.
-```
-
-Here's the output if you are viewing this in a dash app:
-
-.. admonition::Alert Title
-    :icon: radix-icons:github-logo
-
-    This is to show that now you can render alerts directly from the markdown.
-
-##### Image
-
-Render images using dmc.Image like this:
-
-```markdown
-.. image::https://www.dash-mantine-components.com/assets/superman.jpeg
-    :width: 300px
-    :height: 300px
-```
-
-Here's the output if you are viewing this in a dash app:
-
-.. image::https://www.dash-mantine-components.com/assets/superman.jpeg
-    :width: 300px
-    :height: 300px
-
-##### Dash Component API Docs
-
-It's very simple to add API docs of your component using m2d. You just have to specify the package and the component.
-Let's create one for DashIconify:
-
-```markdown
-.. kwargs::DashIconify
-    :library: dash_iconify
-```
-
-Here's the output if you are viewing this in a dash app:
-
-.. kwargs::DashIconify
-    :library: dash_iconify
- 
-##### Table of Contents
-
-In order to get a table of contents using m2d, you need to pass a renderer functions that accepts a placeholder `self` and the actual inputs in the following way:
-
-```python
-
-# a placeholder for self and a list of [<level>, <title>, <id>]
-[
-    (4, 'Installation', 'installation'),
-    (4, 'Quickstart', 'quickstart'), 
-    (5, 'Example App', 'example-app'),
-    (4, 'Special Directives', 'special-directives'),
-    (5, 'Dash Component API Docs', 'dash-component-api-docs'),
-    (5, 'Table of Contents', 'table-of-contents')
-]
-```
-
-Here's the renderer function used on this page:
-
-```python
-def render_toc(self, toc):
-    paddings = {4: 0, 5: 40}
-    links = [
-        html.A(
-            dmc.Text(text, color="dimmed", size="sm"),
-            href="#" + hid,
-            style={
-                "textTransform": "capitalize",
-                "textDecoration": "none",
-                "paddingLeft": paddings[level],
-            },
-        )
-        for level, text, hid in toc
-    ]
-    heading = dmc.Text("Table of Contents", mb=10, weight=500) if links else None
-    return dmc.Stack([heading, *links], spacing=4, mt=20, mb=30)
-```
-
-And then you can enable TOC lke this:
-
-```markdown
-.. toc::
-    :min_level: 3
-```
+package_data = \
+{'': ['*']}
+
+install_requires = \
+['dash-iconify>=0.1.2,<0.2.0',
+ 'dash-mantine-components==0.13.0a3',
+ 'dash>=2.11.1,<3.0.0',
+ 'jsonpath>=0.82,<0.83',
+ 'mistune>=3.0.1,<4.0.0']
+
+setup_kwargs = {
+    'name': 'markdown2dash',
+    'version': '0.1.0a3',
+    'description': 'Render markdown into a dash layout using dash-mantine-components',
+    'long_description': '## Markdown-2-Dash\n\n.. toc::\n    :min_level: 3\n\nMarkdown-2-Dash or m2d is a standalone package forked out of the [official documentation for dash-mantine-components](https://www.dash-mantine-components.com).\nSome form of m2d has always existed since the inception of the documentation, but I figured more people can make use of this to document their dash\napps or component libraries.\n\nHave a look [here](https://github.com/snehilvj/markdown2dash/tree/main/preview) to see how this README would look after parsing with m2d.\n\n### Installation\n\n```bash\npip install markdown2dash\n```\n\n```bash\npoetry add markdown2dash\n```\n\n### Quickstart\n\nJust parse the contents of your markdown file with m2d parser, and voilà! You have a layout ready.\n\n```python\nimport dash_mantine_components as dmc\nfrom dash import Dash\n\nfrom markdown2dash import parse\n\nwith open("../README.md") as f:\n    md = f.read()\n\nlayout = parse(md)\n\napp = Dash(__name__)\n\napp.layout = dmc.MantineProvider(\n    dmc.Container(layout, size="lg", p=20),\n    withGlobalStyles=True,\n    withNormalizeCSS=True,\n    theme={\n        "primaryColor": "indigo",\n        "colorScheme": "light",\n        "fontFamily": "\'Inter\', sans-serif",\n        "components": {\n            "Table": {"defaultProps": {"striped": True, "withBorder": True}},\n            "Alert": {"styles": {"title": {"fontWeight": 500}}},\n        },\n    },\n)\n\nif __name__ == "__main__":\n    app.run(debug=True)\n```\n\nThere\'s no styling by default, so you\'ll have to provide your own css. You can do that in two ways:\n1. Wrap your layout in a MantineProvider and use it to style your page (as you can see above)\n2. Create CSS files. You can get started with the one provided in this repository: [styles.css]()\n\n##### Example App\n\nYou can also just run the example app included in this project locally.\n\n```bash\npython example/app.py\n``` \n\n### Available tokens and class names\n\nm2d can render following types of tokens:\n\n| Token               | Class Name            |\n|---------------------|-----------------------|\n| Links               | .m2d-link             |\n| Paragraph           | .m2d-paragraph        |\n| Emphasis            | .m2d-emphasis         |\n| Strong              | .m2d-strong           |\n| Code Span           | .m2d-code span        |\n| Heading             | .m2d-heading          |\n| Thematic Break      | .m2d-thematic-break   |\n| Block Code          | .m2d-block-code       |\n| Block Quote         | .m2d-block-quote      |\n| List Item           | .m2d-list-item        |\n| List                | .m2d-list             |\n| Strikethrough       | .m2d-strikethrough    |\n| Mark                | .m2d-mark             |\n| Table               | .m2d-table            |\n| Table Head          | .m2d-table-head       |\n| Table Body          | .m2d-table-body       |\n| Table Row           | .m2d-table-row        |\n| Table Cell          | .m2d-table-cell       |\n| Admonition          | .m2d-block-admonition |\n| Image               | .m2d-block-image      |\n| Executable Block    | .m2d-block-exec       |\n| Dash Component Docs | .m2d-block-kwargs     |\n| Table of Contents   | .m2d-block-toc        |\n\n### Special Directives\n\nm2d includes some special directives enabling you to do a lot more than just rendering static markdown into a dash layout.\n\nThe directives are all extensible, and you can just overwrite the render method to suit your own needs. The default render method is provided in all directives out of the box.\n\n##### Executable Block\n\nYou can use the `exec` directive to embed the output of a python script as well as its source code. This directive expects that \nyou have stored the output layout in the variable called `component`.\n\n```markdown\n.. exec::example.component\n```\n\nHere\'s the output if you are viewing this in a dash app:\n\n.. exec::example.component\n\nYou can hide the source code using the `code` argument, and the border using `border`.\n\n```markdown\n.. exec::markdown2dash.example.component\n    :code: false\n    :border: false\n```\n\n##### Admonition\n\nYou can use `admonition` directive to add dmc.Alert components in your page.\nAdmonition directive uses [DashIconify]() to render icons as well.\n\n```markdown\n.. admonition::Alert Title\n    :icon: radix-icons:github-logo\n    \n    This is to show that now you can render alerts directly from the markdown.\n```\n\nHere\'s the output if you are viewing this in a dash app:\n\n.. admonition::Alert Title\n    :icon: radix-icons:github-logo\n\n    This is to show that now you can render alerts directly from the markdown.\n\n##### Image\n\nRender images using dmc.Image like this:\n\n```markdown\n.. image::https://www.dash-mantine-components.com/assets/superman.jpeg\n    :width: 300px\n    :height: 300px\n```\n\nHere\'s the output if you are viewing this in a dash app:\n\n.. image::https://www.dash-mantine-components.com/assets/superman.jpeg\n    :width: 300px\n    :height: 300px\n\n##### Dash Component API Docs\n\nIt\'s very simple to add API docs of your component using m2d. You just have to specify the package and the component.\nLet\'s create one for DashIconify:\n\n```markdown\n.. kwargs::DashIconify\n    :library: dash_iconify\n```\n\nHere\'s the output if you are viewing this in a dash app:\n\n.. kwargs::DashIconify\n    :library: dash_iconify\n \n##### Table of Contents\n\nThis directive will parse all the headings and create a table of contents like this:\n\n```python\n\n# a placeholder for self and a list of [<level>, <title>, <id>]\n[\n    (4, \'Installation\', \'installation\'),\n    (4, \'Quickstart\', \'quickstart\'), \n    (5, \'Example App\', \'example-app\'),\n    (4, \'Special Directives\', \'special-directives\'),\n    (5, \'Dash Component API Docs\', \'dash-component-api-docs\'),\n    (5, \'Table of Contents\', \'table-of-contents\')\n]\n```\n\nThis will then be used to render the TOC using the render method. You can enable TOC lke this:\n\n```markdown\n.. toc::\n    :min_level: 3\n```\n',
+    'author': 'Snehil Vijay',
+    'author_email': 'snehilvj@outlook.com',
+    'maintainer': None,
+    'maintainer_email': None,
+    'url': 'https://github.com/snehilvj/markdown2dash',
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'python_requires': '>=3.7',
+}
+
+
+setup(**setup_kwargs)
```

### Comparing `markdown2dash-0.1.0a2/markdown2dash/src/directives/admonition.py` & `markdown2dash-0.1.0a3/markdown2dash/src/directives/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,34 @@
-import dash_mantine_components as dmc
 from dash.development.base_component import Component
-from dash_iconify import DashIconify
 from mistune.directives import DirectivePlugin
 
 from ..decorators import class_name
 
 
-@class_name
-def admonition(self, title, content, icon=None) -> Component:
-    kwargs = {"icon": DashIconify(icon=icon, width=23)} if icon else {}
-    return dmc.Alert(content, title=title, **kwargs)
+class BaseDirective(DirectivePlugin):
+    NAME = "base"
 
-
-class Admonition(DirectivePlugin):
-    NAME = "admonition"
+    def __init__(self):
+        super().__init__()
+        self.block_name = "block_" + self.NAME
+
+    def render(self, renderer, title: str, content: str, **options) -> Component:
+        raise NotImplementedError
+
+    # noinspection PyMethodMayBeStatic
+    def hook(self, md, state):
+        pass
 
     def parse(self, block, m, state):
         options = dict(self.parse_options(m))
         title = self.parse_title(m)
         content = self.parse_content(m)
         attrs = {"title": title, "content": content, **options}
-        return {"type": "block_admonition", "attrs": attrs}
+        return {"type": self.block_name, "attrs": attrs}
 
     # noinspection PyMethodOverriding
     def __call__(self, directive, md):
+        renderer = class_name(self.render)
         directive.register(self.NAME, self.parse)
         if md.renderer.NAME == "dash":
-            md.renderer.register("block_admonition", admonition)
+            md.renderer.register(self.block_name, renderer)
+            md.before_render_hooks.append(self.hook)
```

### Comparing `markdown2dash-0.1.0a2/markdown2dash/src/parser.py` & `markdown2dash-0.1.0a3/markdown2dash/src/parser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,27 @@
+from typing import List, Optional
+
 import mistune
-from mistune.directives import RSTDirective
-from typing import Callable, Optional
+from mistune.directives import RSTDirective, DirectivePlugin
 
 from .directives.admonition import Admonition
 from .directives.exec import BlockExec
 from .directives.image import Image
 from .directives.kwargs import Kwargs
 from .directives.toc import TableOfContents
 from .renderer import DashRenderer
 
-
-def default_toc_renderer(self, toc):
-    raise NotImplementedError
+DEFAULT_DIRECTIVES = [Admonition(), Image(), BlockExec(), Kwargs(), TableOfContents()]
 
 
-def parse(
-    content: str,
-    toc_renderer: Callable = default_toc_renderer,
-    toc_kwargs: Optional[dict] = None,
-):
-    toc_kwargs = toc_kwargs or {}
+def parse(content: str, directives: Optional[List[DirectivePlugin]] = None):
+    directives = directives or DEFAULT_DIRECTIVES
     parser = mistune.create_markdown(
         renderer=DashRenderer(),
         plugins=[
             "strikethrough",
             "mark",
             "table",
-            RSTDirective(
-                [
-                    Admonition(),
-                    Image(),
-                    BlockExec(),
-                    Kwargs(),
-                    TableOfContents(toc_renderer, **toc_kwargs),
-                ]
-            ),
+            RSTDirective(directives),
         ],
     )
     return parser(content)
```

### Comparing `markdown2dash-0.1.0a2/markdown2dash/src/renderer.py` & `markdown2dash-0.1.0a3/markdown2dash/src/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,8 +109,9 @@
     def table_cell(self, text: str, align=None, head=False):
         return html.Th(text) if head else html.Td(text)
 
     def blank_line(self) -> None:
         return
 
     def render_tokens(self, tokens, state):
-        return list(self.iter_tokens(tokens, state))
+        components = list(self.iter_tokens(tokens, state))
+        return [comp for comp in components if comp]
```

### Comparing `markdown2dash-0.1.0a2/pyproject.toml` & `markdown2dash-0.1.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "markdown2dash"
-version = "0.1.0a2"
+version = "0.1.0a3"
 description = "Render markdown into a dash layout using dash-mantine-components"
 authors = ["Snehil Vijay <snehilvj@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/snehilvj/markdown2dash"
 repository = "https://github.com/snehilvj/markdown2dash"
 documentation = "https://github.com/snehilvj/markdown2dash"
@@ -31,15 +31,15 @@
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Widget Sets",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 dash = "^2.11.1"
-dash-mantine-components = "0.13.0a2"
+dash-mantine-components = "0.13.0a3"
 mistune = "^3.0.1"
 jsonpath = "^0.82"
 dash-iconify = "^0.1.2"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
 twine = "^4.0.2"
```

### Comparing `markdown2dash-0.1.0a2/PKG-INFO` & `markdown2dash-0.1.0a3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown2dash
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: Render markdown into a dash layout using dash-mantine-components
 Home-page: https://github.com/snehilvj/markdown2dash
 License: MIT
 Keywords: dash,plotly,documentation,markdown,dash-mantine-components,dmc
 Author: Snehil Vijay
 Author-email: snehilvj@outlook.com
 Requires-Python: >=3.7
@@ -27,28 +27,28 @@
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Dist: dash (>=2.11.1,<3.0.0)
 Requires-Dist: dash-iconify (>=0.1.2,<0.2.0)
-Requires-Dist: dash-mantine-components (==0.13.0a2)
+Requires-Dist: dash-mantine-components (==0.13.0a3)
 Requires-Dist: jsonpath (>=0.82,<0.83)
 Requires-Dist: mistune (>=3.0.1,<4.0.0)
 Project-URL: Documentation, https://github.com/snehilvj/markdown2dash
 Project-URL: Repository, https://github.com/snehilvj/markdown2dash
 Description-Content-Type: text/markdown
 
 ## Markdown-2-Dash
 
 .. toc::
     :min_level: 3
 
 Markdown-2-Dash or m2d is a standalone package forked out of the [official documentation for dash-mantine-components](https://www.dash-mantine-components.com).
-Some form of m2d has existed since the inception of the documentation, but I figured more people can make use of this to document their dash
+Some form of m2d has always existed since the inception of the documentation, but I figured more people can make use of this to document their dash
 apps or component libraries.
 
 Have a look [here](https://github.com/snehilvj/markdown2dash/tree/main/preview) to see how this README would look after parsing with m2d.
 
 ### Installation
 
 ```bash
@@ -61,41 +61,22 @@
 
 ### Quickstart
 
 Just parse the contents of your markdown file with m2d parser, and voilà! You have a layout ready.
 
 ```python
 import dash_mantine_components as dmc
-from dash import Dash, html
+from dash import Dash
 
 from markdown2dash import parse
 
 with open("../README.md") as f:
     md = f.read()
 
-
-def render_toc(self, toc):
-    paddings = {3: 0, 5: 40}
-    links = [
-        html.A(
-            dmc.Text(text, color="dimmed", size="sm"),
-            href="#" + hid,
-            style={
-                "textTransform": "capitalize",
-                "textDecoration": "none",
-                "paddingLeft": paddings[level],
-            },
-        )
-        for level, text, hid in toc
-    ]
-    heading = dmc.Text("Table of Contents", mb=10, weight=500) if links else None
-    return dmc.Stack([heading, *links], spacing=4, mt=20, mb=30)
-
-
-layout = parse(md, toc_renderer=render_toc)
+layout = parse(md)
 
 app = Dash(__name__)
 
 app.layout = dmc.MantineProvider(
     dmc.Container(layout, size="lg", p=20),
     withGlobalStyles=True,
     withNormalizeCSS=True,
@@ -110,59 +91,61 @@
     },
 )
 
 if __name__ == "__main__":
     app.run(debug=True)
 ```
 
-There's now styling by default, so you'll have to provide your own css. You can do that in two ways:
-1. Wrap your layout in a MantineProvider and use it to style your page
+There's no styling by default, so you'll have to provide your own css. You can do that in two ways:
+1. Wrap your layout in a MantineProvider and use it to style your page (as you can see above)
 2. Create CSS files. You can get started with the one provided in this repository: [styles.css]()
 
 ##### Example App
 
 You can also just run the example app included in this project locally.
 
 ```bash
 python example/app.py
 ``` 
 
 ### Available tokens and class names
 
 m2d can render following types of tokens:
 
-| Token               | Class Name          |
-|---------------------|---------------------|
-| Links               | .m2d-link           |
-| Paragraph           | .m2d-paragraph      |
-| Emphasis            | .m2d-emphasis       |
-| Strong              | .m2d-strong         |
-| Code Span           | .m2d-code span      |
-| Heading             | .m2d-heading        |
-| Thematic Break      | .m2d-thematic-break |
-| Block Code          | .m2d-block-code     |
-| Block Quote         | .m2d-block-quote    |
-| List Item           | .m2d-list-item      |
-| List                | .m2d-list           |
-| Strikethrough       | .m2d-strikethrough  |
-| Mark                | .m2d-mark           |
-| Table               | .m2d-table          |
-| Table Head          | .m2d-table-head     |
-| Table Body          | .m2d-table-body     |
-| Table Row           | .m2d-table-row      |
-| Table Cell          | .m2d-table-cell     |
-| Admonition          | .m2d-admonition     |
-| Image               | .m2d-image          |
-| Executable Block    | .m2d-block-exec     |
-| Dash Component Docs | .m2d-kwargs         |
-| Table of Contents   | << user defined >>  |
+| Token               | Class Name            |
+|---------------------|-----------------------|
+| Links               | .m2d-link             |
+| Paragraph           | .m2d-paragraph        |
+| Emphasis            | .m2d-emphasis         |
+| Strong              | .m2d-strong           |
+| Code Span           | .m2d-code span        |
+| Heading             | .m2d-heading          |
+| Thematic Break      | .m2d-thematic-break   |
+| Block Code          | .m2d-block-code       |
+| Block Quote         | .m2d-block-quote      |
+| List Item           | .m2d-list-item        |
+| List                | .m2d-list             |
+| Strikethrough       | .m2d-strikethrough    |
+| Mark                | .m2d-mark             |
+| Table               | .m2d-table            |
+| Table Head          | .m2d-table-head       |
+| Table Body          | .m2d-table-body       |
+| Table Row           | .m2d-table-row        |
+| Table Cell          | .m2d-table-cell       |
+| Admonition          | .m2d-block-admonition |
+| Image               | .m2d-block-image      |
+| Executable Block    | .m2d-block-exec       |
+| Dash Component Docs | .m2d-block-kwargs     |
+| Table of Contents   | .m2d-block-toc        |
 
 ### Special Directives
 
-m2d includes some special directives enabling you to do a lot more than just rendering static markdown into a dash layout. 
+m2d includes some special directives enabling you to do a lot more than just rendering static markdown into a dash layout.
+
+The directives are all extensible, and you can just overwrite the render method to suit your own needs. The default render method is provided in all directives out of the box.
 
 ##### Executable Block
 
 You can use the `exec` directive to embed the output of a python script as well as its source code. This directive expects that 
 you have stored the output layout in the variable called `component`.
 
 ```markdown
@@ -229,50 +212,29 @@
 Here's the output if you are viewing this in a dash app:
 
 .. kwargs::DashIconify
     :library: dash_iconify
  
 ##### Table of Contents
 
-In order to get a table of contents using m2d, you need to pass a renderer functions that accepts a placeholder `self` and the actual inputs in the following way:
+This directive will parse all the headings and create a table of contents like this:
 
 ```python
 
 # a placeholder for self and a list of [<level>, <title>, <id>]
 [
     (4, 'Installation', 'installation'),
     (4, 'Quickstart', 'quickstart'), 
     (5, 'Example App', 'example-app'),
     (4, 'Special Directives', 'special-directives'),
     (5, 'Dash Component API Docs', 'dash-component-api-docs'),
     (5, 'Table of Contents', 'table-of-contents')
 ]
 ```
 
-Here's the renderer function used on this page:
-
-```python
-def render_toc(self, toc):
-    paddings = {4: 0, 5: 40}
-    links = [
-        html.A(
-            dmc.Text(text, color="dimmed", size="sm"),
-            href="#" + hid,
-            style={
-                "textTransform": "capitalize",
-                "textDecoration": "none",
-                "paddingLeft": paddings[level],
-            },
-        )
-        for level, text, hid in toc
-    ]
-    heading = dmc.Text("Table of Contents", mb=10, weight=500) if links else None
-    return dmc.Stack([heading, *links], spacing=4, mt=20, mb=30)
-```
-
-And then you can enable TOC lke this:
+This will then be used to render the TOC using the render method. You can enable TOC lke this:
 
 ```markdown
 .. toc::
     :min_level: 3
 ```
```

