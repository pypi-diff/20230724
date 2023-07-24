# Comparing `tmp/zhijiang-0.2.5-py3-none-any.whl.zip` & `tmp/zhijiang-0.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,22 @@
-Zip file size: 11198 bytes, number of entries: 19
--rw-rw-r--  2.0 unx     2635 b- defN 23-Jun-19 01:51 zhijiang/__init__.py
+Zip file size: 12303 bytes, number of entries: 20
+-rw-rw-r--  2.0 unx     4321 b- defN 23-Jul-24 01:31 zhijiang/__init__.py
 -rw-rw-r--  2.0 unx       81 b- defN 10-Jan-12 13:48 zhijiang/index.html
--rw-rw-r--  2.0 unx      231 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/alias
+-rw-rw-r--  2.0 unx      355 b- defN 23-Jul-23 07:05 zhijiang/data/rc_files/alias
+-rw-rw-r--  2.0 unx      994 b- defN 23-Jul-24 02:51 zhijiang/data/rc_files/bashrc
 -rw-rw-r--  2.0 unx       75 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/dockerignore
 -rw-rw-r--  2.0 unx      393 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/gdbinit
--rw-rw-r--  2.0 unx      118 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/gitconfig
+-rw-rw-r--  2.0 unx      153 b- defN 23-Jul-11 03:11 zhijiang/data/rc_files/gitconfig
 -rw-rw-r--  2.0 unx      561 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/inputrc
 -rw-rw-r--  2.0 unx      153 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/tmux.config
 -rw-rw-r--  2.0 unx      415 b- defN 23-Jun-08 04:57 zhijiang/data/rc_files/vimrc
--rw-rw-r--  2.0 unx      545 b- defN 23-Jun-16 08:07 zhijiang/scripts/enhance_python.sh
--rw-rw-r--  2.0 unx     1150 b- defN 23-Jun-09 06:13 zhijiang/scripts/install_useful_tools.sh
--rw-rw-r--  2.0 unx     7030 b- defN 23-Jun-20 03:35 zhijiang/scripts/useful_func.py
--rw-rw-r--  2.0 unx     2277 b- defN 23-Jun-16 08:02 zhijiang/scripts/zhijxu_onnx_helper.py
--rw-rw-r--  2.0 unx     1081 b- defN 23-Jun-20 04:04 zhijiang-0.2.5.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      921 b- defN 23-Jun-20 04:04 zhijiang-0.2.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-20 04:04 zhijiang-0.2.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       43 b- defN 23-Jun-20 04:04 zhijiang-0.2.5.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-20 04:04 zhijiang-0.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1618 b- defN 23-Jun-20 04:04 zhijiang-0.2.5.dist-info/RECORD
-19 files, 19428 bytes uncompressed, 8516 bytes compressed:  56.2%
+-rw-rw-r--  2.0 unx      546 b- defN 23-Jul-11 03:06 zhijiang/scripts/enhance_python.sh
+-rw-rw-r--  2.0 unx     1266 b- defN 23-Jul-24 02:47 zhijiang/scripts/install_useful_tools.sh
+-rw-rw-r--  2.0 unx     7245 b- defN 23-Jul-24 01:33 zhijiang/scripts/useful_func.py
+-rw-rw-r--  2.0 unx     2283 b- defN 23-Jul-11 01:50 zhijiang/scripts/zhijiang_onnx_helper.py
+-rw-rw-r--  2.0 unx     1081 b- defN 23-Jul-24 03:01 zhijiang-0.2.6.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      921 b- defN 23-Jul-24 03:01 zhijiang-0.2.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-24 03:01 zhijiang-0.2.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       43 b- defN 23-Jul-24 03:01 zhijiang-0.2.6.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jul-24 03:01 zhijiang-0.2.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1705 b- defN 23-Jul-24 03:01 zhijiang-0.2.6.dist-info/RECORD
+20 files, 22692 bytes uncompressed, 9483 bytes compressed:  58.2%
```

## zipnote {}

```diff
@@ -3,14 +3,17 @@
 
 Filename: zhijiang/index.html
 Comment: 
 
 Filename: zhijiang/data/rc_files/alias
 Comment: 
 
+Filename: zhijiang/data/rc_files/bashrc
+Comment: 
+
 Filename: zhijiang/data/rc_files/dockerignore
 Comment: 
 
 Filename: zhijiang/data/rc_files/gdbinit
 Comment: 
 
 Filename: zhijiang/data/rc_files/gitconfig
@@ -30,29 +33,29 @@
 
 Filename: zhijiang/scripts/install_useful_tools.sh
 Comment: 
 
 Filename: zhijiang/scripts/useful_func.py
 Comment: 
 
-Filename: zhijiang/scripts/zhijxu_onnx_helper.py
+Filename: zhijiang/scripts/zhijiang_onnx_helper.py
 Comment: 
 
-Filename: zhijiang-0.2.5.dist-info/LICENSE.txt
+Filename: zhijiang-0.2.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: zhijiang-0.2.5.dist-info/METADATA
+Filename: zhijiang-0.2.6.dist-info/METADATA
 Comment: 
 
-Filename: zhijiang-0.2.5.dist-info/WHEEL
+Filename: zhijiang-0.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: zhijiang-0.2.5.dist-info/entry_points.txt
+Filename: zhijiang-0.2.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: zhijiang-0.2.5.dist-info/top_level.txt
+Filename: zhijiang-0.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: zhijiang-0.2.5.dist-info/RECORD
+Filename: zhijiang-0.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zhijiang/__init__.py

```diff
@@ -1,8 +1,9 @@
 import os
+import subprocess
 from termcolor import cprint
 import fire
 import zhijiang as pkg
 
 
 pkg_installed_path = pkg.__path__[0]
 
@@ -16,65 +17,104 @@
             "you are in dry run mode, use '--dry_run=False' to disable dry run", "red"
         )
 
     rc_files_path = os.path.join(pkg_installed_path, "data/rc_files")
     for root, _, files in os.walk(rc_files_path):
         for f in files:
             rc_file = os.path.join(root, f)
-            dst = f"~/.{f}"
-            backup = f"{dst}.bk"
-            # backup the file if backup file is not existed
-            if not os.path.exists(os.path.expanduser(backup)):
-                # when user is root, then the rc file is not existed
-                if not os.path.exists(os.path.expanduser(dst)):
-                    os.system(f"touch {dst}")
-                os.system(f"cp {dst} {backup}")
+            if f not in ["bashrc", "alias"] and ".sw" not in f:
+                if ".sw" in f:
+                    continue
+                dst = f"~/.{f}"
+                backup = f"{dst}.bk"
+                # backup the file if backup file is not existed
+                if not os.path.exists(os.path.expanduser(backup)):
+                    # when user is root, then the rc file is not existed
+                    if not os.path.exists(os.path.expanduser(dst)):
+                        os.system(f"touch {dst}")
+                    os.system(f"cp {dst} {backup}")
 
-            if restore_rc:
                 cmd = f"cp {backup} {dst}"
+                if not restore_rc:
+                    # restore to backup file first, then do the changes
+                    cmd = f"{cmd} && cp {rc_file} {dst}"
+                print(cmd)
+
+                if not dry_run:
+                    os.system(cmd)
             else:
-                cmd = f"cp {rc_file} {dst}"
-            print(cmd)
-            if not dry_run:
-                os.system(cmd)
-                os.system("echo source ~/.alias >> ~/.bashrc")
+                dst = "~/.bashrc"
+                backup = f"{dst}.bk"
+                # backup the file if backup file is not existed
+                if not os.path.exists(os.path.expanduser(backup)):
+                    # when user is root, then the rc file is not existed
+                    if not os.path.exists(os.path.expanduser(dst)):
+                        os.system(f"touch {dst}")
+                    # if file is alias then just backup related is not need
+                    if f != "alias":
+                        os.system(f"cp {dst} {backup}")
+
+                cmd = "echo -n" # noop
+                if f == "bashrc":
+                    cmd = f"cp {backup} {dst}"
+                if not restore_rc:
+                    cmd = f"{cmd} && cat {rc_file} >> {dst}"
+                print(cmd)
+
+                if not dry_run:
+                    os.system(cmd)
+    if not dry_run:
+        os.system("echo 'echo -------------bashrc done-------------------' >> ~/.bashrc")
 
 
 def install_useful_tools():
     """
     install usefule shell commands and python pkg, e.g. profiling tools, debugging tools;
     """
     script_path = os.path.join(pkg_installed_path, "scripts/install_useful_tools.sh")
-    os.system(f"bash {script_path}")
+    subprocess.run(f"bash {script_path}".split(), check=True)
 
 
 def enhance_python():
     """
     add useful functions to python site.py, so you can call them like built-in functions, they are prefixed with zhijxu
     """
     script_path = os.path.join(pkg_installed_path, "scripts/enhance_python.sh")
-    os.system(f"bash {script_path}")
+    subprocess.run(f"bash {script_path}".split(), check=True)
 
 
 def info():
     """
     print help info;
     to enable tab completion >> zhijiang -- --completion > ~/.zhijiang; echo source  ~/.zhijiang >> ~/.bashrc; source ~/.bashrc
     """
     cprint("1. if you want tab completion, please 'zhijiang -- --completion > ~/.zhijiang; echo source  ~/.zhijiang >> ~/.bashrc; source ~/.bashrc'", "red")
     cprint("2. zhijiang subcommand-xx --help to see how to control subcommand", "red")
     cprint(f"3. you can modify the file before executing them, they are put at {pkg_installed_path}", "red")
+    cprint("4. added python function or bash command are all prefixed with zhijiang- ", "red")
+
+
+def all():
+    """
+        run all subcommands
+    """
+    setup_rc_files(dry_run=False)
+    install_useful_tools()
+    enhance_python()
+    os.system("zhijiang -- --completion > ~/.zhijiang; echo source  ~/.zhijiang >> ~/.bashrc")
+    cprint("remember to source ~/.bashrc to make the changes take effect", "red")
 
 
 def main():
     fire.Fire(
         {
             "setup_rc_files": setup_rc_files,
             "install_useful_tools": install_useful_tools,
             "enhance_python": enhance_python,
             "info": info,
+            "all": all,
         }
     )
 
 
 if __name__ == "__main__":
     main()
```

## zhijiang/data/rc_files/alias

```diff
@@ -2,7 +2,13 @@
 alias grep='grep --color=auto'
 alias less='less -i' # ignore case when searching
 alias ps='ps auxf' # process tree
 alias top='top c'
 alias sudo='sudo env PATH=$PATH'
 alias j='autojump'
 alias gdb='gdb -q'
+alias zhijiang-peco=peco
+alias zhijiang-cat=batcat
+
+alias gd='git diff'
+alias gca='git commit -a'
+alias gb='git branch -vv'
```

## zhijiang/data/rc_files/gitconfig

```diff
@@ -1,6 +1,7 @@
 [user]
         email = zhijxu@microsoft.com
         name = zhijxu
 [core]
         editor = vim
         pager = less -i
+        excludesFile = '.vscode/*'
```

## zhijiang/scripts/enhance_python.sh

```diff
@@ -9,9 +9,8 @@
 else
   ## site.py is unchanged, so backup it
   cp $sitepy_path $backup
 fi
 
 pkg_script_path=`dirname $BASH_SOURCE`
 cat $pkg_script_path/useful_func.py >> $sitepy_path
-cp $pkg_script_path/zhijxu_onnx_helper.py `dirname $sitepy_path`
-
+cp $pkg_script_path/zhijiang_onnx_helper.py `dirname $sitepy_path`
```

## zhijiang/scripts/install_useful_tools.sh

```diff
@@ -2,19 +2,21 @@
 
 sudo apt update
 sudo apt install -y tldr tmux
 sudo apt install -y vim-gtk  # vim with +clipboard, so vim can use os's clipboard
 
 sudo apt install -y gdb cgdb
 
-sudo apt install -y nsight-systems-2021.2.4 nsight-compute-2021.3.1
-sudo ln -s /opt/nvidia/nsight-compute/2021.3.1/ncu /usr/local/bin
+if [ ! -e /usr/local/bin/ncu ]; then
+    sudo apt install -y nsight-systems-2021.2.4 nsight-compute-2021.3.1
+    sudo ln -s /opt/nvidia/nsight-compute/2021.3.1/ncu /usr/local/bin
+fi
 
-sudo apt install -y peco
-wget -O /tmp/bat.deb https://github.com/sharkdp/bat/releases/download/v0.21.0/bat-musl_0.21.0_amd64.deb && sudo dpkg -i /tmp/bat.deb
+sudo apt install -y peco bat
+# wget -O /tmp/bat.deb https://github.com/sharkdp/bat/releases/download/v0.21.0/bat-musl_0.21.0_amd64.deb && sudo dpkg -i /tmp/bat.deb
 
 sudo apt install -y python3.8-dbg
 sudo env "PATH=$PATH" pip install py-spy viztracer debugpy \
     cmake==3.21.4
 
 # tab complete of git
 curl https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash -o ~/.git-completion.bash
@@ -22,10 +24,12 @@
 # install tool to outuput c++ call graph, class grpah
 sudo  apt-get install -y silversearcher-ag
 (
 cd /tmp
 wget https://raw.githubusercontent.com/satanson/cpp_etudes/master/calltree.pl
 wget https://raw.githubusercontent.com/satanson/cpp_etudes/master/cpptree.pl
 chmod 777 calltree.pl cpptree.pl
-sudo mv calltree.pl /usr/local/bin/calltree
-sudo mv cpptree.pl /usr/local/bin/cpptree
+sudo mv calltree.pl /usr/local/bin/zhijiang-calltree
+sudo mv cpptree.pl /usr/local/bin/zhijiang-cpptree
 )
+
+sudo env "PATH=$PATH" pip install plantweb
```

## zhijiang/scripts/useful_func.py

```diff
@@ -3,58 +3,62 @@
 import pdb
 import inspect
 import builtins
 from functools import wraps
 import atexit
 import time
 from tempfile import mkdtemp
+import inspect
 
 try:
     import torch
     import debugpy
     from termcolor import cprint
     from viztracer import VizTracer
-    from zhijxu_onnx_helper import Analyze_onnx_model
+    from zhijiang_onnx_helper import Analyze_onnx_model
 except ImportError:
     pass
 
 
-def __zhijxu_is_rank_0():
+def __zhijiang_is_rank_0():
     if os.environ.get("LOCAL_RANK", "0") == "0":
         return True
     return False
 
 
-def zhijxu_run_once(func):
+def zhijiang_run_once(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
         if not wrapper.has_run:
             wrapper.has_run = True
             return func(*args, **kwargs)
 
     wrapper.has_run = False
     return wrapper
 
 
-@zhijxu_run_once
-def zhijxu_vscode_attach(sleep_time_sec=3):
+@zhijiang_run_once
+def zhijiang_vscode_attach(sleep_time_sec=3):
     """
     only rank 0 will wait for vscode debug attach, other rank continue to run
     """
-    if __zhijxu_is_rank_0():
+    if __zhijiang_is_rank_0():
         debugpy.listen(("localhost", 56789))
         time.sleep(
             sleep_time_sec
         )  # so the next print can be shown at last line of terminal in multiprocess case
-        cprint("\n\nzhijxu, waiting for debug connect\n\n", color="red", flush=True)
+        stack = inspect.stack()
+        caller_frame = stack[2]
+        location = f"{caller_frame.filename}:{caller_frame.lineno}"
+        cprint(f"\n\nzhijiang, waiting at {location} for debug connect\n\n", color="red", flush=True)
         debugpy.wait_for_client()
-        cprint("\n\nzhijxu,debug connection done!!!\n\n", color="red", flush=True)
+        cprint("\n\nzhijiang,debug connection done!!!\n\n", color="red", flush=True)
 
 
-def zhijxu_do_bench(
+def zhijiang_do_bench(
     fn,
     warmup=25,
     rep=100,
     grad_to_none=None,
     percentiles=(0.5, 0.2, 0.8),
     fast_flush=False,
 ):
@@ -123,17 +127,17 @@
     if percentiles:
         percentiles = torch.quantile(times, torch.tensor(percentiles)).tolist()
         return tuple(percentiles)
     else:
         return torch.mean(times).item()
 
 
-def zhijxu_cuda_profiling(step):
+def zhijiang_cuda_profiling(step):
     """
-    the control env and its possible values are:
+    the environment variable and their possible values are:
         - VIZTRACER, 0/1
         - NSYS, 0/1
         - START_STEP, any integer larger than 0
         - END_STEP, any integer larger than START_STEP, END_STEP is excluded from profiling
     """
     if os.environ.get("VIZTRACER", "0") == "1":
         assert (
@@ -159,53 +163,53 @@
             torch.cuda.cudart().cudaProfilerStart()
         if step == int(os.environ.get("END_STEP", 20)):
             cprint("Stop tracing", "red")
             torch.cuda.cudart().cudaProfilerStop()
             sys.exit(0)
 
 
-@zhijxu_run_once
-def zhijxu_pdb():
+@zhijiang_run_once
+def zhijiang_pdb():
     """
         only rank 0 will enter pdb, other ranks continue execution
     """
-    if __zhijxu_is_rank_0():
-        cprint("zhijxu, i am rank 0, enter pdb now", "red")
+    if __zhijiang_is_rank_0():
+        cprint("zhijiang, i am rank 0, enter pdb now", "red")
         pdb.set_trace()
 
 
-@zhijxu_run_once
-def zhijxu_enter_pdb_at_exception():
+@zhijiang_run_once
+def zhijiang_enter_pdb_at_exception():
     """
         register a hook which will enter pdb when process wants to exit, this will help debugging when process has un-caught exception
     """
     atexit.register(pdb.pm)
 
 
-def zhijxu_open_onnx_in_tensorboard(model, port):
+def zhijiang_open_onnx_in_tensorboard(model, port):
     """
     give the onnx model path and tensorboard port, then will convert to tensorboard and launch tensorboard automatically for you
     """
     os.environ['PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION']='python'
     tmp_dir = mkdtemp(prefix="onnx-tensorboard-")
     cprint(f"converted tensorboard is put at {tmp_dir}", "red")
-    os.system(f"python /home/zhijxu/onnxruntime/tools/python/onnx2tfevents.py --logdir={tmp_dir} --model {model}")
+    os.system(f"python /home/zhijiang/onnxruntime/tools/python/onnx2tfevents.py --logdir={tmp_dir} --model {model}")
     os.system(f"tensorboard --logdir={tmp_dir} --port {port} &")
     time.sleep(3)
 
 
-def zhijxu_analyze_onnx_model(onnx_file):
+def zhijiang_analyze_onnx_model(onnx_file):
     os.system("reset")
     model = Analyze_onnx_model(onnx_file)
     model.print_info()
-    cprint("1. search items by \"zhijxu,\"\n2. return class object has attribute \"constant_registery\" to get constant value", "red")
+    cprint("1. search items by \"zhijiang,\"\n2. return class object has attribute \"constant_registery\" to get constant value", "red")
     return model
 
 
 fset = {
     name: obj
     for name, obj in inspect.getmembers(sys.modules[__name__])
-    if inspect.isfunction(obj) and name.startswith("zhijxu_")
+    if inspect.isfunction(obj) and name.startswith("zhijiang_")
 }
 for name, obj in fset.items():
     if inspect.isfunction(obj):
         setattr(builtins, name, obj)
```

## Comparing `zhijiang/scripts/zhijxu_onnx_helper.py` & `zhijiang/scripts/zhijiang_onnx_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         value_infos = self.model.graph.value_info
         value_info_dict = {}
         for value_info in value_infos:
             value_info_dict[value_info.name] = [[i.dim_value for i in value_info.type.tensor_type.shape.dim], tensor_dtype_to_string(value_info.type.tensor_type.elem_type).lstrip("TensorProto.")]
         return value_info_dict
 
     def print_info(self):
-        cprint("zhijxu, node op info:", "red")
+        cprint("zhijiang, node op info:", "red")
         print(self.print_dict_one_by_one(self.get_node_dict()))
 
-        cprint("zhijxu, constant info:", "red")
+        cprint("zhijiang, constant info:", "red")
         print(self.print_dict_one_by_one(self.get_constant_dict()))
 
-        cprint("zhijxu, value info:", "red")
+        cprint("zhijiang, value info:", "red")
         print(self.print_dict_one_by_one(self.get_value_info_dict()))
```

## Comparing `zhijiang-0.2.5.dist-info/LICENSE.txt` & `zhijiang-0.2.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `zhijiang-0.2.5.dist-info/METADATA` & `zhijiang-0.2.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhijiang
-Version: 0.2.5
+Version: 0.2.6
 Summary: setup linux env, such as bashrc etc.
 Home-page: https://github.com/xu-zhijiang/env-setup.git
 Author: Xu Zhijiang
 Author-email: 15852939122@163.com
 Project-URL: Funding, https://github.com/xu-zhijiang
 Project-URL: Source, https://github.com/xu-zhijiang/env-setup.git
 Keywords: env setup,development,zhijiang
```

## Comparing `zhijiang-0.2.5.dist-info/RECORD` & `zhijiang-0.2.6.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-zhijiang/__init__.py,sha256=DUEc6SIeLIpugwNJ2PHGbVII5zdEMlQyZWTAs6L4oZA,2635
+zhijiang/__init__.py,sha256=DyTsQy9gifTS4w9iU5_zi4R9E7KKGIKLUZgpwR1xHeA,4321
 zhijiang/index.html,sha256=HS2Ji47iYR7u0Cho4nsePbLSZrQBa1QWDxKBh5YUMfs,81
-zhijiang/data/rc_files/alias,sha256=uw0D-awccLVoQandcJ_nabKOomQI-BfZsEhIHC5q0mg,231
+zhijiang/data/rc_files/alias,sha256=MntZAoCwFDqtYKDgEkfbTJgAE_auVTVVi8YCcE7DOhw,355
+zhijiang/data/rc_files/bashrc,sha256=yrR5NkimSh9J0zrmJuDpKN4wMwrFjJPjXo49_dc2_3s,994
 zhijiang/data/rc_files/dockerignore,sha256=fNTcMXrdUU9h9Y0tkLpfQKbLhwRwaVNd-MyP-ycI3sE,75
 zhijiang/data/rc_files/gdbinit,sha256=Om1pIhhf-_lIfLgx8Gt730W2R4vvZLr05hbgnhNy0Hs,393
-zhijiang/data/rc_files/gitconfig,sha256=kJZIubN64CoqXqHlHlkof8HzGh0E0KlAWWRHCkpQc6Y,118
+zhijiang/data/rc_files/gitconfig,sha256=oPL1kx7xOT0xuO5MTm0jwsLicu1dLto1MUKgriTWT8Q,153
 zhijiang/data/rc_files/inputrc,sha256=yl22z2lj2jWLaE85I9QpV9NjoYoOhpmPemNxEsxMC5Y,561
 zhijiang/data/rc_files/tmux.config,sha256=m0TZ9DBK72V3IXXWir2YqHjLWbuTLwxqkYrhdTvEgRc,153
 zhijiang/data/rc_files/vimrc,sha256=T-rxTkB8WJdxuQRLIbNYe-ybahRXmssVi7nE2ER7RsM,415
-zhijiang/scripts/enhance_python.sh,sha256=fh5B4wVZ3i4SR9twTj8bGaLIhfO0epPxOPc4z_7NjPY,545
-zhijiang/scripts/install_useful_tools.sh,sha256=7C287YLb57j0hxKWLWeM2KIZcI6cM1L4DDHGIlju9UE,1150
-zhijiang/scripts/useful_func.py,sha256=KdI4MkXojN2fSTUaBZhl_i8xX8NmRbKWMNppAvBqdEM,7030
-zhijiang/scripts/zhijxu_onnx_helper.py,sha256=NZHGOHVsDYxCClU5Q6YBXKvOCI9yW5YkXJEehn3MszI,2277
-zhijiang-0.2.5.dist-info/LICENSE.txt,sha256=ceC9ZJOV9H6CtQDcYmHOS46NA3dHJ_WD4J9blH513pc,1081
-zhijiang-0.2.5.dist-info/METADATA,sha256=TJx5i3leyWp0b5ivzkTEfpI6aOA0NOPjIschPIO9Wvk,921
-zhijiang-0.2.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-zhijiang-0.2.5.dist-info/entry_points.txt,sha256=Q_-WKs0WMLyxX1t8rWQzIE94DfhcGxeqYzdM-09IxCs,43
-zhijiang-0.2.5.dist-info/top_level.txt,sha256=CLVD_HFtdNB3uaa7tp2r1-vOsvccTYHrlIxNxW06rAU,9
-zhijiang-0.2.5.dist-info/RECORD,,
+zhijiang/scripts/enhance_python.sh,sha256=NJqYh3D_5izRGEwZiLYcwViXl_hikVZYqKJpRtV_AGY,546
+zhijiang/scripts/install_useful_tools.sh,sha256=2Y5arF_XRDCJAPKySunxXD3nQWetyzsUyNyyDr_Lqvs,1266
+zhijiang/scripts/useful_func.py,sha256=1M7_qoeabPmbcafhZKgQdBoCzvL2Uq4nWkXfGR_hbBY,7245
+zhijiang/scripts/zhijiang_onnx_helper.py,sha256=CsMwCx2JkTIOmJnJyq1oetRwH2ufkSJ_9JlwgGMHFVE,2283
+zhijiang-0.2.6.dist-info/LICENSE.txt,sha256=ceC9ZJOV9H6CtQDcYmHOS46NA3dHJ_WD4J9blH513pc,1081
+zhijiang-0.2.6.dist-info/METADATA,sha256=ucclXC41pxwtvv1LDRlQXYcCauRRwcXkB6aZutW9YvE,921
+zhijiang-0.2.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+zhijiang-0.2.6.dist-info/entry_points.txt,sha256=Q_-WKs0WMLyxX1t8rWQzIE94DfhcGxeqYzdM-09IxCs,43
+zhijiang-0.2.6.dist-info/top_level.txt,sha256=CLVD_HFtdNB3uaa7tp2r1-vOsvccTYHrlIxNxW06rAU,9
+zhijiang-0.2.6.dist-info/RECORD,,
```

