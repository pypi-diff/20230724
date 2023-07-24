# Comparing `tmp/easy_deployer-0.1.2.tar.gz` & `tmp/easy_deployer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\easy_deployer-0.1.2.tar", last modified: Wed Mar 30 02:21:19 2022, max compression
+gzip compressed data, was "easy_deployer-0.1.3.tar", last modified: Mon Jul 24 17:28:19 2023, max compression
```

## Comparing `easy_deployer-0.1.2.tar` & `easy_deployer-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-03-30 02:21:19.914966 easy_deployer-0.1.2/
--rw-rw-rw-   0        0        0      827 2022-03-30 02:21:19.907961 easy_deployer-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      185 2022-03-29 22:50:10.000000 easy_deployer-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2022-03-30 02:21:19.812893 easy_deployer-0.1.2/easy_deployer/
--rw-rw-rw-   0        0        0       90 2022-03-30 02:17:42.000000 easy_deployer-0.1.2/easy_deployer/__init__.py
--rw-rw-rw-   0        0        0    26486 2022-03-30 01:57:46.000000 easy_deployer-0.1.2/easy_deployer/github.py
--rw-rw-rw-   0        0        0    11088 2022-03-30 01:57:34.000000 easy_deployer-0.1.2/easy_deployer/heroku.py
--rw-rw-rw-   0        0        0     7759 2022-03-30 02:18:33.000000 easy_deployer-0.1.2/easy_deployer/main.py
--rw-rw-rw-   0        0        0    12250 2022-03-29 04:46:28.000000 easy_deployer-0.1.2/easy_deployer/shared_functions.py
-drwxrwxrwx   0        0        0        0 2022-03-30 02:21:19.890948 easy_deployer-0.1.2/easy_deployer.egg-info/
--rw-rw-rw-   0        0        0      827 2022-03-30 02:21:18.000000 easy_deployer-0.1.2/easy_deployer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2022-03-30 02:21:18.000000 easy_deployer-0.1.2/easy_deployer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-30 02:21:18.000000 easy_deployer-0.1.2/easy_deployer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      157 2022-03-30 02:21:18.000000 easy_deployer-0.1.2/easy_deployer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2022-03-30 02:21:18.000000 easy_deployer-0.1.2/easy_deployer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-03-30 02:21:19.916967 easy_deployer-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1373 2022-03-30 02:21:08.000000 easy_deployer-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 17:28:19.590037 easy_deployer-0.1.3/
+-rw-rw-rw-   0        0        0     1086 2021-07-27 13:30:42.000000 easy_deployer-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      766 2023-07-24 17:28:19.589039 easy_deployer-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2022-03-29 22:50:10.000000 easy_deployer-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 17:28:19.573083 easy_deployer-0.1.3/easy_deployer/
+-rw-rw-rw-   0        0        0       90 2022-03-30 02:17:42.000000 easy_deployer-0.1.3/easy_deployer/__init__.py
+-rw-rw-rw-   0        0        0    26588 2023-07-24 15:55:57.000000 easy_deployer-0.1.3/easy_deployer/github.py
+-rw-rw-rw-   0        0        0    11211 2023-07-23 15:15:38.000000 easy_deployer-0.1.3/easy_deployer/heroku.py
+-rw-rw-rw-   0        0        0     9149 2023-07-23 15:19:03.000000 easy_deployer-0.1.3/easy_deployer/main.py
+-rw-rw-rw-   0        0        0    12360 2023-07-23 15:28:41.000000 easy_deployer-0.1.3/easy_deployer/shared_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-24 17:28:19.588042 easy_deployer-0.1.3/easy_deployer.egg-info/
+-rw-rw-rw-   0        0        0      766 2023-07-24 17:28:19.000000 easy_deployer-0.1.3/easy_deployer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-07-24 17:28:19.000000 easy_deployer-0.1.3/easy_deployer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 17:28:19.000000 easy_deployer-0.1.3/easy_deployer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      156 2023-07-24 17:28:19.000000 easy_deployer-0.1.3/easy_deployer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-07-24 17:28:19.000000 easy_deployer-0.1.3/easy_deployer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 17:28:19.591034 easy_deployer-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1373 2023-07-24 17:25:00.000000 easy_deployer-0.1.3/setup.py
```

### Comparing `easy_deployer-0.1.2/PKG-INFO` & `easy_deployer-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: easy_deployer
-Version: 0.1.2
-Summary: UNKNOWN
+Version: 0.1.3
 Home-page: https://github.com/medamine980/easy-deployer
 Author: Mohamed-Amine Benali
 Author-email: namelowy_64@hotmail.com
 License: MIT
-Description: # Easy-Deployer:
-        Easy-deployer is used to simplify and speed up the deployment process.
-        It's mostly still in progress...
-        
-        ## OS Support:
-        Currently windows is the only supported os.
 Keywords: python,github,github-deployer,heroku,heroku-deployer,deploy,easy,easy-deployer,simple,simple-deployer
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Easy-Deployer:
+Easy-deployer is used to simplify and speed up the deployment process.
+It's mostly still in progress...
+
+## OS Support:
+Currently windows is the only supported os.
```

### Comparing `easy_deployer-0.1.2/easy_deployer/github.py` & `easy_deployer-0.1.3/easy_deployer/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # coding=<utf-8>
 from subprocess import Popen, PIPE, DEVNULL
 from argparse import ArgumentParser
 import os, sys, json, getpass, re, time, itertools, threading, signal, webbrowser, keyboard
 
-from .shared_functions import printWarning, listPromptInquirer, promptPyInquirer, runCmd, getOS, openBash, defaultCommit
+from shared_functions import printWarning, listPromptInquirer, promptPyInquirer, runCmd, getOS, openBash, defaultCommit
 
 def main():
     args = takeArgs() # Take the arguments
     if not os.path.exists(args["path"]):
         print("Invalid Path!")
         sys.exit(5)
     args["path"] = os.path.abspath(args["path"])
     args["path"] = args["path"].strip()
     checkSoftware("git", "git --help") # check if git is installed in the current machine
     args["path"] = os.path.abspath(args["path"]) # just changing 
     createResourceDir() #create resources
     # os.chdir(args["path"]) # changing directory
     if getOS() == "windows": # to clean the screen
-        os.system("cls") #
-    # if args["cmd"] == "add-to-path":
-    #     add2Path(args)
+        os.system("cls") # clears the console
     if args["git_ignore"]:
         handleGitIgnore(args["path"])
     if args["rm_git_ignore"]:
         handleRmGitIgnore(args["path"])
     if args["cmd"] == "update": # check if -u or --update is present when the user runs the script
         update(args)
         return
@@ -38,15 +36,15 @@
     parser = ArgumentParser(prog="github-deployer",
     usage="""You basically enter one of the following commands:
         ¤ create-update (which is the default one)
         ¤ update (to update an existing repository)
         ¤ delete (to delete an existing repository)
 then you need to specify the path by using the -p or --path argument.""", description="%(prog)s <commands> [options]")
     parser.add_argument("-v","--version", action="version", version="version 1.0", help="%(prog)s current version")
-    parser.add_argument("cmd", nargs="?", default="create-update", choices=["create-update", "update", "delete", "add-to-path"],help="commands, default command is 'create-update'")
+    parser.add_argument("cmd", nargs="?", default="create-update", choices=["create-update", "update", "delete"],help="commands, default command is 'create-update'")
     parser.add_argument("-p","--path", help="path of the folder intended to deploy.", required=True)
     parser.add_argument("-new", nargs="*", default=[], choices=["user","token"], help="if you want to resave user or token")
     parser.add_argument("-repo", "--repository",dest="name", help="repository name")
     parser.add_argument("-ac", "--add-collaborators", action="store_true",help="if you want to add collaborators, repository must exist to do so else you'll get an error")
     parser.add_argument("-visibility", action="store_true")
     # parser.add_argument("-atp","--add-to-path-var", action="store_true", help="if you want to add the program to path environnement variable so that you can run it wherever you are")
     parser.add_argument("-git-ig", "--git-ignore", action="store_true")
@@ -65,67 +63,67 @@
     createRepo = repositoryCreationNeeded(url, token, args["path"])
     if createRepo:
         loading = Loading(startText="Creating repository", stopText="repository has been created!", type="dynamic", timeout=.1)
         isCollaborators = data["collaborators"]
         data = {k:v for k,v in data.items() if k != "username" and k != "collaborators"}
         # cmd down is a command for creating a repository 
         loading.start()
-        cmd = 'curl -f -u :'+token+' https://api.github.com/user/repos -d \''+json.dumps(data)+'\' '
+        cmd = 'curl -f -u '+username+':'+token+' https://api.github.com/user/repos -d "'+json.dumps(data).replace("\"","\\\"")+'"'
         out = openBash(cmd, stderr=PIPE ,stdout=PIPE, loading=loading, error="""Error has been caught:
             Authorization Required! check your username and password
         """, printBashError=False)
         loading.stop()
         saveTokenIfnotSaved(token)
         if isCollaborators:
-            handleCollaborators(username=username, token=token, name=data["name"])
+            handleCollaborators(username=username, token=token, repo_name=data["name"])
     elif not createRepo:
         #if we don't need to create a repository (which means it's already available) then we simply print that below
         print("repository already exist...")
         if(args["visibility"]):
             if args["visibility"]:
-                changeVisibility(username=username, token=token, name=data["name"])
+                changeVisibility(username=username, token=token, repo_name=data["name"])
         if(args["add_collaborators"]):
-            handleCollaborators(username=username, token=token, name=data["name"])
+            handleCollaborators(username=username, token=token, repo_name=data["name"])
     masterToMain(args["path"])
     addRemoteAndPush(url, args["path"])
 
 def update(args):
     """
     it gets called when "-u" or "--update" are available
     it updates or (pushs) the specified directory to the specified repository
     """
     defaultCommit(args)
     username = handleUsername(args)
     token = handleToken(args, username)
-    repo = getRepoName(args["name"], args["path"])
-    url = getGithubUrl({"username":username,"name":repo})
+    repo_name = getRepoName(args["name"], args["path"])
+    url = getGithubUrl({"username":username,"name":repo_name})
     if args["add_collaborators"]:
-        addCollaborators(args, username=username, token=token, name=repo)
+        addCollaborators(args, username=username, token=token, name=repo_name)
     if args["visibility"]:
-        changeVisibility(username=username, token=token, name=repo)
+        changeVisibility(username=username, token=token, name=repo_name)
     createRepo = repositoryCreationNeeded(url,token, args["path"])
     saveTokenIfnotSaved(token)
     if createRepo:
         repoNotFoundError()
     elif not createRepo:
         masterToMain(args["path"])
         addRemoteAndPush(url, args["path"])
 
 def delete(args):
     username = handleUsername(args)
     token = handleToken(args, username)
-    repo = getRepoName(args["name"], args["path"])
-    url = getGithubUrl({ "username":username, "name":repo })
+    repo_name = getRepoName(args["name"], args["path"])
+    url = getGithubUrl({ "username":username, "name":repo_name })
     createRepo = repositoryCreationNeeded(url=url,token=token, path=args["path"])
     if createRepo:
         repoNotFoundError()
     elif not createRepo:
         loading = Loading(startText="Deleting Repository",stopText="Repository Deleted", type="dynamic", timeout=.1)
         loading.start()
-        openBash(f"curl -X DELETE -H 'Authorization: token {token}' https://api.github.com/repos/{username}/{repo}", stdout=PIPE, stderr=PIPE ,loading=loading)
+        openBash(f"curl -X DELETE -H 'Authorization: token {token}' https://api.github.com/repos/{username}/{repo_name}", stdout=PIPE, stderr=PIPE ,loading=loading)
         loading.stop()
 
 def addCollaborators(args,**credentials):
     if not credentials:
         username = handleUsername(args)
         token = handleToken(args, username)
         repo = getRepoName(args["name"], args["path"])
@@ -313,15 +311,15 @@
     runCmd(f"git -C {path} rm -rf --cached .")
 
 
 
 def handleCollaborators(**credentials):
     username = credentials["username"]
     token = credentials["token"]
-    name = credentials["name"]
+    name = credentials["repo_name"]
     try:
         n = int(input("how many collaborators do you want to invite: ")) # number of collaborattors
     except ValueError:
         print("Error! invalid number!")
         sys.exit(13)
     collaborators = []
     hotkey = "ctrl + c"
@@ -373,15 +371,15 @@
             print(out["message"])
         else:
             print("Added!")
 
 def changeVisibility(**credentials):
     username = credentials["username"]
     token = credentials["token"]
-    name = credentials["name"]
+    repo_name = credentials["repo_name"]
     # visiblity = promptPyInquirer({
     #     "name": "visibility",
     #     "question": "change it to?",
     #     "choices": ["private", "public"]
     # })["visibility"]
     if(getOS() == "windows"):
         visiblity = promptPyInquirer({
@@ -392,15 +390,15 @@
         })["visibility"]
     else:
         visiblity = listPromptInquirer({
             "name": "visibility",
             "question": "change it to?",
             "choices": ["private", "public"]
         })
-    command = "curl -H 'Authorization: token "+token+"' 'https://api.github.com/repos/"+username+"/"+name+"' -H 'Accept: application/vnd.github.nebula-preview+json' -X PATCH -d '{\"visibility\":\""+visiblity+"\"}'"
+    command = "curl -H 'Authorization: token "+token+"' 'https://api.github.com/repos/"+username+"/"+repo_name+"' -H 'Accept: application/vnd.github.nebula-preview+json' -X PATCH -d '{\"visibility\":\""+visiblity+"\"}'"
     
     loading = Loading(type="dynamic", startText="Changing", stopText="Changed!")
     loading.start()
     process = openBash(command, stderr=PIPE, stdout=PIPE, returncode=True)
     if("Visibility is already " in process["out"]):
         loading.abort()
         print("Visibility is already private.")
@@ -464,30 +462,30 @@
     return f"https://github.com/{data['username']}/{data['name']}.git"
 
 
 def infoAboutToken():
     print("If you don't have your token yet go get it from https://github.com/settings/tokens (you must be loggedIn)")
 
 def infoAboutRepo(username,token,repo,collaboratorsCmdExist, path):
-    name = getRepoName(repo, path)
-    if not repositoryCreationNeeded( getGithubUrl({"name":name, "username":username}), token, path):
-        return {"name":name, "username":username}
+    repo_name = getRepoName(repo, path)
+    if not repositoryCreationNeeded( getGithubUrl({"name":repo_name, "username":username}), token, path):
+        return {"name":repo_name, "username":username}
     
     private = input("want it to be private? (y/n): ").lower()
     if private == "y":
         private = True
     elif private == "n":
         private = False
     else:
         invalidAnswerExit()
     if collaboratorsCmdExist:
         collaborators = True
     elif not collaboratorsCmdExist:
         collaborators = promptCollaborators()
-    return {"name": name,"private":private,"username":username, "collaborators":collaborators}
+    return {"name": repo_name,"private":private,"username":username, "collaborators":collaborators}
 
 def openBrowser(url):
     print("[¤] press any key to open repository in your browser or q to quit the program.")
     if keyboard.read_key() == "q":
         sys.exit(0)
     else:
         loading = Loading(startText="Opening",stopText="Opened!", timeout=0.18)
@@ -546,34 +544,34 @@
         loading.abort()
         print("Invalid token")
         sys.exit(17)
     openBash(f"curl -f -H \"Authorization: token {token}\" https://api.github.com/users/codertocat -I", stdout=PIPE, stderr=PIPE, error="there is no such token available",loading=loading, printBashError=False,timeout=10)
     loading.stop()
     pass
 
-def checkRepositoryName(name):
+def checkRepositoryName(repo_name):
     regex = re.compile("[^A-Za-z0-9_\-]{1,}")
-    maxChar = 100
-    name = name[:maxChar]
+    max_char = 100
+    repo_name = repo_name[:max_char]
     
-    if regex.search(name):
-        newName = regex.sub("-", name)
-        printWarning("Your new repository will be created as:",newName,sep="\n\t",flush=True)
+    if regex.search(repo_name):
+        new_name = regex.sub("-", repo_name)
+        printWarning("Your new repository will be created as:",new_name,sep="\n\t",flush=True)
         confirm = input("Do you want to Try another one? (y/n): ").strip().lower()
         if confirm == "y":
             confirm = False
         elif confirm == "n":
             confirm = True
         else:
             invalidAnswerExit()
         if not confirm:
-            name = checkRepositoryName(input("Try another repository name: "))
+            repo_name = checkRepositoryName(input("Try another repository name: "))
         elif confirm:
-            name = newName
-    return name
+            repo_name = new_name
+    return repo_name
 
 def checkSoftware(name, cmd, url=None):
     err = f"It seems that {name} is not in your machine, please make sure to download it first"
     err += f"\n you can find it at {url}" if url else ""
     runCmd(cmd, stdout=DEVNULL,
         error= err
     )
```

### Comparing `easy_deployer-0.1.2/easy_deployer/heroku.py` & `easy_deployer-0.1.3/easy_deployer/heroku.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os, sys, keyboard, json, re
 from subprocess import Popen, PIPE, run, DEVNULL
 from argparse import ArgumentParser
 
-from .shared_functions import Loading, runCmd, promptPyInquirer, defaultCommit
+from shared_functions import Loading, runCmd, promptPyInquirer, defaultCommit
 
 def main():
     args = takeArgs()
     checkSoftware("git", "git --help")
     checkSoftware("heroku", "heroku --help", "https://devcenter.heroku.com/articles/heroku-cli#download-and-install")
     args["path"] = os.path.abspath(args["path"])
     os.chdir(args["path"]) #changing to path
@@ -48,14 +48,16 @@
 def delete(args:dict):
     if not herokuIsLoggedIn(args["new_login"]):
         herokuLogin()
     runCmd("heroku apps:destroy")
     sys.exit(0)
 
 def takeArgs():
+    print("""Heroku is no longer available as a target deployer because it no longer offers the plan!""")
+    sys.exit(0)
     parser = ArgumentParser(prog="heroku-deployer",
     usage="""You basically enter one of the following commands:
         ¤ create-update (which is the default one)
         ¤ update (to update an existing heroku-website)
         ¤ delete (to delete an existing heroku-website)
         ¤ logs (to log if there were any errors)
     then you need to specify the path by using the -p or --path argument.
```

### Comparing `easy_deployer-0.1.2/easy_deployer/main.py` & `easy_deployer-0.1.3/easy_deployer/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from .shared_functions import listPromptInquirer, checkBoxPromptInquirer, runCmd, invalidAnswerExit, promptPyInquirer
+from asyncio.subprocess import PIPE
+from shared_functions import listPromptInquirer, checkBoxPromptInquirer, runCmd, invalidAnswerExit, promptPyInquirer
 from argparse import ArgumentParser
 import os, sys
 import re
 
-deploy_to_choices = ["github", "heroku"]
+deploy_to_choices = ["github"]
 command_choices = ["create-update", "update", "delete"]
 
 def main():
-    args = takeArgs()
+    args = take_args()
     if not args["to"]:
         args["to"] = listPromptInquirer({
             "name": "deploy_to",
             "question": "where d you want to deploy it?",
             "choices":deploy_to_choices
         })["deploy_to"]
     if not args["path"]:
@@ -22,56 +23,84 @@
             "message": f"Path of the project folder: ",
             "default": os.getcwd(),
             "validate": lambda x: "Invalid path" if not os.path.exists(x) else True
         })["path"]
     elif not os.path.exists(args["path"]):
             print("Invalid path")
             sys.exit(5)
-    additional_cmd = handleAdditionalCmds(args)
-    # runCmd(f"py easy_deployer/{args['to']}.py -p {args['path']} {additional_cmd}") # main command
+    additional_cmds = handle_additional_cmds(args)
+    # runCmd(f"py easy_deployer/{args['to']}.py -p {args['path']} {additional_cmds}") # main command
+    args_to = f"easy-deployer-{args['to']}"
+    current_dir = os.path.dirname(__file__)
+    """
+        priorities of execution:
+            ¤ this is .exe 
+                ¤ and executables are in same directory -> run 
+                ¤ and executables are not in the same directory 
+                    -> run global executables (the ones in the path env variable)
+            ¤ this is .py
+                ¤ and python (.py) package(s)/module(s) is in the same directory -> run those .py files
+                ¤ and python (.py) package(s)/module(s) is not in the same directory 
+                    -> run global executables (the ones in the path env variable)
+    """
+    # main command
     if(re.match(".+\.exe$", __file__)):
         # This is Executable (*.exe)
-        args_to = f"easy-{args['to']}"
-        current_dir = os.path.dirname(__file__)
-        runCmd(f"{os.path.join(current_dir, args_to)} -p {args['path']} {additional_cmd}") # main command
+        if(args_to +".exe" in os.listdir(current_dir)):
+            # if local file .exe is in the same directory then it will run it
+            runCmd(f"{os.path.join(current_dir, args_to)}.exe -p {args['path']} {additional_cmds}")
+        else:
+            # else it runs the global one
+            run_global_exe(args_to,args['path'],additional_cmds)
     else:
         # Assuming this is a python file (.py)
-        runCmd(f"py easy-{args['to']}.py -p {args['path']} {additional_cmd}") # main command
+        if(args["to"]+".py" in os.listdir(current_dir)):
+            # if python (.py) package(s)/module(s) is in the same directory then it will run it
+            runCmd(f"py {os.path.join(current_dir, args['to'])}.py -p {args['path']} {additional_cmds}")
+        else:
+            # else it runs the global one
+            run_global_exe(args_to,args['path'],additional_cmds) 
 
-def takeArgs():
+def run_global_exe(to, path, additional_cmds):
+    runCmd(f"easy-deployer-{to} -p {path} {additional_cmds}")
+
+
+def take_args():
     parser = ArgumentParser(prog="github-deployer",
     usage="""""", description="%(prog)s <commands> [options]")
     parser.add_argument("-p", "--path", required=False)
     parser.add_argument("-to", required=False, choices=deploy_to_choices)
     parser.add_argument("-cmd", "--command", choices=command_choices, help="Command to execute")
-    parser.add_argument("-q", "--quick", action="store_true", help="")
+    parser.add_argument("-q", "--quick", action="store_true", help="No additional commands needed")
     args = parser.parse_args()
     return vars(args)
 
-def handleAdditionalCmds(args):
-    additional_cmd = ""
+
+
+def handle_additional_cmds(args):
+    additional_cmds = ""
     if args["to"] == "github":
-        additional_cmd = githubCommands(args)
+        additional_cmds = github_commands(args)
     elif args["to"] == "heroku":
-        additional_cmd = herokuCommands(args)
+        additional_cmds = heroku_commands(args)
         # add_addtional_cmds = listPromptInquirer({
         #     "name":"add_addtional_cmds",
         #     "question": "want to add some additional commands?",
         #     "choices": ["Yes", "No"]
         #     })["add_addtional_cmds"]
-    return additional_cmd
+    return additional_cmds
 
-def githubCommands(args):
-    additional_cmd = ""
+def github_commands(args):
+    additional_cmds = ""
     command = listPromptInquirer({
         "name":"command",
         "question": "which command you want? (create-update is the default one)",
         "choices": ["create-update", "update", "delete"],
     })['command'] if not args["command"] else args["command"]
-    additional_cmd += f"{command} "
+    additional_cmds += f"{command} "
     if command == 'create-update':
         pass
     if not args["quick"]:
         add_addtional_cmds = listPromptInquirer({
             "name":"add_addtional_cmds",
             "question": "Want to add some additional commands?",
             "choices": ["Yes", "No"]
@@ -88,79 +117,79 @@
                     "question": "Add what you want (use spacebar to add stuff and enter to confirm)",
                     "choices": [
                         ADD_COLLABORATORS_CHOICE, GIT_IGNORE_CHOICE,
                         VISIBILITY_CHOICE, RESET_TOKEN_CHOICE, RESET_USER_CHOICE
                     ]
                 })
                 if(RESET_TOKEN_CHOICE in checkBoxAnswers["secondaryOptions"]) or (RESET_USER_CHOICE in checkBoxAnswers["secondaryOptions"]):
-                    additional_cmd += "-new "
+                    additional_cmds += "-new "
                     if RESET_TOKEN_CHOICE in checkBoxAnswers["secondaryOptions"]:
-                        additional_cmd += "token "
+                        additional_cmds += "token "
                     if RESET_USER_CHOICE in checkBoxAnswers["secondaryOptions"]:
-                        additional_cmd += "user "
+                        additional_cmds += "user "
                 if(GIT_IGNORE_CHOICE in checkBoxAnswers["secondaryOptions"]):
-                    additional_cmd += "-git-ig "
+                    additional_cmds += "-git-ig "
                 if(VISIBILITY_CHOICE in checkBoxAnswers["secondaryOptions"]):
-                    additional_cmd += "-visibility "
+                    additional_cmds += "-visibility "
                 if(ADD_COLLABORATORS_CHOICE in checkBoxAnswers["secondaryOptions"]):
-                    additional_cmd += "-ac "
+                    additional_cmds += "-ac "
             else:
                 RESET_TOKEN_CHOICE = "Reset token"
                 RESET_USER_CHOICE = "Reset user"
                 checkBoxAnswers = checkBoxPromptInquirer({
                     "name": "secondaryOptions",
                     "question": "Add what you want (use spacebar to add stuff and enter to confirm)",
                     "choices": [
                         RESET_TOKEN_CHOICE, RESET_USER_CHOICE
                     ]
                 })
                 if(RESET_TOKEN_CHOICE in checkBoxAnswers["secondaryOptions"]) or (RESET_USER_CHOICE in checkBoxAnswers["secondaryOptions"]):
-                    additional_cmd += "-new "
+                    additional_cmds += "-new "
                     if RESET_TOKEN_CHOICE in checkBoxAnswers["secondaryOptions"]:
-                        additional_cmd += "token "
+                        additional_cmds += "token "
                     if RESET_USER_CHOICE in checkBoxAnswers["secondaryOptions"]:
-                        additional_cmd += "user "
-    return additional_cmd
+                        additional_cmds += "user "
+    return additional_cmds
 
-def herokuCommands(args):
-    additional_cmd = ""
+def heroku_commands(args):
+    additional_cmds = ""
     FRAMEWORK_LANGUAGE_CHOICES = ["nodejs", "flask"]
     command = listPromptInquirer({
         "name":"command",
         "question": "which command you want? (create-update is the default one)",
         "choices": ["create-update", "update", "delete"],
     })['command'] if not args["command"] else args["command"]
-    additional_cmd += f"{command} "
+    additional_cmds += f"{command} "
     if command == 'create-update':
         listAnswers = listPromptInquirer({
                     "name": "language",
                     "question": "what language/framework are you using?",
                     "choices": FRAMEWORK_LANGUAGE_CHOICES
                 })
-        additional_cmd += f"-lang {listAnswers['language']} "
+        additional_cmds += f"-lang {listAnswers['language']} "
     if not args["quick"]:
         add_additional_cmds = promptPyInquirer({
             "type": "confirm",
             "name": "add_additional_cmds",
             "message": "Want to add some additional commands?",
         })["add_additional_cmds"]
         if add_additional_cmds:
             NEW_LOGIN = "Force a new login"
             NO_CACHE = "Remove cached info (like application name)"
-            additional_cmds = promptPyInquirer({
+            add_additional_cmds = promptPyInquirer({
                 "name":"secondaryOptions",
                 "type": "checkbox",
                 "choices": [
                     {"name": NEW_LOGIN},
                     {"name": NO_CACHE}
                 ],
                 "message": "Add the option(s) you want "
             })
-            if NEW_LOGIN in additional_cmds['secondaryOptions']:
-                additional_cmd += f"-new-login "
-            if NO_CACHE in additional_cmds['secondaryOptions']:
-                additional_cmd += f"-no-cache "
-    return additional_cmd
+            if NEW_LOGIN in add_additional_cmds['secondaryOptions']:
+                additional_cmds += f"-new-login "
+            if NO_CACHE in add_additional_cmds['secondaryOptions']:
+                additional_cmds += f"-no-cache "
+    return additional_cmds
             
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `easy_deployer-0.1.2/easy_deployer/shared_functions.py` & `easy_deployer-0.1.3/easy_deployer/shared_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,17 +165,19 @@
         if "\"" in commit_msg:
             print("double quotes detected, error!")
             sys.exit(15)
         cmds.append(f"git -C {path} commit -m \"{commit_msg}\"")
     
     for cmd in cmds:
         startText="processing"
-        if "add" in cmd:
+        if cmds.index(cmd) == 0:
+            # command is "git add ."
             startText="Adding files"
-        elif "commit" in cmd:
+        elif cmds.index(cmd) == 1:
+            # command is git commit
             startText="Committing changes"
         loading = Loading(startText=startText, stopText="", timeout=1)
         loading.start()
         runCmd(cmd, stdout=PIPE, stderr=PIPE, loading=loading)
         loading.stop()
 
 def handleGitInit(path):
@@ -220,22 +222,22 @@
             else:
                 print(error)
             sys.exit(5)
         return out.decode() if out else out
 
 def runCmd(cmd, **options):
     """
-    *cmd (string): the command to be executed
-    * stdin (dict):
-        stdin (None|PIPE)
-        stdout (None|PIPE)
-        error (str)
-        quitOnError (bool)
-        timeout (None|float)
-        loading (Loading)  
+    * cmd (string): the command to be executed
+    * options(dict):
+            * stdin (None|PIPE)
+            * stdout (None|PIPE)
+            * error (str)
+            * quitOnError (bool)
+            * timeout (None|float)
+            * loading (Loading)  
     """
     stdin = options["stdin"] if "stdin" in options else None
     stdout = options["stdout"] if "stdout" in options else None
     stderr = options["stderr"] if "stderr" in options else None
     error = options["error"] if "error" in options else "an error has been caught\n"
     quitOnError = options["quitOnError"] if "quitOnError" in options else True
     timeout = options["timeout"] if "timeout" in options else None
@@ -272,15 +274,14 @@
     out = runCmd("git branch", stdout=PIPE, stderr=PIPE)
     if "main" in out:
         return
     runCmd("git branch -m master main", stdout=PIPE, stderr=PIPE)
     runCmd("git checkout main", stdout=DEVNULL, stderr=PIPE)
 
 def printWarning(*text,**keywords):
-    print("*")
     print("""
     ******************************************
                   _   __               __    
         \  /\  / /_\ |__| |\ | | |\ | |  __
          \/  \/ /   \|  \ | \| | | \| |__|  """)
     print("\t",*text, **keywords)
     print("""
```

### Comparing `easy_deployer-0.1.2/easy_deployer.egg-info/PKG-INFO` & `easy_deployer-0.1.3/easy_deployer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: easy-deployer
-Version: 0.1.2
-Summary: UNKNOWN
+Version: 0.1.3
 Home-page: https://github.com/medamine980/easy-deployer
 Author: Mohamed-Amine Benali
 Author-email: namelowy_64@hotmail.com
 License: MIT
-Description: # Easy-Deployer:
-        Easy-deployer is used to simplify and speed up the deployment process.
-        It's mostly still in progress...
-        
-        ## OS Support:
-        Currently windows is the only supported os.
 Keywords: python,github,github-deployer,heroku,heroku-deployer,deploy,easy,easy-deployer,simple,simple-deployer
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Easy-Deployer:
+Easy-deployer is used to simplify and speed up the deployment process.
+It's mostly still in progress...
+
+## OS Support:
+Currently windows is the only supported os.
```

### Comparing `easy_deployer-0.1.2/setup.py` & `easy_deployer-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_desc = f.read()
 setup(
     name="easy_deployer",
-    version="0.1.2",
+    version="0.1.3",
     long_description=long_desc,
     long_description_content_type='text/markdown',
     author="Mohamed-Amine Benali",
     author_email="namelowy_64@hotmail.com",
     url="https://github.com/medamine980/easy-deployer",
     
     packages=find_packages(exclude=["easy_deployer.dist", "easy_deployer.ignore"]),
```

