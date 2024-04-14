# Comparing `tmp/neopyter-0.2.0.tar.gz` & `tmp/neopyter-0.2.1.tar.gz`

## Comparing `neopyter-0.2.0.tar` & `neopyter-0.2.1.tar`

### file list

```diff
@@ -1,97 +1,103 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 neopyter-0.2.0/.commitlintrc.cjs
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 neopyter-0.2.0/.editorconfig
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 neopyter-0.2.0/.eslintignore
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 neopyter-0.2.0/.eslintrc.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 neopyter-0.2.0/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 neopyter-0.2.0/.yarnrc.yml
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 neopyter-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 neopyter-0.2.0/Makefile
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 neopyter-0.2.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 neopyter-0.2.0/babel.config.js
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 neopyter-0.2.0/conftest.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 neopyter-0.2.0/install.json
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 neopyter-0.2.0/jest.config.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 neopyter-0.2.0/jest.polyfills.js
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 neopyter-0.2.0/package.json
--rw-r--r--   0        0        0   345980 2020-02-02 00:00:00.000000 neopyter-0.2.0/pnpm-lock.yaml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 neopyter-0.2.0/pnpm-workspace.yaml
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 neopyter-0.2.0/pyrightconfig.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neopyter-0.2.0/requirements.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 neopyter-0.2.0/setup.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 neopyter-0.2.0/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 neopyter-0.2.0/tsconfig.test.json
--rw-r--r--   0        0        0   444961 2020-02-02 00:00:00.000000 neopyter-0.2.0/yarn.lock
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 neopyter-0.2.0/.husky/commit-msg
--rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 neopyter-0.2.0/.husky/pre-commit
--rw-r--r--   0        0        0    74924 2020-02-02 00:00:00.000000 neopyter-0.2.0/doc/cell_magic.png
--rw-r--r--   0        0        0  1138980 2020-02-02 00:00:00.000000 neopyter-0.2.0/doc/communication.png
--rw-r--r--   0        0        0    81980 2020-02-02 00:00:00.000000 neopyter-0.2.0/doc/completion.png
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 neopyter-0.2.0/doc/example.ju.py
--rw-r--r--   0        0        0    72000 2020-02-02 00:00:00.000000 neopyter-0.2.0/doc/line_magic.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neopyter-0.2.0/doc/neopyter.txt
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 neopyter-0.2.0/jupyter-config/server-config/neopyter.json
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 neopyter-0.2.0/lua/neopyter.lua
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 neopyter-0.2.0/lua/neopyter/asyncwrap.lua
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 neopyter-0.2.0/lua/neopyter/cmp.lua
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 neopyter-0.2.0/lua/neopyter/health.lua
--rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 neopyter-0.2.0/lua/neopyter/highlight.lua
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 neopyter-0.2.0/lua/neopyter/logger.lua
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 neopyter-0.2.0/lua/neopyter/textobjects.lua
--rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 neopyter-0.2.0/lua/neopyter/utils.lua
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 neopyter-0.2.0/lua/neopyter/jupyter/init.lua
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 neopyter-0.2.0/lua/neopyter/jupyter/jupyterlab.lua
--rw-r--r--   0        0        0     9942 2020-02-02 00:00:00.000000 neopyter-0.2.0/lua/neopyter/jupyter/notebook.lua
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 neopyter-0.2.0/lua/neopyter/rpc/asyncclient.lua
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 neopyter-0.2.0/lua/neopyter/rpc/baseclient.lua
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 neopyter-0.2.0/lua/neopyter/rpc/blockclient.lua
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 neopyter-0.2.0/lua/neopyter/rpc/init.lua
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 neopyter-0.2.0/lua/neopyter/rpc/msgpack.lua
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 neopyter-0.2.0/lua-tests/minimal_init.lua
--rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 neopyter-0.2.0/lua-tests/neopyter/utils_spec.lua
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 neopyter-0.2.0/neopyter/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 neopyter-0.2.0/neopyter/_version.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 neopyter-0.2.0/neopyter/handler.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 neopyter-0.2.0/neopyter/msgpack_queue.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 neopyter-0.2.0/neopyter/tcp_server.py
--rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 neopyter-0.2.0/neopyter/labextension/package.json
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 neopyter-0.2.0/neopyter/labextension/schemas/neopyter/labplugin.json
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 neopyter-0.2.0/neopyter/labextension/schemas/neopyter/package.json.orig
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 neopyter-0.2.0/neopyter/labextension/static/330.91022d3a2c8e60de7676.js
--rw-r--r--   0        0        0     9898 2020-02-02 00:00:00.000000 neopyter-0.2.0/neopyter/labextension/static/336.f2f9124a0511bcaade9f.js
--rw-r--r--   0        0        0    29596 2020-02-02 00:00:00.000000 neopyter-0.2.0/neopyter/labextension/static/7.8eb9a8e937e5deb3af13.js
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 neopyter-0.2.0/neopyter/labextension/static/728.d85cbe66bc2da24c7357.js
--rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 neopyter-0.2.0/neopyter/labextension/static/769.477fd518dada39821aad.js
--rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 neopyter-0.2.0/neopyter/labextension/static/remoteEntry.6c91dc6f35c735e32d34.js
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 neopyter-0.2.0/neopyter/labextension/static/style.js
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 neopyter-0.2.0/neopyter/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 neopyter-0.2.0/neopyter/tests/__init__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 neopyter-0.2.0/neopyter/tests/server/test_handlers.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 neopyter-0.2.0/plugin/neopyter.lua
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neopyter-0.2.0/queries/python/folds.scm
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 neopyter-0.2.0/queries/python/highlights.scm
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 neopyter-0.2.0/queries/python/injections.scm
--rw-r--r--   0        0        0     6338 2020-02-02 00:00:00.000000 neopyter-0.2.0/queries/python/textobjects.scm
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 neopyter-0.2.0/schema/labplugin.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 neopyter-0.2.0/src/error.ts
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 neopyter-0.2.0/src/icons.ts
--rw-r--r--   0        0        0    12990 2020-02-02 00:00:00.000000 neopyter-0.2.0/src/index.ts
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 neopyter-0.2.0/src/msgpackRpcProtocol.ts
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 neopyter-0.2.0/src/rpcServer.ts
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 neopyter-0.2.0/src/statusidepanel.ts
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 neopyter-0.2.0/src/svg.d.ts
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 neopyter-0.2.0/src/__tests__/neojupy.spec.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neopyter-0.2.0/src/dispatcher/basic.ts
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 neopyter-0.2.0/src/dispatcher/docmanager.ts
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 neopyter-0.2.0/src/transport/base.ts
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 neopyter-0.2.0/src/transport/index.ts
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 neopyter-0.2.0/src/transport/reverseHttpTransport.ts
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 neopyter-0.2.0/src/transport/websocketTransport.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 neopyter-0.2.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 neopyter-0.2.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 neopyter-0.2.0/style/index.js
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 neopyter-0.2.0/style/icons/statuspage.svg
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 neopyter-0.2.0/.gitignore
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 neopyter-0.2.0/LICENSE
--rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 neopyter-0.2.0/README.md
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 neopyter-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    13446 2020-02-02 00:00:00.000000 neopyter-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 neopyter-0.2.1/.commitlintrc.cjs
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 neopyter-0.2.1/.editorconfig
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 neopyter-0.2.1/.eslintignore
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 neopyter-0.2.1/.eslintrc.json
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 neopyter-0.2.1/.neoconf.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 neopyter-0.2.1/.prettierignore
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 neopyter-0.2.1/.stylua.toml
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 neopyter-0.2.1/.yarnrc.yml
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 neopyter-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 neopyter-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 neopyter-0.2.1/Makefile
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 neopyter-0.2.1/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 neopyter-0.2.1/babel.config.js
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 neopyter-0.2.1/conftest.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 neopyter-0.2.1/install.json
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 neopyter-0.2.1/jest.config.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 neopyter-0.2.1/jest.polyfills.js
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 neopyter-0.2.1/package.json
+-rw-r--r--   0        0        0   345980 2020-02-02 00:00:00.000000 neopyter-0.2.1/pnpm-lock.yaml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 neopyter-0.2.1/pnpm-workspace.yaml
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 neopyter-0.2.1/pyrightconfig.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neopyter-0.2.1/requirements.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 neopyter-0.2.1/setup.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 neopyter-0.2.1/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 neopyter-0.2.1/tsconfig.test.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 neopyter-0.2.1/.husky/commit-msg
+-rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 neopyter-0.2.1/.husky/pre-commit
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 neopyter-0.2.1/after/plugin/cmp_neopyter.lua
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neopyter-0.2.1/after/queries/python/folds.scm
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 neopyter-0.2.1/after/queries/python/highlights.scm
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 neopyter-0.2.1/after/queries/python/injections.scm
+-rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 neopyter-0.2.1/after/queries/python/textobjects.scm
+-rw-r--r--   0        0        0    74924 2020-02-02 00:00:00.000000 neopyter-0.2.1/doc/cell_magic.png
+-rw-r--r--   0        0        0   799344 2020-02-02 00:00:00.000000 neopyter-0.2.1/doc/communication_direct.png
+-rw-r--r--   0        0        0  1138980 2020-02-02 00:00:00.000000 neopyter-0.2.1/doc/communication_proxy.png
+-rw-r--r--   0        0        0    81980 2020-02-02 00:00:00.000000 neopyter-0.2.1/doc/completion.png
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 neopyter-0.2.1/doc/example.ju.py
+-rw-r--r--   0        0        0    72000 2020-02-02 00:00:00.000000 neopyter-0.2.1/doc/line_magic.png
+-rw-r--r--   0        0        0    11581 2020-02-02 00:00:00.000000 neopyter-0.2.1/doc/neopyter.txt
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 neopyter-0.2.1/jupyter-config/server-config/neopyter.json
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter.lua
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/asyncwrap.lua
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/cmp.lua
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/health.lua
+-rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/highlight.lua
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/logger.lua
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/textobjects.lua
+-rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/utils.lua
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/jupyter/init.lua
+-rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/jupyter/jupyterlab.lua
+-rw-r--r--   0        0        0     9926 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/jupyter/notebook.lua
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/rpc/asyncclient.lua
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/rpc/baseclient.lua
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/rpc/blockclient.lua
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/rpc/msgpack.lua
+-rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/rpc/wsserverclient.lua
+-rw-r--r--   0        0        0     7527 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua-tests/neopyter/utils_spec.lua
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/_version.py
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/handler.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/msgpack_queue.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/tcp_server.py
+-rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/package.json
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/schemas/neopyter/labplugin.json
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/schemas/neopyter/package.json.orig
+-rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/static/330.aa97145ed71c9fb187d2.js
+-rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/static/336.a49647ad642daa70dfb8.js
+-rw-r--r--   0        0        0    37319 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/static/537.62c041ec63a28b9c91aa.js
+-rw-r--r--   0        0        0    29596 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/static/7.8eb9a8e937e5deb3af13.js
+-rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/static/728.d85cbe66bc2da24c7357.js
+-rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/static/remoteEntry.dfbe5e3084dd43118cf8.js
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/static/style.js
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/tests/__init__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/tests/server/test_handlers.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 neopyter-0.2.1/plugin/neopyter.lua
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 neopyter-0.2.1/schema/labplugin.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 neopyter-0.2.1/scripts/minidoc.lua
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 neopyter-0.2.1/scripts/minimal_init.lua
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/error.ts
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/icons.ts
+-rw-r--r--   0        0        0    14551 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/index.ts
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/msgpackRpcProtocol.ts
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/rpcServer.ts
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/settings.ts
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/statusidepanel.ts
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/svg.d.ts
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/__tests__/neojupy.spec.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/dispatcher/basic.ts
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/dispatcher/docmanager.ts
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/transport/base.ts
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/transport/index.ts
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/transport/reverseHttpTransport.ts
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/transport/websocketTransport.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 neopyter-0.2.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 neopyter-0.2.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 neopyter-0.2.1/style/index.js
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 neopyter-0.2.1/style/icons/statuspage.svg
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 neopyter-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 neopyter-0.2.1/LICENSE
+-rw-r--r--   0        0        0     9062 2020-02-02 00:00:00.000000 neopyter-0.2.1/README.md
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 neopyter-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 neopyter-0.2.1/PKG-INFO
```

### Comparing `neopyter-0.2.0/.eslintrc.json` & `neopyter-0.2.1/.eslintrc.json`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/CHANGELOG.md` & `neopyter-0.2.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/RELEASE.md` & `neopyter-0.2.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/jest.config.js` & `neopyter-0.2.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/package.json` & `neopyter-0.2.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782608695652174%*

 * *Differences: {"'version'": "'0.2.1'"}*

```diff
@@ -135,12 +135,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.0",
+    "version": "0.2.1",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `neopyter-0.2.0/pnpm-lock.yaml` & `neopyter-0.2.1/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/tsconfig.json` & `neopyter-0.2.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/doc/cell_magic.png` & `neopyter-0.2.1/doc/cell_magic.png`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/doc/communication.png` & `neopyter-0.2.1/doc/communication_proxy.png`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/doc/completion.png` & `neopyter-0.2.1/doc/completion.png`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/doc/example.ju.py` & `neopyter-0.2.1/doc/example.ju.py`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/doc/line_magic.png` & `neopyter-0.2.1/doc/line_magic.png`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/lua/neopyter.lua` & `neopyter-0.2.1/lua/neopyter.lua`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,54 @@
 local highlight = require("neopyter.highlight")
 local jupyter = require("neopyter.jupyter")
 local JupyterLab = require("neopyter.jupyter.jupyterlab")
 local utils = require("neopyter.utils")
 
+---@toc
+
+local neopyter = {}
+
+---@text
+
+--- What is Neopyter ?
+---
+--- # Abstract~
+---
+--- The bridge between Neovim and jupyter lab, edit in Neovim and preview/run in jupyter lab.
+---
+---@tag neopyter
+---@toc_entry Neopyter's purpose
+
+---@tag neopyter-usage
+---@toc_entry Usages
 ---@class neopyter.Option
 ---@field remote_address string
 ---@field file_pattern string[]
 ---@field auto_attach boolean Automatically attach to the Neopyter server when open file_pattern matched files
 ---@field auto_connect boolean # auto connect jupyter lab
----@field rpc_client
----| "'async'" # AsyncRpcClient, default
----| "'block'" # BlockRpcClient
+---@field mode "direct"|"proxy"
 ---@field filename_mapper fun(ju_path:string):string
 ---@field on_attach? fun(bufnr:number)
 ---@field jupyter neopyter.JupyterOption
 ---@field highlight neopyter.HighlightOption
 ---@field parse_option neopyter.ParseOption
-local M = {}
 
+---@eval return MiniDoc.afterlines_to_code(MiniDoc.current.eval_section)
 ---@type neopyter.Option
-M.config = {
+neopyter.config = {
     remote_address = "127.0.0.1:9001",
     file_pattern = { "*.ju.*" },
     filename_mapper = function(ju_path)
         local ipynb_path = ju_path:gsub("%.ju%.%w+", ".ipynb")
         return ipynb_path
     end,
 
     auto_attach = true,
     auto_connect = true,
-    rpc_client = "async",
+    mode = "proxy",
     jupyter = {
         auto_activate_file = true,
         -- Always scroll to the current cell.
         scroll = {
             enable = true,
             mode = "always", -- "always" or "invisible"
             step = 0.5,
@@ -48,42 +63,37 @@
         shortsighted = true,
     },
     parse_option = {
         line_magic = true,
     },
 }
 
----setup neopyter
 ---@param config neopyter.Option
-function M.setup(config)
-    M.config = vim.tbl_deep_extend("force", M.config, config or {})
+function neopyter.setup(config)
+    neopyter.config = vim.tbl_deep_extend("force", neopyter.config, config or {})
 
     jupyter.jupyterlab = JupyterLab:new({
-        address = M.config.remote_address,
+        address = neopyter.config.remote_address,
     })
 
-    if M.config.auto_attach then
+    if neopyter.config.auto_attach then
         local augroup = vim.api.nvim_create_augroup("neopyter", { clear = true })
         utils.nvim_create_autocmd({ "BufReadPost" }, {
             group = augroup,
-            pattern = M.config.file_pattern,
+            pattern = neopyter.config.file_pattern,
             callback = function()
-                if M.config.auto_connect and not jupyter.jupyterlab:is_connecting() then
+                if neopyter.config.auto_connect and not jupyter.jupyterlab:is_connecting() then
                     jupyter.jupyterlab:connect()
                 end
                 if not jupyter.jupyterlab:is_attached() then
                     jupyter.jupyterlab:attach()
                 end
             end,
         })
     end
 
-    highlight.setup(M.config.highlight)
-
-    local status, cmp = pcall(require, "cmp")
-    if status then
-        cmp.register_source("neopyter", require("neopyter.cmp"))
-        return
-    end
+    highlight.setup(neopyter.config.highlight)
 end
 
-return M
+---@tag neopyter-api
+---@toc_entry API
+return neopyter
```

### Comparing `neopyter-0.2.0/lua/neopyter/asyncwrap.lua` & `neopyter-0.2.1/lua/neopyter/asyncwrap.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/lua/neopyter/cmp.lua` & `neopyter-0.2.1/lua/neopyter/cmp.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/lua/neopyter/health.lua` & `neopyter-0.2.1/lua/neopyter/health.lua`

 * *Files 13% similar despite different names*

```diff
@@ -16,54 +16,53 @@
         end, 2)
     end
 end
 
 local function run_blocking(suspend_fn, ...)
     local resolved = false
     vim.schedule(function()
-        a.run(suspend_fn, function()
-            print("complete")
+        a.run(suspend_fn, function(ee)
             resolved = true
         end)
     end)
 
     vim.wait(0x7FFFFFFF, function()
         return resolved
     end, 1000)
 end
 
 function M.check()
     run_blocking(function()
         local status = jupyter.jupyterlab:is_attached()
         if status then
-            health.info("Neopyter status: active")
+            local nvim_plugin_ver = jupyter.jupyterlab:get_nvim_plugin_version()
+            health.info(string.format("Neopyter@%s status: active", nvim_plugin_ver))
             local is_connecting = jupyter.jupyterlab.client:is_connecting()
             if is_connecting then
                 health.info("Rpc server status: active")
+                local jupyterlab_extension_ver = jupyter.jupyterlab:get_jupyterlab_extension_version()
+                health.info(string.format("Jupyter lab extension version: %s", jupyterlab_extension_ver))
             else
                 health.info("Rpc server status: inactive")
             end
             health.start("Jupyter lab")
             for _, notebook in pairs(jupyter.jupyterlab.notebook_map) do
                 local select_mark = " "
                 if jupyter.notebook == notebook then
                     select_mark = "*"
                 end
                 local msg = ""
-                print(notebook.local_path)
                 local nbconnect = notebook:is_connecting()
-                print(notebook.remote_path)
                 if nbconnect then
                     msg = string.format("%s %s 💫 %s", select_mark, notebook.local_path, notebook.remote_path)
                 else
                     msg = string.format("%s %s 💥", select_mark, notebook.local_path, notebook.remote_path)
                 end
                 health.info(msg)
             end
         else
             health.info(string.format("Neopyter status: inactive"))
         end
-        print("complete")
     end)
 end
 
 return M
```

### Comparing `neopyter-0.2.0/lua/neopyter/highlight.lua` & `neopyter-0.2.1/lua/neopyter/highlight.lua`

 * *Files 18% similar despite different names*

```diff
@@ -12,24 +12,41 @@
 
 ---setup/update highlight module
 ---@param opts neopyter.HighlightOption
 function M.setup(opts)
     if opts.enable then
         local config = require("neopyter").config
         local augroup = vim.api.nvim_create_augroup("neopyter-highlighter", {})
+        local updated = false
         if opts.shortsighted then
             vim.api.nvim_create_autocmd({ "CursorMoved", "CursorMovedI", "WinScrolled" }, {
                 pattern = config.file_pattern,
-                callback = M.update_dynamic_highlight,
+                callback = function()
+                    updated = false
+                    vim.defer_fn(function()
+                        if updated == false then
+                            updated = true
+                            M.update_dynamic_highlight()
+                        end
+                    end, 10)
+                end,
                 group = augroup,
             })
         else
             vim.api.nvim_create_autocmd({ "BufWinEnter", "BufWritePost", "TextChanged", "TextChangedI" }, {
                 pattern = config.file_pattern,
-                callback = M.update_static_highlight,
+                callback = function()
+                    updated = false
+                    vim.defer_fn(function()
+                        if updated == false then
+                            updated = true
+                            M.update_static_highlight()
+                        end
+                    end, 10)
+                end,
                 group = augroup,
             })
         end
     end
 end
 
 function M.update_static_highlight()
```

### Comparing `neopyter-0.2.0/lua/neopyter/textobjects.lua` & `neopyter-0.2.1/lua/neopyter/textobjects.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/lua/neopyter/utils.lua` & `neopyter-0.2.1/lua/neopyter/utils.lua`

 * *Files 5% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         opts.callback = function(...)
             local args = { ... }
             a.run(function()
                 old_callback(unpack(args))
             end, function() end)
         end
     end
-    vim.api.nvim_create_autocmd(event, opts)
+    a.api.nvim_create_autocmd(event, opts)
 end
 
 ---@class neopyter.ParseOption
 ---@field line_magic boolean|nil
 ---@field content_annotated_cell_types string[]|nil
 
 ---parse lines
@@ -190,8 +190,16 @@
         if api.nvim_win_get_buf(win) == bufnr then
             return win
         end
     end
     return nil
 end
 
+---@param address string
+---@return string host
+---@return number port
+function M.parse_address(address)
+    local host, port = address:match("^(.-):(%d+)$")
+    return host, tonumber(port)--[[@as number]]
+end
+
 return M
```

### Comparing `neopyter-0.2.0/lua/neopyter/jupyter/jupyterlab.lua` & `neopyter-0.2.1/lua/neopyter/jupyter/jupyterlab.lua`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-local rpc = require("neopyter.rpc")
 local Notebook = require("neopyter.jupyter.notebook")
 local utils = require("neopyter.utils")
 local async_wrap = require("neopyter.asyncwrap")
 local a = require("plenary.async")
 local Path = require("plenary.path")
 local api = a.api
 
@@ -20,24 +19,31 @@
 ---@class neopyter.NewJupyterLabOption
 ---@field address? string
 
 ---create RpcClient and connect
 ---@param opts neopyter.NewJupyterLabOption
 ---@return neopyter.JupyterLab
 function JupyterLab:new(opts)
-    local o = {} --[[@as neopyter.JupyterLab]]
+    local o = {}
     setmetatable(o, self)
     self.__index = self
 
     local config = require("neopyter").config
     local RpcClient
-    if config.rpc_client == "block" then
-        RpcClient = rpc.BlockRpcClient
+    if config["rpc_client"] ~= nil then
+        vim.notify(
+            "`rpc_client` is deprecated, please reference to https://github.com/SUSTech-data/neopyter/issues/4",
+            vim.log.levels.ERROR,
+            { title = "Neopyter" }
+        )
+    end
+    if config.mode == "direct" then
+        RpcClient = require("neopyter.rpc.wsserverclient")
     else
-        RpcClient = rpc.AsyncRpcClient
+        RpcClient = require("neopyter.rpc.asyncclient")
     end
     o.client = RpcClient:new({
         address = opts.address,
     })
     self.notebook_map = {}
     return o
 end
@@ -85,24 +91,22 @@
     return self.augroup ~= nil
 end
 
 ---connect server
 ---@param address? string address of neopyter server
 function JupyterLab:connect(address)
     self.client:connect(address)
-    local jupyterlab_version = self:get_jupyterlab_extension_version()
-    local nvim_version = self:get_nvim_plugin_version()
-    if jupyterlab_version ~= nil and nvim_version ~= jupyterlab_version then
-        utils.notify_error(
-            string.format(
-                "The version of jupyterlab extension(%s) and neovim plugin(%s) do not match",
-                jupyterlab_version,
-                nvim_version
+    if self.client:is_connecting() then
+        local jupyterlab_version = self:get_jupyterlab_extension_version()
+        local nvim_version = self:get_nvim_plugin_version()
+        if jupyterlab_version ~= nil and nvim_version ~= jupyterlab_version then
+            utils.notify_error(
+                string.format("The version of jupyterlab extension(%s) and neovim plugin(%s) do not match", jupyterlab_version, nvim_version)
             )
-        )
+        end
     end
 end
 
 function JupyterLab:disconnect(address)
     self.client:disconnect(address)
 end
 
@@ -132,15 +136,17 @@
             local_path = file_path,
         })
         self.notebook_map[file_path] = notebook
         jupyter.notebook = notebook
         notebook:attach()
         local config = require("neopyter").config
         if type(config.on_attach) == "function" then
-            config.on_attach(buf)
+            vim.schedule(function()
+                config.on_attach(buf)
+            end)
         end
     end
 
     if self:is_connecting() and notebook:is_exist() then
         if notebook:is_open() then
             notebook:activate()
         else
@@ -202,11 +208,10 @@
     return self.client:request("getCurrentNotebook", ops)
 end
 
 JupyterLab = async_wrap(JupyterLab, {
     "attach",
     "is_attached",
     "is_connecting",
-    "get_nvim_plugin_version",
 })
 
 return JupyterLab
```

### Comparing `neopyter-0.2.0/lua/neopyter/jupyter/notebook.lua` & `neopyter-0.2.1/lua/neopyter/jupyter/notebook.lua`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         on_lines = function(_, _, _, start_row, old_end_row, new_end_row, _)
             a.run(function()
                 if not self:is_connecting() then
                     self:update_cells()
                     return
                 end
                 self:partial_sync(start_row, old_end_row, new_end_row)
-            end, function() end)
+            end)
         end,
     })
 
     self:update_cells()
 
     if self:is_connecting() then
         self:open_or_reveal()
```

### Comparing `neopyter-0.2.0/lua/neopyter/rpc/asyncclient.lua` & `neopyter-0.2.1/lua/neopyter/rpc/asyncclient.lua`

 * *Files 8% similar despite different names*

```diff
@@ -8,65 +8,60 @@
 ---@field tcp_client? uv_tcp_t # nil means not connect
 ---@field private msg_count number
 ---@field private request_pool table<number, fun(...):any>
 ---@field private decoder neopyter.MsgpackDecoder
 local AsyncRpcClient = RpcClient:new({}) --[[@as neopyter.AsyncRpcClient]]
 
 ---RpcClient constructor
----@param o neopyter.NewRpcClientOption
+---@param opt neopyter.NewRpcClientOption
 ---@return neopyter.AsyncRpcClient
-function AsyncRpcClient:new(o)
-    o = o or {} --[[@as neopyter.AsyncRpcClient]]
-    setmetatable(o, self)
+function AsyncRpcClient:new(opt)
+    opt = opt or {}
+    local o = setmetatable(opt, self)
     self.__index = self
 
     o.msg_count = 0
     o.request_pool = {}
     o.decoder = msgpack.Decoder:new()
-    return o
-end
-
----@package
----@param address string
-local function parse_address(address)
-    local host, port = address:match("^(.-):(%d+)$")
-    return host, tonumber(port)
+    return o --[[@type neopyter.AsyncRpcClient]]
 end
 
 ---comment
 ---@param address? string
 ---@async
 function AsyncRpcClient:connect(address)
     self.address = address or self.address
     assert(self.tcp_client == nil, "current connection exists, can't call connect, please disconnect first")
     assert(self.address, "Rpc client address is empty")
     self.tcp_client = vim.loop.new_tcp()
-    local host, port = parse_address(self.address)
+    local host, port = utils.parse_address(self.address)
     local err = a.uv.tcp_connect(self.tcp_client, host, port)
     if err ~= nil then
         utils.notify_error(string.format("Connect rpc server [%s] failed", self.address))
         self.tcp_client = nil
     else
         self.tcp_client:read_start(function(e, data)
             if e ~= nil or data == nil then
                 for _, callback in ipairs(self.request_pool) do
                     callback(false, e)
                 end
-                self:close()
+                self:disconnect()
             else
                 self:handle_response(data)
             end
         end)
     end
 end
 
 ---disconnect connect
 function AsyncRpcClient:disconnect()
-    self.tcp_client:close()
-    self.tcp_client = nil
+    if self.tcp_client then
+        self.tcp_client:close()
+        self.tcp_client = nil
+    end
 end
 
 ---check client is connecting
 ---@return boolean
 function AsyncRpcClient:is_connecting()
     return self.tcp_client ~= nil
 end
@@ -96,19 +91,15 @@
     logger.log(string.format("msgid [%s] finished: %s", msgid, vim.inspect(res)))
 
     if status then
         return res
     else
         if method == "getVersion" then
             utils.notify_error(
-                string.format(
-                    "jupyterlab extension is outdated, it is recommended to update with `pip install -U neopyter`",
-                    method,
-                    res
-                )
+                string.format("jupyterlab extension is outdated, it is recommended to update with `pip install -U neopyter`", method, res)
             )
         else
             utils.notify_error(string.format("RPC request [%s] failed, with error: %s", method, res))
         end
     end
 end
 
@@ -124,33 +115,22 @@
         end
         -- logger.log(vim.inspect(msg))
         if #msg == 4 and msg[1] == 1 then
             local msgid, error, result = msg[2], msg[3], msg[4]
             local callback = self.request_pool[msgid]
             self.request_pool[msgid] = nil
             logger.log(string.format("msgid [%s] response acceptd", msgid))
-            assert(
-                callback,
-                string.format("msg %s can't find callback: request_pool=%s", msgid, vim.inspect(self.request_pool))
-            )
+            assert(callback, string.format("msg %s can't find callback: request_pool=%s", msgid, vim.inspect(self.request_pool)))
             if error == vim.NIL then
                 callback(true, result)
             else
                 callback(false, error)
             end
         else
             assert(false, "msgpack rpc response spec error, msg=" .. data)
         end
     end
 end
 
 function AsyncRpcClient:notify(event, ...) end
 
----close tcp
----@async
-function AsyncRpcClient:close()
-    if self.tcp_client then
-        self.tcp_client:close(function() end)
-    end
-end
-
 return AsyncRpcClient
```

### Comparing `neopyter-0.2.0/lua/neopyter/rpc/baseclient.lua` & `neopyter-0.2.1/lua/neopyter/rpc/baseclient.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/lua/neopyter/rpc/blockclient.lua` & `neopyter-0.2.1/lua/neopyter/rpc/blockclient.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/lua/neopyter/rpc/msgpack.lua` & `neopyter-0.2.1/lua/neopyter/rpc/msgpack.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/lua-tests/neopyter/utils_spec.lua` & `neopyter-0.2.1/lua-tests/neopyter/utils_spec.lua`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,14 @@
                         '"""',
                         "# this is markdown cell with markdown too",
                         '"""',
                     },
                     source = "# this is markdown cell with markdown too",
                     start_line = 1,
                     end_line = 5,
-                    title= "cell's title",
+                    title = "cell's title",
                     cell_type = "markdown",
                 },
             }, cells)
         end)
     end)
 end)
```

### Comparing `neopyter-0.2.0/neopyter/__init__.py` & `neopyter-0.2.1/neopyter/__init__.py`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/neopyter/handler.py` & `neopyter-0.2.1/neopyter/handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,17 +7,26 @@
 from typing import Union, Optional, Awaitable
 import base64
 
 from .msgpack_queue import labextension_queue, client_queue
 from .tcp_server import tcpServer
 
 
+settings = {"mode": "proxy", "host": "127.0.0.1", "port": 9001}
+
+
 class ForwardWebsocketHandler(WebSocketHandler):
     def open(self, *args: str, **kwargs: str) -> Optional[Awaitable[None]]:
         print("Websocket opened for lab extension")
+        if settings["mode"] == "direct":
+            print("mode is direct, cann't connect jupyter server websocket")
+            self.write("mode is direct, cann't connect jupyter server websocket")
+            self.close()
+            return
+
         self.task = asyncio.create_task(self.start_loop())
 
         if not tcpServer.is_running:
             asyncio.create_task(tcpServer.start())
 
     def on_message(self, message: Union[str, bytes]) -> Optional[Awaitable[None]]:
         buf = message
@@ -39,22 +48,22 @@
                 # await self.write_message(buf)
             await asyncio.sleep(0.2)
 
 
 class TcpServerInfoHandler(APIHandler):
     @tornado.web.authenticated
     def get(self):
-        if not tcpServer.server:
+        if not tcpServer.is_running:
             return self.finish(
                 {"code": 1, "message": "tcp server not start, please check server port"}
             )
 
         addrs = []
         for sock in tcpServer.server.sockets:
-            ip,port = sock.getsockname()
+            ip, port = sock.getsockname()
             addrs.append(f"{ip}:{port}")
 
         return self.finish(
             {
                 "code": 0,
                 "message": "success",
                 "data": {"addrs": addrs},
@@ -62,19 +71,42 @@
         )
 
 
 class UpdateSettingsHandler(APIHandler):
     @tornado.web.authenticated
     def post(self):
         settings = tornado.escape.json_decode(self.request.body)
+        mode = settings.get("mode", "proxy")
+
         host = (settings.get("ip", "") or "").strip().split(",")
         while "" in host:
             host.remove("")
 
         port = settings["port"]
+
+        print("-------------debug-------------------")
+        settings["mode"] = mode
+        settings["host"] = host
+        settings["port"] = port
+        print(mode, host, port, tcpServer.is_running)
+        if mode == "direct":
+            if tcpServer.is_running:
+                asyncio.create_task(tcpServer.stop())
+                return self.finish(
+                    {
+                        "code": 0,
+                        "message": "success, tcp server is running, shutdown it",
+                    }
+                )
+            return self.finish(
+                {
+                    "code": 0,
+                    "message": "success, tcp server is shutdown",
+                }
+            )
         if host == tcpServer.host and port == tcpServer.port:
             return self.finish(
                 {
                     "code": 0,
                     "message": "success, don't restart server",
                 }
             )
```

### Comparing `neopyter-0.2.0/neopyter/tcp_server.py` & `neopyter-0.2.1/neopyter/tcp_server.py`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/neopyter/labextension/package.json` & `neopyter-0.2.1/neopyter/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9778079710144927%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.dfbe5e3084dd43118cf8.js'}}",*

 * * "'version'": "'0.2.1'"}*

```diff
@@ -56,15 +56,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/SUSTech-data/neopyter",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.6c91dc6f35c735e32d34.js",
+            "load": "static/remoteEntry.dfbe5e3084dd43118cf8.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "neopyter/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -140,12 +140,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.0",
+    "version": "0.2.1",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `neopyter-0.2.0/neopyter/labextension/schemas/neopyter/package.json.orig` & `neopyter-0.2.1/neopyter/labextension/schemas/neopyter/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782608695652174%*

 * *Differences: {"'version'": "'0.2.1'"}*

```diff
@@ -135,12 +135,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.0",
+    "version": "0.2.1",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `neopyter-0.2.0/neopyter/labextension/static/330.91022d3a2c8e60de7676.js` & `neopyter-0.2.1/neopyter/labextension/static/330.aa97145ed71c9fb187d2.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
 "use strict";
 (self.webpackChunkneopyter = self.webpackChunkneopyter || []).push([
     [330], {
         330: e => {
-            e.exports = JSON.parse('{"name":"neopyter","version":"0.2.0","description":"A JupyterLab extension. Integrate JupyterLab and Neovim","workspaces":["ui-tests"],"keywords":["jupyter","jupyterlab","jupyterlab-extension","neovim"],"homepage":"https://github.com/SUSTech-data/neopyter","bugs":{"url":"https://github.com/SUSTech-data/neopyter/issues"},"license":"BSD-3-Clause","author":{"name":"Abao Zhang","email":"abaodoit@gmail.com"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/SUSTech-data/neopyter"},"scripts":{"build":"pnpm build:lib && pnpm build:labextension:dev","build:prod":"run-s clean build:lib:prod build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:lib:prod":"tsc","clean":"pnpm clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:lintcache":"rimraf .eslintcache .stylelintcache","clean:labextension":"rimraf neopyter/labextension neopyter/_version.py","clean:all":"pnpm clean:lib && pnpm clean:labextension && pnpm clean:lintcache","eslint":"pnpm eslint:check --fix","eslint:check":"eslint . --cache --ext .ts,.tsx","install:extension":"pnpm build","lint":"pnpm stylelint && pnpm prettier && pnpm eslint","lint:check":"pnpm stylelint:check && pnpm prettier:check && pnpm eslint:check","prettier":"pnpm prettier:base --write --list-different","prettier:base":"prettier \\"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\\"","prettier:check":"pnpm prettier:base --check","stylelint":"pnpm stylelint:check --fix","stylelint:check":"stylelint --cache \\"style/**/*.css\\"","test":"jest --coverage","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w --strict false --sourceMap","watch:labextension":"jupyter labextension watch .","prepare":"husky install"},"dependencies":{"@jupyterlab/application":"^4.1.5","@jupyterlab/apputils":"^4.2.5","@jupyterlab/logconsole":"^4.1.5","@jupyterlab/notebook":"^4.1.5","@lumino/widgets":"^2.3.1","@msgpack/msgpack":"3.0.0-beta2","remeda":"^1.55.0"},"devDependencies":{"@commitlint/cli":"^18.6.1","@commitlint/config-conventional":"^18.6.3","@jupyterlab/builder":"^4.1.5","@jupyterlab/completer":"^4.1.5","@jupyterlab/coreutils":"^6.1.5","@jupyterlab/docmanager":"^4.1.5","@jupyterlab/services":"^7.1.5","@jupyterlab/settingregistry":"^4.1.5","@jupyterlab/testutils":"^4.1.5","@jupyterlab/ui-components":"^4.1.5","@lumino/coreutils":"^2.1.2","@lumino/disposable":"^2.1.2","@types/jest":"^29.5.12","@types/json-schema":"^7.0.15","@typescript-eslint/eslint-plugin":"^6.21.0","@typescript-eslint/parser":"^6.21.0","css-loader":"^6.10.0","eslint":"^8.57.0","eslint-config-prettier":"^8.10.0","eslint-plugin-prettier":"^5.1.3","husky":"^8.0.3","jest":"^29.7.0","npm-run-all":"^4.1.5","prettier":"^3.2.5","rimraf":"^5.0.5","source-map-loader":"^1.1.3","style-loader":"^3.3.4","stylelint":"^15.11.0","stylelint-config-recommended":"^13.0.0","stylelint-config-standard":"^34.0.0","stylelint-prettier":"^4.1.0","typescript":"~5.0.4","yjs":"^13.6.14"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","publishConfig":{"access":"public"},"jupyterlab":{"extension":true,"schemaDir":"schema","outputDir":"neopyter/labextension"},"prettier":{"singleQuote":true,"trailingComma":"none","arrowParens":"avoid","endOfLine":"auto","overrides":[{"files":"package.json","options":{"tabWidth":4}}]},"stylelint":{"extends":["stylelint-config-recommended","stylelint-config-standard","stylelint-prettier/recommended"],"rules":{"property-no-vendor-prefix":null,"selector-no-vendor-prefix":null,"value-no-vendor-prefix":null}}}')
+            e.exports = JSON.parse('{"name":"neopyter","version":"0.2.1","description":"A JupyterLab extension. Integrate JupyterLab and Neovim","workspaces":["ui-tests"],"keywords":["jupyter","jupyterlab","jupyterlab-extension","neovim"],"homepage":"https://github.com/SUSTech-data/neopyter","bugs":{"url":"https://github.com/SUSTech-data/neopyter/issues"},"license":"BSD-3-Clause","author":{"name":"Abao Zhang","email":"abaodoit@gmail.com"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/SUSTech-data/neopyter"},"scripts":{"build":"pnpm build:lib && pnpm build:labextension:dev","build:prod":"run-s clean build:lib:prod build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:lib:prod":"tsc","clean":"pnpm clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:lintcache":"rimraf .eslintcache .stylelintcache","clean:labextension":"rimraf neopyter/labextension neopyter/_version.py","clean:all":"pnpm clean:lib && pnpm clean:labextension && pnpm clean:lintcache","eslint":"pnpm eslint:check --fix","eslint:check":"eslint . --cache --ext .ts,.tsx","install:extension":"pnpm build","lint":"pnpm stylelint && pnpm prettier && pnpm eslint","lint:check":"pnpm stylelint:check && pnpm prettier:check && pnpm eslint:check","prettier":"pnpm prettier:base --write --list-different","prettier:base":"prettier \\"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\\"","prettier:check":"pnpm prettier:base --check","stylelint":"pnpm stylelint:check --fix","stylelint:check":"stylelint --cache \\"style/**/*.css\\"","test":"jest --coverage","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w --strict false --sourceMap","watch:labextension":"jupyter labextension watch .","prepare":"husky install"},"dependencies":{"@jupyterlab/application":"^4.1.5","@jupyterlab/apputils":"^4.2.5","@jupyterlab/logconsole":"^4.1.5","@jupyterlab/notebook":"^4.1.5","@lumino/widgets":"^2.3.1","@msgpack/msgpack":"3.0.0-beta2","remeda":"^1.55.0"},"devDependencies":{"@commitlint/cli":"^18.6.1","@commitlint/config-conventional":"^18.6.3","@jupyterlab/builder":"^4.1.5","@jupyterlab/completer":"^4.1.5","@jupyterlab/coreutils":"^6.1.5","@jupyterlab/docmanager":"^4.1.5","@jupyterlab/services":"^7.1.5","@jupyterlab/settingregistry":"^4.1.5","@jupyterlab/testutils":"^4.1.5","@jupyterlab/ui-components":"^4.1.5","@lumino/coreutils":"^2.1.2","@lumino/disposable":"^2.1.2","@types/jest":"^29.5.12","@types/json-schema":"^7.0.15","@typescript-eslint/eslint-plugin":"^6.21.0","@typescript-eslint/parser":"^6.21.0","css-loader":"^6.10.0","eslint":"^8.57.0","eslint-config-prettier":"^8.10.0","eslint-plugin-prettier":"^5.1.3","husky":"^8.0.3","jest":"^29.7.0","npm-run-all":"^4.1.5","prettier":"^3.2.5","rimraf":"^5.0.5","source-map-loader":"^1.1.3","style-loader":"^3.3.4","stylelint":"^15.11.0","stylelint-config-recommended":"^13.0.0","stylelint-config-standard":"^34.0.0","stylelint-prettier":"^4.1.0","typescript":"~5.0.4","yjs":"^13.6.14"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","publishConfig":{"access":"public"},"jupyterlab":{"extension":true,"schemaDir":"schema","outputDir":"neopyter/labextension"},"prettier":{"singleQuote":true,"trailingComma":"none","arrowParens":"avoid","endOfLine":"auto","overrides":[{"files":"package.json","options":{"tabWidth":4}}]},"stylelint":{"extends":["stylelint-config-recommended","stylelint-config-standard","stylelint-prettier/recommended"],"rules":{"property-no-vendor-prefix":null,"selector-no-vendor-prefix":null,"value-no-vendor-prefix":null}}}')
         }
     }
 ]);
```

### Comparing `neopyter-0.2.0/neopyter/labextension/static/336.f2f9124a0511bcaade9f.js` & `neopyter-0.2.1/neopyter/labextension/static/336.a49647ad642daa70dfb8.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,131 +1,137 @@
 "use strict";
 (self.webpackChunkneopyter = self.webpackChunkneopyter || []).push([
     [336], {
         336: (e, t, o) => {
             o.r(t), o.d(t, {
-                default: () => C
+                default: () => v
             });
-            var n = o(979),
-                s = o(228),
-                l = o(976),
-                r = o(933),
-                a = o(989),
-                c = o(743),
-                i = o(195),
+            var n = o(486),
+                s = o(597),
+                r = o(465),
+                l = o(372),
+                a = o(308),
+                c = o(618),
+                i = o(886),
                 d = o(502),
                 u = o(473);
             class p extends Error {
                 constructor(e) {
                     super(e), this.name = "RPCError"
                 }
             }
             const h = "https://github.com/msgpack-rpc/msgpack-rpc/blob/master/spec.md";
-            var g;
+            var y;
             ! function(e) {
                 e[e.Request = 0] = "Request", e[e.Response = 1] = "Response", e[e.Notification = 2] = "Notification"
-            }(g || (g = {}));
-            class y {
+            }(y || (y = {}));
+            class g {
                 constructor(e) {
                     this.dispatcher = e
                 }
                 start(e, ...t) {
                     this.transport = new e(this, ...t)
                 }
                 async dispatchMethod(e, t) {
                     if (!this.dispatcher[e.method]) {
                         const o = new p(`Method not found ${e.method}`);
-                        throw e.type === g.Request && t && t({
-                            type: g.Response,
+                        throw e.type === y.Request && t && t({
+                            type: y.Response,
                             msgid: e.msgid,
                             error: o,
                             result: void 0
                         }), o
                     }
                     try {
                         const o = await this.dispatcher[e.method](...e.params);
-                        e.type === g.Request && t && t({
-                            type: g.Response,
+                        e.type === y.Request && t && t({
+                            type: y.Response,
                             msgid: e.msgid,
                             result: o
                         })
                     } catch (o) {
-                        console.error(o), e.type === g.Request && t && t({
-                            type: g.Response,
+                        console.error(o), e.type === y.Request && t && t({
+                            type: y.Response,
                             msgid: e.msgid,
                             error: o
                         })
                     }
                 }
             }
             class m {
                 constructor(e) {
                     this.server = e
                 }
                 async onRequest(e) {
                     await this.server.dispatchMethod(e, (e => {
                         this.sendData(function(e) {
-                            return e.type === g.Request ? (0, u.encode)([e.type, e.msgid, e.method, e.params]) : e.type === g.Response ? (0, u.encode)([e.type, e.msgid, e.error ? e.error.toString() : void 0, e.result]) : (0, u.encode)([e.type, e.method, e.params])
+                            return e.type === y.Request ? (0, u.encode)([e.type, e.msgid, e.method, e.params]) : e.type === y.Response ? (0, u.encode)([e.type, e.msgid, e.error ? e.error.toString() : void 0, e.result]) : (0, u.encode)([e.type, e.method, e.params])
                         }(e))
                     }))
                 }
                 async onNotify(e) {
                     this.server.dispatchMethod(e)
                 }
             }
             class b extends m {
-                constructor(e, t) {
-                    super(e), this.url = t, this.websocket = new WebSocket(this.url), this.websocket.binaryType = "arraybuffer", this.readableStream = new ReadableStream({
-                        start: e => {
-                            this.websocket.addEventListener("open", (e => {
-                                this.onOpen(e)
-                            })), this.websocket.addEventListener("message", (t => {
-                                const o = function(e) {
-                                    const t = atob(e);
-                                    return Uint8Array.from(t, (e => e.codePointAt(0)))
-                                }(t.data);
-                                e.enqueue(o)
-                            })), this.websocket.addEventListener("error", (e => {
-                                throw this.onError(e), e
-                            })), this.websocket.addEventListener("close", (t => {
-                                this.onClose(t), e.close()
-                            }))
-                        }
-                    }), setTimeout((async () => {
+                constructor(e, t, o) {
+                    super(e), this.url = t, this.autoRetry = o, this.start()
+                }
+                async start() {
+                    try {
+                        this.websocket = new WebSocket(this.url), this.websocket.binaryType = "arraybuffer", this.readableStream = new ReadableStream({
+                            start: e => {
+                                this.websocket.addEventListener("open", (e => {
+                                    this.onOpen(e)
+                                })), this.websocket.addEventListener("message", (t => {
+                                    const o = function(e) {
+                                        const t = atob(e);
+                                        return Uint8Array.from(t, (e => e.codePointAt(0)))
+                                    }(t.data);
+                                    e.enqueue(o)
+                                })), this.websocket.addEventListener("error", (e => {
+                                    throw this.onError(e), e
+                                })), this.websocket.addEventListener("close", (t => {
+                                    this.onClose(t), e.close()
+                                }))
+                            }
+                        });
                         for await (const e of async function*(e) {
                             const t = (0, u.decodeMultiStream)(e);
                             for await (const e of t) {
                                 if (!Array.isArray(e) || 4 !== e.length && 3 !== e.length) throw new p(`Invalid msgpack-rpc message: ${JSON.stringify(e)}, please reference ${h}`);
                                 const t = e[0];
                                 if (0 !== t && 1 !== t && 2 !== t) throw new p(`Invalid msgpack-rpc message: ${JSON.stringify(e)}, please reference ${h}`);
-                                t === g.Request ? yield {
-                                    type: g.Request,
+                                t === y.Request ? yield {
+                                    type: y.Request,
                                     msgid: e[1],
                                     method: e[2],
                                     params: e[3]
-                                } : t === g.Response ? yield {
-                                    type: g.Response,
+                                } : t === y.Response ? yield {
+                                    type: y.Response,
                                     msgid: e[1],
                                     error: e[2],
                                     result: e[3]
                                 } : yield {
-                                    type: g.Notification,
+                                    type: y.Notification,
                                     method: e[1],
                                     params: e[2]
                                 }
                             }
                         }(this.readableStream)) this.onRead(e)
-                    }), 0)
+                    } catch (e) {
+                        throw console.error(e), this.checkRetry(), e
+                    }
                 }
                 async onRead(e) {
                     switch (e.type) {
-                        case g.Request:
+                        case y.Request:
                             await this.onRequest(e);
                             break;
-                        case g.Notification:
+                        case y.Notification:
                             await this.onNotify(e);
                             break;
                         default:
                             throw new p(`Unknown message: ${e}`)
                     }
                 }
                 sendData(e) {
@@ -137,208 +143,252 @@
                 onOpen(e) {
                     console.log(`Connection to neopyter jupyter server by websocket ${this.websocket.url}`)
                 }
                 onError(e) {
                     console.error("Websocket error", e)
                 }
                 onClose(e) {
-                    console.log(`DisConnection to neopyter jupyter server by websocket ${this.websocket.url}`)
+                    console.log(`Disconnect to neopyter jupyter server by websocket ${this.websocket.url}`), this.websocket.close(), this.websocket = void 0, this.readableStream = void 0, this.checkRetry()
+                }
+                checkRetry() {
+                    this.autoRetry && void 0 === this.websocket && (console.log("reconnect websocket server after 1s"), setTimeout((() => {
+                        this.autoRetry && void 0 === this.websocket ? this.start() : console.error("checkRetry repeat")
+                    }), 1e3))
                 }
             }
-            var w = o(153);
-            class k extends w.SidePanel {
+            var w = o(664);
+            class f extends w.SidePanel {
                 constructor(e) {
                     super(), this.settingRegistry = e, this.id = "neopyter-status-sidepanel", this.watchSettings()
                 }
                 async updatePanel() {
-                    const e = n.ServerConnection.makeSettings(),
-                        t = s.URLExt.join(e.baseUrl, "neopyter", "get_server_info"),
-                        o = await fetch(t);
-                    if (this.content.node.textContent = "", !o.ok) {
-                        const e = document.createElement("p");
-                        return this.content.node.appendChild(e), void(e.textContent = "Access API failed")
+                    const e = (await this.settingRegistry.load("neopyter:labplugin")).composite;
+                    this.content.node.textContent = "";
+                    {
+                        const t = document.createElement("h2");
+                        this.content.node.appendChild(t), t.textContent = `Work mode: ${e.mode}`
                     }
-                    const {
-                        code: l,
-                        message: r,
-                        data: a
-                    } = await o.json();
-                    if (0 !== l) {
-                        const e = document.createElement("p");
-                        return this.content.node.appendChild(e), void(e.textContent = r)
-                    }
-                    for (const e of a.addrs) {
-                        const t = document.createElement("p");
-                        this.content.node.appendChild(t), t.textContent = e
+                    if ("proxy" === e.mode) {
+                        const e = n.ServerConnection.makeSettings(),
+                            t = s.URLExt.join(e.baseUrl, "neopyter", "get_server_info"),
+                            o = await fetch(t);
+                        if (!o.ok) {
+                            const e = document.createElement("p");
+                            return this.content.node.appendChild(e), void(e.textContent = "Access API failed")
+                        }
+                        const {
+                            code: r,
+                            message: l,
+                            data: a
+                        } = await o.json();
+                        if (0 !== r) {
+                            const e = document.createElement("p");
+                            return this.content.node.appendChild(e), void(e.textContent = l)
+                        }
+                        for (const e of a.addrs) {
+                            const t = document.createElement("p");
+                            this.content.node.appendChild(t), t.textContent = e
+                        }
+                    } else {
+                        {
+                            const t = document.createElement("p");
+                            this.content.node.appendChild(t), t.textContent = `IP: ${e.ip}`
+                        } {
+                            const t = document.createElement("p");
+                            this.content.node.appendChild(t), t.textContent = `port: ${e.port}`
+                        }
                     }
                 }
                 async watchSettings() {
-                    let e = {};
-                    const t = async t => {
-                        e = t.composite, console.log("updateSettings", e);
+                    const e = async e => {
+                        const t = e.composite;
+                        console.log("updateSettings", t);
                         const o = n.ServerConnection.makeSettings(),
-                            l = o.baseUrl,
-                            r = s.URLExt.join(l, "neopyter", "update_settings"),
-                            a = await n.ServerConnection.makeRequest(r, {
+                            r = o.baseUrl,
+                            l = s.URLExt.join(r, "neopyter", "update_settings"),
+                            a = await n.ServerConnection.makeRequest(l, {
                                 method: "POST",
-                                body: JSON.stringify(e)
+                                body: JSON.stringify(t)
                             }, o);
                         console.log(await a.json()), this.updatePanel()
-                    }, o = await this.settingRegistry.load("neopyter:labplugin");
-                    o.changed.connect((() => {
-                        t(o)
-                    })), t(o)
+                    }, t = await this.settingRegistry.load("neopyter:labplugin");
+                    t.changed.connect((() => {
+                        e(t)
+                    })), e(t)
                 }
                 async restartServer() {}
             }
-            const f = new w.LabIcon({
+            const k = new w.LabIcon({
                     name: "neopyter:status-page",
                     svgstr: '<svg t="1704342603868" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="1462" width="200" height="200"><path d="M512.416 409.472a239.914667 239.914667 0 1 1 0 479.786667 239.914667 239.914667 0 0 1 0-479.786667zM6.645333 371.925333l128.853334 152.490667a27.264 27.264 0 0 0 38.954666 2.901333c208.426667-186.837333 468.053333-186.837333 675.84 0a27.392 27.392 0 0 0 39.082667-2.901333l128.256-152.490667a27.562667 27.562667 0 0 0-3.2-38.656c-302.933333-264.704-702.378667-264.704-1005.013333 0a27.733333 27.733333 0 0 0-2.773334 38.656z" p-id="1463"></path></svg>\n'
                 }),
-                C = [{
+                v = [{
                     id: "neopyter:labplugin",
                     description: "A JupyterLab extension.",
                     autoStart: !0,
-                    requires: [l.ILabShell, a.IDocumentManager, r.INotebookTracker, l.ILayoutRestorer, c.ISettingRegistry, i.ICompletionProviderManager],
-                    activate: (e, t, l, a, c, i, u) => {
+                    requires: [r.ILabShell, a.IDocumentManager, l.INotebookTracker, r.ILayoutRestorer, c.ISettingRegistry, i.ICompletionProviderManager],
+                    activate: (e, t, r, a, c, i, u) => {
                         const p = u,
                             h = p.getProviders();
                         console.log("JupyterLab extension neopyter is activated!"), console.log("provider", p.getProviders());
-                        const g = h.get("CompletionProvider:kernel"),
-                            m = new k(i);
-                        m.title.caption = "Neopyter", m.title.icon = f, e.shell.add(m, "right"), c && c.add(m, "@neopyter/graphsidebar");
-                        const w = n.ServerConnection.makeSettings(),
-                            C = s.URLExt.join(w.wsUrl, "neopyter", "channel");
-                        let v = a.currentWidget;
-                        t.currentChanged.connect((() => {
-                            t.currentWidget instanceof r.NotebookPanel && (v = t.currentWidget)
-                        }));
-                        const S = e => {
-                                var t;
-                                let o;
-                                e && (o = l.findWidget(e));
-                                let n = null == o ? void 0 : o.content;
-                                n || (null == v ? void 0 : v.isUntitled) && (o = v, n = o.content);
-                                const s = null === (t = null == n ? void 0 : n.model) || void 0 === t ? void 0 : t.sharedModel;
-                                if (!o || !s || !n) throw `Don't open ${e} and current don't select untitled ipynb`;
+                        const y = h.get("CompletionProvider:kernel"),
+                            m = new f(i);
+                        m.title.caption = "Neopyter", m.title.icon = k, e.shell.add(m, "right"), c && c.add(m, "@neopyter/graphsidebar");
+                        const w = e => {
+                                var o;
+                                let n;
+                                e && (n = r.findWidget(e));
+                                let s = null == n ? void 0 : n.content;
+                                if (!s) {
+                                    const e = t.currentWidget;
+                                    (null == e ? void 0 : e.isUntitled) && (n = e, s = n.content)
+                                }
+                                const l = null === (o = null == s ? void 0 : s.model) || void 0 === o ? void 0 : o.sharedModel;
+                                if (!n || !l || !s) throw `Don't open ${e} and current don't select untitled ipynb`;
                                 return {
-                                    notebookPanel: o,
-                                    notebook: n,
-                                    sharedModel: s
+                                    notebookPanel: n,
+                                    notebook: s,
+                                    sharedModel: l
                                 }
                             },
-                            R = (e, t) => {
+                            v = (e, t) => {
                                 const {
                                     notebook: o,
                                     sharedModel: n
-                                } = S(e), s = n.getCell(t);
+                                } = w(e), s = n.getCell(t);
                                 return {
                                     notebook: o,
                                     sharedNotebookModel: n,
                                     sharedModel: s
                                 }
                             },
-                            x = {
+                            C = {
                                 getVersion: async () => (await o.e(330).then(o.t.bind(o, 330, 19))).version,
                                 echo: e => `hello: ${e}`,
                                 executeCommand: async (t, o) => {
                                     await e.commands.execute(t, o)
                                 }
                             },
-                            M = {
+                            R = {
                                 getCurrentNotebook: () => {
-                                    const e = v;
+                                    const e = t.currentWidget;
                                     if (e) {
-                                        const t = l.contextForWidget(e);
+                                        const t = r.contextForWidget(e);
                                         return null == t ? void 0 : t.localPath
                                     }
                                 },
-                                isFileOpen: e => !!l.findWidget(e),
+                                isFileOpen: e => !!r.findWidget(e),
                                 isFileExist: async e => {
                                     try {
-                                        return !!await l.services.contents.get(e)
+                                        return !!await r.services.contents.get(e)
                                     } catch (e) {
                                         return e.response.status, console.log(e), !1
                                     }
                                 },
-                                createNew: (e, t, o) => l.createNew(e, t, o),
-                                openFile: e => !!l.open(e),
-                                openOrReveal: e => !!l.openOrReveal(e),
+                                createNew: (e, t, o) => r.createNew(e, t, o),
+                                openFile: e => !!r.open(e),
+                                openOrReveal: e => !!r.openOrReveal(e),
                                 activateNotebook: e => {
                                     const {
                                         notebookPanel: o
-                                    } = S(e);
-                                    t.activateById(o.id), o.node.focus(), v = o
+                                    } = w(e);
+                                    t.activateById(o.id), o.activate();
+                                    const n = e => {
+                                            const t = new FocusEvent("focus", {
+                                                bubbles: !0,
+                                                cancelable: !0,
+                                                view: window
+                                            });
+                                            e.click(), e.dispatchEvent(t), e.focus(),
+                                                function(e) {
+                                                    const t = "onfocusin" in e ? "focusin" : "focus",
+                                                        o = "onfocusin" in e;
+                                                    let n;
+                                                    "createEvent" in document ? (n = document.createEvent("Event"), n.initEvent(t, o, !0)) : "Event" in window && (n = new Event(t, {
+                                                        bubbles: o,
+                                                        cancelable: !0
+                                                    })), e.focus(), e.dispatchEvent(n)
+                                                }(e)
+                                        },
+                                        s = t._dockPanel;
+                                    for (const e of s.tabBars()) {
+                                        const t = e.titles.findIndex((e => e.owner === o));
+                                        if (t >= 0) {
+                                            n(e.contentNode.children[t]);
+                                            break
+                                        }
+                                    }
+                                    n(o.node)
                                 },
-                                closeFile: async e => await l.closeFile(e),
+                                closeFile: async e => await r.closeFile(e),
                                 selectAbove: () => {
                                     const {
                                         notebook: e
-                                    } = S();
-                                    e && r.NotebookActions.selectBelow(e)
+                                    } = w();
+                                    e && l.NotebookActions.selectBelow(e)
                                 },
                                 selectBelow: () => {
                                     const {
                                         notebook: e
-                                    } = S();
-                                    e && r.NotebookActions.selectBelow(e)
+                                    } = w();
+                                    e && l.NotebookActions.selectBelow(e)
                                 }
                             },
-                            N = {
-                                getCellNum: e => S(e).sharedModel.cells.length,
+                            S = {
+                                getCellNum: e => w(e).sharedModel.cells.length,
                                 setCellNum: (e, t) => {
                                     const {
                                         notebook: o,
                                         sharedModel: n
-                                    } = S(e), s = n.cells.length;
+                                    } = w(e), s = n.cells.length;
                                     if (t > s) n.insertCells(s, d.range(0, t - s).map((() => ({
                                         cell_type: o.notebookConfig.defaultCell,
                                         metadata: "code" === o.notebookConfig.defaultCell ? {
                                             trusted: !0
                                         } : {}
                                     }))));
                                     else
                                         for (; t < n.cells.length;) n.deleteCell(n.cells.length - 1)
                                 },
                                 getCell: (e, t) => {
                                     const {
                                         sharedModel: o
-                                    } = R(e, t);
+                                    } = v(e, t);
                                     return o.toJSON()
                                 },
-                                deleteCell: (e, t) => S(e).sharedModel.deleteCell(t),
+                                deleteCell: (e, t) => w(e).sharedModel.deleteCell(t),
                                 insertCell: (e, t) => {
                                     const {
                                         notebook: o,
                                         sharedModel: n
-                                    } = S(e);
+                                    } = w(e);
                                     return n.insertCell(t, {
                                         cell_type: o.notebookConfig.defaultCell,
                                         metadata: "code" === o.notebookConfig.defaultCell ? {
                                             trusted: !0
                                         } : {}
                                     })
                                 },
                                 activateCell: (e, t) => {
                                     const {
                                         notebook: o
-                                    } = S(e);
+                                    } = w(e);
                                     o.activeCellIndex = t
                                 },
                                 scrollToItem: (e, t, o, n) => {
                                     const {
                                         notebook: s
-                                    } = S(e);
+                                    } = w(e);
                                     s.scrollToItem(t, o, n)
                                 },
                                 fullSync: (e, t) => {
                                     const {
                                         notebook: o,
                                         sharedModel: n
-                                    } = S(e);
+                                    } = w(e);
                                     for (t.forEach(((e, t) => {
                                             const s = n.getCell(t);
                                             s ? void 0 === e.cell_type || s.cell_type === e.cell_type ? s.setSource(e.source) : (n.deleteCell(t), n.insertCell(t, {
                                                 cell_type: e.cell_type,
                                                 source: e.source,
                                                 metadata: s.getMetadata()
                                             })) : n.insertCell(t, {
@@ -349,93 +399,105 @@
                                                 } : {}
                                             })
                                         })); t.length < n.cells.length;) n.deleteCell(n.cells.length - 1)
                                 },
                                 partialSync: (e, t, o, n) => {
                                     const {
                                         notebook: s,
-                                        sharedModel: l
-                                    } = S(e);
-                                    for (console.log(`partialSync: current cell num:${l.cells.length}, from:${t}(include), to:${o}(include), update to cell num:${n.length}`), n.forEach(((e, n) => {
-                                            const r = n + t,
-                                                a = l.getCell(r);
-                                            r <= o && a ? void 0 === e.cell_type || a.cell_type === e.cell_type ? a.setSource(e.source) : (l.deleteCell(r), l.insertCell(r, {
+                                        sharedModel: r
+                                    } = w(e);
+                                    for (console.log(`partialSync: current cell num:${r.cells.length}, from:${t}(include), to:${o}(include), update to cell num:${n.length}`), n.forEach(((e, n) => {
+                                            const l = n + t,
+                                                a = r.getCell(l);
+                                            l <= o && a ? void 0 === e.cell_type || a.cell_type === e.cell_type ? a.setSource(e.source) : (r.deleteCell(l), r.insertCell(l, {
                                                 cell_type: e.cell_type,
                                                 source: e.source,
                                                 metadata: a.getMetadata()
-                                            })) : l.insertCell(r, {
+                                            })) : r.insertCell(l, {
                                                 cell_type: e.cell_type,
                                                 source: e.source,
                                                 metadata: "code" === s.notebookConfig.defaultCell ? {
                                                     trusted: !0
                                                 } : {}
                                             })
-                                        })); o - t + 1 > n.length;) l.deleteCell(o), o -= 1
+                                        })); o - t + 1 > n.length;) r.deleteCell(o), o -= 1
                                 },
                                 save: async e => {
                                     const {
                                         notebookPanel: t
-                                    } = S(e), o = l.contextForWidget(t);
+                                    } = w(e), o = r.contextForWidget(t);
                                     return null == o || o.path, await (null == o ? void 0 : o.save())
                                 },
                                 runSelectedCell: async t => await e.commands.execute("notebook:run-cell"),
                                 runAllAbove: async t => await e.commands.execute("notebook:run-all-above"),
                                 runAllBelow: async t => await e.commands.execute("notebook:run-all-below"),
                                 runAll: async t => await e.commands.execute("notebook:run-all-cells"),
                                 restartKernel: async e => {
                                     const {
                                         notebookPanel: t
-                                    } = S(e);
+                                    } = w(e);
                                     return await t.sessionContext.restartKernel()
                                 },
                                 restartRunAll: async t => {
                                     const {
                                         notebookPanel: o
-                                    } = S(t);
+                                    } = w(t);
                                     return await o.sessionContext.restartKernel(), await e.commands.execute("notebook:run-all-cells")
                                 },
                                 setMode: (e, t) => {
                                     const {
                                         notebookPanel: o
-                                    } = S(e);
+                                    } = w(e);
                                     o.content.mode = t
                                 },
                                 kernelComplete: async (e, t, o) => {
                                     const {
                                         notebookPanel: n
-                                    } = S(e);
+                                    } = w(e);
                                     console.log("kernelComplete:", t, o);
-                                    const s = await g.fetch({
+                                    const s = await y.fetch({
                                         text: t,
                                         offset: o
                                     }, {
                                         widget: n,
                                         session: n.sessionContext.session
                                     });
                                     return console.log(s), s.items
                                 }
                             },
-                            P = {
+                            x = {
                                 setCellSource: (e, t, o) => {
                                     const {
                                         sharedModel: n
-                                    } = R(e, t);
+                                    } = v(e, t);
                                     n.setSource(o)
                                 },
                                 setCellType: (e, t, o) => {
                                     const {
                                         sharedNotebookModel: n,
                                         sharedModel: s
-                                    } = R(e, t);
+                                    } = v(e, t);
                                     s.cell_type !== o && (n.deleteCell(t), n.insertCell(t, {
                                         cell_type: o,
                                         source: s.getSource(),
                                         metadata: s.getMetadata()
                                     }))
                                 }
                             };
-                        Object.assign(x, M), Object.assign(x, N), Object.assign(x, P), new y(x).start(b, C)
+                        Object.assign(C, R), Object.assign(C, S), Object.assign(C, x), (async () => {
+                            const e = new g(C),
+                                {
+                                    mode: t,
+                                    ip: o,
+                                    port: r
+                                } = (await i.load("neopyter:labplugin")).composite;
+                            let l;
+                            if ("proxy" === t) {
+                                const t = n.ServerConnection.makeSettings();
+                                l = s.URLExt.join(t.wsUrl, "neopyter", "channel"), e.start(b, l, !1)
+                            } else l = `ws://${o}:${r}`, e.start(b, l, !0)
+                        })()
                     }
                 }]
         }
     }
 ]);
```

### Comparing `neopyter-0.2.0/neopyter/labextension/static/7.8eb9a8e937e5deb3af13.js` & `neopyter-0.2.1/neopyter/labextension/static/7.8eb9a8e937e5deb3af13.js`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/neopyter/labextension/static/728.d85cbe66bc2da24c7357.js` & `neopyter-0.2.1/neopyter/labextension/static/728.d85cbe66bc2da24c7357.js`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/neopyter/labextension/static/769.477fd518dada39821aad.js` & `neopyter-0.2.1/neopyter/labextension/static/537.62c041ec63a28b9c91aa.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,376 +1,379 @@
 "use strict";
 (self.webpackChunkneopyter = self.webpackChunkneopyter || []).push([
-    [769], {
-        769: (n, r, t) => {
+    [537], {
+        537: (n, r, t) => {
             t.r(r), t.d(r, {
-                _setPath: () => Be,
-                add: () => i,
-                addProp: () => c,
-                allPass: () => l,
-                anyPass: () => v,
-                ceil: () => p,
-                chunk: () => g,
-                clamp: () => b,
-                clone: () => j,
+                _setPath: () => Ce,
+                add: () => o,
+                addProp: () => a,
+                allPass: () => s,
+                anyPass: () => y,
+                ceil: () => g,
+                chunk: () => x,
+                clamp: () => m,
+                clone: () => N,
                 compact: () => w,
-                concat: () => A,
-                conditional: () => k,
-                constant: () => B,
-                countBy: () => W,
-                createPipe: () => R,
-                debounce: () => F,
-                difference: () => K,
-                differenceWith: () => U,
-                divide: () => G,
-                doNothing: () => J,
-                drop: () => X,
-                dropFirstBy: () => vn,
-                dropLast: () => hn,
-                dropLastWhile: () => pn,
-                dropWhile: () => xn,
-                entries: () => mn,
-                equals: () => zn,
-                evolve: () => wn,
-                filter: () => Pn,
-                find: () => En,
-                findIndex: () => Wn,
-                findLast: () => Ln,
-                findLastIndex: () => Fn,
-                first: () => Kn,
-                firstBy: () => Un,
-                flatMap: () => Jn,
-                flatMapToObj: () => Xn,
-                flatten: () => Gn,
-                flattenDeep: () => Zn,
-                floor: () => rr,
-                forEach: () => tr,
-                forEachObj: () => ir,
-                fromEntries: () => fr,
-                fromKeys: () => ar,
-                fromPairs: () => sr,
-                groupBy: () => yr,
-                hasAtLeast: () => _,
-                hasSubObject: () => gr,
-                identity: () => br,
-                indexBy: () => mr,
-                intersection: () => Nr,
-                intersectionWith: () => Ar,
-                invert: () => Pr,
-                isArray: () => Sr,
-                isBoolean: () => Mr,
-                isDate: () => Er,
-                isDeepEqual: () => dr,
-                isDefined: () => Br,
-                isEmpty: () => Dr,
-                isError: () => qr,
-                isFunction: () => Lr,
-                isIncludedIn: () => Rr,
-                isNil: () => Fr,
-                isNonNull: () => Cr,
-                isNonNullish: () => Kr,
-                isNot: () => Vr,
-                isNullish: () => Ur,
-                isNumber: () => $r,
-                isObject: () => Tr,
-                isObjectType: () => Gr,
-                isPlainObject: () => Hr,
-                isPromise: () => Jr,
-                isString: () => Wr,
-                isSymbol: () => Qr,
-                isTruthy: () => N,
-                join: () => Xr,
-                keys: () => Zr,
-                last: () => _r,
-                length: () => rt,
-                map: () => et,
-                mapKeys: () => ot,
-                mapToObj: () => ct,
-                mapValues: () => lt,
-                mapWithFeedback: () => vt,
-                maxBy: () => pt,
-                meanBy: () => xt,
-                merge: () => mt,
-                mergeAll: () => jt,
-                mergeDeep: () => wt,
-                minBy: () => kt,
-                multiply: () => St,
-                noop: () => Et,
-                nthBy: () => Wt,
-                objOf: () => qt,
-                omit: () => Ct,
-                omitBy: () => Vt,
-                once: () => $t,
-                only: () => Gt,
-                partition: () => Jt,
-                pathOr: () => Xt,
-                pick: () => Zt,
-                pickBy: () => ne,
-                pipe: () => D,
-                piped: () => ee,
-                product: () => ue,
-                prop: () => oe,
-                pullObject: () => fe,
-                purry: () => u,
-                randomString: () => se,
-                range: () => he,
-                rankBy: () => pe,
-                reduce: () => xe,
-                reject: () => me,
-                reverse: () => je,
-                round: () => we,
-                sample: () => Ae,
-                set: () => ke,
-                setPath: () => Ee,
-                shuffle: () => Te,
-                sliceString: () => De,
-                sort: () => qe,
-                sortBy: () => Re,
-                sortedIndex: () => Ke,
-                sortedIndexBy: () => Ue,
-                sortedIndexWith: () => Ge,
-                sortedLastIndex: () => He,
-                sortedLastIndexBy: () => Qe,
-                splice: () => Ze,
-                splitAt: () => nu,
-                splitWhen: () => tu,
-                stringToPath: () => iu,
-                subtract: () => fu,
-                sum: () => au,
-                sumBy: () => vu,
-                swapIndices: () => yu,
-                swapProps: () => gu,
-                take: () => bu,
-                takeFirstBy: () => zu,
-                takeLastWhile: () => ju,
-                takeWhile: () => wu,
-                tap: () => Iu,
-                times: () => ae,
-                toPairs: () => jn,
-                type: () => z,
-                uniq: () => ku,
-                uniqBy: () => Mu,
-                uniqWith: () => Tu,
-                unique: () => qu,
-                uniqueBy: () => Ru,
-                uniqueWith: () => Ku,
-                values: () => $u,
-                zip: () => Gu,
-                zipObj: () => Ju,
-                zipWith: () => Xu
+                concat: () => I,
+                conditional: () => S,
+                constant: () => W,
+                countBy: () => q,
+                createPipe: () => C,
+                debounce: () => K,
+                difference: () => U,
+                differenceWith: () => G,
+                divide: () => J,
+                doNothing: () => X,
+                drop: () => Z,
+                dropFirstBy: () => hn,
+                dropLast: () => pn,
+                dropLastWhile: () => xn,
+                dropWhile: () => mn,
+                entries: () => On,
+                equals: () => jn,
+                evolve: () => In,
+                filter: () => Sn,
+                find: () => Tn,
+                findIndex: () => qn,
+                findLast: () => Fn,
+                findLastIndex: () => Kn,
+                first: () => Un,
+                firstBy: () => Gn,
+                flat: () => Qn,
+                flatMap: () => tr,
+                flatMapToObj: () => ur,
+                flatten: () => nr,
+                flattenDeep: () => or,
+                floor: () => ar,
+                forEach: () => lr,
+                forEachObj: () => yr,
+                fromEntries: () => dr,
+                fromKeys: () => gr,
+                fromPairs: () => br,
+                groupBy: () => zr,
+                hasAtLeast: () => rn,
+                hasSubObject: () => Ar,
+                identity: () => Ir,
+                indexBy: () => Pr,
+                intersection: () => Er,
+                intersectionWith: () => Tr,
+                invert: () => Dr,
+                isArray: () => Lr,
+                isBoolean: () => Rr,
+                isDate: () => Fr,
+                isDeepEqual: () => jr,
+                isDefined: () => Cr,
+                isEmpty: () => Ur,
+                isError: () => $r,
+                isFunction: () => Gr,
+                isIncludedIn: () => Hr,
+                isNil: () => Jr,
+                isNonNull: () => Qr,
+                isNonNullish: () => Xr,
+                isNot: () => Yr,
+                isNullish: () => Zr,
+                isNumber: () => _r,
+                isObject: () => Kr,
+                isObjectType: () => nt,
+                isPlainObject: () => rt,
+                isPromise: () => tt,
+                isString: () => Vr,
+                isSymbol: () => et,
+                isTruthy: () => A,
+                join: () => ut,
+                keys: () => ot,
+                last: () => ft,
+                length: () => at,
+                map: () => st,
+                mapKeys: () => ht,
+                mapToObj: () => pt,
+                mapValues: () => xt,
+                mapWithFeedback: () => mt,
+                maxBy: () => Nt,
+                meanBy: () => wt,
+                merge: () => Pt,
+                mergeAll: () => Mt,
+                mergeDeep: () => Bt,
+                minBy: () => qt,
+                multiply: () => Lt,
+                noop: () => Ft,
+                nthBy: () => Vt,
+                objOf: () => $t,
+                omit: () => Qt,
+                omitBy: () => Yt,
+                once: () => _t,
+                only: () => ne,
+                partition: () => te,
+                pathOr: () => ue,
+                pick: () => oe,
+                pickBy: () => ce,
+                pipe: () => L,
+                piped: () => se,
+                product: () => ve,
+                prop: () => he,
+                pullObject: () => de,
+                purry: () => i,
+                randomString: () => be,
+                range: () => Oe,
+                rankBy: () => Ne,
+                reduce: () => we,
+                reject: () => Pe,
+                reverse: () => Me,
+                round: () => Be,
+                sample: () => Te,
+                set: () => qe,
+                setPath: () => Fe,
+                shuffle: () => Ke,
+                sliceString: () => Ue,
+                sort: () => $e,
+                sortBy: () => He,
+                sortedIndex: () => Xe,
+                sortedIndexBy: () => Ze,
+                sortedIndexWith: () => nu,
+                sortedLastIndex: () => ru,
+                sortedLastIndexBy: () => eu,
+                splice: () => ou,
+                splitAt: () => cu,
+                splitWhen: () => lu,
+                stringToPath: () => yu,
+                subtract: () => du,
+                sum: () => gu,
+                sumBy: () => mu,
+                swapIndices: () => zu,
+                swapProps: () => Au,
+                take: () => Iu,
+                takeFirstBy: () => ku,
+                takeLastWhile: () => Mu,
+                takeWhile: () => Bu,
+                tap: () => Wu,
+                times: () => ge,
+                toPairs: () => An,
+                type: () => O,
+                uniq: () => qu,
+                uniqBy: () => Ru,
+                uniqWith: () => Ku,
+                unique: () => $u,
+                uniqueBy: () => Hu,
+                uniqueWith: () => Xu,
+                values: () => _u,
+                zip: () => ni,
+                zipObj: () => ti,
+                zipWith: () => ui
             });
             var e = function(n, r, t) {
                 if (t || 2 === arguments.length)
                     for (var e, u = 0, i = r.length; u < i; u++) !e && u in r || (e || (e = Array.prototype.slice.call(r, 0, u)), e[u] = r[u]);
                 return n.concat(e || Array.prototype.slice.call(r))
             };
 
             function u(n, r, t) {
-                var u = Array.from(r),
-                    i = n.length - r.length;
-                if (0 === i) return n.apply(void 0, u);
-                if (1 === i) {
-                    var o = function(r) {
-                            return n.apply(void 0, e([r], u, !1))
-                        },
-                        f = null != t ? t : n.lazy;
-                    return void 0 === f ? o : Object.assign(o, {
-                        lazy: f,
-                        lazyArgs: r
-                    })
-                }
+                var u = function(t) {
+                        return n.apply(void 0, e([t], Array.from(r), !1))
+                    },
+                    i = null != t ? t : n.lazy;
+                return void 0 === i ? u : Object.assign(u, {
+                    lazy: i,
+                    lazyArgs: r
+                })
+            }
+
+            function i(n, r, t) {
+                var e = n.length - r.length;
+                if (0 === e) return n.apply(void 0, Array.from(r));
+                if (1 === e) return u(n, r, t);
                 throw new Error("Wrong number of arguments")
             }
 
-            function i() {
-                return u(o, arguments)
+            function o() {
+                return i(f, arguments)
             }
 
-            function o(n, r) {
+            function f(n, r) {
                 return n + r
             }
-            var f = function() {
-                return f = Object.assign || function(n) {
+            var c = function() {
+                return c = Object.assign || function(n) {
                     for (var r, t = 1, e = arguments.length; t < e; t++)
                         for (var u in r = arguments[t]) Object.prototype.hasOwnProperty.call(r, u) && (n[u] = r[u]);
                     return n
-                }, f.apply(this, arguments)
+                }, c.apply(this, arguments)
             };
 
-            function c() {
-                return u(a, arguments)
+            function a() {
+                return i(l, arguments)
             }
 
-            function a(n, r, t) {
+            function l(n, r, t) {
                 var e;
-                return f(f({}, n), ((e = {})[r] = t, e))
+                return c(c({}, n), ((e = {})[r] = t, e))
             }
 
-            function l() {
-                return u(s, arguments)
+            function s() {
+                return i(v, arguments)
             }
 
-            function s(n, r) {
+            function v(n, r) {
                 return r.every((function(r) {
                     return r(n)
                 }))
             }
 
-            function v() {
-                return u(y, arguments)
+            function y() {
+                return i(h, arguments)
             }
 
-            function y(n, r) {
+            function h(n, r) {
                 return r.some((function(r) {
                     return r(n)
                 }))
             }
-            var h = 15;
+            var d = 15;
 
-            function d(n) {
+            function p(n) {
                 return function(r, t) {
                     if (0 === t) return n(r);
                     if (!Number.isInteger(t)) throw new TypeError("precision must be an integer: ".concat(t));
-                    if (t > h || t < -h) throw new RangeError("precision must be between -15 and 15");
+                    if (t > d || t < -d) throw new RangeError("precision must be between -15 and 15");
                     if (Number.isNaN(r) || !Number.isFinite(r)) return n(r);
                     var e = Math.pow(10, t);
                     return n(r * e) / e
                 }
             }
 
-            function p() {
-                return u(d(Math.ceil), arguments)
+            function g() {
+                return i(p(Math.ceil), arguments)
             }
 
-            function g() {
-                return u(x, arguments)
+            function x() {
+                return i(b, arguments)
             }
 
-            function x(n, r) {
+            function b(n, r) {
                 for (var t = [], e = 0; e < n.length; e += r) t.push(n.slice(e, e + r));
                 return t
             }
 
-            function b() {
-                return u(m, arguments)
+            function m() {
+                return i(z, arguments)
             }
 
-            function m(n, r) {
+            function z(n, r) {
                 var t = r.min,
                     e = r.max;
                 return void 0 !== t && n < t ? t : void 0 !== e && n > e ? e : n
             }
 
-            function z(n) {
+            function O(n) {
                 return null === n ? "Null" : void 0 === n ? "Undefined" : Object.prototype.toString.call(n).slice(8, -1)
             }
 
-            function O(n, r, t, e) {
+            function j(n, r, t, e) {
                 function u(u) {
                     for (var i = r.length, o = 0; o < i;) {
                         if (n === r[o]) return t[o];
                         o += 1
                     }
-                    for (var f in r[o + 1] = n, t[o + 1] = u, n) u[f] = e ? O(n[f], r, t, !0) : n[f];
+                    for (var f in r[o + 1] = n, t[o + 1] = u, n) u[f] = e ? j(n[f], r, t, !0) : n[f];
                     return u
                 }
-                switch (z(n)) {
+                switch (O(n)) {
                     case "Object":
                         return u({});
                     case "Array":
                         return u([]);
                     case "Date":
                         return new Date(n.valueOf());
                     case "RegExp":
                         return i = n, new RegExp(i.source, (i.global ? "g" : "") + (i.ignoreCase ? "i" : "") + (i.multiline ? "m" : "") + (i.sticky ? "y" : "") + (i.unicode ? "u" : ""));
                     default:
                         return n
                 }
                 var i
             }
 
-            function j(n) {
-                return null != n && "function" == typeof n.clone ? n.clone() : O(n, [], [], !0)
+            function N(n) {
+                return null != n && "function" == typeof n.clone ? n.clone() : j(n, [], [], !0)
             }
 
-            function N(n) {
+            function A(n) {
                 return Boolean(n)
             }
 
             function w(n) {
-                return n.filter(N)
+                return n.filter(A)
             }
 
-            function A() {
-                return u(I, arguments)
+            function I() {
+                return i(P, arguments)
             }
 
-            function I(n, r) {
+            function P(n, r) {
                 return n.concat(r)
             }
-            var P = function(n, r, t) {
+            var k = function(n, r, t) {
                 if (t || 2 === arguments.length)
                     for (var e, u = 0, i = r.length; u < i; u++) !e && u in r || (e || (e = Array.prototype.slice.call(r, 0, u)), e[u] = r[u]);
                 return n.concat(e || Array.prototype.slice.call(r))
             };
 
-            function k() {
-                return n = M, r = S, t = arguments, e = Array.from(t), n(t[0]) ? function(n) {
-                    return r.apply(void 0, P([n], e, !1))
+            function S() {
+                return n = E, r = M, t = arguments, e = Array.from(t), n(t[0]) ? function(n) {
+                    return r.apply(void 0, k([n], e, !1))
                 } : r.apply(void 0, e);
                 var n, r, t, e
             }
 
-            function S(n) {
+            function M(n) {
                 for (var r = [], t = 1; t < arguments.length; t++) r[t - 1] = arguments[t];
                 for (var e = 0, u = r; e < u.length; e++) {
                     var i = u[e],
                         o = i[0],
                         f = i[1];
                     if (o(n)) return f(n)
                 }
                 throw new Error("conditional: data failed for all cases")
             }
 
-            function M(n) {
+            function E(n) {
                 if (!Array.isArray(n)) return !1;
                 var r = n,
                     t = r[0],
                     e = r[1],
                     u = r.slice(2);
                 return "function" == typeof t && t.length <= 1 && "function" == typeof e && e.length <= 1 && 0 === u.length
             }! function(n) {
                 n.defaultCase = function(n) {
-                    return void 0 === n && (n = E), [function() {
-                        return !0
-                    }, n]
+                    return void 0 === n && (n = T), [B, n]
                 }
-            }(k || (k = {}));
-            var E = function() {};
+            }(S || (S = {}));
+            var B = function() {
+                    return !0
+                },
+                T = function() {};
 
-            function B(n) {
+            function W(n) {
                 return function() {
                     return n
                 }
             }
-            var T = function(n) {
+            var D = function(n) {
                 return function(r, t) {
                     for (var e = 0, u = 0; u < r.length; u++) {
                         var i = r[u];
                         e += (n ? t(i, u, r) : t(i)) ? 1 : 0
                     }
                     return e
                 }
             };
 
-            function W() {
-                return u(T(!1), arguments)
+            function q() {
+                return i(D(!1), arguments)
             }
 
-            function D(n) {
+            function L(n) {
                 for (var r, t = [], e = 1; e < arguments.length; e++) t[e - 1] = arguments[e];
                 for (var u, i = n, o = t.map((function(n) {
                         return "lazy" in n ? function(n) {
                             var r = n.lazy,
                                 t = n.lazyArgs,
                                 e = r.apply(void 0, null != t ? t : []);
                             return Object.assign(e, {
@@ -386,63 +389,63 @@
                             var l = o[a];
                             if (void 0 === l) break;
                             if (c.push(l), l.isSingle) break
                         }
                         for (var s = [], v = i[Symbol.iterator]();;) {
                             var y = v.next();
                             if (null !== (r = y.done) && void 0 !== r && r) break;
-                            if (q(y.value, s, c)) break
+                            if (R(y.value, s, c)) break
                         }
                         i = c[c.length - 1].isSingle ? s[0] : s, f += c.length
                     } else i = (0, t[f])(i), f += 1;
                 return i
             }
 
-            function q(n, r, t) {
+            function R(n, r, t) {
                 var e;
                 if (0 === t.length) return r.push(n), !1;
                 for (var u = n, i = {
                         done: !1,
                         hasNext: !1
                     }, o = !1, f = 0; f < t.length; f++) {
                     var c = t[f],
                         a = c.isIndexed,
                         l = c.index,
                         s = c.items;
                     if (s.push(u), i = a ? c(u, l, s) : c(u), c.index += 1, i.hasNext) {
                         if (null !== (e = i.hasMany) && void 0 !== e && e) {
                             for (var v = 0, y = i.next; v < y.length; v++)
-                                if (q(y[v], r, t.slice(f + 1))) return !0;
+                                if (R(y[v], r, t.slice(f + 1))) return !0;
                             return !1
                         }
                         u = i.next
                     }
                     if (!i.hasNext) break;
                     i.done && (o = !0)
                 }
                 return i.hasNext && r.push(u), !!o
             }! function(n) {
                 n.indexed = function() {
-                    return u(T(!0), arguments)
+                    return i(D(!0), arguments)
                 }
-            }(W || (W = {}));
-            var L = function(n, r, t) {
+            }(q || (q = {}));
+            var F = function(n, r, t) {
                 if (t || 2 === arguments.length)
                     for (var e, u = 0, i = r.length; u < i; u++) !e && u in r || (e || (e = Array.prototype.slice.call(r, 0, u)), e[u] = r[u]);
                 return n.concat(e || Array.prototype.slice.call(r))
             };
 
-            function R() {
+            function C() {
                 for (var n = [], r = 0; r < arguments.length; r++) n[r] = arguments[r];
                 return function(r) {
-                    return D.apply(void 0, L([r], n, !1))
+                    return L.apply(void 0, F([r], n, !1))
                 }
             }
 
-            function F(n, r) {
+            function K(n, r) {
                 var t, e, u, i, o = r.waitMs,
                     f = r.timing,
                     c = void 0 === f ? "trailing" : f,
                     a = r.maxWaitMs;
                 if (void 0 !== a && void 0 !== o && a < o) throw new Error("debounce: maxWaitMs (".concat(a, ") cannot be less than waitMs (").concat(o, ")"));
                 var l = function() {
                         if (void 0 !== u) {
@@ -489,85 +492,85 @@
                     },
                     get cachedValue() {
                         return i
                     }
                 }
             }
 
-            function C(n, r, t) {
+            function V(n, r, t) {
                 void 0 === t && (t = !1);
                 for (var e = [], u = 0; u < n.length; u++) {
                     var i = n[u],
                         o = t ? r(i, u, n) : r(i);
                     if (!0 === o.hasMany ? e.push.apply(e, o.next) : o.hasNext && e.push(o.next), o.done) break
                 }
                 return e
             }
 
-            function K() {
-                return u(V, arguments, K.lazy)
+            function U() {
+                return i($, arguments, U.lazy)
             }
 
-            function V(n, r) {
-                return C(n, K.lazy(r))
+            function $(n, r) {
+                return V(n, U.lazy(r))
             }
 
-            function U() {
-                return u($, arguments, U.lazy)
+            function G() {
+                return i(H, arguments, G.lazy)
             }
 
-            function $(n, r, t) {
-                return C(n, U.lazy(r, t))
+            function H(n, r, t) {
+                return V(n, G.lazy(r, t))
             }
 
-            function G() {
-                return u(H, arguments)
+            function J() {
+                return i(Q, arguments)
             }
 
-            function H(n, r) {
+            function Q(n, r) {
                 return n / r
             }
 
-            function J() {
-                return Q
+            function X() {
+                return Y
             }
 
-            function Q() {}
+            function Y() {}
 
-            function X() {
-                return u(Y, arguments, X.lazy)
+            function Z() {
+                return i(_, arguments, Z.lazy)
             }
 
-            function Y(n, r) {
-                return C(n, X.lazy(r))
+            function _(n, r) {
+                return V(n, Z.lazy(r))
             }
 
-            function Z(n, r, t) {
+            function nn(n, r, t) {
                 var e;
                 e = [n[t], n[r]], n[r] = e[0], n[t] = e[1]
             }
 
-            function _() {
+            function rn() {
                 for (var n = [], r = 0; r < arguments.length; r++) n[r] = arguments[r];
-                return u(nn, n)
+                return i(tn, n)
             }! function(n) {
                 n.lazy = function(n) {
                     var r = new Set(n);
                     return function(n) {
                         return r.has(n) ? {
                             done: !1,
                             hasNext: !1
                         } : {
                             done: !1,
                             hasNext: !0,
                             next: n
                         }
                     }
                 }
-            }(K || (K = {})),
+            }(U || (U = {})),
             function(n) {
                 n.lazy = function(n, r) {
                     return function(t) {
                         return n.every((function(n) {
                             return !r(t, n)
                         })) ? {
                             done: !1,
@@ -575,184 +578,184 @@
                             next: t
                         } : {
                             done: !1,
                             hasNext: !1
                         }
                     }
                 }
-            }(U || (U = {})),
+            }(G || (G = {})),
             function(n) {
                 n.lazy = function(n) {
                     var r = n;
                     return function(n) {
                         return r > 0 ? (r -= 1, {
                             done: !1,
                             hasNext: !1
                         }) : {
                             done: !1,
                             hasNext: !0,
                             next: n
                         }
                     }
                 }
-            }(X || (X = {}));
-            var nn = function(n, r) {
+            }(Z || (Z = {}));
+            var tn = function(n, r) {
                 return n.length >= r
             };
 
-            function rn(n, r) {
-                for (var t = Math.floor(n.length / 2) - 1; t >= 0; t--) en(n, t, r)
+            function en(n, r) {
+                for (var t = Math.floor(n.length / 2) - 1; t >= 0; t--) on(n, t, r)
             }
 
-            function tn(n, r, t) {
-                if (_(n, 1)) {
+            function un(n, r, t) {
+                if (rn(n, 1)) {
                     var e = n[0];
-                    if (!(r(t, e) >= 0)) return n[0] = t, en(n, 0, r), e
+                    if (!(r(t, e) >= 0)) return n[0] = t, on(n, 0, r), e
                 }
             }
 
-            function en(n, r, t) {
+            function on(n, r, t) {
                 for (var e = r; 2 * e + 1 < n.length;) {
                     var u = 2 * e + 1,
                         i = t(n[e], n[u]) < 0 ? u : e,
                         o = u + 1;
                     if (o < n.length && t(n[i], n[o]) < 0 && (i = o), i === e) return;
-                    Z(n, e, i), e = i
+                    nn(n, e, i), e = i
                 }
             }
-            var un = function(n, r, t) {
+            var fn = function(n, r, t) {
                     if (t || 2 === arguments.length)
                         for (var e, u = 0, i = r.length; u < i; u++) !e && u in r || (e || (e = Array.prototype.slice.call(r, 0, u)), e[u] = r[u]);
                     return n.concat(e || Array.prototype.slice.call(r))
                 },
-                on = {
+                cn = {
                     asc: function(n, r) {
                         return n > r
                     },
                     desc: function(n, r) {
                         return n < r
                     }
                 };
 
-            function fn(n, r) {
+            function an(n, r) {
                 var t = Array.isArray(r) ? r : Array.from(r),
                     e = t[0],
                     u = t.slice(1);
-                if (!ln(e)) {
-                    var i = an.apply(void 0, u);
+                if (!vn(e)) {
+                    var i = sn.apply(void 0, u);
                     return n(e, i)
                 }
-                var o = an.apply(void 0, un([e], u, !1));
+                var o = sn.apply(void 0, fn([e], u, !1));
                 return function(r) {
                     return n(r, o)
                 }
             }
 
-            function cn(n, r) {
+            function ln(n, r) {
                 var t, e, u = Array.from(r),
                     i = u[0],
                     o = u[1],
                     f = u.slice(2);
-                return ln(o) ? (t = i, e = un([o], f, !0)) : (t = o, e = un([i], f, !0)), fn((function() {
+                return vn(o) ? (t = i, e = fn([o], f, !0)) : (t = o, e = fn([i], f, !0)), an((function() {
                     for (var r = [], e = 0; e < arguments.length; e++) r[e] = arguments[e];
-                    return n.apply(void 0, un(un([], r, !1), [t], !1))
+                    return n.apply(void 0, fn(fn([], r, !1), [t], !1))
                 }), e)
             }
 
-            function an(n, r) {
+            function sn(n, r) {
                 for (var t = [], e = 2; e < arguments.length; e++) t[e - 2] = arguments[e];
                 var u = "function" == typeof n ? n : n[0],
                     i = "function" == typeof n ? "asc" : n[1],
-                    o = on[i],
-                    f = void 0 === r ? void 0 : an.apply(void 0, un([r], t, !1));
+                    o = cn[i],
+                    f = void 0 === r ? void 0 : sn.apply(void 0, fn([r], t, !1));
                 return function(n, r) {
                     var t, e = u(n),
                         i = u(r);
                     return o(e, i) ? 1 : o(i, e) ? -1 : null !== (t = null == f ? void 0 : f(n, r)) && void 0 !== t ? t : 0
                 }
             }
 
-            function ln(n) {
-                if (sn(n)) return !0;
+            function vn(n) {
+                if (yn(n)) return !0;
                 if ("object" != typeof n || !Array.isArray(n)) return !1;
                 var r = n,
                     t = r[0],
                     e = r[1],
                     u = r.slice(2);
-                return sn(t) && "string" == typeof e && e in on && 0 === u.length
+                return yn(t) && "string" == typeof e && e in cn && 0 === u.length
             }
-            var sn = function(n) {
+            var yn = function(n) {
                 return "function" == typeof n && 1 === n.length
             };
 
-            function vn() {
-                return cn(yn, arguments)
+            function hn() {
+                return ln(dn, arguments)
             }
 
-            function yn(n, r, t) {
+            function dn(n, r, t) {
                 if (t >= n.length) return [];
                 if (t <= 0) return n.slice();
                 var e = n.slice(0, t);
-                rn(e, r);
+                en(e, r);
                 for (var u = [], i = 0, o = n.slice(t); i < o.length; i++) {
                     var f = o[i],
-                        c = tn(e, r, f);
+                        c = un(e, r, f);
                     u.push(null != c ? c : f)
                 }
                 return u
             }
 
-            function hn() {
-                return u(dn, arguments)
+            function pn() {
+                return i(gn, arguments)
             }
 
-            function dn(n, r) {
+            function gn(n, r) {
                 var t = n.slice();
                 return r > 0 && t.splice(-r), t
             }
 
-            function pn() {
-                return u(gn, arguments)
+            function xn() {
+                return i(bn, arguments)
             }
 
-            function gn(n, r) {
+            function bn(n, r) {
                 for (var t = n.length - 1; t >= 0; t--)
                     if (!r(n[t])) return n.slice(0, t + 1);
                 return []
             }
 
-            function xn() {
-                return u(bn, arguments)
+            function mn() {
+                return i(zn, arguments)
             }
 
-            function bn(n, r) {
+            function zn(n, r) {
                 for (var t = 0; t < n.length; t++)
                     if (!r(n[t])) return n.slice(t);
                 return []
             }
 
-            function mn() {
-                return u(Object.entries, arguments)
+            function On() {
+                return i(Object.entries, arguments)
             }
 
-            function zn() {
-                return u(On, arguments)
+            function jn() {
+                return i(Nn, arguments)
             }
 
-            function On(n, r) {
+            function Nn(n, r) {
                 if (n === r) return !0;
                 if ("number" == typeof n && "number" == typeof r) return n != n && r != r;
                 if ("object" != typeof n || "object" != typeof r) return !1;
                 if (null === n || null === r) return !1;
                 var t = Array.isArray(n),
                     e = Array.isArray(r);
                 if (t && e) {
                     if (n.length !== r.length) return !1;
                     for (var u = 0; u < n.length; u++)
-                        if (!On(n[u], r[u])) return !1;
+                        if (!Nn(n[u], r[u])) return !1;
                     return !0
                 }
                 if (t !== e) return !1;
                 var i = n instanceof Date,
                     o = r instanceof Date;
                 if (i && o) return n.getTime() === r.getTime();
                 if (i !== o) return !1;
@@ -761,64 +764,64 @@
                 if (f && c) return n.toString() === r.toString();
                 if (f !== c) return !1;
                 var a = Object.keys(n);
                 if (a.length !== Object.keys(r).length) return !1;
                 for (var l = 0, s = a; l < s.length; l++) {
                     var v = s[l];
                     if (!Object.prototype.hasOwnProperty.call(r, v)) return !1;
-                    if (!On(n[v], r[v])) return !1
+                    if (!Nn(n[v], r[v])) return !1
                 }
                 return !0
             }
 
-            function jn() {
-                return u(Object.entries, arguments)
+            function An() {
+                return i(Object.entries, arguments)
             }! function(n) {
                 n.strict = n
-            }(mn || (mn = {})),
+            }(On || (On = {})),
             function(n) {
                 n.strict = n
-            }(jn || (jn = {}));
-            var Nn = function() {
-                return Nn = Object.assign || function(n) {
+            }(An || (An = {}));
+            var wn = function() {
+                return wn = Object.assign || function(n) {
                     for (var r, t = 1, e = arguments.length; t < e; t++)
                         for (var u in r = arguments[t]) Object.prototype.hasOwnProperty.call(r, u) && (n[u] = r[u]);
                     return n
-                }, Nn.apply(this, arguments)
+                }, wn.apply(this, arguments)
             };
 
-            function wn() {
-                return u(An, arguments)
+            function In() {
+                return i(Pn, arguments)
             }
 
-            function An(n, r) {
+            function Pn(n, r) {
                 if ("object" != typeof n || null === n) return n;
-                for (var t = Nn({}, n), e = 0, u = jn.strict(r); e < u.length; e++) {
+                for (var t = wn({}, n), e = 0, u = An.strict(r); e < u.length; e++) {
                     var i = u[e],
                         o = i[0],
                         f = i[1];
-                    o in t && (t[o] = "function" == typeof f ? f(t[o]) : An(t[o], f))
+                    o in t && (t[o] = "function" == typeof f ? f(t[o]) : Pn(t[o], f))
                 }
                 return t
             }
-            var In = function(n) {
+            var kn = function(n) {
                 return Object.assign(n, {
                     indexed: !0
                 })
             };
 
-            function Pn() {
-                return u(kn(!1), arguments, Pn.lazy)
+            function Sn() {
+                return i(Mn(!1), arguments, Sn.lazy)
             }
-            var kn = function(n) {
+            var Mn = function(n) {
                     return function(r, t) {
-                        return C(r, n ? Pn.lazyIndexed(t) : Pn.lazy(t), n)
+                        return V(r, n ? Sn.lazyIndexed(t) : Sn.lazy(t), n)
                     }
                 },
-                Sn = function(n) {
+                En = function(n) {
                     return function(r) {
                         return function(t, e, u) {
                             return (n ? r(t, e, u) : r(t)) ? {
                                 done: !1,
                                 hasNext: !0,
                                 next: t
                             } : {
@@ -826,63 +829,63 @@
                                 hasNext: !1
                             }
                         }
                     }
                 };
             ! function(n) {
                 n.indexed = function() {
-                    return u(kn(!0), arguments, n.lazyIndexed)
-                }, n.lazy = Sn(!1), n.lazyIndexed = In(Sn(!0))
-            }(Pn || (Pn = {}));
-            var Mn = function(n) {
+                    return i(Mn(!0), arguments, n.lazyIndexed)
+                }, n.lazy = En(!1), n.lazyIndexed = kn(En(!0))
+            }(Sn || (Sn = {}));
+            var Bn = function(n) {
                 return Object.assign(n, {
                     single: !0
                 })
             };
 
-            function En() {
-                return u(Bn(!1), arguments, En.lazy)
+            function Tn() {
+                return i(Wn(!1), arguments, Tn.lazy)
             }
-            var Bn = function(n) {
+            var Wn = function(n) {
                     return function(r, t) {
                         return r.find((function(r, e, u) {
                             return n ? t(r, e, u) : t(r)
                         }))
                     }
                 },
-                Tn = function(n) {
+                Dn = function(n) {
                     return function(r) {
                         return function(t, e, u) {
                             return (n ? r(t, e, u) : r(t)) ? {
                                 done: !0,
                                 hasNext: !0,
                                 next: t
                             } : {
                                 done: !1,
                                 hasNext: !1
                             }
                         }
                     }
                 };
 
-            function Wn() {
-                return u(Dn(!1), arguments, Wn.lazy)
+            function qn() {
+                return i(Ln(!1), arguments, qn.lazy)
             }! function(n) {
                 n.indexed = function() {
-                    return u(Bn(!0), arguments, n.lazyIndexed)
-                }, n.lazy = Mn(Tn(!1)), n.lazyIndexed = Mn(In(Tn(!0)))
-            }(En || (En = {}));
-            var Dn = function(n) {
+                    return i(Wn(!0), arguments, n.lazyIndexed)
+                }, n.lazy = Bn(Dn(!1)), n.lazyIndexed = Bn(kn(Dn(!0)))
+            }(Tn || (Tn = {}));
+            var Ln = function(n) {
                     return function(r, t) {
                         return r.findIndex((function(r, e, u) {
                             return n ? t(r, e, u) : t(r)
                         }))
                     }
                 },
-                qn = function(n) {
+                Rn = function(n) {
                     return function(r) {
                         var t = 0;
                         return function(e, u, i) {
                             return (n ? r(e, u, i) : r(e)) ? {
                                 done: !0,
                                 hasNext: !0,
                                 next: t
@@ -890,120 +893,166 @@
                                 done: !1,
                                 hasNext: !1
                             })
                         }
                     }
                 };
 
-            function Ln() {
-                return u(Rn(!1), arguments)
+            function Fn() {
+                return i(Cn(!1), arguments)
             }! function(n) {
                 n.indexed = function() {
-                    return u(Dn(!0), arguments, n.lazyIndexed)
-                }, n.lazy = Mn(qn(!1)), n.lazyIndexed = Mn(In(qn(!0)))
-            }(Wn || (Wn = {}));
-            var Rn = function(n) {
+                    return i(Ln(!0), arguments, n.lazyIndexed)
+                }, n.lazy = Bn(Rn(!1)), n.lazyIndexed = Bn(kn(Rn(!0)))
+            }(qn || (qn = {}));
+            var Cn = function(n) {
                 return function(r, t) {
                     for (var e = r.length - 1; e >= 0; e--)
                         if (n ? t(r[e], e, r) : t(r[e])) return r[e]
                 }
             };
 
-            function Fn() {
-                return u(Cn(!1), arguments)
+            function Kn() {
+                return i(Vn(!1), arguments)
             }! function(n) {
                 n.indexed = function() {
-                    return u(Rn(!0), arguments)
+                    return i(Cn(!0), arguments)
                 }
-            }(Ln || (Ln = {}));
-            var Cn = function(n) {
+            }(Fn || (Fn = {}));
+            var Vn = function(n) {
                 return function(r, t) {
                     for (var e = r.length - 1; e >= 0; e--)
                         if (n ? t(r[e], e, r) : t(r[e])) return e;
                     return -1
                 }
             };
 
-            function Kn() {
-                return u(Vn, arguments, Kn.lazy)
+            function Un() {
+                return i($n, arguments, Un.lazy)
             }
 
-            function Vn(n) {
+            function $n(n) {
                 return n[0]
             }
 
-            function Un() {
-                return fn($n, arguments)
+            function Gn() {
+                return an(Hn, arguments)
             }
 
-            function $n(n, r) {
-                if (!_(n, 2)) return n[0];
+            function Hn(n, r) {
+                if (!rn(n, 2)) return n[0];
                 for (var t = n[0], e = 0, u = n.slice(1); e < u.length; e++) {
                     var i = u[e];
                     r(i, t) < 0 && (t = i)
                 }
                 return t
-            }
-
-            function Gn() {
-                return u(Hn, arguments, Gn.lazy)
-            }
-
-            function Hn(n) {
-                return C(n, Gn.lazy())
-            }
-
-            function Jn() {
-                return u(Qn, arguments, Jn.lazy)
-            }
-
-            function Qn(n, r) {
-                return Gn(n.map((function(n) {
-                    return r(n)
-                })))
-            }
-
-            function Xn() {
-                return u(Yn(!1), arguments)
             }! function(n) {
                 n.indexed = function() {
-                    return u(Cn(!0), arguments)
+                    return i(Vn(!0), arguments)
                 }
-            }(Fn || (Fn = {})),
+            }(Kn || (Kn = {})),
             function(n) {
                 function r() {
                     return function(n) {
                         return {
                             done: !0,
                             hasNext: !0,
                             next: n
                         }
                     }
                 }
                 n.lazy = r,
                     function(n) {
                         n.single = !0
                     }(r = n.lazy || (n.lazy = {}))
-            }(Kn || (Kn = {})),
-            function(n) {
+            }(Un || (Un = {}));
+            var Jn = 1;
+
+            function Qn(n, r) {
+                return "object" == typeof n ? _n(n, r) : u(_n, arguments, Xn)
+            }
+            var Xn = function(n) {
+                    return void 0 === n && (n = Jn), n <= 0 ? Yn : 1 === n ? Zn : function(r) {
+                        return Array.isArray(r) ? {
+                            next: _n(r, n - 1),
+                            hasNext: !0,
+                            hasMany: !0,
+                            done: !1
+                        } : {
+                            next: r,
+                            hasNext: !0,
+                            done: !1
+                        }
+                    }
+                },
+                Yn = function(n) {
+                    return {
+                        next: n,
+                        hasNext: !0,
+                        done: !1
+                    }
+                },
+                Zn = function(n) {
+                    return Array.isArray(n) ? {
+                        next: n,
+                        hasNext: !0,
+                        hasMany: !0,
+                        done: !1
+                    } : {
+                        next: n,
+                        hasNext: !0,
+                        done: !1
+                    }
+                };
+
+            function _n(n, r) {
+                if (void 0 === r && (r = Jn), r <= 0) return n.slice();
+                for (var t = [], e = 0, u = n; e < u.length; e++) {
+                    var i = u[e];
+                    Array.isArray(i) ? t.push.apply(t, _n(i, r - 1)) : t.push(i)
+                }
+                return t
+            }
+
+            function nr() {
+                return i(rr, arguments, nr.lazy)
+            }
+
+            function rr(n) {
+                return V(n, nr.lazy())
+            }
+
+            function tr() {
+                return i(er, arguments, tr.lazy)
+            }
+
+            function er(n, r) {
+                return nr(n.map((function(n) {
+                    return r(n)
+                })))
+            }
+
+            function ur() {
+                return i(ir(!1), arguments)
+            }! function(n) {
                 n.lazy = function() {
                     return function(n) {
                         return Array.isArray(n) ? {
                             done: !1,
                             hasNext: !0,
                             hasMany: !0,
                             next: n
                         } : {
                             done: !1,
                             hasNext: !0,
                             next: n
                         }
                     }
                 }
-            }(Gn || (Gn = {})),
+            }(nr || (nr = {})),
             function(n) {
                 n.lazy = function(n) {
                     return function(r) {
                         var t = n(r);
                         return Array.isArray(t) ? {
                             done: !1,
                             hasNext: !0,
@@ -1012,366 +1061,375 @@
                         } : {
                             done: !1,
                             hasNext: !0,
                             next: t
                         }
                     }
                 }
-            }(Jn || (Jn = {}));
-            var Yn = function(n) {
+            }(tr || (tr = {}));
+            var ir = function(n) {
                 return function(r, t) {
                     for (var e = {}, u = 0; u < r.length; u++)
                         for (var i = r[u], o = 0, f = n ? t(i, u, r) : t(i); o < f.length; o++) {
                             var c = f[o],
                                 a = c[0],
                                 l = c[1];
                             e[a] = l
                         }
                     return e
                 }
             };
 
-            function Zn() {
-                return u(_n, arguments, Zn.lazy)
+            function or() {
+                return i(fr, arguments, or.lazy)
             }
 
-            function _n(n) {
-                return C(n, Zn.lazy())
+            function fr(n) {
+                return V(n, or.lazy())
             }
 
-            function nr(n) {
+            function cr(n) {
                 if (!Array.isArray(n)) return n;
                 for (var r = [], t = 0, e = n; t < e.length; t++) {
                     var u = e[t];
-                    Array.isArray(u) ? r.push.apply(r, Zn(u)) : r.push(u)
+                    Array.isArray(u) ? r.push.apply(r, or(u)) : r.push(u)
                 }
                 return r
             }
 
-            function rr() {
-                return u(d(Math.floor), arguments)
+            function ar() {
+                return i(p(Math.floor), arguments)
             }
 
-            function tr() {
-                return u(er(!1), arguments, tr.lazy)
+            function lr() {
+                return i(sr(!1), arguments, lr.lazy)
             }! function(n) {
                 n.indexed = function() {
-                    return u(Yn(!0), arguments)
+                    return i(ir(!0), arguments)
                 }
-            }(Xn || (Xn = {})),
+            }(ur || (ur = {})),
             function(n) {
                 n.lazy = function() {
                     return function(n) {
-                        var r = nr(n);
+                        var r = cr(n);
                         return Array.isArray(r) ? {
                             done: !1,
                             hasNext: !0,
                             hasMany: !0,
                             next: r
                         } : {
                             done: !1,
                             hasNext: !0,
                             next: r
                         }
                     }
                 }
-            }(Zn || (Zn = {}));
-            var er = function(n) {
+            }(or || (or = {}));
+            var sr = function(n) {
                     return function(r, t) {
-                        return C(r, n ? tr.lazyIndexed(t) : tr.lazy(t), n)
+                        return V(r, n ? lr.lazyIndexed(t) : lr.lazy(t), n)
                     }
                 },
-                ur = function(n) {
+                vr = function(n) {
                     return function(r) {
                         return function(t, e, u) {
                             return n ? r(t, e, u) : r(t), {
                                 done: !1,
                                 hasNext: !0,
                                 next: t
                             }
                         }
                     }
                 };
 
-            function ir() {
-                return u(or(!1), arguments)
+            function yr() {
+                return i(hr(!1), arguments)
             }! function(n) {
                 n.indexed = function() {
-                    return u(er(!0), arguments, n.lazyIndexed)
-                }, n.lazy = ur(!1), n.lazyIndexed = In(ur(!0))
-            }(tr || (tr = {}));
-            var or = function(n) {
+                    return i(sr(!0), arguments, n.lazyIndexed)
+                }, n.lazy = vr(!1), n.lazyIndexed = kn(vr(!0))
+            }(lr || (lr = {}));
+            var hr = function(n) {
                 return function(r, t) {
                     for (var e in r)
                         if (Object.prototype.hasOwnProperty.call(r, e)) {
                             var u = r[e];
                             n ? t(u, e, r) : t(u)
                         } return r
                 }
             };
 
-            function fr() {
-                return u(cr, arguments)
+            function dr() {
+                return i(pr, arguments)
             }
 
-            function cr(n) {
+            function pr(n) {
                 for (var r = {}, t = 0, e = n; t < e.length; t++) {
                     var u = e[t],
                         i = u[0],
                         o = u[1];
                     r[i] = o
                 }
                 return r
             }
 
-            function ar() {
-                return u(lr, arguments)
+            function gr() {
+                return i(xr, arguments)
             }
 
-            function lr(n, r) {
+            function xr(n, r) {
                 for (var t = {}, e = 0, u = n; e < u.length; e++) {
                     var i = u[e];
                     t[i] = r(i)
                 }
                 return t
             }
 
-            function sr() {
-                return u(vr, arguments)
+            function br() {
+                return i(mr, arguments)
             }
 
-            function vr(n) {
+            function mr(n) {
                 for (var r = {}, t = 0, e = n; t < e.length; t++) {
                     var u = e[t],
                         i = u[0],
                         o = u[1];
                     r[i] = o
                 }
                 return r
             }
 
-            function yr() {
-                return u(hr(!1), arguments)
+            function zr() {
+                return i(Or(!1), arguments)
             }! function(n) {
                 n.indexed = function() {
-                    return u(or(!0), arguments)
+                    return i(hr(!0), arguments)
                 }
-            }(ir || (ir = {})),
+            }(yr || (yr = {})),
             function(n) {
                 n.strict = n
-            }(fr || (fr = {})),
+            }(dr || (dr = {})),
             function(n) {
                 n.strict = n
-            }(sr || (sr = {}));
-            var hr = function(n) {
+            }(br || (br = {}));
+            var Or = function(n) {
                 return function(r, t) {
                     for (var e = {}, u = 0; u < r.length; u++) {
                         var i = r[u],
                             o = n ? t(i, u, r) : t(i);
                         if (void 0 !== o) {
                             var f = String(o),
                                 c = e[f];
                             void 0 === c && (c = [], e[f] = c), c.push(i)
                         }
                     }
                     return e
                 }
             };
 
-            function dr() {
-                return u(pr, arguments)
+            function jr() {
+                return i(Nr, arguments)
             }
 
-            function pr(n, r) {
+            function Nr(n, r) {
                 if (n === r) return !0;
                 if ("number" == typeof n && "number" == typeof r) return n != n && r != r;
                 if ("object" != typeof n || "object" != typeof r) return !1;
                 if (null === n || null === r) return !1;
                 if (Object.getPrototypeOf(n) !== Object.getPrototypeOf(r)) return !1;
                 if (Array.isArray(n)) {
                     if (n.length !== r.length) return !1;
                     for (var t = 0; t < n.length; t++)
-                        if (!pr(n[t], r[t])) return !1;
+                        if (!Nr(n[t], r[t])) return !1;
                     return !0
                 }
                 if (n instanceof Date) return n.getTime() === r.getTime();
                 if (n instanceof RegExp) return n.toString() === r.toString();
+                if (n instanceof Map) return function(n, r) {
+                    if (n.size !== r.size) return !1;
+                    for (var t = 0, e = Array.from(n.keys()); t < e.length; t++) {
+                        var u = e[t];
+                        if (!r.has(u)) return !1;
+                        if (!Nr(n.get(u), r.get(u))) return !1
+                    }
+                    return !0
+                }(n, r);
                 var e = Object.keys(n);
                 if (e.length !== Object.keys(r).length) return !1;
                 for (var u = 0, i = e; u < i.length; u++) {
                     var o = i[u];
                     if (!Object.prototype.hasOwnProperty.call(r, o)) return !1;
-                    if (!pr(n[o], r[o])) return !1
+                    if (!Nr(n[o], r[o])) return !1
                 }
                 return !0
             }
 
-            function gr() {
-                return u(xr, arguments)
+            function Ar() {
+                return i(wr, arguments)
             }
 
-            function xr(n, r) {
+            function wr(n, r) {
                 for (var t = 0, e = Object.keys(r); t < e.length; t++) {
                     var u = e[t];
                     if (!Object.prototype.hasOwnProperty.call(n, u)) return !1;
-                    if (!dr(r[u], n[u])) return !1
+                    if (!jr(r[u], n[u])) return !1
                 }
                 return !0
             }
 
-            function br(n) {
+            function Ir(n) {
                 return n
             }
 
-            function mr() {
-                return u(zr(!1), arguments)
+            function Pr() {
+                return i(kr(!1), arguments)
             }! function(n) {
                 n.indexed = function() {
-                    return u(hr(!0), arguments)
+                    return i(Or(!0), arguments)
                 }, n.strict = n
-            }(yr || (yr = {}));
-            var zr = function(n) {
+            }(zr || (zr = {}));
+            var kr = function(n) {
                 return function(r, t) {
                     for (var e = {}, u = 0; u < r.length; u++) {
                         var i = r[u],
                             o = n ? t(i, u, r) : t(i);
                         e[String(o)] = i
                     }
                     return e
                 }
             };
 
-            function Or() {
-                return u(jr, arguments)
+            function Sr() {
+                return i(Mr, arguments)
             }
 
-            function jr(n, r) {
+            function Mr(n, r) {
                 for (var t = {}, e = 0, u = n; e < u.length; e++) {
                     var i = u[e];
                     t[r(i)] = i
                 }
                 return t
             }
 
-            function Nr() {
-                return u(wr, arguments, Nr.lazy)
+            function Er() {
+                return i(Br, arguments, Er.lazy)
             }
 
-            function wr(n, r) {
-                return C(n, Nr.lazy(r))
+            function Br(n, r) {
+                return V(n, Er.lazy(r))
             }
 
-            function Ar() {
-                return u(Ir, arguments, Ar.lazy)
+            function Tr() {
+                return i(Wr, arguments, Tr.lazy)
             }
 
-            function Ir(n, r, t) {
-                return C(n, Ar.lazy(r, t))
+            function Wr(n, r, t) {
+                return V(n, Tr.lazy(r, t))
             }
 
-            function Pr() {
-                return u(kr, arguments)
+            function Dr() {
+                return i(qr, arguments)
             }
 
-            function kr(n) {
+            function qr(n) {
                 var r = {};
                 for (var t in n) Object.prototype.hasOwnProperty.call(n, t) && (r[n[t]] = t);
                 return r
             }
 
-            function Sr(n) {
+            function Lr(n) {
                 return Array.isArray(n)
             }
 
-            function Mr(n) {
+            function Rr(n) {
                 return "boolean" == typeof n
             }
 
-            function Er(n) {
+            function Fr(n) {
                 return n instanceof Date
             }
 
-            function Br(n) {
+            function Cr(n) {
                 return null != n
             }
 
-            function Tr(n) {
+            function Kr(n) {
                 return Boolean(n) && !Array.isArray(n) && "object" == typeof n
             }
 
-            function Wr(n) {
+            function Vr(n) {
                 return "string" == typeof n
             }
 
-            function Dr(n) {
-                return void 0 === n || (Sr(n) || Wr(n) ? 0 === n.length : !!Tr(n) && 0 === Object.keys(n).length)
+            function Ur(n) {
+                return void 0 === n || (Lr(n) || Vr(n) ? 0 === n.length : !!Kr(n) && 0 === Object.keys(n).length)
             }
 
-            function qr(n) {
+            function $r(n) {
                 return n instanceof Error
             }
 
-            function Lr(n) {
+            function Gr(n) {
                 return "function" == typeof n
             }
 
-            function Rr(n, r) {
+            function Hr(n, r) {
                 if (void 0 === r) {
                     var t = new Set(n);
                     return function(n) {
                         return t.has(n)
                     }
                 }
                 return r.indexOf(n) >= 0
             }
 
-            function Fr(n) {
+            function Jr(n) {
                 return null == n
             }
 
-            function Cr(n) {
+            function Qr(n) {
                 return null !== n
             }
 
-            function Kr(n) {
+            function Xr(n) {
                 return null != n
             }
 
-            function Vr(n) {
+            function Yr(n) {
                 return function(r) {
                     return !n(r)
                 }
             }
 
-            function Ur(n) {
+            function Zr(n) {
                 return null == n
             }
 
-            function $r(n) {
+            function _r(n) {
                 return "number" == typeof n && !isNaN(n)
             }! function(n) {
                 n.indexed = function() {
-                    return u(zr(!0), arguments)
-                }, n.strict = Or
-            }(mr || (mr = {})),
+                    return i(kr(!0), arguments)
+                }, n.strict = Sr
+            }(Pr || (Pr = {})),
             function(n) {
                 n.lazy = function(n) {
                     var r = new Set(n);
                     return function(n) {
                         return r.has(n) ? {
                             done: !1,
                             hasNext: !0,
                             next: n
                         } : {
                             done: !1,
                             hasNext: !1
                         }
                     }
                 }
-            }(Nr || (Nr = {})),
+            }(Er || (Er = {})),
             function(n) {
                 n.lazy = function(n, r) {
                     return function(t) {
                         return n.some((function(n) {
                             return r(t, n)
                         })) ? {
                             done: !1,
@@ -1379,570 +1437,570 @@
                             next: t
                         } : {
                             done: !1,
                             hasNext: !1
                         }
                     }
                 }
-            }(Ar || (Ar = {})),
+            }(Tr || (Tr = {})),
             function(n) {
                 n.strict = function(n) {
                     return void 0 !== n
                 }
-            }(Br || (Br = {}));
-            var Gr = function(n) {
+            }(Cr || (Cr = {}));
+            var nt = function(n) {
                 return "object" == typeof n && null !== n
             };
 
-            function Hr(n) {
+            function rt(n) {
                 if ("object" != typeof n || null === n) return !1;
                 var r = Object.getPrototypeOf(n);
                 return null === r || r === Object.prototype
             }
 
-            function Jr(n) {
+            function tt(n) {
                 return n instanceof Promise
             }
 
-            function Qr(n) {
+            function et(n) {
                 return "symbol" == typeof n
             }
 
-            function Xr() {
-                return u(Yr, arguments)
+            function ut() {
+                return i(it, arguments)
             }
-            var Yr = function(n, r) {
+            var it = function(n, r) {
                 return n.join(r)
             };
 
-            function Zr() {
-                return u(Object.keys, arguments)
+            function ot() {
+                return i(Object.keys, arguments)
             }
 
-            function _r() {
-                return u(nt, arguments)
+            function ft() {
+                return i(ct, arguments)
             }
 
-            function nt(n) {
+            function ct(n) {
                 return n[n.length - 1]
             }
 
-            function rt() {
-                return u(tt, arguments)
+            function at() {
+                return i(lt, arguments)
             }
 
-            function tt(n) {
+            function lt(n) {
                 return "length" in n ? n.length : Array.from(n).length
             }
 
-            function et() {
-                return u(ut(!1), arguments, et.lazy)
+            function st() {
+                return i(vt(!1), arguments, st.lazy)
             }! function(n) {
                 n.strict = n
-            }(Zr || (Zr = {}));
-            var ut = function(n) {
+            }(ot || (ot = {}));
+            var vt = function(n) {
                     return function(r, t) {
-                        return C(r, n ? et.lazyIndexed(t) : et.lazy(t), n)
+                        return V(r, n ? st.lazyIndexed(t) : st.lazy(t), n)
                     }
                 },
-                it = function(n) {
+                yt = function(n) {
                     return function(r) {
                         return function(t, e, u) {
                             return {
                                 done: !1,
                                 hasNext: !0,
                                 next: n ? r(t, e, u) : r(t)
                             }
                         }
                     }
                 };
 
-            function ot() {
-                return u(ft, arguments)
+            function ht() {
+                return i(dt, arguments)
             }
 
-            function ft(n, r) {
-                for (var t = {}, e = 0, u = jn.strict(n); e < u.length; e++) {
+            function dt(n, r) {
+                for (var t = {}, e = 0, u = An.strict(n); e < u.length; e++) {
                     var i = u[e],
                         o = i[0],
                         f = i[1];
                     t[r(o, f)] = f
                 }
                 return t
             }
 
-            function ct() {
-                return u(at(!1), arguments)
+            function pt() {
+                return i(gt(!1), arguments)
             }! function(n) {
                 n.indexed = function() {
-                    return u(ut(!0), arguments, n.lazyIndexed)
-                }, n.lazy = it(!1), n.lazyIndexed = In(it(!0)), n.strict = n
-            }(et || (et = {}));
-            var at = function(n) {
+                    return i(vt(!0), arguments, n.lazyIndexed)
+                }, n.lazy = yt(!1), n.lazyIndexed = kn(yt(!0)), n.strict = n
+            }(st || (st = {}));
+            var gt = function(n) {
                 return function(r, t) {
                     for (var e = {}, u = 0; u < r.length; u++) {
                         var i = r[u],
                             o = n ? t(i, u, r) : t(i),
                             f = o[0],
                             c = o[1];
                         e[f] = c
                     }
                     return e
                 }
             };
 
-            function lt() {
-                return u(st, arguments)
+            function xt() {
+                return i(bt, arguments)
             }
 
-            function st(n, r) {
-                for (var t = {}, e = 0, u = jn.strict(n); e < u.length; e++) {
+            function bt(n, r) {
+                for (var t = {}, e = 0, u = An.strict(n); e < u.length; e++) {
                     var i = u[e],
                         o = i[0],
                         f = r(i[1], o);
                     t[o] = f
                 }
                 return t
             }
 
-            function vt() {
-                return u(yt(!1), arguments, vt.lazy)
+            function mt() {
+                return i(zt(!1), arguments, mt.lazy)
             }! function(n) {
                 n.indexed = function() {
-                    return u(at(!0), arguments)
+                    return i(gt(!0), arguments)
                 }
-            }(ct || (ct = {}));
-            var yt = function(n) {
+            }(pt || (pt = {}));
+            var zt = function(n) {
                     return function(r, t, e) {
-                        return C(r, (n ? vt.lazyIndexed : vt.lazy)(t, e), n)
+                        return V(r, (n ? mt.lazyIndexed : mt.lazy)(t, e), n)
                     }
                 },
-                ht = function(n) {
+                Ot = function(n) {
                     return function(r, t) {
                         var e = t;
                         return function(t, u, i) {
                             return {
                                 done: !1,
                                 hasNext: !0,
                                 next: e = n ? r(e, t, u, i) : r(e, t)
                             }
                         }
                     }
                 };
             ! function(n) {
                 n.indexed = function() {
-                    return u(yt(!0), arguments, n.lazyIndexed)
-                }, n.lazy = ht(!1), n.lazyIndexed = In(ht(!0))
-            }(vt || (vt = {}));
-            var dt = function(n) {
+                    return i(zt(!0), arguments, n.lazyIndexed)
+                }, n.lazy = Ot(!1), n.lazyIndexed = kn(Ot(!0))
+            }(mt || (mt = {}));
+            var jt = function(n) {
                 return function(r, t) {
                     for (var e, u, i = 0; i < r.length; i++) {
                         var o = r[i],
                             f = n ? t(o, i, r) : t(o);
                         (void 0 === u || f > u) && (e = o, u = f)
                     }
                     return e
                 }
             };
 
-            function pt() {
-                return u(dt(!1), arguments)
+            function Nt() {
+                return i(jt(!1), arguments)
             }! function(n) {
                 n.indexed = function() {
-                    return u(dt(!0), arguments)
+                    return i(jt(!0), arguments)
                 }
-            }(pt || (pt = {}));
-            var gt = function(n) {
+            }(Nt || (Nt = {}));
+            var At = function(n) {
                 return function(r, t) {
                     if (0 === r.length) return NaN;
                     for (var e = 0, u = 0; u < r.length; u++) {
                         var i = r[u];
                         e += n ? t(i, u, r) : t(i)
                     }
                     return e / r.length
                 }
             };
 
-            function xt() {
-                return u(gt(!1), arguments)
+            function wt() {
+                return i(At(!1), arguments)
             }! function(n) {
                 n.indexed = function() {
-                    return u(gt(!0), arguments)
+                    return i(At(!0), arguments)
                 }
-            }(xt || (xt = {}));
-            var bt = function() {
-                return bt = Object.assign || function(n) {
+            }(wt || (wt = {}));
+            var It = function() {
+                return It = Object.assign || function(n) {
                     for (var r, t = 1, e = arguments.length; t < e; t++)
                         for (var u in r = arguments[t]) Object.prototype.hasOwnProperty.call(r, u) && (n[u] = r[u]);
                     return n
-                }, bt.apply(this, arguments)
+                }, It.apply(this, arguments)
             };
 
-            function mt() {
-                return u(zt, arguments)
+            function Pt() {
+                return i(kt, arguments)
             }
 
-            function zt(n, r) {
-                return bt(bt({}, n), r)
+            function kt(n, r) {
+                return It(It({}, n), r)
             }
-            var Ot = function() {
-                return Ot = Object.assign || function(n) {
+            var St = function() {
+                return St = Object.assign || function(n) {
                     for (var r, t = 1, e = arguments.length; t < e; t++)
                         for (var u in r = arguments[t]) Object.prototype.hasOwnProperty.call(r, u) && (n[u] = r[u]);
                     return n
-                }, Ot.apply(this, arguments)
+                }, St.apply(this, arguments)
             };
 
-            function jt(n) {
+            function Mt(n) {
                 for (var r = {}, t = 0, e = n; t < e.length; t++) {
                     var u = e[t];
-                    r = Ot(Ot({}, r), u)
+                    r = St(St({}, r), u)
                 }
                 return r
             }
-            var Nt = function() {
-                return Nt = Object.assign || function(n) {
+            var Et = function() {
+                return Et = Object.assign || function(n) {
                     for (var r, t = 1, e = arguments.length; t < e; t++)
                         for (var u in r = arguments[t]) Object.prototype.hasOwnProperty.call(r, u) && (n[u] = r[u]);
                     return n
-                }, Nt.apply(this, arguments)
+                }, Et.apply(this, arguments)
             };
 
-            function wt() {
-                return u(At, arguments)
+            function Bt() {
+                return i(Tt, arguments)
             }
 
-            function At(n, r) {
-                var t = Nt(Nt({}, n), r);
+            function Tt(n, r) {
+                var t = Et(Et({}, n), r);
                 for (var e in r)
                     if (e in n) {
                         var u = n[e];
-                        if (It(u)) {
+                        if (Wt(u)) {
                             var i = r[e];
-                            It(i) && (t[e] = At(u, i))
+                            Wt(i) && (t[e] = Tt(u, i))
                         }
                     } return t
             }
 
-            function It(n) {
+            function Wt(n) {
                 return "object" == typeof n && null !== n && Object.getPrototypeOf(n) === Object.prototype
             }
-            var Pt = function(n) {
+            var Dt = function(n) {
                 return function(r, t) {
                     for (var e, u, i = 0; i < r.length; i++) {
                         var o = r[i],
                             f = n ? t(o, i, r) : t(o);
                         (void 0 === u || f < u) && (e = o, u = f)
                     }
                     return e
                 }
             };
 
-            function kt() {
-                return u(Pt(!1), arguments)
+            function qt() {
+                return i(Dt(!1), arguments)
             }
 
-            function St() {
-                return u(Mt, arguments)
+            function Lt() {
+                return i(Rt, arguments)
             }
 
-            function Mt(n, r) {
+            function Rt(n, r) {
                 return n * r
             }! function(n) {
                 n.indexed = function() {
-                    return u(Pt(!0), arguments)
+                    return i(Dt(!0), arguments)
                 }
-            }(kt || (kt = {}));
-            var Et = function() {},
-                Bt = function(n, r, t) {
-                    return r < 0 || r >= n.length ? void 0 : Tt(n.slice(), 0, n.length - 1, r, t)
+            }(qt || (qt = {}));
+            var Ft = function() {},
+                Ct = function(n, r, t) {
+                    return r < 0 || r >= n.length ? void 0 : Kt(n.slice(), 0, n.length - 1, r, t)
                 };
 
-            function Tt(n, r, t, e, u) {
+            function Kt(n, r, t, e, u) {
                 if (r === t) return n[r];
                 var i = function(n, r, t, e) {
-                    for (var u = n[t], i = r, o = r; o < t; o++) e(n[o], u) < 0 && (Z(n, i, o), i += 1);
-                    return Z(n, i, t), i
+                    for (var u = n[t], i = r, o = r; o < t; o++) e(n[o], u) < 0 && (nn(n, i, o), i += 1);
+                    return nn(n, i, t), i
                 }(n, r, t, u);
-                return e === i ? n[e] : Tt(n, e < i ? r : i + 1, e < i ? i - 1 : t, e, u)
+                return e === i ? n[e] : Kt(n, e < i ? r : i + 1, e < i ? i - 1 : t, e, u)
             }
 
-            function Wt() {
-                return cn(Dt, arguments)
+            function Vt() {
+                return ln(Ut, arguments)
             }
-            var Dt = function(n, r, t) {
-                return Bt(n, t >= 0 ? t : n.length + t, r)
+            var Ut = function(n, r, t) {
+                return Ct(n, t >= 0 ? t : n.length + t, r)
             };
 
-            function qt() {
-                return u(Lt, arguments)
+            function $t() {
+                return i(Gt, arguments)
             }
 
-            function Lt(n, r) {
+            function Gt(n, r) {
                 var t;
                 return (t = {})[r] = n, t
             }
-            var Rt = function() {
-                    return Rt = Object.assign || function(n) {
+            var Ht = function() {
+                    return Ht = Object.assign || function(n) {
                         for (var r, t = 1, e = arguments.length; t < e; t++)
                             for (var u in r = arguments[t]) Object.prototype.hasOwnProperty.call(r, u) && (n[u] = r[u]);
                         return n
-                    }, Rt.apply(this, arguments)
+                    }, Ht.apply(this, arguments)
                 },
-                Ft = function(n, r) {
+                Jt = function(n, r) {
                     var t = {};
                     for (var e in n) Object.prototype.hasOwnProperty.call(n, e) && r.indexOf(e) < 0 && (t[e] = n[e]);
                     if (null != n && "function" == typeof Object.getOwnPropertySymbols) {
                         var u = 0;
                         for (e = Object.getOwnPropertySymbols(n); u < e.length; u++) r.indexOf(e[u]) < 0 && Object.prototype.propertyIsEnumerable.call(n, e[u]) && (t[e[u]] = n[e[u]])
                     }
                     return t
                 };
 
-            function Ct() {
-                return u(Kt, arguments)
+            function Qt() {
+                return i(Xt, arguments)
             }
 
-            function Kt(n, r) {
-                if (!_(r, 1)) return Rt({}, n);
-                if (!_(r, 2)) {
+            function Xt(n, r) {
+                if (!rn(r, 1)) return Ht({}, n);
+                if (!rn(r, 2)) {
                     var t = r[0],
                         e = n,
                         u = t;
-                    return e[u], Ft(e, ["symbol" == typeof u ? u : u + ""])
+                    return e[u], Jt(e, ["symbol" == typeof u ? u : u + ""])
                 }
                 if (!r.some((function(r) {
                         return r in n
-                    }))) return Rt({}, n);
+                    }))) return Ht({}, n);
                 var i = new Set(r);
-                return fr(Object.entries(n).filter((function(n) {
+                return dr(Object.entries(n).filter((function(n) {
                     var r = n[0];
                     return !i.has(r)
                 })))
             }
 
-            function Vt() {
-                return u(Ut, arguments)
+            function Yt() {
+                return i(Zt, arguments)
             }
 
-            function Ut(n, r) {
+            function Zt(n, r) {
                 if (null == n) return n;
-                for (var t = {}, e = 0, u = Zr.strict(n); e < u.length; e++) {
+                for (var t = {}, e = 0, u = ot.strict(n); e < u.length; e++) {
                     var i = u[e];
                     r(n[i], i) || (t[i] = n[i])
                 }
                 return t
             }
 
-            function $t(n) {
+            function _t(n) {
                 var r, t = !1;
                 return function() {
                     return t || (r = n(), t = !0), r
                 }
             }
 
-            function Gt() {
-                return u(Ht, arguments)
+            function ne() {
+                return i(re, arguments)
             }
 
-            function Ht(n) {
+            function re(n) {
                 return 1 === n.length ? n[0] : void 0
             }
 
-            function Jt() {
-                return u(Qt(!1), arguments)
+            function te() {
+                return i(ee(!1), arguments)
             }
-            var Qt = function(n) {
+            var ee = function(n) {
                 return function(r, t) {
                     for (var e = [
                             [],
                             []
                         ], u = 0; u < r.length; u++) {
                         var i = r[u];
                         e[(n ? t(i, u, r) : t(i)) ? 0 : 1].push(i)
                     }
                     return e
                 }
             };
 
-            function Xt() {
-                return u(Yt, arguments)
+            function ue() {
+                return i(ie, arguments)
             }
 
-            function Yt(n, r, t) {
+            function ie(n, r, t) {
                 for (var e = n, u = 0, i = r; u < i.length; u++) {
                     var o = i[u];
                     if (null == e) break;
                     e = e[o]
                 }
                 return null != e ? e : t
             }
 
-            function Zt() {
-                return u(_t, arguments)
+            function oe() {
+                return i(fe, arguments)
             }
 
-            function _t(n, r) {
+            function fe(n, r) {
                 for (var t = {}, e = 0, u = r; e < u.length; e++) {
                     var i = u[e];
                     i in n && (t[i] = n[i])
                 }
                 return t
             }
 
-            function ne() {
-                return u(re, arguments)
+            function ce() {
+                return i(ae, arguments)
             }
 
-            function re(n, r) {
+            function ae(n, r) {
                 if (null == n) return {};
-                for (var t = {}, e = 0, u = Zr.strict(n); e < u.length; e++) {
+                for (var t = {}, e = 0, u = ot.strict(n); e < u.length; e++) {
                     var i = u[e];
                     r(n[i], i) && (t[i] = n[i])
                 }
                 return t
-            }(Jt || (Jt = {})).indexed = function() {
-                return u(Qt(!0), arguments)
+            }(te || (te = {})).indexed = function() {
+                return i(ee(!0), arguments)
             };
-            var te = function(n, r, t) {
+            var le = function(n, r, t) {
                 if (t || 2 === arguments.length)
                     for (var e, u = 0, i = r.length; u < i; u++) !e && u in r || (e || (e = Array.prototype.slice.call(r, 0, u)), e[u] = r[u]);
                 return n.concat(e || Array.prototype.slice.call(r))
             };
 
-            function ee() {
+            function se() {
                 for (var n = [], r = 0; r < arguments.length; r++) n[r] = arguments[r];
                 return function(r) {
-                    return D.apply(void 0, te([r], n, !1))
+                    return L.apply(void 0, le([r], n, !1))
                 }
             }
 
-            function ue() {
-                return u(ie, arguments)
+            function ve() {
+                return i(ye, arguments)
             }
 
-            function ie(n) {
+            function ye(n) {
                 for (var r = 1, t = 0, e = n; t < e.length; t++) r *= e[t];
                 return r
             }
-            var oe = function(n) {
+            var he = function(n) {
                 return function(r) {
                     return r[n]
                 }
             };
 
-            function fe() {
-                return u(ce, arguments)
+            function de() {
+                return i(pe, arguments)
             }
 
-            function ce(n, r, t) {
+            function pe(n, r, t) {
                 for (var e = {}, u = 0, i = n; u < i.length; u++) {
                     var o = i[u],
                         f = r(o),
                         c = t(o);
                     e[f] = c
                 }
                 return e
             }
 
-            function ae() {
-                return u(le, arguments)
+            function ge() {
+                return i(xe, arguments)
             }
 
-            function le(n, r) {
+            function xe(n, r) {
                 if (n < 0) throw new RangeError("n must be a non-negative number");
                 for (var t = [], e = 0; e < n; e++) t.push(r(e));
                 return t
             }
 
-            function se() {
-                return u(ve, arguments)
+            function be() {
+                return i(me, arguments)
             }
 
-            function ve(n) {
-                return ae(n, ye).join("")
+            function me(n) {
+                return ge(n, ze).join("")
             }
-            var ye = function() {
+            var ze = function() {
                 return "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789" [Math.floor(62 * Math.random())]
             };
 
-            function he() {
-                return u(de, arguments)
+            function Oe() {
+                return i(je, arguments)
             }
 
-            function de(n, r) {
+            function je(n, r) {
                 for (var t = [], e = n; e < r; e++) t.push(e);
                 return t
             }
 
-            function pe() {
-                return cn(ge, arguments)
+            function Ne() {
+                return ln(Ae, arguments)
             }
 
-            function ge(n, r, t) {
+            function Ae(n, r, t) {
                 for (var e = 0, u = 0, i = n; u < i.length; u++) r(t, i[u]) > 0 && (e += 1);
                 return e
             }
 
-            function xe() {
-                return u(be(!1), arguments)
+            function we() {
+                return i(Ie(!1), arguments)
             }
-            var be = function(n) {
+            var Ie = function(n) {
                 return function(r, t, e) {
                     return r.reduce((function(e, u, i) {
                         return n ? t(e, u, i, r) : t(e, u)
                     }), e)
                 }
             };
 
-            function me() {
-                return u(ze(!1), arguments, me.lazy)
+            function Pe() {
+                return i(ke(!1), arguments, Pe.lazy)
             }! function(n) {
                 n.indexed = function() {
-                    return u(be(!0), arguments)
+                    return i(Ie(!0), arguments)
                 }
-            }(xe || (xe = {}));
-            var ze = function(n) {
+            }(we || (we = {}));
+            var ke = function(n) {
                     return function(r, t) {
-                        return C(r, n ? me.lazyIndexed(t) : me.lazy(t), n)
+                        return V(r, n ? Pe.lazyIndexed(t) : Pe.lazy(t), n)
                     }
                 },
-                Oe = function(n) {
+                Se = function(n) {
                     return function(r) {
                         return function(t, e, u) {
                             return (n ? r(t, e, u) : r(t)) ? {
                                 done: !1,
                                 hasNext: !1
                             } : {
                                 done: !1,
                                 hasNext: !0,
                                 next: t
                             }
                         }
                     }
                 };
 
-            function je() {
-                return u(Ne, arguments)
+            function Me() {
+                return i(Ee, arguments)
             }
 
-            function Ne(n) {
+            function Ee(n) {
                 return n.slice().reverse()
             }
 
-            function we() {
-                return u(d(Math.round), arguments)
+            function Be() {
+                return i(p(Math.round), arguments)
             }
 
-            function Ae() {
+            function Te() {
                 for (var n = [], r = 0; r < arguments.length; r++) n[r] = arguments[r];
-                return u(Ie, n)
+                return i(We, n)
             }
 
-            function Ie(n, r) {
+            function We(n, r) {
                 if (r < 0) throw new RangeError("sampleSize must cannot be negative: ".concat(r));
                 if (!Number.isInteger(r)) throw new TypeError("sampleSize must be an integer: ".concat(r));
                 if (r >= n.length) return n.slice();
                 if (0 === r) return [];
                 for (var t = Math.min(r, n.length - r), e = new Set; e.size < t;) {
                     var u = Math.floor(Math.random() * n.length);
                     e.add(u)
@@ -1952,373 +2010,373 @@
                 })).map((function(r) {
                     return n[r]
                 })) : n.filter((function(n, r) {
                     return !e.has(r)
                 }))
             }! function(n) {
                 n.indexed = function() {
-                    return u(ze(!0), arguments, n.lazyIndexed)
-                }, n.lazy = Oe(!1), n.lazyIndexed = In(Oe(!0))
-            }(me || (me = {}));
-            var Pe = function() {
-                return Pe = Object.assign || function(n) {
+                    return i(ke(!0), arguments, n.lazyIndexed)
+                }, n.lazy = Se(!1), n.lazyIndexed = kn(Se(!0))
+            }(Pe || (Pe = {}));
+            var De = function() {
+                return De = Object.assign || function(n) {
                     for (var r, t = 1, e = arguments.length; t < e; t++)
                         for (var u in r = arguments[t]) Object.prototype.hasOwnProperty.call(r, u) && (n[u] = r[u]);
                     return n
-                }, Pe.apply(this, arguments)
+                }, De.apply(this, arguments)
             };
 
-            function ke() {
-                return u(Se, arguments)
+            function qe() {
+                return i(Le, arguments)
             }
 
-            function Se(n, r, t) {
+            function Le(n, r, t) {
                 var e;
-                return Pe(Pe({}, n), ((e = {})[r] = t, e))
+                return De(De({}, n), ((e = {})[r] = t, e))
             }
-            var Me = function() {
-                return Me = Object.assign || function(n) {
+            var Re = function() {
+                return Re = Object.assign || function(n) {
                     for (var r, t = 1, e = arguments.length; t < e; t++)
                         for (var u in r = arguments[t]) Object.prototype.hasOwnProperty.call(r, u) && (n[u] = r[u]);
                     return n
-                }, Me.apply(this, arguments)
+                }, Re.apply(this, arguments)
             };
 
-            function Ee() {
-                return u(Be, arguments)
+            function Fe() {
+                return i(Ce, arguments)
             }
 
-            function Be(n, r, t) {
+            function Ce(n, r, t) {
                 var e, u = r[0],
                     i = r.slice(1);
                 if (void 0 === u) return t;
                 if (Array.isArray(n)) return n.map((function(n, r) {
-                    return r === u ? Be(n, i, t) : n
+                    return r === u ? Ce(n, i, t) : n
                 }));
                 if (null == n) throw new Error("Path doesn't exist in object!");
-                return Me(Me({}, n), ((e = {})[u] = Be(n[u], i, t), e))
+                return Re(Re({}, n), ((e = {})[u] = Ce(n[u], i, t), e))
             }
 
-            function Te() {
-                return u(We, arguments)
+            function Ke() {
+                return i(Ve, arguments)
             }
 
-            function We(n) {
+            function Ve(n) {
                 for (var r = n.slice(), t = 0; t < n.length; t++) {
                     var e = t + Math.floor(Math.random() * (n.length - t)),
                         u = r[e];
                     r[e] = r[t], r[t] = u
                 }
                 return r
             }
-            var De = function(n, r) {
+            var Ue = function(n, r) {
                 return function(t) {
                     return t.slice(n, r)
                 }
             };
 
-            function qe() {
-                return u(Le, arguments)
+            function $e() {
+                return i(Ge, arguments)
             }
 
-            function Le(n, r) {
+            function Ge(n, r) {
                 var t = n.slice();
                 return t.sort(r), t
             }
 
-            function Re() {
-                return fn(Fe, arguments)
+            function He() {
+                return an(Je, arguments)
             }! function(n) {
                 n.strict = n
-            }(qe || (qe = {}));
-            var Fe = function(n, r) {
+            }($e || ($e = {}));
+            var Je = function(n, r) {
                 return n.slice().sort(r)
             };
 
-            function Ce(n, r) {
+            function Qe(n, r) {
                 for (var t = 0, e = n.length; t < e;) {
                     var u = t + e >>> 1;
                     r(n[u], u) ? t = u + 1 : e = u
                 }
                 return e
             }
 
-            function Ke() {
-                return u(Ve, arguments)
+            function Xe() {
+                return i(Ye, arguments)
             }! function(n) {
                 n.strict = n
-            }(Re || (Re = {}));
-            var Ve = function(n, r) {
-                return Ce(n, (function(n) {
+            }(He || (He = {}));
+            var Ye = function(n, r) {
+                return Qe(n, (function(n) {
                     return n < r
                 }))
             };
 
-            function Ue() {
-                return u($e, arguments)
+            function Ze() {
+                return i(_e, arguments)
             }
 
-            function $e(n, r, t) {
+            function _e(n, r, t) {
                 var e = t(r);
-                return Ce(n, (function(n, r) {
+                return Qe(n, (function(n, r) {
                     return t(n, r) < e
                 }))
             }
 
-            function Ge() {
-                return u(Ce, arguments)
+            function nu() {
+                return i(Qe, arguments)
             }
 
-            function He() {
-                return u(Je, arguments)
+            function ru() {
+                return i(tu, arguments)
             }! function(n) {
                 n.indexed = function() {
-                    return u($e, arguments)
+                    return i(_e, arguments)
                 }
-            }(Ue || (Ue = {})),
+            }(Ze || (Ze = {})),
             function(n) {
                 n.indexed = function() {
-                    return u(Ce, arguments)
+                    return i(Qe, arguments)
                 }
-            }(Ge || (Ge = {}));
-            var Je = function(n, r) {
-                return Ce(n, (function(n) {
+            }(nu || (nu = {}));
+            var tu = function(n, r) {
+                return Qe(n, (function(n) {
                     return n <= r
                 }))
             };
 
-            function Qe() {
-                return u(Xe, arguments)
+            function eu() {
+                return i(uu, arguments)
             }
 
-            function Xe(n, r, t) {
+            function uu(n, r, t) {
                 var e = t(r);
-                return Ce(n, (function(n, r) {
+                return Qe(n, (function(n, r) {
                     return t(n, r) <= e
                 }))
             }! function(n) {
                 n.indexed = function() {
-                    return u(Xe, arguments)
+                    return i(uu, arguments)
                 }
-            }(Qe || (Qe = {}));
-            var Ye = function(n, r, t) {
+            }(eu || (eu = {}));
+            var iu = function(n, r, t) {
                 if (t || 2 === arguments.length)
                     for (var e, u = 0, i = r.length; u < i; u++) !e && u in r || (e || (e = Array.prototype.slice.call(r, 0, u)), e[u] = r[u]);
                 return n.concat(e || Array.prototype.slice.call(r))
             };
 
-            function Ze() {
-                return u(_e, arguments)
+            function ou() {
+                return i(fu, arguments)
             }
 
-            function _e(n, r, t, e) {
+            function fu(n, r, t, e) {
                 var u = n.slice();
-                return u.splice.apply(u, Ye([r, t], e, !1)), u
+                return u.splice.apply(u, iu([r, t], e, !1)), u
             }
 
-            function nu() {
-                return u(ru, arguments)
+            function cu() {
+                return i(au, arguments)
             }
 
-            function ru(n, r) {
+            function au(n, r) {
                 var t = n.slice(),
                     e = t.splice(r);
                 return [t, e]
             }
 
-            function tu() {
-                return u(eu, arguments)
+            function lu() {
+                return i(su, arguments)
             }
 
-            function eu(n, r) {
+            function su(n, r) {
                 for (var t = 0; t < n.length; t++)
-                    if (r(n[t])) return nu(n, t);
+                    if (r(n[t])) return cu(n, t);
                 return [n.slice(), []]
             }
-            var uu = function(n, r, t) {
+            var vu = function(n, r, t) {
                 if (t || 2 === arguments.length)
                     for (var e, u = 0, i = r.length; u < i; u++) !e && u in r || (e || (e = Array.prototype.slice.call(r, 0, u)), e[u] = r[u]);
                 return n.concat(e || Array.prototype.slice.call(r))
             };
 
-            function iu(n) {
-                return ou(n)
+            function yu(n) {
+                return hu(n)
             }
 
-            function ou(n) {
+            function hu(n) {
                 var r;
                 if (0 === n.length) return [];
                 var t = null !== (r = /^\[(.+?)\](.*)$/u.exec(n)) && void 0 !== r ? r : /^\.?([^.[\]]+)(.*)$/u.exec(n);
                 if (null !== t) {
                     var e = t[1],
                         u = t[2];
-                    return uu([e], ou(u), !0)
+                    return vu([e], hu(u), !0)
                 }
                 return [n]
             }
 
-            function fu() {
-                return u(cu, arguments)
+            function du() {
+                return i(pu, arguments)
             }
 
-            function cu(n, r) {
+            function pu(n, r) {
                 return n - r
             }
 
-            function au() {
-                return u(lu, arguments)
+            function gu() {
+                return i(xu, arguments)
             }
 
-            function lu(n) {
+            function xu(n) {
                 for (var r = 0, t = 0, e = n; t < e.length; t++) r += e[t];
                 return r
             }
-            var su = function(n) {
+            var bu = function(n) {
                 return function(r, t) {
                     for (var e = 0, u = 0; u < r.length; u++) {
                         var i = r[u];
                         e += n ? t(i, u, r) : t(i)
                     }
                     return e
                 }
             };
 
-            function vu() {
-                return u(su(!1), arguments)
+            function mu() {
+                return i(bu(!1), arguments)
             }
 
-            function yu() {
-                return u(hu, arguments)
+            function zu() {
+                return i(Ou, arguments)
             }
 
-            function hu(n, r, t) {
+            function Ou(n, r, t) {
                 return "string" == typeof n ? function(n, r, t) {
-                    return du(n.split(""), r, t).join("")
-                }(n, r, t) : du(n, r, t)
+                    return ju(n.split(""), r, t).join("")
+                }(n, r, t) : ju(n, r, t)
             }
 
-            function du(n, r, t) {
+            function ju(n, r, t) {
                 var e = n.slice();
                 if (isNaN(r) || isNaN(t)) return e;
                 var u = r < 0 ? n.length + r : r,
                     i = t < 0 ? n.length + t : t;
                 return u < 0 || u > n.length || i < 0 || i > n.length || (e[u] = n[i], e[i] = n[u]), e
             }! function(n) {
                 n.indexed = function() {
-                    return u(su(!0), arguments)
+                    return i(bu(!0), arguments)
                 }
-            }(vu || (vu = {}));
-            var pu = function() {
-                return pu = Object.assign || function(n) {
+            }(mu || (mu = {}));
+            var Nu = function() {
+                return Nu = Object.assign || function(n) {
                     for (var r, t = 1, e = arguments.length; t < e; t++)
                         for (var u in r = arguments[t]) Object.prototype.hasOwnProperty.call(r, u) && (n[u] = r[u]);
                     return n
-                }, pu.apply(this, arguments)
+                }, Nu.apply(this, arguments)
             };
 
-            function gu() {
-                return u(xu, arguments)
+            function Au() {
+                return i(wu, arguments)
             }
 
-            function xu(n, r, t) {
+            function wu(n, r, t) {
                 var e, u = n,
                     i = u[r],
                     o = u[t];
-                return pu(pu({}, n), ((e = {})[r] = o, e[t] = i, e))
+                return Nu(Nu({}, n), ((e = {})[r] = o, e[t] = i, e))
             }
 
-            function bu() {
-                return u(mu, arguments, bu.lazy)
+            function Iu() {
+                return i(Pu, arguments, Iu.lazy)
             }
 
-            function mu(n, r) {
-                return C(n, bu.lazy(r))
+            function Pu(n, r) {
+                return V(n, Iu.lazy(r))
             }
 
-            function zu() {
-                return cn(Ou, arguments)
+            function ku() {
+                return ln(Su, arguments)
             }
 
-            function Ou(n, r, t) {
+            function Su(n, r, t) {
                 if (t <= 0) return [];
                 if (t >= n.length) return n.slice();
                 var e = n.slice(0, t);
-                rn(e, r);
-                for (var u = 0, i = n.slice(t); u < i.length; u++) tn(e, r, i[u]);
+                en(e, r);
+                for (var u = 0, i = n.slice(t); u < i.length; u++) un(e, r, i[u]);
                 return e
             }
 
-            function ju() {
-                return u(Nu, arguments)
+            function Mu() {
+                return i(Eu, arguments)
             }
 
-            function Nu(n, r) {
+            function Eu(n, r) {
                 for (var t = n.length - 1; t >= 0; t--)
                     if (!r(n[t])) return n.slice(t + 1);
                 return n.slice()
             }
 
-            function wu() {
-                return u(Au, arguments)
+            function Bu() {
+                return i(Tu, arguments)
             }
 
-            function Au(n, r) {
+            function Tu(n, r) {
                 for (var t = [], e = 0, u = n; e < u.length; e++) {
                     var i = u[e];
                     if (!r(i)) break;
                     t.push(i)
                 }
                 return t
             }
 
-            function Iu() {
-                return u(Pu, arguments)
+            function Wu() {
+                return i(Du, arguments)
             }
 
-            function Pu(n, r) {
+            function Du(n, r) {
                 return r(n), n
             }
 
-            function ku() {
-                return u(Su, arguments, ku.lazy)
+            function qu() {
+                return i(Lu, arguments, qu.lazy)
             }
 
-            function Su(n) {
-                return C(n, ku.lazy())
+            function Lu(n) {
+                return V(n, qu.lazy())
             }
 
-            function Mu() {
-                return u(Eu, arguments, Bu)
+            function Ru() {
+                return i(Fu, arguments, Cu)
             }
 
-            function Eu(n, r) {
-                return C(n, Bu(r))
+            function Fu(n, r) {
+                return V(n, Cu(r))
             }
 
-            function Bu(n) {
+            function Cu(n) {
                 var r = new Set;
                 return function(t) {
                     var e = n(t);
                     return r.has(e) ? {
                         done: !1,
                         hasNext: !1
                     } : (r.add(e), {
                         done: !1,
                         hasNext: !0,
                         next: t
                     })
                 }
             }
 
-            function Tu() {
-                return u(Wu, arguments, Tu.lazy)
+            function Ku() {
+                return i(Vu, arguments, Ku.lazy)
             }
 
-            function Wu(n, r) {
-                return C(n, Tu.lazy(r), !0)
+            function Vu(n, r) {
+                return V(n, Ku.lazy(r), !0)
             }! function(n) {
                 n.lazy = function(n) {
                     if (n <= 0) return function() {
                         return {
                             done: !0,
                             hasNext: !1
                         }
@@ -2328,152 +2386,152 @@
                         return {
                             done: (r -= 1) <= 0,
                             hasNext: !0,
                             next: n
                         }
                     }
                 }
-            }(bu || (bu = {})),
+            }(Iu || (Iu = {})),
             function(n) {
                 n.lazy = function() {
                     var n = new Set;
                     return function(r) {
                         return n.has(r) ? {
                             done: !1,
                             hasNext: !1
                         } : (n.add(r), {
                             done: !1,
                             hasNext: !0,
                             next: r
                         })
                     }
                 }
-            }(ku || (ku = {}));
-            var Du = function(n) {
+            }(qu || (qu = {}));
+            var Uu = function(n) {
                 return function(r, t, e) {
                     return void 0 !== e && e.findIndex((function(t) {
                         return n(r, t)
                     })) === t ? {
                         done: !1,
                         hasNext: !0,
                         next: r
                     } : {
                         done: !1,
                         hasNext: !1
                     }
                 }
             };
 
-            function qu() {
-                return u(Lu, arguments, qu.lazy)
+            function $u() {
+                return i(Gu, arguments, $u.lazy)
             }
 
-            function Lu(n) {
-                return C(n, qu.lazy())
+            function Gu(n) {
+                return V(n, $u.lazy())
             }
 
-            function Ru() {
-                return u(Fu, arguments, Cu)
+            function Hu() {
+                return i(Ju, arguments, Qu)
             }
 
-            function Fu(n, r) {
-                return C(n, Cu(r))
+            function Ju(n, r) {
+                return V(n, Qu(r))
             }
 
-            function Cu(n) {
+            function Qu(n) {
                 var r = new Set;
                 return function(t) {
                     var e = n(t);
                     return r.has(e) ? {
                         done: !1,
                         hasNext: !1
                     } : (r.add(e), {
                         done: !1,
                         hasNext: !0,
                         next: t
                     })
                 }
             }
 
-            function Ku() {
-                return u(Vu, arguments, Ku.lazy)
+            function Xu() {
+                return i(Yu, arguments, Xu.lazy)
             }
 
-            function Vu(n, r) {
-                return C(n, Ku.lazy(r), !0)
+            function Yu(n, r) {
+                return V(n, Xu.lazy(r), !0)
             }! function(n) {
-                n.lazy = In(Du)
-            }(Tu || (Tu = {})),
+                n.lazy = kn(Uu)
+            }(Ku || (Ku = {})),
             function(n) {
                 n.lazy = function() {
                     var n = new Set;
                     return function(r) {
                         return n.has(r) ? {
                             done: !1,
                             hasNext: !1
                         } : (n.add(r), {
                             done: !1,
                             hasNext: !0,
                             next: r
                         })
                     }
                 }
-            }(qu || (qu = {}));
-            var Uu = function(n) {
+            }($u || ($u = {}));
+            var Zu = function(n) {
                 return function(r, t, e) {
                     return void 0 !== e && e.findIndex((function(t) {
                         return n(r, t)
                     })) === t ? {
                         done: !1,
                         hasNext: !0,
                         next: r
                     } : {
                         done: !1,
                         hasNext: !1
                     }
                 }
             };
 
-            function $u() {
-                return u(Object.values, arguments)
+            function _u() {
+                return i(Object.values, arguments)
             }
 
-            function Gu() {
-                return u(Hu, arguments)
+            function ni() {
+                return i(ri, arguments)
             }
 
-            function Hu(n, r) {
+            function ri(n, r) {
                 for (var t = n.length > r.length ? r.length : n.length, e = [], u = 0; u < t; u++) e.push([n[u], r[u]]);
                 return e
             }
 
-            function Ju() {
-                return u(Qu, arguments)
+            function ti() {
+                return i(ei, arguments)
             }
 
-            function Qu(n, r) {
+            function ei(n, r) {
                 for (var t = n.length > r.length ? r.length : n.length, e = {}, u = 0; u < t; u++) e[n[u]] = r[u];
                 return e
             }
 
-            function Xu(n, r, t) {
+            function ui(n, r, t) {
                 if ("function" == typeof n) return void 0 === r ? function(r, t) {
-                    return Yu(r, t, n)
+                    return ii(r, t, n)
                 } : function(t) {
-                    return Yu(t, r, n)
+                    return ii(t, r, n)
                 };
                 if (void 0 === r || void 0 === t) throw new Error("zipWith: Missing arguments in dataFirst function call");
-                return Yu(n, r, t)
+                return ii(n, r, t)
             }
 
-            function Yu(n, r, t) {
+            function ii(n, r, t) {
                 for (var e = n.length > r.length ? r.length : n.length, u = [], i = 0; i < e; i++) u.push(t(n[i], r[i]));
                 return u
             }! function(n) {
-                n.lazy = In(Uu)
-            }(Ku || (Ku = {})),
+                n.lazy = kn(Zu)
+            }(Xu || (Xu = {})),
             function(n) {
                 n.strict = n
-            }(Gu || (Gu = {}))
+            }(ni || (ni = {}))
         }
     }
 ]);
```

### Comparing `neopyter-0.2.0/neopyter/labextension/static/remoteEntry.6c91dc6f35c735e32d34.js` & `neopyter-0.2.1/neopyter/labextension/static/remoteEntry.dfbe5e3084dd43118cf8.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, f, d, c, s, p, h, v, b, g, y, m, w, j, S = {
+    var e, r, t, n, o, a, i, u, f, d, l, s, p, c, h, v, b, g, y, m, w, j, S = {
             385: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(336).then((() => () => t(336))),
                         "./extension": () => t.e(336).then((() => () => t(336))),
                         "./style": () => t.e(728).then((() => () => t(728)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -57,54 +57,54 @@
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
         7: "8eb9a8e937e5deb3af13",
-        330: "91022d3a2c8e60de7676",
-        336: "f2f9124a0511bcaade9f",
-        728: "d85cbe66bc2da24c7357",
-        769: "477fd518dada39821aad"
+        330: "aa97145ed71c9fb187d2",
+        336: "a49647ad642daa70dfb8",
+        537: "62c041ec63a28b9c91aa",
+        728: "d85cbe66bc2da24c7357"
     } [e] + ".js?v=" + {
         7: "8eb9a8e937e5deb3af13",
-        330: "91022d3a2c8e60de7676",
-        336: "f2f9124a0511bcaade9f",
-        728: "d85cbe66bc2da24c7357",
-        769: "477fd518dada39821aad"
+        330: "aa97145ed71c9fb187d2",
+        336: "a49647ad642daa70dfb8",
+        537: "62c041ec63a28b9c91aa",
+        728: "d85cbe66bc2da24c7357"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), t = {}, n = "neopyter:", E.l = (e, r, o, a) => {
         if (t[e]) t[e].push(r);
         else {
             var i, u;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var d = l[f];
-                    if (d.getAttribute("src") == e || d.getAttribute("data-webpack") == n + o) {
-                        i = d;
+                for (var f = document.getElementsByTagName("script"), d = 0; d < f.length; d++) {
+                    var l = f[d];
+                    if (l.getAttribute("src") == e || l.getAttribute("data-webpack") == n + o) {
+                        i = l;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", n + o), i.src = e), t[e] = [r];
-            var c = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(s);
+            var s = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var o = t[e];
                     if (delete t[e], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                s = setTimeout(c.bind(null, void 0, {
+                p = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -125,16 +125,16 @@
                             u = o[r];
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
-                    l = [];
-                return "default" === t && (u("@msgpack/msgpack", "3.0.0-beta2", (() => E.e(7).then((() => () => E(7))))), u("neopyter", "0.2.0", (() => E.e(336).then((() => () => E(336))))), u("remeda", "1.56.0", (() => E.e(769).then((() => () => E(769)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                    f = [];
+                return "default" === t && (u("@msgpack/msgpack", "3.0.0-beta2", (() => E.e(7).then((() => () => E(7))))), u("neopyter", "0.2.1", (() => E.e(336).then((() => () => E(336))))), u("remeda", "1.59.0", (() => E.e(537).then((() => () => E(537)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -170,90 +170,90 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(u = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var a = [];
         for (o = 1; o < e.length; o++) {
             var u = e[o];
-            a.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? a.pop() + " " + a.pop() : i(u))
+            a.push(0 === u ? "not(" + f() + ")" : 1 === u ? "(" + f() + " || " + f() + ")" : 2 === u ? a.pop() + " " + a.pop() : i(u))
         }
-        return l();
+        return f();
 
-        function l() {
+        function f() {
             return a.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, u = (e, r) => {
         if (0 in e) {
             r = o(r);
             var t = e[0],
                 n = t < 0;
             n && (t = -t - 1);
-            for (var a = 0, i = 1, l = !0;; i++, a++) {
-                var f, d, c = i < e.length ? (typeof e[i])[0] : "";
-                if (a >= r.length || "o" == (d = (typeof(f = r[a]))[0])) return !l || ("u" == c ? i > t && !n : "" == c != n);
-                if ("u" == d) {
-                    if (!l || "u" != c) return !1
-                } else if (l)
-                    if (c == d)
+            for (var a = 0, i = 1, f = !0;; i++, a++) {
+                var d, l, s = i < e.length ? (typeof e[i])[0] : "";
+                if (a >= r.length || "o" == (l = (typeof(d = r[a]))[0])) return !f || ("u" == s ? i > t && !n : "" == s != n);
+                if ("u" == l) {
+                    if (!f || "u" != s) return !1
+                } else if (f)
+                    if (s == l)
                         if (i <= t) {
-                            if (f != e[i]) return !1
+                            if (d != e[i]) return !1
                         } else {
-                            if (n ? f > e[i] : f < e[i]) return !1;
-                            f != e[i] && (l = !1)
+                            if (n ? d > e[i] : d < e[i]) return !1;
+                            d != e[i] && (f = !1)
                         }
-                else if ("s" != c && "n" != c) {
+                else if ("s" != s && "n" != s) {
                     if (n || i <= t) return !1;
-                    l = !1, i--
+                    f = !1, i--
                 } else {
-                    if (i <= t || d < c != n) return !1;
-                    l = !1
-                } else "s" != c && "n" != c && (l = !1, i--)
+                    if (i <= t || l < s != n) return !1;
+                    f = !1
+                } else "s" != s && "n" != s && (f = !1, i--)
             }
         }
-        var s = [],
-            p = s.pop.bind(s);
+        var p = [],
+            c = p.pop.bind(p);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
-            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? u(h, r) : !p())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? u(h, r) : !c())
         }
-        return !!p()
-    }, l = (e, r) => {
+        return !!c()
+    }, f = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, f = (e, r) => {
+    }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", c = (e, r, t, n) => {
-        var o = f(e, t);
-        return u(n, o) || p(d(e, t, o, n)), h(e[t][o])
-    }, s = (e, r, t) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", s = (e, r, t, n) => {
+        var o = d(e, t);
+        return u(n, o) || c(l(e, t, o, n)), h(e[t][o])
+    }, p = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !u(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
-    }, p = e => {
+    }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, h = e => (e.loaded = 1, e.get()), b = (v = e => function(r, t, n, o) {
         var a = E.I(r);
         return a && a.then ? a.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
-    })(((e, r, t, n) => (l(e, t), c(r, 0, t, n)))), g = v(((e, r, t, n, o) => {
-        var a = r && E.o(r, t) && s(r, t, n);
+    })(((e, r, t, n) => (f(e, t), s(r, 0, t, n)))), g = v(((e, r, t, n, o) => {
+        var a = r && E.o(r, t) && p(r, t, n);
         return a ? h(a) : o()
     })), y = {}, m = {
-        153: () => b("default", "@jupyterlab/ui-components", [1, 4, 1, 5]),
-        195: () => b("default", "@jupyterlab/completer", [1, 4, 1, 5]),
-        228: () => b("default", "@jupyterlab/coreutils", [1, 6, 1, 5]),
+        308: () => b("default", "@jupyterlab/docmanager", [1, 4, 1, 6]),
+        372: () => b("default", "@jupyterlab/notebook", [1, 4, 1, 6]),
+        465: () => b("default", "@jupyterlab/application", [1, 4, 1, 6]),
         473: () => g("default", "@msgpack/msgpack", [6, 3, 0, 0, , "beta2"], (() => E.e(7).then((() => () => E(7))))),
-        502: () => g("default", "remeda", [1, 1, 55, 0], (() => E.e(769).then((() => () => E(769))))),
-        743: () => b("default", "@jupyterlab/settingregistry", [1, 4, 1, 5]),
-        933: () => b("default", "@jupyterlab/notebook", [1, 4, 1, 5]),
-        976: () => b("default", "@jupyterlab/application", [1, 4, 1, 5]),
-        979: () => b("default", "@jupyterlab/services", [1, 7, 1, 5]),
-        989: () => b("default", "@jupyterlab/docmanager", [1, 4, 1, 5])
+        486: () => b("default", "@jupyterlab/services", [1, 7, 1, 6]),
+        502: () => g("default", "remeda", [1, 1, 55, 0], (() => E.e(537).then((() => () => E(537))))),
+        597: () => b("default", "@jupyterlab/coreutils", [1, 6, 1, 6]),
+        618: () => b("default", "@jupyterlab/settingregistry", [1, 4, 1, 6]),
+        664: () => b("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
+        886: () => b("default", "@jupyterlab/completer", [1, 4, 1, 6])
     }, w = {
-        336: [153, 195, 228, 473, 502, 743, 933, 976, 979, 989]
+        336: [308, 372, 465, 473, 486, 502, 597, 618, 664, 886]
     }, j = {}, E.f.consumes = (e, r) => {
         E.o(w, e) && w[e].forEach((e => {
             if (E.o(y, e)) return r.push(y[e]);
             if (!j[e]) {
                 var t = r => {
                     y[e] = 0, E.m[e] = t => {
                         delete E.c[e], t.exports = r()
@@ -293,20 +293,20 @@
                             i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, o, [a, i, u] = t,
-                    l = 0;
+                    f = 0;
                 if (a.some((r => 0 !== e[r]))) {
                     for (n in i) E.o(i, n) && (E.m[n] = i[n]);
                     u && u(E)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); f < a.length; f++) o = a[f], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkneopyter = self.webpackChunkneopyter || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), E.nc = void 0;
     var O = E(385);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).neopyter = O
 })();
```

### Comparing `neopyter-0.2.0/neopyter/labextension/static/third-party-licenses.json` & `neopyter-0.2.1/neopyter/labextension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'packages'": "{1: {'versionInfo': '6.11.0'}, 2: {'versionInfo': '1.59.0'}}"}*

```diff
@@ -6,21 +6,21 @@
             "name": "@msgpack/msgpack",
             "versionInfo": "3.0.0-beta2"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
-            "versionInfo": "6.10.0"
+            "versionInfo": "6.11.0"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) 2018 remeda\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "remeda",
-            "versionInfo": "1.56.0"
+            "versionInfo": "1.59.0"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
             "versionInfo": "3.3.4"
         }
```

### Comparing `neopyter-0.2.0/neopyter/tests/server/test_handlers.py` & `neopyter-0.2.1/neopyter/tests/server/test_handlers.py`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/plugin/neopyter.lua` & `neopyter-0.2.1/plugin/neopyter.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/queries/python/highlights.scm` & `neopyter-0.2.1/after/queries/python/injections.scm`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,25 @@
-; extends
+;; extends
 
+(
+ [
+  ((comment) @cellseparator.code
+             (#lua-match? @cellseparator.code "^# %%%%$"))
+  ((comment) @cellseparator.code
+             (#match? @cellseparator.code "^# [%]{2} ([[]\\w\+[]])\@!"))
+  ] @_start
+ (comment) @_end
+ (#make-range! "cell.code" @_start @_end)
+ )
 
-((comment) @cellseparator.code
-           (#lua-match? @cellseparator.code "^# %%%%$"))
-
-((comment) @cellseparator.code
-    (#match? @cellseparator.code "^# [%]{2} ([[]\\w\+[]])\@!"))
 
 ((comment) @cellseparator.markdown
-    . (expression_statement
-        (string 
-            (string_start) @cellborder.markdown
-            (string_content) @cellcontent.markdown
-            (string_end) @cellborder.markdown
-        )
-    )? @cellbody.markdown
-    (#match? @cellseparator.markdown "^# [%]{2} [[]\<markdown>|\<md>[]].*$")
-    (#match? @cellbody.markdown "^[\"']{3}.*[\"']{3}$"))
-
-
-((comment) @cellseparator.raw
-    . (expression_statement
-        (string
-            (string_start) @cellborder.raw
-            (string_content) @cellcontent.raw
-            (string_end) @cellborder.raw
-        )
-    )? @cellbody.raw
-    (#match? @cellseparator.raw "^# [%]{2} [[]\<raw>[]].*$")
-    (#match? @cellbody.raw "^[\"']{3}.*[\"']{3}$"))
-
-((comment) @cellseparator.special
-    . (expression_statement
-        (string
-            (string_start) @cellborder.special
-            (string_content) @cellcontent.special
-            (string_end) @cellborder.special
-        )
-    )? @cellbody.special
-    (#match? @cellseparator.special "^# [%]{2} [[](\<markdown>|\<md>|\<raw>)\@!\\w\+[]].*$")
-    (#match? @cellbody.special "^[\"']{3}.*[\"']{3}$"))
+           . (expression_statement
+               (string 
+                 (string_start) @cellborder.markdown
+                 (string_content) @cellcontent.markdown @injection.content
+                 (string_end) @cellborder.markdown
+                 (#set! injection.language "markdown")
+                 )
+               )? @cellbody.markdown
+           (#match? @cellseparator.markdown "^# [%]{2} [[]\<markdown>|\<md>[]].*$")
+           (#match? @cellbody.markdown "^[\"']{3}.*[\"']{3}$"))
```

### Comparing `neopyter-0.2.0/queries/python/textobjects.scm` & `neopyter-0.2.1/after/queries/python/textobjects.scm`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+;; extends
 
 ; first cell without separator
 (module
   .
   (_) @_non_header @_start
   .
   (_)* @_non_header @_end
```

### Comparing `neopyter-0.2.0/src/index.ts` & `neopyter-0.2.1/src/index.ts`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,32 @@
 import * as R from 'remeda';
 
 import { RpcServer, Dispatcher } from './rpcServer';
 import { WebsocketTransport } from './transport';
 import { StatusSidePanel } from './statusidepanel';
 import { statusPageIcon } from './icons';
 import { WindowedList } from '@jupyterlab/ui-components';
+import { IConfig } from './settings';
+import { DockPanel } from '@lumino/widgets';
+
+function triggerFocus(element: HTMLElement) {
+  const eventType = 'onfocusin' in element ? 'focusin' : 'focus';
+  const bubbles = 'onfocusin' in element;
+  let event;
+
+  if ('createEvent' in document) {
+    event = document.createEvent('Event');
+    event.initEvent(eventType, bubbles, true);
+  } else if ('Event' in window) {
+    event = new Event(eventType, { bubbles: bubbles, cancelable: true });
+  }
+
+  element.focus();
+  element.dispatchEvent(event as Event);
+}
 
 // Transfer Data
 type TCell = {
   cell_type: string;
   source: string;
 };
 
@@ -56,31 +74,22 @@
     sidebar.title.icon = statusPageIcon;
     app.shell.add(sidebar, 'right');
 
     if (restorer) {
       restorer.add(sidebar, '@neopyter/graphsidebar');
     }
 
-    const settings = ServerConnection.makeSettings();
-    const url = URLExt.join(settings.wsUrl, 'neopyter', 'channel');
-
-    let currentNotebookPanel: NotebookPanel | null = nbtracker.currentWidget;
-    labShell.currentChanged.connect(() => {
-      if (labShell.currentWidget instanceof NotebookPanel) {
-        currentNotebookPanel = labShell.currentWidget;
-      }
-    });
-
     const getNotebookModel = (path?: string) => {
       let notebookPanel;
       if (path) {
         notebookPanel = docmanager.findWidget(path) as unknown as NotebookPanel;
       }
       let notebook = notebookPanel?.content as Notebook | undefined;
       if (!notebook) {
+        const currentNotebookPanel = labShell.currentWidget as NotebookPanel;
         if (currentNotebookPanel?.isUntitled) {
           notebookPanel = currentNotebookPanel;
           notebook = notebookPanel.content;
         }
       }
       const sharedModel = notebook?.model?.sharedModel;
 
@@ -115,15 +124,15 @@
       },
       executeCommand: async (command: string, args?: ReadonlyPartialJSONObject) => {
         await app.commands.execute(command, args);
       }
     };
     const docmanagerDispatcher = {
       getCurrentNotebook: () => {
-        const notebookPanel = currentNotebookPanel;
+        const notebookPanel = labShell.currentWidget as NotebookPanel;
         if (notebookPanel) {
           const context = docmanager.contextForWidget(notebookPanel);
           return context?.localPath;
         }
       },
       isFileOpen: (path: string) => {
         return !!docmanager.findWidget(path);
@@ -145,18 +154,43 @@
       openFile: (path: string) => {
         return !!docmanager.open(path);
       },
       openOrReveal: (path: string) => {
         return !!docmanager.openOrReveal(path);
       },
       activateNotebook: (path: string) => {
+        // some hack code
         const { notebookPanel } = getNotebookModel(path);
         labShell.activateById(notebookPanel.id);
-        notebookPanel.node.focus();
-        currentNotebookPanel = notebookPanel;
+        notebookPanel.activate();
+        const emitEvent = (node: HTMLElement) => {
+          const event = new FocusEvent('focus', {
+            bubbles: true,
+            cancelable: true,
+            view: window
+          });
+          node.click();
+          node.dispatchEvent(event);
+          node.focus();
+          triggerFocus(node);
+        };
+        // @ts-expect-error hack private property
+        const dockPanel: DockPanel = labShell._dockPanel;
+
+        for (const tabBar of dockPanel.tabBars()) {
+          const tabIndex = tabBar.titles.findIndex(title => {
+            return title.owner === notebookPanel;
+          });
+          if (tabIndex >= 0) {
+            const tab = tabBar.contentNode.children[tabIndex] as HTMLElement;
+            emitEvent(tab);
+            break;
+          }
+        }
+        emitEvent(notebookPanel.node);
       },
       closeFile: async (path: string) => {
         return await docmanager.closeFile(path);
       },
       selectAbove: () => {
         const { notebook } = getNotebookModel();
         notebook && NotebookActions.selectBelow(notebook);
@@ -338,13 +372,27 @@
         }
       }
     };
 
     Object.assign(dispatcher, docmanagerDispatcher);
     Object.assign(dispatcher, notebookDispatcher);
     Object.assign(dispatcher, cellDispatcher);
-    const server = new RpcServer(dispatcher);
-    server.start(WebsocketTransport, url);
+
+    const startConnection = async () => {
+      const server = new RpcServer(dispatcher);
+
+      const { mode, ip, port } = (await settingRegistry.load('neopyter:labplugin')).composite as unknown as IConfig;
+      let url;
+      if (mode === 'proxy') {
+        const settings = ServerConnection.makeSettings();
+        url = URLExt.join(settings.wsUrl, 'neopyter', 'channel');
+        server.start(WebsocketTransport, url, false);
+      } else {
+        url = `ws://${ip}:${port}`;
+        server.start(WebsocketTransport, url, true);
+      }
+    };
+    startConnection();
   }
 };
 
 export default [neopyterPlugin];
```

### Comparing `neopyter-0.2.0/src/msgpackRpcProtocol.ts` & `neopyter-0.2.1/src/msgpackRpcProtocol.ts`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/src/rpcServer.ts` & `neopyter-0.2.1/src/rpcServer.ts`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/src/statusidepanel.ts` & `neopyter-0.2.1/src/statusidepanel.ts`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,68 @@
 import { URLExt } from '@jupyterlab/coreutils';
 import { ServerConnection } from '@jupyterlab/services';
 import { SidePanel } from '@jupyterlab/ui-components';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
-
-interface IConfig {
-  port?: number;
-  ip?: string;
-}
+import { IConfig } from './settings';
 
 export class StatusSidePanel extends SidePanel {
   constructor(private settingRegistry: ISettingRegistry) {
     super();
     this.id = 'neopyter-status-sidepanel';
     this.watchSettings();
   }
   async updatePanel() {
-    const settings = ServerConnection.makeSettings();
-    const url = URLExt.join(settings.baseUrl, 'neopyter', 'get_server_info');
-    const response = await fetch(url);
-
+    const settings = (await this.settingRegistry.load('neopyter:labplugin')).composite as unknown as IConfig;
     this.content.node.textContent = '';
-    if (!response.ok) {
-      const p = document.createElement('p');
-      this.content.node.appendChild(p);
-      p.textContent = 'Access API failed';
-      return;
-    }
-    const { code, message, data } = await response.json();
-    if (code !== 0) {
-      const p = document.createElement('p');
-      this.content.node.appendChild(p);
-      p.textContent = message;
-      return;
+    {
+      const h2 = document.createElement('h2');
+      this.content.node.appendChild(h2);
+      h2.textContent = `Work mode: ${settings.mode}`;
     }
-    for (const addr of data.addrs) {
-      const p = document.createElement('p');
-      this.content.node.appendChild(p);
-      p.textContent = addr;
+    if (settings.mode === 'proxy') {
+      const serverSettings = ServerConnection.makeSettings();
+      const url = URLExt.join(serverSettings.baseUrl, 'neopyter', 'get_server_info');
+      const response = await fetch(url);
+
+      if (!response.ok) {
+        const p = document.createElement('p');
+        this.content.node.appendChild(p);
+        p.textContent = 'Access API failed';
+        return;
+      }
+      const { code, message, data } = await response.json();
+      if (code !== 0) {
+        const p = document.createElement('p');
+        this.content.node.appendChild(p);
+        p.textContent = message;
+        return;
+      }
+      for (const addr of data.addrs) {
+        const p = document.createElement('p');
+        this.content.node.appendChild(p);
+        p.textContent = addr;
+      }
+    } else {
+      {
+        const p = document.createElement('p');
+        this.content.node.appendChild(p);
+        p.textContent = `IP: ${settings.ip}`;
+      }
+
+      {
+        const p = document.createElement('p');
+        this.content.node.appendChild(p);
+        p.textContent = `port: ${settings.port}`;
+      }
     }
   }
 
   async watchSettings() {
-    let config: IConfig = {};
     const updateSettings = async (settings: ISettingRegistry.ISettings) => {
-      config = settings.composite as IConfig;
+      const config = settings.composite as unknown as IConfig;
       console.log('updateSettings', config);
       const connectSettings = ServerConnection.makeSettings();
       const baseUrl = connectSettings.baseUrl;
       const url = URLExt.join(baseUrl, 'neopyter', 'update_settings');
       const response = await ServerConnection.makeRequest(
         url,
         {
```

### Comparing `neopyter-0.2.0/src/__tests__/neojupy.spec.ts` & `neopyter-0.2.1/src/__tests__/neojupy.spec.ts`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     expect(
       new Promise((resolve, reject) => {
         const server = new RpcServer({
           echo: (message: string) => {
             resolve(message);
           }
         });
-        server.start(WebsocketTransport, url);
+        server.start(WebsocketTransport, url, false);
         server.transport!.onRequest({
           type: MessageType.Request,
           msgid: 0,
           method: 'echo',
           params: ['World']
         });
         // mock
```

### Comparing `neopyter-0.2.0/src/dispatcher/docmanager.ts` & `neopyter-0.2.1/src/dispatcher/docmanager.ts`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/src/transport/base.ts` & `neopyter-0.2.1/src/transport/base.ts`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/src/transport/reverseHttpTransport.ts` & `neopyter-0.2.1/src/transport/reverseHttpTransport.ts`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/src/transport/websocketTransport.ts` & `neopyter-0.2.1/src/transport/websocketTransport.ts`

 * *Files 13% similar despite different names*

```diff
@@ -10,50 +10,58 @@
 
 function bytesToBase64(bytes: Uint8Array) {
   const binString = String.fromCodePoint(...bytes);
   return btoa(binString);
 }
 
 export class WebsocketTransport extends BaseTransport {
-  private websocket: WebSocket;
-  private readableStream: ReadableStream;
+  private websocket?: WebSocket;
+  private readableStream?: ReadableStream;
   constructor(
     server: RpcServer,
-    private url: string
+    private url: string,
+    private autoRetry: boolean
   ) {
     super(server);
-    this.websocket = new WebSocket(this.url);
-    this.websocket.binaryType = 'arraybuffer';
-    this.readableStream = new ReadableStream({
-      start: controller => {
-        // console.log('start');
-        this.websocket.addEventListener('open', event => {
-          this.onOpen(event);
-        });
-        this.websocket.addEventListener('message', event => {
-          const buf = base64ToBytes(event.data);
-          controller.enqueue(buf);
-        });
-
-        this.websocket.addEventListener('error', event => {
-          this.onError(event);
-          throw event;
-        });
-        this.websocket.addEventListener('close', event => {
-          this.onClose(event);
-          controller.close();
-        });
-      }
-    });
-    setTimeout(async () => {
+    this.start();
+  }
+  async start() {
+    try {
+      this.websocket = new WebSocket(this.url);
+      this.websocket.binaryType = 'arraybuffer';
+      this.readableStream = new ReadableStream({
+        start: controller => {
+          // console.log('start');
+          this.websocket!.addEventListener('open', event => {
+            this.onOpen(event);
+          });
+          this.websocket!.addEventListener('message', event => {
+            const buf = base64ToBytes(event.data);
+            controller.enqueue(buf);
+          });
+
+          this.websocket!.addEventListener('error', event => {
+            this.onError(event);
+            throw event;
+          });
+          this.websocket!.addEventListener('close', event => {
+            this.onClose(event);
+            controller.close();
+          });
+        }
+      });
       for await (const message of deserializeStream(this.readableStream)) {
         // console.log(message);
         this.onRead(message);
       }
-    }, 0);
+    } catch (e) {
+      console.error(e);
+      this.checkRetry();
+      throw e;
+    }
   }
 
   async onRead(message: Message) {
     switch (message.type) {
       case MessageType.Request:
         await this.onRequest(message);
         break;
@@ -62,20 +70,37 @@
         break;
       default:
         throw new RPCError(`Unknown message: ${message}`);
     }
   }
 
   sendData(data: Uint8Array): void {
-    this.websocket.send(bytesToBase64(data));
+    this.websocket!.send(bytesToBase64(data));
   }
 
   protected onOpen(_event: Event) {
-    console.log(`Connection to neopyter jupyter server by websocket ${this.websocket.url}`);
+    console.log(`Connection to neopyter jupyter server by websocket ${this.websocket!.url}`);
   }
   protected onError(event: Event) {
     console.error('Websocket error', event);
   }
   protected onClose(_event: Event) {
-    console.log(`DisConnection to neopyter jupyter server by websocket ${this.websocket.url}`);
+    console.log(`Disconnect to neopyter jupyter server by websocket ${this.websocket!.url}`);
+    this.websocket!.close();
+    this.websocket = undefined;
+    this.readableStream = undefined;
+    this.checkRetry();
+  }
+
+  protected checkRetry() {
+    if (this.autoRetry && this.websocket === undefined) {
+      console.log('reconnect websocket server after 1s');
+      setTimeout(() => {
+        if (this.autoRetry && this.websocket === undefined) {
+          this.start();
+        } else {
+          console.error('checkRetry repeat');
+        }
+      }, 1000);
+    }
   }
 }
```

### Comparing `neopyter-0.2.0/style/icons/statuspage.svg` & `neopyter-0.2.1/style/icons/statuspage.svg`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/.gitignore` & `neopyter-0.2.1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -122,7 +122,10 @@
 .DS_Store
 
 # Yarn cache
 .yarn/
 
 # jest
 junit.xml
+
+doc/tags
+yarn.lock
```

### Comparing `neopyter-0.2.0/LICENSE` & `neopyter-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/README.md` & `neopyter-0.2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,77 @@
 # JupyterLab + Neovim
 
 - A JupyterLab extension.
 - A Neovim plugin
 
 ## How does it work?
 
-![](./doc/communication.png)
+This project includes two parts: a [`JupyterLab extension`](https://jupyterlab.readthedocs.io/en/stable/user/extensions.html) and a Neovim plugin
 
-The `Jupyter lab`'s frontend plugin provides RPC service which expose functions of `Jupyter lab`, Jupyterlab server
-forward these RPC service by TCP Server. `Neovim`s plugin connect to TCP Server and call RPC service when receive events
-from `Neovim` via `autocmd`. In the end, `Neopyter` can control `Juppyter lab`. `Neopyter` can implement more ability like [jupynium.nvim](https://github.com/kiyoon/jupynium.nvim), but better performance.
+- The `JupyterLab extension` exposes functions of `Jupyter lab`, and provides a remote procedure call(RPC) service
+- The `Neovim plugin` calls the RPC service when it receives events from `Neovim` via `autocmd`
+
+|                           proxy                            |                            direct                            |
+| :--------------------------------------------------------: | :----------------------------------------------------------: |
+| <img alt="proxy mode" src="./doc/communication_proxy.png"> | <img alt="direct mode" src="./doc/communication_direct.png"> |
+
+This project provides two working modes for different network environments. If the browser where your jupyiter lab is
+located cannot directly access nvim, you must use `proxy` mode; If you need to collaborate and use the same Jupyter with
+others, you must use direct mode
+
+- `proxy` mode: Jupyterlab server
+  proxies the RPC service as a TCP server which `Neovim`s plugin connects to
+- `direct` mode: Neovim plugin accesses these RPC service directly
+
+Ultimately, `Neopyter` can control `Juppyter lab`. `Neopyter` can implement abilities like [jupynium.nvim](https://github.com/kiyoon/jupynium.nvim).
 
 ## Screenshots
 
 |                    Completion                     |                    Cell Magic                     |                    Line Magic                     |
 | :-----------------------------------------------: | :-----------------------------------------------: | :-----------------------------------------------: |
 | <img alt="Completion" src="./doc/completion.png"> | <img alt="Cell Magic" src="./doc/cell_magic.png"> | <img alt="Line Magic" src="./doc/line_magic.png"> |
 
-## Installation
-
-### Requirements
+## Requirements
 
 - 📔JupyterLab >= 4.0.0
-- ✌️ Neovim >= 9.0
+- ✌️ Neovim nightly
   - 👍`nvim-lua/plenary.nvim`
+  - 🤏`AbaoFromCUG/websocket.nvim` (optional for `mode="proxy"`)
+
+## Installation
 
 ### JupyterLab Extension
 
 To install the jupyterlab extension, execute:
 
 ```bash
 pip install neopyter
 ```
 
-To remove the extension, execute:
+Configure `JupyterLab` in menu `Settings`>`Settings Editor`>`Neopyter`
 
-```bash
-pip uninstall neopyter
-```
+- `mode`: refer to the previous introduction about mode
+- `IP`: if `mode=proxy`, set to the IP of the host where jupyter is located. If `proxy=direct`, set to the IP of the
+  host where neovim is located
+- `port`: idle port
 
 ### Neovim plugin
 
 With 💤lazy.nvim:
 
 ```lua
 {
     "SUSTech-data/neopyter",
     opts = {
         -- auto define autocmd
         auto_attach = true,
-        -- auto connect server
+        -- auto connect rpc service
         auto_connect = true,
-        -- your jupyter host + neopyter port
+        mode="direct",
+        -- same with JupyterLab settings
         remote_address = "127.0.0.1:9001",
         file_pattern = { "*.ju.*" },
         on_attach = function(bufnr)
         end,
 
         highlight = {
             enable = true,
@@ -139,17 +155,22 @@
 - @cellcontent
   - @cellcontent.code
   - @cellcontent.magic
   - @cellcontent.markdown
   - @cellcontent.raw
   - @cellcontent.special
 - @cellborder
-  - @cellborder.markdown
-  - @cellborder.raw
-  - @cellborder.special
+  - @cellborder.start
+    - @cellborder.start.markdown
+    - @cellborder.start.raw
+    - @cellborder.start.special
+  - @cellborder.end
+    - @cellborder.end.markdown
+    - @cellborder.end.raw
+    - @cellborder.end.special
 - @linemagic
 
 ```lua
 require'nvim-treesitter.configs'.setup {
     textobjects = {
         move = {
             enable = true,
@@ -167,15 +188,14 @@
 
 ```
 
 ## Quick Start
 
 - Open JupyterLab `jupyter lab`, there is a sidebar named `Neopyter`, which display neopyter ip+port
 - Open a `*.ju.py` file in neovim
-- [Optional] if `auto_attach` is `false`, you can connect jupyterlab manually via `:Neopyter connect 127.0.0.1:9001`
 - Now you can type `# %%` in Neovim to create a code cell.
   - You'll see everything you type below that will be synchronised in the browser
 
 ### Available Vim Commands
 
 - Server
   - `:Neopyter connect [remote 'ip:port']`, e.g. `:Neopyter command 127.0.0.1:9001`, connect `Jupyter lab` manually
@@ -259,77 +279,7 @@
         `vim.rpcrequest` and `vim.rpcnotify`
 - Document
   - [ ] API Document
 
 ## Acknowledges
 
 - [jupynium.nvim](https://github.com/kiyoon/jupynium.nvim): Selenium-automated Jupyter Notebook that is synchronised with NeoVim in real-time.
-
-## Contributing
-
-### JupyterLab Extension
-
-#### Development install
-
-Note: You will need `NodeJS` to build the extension package. Recommend use `pnpm`
-
-```bash
-# Clone the repo to your local environment
-# Change directory to the current project directory
-# Install package in development mode
-pip install -e "."
-# Link your development version of the extension with JupyterLab
-jupyter labextension develop . --overwrite
-# Rebuild extension Typescript source after making changes
-pnpm build
-```
-
-You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
-
-```bash
-# Watch the source directory in one terminal, automatically rebuilding when needed
-pnpm watch
-# Run JupyterLab in another terminal
-jupyter lab
-```
-
-With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).
-
-By default, the `pnpm build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
-
-```bash
-jupyter lab build --minimize=False
-```
-
-#### Development uninstall
-
-```bash
-pip uninstall neopyter
-```
-
-In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
-command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
-folder is located. Then you can remove the symlink named `neopyter` within that folder.
-
-#### Testing the extension
-
-##### Frontend tests
-
-This extension is using [Jest](https://jestjs.io/) for JavaScript code testing.
-
-To execute them, execute:
-
-```sh
-pnpm install
-pnpm test
-```
-
-##### Integration tests
-
-This extension uses [Playwright](https://playwright.dev/docs/intro) for the integration tests (aka user level tests).
-More precisely, the JupyterLab helper [Galata](https://github.com/jupyterlab/jupyterlab/tree/master/galata) is used to handle testing the extension in JupyterLab.
-
-More information are provided within the [ui-tests](./ui-tests/README.md) README.
-
-#### Packaging the extension
-
-See [RELEASE](RELEASE.md)
```

### Comparing `neopyter-0.2.0/pyproject.toml` & `neopyter-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.0/PKG-INFO` & `neopyter-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: neopyter
-Version: 0.2.0
+Version: 0.2.1
 Dynamic: Keywords
 Summary: A JupyterLab extension. Integrate JupyterLab and Neovim
 Project-URL: Homepage, https://github.com/SUSTech-data/neopyter
 Project-URL: Bug Tracker, https://github.com/SUSTech-data/neopyter/issues
 Project-URL: Repository, https://github.com/SUSTech-data/neopyter
 Author-email: Abao Zhang <abaodoit@gmail.com>
 License: BSD 3-Clause License
@@ -64,61 +64,77 @@
 # JupyterLab + Neovim
 
 - A JupyterLab extension.
 - A Neovim plugin
 
 ## How does it work?
 
-![](./doc/communication.png)
+This project includes two parts: a [`JupyterLab extension`](https://jupyterlab.readthedocs.io/en/stable/user/extensions.html) and a Neovim plugin
 
-The `Jupyter lab`'s frontend plugin provides RPC service which expose functions of `Jupyter lab`, Jupyterlab server
-forward these RPC service by TCP Server. `Neovim`s plugin connect to TCP Server and call RPC service when receive events
-from `Neovim` via `autocmd`. In the end, `Neopyter` can control `Juppyter lab`. `Neopyter` can implement more ability like [jupynium.nvim](https://github.com/kiyoon/jupynium.nvim), but better performance.
+- The `JupyterLab extension` exposes functions of `Jupyter lab`, and provides a remote procedure call(RPC) service
+- The `Neovim plugin` calls the RPC service when it receives events from `Neovim` via `autocmd`
+
+|                           proxy                            |                            direct                            |
+| :--------------------------------------------------------: | :----------------------------------------------------------: |
+| <img alt="proxy mode" src="./doc/communication_proxy.png"> | <img alt="direct mode" src="./doc/communication_direct.png"> |
+
+This project provides two working modes for different network environments. If the browser where your jupyiter lab is
+located cannot directly access nvim, you must use `proxy` mode; If you need to collaborate and use the same Jupyter with
+others, you must use direct mode
+
+- `proxy` mode: Jupyterlab server
+  proxies the RPC service as a TCP server which `Neovim`s plugin connects to
+- `direct` mode: Neovim plugin accesses these RPC service directly
+
+Ultimately, `Neopyter` can control `Juppyter lab`. `Neopyter` can implement abilities like [jupynium.nvim](https://github.com/kiyoon/jupynium.nvim).
 
 ## Screenshots
 
 |                    Completion                     |                    Cell Magic                     |                    Line Magic                     |
 | :-----------------------------------------------: | :-----------------------------------------------: | :-----------------------------------------------: |
 | <img alt="Completion" src="./doc/completion.png"> | <img alt="Cell Magic" src="./doc/cell_magic.png"> | <img alt="Line Magic" src="./doc/line_magic.png"> |
 
-## Installation
-
-### Requirements
+## Requirements
 
 - 📔JupyterLab >= 4.0.0
-- ✌️ Neovim >= 9.0
+- ✌️ Neovim nightly
   - 👍`nvim-lua/plenary.nvim`
+  - 🤏`AbaoFromCUG/websocket.nvim` (optional for `mode="proxy"`)
+
+## Installation
 
 ### JupyterLab Extension
 
 To install the jupyterlab extension, execute:
 
 ```bash
 pip install neopyter
 ```
 
-To remove the extension, execute:
+Configure `JupyterLab` in menu `Settings`>`Settings Editor`>`Neopyter`
 
-```bash
-pip uninstall neopyter
-```
+- `mode`: refer to the previous introduction about mode
+- `IP`: if `mode=proxy`, set to the IP of the host where jupyter is located. If `proxy=direct`, set to the IP of the
+  host where neovim is located
+- `port`: idle port
 
 ### Neovim plugin
 
 With 💤lazy.nvim:
 
 ```lua
 {
     "SUSTech-data/neopyter",
     opts = {
         -- auto define autocmd
         auto_attach = true,
-        -- auto connect server
+        -- auto connect rpc service
         auto_connect = true,
-        -- your jupyter host + neopyter port
+        mode="direct",
+        -- same with JupyterLab settings
         remote_address = "127.0.0.1:9001",
         file_pattern = { "*.ju.*" },
         on_attach = function(bufnr)
         end,
 
         highlight = {
             enable = true,
@@ -202,17 +218,22 @@
 - @cellcontent
   - @cellcontent.code
   - @cellcontent.magic
   - @cellcontent.markdown
   - @cellcontent.raw
   - @cellcontent.special
 - @cellborder
-  - @cellborder.markdown
-  - @cellborder.raw
-  - @cellborder.special
+  - @cellborder.start
+    - @cellborder.start.markdown
+    - @cellborder.start.raw
+    - @cellborder.start.special
+  - @cellborder.end
+    - @cellborder.end.markdown
+    - @cellborder.end.raw
+    - @cellborder.end.special
 - @linemagic
 
 ```lua
 require'nvim-treesitter.configs'.setup {
     textobjects = {
         move = {
             enable = true,
@@ -230,15 +251,14 @@
 
 ```
 
 ## Quick Start
 
 - Open JupyterLab `jupyter lab`, there is a sidebar named `Neopyter`, which display neopyter ip+port
 - Open a `*.ju.py` file in neovim
-- [Optional] if `auto_attach` is `false`, you can connect jupyterlab manually via `:Neopyter connect 127.0.0.1:9001`
 - Now you can type `# %%` in Neovim to create a code cell.
   - You'll see everything you type below that will be synchronised in the browser
 
 ### Available Vim Commands
 
 - Server
   - `:Neopyter connect [remote 'ip:port']`, e.g. `:Neopyter command 127.0.0.1:9001`, connect `Jupyter lab` manually
@@ -322,77 +342,7 @@
         `vim.rpcrequest` and `vim.rpcnotify`
 - Document
   - [ ] API Document
 
 ## Acknowledges
 
 - [jupynium.nvim](https://github.com/kiyoon/jupynium.nvim): Selenium-automated Jupyter Notebook that is synchronised with NeoVim in real-time.
-
-## Contributing
-
-### JupyterLab Extension
-
-#### Development install
-
-Note: You will need `NodeJS` to build the extension package. Recommend use `pnpm`
-
-```bash
-# Clone the repo to your local environment
-# Change directory to the current project directory
-# Install package in development mode
-pip install -e "."
-# Link your development version of the extension with JupyterLab
-jupyter labextension develop . --overwrite
-# Rebuild extension Typescript source after making changes
-pnpm build
-```
-
-You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
-
-```bash
-# Watch the source directory in one terminal, automatically rebuilding when needed
-pnpm watch
-# Run JupyterLab in another terminal
-jupyter lab
-```
-
-With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).
-
-By default, the `pnpm build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
-
-```bash
-jupyter lab build --minimize=False
-```
-
-#### Development uninstall
-
-```bash
-pip uninstall neopyter
-```
-
-In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
-command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
-folder is located. Then you can remove the symlink named `neopyter` within that folder.
-
-#### Testing the extension
-
-##### Frontend tests
-
-This extension is using [Jest](https://jestjs.io/) for JavaScript code testing.
-
-To execute them, execute:
-
-```sh
-pnpm install
-pnpm test
-```
-
-##### Integration tests
-
-This extension uses [Playwright](https://playwright.dev/docs/intro) for the integration tests (aka user level tests).
-More precisely, the JupyterLab helper [Galata](https://github.com/jupyterlab/jupyterlab/tree/master/galata) is used to handle testing the extension in JupyterLab.
-
-More information are provided within the [ui-tests](./ui-tests/README.md) README.
-
-#### Packaging the extension
-
-See [RELEASE](RELEASE.md)
```

