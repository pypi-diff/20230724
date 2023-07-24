# Comparing `tmp/cog2-0.1.1.tar.gz` & `tmp/cog2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cog2-0.1.1.tar", max compression
+gzip compressed data, was "cog2-0.1.2.tar", max compression
```

## Comparing `cog2-0.1.1.tar` & `cog2-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       32 2023-07-23 13:47:37.324665 cog2-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-23 08:06:40.702710 cog2-0.1.1/cog2/__init__.py
--rw-r--r--   0        0        0     2848 2023-07-23 14:03:56.413434 cog2-0.1.1/cog2/main.py
--rw-r--r--   0        0        0      404 2023-07-23 14:05:26.303387 cog2-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 cog2-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      471 2023-07-24 01:23:20.558785 cog2-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-24 00:37:04.090024 cog2-0.1.2/cog2/__init__.py
+-rw-r--r--   0        0        0     2955 2023-07-24 05:06:38.456104 cog2-0.1.2/cog2/main.py
+-rw-r--r--   0        0        0      427 2023-07-24 05:07:08.649026 cog2-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 cog2-0.1.2/PKG-INFO
```

### Comparing `cog2-0.1.1/cog2/main.py` & `cog2-0.1.2/cog2/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,28 @@
         "This command will authenticate Docker with WizModel's Docker registry. You will need a WizModel.com account."
     )
     input(
         "Hit enter to get started. A browser will open with an authentication token that you need to paste here."
     )
     webbrowser.open("https://www.wizmodel.com/")
     token = typer.prompt("Paste your token here and press Enter to login")
-    data = {"token":token}
-    response = requests.post(url="https://api.stagingwazs.online/cog/v1/verify-token",json=data)
-    user_name = response.json()['username']
-    os.system("docker login -u {} -p {} registry.gpu-backend-prod.xyz".format(user_name,token))  # noqa: E501
+    data = {"token": token}
+    response = requests.post(url="https://api.stagingwazs.online/cog/v1/verify-token", json=data).json()
+    user_name = response['username']
+    password = response['docker_token']
+    os.system("docker login -u {} -p {} registry.gpu-backend-prod.xyz".format(user_name, password))  # noqa: E501
     typer.echo("Login cmd finished")
 
+
 @app.command()
 def build(
-    tag: Annotated[str,typer.Option("--tag","-t")]="" ,
-    no_cache: bool = typer.Option(False),
-    separate_weights: bool = typer.Option(False),
-    secret: Annotated[str,typer.Option("--secret")]=""
+        tag: Annotated[str, typer.Option("--tag", "-t")] = "",
+        no_cache: bool = typer.Option(False),
+        separate_weights: bool = typer.Option(False),
+        secret: Annotated[str, typer.Option("--secret")] = ""
 ):  # noqa: E501
     typer.echo("Building image with tag %s" % tag)
     prefix_cmd = "cog build"
     if tag != "":
         prefix_cmd = prefix_cmd + " -t {}".format(tag)
     if no_cache:
         prefix_cmd = prefix_cmd + " --no-cache"
@@ -43,45 +45,42 @@
         prefix_cmd = prefix_cmd + " --secret {}".format(secret)
     os.system(prefix_cmd)
     typer.echo("Build cmd finish: " + prefix_cmd)
 
 
 @app.command()
 def push(
-    no_cache: bool = typer.Option(False),
-    separate_weights: bool = typer.Option(False),
-    secret: Annotated[str,typer.Option("--secret")]=""
+        no_cache: bool = typer.Option(False),
+        separate_weights: bool = typer.Option(False),
+        secret: Annotated[str, typer.Option("--secret")] = ""
 ):
     prefix_cmd = "cog push"
     if no_cache:
         prefix_cmd = prefix_cmd + " --no-cache"
     if separate_weights:
         prefix_cmd = prefix_cmd + " --separate-weights"
     if len(secret) > 0:
         prefix_cmd = prefix_cmd + " --secret {}".format(secret)
     os.system(prefix_cmd)
     typer.echo("Push cmd finish: " + prefix_cmd)
 
+
 @app.command()
-def predict(input:Annotated[List[str],typer.Option("--input","-i")]=[], output:Annotated[str,typer.Option("--output","-o")]=""):  # noqa: E501
+def predict(input: Annotated[List[str], typer.Option("--input", "-i")] = [],
+            output: Annotated[str, typer.Option("--output", "-o")] = ""):  # noqa: E501
     prefix_cmd = "cog predict"
     if len(input) > 0:
         for item in input:
             prefix_cmd = prefix_cmd + " -i {}".format(item)
     if output != "":
         prefix_cmd = prefix_cmd + " --output {}".format(output)
     os.system(prefix_cmd)
-    typer.echo("Predict cmd finished: "+prefix_cmd)
+    typer.echo("Predict cmd finished: " + prefix_cmd)
+
 
 @app.command()
-def run(publish:Annotated[str,typer.Option("--publish","-p")]=""):
+def run(publish: Annotated[str, typer.Option("--publish", "-p")] = ""):
     prefix_cmd = "cog run"
     if len(publish) > 0:
         prefix_cmd = prefix_cmd + " -p {}".format(publish)
     os.system(prefix_cmd)
-    typer.echo("Run cmd finished: "+prefix_cmd)
-
-    
-
-
-
-
+    typer.echo("Run cmd finished: " + prefix_cmd)
```

