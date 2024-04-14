# Comparing `tmp/sshpyk-0.13.tar.gz` & `tmp/sshpyk-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshpyk-0.13.tar", last modified: Sun Apr 14 17:58:01 2024, max compression
+gzip compressed data, was "sshpyk-0.9.tar", last modified: Thu Apr 11 22:23:11 2024, max compression
```

## Comparing `sshpyk-0.13.tar` & `sshpyk-0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2024-04-14 17:57:40.729201 sshpyk-0.13/LICENSE
--rw-r--r--   0        0        0     8916 2024-04-14 17:57:40.729201 sshpyk-0.13/README.rst
--rw-r--r--   0        0        0      560 2024-04-14 17:57:40.729201 sshpyk-0.13/pyproject.toml
--rw-r--r--   0        0        0     3420 2024-04-14 17:57:40.729201 sshpyk-0.13/sshpyk/__init__.py
--rw-r--r--   0        0        0     5080 2024-04-14 17:57:40.729201 sshpyk-0.13/sshpyk/__main__.py
--rw-r--r--   0        0        0     1934 2024-04-14 17:57:40.729201 sshpyk-0.13/sshpyk/kernel/add.py
--rw-r--r--   0        0        0     4227 2024-04-14 17:57:40.729201 sshpyk-0.13/sshpyk/kernel/ls.py
--rw-r--r--   0        0        0     9173 1970-01-01 00:00:00.000000 sshpyk-0.13/PKG-INFO
+-rw-r--r--   0        0        0     1516 2024-04-11 22:22:50.384929 sshpyk-0.9/LICENSE
+-rw-r--r--   0        0        0     8855 2024-04-11 22:22:50.384929 sshpyk-0.9/README.rst
+-rw-r--r--   0        0        0      536 2024-04-11 22:22:50.384929 sshpyk-0.9/pyproject.toml
+-rw-r--r--   0        0        0     3011 2024-04-11 22:22:50.384929 sshpyk-0.9/sshpyk/__init__.py
+-rw-r--r--   0        0        0     4521 2024-04-11 22:22:50.384929 sshpyk-0.9/sshpyk/__main__.py
+-rw-r--r--   0        0        0     1762 2024-04-11 22:22:50.384929 sshpyk-0.9/sshpyk/kernel/add.py
+-rw-r--r--   0        0        0     4972 2024-04-11 22:22:50.384929 sshpyk-0.9/sshpyk/kernel/ls.py
+-rw-r--r--   0        0        0     9088 1970-01-01 00:00:00.000000 sshpyk-0.9/PKG-INFO
```

### Comparing `sshpyk-0.13/LICENSE` & `sshpyk-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sshpyk-0.13/README.rst` & `sshpyk-0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,37 @@
+Metadata-Version: 2.1
+Name: sshpyk
+Version: 0.9
+Summary: remote jupyter kernels via ssh tunnels
+License: BSD-3-Clause
+Author-email: Darrell Schiebel <darrell@schiebel.us>
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+
 Remote Jupyter Kernels via SSH tunnels
 ######################################
 
-The design of this pakage is based upon `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ which
-in turn is based upon `remote_ikernel <https://bitbucket.org/tdaff/remote_ikernel>`_. This implementation shares
-a common set of command line parameters with `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_, but it was
-implemented from scratch to adapt to recent changes to :code:`jupyter_client` (which broke :code:`ssh_ipykernel`)
-and to support Python 3.10. This package adds an :code:`ls` implementation which allows listing info about the
-available kernel specifications.
+The design of this pakage is based upon `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ which is
+in turn based upon `remote_ikernel <https://bitbucket.org/tdaff/remote_ikernel>`_. This implementation shares
+the same command line parameters as `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_, but it was
+reimplemented from scratch to support Python 3.10. It also includes an :code:`ls` implementation which allows
+checking on the available kernel specifications.
 
 While there are modest additions to `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_, there are
-also modest subtractions. There are fewer configuration options for things like the internal name used
-by `Jupyter Client <https://jupyter-client.readthedocs.io/en/stable/#>`_ to refer to the created
-kernel.
+also modest subtractions. There are fewer configuration options for things like the name that
+`Jupyter Client <https://jupyter-client.readthedocs.io/en/stable/#>`_ uses to refer to the
+kernel. This is still based on the kernel description that the user sees, but the entire name
+is no longer completely configurable.
 
 Listing the Jupyter Kernels that are available
 **********************************************
 
-It can be difficult to know which Jupyter Kernels are available because there are multiple locations where
+It can be difficult to know which Jupyter Kernels are available because there is more than one location that
 the `Kernel Spec files <https://jupyter-client.readthedocs.io/en/latest/kernels.html#kernel-specs>`_ can be
-found. :code:`sshpyk` has an :code:`ls` option which lists the kernels that are available (even those which are
+stored. :code:`sshpyk` has an :code:`ls` option to all for seeing which kernels are available (even if they are
 **not** `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ or :code:`sshpyk` kernels::
 
   bash$
   bash$ python -m sshpyk.kernel.ls --no-check -a
   python3                                   /Users/drs/develop/python/conda/envs/py310/share/jupyter/kernels/python3
   python3.8                                 /usr/local/share/jupyter/kernels/python3.8
   python3dbg                                /Users/drs/Library/Jupyter/kernels/python3dbg
@@ -32,20 +41,19 @@
   bash$
 
 The :code:`--no-check` (or alternatively :code:`-nc`) flag indicates that the validity of the kernel spec files
 should **not** be checked. The :code:`-a` (or :code:`--all`) flag indicates that it should show **all** kernel
 specifications rather than just the ones for `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ or
 :code:`sshpyk` kernel specification files.
 
-If :code:`--no-check` is **not** supplied, part of listing the kernel information will include 
+If :code:`--no-check` is **not** supplied, then as part of listing the kernel information :code:`sshpyk` will
 verify that the Python executable specified in the kernel specification exist on the local and remote systems.
-This check allows the ouput to be colorized so red text indicates a problem. :code:`--local` will limit the
-check to just the local Python executable and :code:`--remote` will limit the check to only the remote Python
-executable. These options also list the local or remote Python path **instead** of the path to the kernel
-specification directory.
+:code:`--local` will limit the check to just the local Python executable and :code:`--remote` will limit the
+check to only the remote Python executable. These options also list the local or remote Python path **instead**
+of the path to the kernel specification directory.
 
 
 Command line "ls" options
 =========================
 
 The following options are available for listing the Jupyter kernel specifications:
 
@@ -106,15 +114,15 @@
   bash$
 
 Unlike the example above, here we have asked that the remote Python path be displayed
 instead of showing the kernel specificaton directory. Since we again asked that *all kernels*
 be displayed instead of only the SSH kernels, a Python path is displayed for the
 non-SSH kernels, but it is the local Python path as indicated by :code:`localhost:`.
 Because these three kernels are non-SSH kernels this is the only Python path that is
-available. However for the SSH kernels, we can see the remote Python path listed.
+available. However for the SSH kernels, we can see the remote Pyton path listed.
 These paths are prefixed with the hostname, here :code:`host06:`. We can also see
 the newly added kernel listed as :code:`ssh_host06_host06kernel`. This name is an internal
 name created from the :code:`--display-name` string which the end user will typically
 never see.
 
 Command line "add" options
 ==========================
@@ -183,7 +191,8 @@
 is on some protected network behind :code:`ssh.example.com`. When the *local* account
 runs :code:`ssh host06`, SSH will first connect as :code:`BASTION-USERNAME` on
 :code:`ssh.example.com` and then it connect to host :code:`host06` as username
 :code:`HOST06-USERNAME`.
 
 This sort of configuration will allow :code:`host06` to be allowed as a hostname
 for remote kernels.
+
```

### Comparing `sshpyk-0.13/pyproject.toml` & `sshpyk-0.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "sshpyk"
 dynamic = []
 description = "remote jupyter kernels via ssh tunnels"
 authors = [
-    { name = "National Radio Astronomy Observatory", email = "casa-feedback@nrao.edu" },
+    { name = "Darrell Schiebel", email = "darrell@schiebel.us" },
 ]
 dependencies = [
     "jupyter-client",
 ]
 requires-python = ">=3.8"
 readme = "README.rst"
-version = "0.13"
+version = "0.9"
 
 [project.license]
 text = "BSD-3-Clause"
 
 [tool.pdm.build]
 
 [tool.pdm.version]
```

### Comparing `sshpyk-0.13/sshpyk/__init__.py` & `sshpyk-0.9/sshpyk/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from jupyter_client import kernelspec as ks
 from subprocess import run, PIPE
 from getpass import getuser
 from shutil import which
-from os.path import join
 from json import dump
 import tempfile
-import json
 import sys
 import re
 import os
 
 try:
     from .__version__ import __version__
     _VERSION = __version__
@@ -92,17 +90,10 @@
         with open(os.path.join(temp_dir, "kernel.json"), "w") as fd:
             dump(kernel_json, fd, sort_keys=True, indent=2)
 
         ks.install_kernel_spec( temp_dir, kernel_name, user=False if system else getuser( ), replace=True )
 
     return kernel_name
     
-def get_kernel_desc( all=False ):
-    def _json( kernel_path ):
-        with open( join( kernel_path, 'kernel.json' ) ) as f:
-            return json.load(f)
-        return None
-
+def ls_kernel( ):
     km = ks.KernelSpecManager( )
-    kdirs = km.find_kernel_specs( )
-    keys = sorted( kdirs.keys( ) if all else filter( lambda k: k.startswith('ssh_'), kdirs.keys( ) ) )
-    return { k: { 'ssh': k.startswith("ssh_"), 'path': kdirs[k], 'spec': _json(kdirs[k]) } for k in keys }
+    return km.find_kernel_specs( )
```

### Comparing `sshpyk-0.13/sshpyk/__main__.py` & `sshpyk-0.9/sshpyk/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import os
-import sys
 import json
 from os import execvp
-from pathlib import Path
 from functools import reduce as fold
 from uuid import uuid4
 from shutil import which
 from os.path import isfile, join
 from argparse import ArgumentParser, SUPPRESS
 from subprocess import run, PIPE
 
@@ -20,74 +18,60 @@
 write_connection_file(fname=fname, ip="{ip}", key=b"{key}", transport="{transport}", signature_scheme="{signature_scheme}", kernel_name="{kernel_name}")
 fd = open(fname, "r")
 ci = fd.read()
 fd.close()
 print(ci)
 """
 
-def store( conf ):
-    path = join( Path.home( ), '.sshpyk', 'sessions', conf['host'] )
-    try:
-        ### umask modifies mode parameter of makedirs...
-        ### however, umask=0 and mode=0o700 gives EVERYONE R/W/X permission...
-        original_umask = os.umask(0o077)
-        os.makedirs( path, exist_ok=True )
-    finally:
-        os.umask(original_umask)
-    with open( join( path, f'''{conf['id']}.json''' ), "w" ) as f:
-        json.dump( conf, f )
-
-def main( host, python, connection_info, env, session ):
+def main( host, python, connection_info, env ):
     ssh = which('ssh')
-    remote_id = uuid4( )
-    remote_kernel_file = f'''/tmp/.sshpyk_{remote_id}.json'''
+    remote_kernel_file = f'''/tmp/.sshpyk_{uuid4( )}.json'''
     substituted_script = KERNEL_SCRIPT.format(fname=remote_kernel_file, **connection_info)
     script = '; '.join(substituted_script.strip( ).split("\n"))
 
     ###
     ### Create remote kernel file with port information...
     ###
     result = run( [ ssh, host, f"""{python} -c '{script}'""" ], stdout=PIPE, stderr=PIPE )
     remote_state = json.loads(result.stdout.decode('utf-8'))
-
-    if session:
-        store( { 'host': host, 'id': str(remote_id),
-                 'paths': { 'ssh': ssh, 'remote py': python, 'local py': sys.executable, 'remote kernel file': remote_kernel_file },
-                 'connect': { 'local': connection_info, 'remote': remote_state } } )
-
+    f = open( "/tmp/out.txt", "w" )
+    print( '--------------------------------------------------------------------------------', file=f )
+    print( repr(remote_state), file=f )
+    print( '--------------------------------------------------------------------------------', file=f )
     if type(remote_state) != dict or len(remote_state) <= 0:
         exit( 'Creation of remote ipykernel state failed.' )
 
     ###
     ### Launch kernel on remote system with SSH tunnels between the local ports
     ### and the remote ports... tunnel format is '-L {local}:IP:{remote}' where
     ### IP is one of 127.0.0.1 or localhost (not sure if this is referring to
     ### the local or remote host...
     ###
     ### This also removes the kernel configuration file after the ipykernel exits...
     ###
     ssh_env = env if env else [ ]
     ssh_tunnels = fold( lambda acc,k: [ '-L', f'''{connection_info[k]}:{connection_info['ip']}:{remote_state[k]}''' ] + acc,
                         filter( lambda k: k.endswith('_port'), remote_state.keys() ), [] )
-
-    execvp( ssh, [ 'ssh', '-q', '-t', *ssh_tunnels, host, f'''{' '.join(ssh_env)} {python} -m ipykernel_launcher --HistoryManager.hist_file=:memory: -f {remote_kernel_file}; echo {remote_id} $? >> "/tmp/.sshpyk_status.$USER.txt"; rm -f {remote_kernel_file}''' ] )
+    print( repr( ssh_tunnels ), file=f )
+    print( '--------------------------------------------------------------------------------', file=f )
+    f.close( )
+    execvp( ssh, [ 'ssh', '-q', '-t', *ssh_tunnels, host, f'''{' '.join(ssh_env)} {python} -m ipykernel_launcher --HistoryManager.hist_file=:memory: -f {remote_kernel_file}; rm -f {remote_kernel_file}''' ] )
 
 if __name__ == "__main__":
     parse = ArgumentParser( add_help=False )
     optional = parse.add_argument_group("optional arguments")
 
     ### prevents --help from appearing in it's own "options:" group
     optional.add_argument( "--help", "-h", action="help", default=SUPPRESS, help="show this help message and exit" )
     optional.add_argument( "--version", action='version', version=f'''sshrpy {version( )}''' )
 
     optional.add_argument( "--timeout", "-t", type=int, help="timeout for remote commands", default=5 )
     optional.add_argument( "--name", "-n", type=str, help="kernel name" )
     optional.add_argument( "--env", "-e", nargs="*",
                            help="environment variables for the remote kernel in the form: VAR1=value1 VAR2=value2" )
-    optional.add_argument( "--session", action="store_true", help="store session information for this kernel" )
     optional.add_argument( "-s", action="store_true", help="sudo required to start kernel on the remote machine" )
 
 
     required = parse.add_argument_group("required arguments")
     required.add_argument( "--file", "-f", required=True, help="jupyter kernel connection file" )
     required.add_argument( "--host", "-H", required=True, help="remote host" )
     required.add_argument( "--python", "-p", required=True, help="remote python_path" )
@@ -106,8 +90,8 @@
 
     ## seems like newer versions of the connection file do not include 'kernel_name'
     if args.name is not None:
         connection_info['kernel_name'] = args.name
     elif 'kernel_name' not in connection_info:
         connection_info['kernel_name'] = f'''ipykrn{os.getpid( )}'''
 
-    main( args.host, join(args.python, 'bin', 'python'), connection_info, args.env, args.session )
+    main( args.host, join(args.python, 'bin', 'python'), connection_info, args.env )
```

### Comparing `sshpyk-0.13/sshpyk/kernel/add.py` & `sshpyk-0.9/sshpyk/kernel/add.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,21 +13,19 @@
     parse = ArgumentParser( add_help=False )
     optional = parse.add_argument_group("optional arguments")
 
     optional.add_argument( "--help", "-h", action="help", default=SUPPRESS, help="show this help message and exit" )
     optional.add_argument( "--timeout", "-t", type=int, default=5, help="specify timeout to use" )
     optional.add_argument( "--env", "-e", type=_assignment, nargs='*', default=[], help='add environment variable to set in the form: "NAME=VALUE"' )
     optional.add_argument( "--display-name", "-d", type=str, default=None, help='string which will be used to describe this kernel' )
-    optional.add_argument( "--session" action="store_true", help="signal that session information should be stored for this kernel" )
     optional.add_argument( "--sudo", "-s", action="store_true", help="sudo required to start kernel on remote machine" )
 
     required = parse.add_argument_group("required arguments")
     required.add_argument( "--host", "-H", required=True, help="name of remote host (as used to connect with ssh)" )
     required.add_argument( "--python", "-p", required=True, help='path to remote python installation ("PATH/bin/python" would be the python executable)' )
 
     args = parse.parse_args( )
     if args.display_name is None:
         args.display_name = f'''{args.host}: {args.python}'''
 
     add_kernel( args.host, args.display_name, args.python,
-                env=args.env, sudo=args.sudo, system=args.sudo,
-                timeout=args.timeout, session=args.session )
+                env=args.env, sudo=args.sudo, system=args.sudo, timeout=args.timeout )
```

### Comparing `sshpyk-0.13/sshpyk/kernel/ls.py` & `sshpyk-0.9/sshpyk/kernel/ls.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 from argparse import ArgumentParser, SUPPRESS
 from os.path import join, exists, basename
 from subprocess import run, PIPE
 from shutil import which
+import json
 
 def _red( s ):
     return f'''\033[31m{s}\033[0m'''
 
+def _json( kernel_path ):
+    with open( join( kernel_path, 'kernel.json' ) ) as f:
+        return json.load(f)
+    return None
+
 def _remote_exe( argv ):
     result = [None,None]
     for p in zip(argv[1:][::2],argv[2:][::2]):
         if p[0] == '--python' or p[0] == "-p":
             result[0] = f'''{p[1]}/bin/python''' if len(p[1]) > 0 else None
         if p[0] == '--host' or p[0] == "-H":
             result[1] = p[1]
     return result
 
-def _exe( desc ):
-    if desc['ssh']:
-        return ( desc['spec']['argv'][0], *_remote_exe(desc['spec']['argv']) ) if desc['spec'] else ( None, None, None )
+def _exe( kernel_path ):
+    spec = _json(kernel_path)
+    d = basename(kernel_path)
+    if d.startswith('ssh_'):
+        return ( spec['argv'][0], *_remote_exe(spec['argv']) ) if spec else ( None, None, None )
     else:
-        return ( desc['spec']['argv'][0], None, None )
+        return ( spec['argv'][0], None, None )
 
 _rexists_checked_ = { }
 def rexists( host, path ):
     if f'''{host}:{path}''' in _rexists_checked_:
         return _rexists_checked_[f'''{host}:{path}''']
 
     if host is not None and path is not None:
@@ -41,72 +49,84 @@
             return False
 
         _rexists_checked_[f'''{host}:{path}'''] = True
         return True
 
     return False
         
-def _kernel_paths( kinfo ):
+def _kernel_paths( keys, kinfo ):
+    ###
+    ### Python is pathetic... you only get to traverse a filtered list once
+    ###
+    _keys = sorted(keys)
     colsize = 0
-    for k in kinfo.keys( ):
+    for k in _keys:
         if len(k) > colsize: colsize = len(k)
-    for k,info in kinfo.items( ):
-        e = _exe(info)
-        if info['ssh']:
+    for k in _keys:
+        e = _exe(kinfo[k])
+        if k.startswith('ssh_'):
             ### remote kernel spec
             if args.no_check or e[0] is not None and e[1] is not None and e[2] is not None and exists(e[0]) and rexists(e[2],e[1]):
-                print(f'''{k.ljust(colsize)} {info['path']}''')
+                print(f'''{k.ljust(colsize)} {kinfo[k]}''')
             else:
-                print(f'''{k.ljust(colsize)} {_red(info['path'])}''')
+                print(f'''{k.ljust(colsize)} {_red(kinfo[k])}''')
         else:
             ### local kernel spec
             if args.no_check or e[0] is not None and ( not e[0].startswith('/') or exists(e[0]) ):
-                print(f'''{k.ljust(colsize)} {info['path']}''')
+                print(f'''{k.ljust(colsize)} {kinfo[k]}''')
             else:
-                print(f'''{k.ljust(colsize)} {_red(info['path'])}''')
+                print(f'''{k.ljust(colsize)} {_red(kinfo[k])}''')
 
-def _local_paths( kinfo ):
+def _local_paths( keys, kinfo ):
+    ###
+    ### Python is pathetic... you only get to traverse a filtered list once
+    ###
+    _keys = sorted(keys)
     colsize = 0
-    for k in kinfo.keys( ):
+    for k in _keys:
         if len(k) > colsize: colsize = len(k)
-    for k,info in kinfo.items( ):
-        e = _exe(info)
+    for k in _keys:
+        e = _exe(kinfo[k])
         if args.no_check or e[0] is not None and ( not e[0].startswith('/') or exists(e[0]) ):
             print(f'''{k.ljust(colsize)} {e[0]}''')
         else:
             print(f'''{k.ljust(colsize)} {_red(e[0])}''')
 
-def _remote_paths( kinfo ):
+def _remote_paths( keys, kinfo ):
+    ###
+    ### Python is pathetic... you only get to traverse a filtered list once
+    ###
+    _keys = sorted(keys)
     colsize = 0
-    for k in kinfo.keys( ):
+    for k in _keys:
         if len(k) > colsize: colsize = len(k)
-    for k,info in kinfo.items( ):
-        e = _exe(info)
-        if info['ssh']:
+    for k in _keys:
+        e = _exe(kinfo[k])
+        if k.startswith('ssh_'):
             ### remote kernel spec
             if args.no_check or e[1] is not None and e[2] is not None and rexists(e[2],e[1]):
                 print(f'''{k.ljust(colsize)} {e[2]}:{e[1]}''')
             else:
                 print(f'''{k.ljust(colsize)} {_red(e[2] + ':' + e[1])}''')
         else:
             print(f'''{k.ljust(colsize)} localhost:{e[0]}''')
     
 if __name__ == "__main__":
-    from .. import get_kernel_desc
+    from .. import ls_kernel
     parse = ArgumentParser( add_help=False )
 
     optional = parse.add_argument_group("optional arguments")
     optional.add_argument( "--help", "-h", action="help", default=SUPPRESS, help="show this help message and exit" )
     optional.add_argument( "--all", "-a", action="store_true", help="list all kernels (not just ssh/sshpyk)" )
     optional.add_argument( "--local", "-l", action="store_true", help="list the information for the local python executable" )
     optional.add_argument( "--remote", "-r", action="store_true", help="list the information for the remote python executable" )
     optional.add_argument( "--no-check", "-nc", action="store_true", help="do not check for Python executables" )
 
     args = parse.parse_args( )
 
-    kinfo = get_kernel_desc( args.all )
+    kinfo = ls_kernel( )
     if args.local:
-        _local_paths( kinfo )
+        _local_paths( kinfo.keys( ) if args.all else filter( lambda k: k.startswith('ssh_'), kinfo.keys( ) ), kinfo )
     elif args.remote:
-        _remote_paths( kinfo )
+        _remote_paths( kinfo.keys( ) if args.all else filter( lambda k: k.startswith('ssh_'), kinfo.keys( ) ), kinfo )
     else:
-        _kernel_paths( kinfo )
+        _kernel_paths( kinfo.keys( ) if args.all else filter( lambda k: k.startswith('ssh_'), kinfo.keys( ) ), kinfo )
```

### Comparing `sshpyk-0.13/PKG-INFO` & `sshpyk-0.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,28 @@
-Metadata-Version: 2.1
-Name: sshpyk
-Version: 0.13
-Summary: remote jupyter kernels via ssh tunnels
-License: BSD-3-Clause
-Author-email: National Radio Astronomy Observatory <casa-feedback@nrao.edu>
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-
 Remote Jupyter Kernels via SSH tunnels
 ######################################
 
-The design of this pakage is based upon `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ which
-in turn is based upon `remote_ikernel <https://bitbucket.org/tdaff/remote_ikernel>`_. This implementation shares
-a common set of command line parameters with `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_, but it was
-implemented from scratch to adapt to recent changes to :code:`jupyter_client` (which broke :code:`ssh_ipykernel`)
-and to support Python 3.10. This package adds an :code:`ls` implementation which allows listing info about the
-available kernel specifications.
+The design of this pakage is based upon `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ which is
+in turn based upon `remote_ikernel <https://bitbucket.org/tdaff/remote_ikernel>`_. This implementation shares
+the same command line parameters as `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_, but it was
+reimplemented from scratch to support Python 3.10. It also includes an :code:`ls` implementation which allows
+checking on the available kernel specifications.
 
 While there are modest additions to `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_, there are
-also modest subtractions. There are fewer configuration options for things like the internal name used
-by `Jupyter Client <https://jupyter-client.readthedocs.io/en/stable/#>`_ to refer to the created
-kernel.
+also modest subtractions. There are fewer configuration options for things like the name that
+`Jupyter Client <https://jupyter-client.readthedocs.io/en/stable/#>`_ uses to refer to the
+kernel. This is still based on the kernel description that the user sees, but the entire name
+is no longer completely configurable.
 
 Listing the Jupyter Kernels that are available
 **********************************************
 
-It can be difficult to know which Jupyter Kernels are available because there are multiple locations where
+It can be difficult to know which Jupyter Kernels are available because there is more than one location that
 the `Kernel Spec files <https://jupyter-client.readthedocs.io/en/latest/kernels.html#kernel-specs>`_ can be
-found. :code:`sshpyk` has an :code:`ls` option which lists the kernels that are available (even those which are
+stored. :code:`sshpyk` has an :code:`ls` option to all for seeing which kernels are available (even if they are
 **not** `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ or :code:`sshpyk` kernels::
 
   bash$
   bash$ python -m sshpyk.kernel.ls --no-check -a
   python3                                   /Users/drs/develop/python/conda/envs/py310/share/jupyter/kernels/python3
   python3.8                                 /usr/local/share/jupyter/kernels/python3.8
   python3dbg                                /Users/drs/Library/Jupyter/kernels/python3dbg
@@ -41,20 +32,19 @@
   bash$
 
 The :code:`--no-check` (or alternatively :code:`-nc`) flag indicates that the validity of the kernel spec files
 should **not** be checked. The :code:`-a` (or :code:`--all`) flag indicates that it should show **all** kernel
 specifications rather than just the ones for `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ or
 :code:`sshpyk` kernel specification files.
 
-If :code:`--no-check` is **not** supplied, part of listing the kernel information will include 
+If :code:`--no-check` is **not** supplied, then as part of listing the kernel information :code:`sshpyk` will
 verify that the Python executable specified in the kernel specification exist on the local and remote systems.
-This check allows the ouput to be colorized so red text indicates a problem. :code:`--local` will limit the
-check to just the local Python executable and :code:`--remote` will limit the check to only the remote Python
-executable. These options also list the local or remote Python path **instead** of the path to the kernel
-specification directory.
+:code:`--local` will limit the check to just the local Python executable and :code:`--remote` will limit the
+check to only the remote Python executable. These options also list the local or remote Python path **instead**
+of the path to the kernel specification directory.
 
 
 Command line "ls" options
 =========================
 
 The following options are available for listing the Jupyter kernel specifications:
 
@@ -115,15 +105,15 @@
   bash$
 
 Unlike the example above, here we have asked that the remote Python path be displayed
 instead of showing the kernel specificaton directory. Since we again asked that *all kernels*
 be displayed instead of only the SSH kernels, a Python path is displayed for the
 non-SSH kernels, but it is the local Python path as indicated by :code:`localhost:`.
 Because these three kernels are non-SSH kernels this is the only Python path that is
-available. However for the SSH kernels, we can see the remote Python path listed.
+available. However for the SSH kernels, we can see the remote Pyton path listed.
 These paths are prefixed with the hostname, here :code:`host06:`. We can also see
 the newly added kernel listed as :code:`ssh_host06_host06kernel`. This name is an internal
 name created from the :code:`--display-name` string which the end user will typically
 never see.
 
 Command line "add" options
 ==========================
@@ -192,8 +182,7 @@
 is on some protected network behind :code:`ssh.example.com`. When the *local* account
 runs :code:`ssh host06`, SSH will first connect as :code:`BASTION-USERNAME` on
 :code:`ssh.example.com` and then it connect to host :code:`host06` as username
 :code:`HOST06-USERNAME`.
 
 This sort of configuration will allow :code:`host06` to be allowed as a hostname
 for remote kernels.
-
```

