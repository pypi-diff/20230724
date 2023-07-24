# Comparing `tmp/electrolytes-0.2.4.tar.gz` & `tmp/electrolytes-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "electrolytes-0.2.4.tar", last modified: Thu Jul 20 21:42:38 2023, max compression
+gzip compressed data, was "electrolytes-0.3.0.tar", last modified: Mon Jul 24 21:03:47 2023, max compression
```

## Comparing `electrolytes-0.2.4.tar` & `electrolytes-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:42:38.151828 electrolytes-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-20 21:42:28.000000 electrolytes-0.2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-07-20 21:42:38.151828 electrolytes-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-20 21:42:28.000000 electrolytes-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:42:38.151828 electrolytes-0.2.4/electrolytes/
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-07-20 21:42:28.000000 electrolytes-0.2.4/electrolytes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-07-20 21:42:28.000000 electrolytes-0.2.4/electrolytes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   174238 2023-07-20 21:42:28.000000 electrolytes-0.2.4/electrolytes/db1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:42:38.151828 electrolytes-0.2.4/electrolytes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-07-20 21:42:38.000000 electrolytes-0.2.4/electrolytes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-20 21:42:38.000000 electrolytes-0.2.4/electrolytes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:42:38.000000 electrolytes-0.2.4/electrolytes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-20 21:42:38.000000 electrolytes-0.2.4/electrolytes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 21:42:38.000000 electrolytes-0.2.4/electrolytes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 21:42:38.000000 electrolytes-0.2.4/electrolytes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-20 21:42:28.000000 electrolytes-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 21:42:38.151828 electrolytes-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:42:38.151828 electrolytes-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-20 21:42:28.000000 electrolytes-0.2.4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-20 21:42:28.000000 electrolytes-0.2.4/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:03:47.855215 electrolytes-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-24 21:03:34.000000 electrolytes-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-24 21:03:47.855215 electrolytes-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-24 21:03:34.000000 electrolytes-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:03:47.851215 electrolytes-0.3.0/electrolytes/
+-rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-07-24 21:03:34.000000 electrolytes-0.3.0/electrolytes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-07-24 21:03:34.000000 electrolytes-0.3.0/electrolytes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174238 2023-07-24 21:03:34.000000 electrolytes-0.3.0/electrolytes/db1.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:03:34.000000 electrolytes-0.3.0/electrolytes/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:03:47.855215 electrolytes-0.3.0/electrolytes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-24 21:03:47.000000 electrolytes-0.3.0/electrolytes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-24 21:03:47.000000 electrolytes-0.3.0/electrolytes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:03:47.000000 electrolytes-0.3.0/electrolytes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-24 21:03:47.000000 electrolytes-0.3.0/electrolytes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-24 21:03:47.000000 electrolytes-0.3.0/electrolytes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 21:03:47.000000 electrolytes-0.3.0/electrolytes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-24 21:03:34.000000 electrolytes-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:03:47.855215 electrolytes-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:03:47.855215 electrolytes-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-24 21:03:34.000000 electrolytes-0.3.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-24 21:03:34.000000 electrolytes-0.3.0/tests/test_cli.py
```

### Comparing `electrolytes-0.2.4/LICENSE.txt` & `electrolytes-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `electrolytes-0.2.4/PKG-INFO` & `electrolytes-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: electrolytes
-Version: 0.2.4
+Version: 0.3.0
 Summary: Electrolyte database manager
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/microfluidica/electrolytes
 Project-URL: Repository, https://github.com/microfluidica/electrolytes
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pydantic :: 2
@@ -94,20 +94,21 @@
 The public stubs of the `Constituent` class are:
 
 ```python
 class Constituent:
     def __init__(self,
                  *,
                  name: str,
-                 u_neg: Sequence[float],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
-                 u_pos: Sequence[float],  # [+1, +2, +3, ..., +pos_count]
-                 pkas_neg: Sequence[float],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
-                 pkas_pos: Sequence[float],  # [+1, +2, +3, ..., +pos_count]
-                 neg_count: int = -1,
-                 pos_count: int = -1): ...
+                 u_neg: Sequence[float] = [],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
+                 u_pos: Sequence[float] = [],  # [+1, +2, +3, ..., +pos_count]
+                 pkas_neg: Sequence[float] = [],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
+                 pkas_pos: Sequence[float] = [],  # [+1, +2, +3, ..., +pos_count]
+                 neg_count: int = None, # == len(u_neg) == len(pkas_neg)
+                 pos_count: int = None): # == len(u_pos) == len(pkas_pos)
+        ...
 
     # Interface for electroMicroTransport
     def mobilities(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3), SI units
     def pkas(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3)
     def diffusivity(self) -> float: ...  # SI units
 ```
```

### Comparing `electrolytes-0.2.4/README.md` & `electrolytes-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -63,20 +63,21 @@
 The public stubs of the `Constituent` class are:
 
 ```python
 class Constituent:
     def __init__(self,
                  *,
                  name: str,
-                 u_neg: Sequence[float],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
-                 u_pos: Sequence[float],  # [+1, +2, +3, ..., +pos_count]
-                 pkas_neg: Sequence[float],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
-                 pkas_pos: Sequence[float],  # [+1, +2, +3, ..., +pos_count]
-                 neg_count: int = -1,
-                 pos_count: int = -1): ...
+                 u_neg: Sequence[float] = [],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
+                 u_pos: Sequence[float] = [],  # [+1, +2, +3, ..., +pos_count]
+                 pkas_neg: Sequence[float] = [],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
+                 pkas_pos: Sequence[float] = [],  # [+1, +2, +3, ..., +pos_count]
+                 neg_count: int = None, # == len(u_neg) == len(pkas_neg)
+                 pos_count: int = None): # == len(u_pos) == len(pkas_pos)
+        ...
 
     # Interface for electroMicroTransport
     def mobilities(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3), SI units
     def pkas(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3)
     def diffusivity(self) -> float: ...  # SI units
 ```
```

### Comparing `electrolytes-0.2.4/electrolytes/__main__.py` & `electrolytes-0.3.0/electrolytes/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,50 @@
+import sys
 from typing import Tuple, List
+if sys.version_info >= (3, 9):
+    from typing import Annotated
+else:
+    from typing_extensions import Annotated
 
 import typer
 from click import Context, Parameter
 
-from . import _APP_NAME, database, Constituent
+from . import database, Constituent
 
 
 app = typer.Typer()
 
 
 def complete_name(ctx: Context, param: Parameter, incomplete: str) -> List[str]:
     return [name for name in database if name.startswith(incomplete)]
 
 def complete_name_user_defined(ctx: Context, param: Parameter, incomplete: str) -> List[str]:
     return [name for name in database.user_defined() if name.startswith(incomplete)]
 
 
 @app.command()
-def add(name: str = typer.Argument(..., shell_complete=complete_name_user_defined),
-        p1: Tuple[float, float] = typer.Option((None, None), "+1", help="Mobility (*1e-9) and pKa for +1"),
-        p2: Tuple[float, float] = typer.Option((None, None), "+2", help="Mobility (*1e-9) and pKa for +2"),
-        p3: Tuple[float, float] = typer.Option((None, None), "+3", help="Mobility (*1e-9) and pKa for +3"),
-        p4: Tuple[float, float] = typer.Option((None, None), "+4", help="Mobility (*1e-9) and pKa for +4"),
-        p5: Tuple[float, float] = typer.Option((None, None), "+5", help="Mobility (*1e-9) and pKa for +5"),
-        p6: Tuple[float, float] = typer.Option((None, None), "+6", help="Mobility (*1e-9) and pKa for +6"),
-        m1: Tuple[float, float] = typer.Option((None, None), "-1", help="Mobility (*1e-9) and pKa for -1"),
-        m2: Tuple[float, float] = typer.Option((None, None), "-2", help="Mobility (*1e-9) and pKa for -2"),
-        m3: Tuple[float, float] = typer.Option((None, None), "-3", help="Mobility (*1e-9) and pKa for -3"),
-        m4: Tuple[float, float] = typer.Option((None, None), "-4", help="Mobility (*1e-9) and pKa for -4"),
-        m5: Tuple[float, float] = typer.Option((None, None), "-5", help="Mobility (*1e-9) and pKa for -5"),
-        m6: Tuple[float, float] = typer.Option((None, None), "-6", help="Mobility (*1e-9) and pKa for -6"),
-        force: bool = typer.Option(False, "-f", help="Replace any existing user-defined component with the same name")) -> None:
+def add(name: Annotated[str, typer.Argument(shell_complete=complete_name_user_defined)],
+        p1: Annotated[Tuple[float, float], typer.Option("+1", help="Mobility (*1e-9) and pKa for +1")] = (None, None), # type: ignore
+        p2: Annotated[Tuple[float, float], typer.Option("+2", help="Mobility (*1e-9) and pKa for +2")] = (None, None), # type: ignore
+        p3: Annotated[Tuple[float, float], typer.Option("+3", help="Mobility (*1e-9) and pKa for +3")] = (None, None), # type: ignore
+        p4: Annotated[Tuple[float, float], typer.Option("+4", help="Mobility (*1e-9) and pKa for +4")] = (None, None), # type: ignore
+        p5: Annotated[Tuple[float, float], typer.Option("+5", help="Mobility (*1e-9) and pKa for +5")] = (None, None), # type: ignore
+        p6: Annotated[Tuple[float, float], typer.Option("+6", help="Mobility (*1e-9) and pKa for +6")] = (None, None), # type: ignore
+        m1: Annotated[Tuple[float, float], typer.Option("-1", help="Mobility (*1e-9) and pKa for -1")] = (None, None), # type: ignore
+        m2: Annotated[Tuple[float, float], typer.Option("-2", help="Mobility (*1e-9) and pKa for -2")] = (None, None), # type: ignore
+        m3: Annotated[Tuple[float, float], typer.Option("-3", help="Mobility (*1e-9) and pKa for -3")] = (None, None), # type: ignore
+        m4: Annotated[Tuple[float, float], typer.Option("-4", help="Mobility (*1e-9) and pKa for -4")] = (None, None), # type: ignore
+        m5: Annotated[Tuple[float, float], typer.Option("-5", help="Mobility (*1e-9) and pKa for -5")] = (None, None), # type: ignore
+        m6: Annotated[Tuple[float, float], typer.Option("-6", help="Mobility (*1e-9) and pKa for -6")] = (None, None), # type: ignore
+        force: Annotated[bool, typer.Option("-f", help="Replace any existing user-defined component with the same name")] = False) -> None:
     """Save a user-defined component"""
     name = name.upper()
 
-    if not p1 and not m1:
+    if p1[0] is None and m1[0] is None:
+        assert p1[1] is None and m1[1] is None
         typer.echo("Error: at least one of the +1 or -1 options is required", err=True)
         raise typer.Exit(code=1)
 
     neg: List[Tuple[float, float]] = []
     any_omitted = False
     for i,m in enumerate([m1, m2, m3, m4, m5, m6]):
         if m[0] is None:
@@ -58,49 +64,50 @@
             any_omitted = True
         elif any_omitted:
             typer.echo(f"Error: missing charge -{i}", err=True)
             raise typer.Exit(code=1)
         else:
             pos.append(p)
 
-    if not force and database.is_user_defined(name):
-        typer.echo(f"Error: user-defined component {name} already exists (use -f to replace)", err=True)
-        raise typer.Exit(code=1)
+    with database._user_constituents_lock:
+        if not force and database.is_user_defined(name):
+            typer.echo(f"Error: user-defined component {name} already exists (use -f to replace)", err=True)
+            raise typer.Exit(code=1)
 
-    try:
-        constituent = Constituent(name=name,
-                                  u_neg=[x[0] for x in neg],
-                                  u_pos=[x[0] for x in pos],
-                                  pkas_neg=[x[1] for x in neg],
-                                  pkas_pos=[x[1] for x in pos])
-        
         try:
-            del database[name]
-        except KeyError:
-            pass
+            constituent = Constituent(name=name,
+                                    u_neg=[x[0] for x in neg],
+                                    u_pos=[x[0] for x in pos],
+                                    pkas_neg=[x[1] for x in neg],
+                                    pkas_pos=[x[1] for x in pos])
+            
+            try:
+                del database[name]
+            except KeyError:
+                pass
 
-        database.add(constituent)
+            database.add(constituent)
 
-    except Exception as e:
-        typer.echo(f"Error: {e}", err=True)
-        raise typer.Exit(code=1)
+        except Exception as e:
+            typer.echo(f"Error: {e}", err=True)
+            raise typer.Exit(code=1)
 
 
 @app.command()
-def info(name: str = typer.Argument(..., shell_complete=complete_name)) -> None:
+def info(name: Annotated[str, typer.Argument(shell_complete=complete_name)]) -> None:
     """Show the properties of a component"""
     name = name.upper()
 
     try:
         constituent = database[name]
     except KeyError:
         typer.echo(f"Error: {name}: no such component", err=True)
         raise typer.Exit(code=1)
 
-    charges = list(constituent.charges_pos[::-1]) + list(constituent.charges_neg[::-1])
+    charges = list(range(constituent.pos_count, 0, -1)) + list(range(-1, -constituent.neg_count - 1, -1))
     uu = constituent.u_pos[::-1] + constituent.u_neg[::-1]
     pkas = constituent.pkas_pos[::-1] + constituent.pkas_neg[::-1]
 
     assert len(charges) == len(uu) == len(pkas)
     
     typer.echo(f"Component: {name}")
     if database.is_user_defined(name):
@@ -108,27 +115,27 @@
     typer.echo( "                 " + " ".join(f"{c:^+8d}" for c in charges))
     typer.echo( "Mobilities *1e-9:" + " ".join(f"{u:^8.2f}" for u in uu))
     typer.echo( "pKas:            " + " ".join(f"{p:^8.2f}" for p in pkas))
     typer.echo(f"Diffusivity: {constituent.diffusivity():.4e}")
 
 
 @app.command()
-def ls(user_only: bool=typer.Option(False, "--user", help="Show only user-defined components")) -> None:
+def ls(user_only: Annotated[bool, typer.Option("--user", help="Show only user-defined components")] = False) -> None:
     """List available components"""
     if user_only:
         names = database.user_defined()
     else:
         names = database
 
     for name in names:
         typer.echo(name)
 
 
 @app.command()
-def rm(names: List[str] = typer.Argument(..., shell_complete=complete_name_user_defined)) -> None:
+def rm(names: Annotated[List[str], typer.Argument(shell_complete=complete_name_user_defined)]) -> None:
     """Remove user-defined components"""
     errors_ocurred = False
     for name in names:
         name = name.upper()
         try:
             del database[name]
         except KeyError:
@@ -140,15 +147,15 @@
     
     if errors_ocurred:
         raise typer.Exit(code=-1)
 
 
 @app.command()
 def search(text: str,
-           user_only: bool=typer.Option(False, "--user", help="Search only user-defined components")) -> None:
+           user_only: Annotated[bool, typer.Option("--user", help="Search only user-defined components")] = False) -> None:
     """Search the list of components"""
     text = text.upper()
 
     if user_only:
         names = list(database.user_defined())
     else:
         names = list(database)
@@ -157,8 +164,8 @@
 
     for name, index in zip(names, match_indices):
         if index != -1:
             typer.echo(name[0:index] + typer.style(name[index:index+len(text)], bold=True) + name[index+len(text):])
 
 
 if __name__ == "__main__":
-    app(prog_name=_APP_NAME)
+    app(prog_name=__package__)
```

### Comparing `electrolytes-0.2.4/electrolytes/db1.json` & `electrolytes-0.3.0/electrolytes/db1.json`

 * *Files identical despite different names*

### Comparing `electrolytes-0.2.4/electrolytes.egg-info/PKG-INFO` & `electrolytes-0.3.0/electrolytes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: electrolytes
-Version: 0.2.4
+Version: 0.3.0
 Summary: Electrolyte database manager
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/microfluidica/electrolytes
 Project-URL: Repository, https://github.com/microfluidica/electrolytes
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pydantic :: 2
@@ -94,20 +94,21 @@
 The public stubs of the `Constituent` class are:
 
 ```python
 class Constituent:
     def __init__(self,
                  *,
                  name: str,
-                 u_neg: Sequence[float],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
-                 u_pos: Sequence[float],  # [+1, +2, +3, ..., +pos_count]
-                 pkas_neg: Sequence[float],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
-                 pkas_pos: Sequence[float],  # [+1, +2, +3, ..., +pos_count]
-                 neg_count: int = -1,
-                 pos_count: int = -1): ...
+                 u_neg: Sequence[float] = [],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
+                 u_pos: Sequence[float] = [],  # [+1, +2, +3, ..., +pos_count]
+                 pkas_neg: Sequence[float] = [],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
+                 pkas_pos: Sequence[float] = [],  # [+1, +2, +3, ..., +pos_count]
+                 neg_count: int = None, # == len(u_neg) == len(pkas_neg)
+                 pos_count: int = None): # == len(u_pos) == len(pkas_pos)
+        ...
 
     # Interface for electroMicroTransport
     def mobilities(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3), SI units
     def pkas(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3)
     def diffusivity(self) -> float: ...  # SI units
 ```
```

### Comparing `electrolytes-0.2.4/pyproject.toml` & `electrolytes-0.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -26,16 +26,18 @@
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 
 dependencies = [
-    "typer>=0.4.2,<0.10",
+    "typer>=0.9.0,<0.10",
     "pydantic>=2.0.3,<3",
+    "filelock==3.*",
+    "typing-extensions>=3.7.4.3,<5; python_version<'3.9'",
 ]
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 lint = [
     "mypy==1.*",
@@ -55,11 +57,19 @@
 [tool.setuptools]
 packages = ["electrolytes"]
 
 [tool.setuptools.dynamic]
 version = {attr = "electrolytes.__version__"}
 
 [tool.setuptools.package-data]
-electrolytes = ["*.json"]
+electrolytes = [
+    "*.json",
+    "py.typed",
+]
 
 [tool.mypy]
 plugins = ["pydantic.mypy"]
+packages = [
+    "electrolytes",
+    "tests",
+]
+strict = true
```

### Comparing `electrolytes-0.2.4/tests/test_api.py` & `electrolytes-0.3.0/tests/test_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,13 +45,14 @@
         del database["NONEXISTENT2424612644"]
         
 
 def test_try_add_default() -> None:
     assert "SILVER" in database
     assert not database.is_user_defined("SILVER")
     assert "SILVER" not in database.user_defined()
-    database.add(Constituent(name="SILVER",
-                                u_pos=[64.50],
-                                pkas_pos=[11.70]))
+    with pytest.warns(UserWarning):
+        database.add(Constituent(name="SILVER",
+                                 u_pos=[64.50],
+                                 pkas_pos=[11.70]))
     assert "SILVER" in database
     assert not database.is_user_defined("SILVER")
     assert "SILVER" not in database.user_defined()
```

### Comparing `electrolytes-0.2.4/tests/test_cli.py` & `electrolytes-0.3.0/tests/test_cli.py`

 * *Files identical despite different names*

