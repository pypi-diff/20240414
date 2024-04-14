# Comparing `tmp/pybts-1.6.0.tar.gz` & `tmp/pybts-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybts-1.6.0.tar", max compression
+gzip compressed data, was "pybts-1.6.1.tar", max compression
```

## Comparing `pybts-1.6.0.tar` & `pybts-1.6.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0   157658 2024-04-12 21:31:23.883104 pybts-1.6.0/README.assets/DEMO_Sequence  10-10 _ 100.png
--rw-r--r--   0        0        0   189323 2024-04-12 21:31:23.883104 pybts-1.6.0/README.assets/image-20240329031220580.png
--rw-r--r--   0        0        0   208202 2024-04-12 21:31:23.887104 pybts-1.6.0/README.assets/image-20240329031233459.png
--rw-r--r--   0        0        0   255608 2024-04-12 21:31:23.887104 pybts-1.6.0/README.assets/image-20240401211552611.png
--rw-r--r--   0        0        0   202283 2024-04-12 21:31:23.887104 pybts-1.6.0/README.assets/image-20240401211609525.png
--rw-r--r--   0        0        0     5960 2024-04-12 21:31:23.887104 pybts-1.6.0/README.md
--rw-r--r--   0        0        0      385 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/__init__.py
--rw-r--r--   0        0        0       52 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/board/__init__.py
--rw-r--r--   0        0        0     2258 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/board/board.py
--rw-r--r--   0        0        0     9994 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/board/server.py
--rw-r--r--   0        0        0     8003 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/builder.py
--rw-r--r--   0        0        0      596 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/composites/__init__.py
--rw-r--r--   0        0        0     9344 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/composites/composite.py
--rw-r--r--   0        0        0     2175 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/composites/condition_branch.py
--rw-r--r--   0        0        0     5460 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/composites/parallel.py
--rw-r--r--   0        0        0      945 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/composites/ppa.py
--rw-r--r--   0        0        0     2235 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/composites/selector.py
--rw-r--r--   0        0        0     2460 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/composites/sequence.py
--rw-r--r--   0        0        0     1510 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/composites/switcher.py
--rw-r--r--   0        0        0      182 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/composites/template.py
--rw-r--r--   0        0        0     3243 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/constants.py
--rw-r--r--   0        0        0     4548 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/converter.py
--rw-r--r--   0        0        0      121 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/decorators/__init__.py
--rw-r--r--   0        0        0    22175 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/decorators/nodes.py
--rw-r--r--   0        0        0     1073 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/display.py
--rw-r--r--   0        0        0     1521 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/main.py
--rw-r--r--   0        0        0    14150 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/nodes.py
--rw-r--r--   0        0        0       63 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/rl/__init__.py
--rw-r--r--   0        0        0     8862 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/rl/base_class.py
--rw-r--r--   0        0        0      268 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/rl/builder.py
--rw-r--r--   0        0        0      460 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/rl/common.py
--rw-r--r--   0        0        0    15448 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/rl/nodes.py
--rw-r--r--   0        0        0     5688 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/rl/off_policy.py
--rw-r--r--   0        0        0     7196 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/rl/on_policy.py
--rw-r--r--   0        0        0     1184 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/rl/tree.py
--rw-r--r--   0        0        0    16958 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/templates/favicon.ico
--rw-r--r--   0        0        0      433 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/templates/index.html
--rw-r--r--   0        0        0  1967920 2024-04-12 21:31:23.903104 pybts-1.6.0/pybts/templates/static/index-BlldS3Jx.js
--rw-r--r--   0        0        0   320362 2024-04-12 21:31:23.903104 pybts-1.6.0/pybts/templates/static/index-DN1S--qx.css
--rw-r--r--   0        0        0     5267 2024-04-12 21:31:23.903104 pybts-1.6.0/pybts/templates/static/info-lb9hZOuB.png
--rw-r--r--   0        0        0     2140 2024-04-12 21:31:23.903104 pybts-1.6.0/pybts/tree.py
--rw-r--r--   0        0        0    10045 2024-04-12 21:31:23.903104 pybts-1.6.0/pybts/utility.py
--rw-r--r--   0        0        0      844 2024-04-12 21:31:23.903104 pybts-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 pybts-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0   157658 2024-04-14 09:59:09.406932 pybts-1.6.1/README.assets/DEMO_Sequence  10-10 _ 100.png
+-rw-r--r--   0        0        0   189323 2024-04-14 09:59:09.410932 pybts-1.6.1/README.assets/image-20240329031220580.png
+-rw-r--r--   0        0        0   208202 2024-04-14 09:59:09.410932 pybts-1.6.1/README.assets/image-20240329031233459.png
+-rw-r--r--   0        0        0   255608 2024-04-14 09:59:09.410932 pybts-1.6.1/README.assets/image-20240401211552611.png
+-rw-r--r--   0        0        0   202283 2024-04-14 09:59:09.410932 pybts-1.6.1/README.assets/image-20240401211609525.png
+-rw-r--r--   0        0        0     5960 2024-04-14 09:59:09.410932 pybts-1.6.1/README.md
+-rw-r--r--   0        0        0      385 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/board/__init__.py
+-rw-r--r--   0        0        0     2258 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/board/board.py
+-rw-r--r--   0        0        0    11048 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/board/server.py
+-rw-r--r--   0        0        0     8197 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/builder.py
+-rw-r--r--   0        0        0      596 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/composites/__init__.py
+-rw-r--r--   0        0        0     9344 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/composites/composite.py
+-rw-r--r--   0        0        0     2175 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/composites/condition_branch.py
+-rw-r--r--   0        0        0     5460 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/composites/parallel.py
+-rw-r--r--   0        0        0      945 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/composites/ppa.py
+-rw-r--r--   0        0        0     2235 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/composites/selector.py
+-rw-r--r--   0        0        0     2460 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/composites/sequence.py
+-rw-r--r--   0        0        0     1510 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/composites/switcher.py
+-rw-r--r--   0        0        0      182 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/composites/template.py
+-rw-r--r--   0        0        0     3243 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/constants.py
+-rw-r--r--   0        0        0     4943 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/converter.py
+-rw-r--r--   0        0        0      121 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/decorators/__init__.py
+-rw-r--r--   0        0        0    22898 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/decorators/nodes.py
+-rw-r--r--   0        0        0     1073 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/display.py
+-rw-r--r--   0        0        0     1521 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/main.py
+-rw-r--r--   0        0        0    17521 2024-04-14 09:59:09.414932 pybts-1.6.1/pybts/nodes.py
+-rw-r--r--   0        0        0       63 2024-04-14 09:59:09.418932 pybts-1.6.1/pybts/rl/__init__.py
+-rw-r--r--   0        0        0     8856 2024-04-14 09:59:09.418932 pybts-1.6.1/pybts/rl/base_class.py
+-rw-r--r--   0        0        0      268 2024-04-14 09:59:09.418932 pybts-1.6.1/pybts/rl/builder.py
+-rw-r--r--   0        0        0      460 2024-04-14 09:59:09.418932 pybts-1.6.1/pybts/rl/common.py
+-rw-r--r--   0        0        0    15167 2024-04-14 09:59:09.418932 pybts-1.6.1/pybts/rl/nodes.py
+-rw-r--r--   0        0        0     5688 2024-04-14 09:59:09.418932 pybts-1.6.1/pybts/rl/off_policy.py
+-rw-r--r--   0        0        0     8537 2024-04-14 09:59:09.418932 pybts-1.6.1/pybts/rl/on_policy.py
+-rw-r--r--   0        0        0     1172 2024-04-14 09:59:09.418932 pybts-1.6.1/pybts/rl/tree.py
+-rw-r--r--   0        0        0    16958 2024-04-14 09:59:09.418932 pybts-1.6.1/pybts/templates/favicon.ico
+-rw-r--r--   0        0        0      433 2024-04-14 09:59:09.418932 pybts-1.6.1/pybts/templates/index.html
+-rw-r--r--   0        0        0  1967920 2024-04-14 09:59:09.426931 pybts-1.6.1/pybts/templates/static/index-BlldS3Jx.js
+-rw-r--r--   0        0        0   320362 2024-04-14 09:59:09.430931 pybts-1.6.1/pybts/templates/static/index-DN1S--qx.css
+-rw-r--r--   0        0        0     5267 2024-04-14 09:59:09.430931 pybts-1.6.1/pybts/templates/static/info-lb9hZOuB.png
+-rw-r--r--   0        0        0     2140 2024-04-14 09:59:09.430931 pybts-1.6.1/pybts/tree.py
+-rw-r--r--   0        0        0    10045 2024-04-14 09:59:09.430931 pybts-1.6.1/pybts/utility.py
+-rw-r--r--   0        0        0      844 2024-04-14 09:59:09.430931 pybts-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 pybts-1.6.1/PKG-INFO
```

### Comparing `pybts-1.6.0/README.assets/DEMO_Sequence  10-10 _ 100.png` & `pybts-1.6.1/README.assets/DEMO_Sequence  10-10 _ 100.png`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/README.assets/image-20240329031220580.png` & `pybts-1.6.1/README.assets/image-20240329031220580.png`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/README.assets/image-20240329031233459.png` & `pybts-1.6.1/README.assets/image-20240329031233459.png`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/README.assets/image-20240401211552611.png` & `pybts-1.6.1/README.assets/image-20240401211552611.png`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/README.assets/image-20240401211609525.png` & `pybts-1.6.1/README.assets/image-20240401211609525.png`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/README.md` & `pybts-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/board/board.py` & `pybts-1.6.1/pybts/board/board.py`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/board/server.py` & `pybts-1.6.1/pybts/board/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                         "icon" : "",
                     },
                     "myTool2"    : {
                         "show" : True,
                         "title": "下载XML",
                         "icon" : "",
                     },
-                    "myTool3": {
+                    "myTool3"    : {
                         "show" : True,
                         "title": "展示信息",
                         "icon" : "",
                     },
                     "saveAsImage": {
                         "show": True
                     },
@@ -149,40 +149,60 @@
                 if os.path.exists(os.path.join(TEMPLATES_DIR, target_path)):
                     return send_from_directory(TEMPLATES_DIR, target_path)
         return send_from_directory(TEMPLATES_DIR, 'index.html')
 
     def send_static(self, path):
         return send_from_directory(STATIC_DIR, path)
 
-    def get_projects(self):
+    def get_projects(self, dirpath: str):
         # 获取log_dir里面的所有的文件夹
-        projects = []
-        if not os.path.exists(self.log_dir):
+        if not os.path.exists(dirpath):
             return []
 
-        for dirpath, dirnames, filenames in os.walk(self.log_dir):
-            if 'pybts.json' in filenames:
-                relative_path = os.path.relpath(dirpath, self.log_dir)
-                pybts_data = self._get_pybts_data(project=relative_path)
-                if pybts_data is None:
-                    continue
-
-                projects.append({
-                    'name'  : relative_path,
-                    'unread': pybts_data.get('id') - self.last_read_id,
-                    'total' : pybts_data['id'],
-                    'modified_time': os.path.getmtime(os.path.join(dirpath, 'pybts.json'))
-                })
+        projects = []
+        if os.path.isdir(dirpath):
+            for filename in os.listdir(dirpath):
+                if filename == 'pybts.json':
+                    relative_path = os.path.relpath(dirpath, self.log_dir)
+                    pybts_data = self._get_pybts_data(project=relative_path)
+                    if pybts_data is None:
+                        continue
+                    projects.append({
+                        'name'         : relative_path,
+                        'unread'       : pybts_data.get('id') - self.last_read_id,
+                        'total'        : pybts_data['id'],
+                        'modified_time': os.path.getmtime(os.path.join(dirpath, 'pybts.json'))
+                    })
+                    return projects
+
+            for filename in os.listdir(dirpath):
+                sub_dirpath = os.path.join(dirpath, filename)
+                if os.path.isdir(sub_dirpath):
+                    projects.extend(self.get_projects(sub_dirpath))
+
+        # for dirpath, dirnames, filenames in os.walk(self.log_dir):
+        #     if 'pybts.json' in filenames:
+        #         relative_path = os.path.relpath(dirpath, self.log_dir)
+        #         pybts_data = self._get_pybts_data(project=relative_path)
+        #         if pybts_data is None:
+        #             continue
+        #
+        #         projects.append({
+        #             'name'         : relative_path,
+        #             'unread'       : pybts_data.get('id') - self.last_read_id,
+        #             'total'        : pybts_data['id'],
+        #             'modified_time': os.path.getmtime(os.path.join(dirpath, 'pybts.json'))
+        #         })
 
         # 按照modified_time排序
         sorted_projects = sorted(projects, key=lambda project: project['modified_time'])
         return sorted_projects
 
     def get_config(self):
-        projects = self.get_projects()
+        projects = self.get_projects(self.log_dir)
         return jsonify({
             'title'          : self.title,
             'update_interval': self.update_interval,
             'projects'       : projects,
         })
 
     def get_option(self):
```

### Comparing `pybts-1.6.0/pybts/builder.py` & `pybts-1.6.1/pybts/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -171,15 +171,21 @@
                 Success,
                 Running,
                 IsChanged,
                 IsMatchRule,
                 IsEqual,
                 Print,
                 RandomIntValue,
-                RandomFloatValue
+                RandomFloatValue,
+                RandomSuccess,
+                SetValueToContext,
+                SetIntToContext,
+                SetFloatToContext,
+                TimeElapsed,
+                PrintNodeData
         )
 
         self.register_node(
                 Inverter,
                 RunningUntilCondition,
                 OneShot,
                 Count,
```

### Comparing `pybts-1.6.0/pybts/composites/__init__.py` & `pybts-1.6.1/pybts/composites/__init__.py`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/composites/composite.py` & `pybts-1.6.1/pybts/composites/composite.py`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/composites/condition_branch.py` & `pybts-1.6.1/pybts/composites/condition_branch.py`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/composites/parallel.py` & `pybts-1.6.1/pybts/composites/parallel.py`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/composites/ppa.py` & `pybts-1.6.1/pybts/composites/ppa.py`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/composites/selector.py` & `pybts-1.6.1/pybts/composites/selector.py`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/composites/sequence.py` & `pybts-1.6.1/pybts/composites/sequence.py`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/composites/switcher.py` & `pybts-1.6.1/pybts/composites/switcher.py`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/constants.py` & `pybts-1.6.1/pybts/constants.py`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/converter.py` & `pybts-1.6.1/pybts/converter.py`

 * *Files 19% similar despite different names*

```diff
@@ -85,25 +85,37 @@
         elif isinstance(value, list):
             return [cls.status(value=item) for item in value]
         elif isinstance(value, str):
             value_list = value.split(',')
             return [cls.status(value=item) for item in value_list if item != '']
 
     def render(self, value: str, context: dict = None) -> str:
+        if '{{' not in value or '}}' not in value:
+            return value
+
         ctx = { }
         # if self.node.attrs is not None:
         #     ctx.update(self.node.attrs)
         if self.node.context is not None:
             ctx.update(self.node.context)
         if context is not None:
             ctx.update(context)
         for key in ctx:
             if callable(ctx[key]):
                 ctx[key] = ctx[key]()
-        return jinja2.Template(value).render(ctx)
+
+        for i in range(3):
+            # 最多嵌套3层
+            rendered_value = jinja2.Template(value).render(ctx)
+            if '{{' not in rendered_value or '}}' not in rendered_value:
+                return rendered_value
+            if rendered_value == value:
+                return rendered_value
+            value = rendered_value
+        return value
 
     def list(self, value: typing.Any) -> typing.List[typing.Any]:
         if isinstance(value, str):
             return eval(self.render(value))
         elif isinstance(value, list):
             return value
         elif isinstance(value, tuple):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pybts-1.6.0/pybts/decorators/nodes.py` & `pybts-1.6.1/pybts/decorators/nodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -187,30 +187,35 @@
         Init with the decorated child.
 
         Args:
             child: behaviour to shoot
             name: the decorator name
             policy: policy determining when the oneshot should activate
             - SUCCESS
-            - SUCCESS|FAILURE
+            - SUCCESS,FAILURE
         """
         super(OneShot, self).__init__(**kwargs)
         self.final_status: typing.Optional[Status] = None
-        if isinstance(policy, str):
-            self.policy = list(map(lambda x: Status(x), policy.split('|')))
-        else:
-            self.policy = policy
+        self.policy = policy
 
     def to_data(self):
         return {
             **super().to_data(),
             'policy'      : self.policy,
             'final_status': self.final_status
         }
 
+    def setup(self, **kwargs: typing.Any) -> None:
+        super().setup(**kwargs)
+        self.policy = self.converter.status_list(self.policy)
+
+    def reset(self):
+        super().reset()
+        self.final_status = None
+
     def update(self) -> Status:
         """
         Bounce if the child has already successfully completed.
 
         Returns:
             the behaviour's new status :class:`~py_trees.Status`
         """
@@ -265,52 +270,54 @@
     If the timeout is reached, the encapsulated behaviour's
     :meth:`~py_trees.behaviour.Behaviour.stop` method is called with
     status :data:`~py_trees.common.Status.FAILURE` otherwise it will
     simply directly tick and return with the same status
     as that of it's encapsulated behaviour.
     """
 
-    def __init__(self, duration: float = 5.0, **kwargs):
+    def __init__(self, duration: float = 5.0, time: str | float = 'time', **kwargs):
         """
         Init with the decorated child and a timeout duration.
 
         Args:
             child: the child behaviour or subtree
             name: the decorator name
             duration: timeout length in seconds
+            time: 传time表示使用系统时间，{{time}}表示使用context里的时间
         """
         super(Timeout, self).__init__(**kwargs)
         self.duration = duration
         self.finish_time = 0.0
+        self.time = time
 
     def setup(self, **kwargs: typing.Any) -> None:
         super().setup(**kwargs)
         self.duration = self.converter.float(self.duration)
 
     def reset(self):
         super().reset()
         self.finish_time = 0
 
     def initialise(self) -> None:
         """Reset the feedback message and finish time on behaviour entry."""
-        self.finish_time = self.get_time() + self.duration
+        self.finish_time = self.get_time(self.time) + self.duration
         self.feedback_message = ""
 
     def update(self) -> Status:
         """
         Fail on timeout, or block / reflect the child's result accordingly.
 
         Terminate the child and return
         :data:`~py_trees.common.Status.FAILURE`
         if the timeout is exceeded.
 
         Returns:
             the behaviour's new status :class:`~py_trees.common.Status`
         """
-        current_time = self.get_time()
+        current_time = self.get_time(self.time)
         if (
                 self.decorated.status == Status.RUNNING
                 and current_time > self.finish_time
         ):
             self.feedback_message = "timed out"
             self.logger.debug(
                     "{}.update() {}".format(self.__class__.__name__, self.feedback_message)
@@ -551,42 +558,45 @@
 
 class Throttle(Decorator):
     """
     节流: 在一定时间间隔内只执行一次
     每隔一段时间才会触发一次子节点，其他时间直接返回之前的状态
     """
 
-    def __init__(self, duration: float | str = 5.0, **kwargs):
+    def __init__(self, duration: float | str = 5.0, time: str | float = 'time', **kwargs):
         """
         Init with the decorated child and a timeout duration.
 
         Args:
             child: the child behaviour or subtree
             name: the decorator name
             duration: timeout length in seconds
+            time: 当前时间，传time表示使用系统时间
         """
         super().__init__(**kwargs)
         self.duration = duration
         self.last_time = -float('inf')
+        self.time = time
+        self.curr_time = None
 
     def reset(self):
         super().reset()
         self.last_time = -float('inf')
 
     def setup(self, **kwargs: typing.Any) -> None:
         super().setup(**kwargs)
         self.duration = self.converter.float(self.duration)
 
     def update(self) -> Status:
         return self.decorated.status
 
     def tick(self):
-        now_time = self.get_time()
-        if now_time - self.last_time >= self.duration:
-            self.last_time = now_time
+        self.curr_time = self.get_time(self.time)
+        if self.curr_time - self.last_time >= self.duration:
+            self.last_time = self.curr_time
             yield from Decorator.tick(self)
         else:
             yield from Node.tick(self)
 
 
 class IsStatusChanged(Decorator):
     """
@@ -644,7 +654,21 @@
             self.last_status = self.decorated.status
         is_changed = self.check_is_changed()
         self.last_status = self.decorated.status
         if is_changed:
             return Status.SUCCESS
         else:
             return Status.FAILURE
+
+
+class PrintNodeData(Decorator):
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+    def update(self) -> Status:
+        print(self.decorated.to_data())
+        return Status.SUCCESS
+
+    def to_data(self):
+        return {
+            **super().to_data(),
+        }
```

### Comparing `pybts-1.6.0/pybts/display.py` & `pybts-1.6.1/pybts/display.py`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/main.py` & `pybts-1.6.1/pybts/main.py`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/nodes.py` & `pybts-1.6.1/pybts/nodes.py`

 * *Files 12% similar despite different names*

```diff
@@ -160,24 +160,20 @@
             return f'<{self.name} {attrs_str}/>'
         else:
             return f'<{self.name} {attrs_str}/>({len(self.children)})'
 
     def __repr__(self):
         return self.__str__()
 
-    def get_time(self) -> float:
+    def get_time(self, time: str | float) -> float:
         """获取行为树时间，时间可以由context传入，可以是一个函数"""
-        if self.context is not None and 'time' in self.context:
-            if callable(self.context['time']):
-                return self.context['time']()
-            # 在context传递了time的情况下使用context里的时间，方便使用游戏时间
-            return self.context['time']
-        else:
+        if time == 'time':
             import time
             return time.monotonic()
+        return self.converter.float(time)
 
 
 class Action(Node, ABC):
     """
     行为节点
     """
 
@@ -459,7 +455,127 @@
 
     def to_data(self):
         return {
             **super().to_data(),
             'key'  : self.key,
             'value': self.value
         }
+
+
+class RandomSuccess(Node, Condition):
+    """
+    以一定概率成功，其他情况是失败
+    """
+
+    def __init__(self, prob: float | str = 0.5, **kwargs):
+        super().__init__(**kwargs)
+        self.prob = prob
+        self.curr_prob = None
+
+    def to_data(self):
+        return {
+            **super().to_data(),
+            'curr_prob': self.curr_prob
+        }
+
+    def update(self) -> Status:
+        self.curr_prob = self.converter.float(self.prob)
+        assert 0 <= self.curr_prob <= 1, "Probability must be between 0 and 1"
+        if random.random() < self.curr_prob:
+            return Status.SUCCESS
+        return Status.FAILURE
+
+
+class SetValueToContext(Node):
+    def __init__(self, key: str, value: typing.Any, **kwargs):
+        super().__init__(**kwargs)
+        self.key = key
+        self.value = value
+        self.curr_value = None
+
+    def setup(self, **kwargs: typing.Any) -> None:
+        super().__init__(**kwargs)
+        self.key = self.converter.render(self.key)
+
+    def to_data(self):
+        return {
+            **super().to_data(),
+            'key'       : self.key,
+            'curr_value': self.curr_value
+        }
+
+    def compute_curr_value(self) -> typing.Any:
+        return self.converter.render(self.value)
+
+    def update(self) -> Status:
+        self.curr_value = self.compute_curr_value()
+        self.context[self.key] = self.curr_value
+        return Status.SUCCESS
+
+
+class SetIntToContext(SetValueToContext):
+    def compute_curr_value(self) -> typing.Any:
+        return self.converter.int(self.value)
+
+
+class SetFloatToContext(SetValueToContext):
+    def compute_curr_value(self) -> typing.Any:
+        return self.converter.float(self.value)
+
+
+class TimeElapsed(Node, Condition):
+    """
+    时间是否过去了
+    每隔一段时间才会触发一次子节点，其他时间直接返回之前的状态
+    """
+
+    def __init__(self, duration: float | str = 5.0, time: str | float = 'time', immediate: bool | str = False,
+                 **kwargs):
+        """
+        Init with the decorated child and a timeout duration.
+
+        Args:
+            child: the child behaviour or subtree
+            name: the decorator name
+            duration: timeout length in seconds
+            time: 当前时间，传time表示使用系统时间
+            immediate: 一开始是否就触发一次
+        """
+        super().__init__(**kwargs)
+        self.duration = duration
+        self.immediate = immediate
+        self.time = time
+
+        self.curr_duration = None
+        self.last_time = None
+        self.curr_time = None
+
+    def reset(self):
+        super().reset()
+        self.last_time = None
+        self.curr_time = None
+
+    def setup(self, **kwargs: typing.Any) -> None:
+        super().setup(**kwargs)
+        self.immediate = self.converter.bool(self.immediate)
+
+    def to_data(self):
+        return {
+            **super().to_data(),
+            'immediate'    : self.immediate,
+            'curr_time'    : self.curr_time,
+            'last_time'    : self.last_time,
+            'curr_duration': self.curr_duration,
+        }
+
+    def update(self) -> Status:
+        self.curr_time = self.get_time(self.time)
+        self.curr_duration = self.converter.float(self.duration)
+
+        if self.last_time is None:
+            self.last_time = self.curr_time
+            return Status.SUCCESS if self.immediate else Status.FAILURE
+
+        if self.curr_time - self.last_time >= self.curr_duration:
+            self.last_time = self.curr_time
+            return Status.SUCCESS
+        return Status.FAILURE
```

### Comparing `pybts-1.6.0/pybts/rl/base_class.py` & `pybts-1.6.1/pybts/rl/base_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,19 +68,19 @@
 
     @abstractmethod
     def rl_gen_reward(self) -> float:
         reward_scope = self.rl_reward_scope()
         if reward_scope != '':
             assert isinstance(self, Node), 'RLOnPolicyNode 必须得继承Node节点'
             assert self.context is not None, 'context必须得设置好'
-            assert 'rl_reward' in self.context, 'context必须得含有rl_reward键'
+            assert 'reward' in self.context, 'context必须得含有rl_reward键'
             scopes = reward_scope.split(',')
             curr_reward = 0
             for scope in scopes:
-                curr_reward += self.context['rl_reward'].get(scope, 0)
+                curr_reward += self.context['reward'].get(scope, 0)
             return curr_reward - self.rl_accum_reward
         raise NotImplemented
 
     @abstractmethod
     def rl_gen_done(self) -> bool:
         # 返回当前环境是否结束
         raise NotImplemented
```

### Comparing `pybts-1.6.0/pybts/rl/nodes.py` & `pybts-1.6.1/pybts/rl/nodes.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,35 +25,36 @@
     奖励会累积，所以PPO节点在消费奖励时要记录一下上次拿到的奖励值，然后将两次差值作为最终奖励
     """
 
     def __init__(self, reward: str | float, scope: str = 'default', **kwargs):
         super().__init__(**kwargs)
         self.reward = reward
         self.scope = scope
+        self.curr_reward = 0
 
     def setup(self, **kwargs: typing.Any) -> None:
         super().setup(**kwargs)
-        self.reward = self.converter.float(self.reward)
         self.scope = self.converter.render(self.scope).split(',')  # 域，只会将奖励保存在对应的scope中
 
     def update(self) -> Status:
         assert self.context is not None, 'context is not set'
+        self.curr_reward = self.converter.float(self.reward)
         if self.context is not None:
-            if 'rl_reward' not in self.context:
-                self.context['rl_reward'] = defaultdict(float)
+            if 'reward' not in self.context:
+                self.context['reward'] = defaultdict(float)
             for sc in self.scope:
-                self.context['rl_reward'][sc] += self.reward
+                self.context['reward'][sc] += self.curr_reward
         return Status.SUCCESS
 
     def to_data(self):
         return {
-            **super().to_data(),
-            'reward'   : self.reward,
-            'scope'    : self.scope,
-            'rl_reward': self.context['rl_reward'] if self.context is not None else None
+            # **super().to_data(),
+            'curr_reward'   : self.curr_reward,
+            'scope'         : self.scope,
+            'context_reward': dict(self.context['reward'])
         }
 
 
 class ConditionReward(Decorator):
     """
     强化学习奖励装饰节点
     根据子节点的状态来提供奖励
@@ -118,15 +119,15 @@
         elif new_status == Status.FAILURE:
             new_reward = self.failure
         self.reward = new_reward
         self.accum_reward += new_reward
 
         if self.context is not None:
             for sc in self.scope:
-                self.context['rl_reward'][sc] += self.reward
+                self.context['reward'][sc] += self.reward
 
         return new_status
 
 
 class RLBaseNode(ABC):
     """强化学习基础节点，拿来跟其他的Node多继承用"""
 
@@ -188,19 +189,19 @@
 
     @abstractmethod
     def rl_gen_reward(self) -> float:
         reward_scope = self.rl_reward_scope()
         if reward_scope != '':
             assert isinstance(self, Node), 'RLOnPolicyNode 必须得继承Node节点'
             assert self.context is not None, 'context必须得设置好'
-            assert 'rl_reward' in self.context, 'context必须得含有rl_reward键'
+            assert 'reward' in self.context, 'context必须得含有rl_reward键'
             scopes = reward_scope.split(',')
             curr_reward = 0
             for scope in scopes:
-                curr_reward += self.context['rl_reward'].get(scope, 0)
+                curr_reward += self.context['reward'].get(scope, 0)
             return curr_reward - self.rl_accum_reward
         raise NotImplemented
 
     @abstractmethod
     def rl_gen_done(self) -> bool:
         # 返回当前环境是否结束
         raise NotImplemented
@@ -211,37 +212,34 @@
     def rl_policy(self) -> Union[str, typing.Type[ActorCriticPolicy]]:
         return 'MlpPolicy'
 
     def rl_take_action(
             self,
             train: bool,
             log_interval: int = 1,
-            save_interval: int = 5,
-            save_path: str = ''
+            deterministic: bool = False,
     ):
         if isinstance(self.rl_model, OnPolicyAlgorithm):
             return self._rl_on_policy_take_action(
                     train=train,
                     log_interval=log_interval,
-                    save_interval=save_interval,
-                    save_path=save_path)
+                    deterministic=deterministic
+            )
         else:
             return self._rl_off_policy_take_action(
                     train=train,
                     log_interval=log_interval,
-                    save_interval=save_interval,
-                    save_path=save_path
+                    deterministic=deterministic
             )
 
     def _rl_off_policy_take_action(
             self,
             train: bool,
             log_interval: int = 1,
-            save_interval: int = 5,
-            save_path: str = ''
+            deterministic: bool = False,
     ):
         assert self.rl_model is not None, 'RL model not initialized'
         assert isinstance(self.rl_model, OffPolicyAlgorithm), 'RL model must be initialized with OffPolicyAlgorithm'
         model: OffPolicyAlgorithm = self.rl_model
         info = self.rl_gen_info()
         reward = self.rl_gen_reward()
         obs = self.rl_gen_obs()
@@ -284,44 +282,40 @@
                     )
                     action = self.rl_collector.send(None)
             except StopIteration:
                 self.rl_collector = None
                 self.rl_iteration += 1
                 # Display training infos
 
-                if self.rl_iteration % save_interval == 0:
-                    model.save(save_path)
-
                 self.rl_collector = bt_off_policy_collect_rollouts(
                         model,
                         train_freq=model.train_freq,
                         action_noise=model.action_noise,
                         learning_starts=model.learning_starts,
                         replay_buffer=model.replay_buffer,
                         log_interval=log_interval,
                 )
                 action = self.rl_collector.send(None)
         else:
             # 预测模式
-            action, state = model.predict(obs)
+            action, state = model.predict(obs, deterministic=deterministic)
 
         self.rl_obs = obs
         self.rl_reward = reward
         self.rl_info = info
         self.rl_accum_reward += reward
         self.rl_action = action
         self.rl_done = done
         return action
 
     def _rl_on_policy_take_action(
             self,
             train: bool,
             log_interval: int = 1,
-            save_interval: int = 5,
-            save_path: str = ''
+            deterministic: bool = False,
     ):
         assert self.rl_model is not None, 'RL model not initialized'
         assert isinstance(self.rl_model, OnPolicyAlgorithm), 'RL model must be an instance of OnPolicyAlgorithm'
         model: OnPolicyAlgorithm = self.rl_model
         info = self.rl_gen_info()
         reward = self.rl_gen_reward()
         obs = self.rl_gen_obs()
@@ -337,24 +331,22 @@
                     info = info
                     action = self.rl_collector.send((obs, reward, done, info))
             except StopIteration:
                 self.rl_collector = None
                 self.rl_iteration += 1
                 # Display training infos
                 bt_on_policy_train(model, iteration=self.rl_iteration, log_interval=log_interval)
-                if self.rl_iteration % save_interval == 0:
-                    model.save(save_path)
 
                 self.rl_collector = bt_on_policy_collect_rollouts(
                         model,
                         last_obs=obs)
                 action = self.rl_collector.send(None)
         else:
             # 预测模式
-            action, state = model.predict(obs)
+            action, state = model.predict(obs, deterministic=deterministic)
 
         self.rl_obs = obs
         self.rl_reward = reward
         self.rl_info = info
         self.rl_accum_reward += reward
         self.rl_action = action
         self.rl_done = done
@@ -376,15 +368,15 @@
                 observation_space=self.rl_observation_space())
         model: typing.Optional[BaseAlgorithm] = None
 
         if train:
             model = model_class(
                     policy=self.rl_policy(),
                     env=env,
-                    verbose=1,
+                    verbose=verbose,
                     tensorboard_log=tensorboard_log,
                     device=self.rl_device(),
                     **kwargs
             )
 
             if path != '':
                 try:
```

### Comparing `pybts-1.6.0/pybts/rl/off_policy.py` & `pybts-1.6.1/pybts/rl/off_policy.py`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/rl/on_policy.py` & `pybts-1.6.1/pybts/rl/on_policy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,38 @@
 import numpy as np
+import torch
 from gymnasium import spaces
 from stable_baselines3.common.on_policy_algorithm import OnPolicyAlgorithm
 from stable_baselines3.common.utils import (
-    safe_mean, obs_as_tensor,
+    safe_mean,
     configure_logger
 )
+from stable_baselines3.common.type_aliases import GymEnv, Schedule, TensorDict, TrainFreq, TrainFrequencyUnit
 import typing
 import torch as th
 import time
 from collections import deque
 import sys
+from typing import Union, Dict
+
+
+def obs_as_tensor(obs: Union[np.ndarray, Dict[str, np.ndarray]], device: th.device) -> Union[th.Tensor, TensorDict]:
+    """
+    Moves the observation to the given device.
+    为了兼容mps，数据值用float32来保存
+    :param obs:
+    :param device: PyTorch device
+    :return: PyTorch tensor of the observation on a desired device.
+    """
+    if isinstance(obs, np.ndarray):
+        return th.as_tensor(obs, device=device, dtype=th.float32)
+    elif isinstance(obs, dict):
+        return { key: th.as_tensor(_obs, device=device, dtype=th.float32) for (key, _obs) in obs.items() }
+    else:
+        raise Exception(f"Unrecognized type of observation {type(obs)}")
 
 
 def bt_on_policy_setup_learn(
         self: OnPolicyAlgorithm,
         obs,
         tb_log_name: str = 'run',
         reset_num_timesteps: bool = True,
@@ -126,33 +145,38 @@
 
         if isinstance(self.action_space, spaces.Discrete):
             # Reshape in case of discrete action
             actions = actions.reshape(-1, 1)
 
         # Handle timeout by bootstraping with value function
         # see GitHub issue #633
+        # 在环境因达到最大步数而非自然终止时，提供一个合理的未来价值估计，从而帮助学习算法更好地理解和学习到达该状态的长期影响。
+        # 这种处理方式是对传统强化学习中的处理截断问题的一种常见实践。
+        # 在没有这种处理时，算法可能会错误地认为达到步数限制是一种负面的结果，而实际上它仅仅是由环境的设定导致的。
         for idx, done in enumerate(dones):
             if (
                     done
-                    and infos[idx].get("terminal_observation") is not None
-                    and infos[idx].get("TimeLimit.truncated", False)
+                    and infos[idx].get("truncated", False)
             ):
-                terminal_obs = self.policy.obs_to_tensor(infos[idx]["terminal_observation"])[0]
+                terminal_obs = obs_as_tensor(self._last_obs, self.device)
                 with th.no_grad():
                     terminal_value = self.policy.predict_values(terminal_obs)[0]  # type: ignore[arg-type]
                 rewards[idx] += self.gamma * terminal_value
 
         self.rollout_buffer.add(
                 self._last_obs,  # type: ignore[arg-type]
                 actions,
                 rewards,
                 self._last_episode_starts,  # type: ignore[arg-type]
                 values,
                 log_probs,
         )
+        # print(
+        #         f'collector_{self.n_steps}: {n_steps} actions={actions.tolist()} rewards={rewards.tolist()} dones={dones.tolist()} values={values.tolist()}')
+
         self._last_obs = new_obs  # type: ignore[assignment]
         self._last_episode_starts = dones
 
     with th.no_grad():
         # Compute value for the last timestep
         values = self.policy.predict_values(obs_as_tensor(new_obs, self.device))  # type: ignore[arg-type]
```

### Comparing `pybts-1.6.0/pybts/rl/tree.py` & `pybts-1.6.1/pybts/rl/tree.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 class RLTree(Tree):
     """
     强化学习树
     """
 
     def __init__(self, root: Node, name: str = '', context: dict = None):
         super().__init__(root=root, name=name, context=context)
-        self.context['rl_reward'] = defaultdict(int)  # 本轮的奖励，默认scope是default
+        self.context['reward'] = defaultdict(int)  # 本轮的奖励，默认scope是default
 
     def reset(self):
         super().reset()
         # 清空奖励
-        self.context['rl_reward'] = defaultdict(int)
+        self.context['reward'] = defaultdict(int)
 
     def tick(
             self: RLTree,
             pre_tick_handler: typing.Optional[
                 typing.Callable[[RLTree], None]
             ] = None,
             post_tick_handler: typing.Optional[
                 typing.Callable[[RLTree], None]
             ] = None,
     ) -> None:
         # 不清空奖励，由PPO节点自行判断
-        # for scope in self.context['rl_reward']:
-        #     self.context['rl_reward'][scope] = 0  # 在tick之前清空奖励
+        # for scope in self.context['reward']:
+        #     self.context['reward'][scope] = 0  # 在tick之前清空奖励
         super().tick(pre_tick_handler=pre_tick_handler, post_tick_handler=post_tick_handler)
```

### Comparing `pybts-1.6.0/pybts/templates/favicon.ico` & `pybts-1.6.1/pybts/templates/favicon.ico`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/templates/static/index-BlldS3Jx.js` & `pybts-1.6.1/pybts/templates/static/index-BlldS3Jx.js`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/templates/static/index-DN1S--qx.css` & `pybts-1.6.1/pybts/templates/static/index-DN1S--qx.css`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/templates/static/info-lb9hZOuB.png` & `pybts-1.6.1/pybts/templates/static/info-lb9hZOuB.png`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/tree.py` & `pybts-1.6.1/pybts/tree.py`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pybts/utility.py` & `pybts-1.6.1/pybts/utility.py`

 * *Files identical despite different names*

### Comparing `pybts-1.6.0/pyproject.toml` & `pybts-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybts"
-version = "1.6.0"
+version = "1.6.1"
 description = ""
 authors = ["王童 <785271992@qq.com>"]
 readme = "README.md"
 homepage = "https://github.com/wangtong2015/pybts"
 repository = "https://github.com/wangtong2015/pybts"
 keywords = ["BehaviorTree", "AI"]
 include = ["README.md", "pybts/templates/static/*", 'pybts/templates/*', 'README.assets']
```

### Comparing `pybts-1.6.0/PKG-INFO` & `pybts-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybts
-Version: 1.6.0
+Version: 1.6.1
 Summary: 
 Home-page: https://github.com/wangtong2015/pybts
 Keywords: BehaviorTree,AI
 Author: 王童
 Author-email: 785271992@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

