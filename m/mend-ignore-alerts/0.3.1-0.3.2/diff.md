# Comparing `tmp/mend_ignore_alerts-0.3.1-py3-none-any.whl.zip` & `tmp/mend_ignore_alerts-0.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11964 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-04 07:27 mend_ignore_alerts/__init__.py
--rw-r--r--  2.0 unx      107 b- defN 23-Jul-04 07:27 mend_ignore_alerts/_version.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-04 07:27 mend_ignore_alerts/conftest.py
--rw-r--r--  2.0 unx     1554 b- defN 23-Jul-04 07:27 mend_ignore_alerts/const.py
--rw-r--r--  2.0 unx    10726 b- defN 23-Jul-04 07:27 mend_ignore_alerts/ignore_alerts.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-04 07:27 mend_ignore_alerts-0.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5030 b- defN 23-Jul-04 07:27 mend_ignore_alerts-0.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 07:27 mend_ignore_alerts-0.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-Jul-04 07:27 mend_ignore_alerts-0.3.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-04 07:27 mend_ignore_alerts-0.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      979 b- defN 23-Jul-04 07:27 mend_ignore_alerts-0.3.1.dist-info/RECORD
-11 files, 29936 bytes uncompressed, 10272 bytes compressed:  65.7%
+Zip file size: 12945 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-24 13:39 mend_ignore_alerts/__init__.py
+-rw-r--r--  2.0 unx      107 b- defN 23-Jul-24 13:39 mend_ignore_alerts/_version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-24 13:39 mend_ignore_alerts/conftest.py
+-rw-r--r--  2.0 unx     1669 b- defN 23-Jul-24 13:39 mend_ignore_alerts/const.py
+-rw-r--r--  2.0 unx    15814 b- defN 23-Jul-24 13:39 mend_ignore_alerts/ignore_alerts.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-24 13:39 mend_ignore_alerts-0.3.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6063 b- defN 23-Jul-24 13:39 mend_ignore_alerts-0.3.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 13:39 mend_ignore_alerts-0.3.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Jul-24 13:39 mend_ignore_alerts-0.3.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-24 13:39 mend_ignore_alerts-0.3.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      979 b- defN 23-Jul-24 13:39 mend_ignore_alerts-0.3.2.dist-info/RECORD
+11 files, 36172 bytes uncompressed, 11253 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: mend_ignore_alerts/const.py
 Comment: 
 
 Filename: mend_ignore_alerts/ignore_alerts.py
 Comment: 
 
-Filename: mend_ignore_alerts-0.3.1.dist-info/LICENSE
+Filename: mend_ignore_alerts-0.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: mend_ignore_alerts-0.3.1.dist-info/METADATA
+Filename: mend_ignore_alerts-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: mend_ignore_alerts-0.3.1.dist-info/WHEEL
+Filename: mend_ignore_alerts-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: mend_ignore_alerts-0.3.1.dist-info/entry_points.txt
+Filename: mend_ignore_alerts-0.3.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: mend_ignore_alerts-0.3.1.dist-info/top_level.txt
+Filename: mend_ignore_alerts-0.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mend_ignore_alerts-0.3.1.dist-info/RECORD
+Filename: mend_ignore_alerts-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mend_ignore_alerts/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 __tool_name__ = "ignore_alerts"
 __description__ = "Parse yml file and update alerts"
```

## mend_ignore_alerts/const.py

```diff
@@ -1,23 +1,24 @@
 from enum import Enum
 import os
 
 
 class aliases(Enum): # List of aliases for params
     apikey = ("--apiKey","--api-key", "--orgToken")
     userkey = ("--user-key", "--userKey")
+    url = ("--url", "--mendUrl")
     projectkey = ("--scope", "--projectToken")
     productkey = ("--productToken", "--product")
-    url = ("--url", "--mendUrl")
-    output = ("--out", "--dir")
-    sbom = ("--sbom", "--input")
+    exclude = ("--exclude", "-exclude")
     yaml = ("--yaml", "-yaml")
     githubpat = ("--ghpat", "-ghpat")
     githubowner = ("--ghowner", "-ghowner")
     githubrepo = ("--ghrepo", "-ghrepo")
+    output = ("--out", "-out")
+    mode = ("--mode", "-mode")
 
     @classmethod
     def get_aliases_str(cls, key):
         res = list()
         for elem_ in cls.__dict__[key].value:
             res.append(elem_)
             if elem_ != elem_.lower():
@@ -28,18 +29,20 @@
 class varenvs(Enum): # Lit of Env.variables
     wsuserkey = ("WS_USERKEY", "MEND_USERKEY")
     wsapikey = ("MEND_APIKEY","WS_APIKEY","WS_TOKEN")
     wsurl = ("WS_WSS_URL","MEND_WSS_URL","WS_URL","MEND_URL")
     wsscope = ("WS_SCOPE","MEND_SCOPE")
     wsproduct = ("WS_PRODUCTTOKEN", "MEND_PRODUCTTOKEN")
     wsproject = ("WS_PROJECTTOKEN", "MEND_PROJECTTOKEN")
-    waiver = ("MEND_WAIVER", "WS_WAIVER")
+    wsexclude = ("WS_EXCLUDE", "MEND_EXCLUDE")
+    yaml = ("MEND_YAML", "WS_YAML")
     githubpat = ("WS_GHPAT", "MEND_GHPAT", "GHPAT")
     githubowner = ("WS_GHOWNER", "MEND_GHOWNER", "GHOWNER")
     githubrepo = ("WS_GHREPO", "MEND_GHREPO", "GHREPO")
+    wsmode = ("WS_MODE","MEND_MODE")
 
     @classmethod
     def get_env(cls, key):
         res = ""
         for el_ in cls.__dict__[key].value:
             res = os.environ.get(el_)
             if res:
```

## mend_ignore_alerts/ignore_alerts.py

```diff
@@ -66,29 +66,93 @@
     parser = argparse.ArgumentParser(description=__description__)
     parser.add_argument(*aliases.get_aliases_str("userkey"), help="Mend user key", dest='ws_user_key',
                         default=varenvs.get_env("wsuserkey"), required=not varenvs.get_env("wsuserkey"))
     parser.add_argument(*aliases.get_aliases_str("apikey"), help="Mend API key", dest='ws_token',
                         default=varenvs.get_env("wsapikey"), required=not varenvs.get_env("wsapikey"))
     parser.add_argument(*aliases.get_aliases_str("url"), help="Mend server URL", dest='ws_url',
                         default=varenvs.get_env("wsurl"), required=not varenvs.get_env("wsurl"))
-    #parser.add_argument(*aliases.get_aliases_str("projectkey"), help="Mend project scope", dest='scope_token',
-    #                    default=varenvs.get_env("wsproject"))
-    parser.add_argument(*aliases.get_aliases_str("yaml"), help="YAML file", dest='yaml',
-                        default=varenvs.get_env("waiver"), required=not varenvs.get_env("waiver"))
+    parser.add_argument(*aliases.get_aliases_str("productkey"), help="Mend product scope", dest='producttoken',
+                        default=varenvs.get_env("wsproduct"))
+    parser.add_argument(*aliases.get_aliases_str("projectkey"), help="Mend project scope", dest='projecttoken',
+                        default=varenvs.get_env("wsproject"))
+    parser.add_argument(*aliases.get_aliases_str("exclude"), help="Exclude Mend project/product scope", dest='exclude',
+                        default=varenvs.get_env("wsexclude"))
+    parser.add_argument(*aliases.get_aliases_str("mode"), help="Creation YAML file or loading", dest='mode',
+                        default=varenvs.get_env("wsmode"), required=not varenvs.get_env("wsmode"))
+    parser.add_argument(*aliases.get_aliases_str("yaml"), help="Output or input YAML file", dest='yaml',
+                        default=varenvs.get_env("yaml"))
     parser.add_argument(*aliases.get_aliases_str("githubpat"), help="GitHub PAT", dest='pat',
                         default=varenvs.get_env("githubpat"))
     parser.add_argument(*aliases.get_aliases_str("githubrepo"), help="GitHub Repo", dest='repo',
                         default=varenvs.get_env("githubrepo"))
     parser.add_argument(*aliases.get_aliases_str("githubowner"), help="GitHub Owner", dest='owner',
                         default=varenvs.get_env("githubowner"))
     arguments = parser.parse_args()
 
     return arguments
 
 
+def get_project_list():
+    def get_prj_name(token):
+        data_prj = json.dumps({
+            "requestType": "getProjectVitals",
+            "userKey": args.ws_user_key,
+            "projectToken": token
+        })
+        res = json.loads(call_ws_api(data=data_prj))
+        return try_or_error(lambda: f'{res["projectVitals"][0]["productName"]}:{res["projectVitals"][0]["name"]}', try_or_error(lambda: res["errorMessage"],
+                                                      f"Internal error during getting project data by token {token}"))
+
+    res = []
+    if args.projecttoken:
+        res.extend([{x: get_prj_name(x)} for x in args.projecttoken.split(",")])
+
+    if args.producttoken:
+        products = args.producttoken.split(",")
+        for product_ in products:
+            data_prj = json.dumps(
+                {"requestType": "getAllProjects",
+                 "userKey": args.ws_user_key,
+                 "productToken": product_,
+                 })
+            try:
+                prj_data = json.loads(call_ws_api(data=data_prj))["projects"]
+                res.extend([{x["projectToken"]: get_prj_name(x["projectToken"])} for x in prj_data])  # x["projectName"]
+            except Exception as err:
+                pass
+    elif not args.projecttoken:
+        data_prj = json.dumps(
+            {"requestType": "getOrganizationProjectVitals",
+             "userKey": args.ws_user_key,
+             "orgToken": args.apikey,
+             })
+        try:
+            prj_data = json.loads(call_ws_api(data=data_prj))["projectVitals"]
+            res.extend([{x["token"]: get_prj_name(x["token"])} for x in prj_data])  # x["name"]
+        except:
+            pass
+
+    exclude_tokens = []
+    if args.exclude:
+        excludes = args.exclude.split(",")
+        for exclude_ in excludes:
+            data_prj = json.dumps(
+                {"requestType": "getAllProjects",
+                 "userKey": args.ws_user_key,
+                 "productToken": exclude_,
+                 })
+            try:
+                prj_data = json.loads(call_ws_api(data=data_prj))["projects"]
+                exclude_tokens.extend([{x["projectToken"]: get_prj_name(x["projectToken"])} for x in prj_data])  #  x["projectName"]
+            except:
+                exclude_tokens.append(exclude_)
+        res = list(set(res) - set(exclude_tokens))
+    return res
+
+
 def extract_url(url: str) -> str:
     url_ = url if url.startswith("https://") else f"https://{url}"
     url_ = url_.replace("http://", "")
     pos = url_.find("/", 8)  # Not using any suffix, just direct url
     return url_[0:pos] if pos > -1 else url_
 
 
@@ -105,14 +169,44 @@
 
     except Exception as err:
         res = f"Error was raised. {err}"
         logger.error(f'[{ex()}] {err}')
     return res
 
 
+def create_yaml_ignored_alerts(prj_tokens):
+    try:
+        data_yml = []
+        for token_ in prj_tokens:
+            for key, value in token_.items():
+                alerts = get_ingnored_alerts(key)  # By project token
+                vuln = []
+                if alerts:
+                    for alert_ in alerts:
+                        for key_, value_ in alert_.items():
+                            vuln.append(
+                                {
+                                    'id_vuln': key_,
+                                    'note': value_,
+                                }
+                            )
+                if vuln:
+                    val_arr = value.split(":")
+                    data_yml.append({
+                        'productname': val_arr[0],  # Product Name
+                        'projectname': val_arr[1],  # Project Name
+                        'vulns': vuln
+                    })
+        with open(f'{args.yaml}', 'w') as file:
+            yaml.dump(data_yml, file)
+        return f"The file {args.yaml} created successfully"
+    except Exception as err:
+        return f"The file {args.yaml} was not created. Details: {err}"
+
+
 def create_waiver():
     global args
     data = json.dumps(
         {"requestType": "getProjectAlerts",
          "userKey": args.ws_user_key,
          "projectToken": args.scope_token,
          })
@@ -189,19 +283,25 @@
 
 def read_yaml(yml_file):
     with open(yml_file, 'r') as file:
         data = yaml.safe_load(file)
     return data
 
 
-def get_token_by_prj_name(prj_name):
+def get_token_by_prj_name(prj_name, prd_name):
     for prj_ in short_lst_prj:
         for key, value in prj_.items():
-            if value["name"] == prj_name:
-                return key
+            val_arr = value.split(":")
+            if val_arr[1] == prj_name and (val_arr[0] == prd_name or not prd_name):
+                if prd_name:
+                    return key
+                else:
+                    logger.info(f"The product is not defined in the input file; "
+                                f"the project was found just by project name {prj_name}")
+                    return key
     return ""
 
 
 def get_alerts_by_type(prj_token, alert_type):
     try:
         data = json.dumps({
             "requestType": "getProjectAlertsByType",
@@ -227,40 +327,41 @@
     except:
         return f"Failed Ignore operation for alert UUID {alert_uuid}"
 
 
 def exec_input_yaml(input_data):
     input_data_ = [input_data] if type(input_data) is dict else input_data
     for el_ in input_data_:
-        prj_token = get_token_by_prj_name(el_["name"])
+        prj_token = get_token_by_prj_name(prj_name=try_or_error(lambda: el_["name"], try_or_error(lambda: el_["projectname"], "")), prd_name=try_or_error(lambda : el_["productname"], ""))
         if prj_token:
             #restore_alerts(project=prj_token)
             ignored_al = get_ingnored_alerts(project=prj_token)
             alerts = get_alerts_by_type(prj_token=prj_token, alert_type="SECURITY_VULNERABILITY")
             try:
                 for data_ in el_["vulns"]:
                     note = data_["note"]
-                    status, note_ign = is_vuln_in_ignored(vulnerability=data_["vuln_id"],ign_list=ignored_al)
+                    vuln_id = try_or_error(lambda: data_["vuln_id"], try_or_error(lambda: data_["id_vuln"], ""))
+                    status, note_ign = is_vuln_in_ignored(vulnerability=vuln_id,ign_list=ignored_al)
                     if not status:
                         alert_uuid = ""
                         for alert_ in alerts:
-                            if alert_["vulnerability"]["name"] == data_["vuln_id"] and "SNYK" not in data_["vuln_id"]:
+                            if alert_["vulnerability"]["name"] == vuln_id and "SNYK" not in vuln_id:
                                 alert_uuid = alert_["alertUuid"]
                                 break
                         if alert_uuid :
                             logger.info(set_ignore_alert(alert_uuid=alert_uuid,comment=note))
                         else:
-                            logger.info(f"The {data_['vuln_id']} was not found")
+                            logger.info(f"The {vuln_id} was not found in the project {try_or_error(lambda: el_['name'], try_or_error(lambda: el_['projectname'], ''))}")
                     else:
-                        logger.warning(f"The vulnerability {data_['vuln_id']} in project {el_['name']} "
+                        logger.warning(f"The vulnerability {vuln_id} in the project {try_or_error(lambda: el_['name'], try_or_error(lambda: el_['projectname'], ''))} "
                                     f"has been ignored already with comment: {note_ign}")
             except Exception as err:
                 logger.error(f"Error: {err}")
         else:
-            logger.warning(f"The project {el_['name']} was not identified")
+            logger.warning(f"The project {try_or_error(lambda: el_['name'], try_or_error(lambda: el_['projectname'], ''))} was not identified")
 
 
 def main():
     global args
     global short_lst_prj
 
     hdr_title = f'{APP_TITLE} {__version__}'
@@ -275,26 +376,32 @@
                 g = Github(args.pat)
                 repo = g.get_repo(f'{args.repo}') if "/" in args.repo else g.get_repo(f'{args.owner}/{args.repo}')
                 input_data = repo.get_contents(args.yaml).decoded_content.decode("utf-8")
             except Exception as err:
                 logger.error(f"Access to {args.owner}/{args.repo} forbidden")
         #create_waiver()
         logger.info(f'[{fn()}] Getting project list')
+        '''
         load_prj = json.dumps({
             "requestType" : "getOrganizationProjectVitals",
              "userKey": args.ws_user_key,
              "orgToken" : args.ws_token
         })
-        short_lst_prj = [{x["token"]: {"product": ["productName"], "name": x["name"]}} for x in json.loads(call_ws_api(data=load_prj))["projectVitals"]]
+        short_lst_prj = [{x["token"]: {"product": x["productName"], "name": x["name"]}} for x in json.loads(call_ws_api(data=load_prj))["projectVitals"]]
         logger.info(f'[{fn()}] Analyzing YAML file')
-        try:
-            input_data = yaml.safe_load(input_data) if input_data else read_yaml(args.yaml)
-            exec_input_yaml(input_data=input_data)
-        except Exception as err:
-            logger.error(f"[{fn()}] Impossible to parse file {args.yaml}. Details: {err}")
+        '''
+        short_lst_prj = get_project_list()
+        if args.mode.lower() == "create":
+            logger.info(create_yaml_ignored_alerts(short_lst_prj))
+        elif args.yaml:
+            try:
+                input_data = yaml.safe_load(input_data) if input_data else read_yaml(args.yaml)
+                exec_input_yaml(input_data=input_data)
+            except Exception as err:
+                logger.error(f"[{fn()}] Impossible to parse file {args.yaml}. Details: {err}")
         logger.info(f'[{fn()}] Operation was finished successfully')
     except Exception as err:
         logger.error(f'[{fn()}] Failed to getting project list. Details: {err}')
         exit(-1)
 
 
 if __name__ == '__main__':
```

## Comparing `mend_ignore_alerts-0.3.1.dist-info/LICENSE` & `mend_ignore_alerts-0.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mend_ignore_alerts-0.3.1.dist-info/METADATA` & `mend_ignore_alerts-0.3.2.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mend-ignore-alerts
-Version: 0.3.1
+Version: 0.3.2
 Summary: Parse yml file and update alerts
 Home-page: https://github.com/mend-toolkit/ignore-alerts
 Author: Mend Professional Services
 Author-email: ps@mend.io
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -22,15 +22,15 @@
 
 [![Logo](https://resources.mend.io/mend-sig/logo/mend-dark-logo-horizontal.png)](https://www.mend.io/)  
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
 
 # Ignore Alerts
 
-Set Ignore status for alert based on whaiver Yaml  
+Set Ignore status for alert based on input YAML file  
 
 <hr>
 
 - [Supported Operating Systems](#supported-operating-systems)
 - [Prerequisites](#prerequisites)
 - [Installation](#installation)
 - [Configuration Parameters](#configuration-parameters)
@@ -56,48 +56,49 @@
 > **Note:** Depending on whether the package was installed as a root user or not, you need to make sure the package installation location was added to the `$PATH` environment variable.
 
 ## Configuration Parameters
 >**Note:** Parameters can be specified as either command-line arguments, environment variables, or a combination of both.  
 > 
 > Command-line arguments take precedence over environment variables.  
 
-| CLI argument                 | Env. Variable |   Type   | Required | Description                       |
-|:-----------------------------|:--------------|:--------:|:--------:|:----------------------------------|
-| **&#x2011;&#x2011;help**     |               | `switch` |    No    | Show help and exit                |
-| **&#x2011;&#x2011;user-key** | `WS_USERKEY`  | `string` |   Yes    | Mend User Key                     |
-| **&#x2011;&#x2011;api-key**  | `WS_APIKEY`   | `string` |   Yes    | Mend API Key                      |
-| **&#x2011;&#x2011;url**      | `WS_WSS_URL`  | `string` |   Yes    | Mend Server URL                   |
-| **&#x2011;&#x2011;yaml**     | `WS_WAIVER`   | `string` |   Yes    | Filename of Yaml file for parsing |
-| **&#x2011;&#x2011;ghpat**    | `WS_GHPAT`    | `string` |    No    | GitHub PAT                        |
-| **&#x2011;&#x2011;ghowner**  | `WS_GHOWNER`  | `string` |    No    | GitHub Owner                      |
-| **&#x2011;&#x2011;ghrepo**   | `WS_GHREPO`   | `string` |    No    | GitHub Repo name                  |
+| CLI argument                 | Env. Variable |   Type   | Required | Description                                                                                                       |
+|:-----------------------------|:--------------|:--------:|:--------:|:------------------------------------------------------------------------------------------------------------------|
+| **&#x2011;&#x2011;help**     |               | `switch` |    No    | Show help and exit                                                                                                |
+| **&#x2011;&#x2011;user-key** | `WS_USERKEY`  | `string` |   Yes    | Mend User Key                                                                                                     |
+| **&#x2011;&#x2011;api-key**  | `WS_APIKEY`   | `string` |   Yes    | Mend API Key                                                                                                      |
+| **&#x2011;&#x2011;url**      | `WS_URL`      | `string` |   Yes    | Mend Server URL                                                                                                   |
+| **&#x2011;&#x2011;yaml**     | `WS_YAML`     | `string` |   Yes    | Yaml file's name for parsing in case `mode` is equal `load`. If `mode` is `create` then Yaml file will be created |
+| **&#x2011;&#x2011;mode**     | `WS_MODE`     | `string` |   Yes    | `create` or `load` value                                                                                          |
+| **&#x2011;&#x2011;ghpat**    | `WS_GHPAT`    | `string` |    No    | GitHub PAT                                                                                                        |
+| **&#x2011;&#x2011;ghowner**  | `WS_GHOWNER`  | `string` |    No    | GitHub Owner                                                                                                      |
+| **&#x2011;&#x2011;ghrepo**   | `WS_GHREPO`   | `string` |    No    | GitHub Repo name                                                                                                  |
 
 
 ## Usage
 **Using command-line arguments only:**
 ```shell
-ignore_alerts --user-key WS_USERKEY --api-key WS_APIKEY --url $WS_WSS_URL --yaml $WS_WAIVER
+ignore_alerts --user-key WS_USERKEY --api-key WS_APIKEY --url $WS_WSS_URL --yaml $WS_YAML --mode create
 ```
 **Using environment variables:**
 ```shell
 export WS_USERKEY=xxxxxxxxxxx
 export WS_APIKEY=xxxxxxxxxxx
 export WS_URL=https://saas.mend.io
-export WS_WAYVER=waiverexample.yml
+export WS_YAML=waiverexample.yml
 
 ignore_alerts
 ```
 > **Note:** Either form is accepted. For the rest of the examples, the latter form would be used  
 
 **Getting waiver file from GitHub Repo:**
 ```shell
 export WS_USERKEY=xxxxxxxxxxx
 export WS_APIKEY=xxxxxxxxxxx
 export WS_URL=https://saas.mend.io
-export WS_WAYVER=waiverexample.yml
+export WS_YAML=waiverexample.yml
 export WS_GHPAT=xxxxxxxxxxx
 export WS_GHOWNER = xxxxxxxxxxx
 export WS_GHREPO = TestRepoName 
 
 ignore_alerts
 ```
 
@@ -127,25 +128,25 @@
         env:
           WS_APIKEY: ${{ secrets.apikey }}
           USER_KEY: ${{ secrets.userkey }}
           WS_URL: "saas.mend.io"
           YAML: "examplewaiver.yml"
           
         run: 
-          ignore_alerts --url $WS_URL --yaml $YAML --apiKey $WS_APIKEY --user-key $USER_KEY
+          ignore_alerts --url $WS_URL --yaml $YAML --apiKey $WS_APIKEY --user-key $USER_KEY --mode load
 ```
 
 The YAML file should be placed in the Repo folder on GitHub 
 
 ## Execution Examples
 
-> **Note:** In the following examples, $WS_USERKEY, $WS_APIKEY and $WS_URL are assumed to have been exported as environment variables.  
+> **Note:** In the following examples, $WS_USERKEY, $WS_APIKEY, $WS_URL and $WS_MODE are assumed to have been exported as environment variables.  
 
 ```shell
 $ ignore_alerts --yaml whaiverexample.yml
 ```
 
 Usind examplewaiver.yml file from some Repo
 
 ```shell
-$ ignore_alerts --yaml whaiverexample.yml --ghpat xxxxxxx --ghowner Owner --ghrepo RepoName  
+$ ignore_alerts --yaml whaiverexample.yml --ghpat xxxxxxx --ghowner Owner --ghrepo RepoName --mode create 
 ```
```

## Comparing `mend_ignore_alerts-0.3.1.dist-info/RECORD` & `mend_ignore_alerts-0.3.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 mend_ignore_alerts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mend_ignore_alerts/_version.py,sha256=WNW2ShReXUp0v-qHX3NDr0Bt3oMWEHOL4_sIB1__KnE,107
+mend_ignore_alerts/_version.py,sha256=i06QFJn0Ps42kPe30RY4KW2-TDTgE2A4dmRx5X7hYM8,107
 mend_ignore_alerts/conftest.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mend_ignore_alerts/const.py,sha256=aRDadkUul_6NZB_LDIZTkGf5VkWTPqfnj6eap-1Y7As,1554
-mend_ignore_alerts/ignore_alerts.py,sha256=yOHiByN3TXMZ8bNdDi62CkKKIEvGXVXrUQOB-QtwFNk,10726
-mend_ignore_alerts-0.3.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mend_ignore_alerts-0.3.1.dist-info/METADATA,sha256=uCdMj7UiFYVPMtzuwcesbThGcbigDwQqk_uwde2O3sI,5030
-mend_ignore_alerts-0.3.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mend_ignore_alerts-0.3.1.dist-info/entry_points.txt,sha256=b_q3jF-WbTVm6sR0BrVXts8u1OhXtD1aM2IZ5CfWmpE,72
-mend_ignore_alerts-0.3.1.dist-info/top_level.txt,sha256=ookvTXlTz4JKFzjrBd6U6MmV6RzYs9C8B2E2vMscaZ8,19
-mend_ignore_alerts-0.3.1.dist-info/RECORD,,
+mend_ignore_alerts/const.py,sha256=WCmSRPTpp8sZzaV7jQ0uGfNwlvxk979aSBBPKk3fSz4,1669
+mend_ignore_alerts/ignore_alerts.py,sha256=aapvmAqedcPUSOmNf2tvUK5jiEc7HYJvmrGx9k00Yds,15814
+mend_ignore_alerts-0.3.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mend_ignore_alerts-0.3.2.dist-info/METADATA,sha256=0ztNqMI5AjDYxZ4-km359FY9FjG8AfzOYN4zmpAfLJ8,6063
+mend_ignore_alerts-0.3.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+mend_ignore_alerts-0.3.2.dist-info/entry_points.txt,sha256=b_q3jF-WbTVm6sR0BrVXts8u1OhXtD1aM2IZ5CfWmpE,72
+mend_ignore_alerts-0.3.2.dist-info/top_level.txt,sha256=ookvTXlTz4JKFzjrBd6U6MmV6RzYs9C8B2E2vMscaZ8,19
+mend_ignore_alerts-0.3.2.dist-info/RECORD,,
```

