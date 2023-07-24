# Comparing `tmp/mypy-boto3-apigatewayv2-1.28.0.tar.gz` & `tmp/mypy-boto3-apigatewayv2-1.28.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-apigatewayv2-1.28.0.tar", last modified: Thu Jul  6 20:58:55 2023, max compression
+gzip compressed data, was "mypy-boto3-apigatewayv2-1.28.10.tar", last modified: Mon Jul 24 19:49:46 2023, max compression
```

## Comparing `mypy-boto3-apigatewayv2-1.28.0.tar` & `mypy-boto3-apigatewayv2-1.28.10.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.366214 mypy-boto3-apigatewayv2-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:33:02.000000 mypy-boto3-apigatewayv2-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20492 2023-07-06 20:58:55.366214 mypy-boto3-apigatewayv2-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18987 2023-07-06 20:33:02.000000 mypy-boto3-apigatewayv2-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.366214 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-06 20:33:02.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-06 20:33:02.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:33:02.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51692 2023-07-06 20:33:04.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51603 2023-07-06 20:33:04.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-07-06 20:33:04.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-07-06 20:33:04.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-06 20:33:04.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-07-06 20:33:04.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:33:02.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    75269 2023-07-06 20:33:06.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    75158 2023-07-06 20:33:05.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:33:02.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.366214 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20492 2023-07-06 20:58:55.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 20:58:55.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:55.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:55.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:55.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 20:58:55.000000 mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:55.366214 mypy-boto3-apigatewayv2-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:33:02.000000 mypy-boto3-apigatewayv2-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.284631 mypy-boto3-apigatewayv2-1.28.10/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-24 19:46:52.000000 mypy-boto3-apigatewayv2-1.28.10/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-07-24 19:49:46.284631 mypy-boto3-apigatewayv2-1.28.10/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19201 2023-07-24 19:46:52.000000 mypy-boto3-apigatewayv2-1.28.10/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.284631 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-24 19:46:52.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-24 19:46:52.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-24 19:46:52.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51692 2023-07-24 19:46:52.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51603 2023-07-24 19:46:52.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-07-24 19:46:53.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-24 19:46:53.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-24 19:46:52.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-07-24 19:46:52.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:46:52.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    74892 2023-07-24 19:46:54.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74801 2023-07-24 19:46:54.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 19:46:52.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.284631 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-07-24 19:49:46.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-24 19:49:46.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:49:46.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:49:46.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 19:49:46.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 19:49:46.000000 mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:49:46.284631 mypy-boto3-apigatewayv2-1.28.10/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-24 19:46:52.000000 mypy-boto3-apigatewayv2-1.28.10/setup.py
```

### Comparing `mypy-boto3-apigatewayv2-1.28.0/LICENSE` & `mypy-boto3-apigatewayv2-1.28.10/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.0/PKG-INFO` & `mypy-boto3-apigatewayv2-1.28.10/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigatewayv2
-Version: 1.28.0
-Summary: Type annotations for boto3.ApiGatewayV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.10
+Summary: Type annotations for boto3.ApiGatewayV2 1.28.10 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigatewayv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigatewayv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-apigatewayv2?color=blue)](https://pypistats.org/packages/mypy-boto3-apigatewayv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApiGatewayV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
+[boto3.ApiGatewayV2 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-apigatewayv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,35 +368,37 @@
 ### Typed dictionaries
 
 `mypy_boto3_apigatewayv2.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apigatewayv2.type_defs import (
+    AccessLogSettingsOutputTypeDef,
     AccessLogSettingsTypeDef,
     ApiMappingTypeDef,
+    CorsOutputTypeDef,
+    JWTConfigurationOutputTypeDef,
     CorsTypeDef,
-    JWTConfigurationTypeDef,
     CreateApiMappingRequestRequestTypeDef,
-    CreateApiMappingResponseTypeDef,
+    ResponseMetadataTypeDef,
+    JWTConfigurationTypeDef,
     CreateDeploymentRequestRequestTypeDef,
-    CreateDeploymentResponseTypeDef,
     DomainNameConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
+    DomainNameConfigurationOutputTypeDef,
     MutualTlsAuthenticationTypeDef,
     TlsConfigInputTypeDef,
     CreateIntegrationResponseRequestRequestTypeDef,
-    CreateIntegrationResponseResponseTypeDef,
     TlsConfigTypeDef,
     CreateModelRequestRequestTypeDef,
-    CreateModelResponseTypeDef,
     ParameterConstraintsTypeDef,
+    ParameterConstraintsOutputTypeDef,
     RouteSettingsTypeDef,
+    RouteSettingsOutputTypeDef,
     CreateVpcLinkRequestRequestTypeDef,
-    CreateVpcLinkResponseTypeDef,
     DeleteAccessLogSettingsRequestRequestTypeDef,
     DeleteApiMappingRequestRequestTypeDef,
     DeleteApiRequestRequestTypeDef,
     DeleteAuthorizerRequestRequestTypeDef,
     DeleteCorsConfigurationRequestRequestTypeDef,
     DeleteDeploymentRequestRequestTypeDef,
     DeleteDomainNameRequestRequestTypeDef,
@@ -406,140 +408,144 @@
     DeleteRouteRequestParameterRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
     DeleteRouteResponseRequestRequestTypeDef,
     DeleteRouteSettingsRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeleteVpcLinkRequestRequestTypeDef,
     DeploymentTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportApiRequestRequestTypeDef,
-    ExportApiResponseTypeDef,
     GetApiMappingRequestRequestTypeDef,
-    GetApiMappingResponseTypeDef,
     GetApiMappingsRequestRequestTypeDef,
     GetApiRequestRequestTypeDef,
-    GetApisRequestGetApisPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetApisRequestRequestTypeDef,
     GetAuthorizerRequestRequestTypeDef,
-    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
     GetAuthorizersRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
-    GetDeploymentResponseTypeDef,
-    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDomainNameRequestRequestTypeDef,
-    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
     GetDomainNamesRequestRequestTypeDef,
     GetIntegrationRequestRequestTypeDef,
     GetIntegrationResponseRequestRequestTypeDef,
-    GetIntegrationResponseResponseTypeDef,
-    GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
     GetIntegrationResponsesRequestRequestTypeDef,
     IntegrationResponseTypeDef,
-    GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
     GetIntegrationsRequestRequestTypeDef,
     GetModelRequestRequestTypeDef,
-    GetModelResponseTypeDef,
     GetModelTemplateRequestRequestTypeDef,
-    GetModelTemplateResponseTypeDef,
-    GetModelsRequestGetModelsPaginateTypeDef,
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetRouteRequestRequestTypeDef,
     GetRouteResponseRequestRequestTypeDef,
-    GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
     GetRouteResponsesRequestRequestTypeDef,
-    GetRoutesRequestGetRoutesPaginateTypeDef,
     GetRoutesRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
-    GetStagesRequestGetStagesPaginateTypeDef,
     GetStagesRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
-    GetTagsResponseTypeDef,
     GetVpcLinkRequestRequestTypeDef,
-    GetVpcLinkResponseTypeDef,
     GetVpcLinksRequestRequestTypeDef,
     VpcLinkTypeDef,
     ImportApiRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ReimportApiRequestRequestTypeDef,
     ResetAuthorizersCacheRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiMappingRequestRequestTypeDef,
-    UpdateApiMappingResponseTypeDef,
     UpdateDeploymentRequestRequestTypeDef,
-    UpdateDeploymentResponseTypeDef,
     UpdateIntegrationResponseRequestRequestTypeDef,
-    UpdateIntegrationResponseResponseTypeDef,
     UpdateModelRequestRequestTypeDef,
-    UpdateModelResponseTypeDef,
     UpdateVpcLinkRequestRequestTypeDef,
-    UpdateVpcLinkResponseTypeDef,
-    GetApiMappingsResponseTypeDef,
     ApiTypeDef,
+    AuthorizerTypeDef,
     CreateApiRequestRequestTypeDef,
+    UpdateApiRequestRequestTypeDef,
+    CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
+    CreateAuthorizerResponseTypeDef,
+    CreateDeploymentResponseTypeDef,
+    CreateIntegrationResponseResponseTypeDef,
+    CreateModelResponseTypeDef,
+    CreateVpcLinkResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportApiResponseTypeDef,
+    GetApiMappingResponseTypeDef,
+    GetApiMappingsResponseTypeDef,
     GetApiResponseTypeDef,
+    GetAuthorizerResponseTypeDef,
+    GetDeploymentResponseTypeDef,
+    GetIntegrationResponseResponseTypeDef,
+    GetModelResponseTypeDef,
+    GetModelTemplateResponseTypeDef,
+    GetTagsResponseTypeDef,
+    GetVpcLinkResponseTypeDef,
     ImportApiResponseTypeDef,
     ReimportApiResponseTypeDef,
-    UpdateApiRequestRequestTypeDef,
+    UpdateApiMappingResponseTypeDef,
     UpdateApiResponseTypeDef,
-    AuthorizerTypeDef,
+    UpdateAuthorizerResponseTypeDef,
+    UpdateDeploymentResponseTypeDef,
+    UpdateIntegrationResponseResponseTypeDef,
+    UpdateModelResponseTypeDef,
+    UpdateVpcLinkResponseTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
-    CreateAuthorizerResponseTypeDef,
-    GetAuthorizerResponseTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
-    UpdateAuthorizerResponseTypeDef,
     CreateDomainNameRequestRequestTypeDef,
     UpdateDomainNameRequestRequestTypeDef,
     CreateDomainNameResponseTypeDef,
     DomainNameTypeDef,
     GetDomainNameResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     CreateIntegrationRequestRequestTypeDef,
     UpdateIntegrationRequestRequestTypeDef,
     CreateIntegrationResultTypeDef,
     GetIntegrationResultTypeDef,
     IntegrationTypeDef,
     UpdateIntegrationResultTypeDef,
     CreateRouteRequestRequestTypeDef,
     CreateRouteResponseRequestRequestTypeDef,
+    UpdateRouteRequestRequestTypeDef,
+    UpdateRouteResponseRequestRequestTypeDef,
     CreateRouteResponseResponseTypeDef,
     CreateRouteResultTypeDef,
     GetRouteResponseResponseTypeDef,
     GetRouteResultTypeDef,
     RouteResponseTypeDef,
     RouteTypeDef,
-    UpdateRouteRequestRequestTypeDef,
-    UpdateRouteResponseRequestRequestTypeDef,
     UpdateRouteResponseResponseTypeDef,
     UpdateRouteResultTypeDef,
     CreateStageRequestRequestTypeDef,
+    UpdateStageRequestRequestTypeDef,
     CreateStageResponseTypeDef,
     GetStageResponseTypeDef,
     StageTypeDef,
-    UpdateStageRequestRequestTypeDef,
     UpdateStageResponseTypeDef,
     GetDeploymentsResponseTypeDef,
+    GetApisRequestGetApisPaginateTypeDef,
+    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
+    GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+    GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+    GetModelsRequestGetModelsPaginateTypeDef,
+    GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+    GetRoutesRequestGetRoutesPaginateTypeDef,
+    GetStagesRequestGetStagesPaginateTypeDef,
     GetIntegrationResponsesResponseTypeDef,
     GetModelsResponseTypeDef,
     GetVpcLinksResponseTypeDef,
     GetApisResponseTypeDef,
     GetAuthorizersResponseTypeDef,
     GetDomainNamesResponseTypeDef,
     GetIntegrationsResponseTypeDef,
     GetRouteResponsesResponseTypeDef,
     GetRoutesResponseTypeDef,
     GetStagesResponseTypeDef,
 )
 
 
-def get_structure() -> AccessLogSettingsTypeDef:
+def get_structure() -> AccessLogSettingsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-apigatewayv2-1.28.0/README.md` & `mypy-boto3-apigatewayv2-1.28.10/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigatewayv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigatewayv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-apigatewayv2?color=blue)](https://pypistats.org/packages/mypy-boto3-apigatewayv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApiGatewayV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
+[boto3.ApiGatewayV2 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-apigatewayv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,35 +336,37 @@
 ### Typed dictionaries
 
 `mypy_boto3_apigatewayv2.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apigatewayv2.type_defs import (
+    AccessLogSettingsOutputTypeDef,
     AccessLogSettingsTypeDef,
     ApiMappingTypeDef,
+    CorsOutputTypeDef,
+    JWTConfigurationOutputTypeDef,
     CorsTypeDef,
-    JWTConfigurationTypeDef,
     CreateApiMappingRequestRequestTypeDef,
-    CreateApiMappingResponseTypeDef,
+    ResponseMetadataTypeDef,
+    JWTConfigurationTypeDef,
     CreateDeploymentRequestRequestTypeDef,
-    CreateDeploymentResponseTypeDef,
     DomainNameConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
+    DomainNameConfigurationOutputTypeDef,
     MutualTlsAuthenticationTypeDef,
     TlsConfigInputTypeDef,
     CreateIntegrationResponseRequestRequestTypeDef,
-    CreateIntegrationResponseResponseTypeDef,
     TlsConfigTypeDef,
     CreateModelRequestRequestTypeDef,
-    CreateModelResponseTypeDef,
     ParameterConstraintsTypeDef,
+    ParameterConstraintsOutputTypeDef,
     RouteSettingsTypeDef,
+    RouteSettingsOutputTypeDef,
     CreateVpcLinkRequestRequestTypeDef,
-    CreateVpcLinkResponseTypeDef,
     DeleteAccessLogSettingsRequestRequestTypeDef,
     DeleteApiMappingRequestRequestTypeDef,
     DeleteApiRequestRequestTypeDef,
     DeleteAuthorizerRequestRequestTypeDef,
     DeleteCorsConfigurationRequestRequestTypeDef,
     DeleteDeploymentRequestRequestTypeDef,
     DeleteDomainNameRequestRequestTypeDef,
@@ -374,140 +376,144 @@
     DeleteRouteRequestParameterRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
     DeleteRouteResponseRequestRequestTypeDef,
     DeleteRouteSettingsRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeleteVpcLinkRequestRequestTypeDef,
     DeploymentTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportApiRequestRequestTypeDef,
-    ExportApiResponseTypeDef,
     GetApiMappingRequestRequestTypeDef,
-    GetApiMappingResponseTypeDef,
     GetApiMappingsRequestRequestTypeDef,
     GetApiRequestRequestTypeDef,
-    GetApisRequestGetApisPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetApisRequestRequestTypeDef,
     GetAuthorizerRequestRequestTypeDef,
-    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
     GetAuthorizersRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
-    GetDeploymentResponseTypeDef,
-    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDomainNameRequestRequestTypeDef,
-    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
     GetDomainNamesRequestRequestTypeDef,
     GetIntegrationRequestRequestTypeDef,
     GetIntegrationResponseRequestRequestTypeDef,
-    GetIntegrationResponseResponseTypeDef,
-    GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
     GetIntegrationResponsesRequestRequestTypeDef,
     IntegrationResponseTypeDef,
-    GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
     GetIntegrationsRequestRequestTypeDef,
     GetModelRequestRequestTypeDef,
-    GetModelResponseTypeDef,
     GetModelTemplateRequestRequestTypeDef,
-    GetModelTemplateResponseTypeDef,
-    GetModelsRequestGetModelsPaginateTypeDef,
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetRouteRequestRequestTypeDef,
     GetRouteResponseRequestRequestTypeDef,
-    GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
     GetRouteResponsesRequestRequestTypeDef,
-    GetRoutesRequestGetRoutesPaginateTypeDef,
     GetRoutesRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
-    GetStagesRequestGetStagesPaginateTypeDef,
     GetStagesRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
-    GetTagsResponseTypeDef,
     GetVpcLinkRequestRequestTypeDef,
-    GetVpcLinkResponseTypeDef,
     GetVpcLinksRequestRequestTypeDef,
     VpcLinkTypeDef,
     ImportApiRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ReimportApiRequestRequestTypeDef,
     ResetAuthorizersCacheRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiMappingRequestRequestTypeDef,
-    UpdateApiMappingResponseTypeDef,
     UpdateDeploymentRequestRequestTypeDef,
-    UpdateDeploymentResponseTypeDef,
     UpdateIntegrationResponseRequestRequestTypeDef,
-    UpdateIntegrationResponseResponseTypeDef,
     UpdateModelRequestRequestTypeDef,
-    UpdateModelResponseTypeDef,
     UpdateVpcLinkRequestRequestTypeDef,
-    UpdateVpcLinkResponseTypeDef,
-    GetApiMappingsResponseTypeDef,
     ApiTypeDef,
+    AuthorizerTypeDef,
     CreateApiRequestRequestTypeDef,
+    UpdateApiRequestRequestTypeDef,
+    CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
+    CreateAuthorizerResponseTypeDef,
+    CreateDeploymentResponseTypeDef,
+    CreateIntegrationResponseResponseTypeDef,
+    CreateModelResponseTypeDef,
+    CreateVpcLinkResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportApiResponseTypeDef,
+    GetApiMappingResponseTypeDef,
+    GetApiMappingsResponseTypeDef,
     GetApiResponseTypeDef,
+    GetAuthorizerResponseTypeDef,
+    GetDeploymentResponseTypeDef,
+    GetIntegrationResponseResponseTypeDef,
+    GetModelResponseTypeDef,
+    GetModelTemplateResponseTypeDef,
+    GetTagsResponseTypeDef,
+    GetVpcLinkResponseTypeDef,
     ImportApiResponseTypeDef,
     ReimportApiResponseTypeDef,
-    UpdateApiRequestRequestTypeDef,
+    UpdateApiMappingResponseTypeDef,
     UpdateApiResponseTypeDef,
-    AuthorizerTypeDef,
+    UpdateAuthorizerResponseTypeDef,
+    UpdateDeploymentResponseTypeDef,
+    UpdateIntegrationResponseResponseTypeDef,
+    UpdateModelResponseTypeDef,
+    UpdateVpcLinkResponseTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
-    CreateAuthorizerResponseTypeDef,
-    GetAuthorizerResponseTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
-    UpdateAuthorizerResponseTypeDef,
     CreateDomainNameRequestRequestTypeDef,
     UpdateDomainNameRequestRequestTypeDef,
     CreateDomainNameResponseTypeDef,
     DomainNameTypeDef,
     GetDomainNameResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     CreateIntegrationRequestRequestTypeDef,
     UpdateIntegrationRequestRequestTypeDef,
     CreateIntegrationResultTypeDef,
     GetIntegrationResultTypeDef,
     IntegrationTypeDef,
     UpdateIntegrationResultTypeDef,
     CreateRouteRequestRequestTypeDef,
     CreateRouteResponseRequestRequestTypeDef,
+    UpdateRouteRequestRequestTypeDef,
+    UpdateRouteResponseRequestRequestTypeDef,
     CreateRouteResponseResponseTypeDef,
     CreateRouteResultTypeDef,
     GetRouteResponseResponseTypeDef,
     GetRouteResultTypeDef,
     RouteResponseTypeDef,
     RouteTypeDef,
-    UpdateRouteRequestRequestTypeDef,
-    UpdateRouteResponseRequestRequestTypeDef,
     UpdateRouteResponseResponseTypeDef,
     UpdateRouteResultTypeDef,
     CreateStageRequestRequestTypeDef,
+    UpdateStageRequestRequestTypeDef,
     CreateStageResponseTypeDef,
     GetStageResponseTypeDef,
     StageTypeDef,
-    UpdateStageRequestRequestTypeDef,
     UpdateStageResponseTypeDef,
     GetDeploymentsResponseTypeDef,
+    GetApisRequestGetApisPaginateTypeDef,
+    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
+    GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+    GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+    GetModelsRequestGetModelsPaginateTypeDef,
+    GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+    GetRoutesRequestGetRoutesPaginateTypeDef,
+    GetStagesRequestGetStagesPaginateTypeDef,
     GetIntegrationResponsesResponseTypeDef,
     GetModelsResponseTypeDef,
     GetVpcLinksResponseTypeDef,
     GetApisResponseTypeDef,
     GetAuthorizersResponseTypeDef,
     GetDomainNamesResponseTypeDef,
     GetIntegrationsResponseTypeDef,
     GetRouteResponsesResponseTypeDef,
     GetRoutesResponseTypeDef,
     GetStagesResponseTypeDef,
 )
 
 
-def get_structure() -> AccessLogSettingsTypeDef:
+def get_structure() -> AccessLogSettingsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/__init__.py` & `mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/__init__.pyi` & `mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/__main__.py` & `mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApiGatewayV2 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.ApiGatewayV2 1.28.10\nVersion:         1.28.10\nBuilder"
+        " version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.0")
+    print("1.28.10")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/client.py` & `mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/client.pyi` & `mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/literals.py` & `mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,14 +296,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/literals.pyi` & `mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -294,14 +294,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/paginator.py` & `mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,148 +82,148 @@
 class GetApisPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetApis)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getapispaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetApisResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetApis.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getapispaginator)
         """
 
 
 class GetAuthorizersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetAuthorizers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getauthorizerspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetAuthorizersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetAuthorizers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getauthorizerspaginator)
         """
 
 
 class GetDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getdeploymentspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getdeploymentspaginator)
         """
 
 
 class GetDomainNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDomainNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getdomainnamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDomainNamesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDomainNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getdomainnamespaginator)
         """
 
 
 class GetIntegrationResponsesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrationResponses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getintegrationresponsespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, IntegrationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, IntegrationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetIntegrationResponsesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrationResponses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getintegrationresponsespaginator)
         """
 
 
 class GetIntegrationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getintegrationspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetIntegrationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getintegrationspaginator)
         """
 
 
 class GetModelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetModels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getmodelspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getmodelspaginator)
         """
 
 
 class GetRouteResponsesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRouteResponses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getrouteresponsespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, RouteId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, RouteId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRouteResponsesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRouteResponses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getrouteresponsespaginator)
         """
 
 
 class GetRoutesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRoutes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getroutespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRoutesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRoutes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getroutespaginator)
         """
 
 
 class GetStagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetStages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getstagespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetStagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetStages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getstagespaginator)
         """
```

### Comparing `mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/paginator.pyi` & `mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -79,139 +79,139 @@
 class GetApisPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetApis)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getapispaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetApisResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetApis.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getapispaginator)
         """
 
 class GetAuthorizersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetAuthorizers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getauthorizerspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetAuthorizersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetAuthorizers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getauthorizerspaginator)
         """
 
 class GetDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getdeploymentspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getdeploymentspaginator)
         """
 
 class GetDomainNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDomainNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getdomainnamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDomainNamesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDomainNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getdomainnamespaginator)
         """
 
 class GetIntegrationResponsesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrationResponses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getintegrationresponsespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, IntegrationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, IntegrationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetIntegrationResponsesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrationResponses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getintegrationresponsespaginator)
         """
 
 class GetIntegrationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getintegrationspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetIntegrationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getintegrationspaginator)
         """
 
 class GetModelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetModels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getmodelspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getmodelspaginator)
         """
 
 class GetRouteResponsesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRouteResponses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getrouteresponsespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, RouteId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, RouteId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRouteResponsesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRouteResponses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getrouteresponsespaginator)
         """
 
 class GetRoutesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRoutes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getroutespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRoutesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRoutes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getroutespaginator)
         """
 
 class GetStagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetStages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getstagespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetStagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetStages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getstagespaginator)
         """
```

### Comparing `mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/type_defs.py` & `mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for apigatewayv2 service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_apigatewayv2.type_defs import AccessLogSettingsTypeDef
+    from mypy_boto3_apigatewayv2.type_defs import AccessLogSettingsOutputTypeDef
 
-    data: AccessLogSettingsTypeDef = {...}
+    data: AccessLogSettingsOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -41,35 +41,37 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AccessLogSettingsOutputTypeDef",
     "AccessLogSettingsTypeDef",
     "ApiMappingTypeDef",
+    "CorsOutputTypeDef",
+    "JWTConfigurationOutputTypeDef",
     "CorsTypeDef",
-    "JWTConfigurationTypeDef",
     "CreateApiMappingRequestRequestTypeDef",
-    "CreateApiMappingResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "JWTConfigurationTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
-    "CreateDeploymentResponseTypeDef",
     "DomainNameConfigurationTypeDef",
     "MutualTlsAuthenticationInputTypeDef",
+    "DomainNameConfigurationOutputTypeDef",
     "MutualTlsAuthenticationTypeDef",
     "TlsConfigInputTypeDef",
     "CreateIntegrationResponseRequestRequestTypeDef",
-    "CreateIntegrationResponseResponseTypeDef",
     "TlsConfigTypeDef",
     "CreateModelRequestRequestTypeDef",
-    "CreateModelResponseTypeDef",
     "ParameterConstraintsTypeDef",
+    "ParameterConstraintsOutputTypeDef",
     "RouteSettingsTypeDef",
+    "RouteSettingsOutputTypeDef",
     "CreateVpcLinkRequestRequestTypeDef",
-    "CreateVpcLinkResponseTypeDef",
     "DeleteAccessLogSettingsRequestRequestTypeDef",
     "DeleteApiMappingRequestRequestTypeDef",
     "DeleteApiRequestRequestTypeDef",
     "DeleteAuthorizerRequestRequestTypeDef",
     "DeleteCorsConfigurationRequestRequestTypeDef",
     "DeleteDeploymentRequestRequestTypeDef",
     "DeleteDomainNameRequestRequestTypeDef",
@@ -79,190 +81,202 @@
     "DeleteRouteRequestParameterRequestRequestTypeDef",
     "DeleteRouteRequestRequestTypeDef",
     "DeleteRouteResponseRequestRequestTypeDef",
     "DeleteRouteSettingsRequestRequestTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DeleteVpcLinkRequestRequestTypeDef",
     "DeploymentTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportApiRequestRequestTypeDef",
-    "ExportApiResponseTypeDef",
     "GetApiMappingRequestRequestTypeDef",
-    "GetApiMappingResponseTypeDef",
     "GetApiMappingsRequestRequestTypeDef",
     "GetApiRequestRequestTypeDef",
-    "GetApisRequestGetApisPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetApisRequestRequestTypeDef",
     "GetAuthorizerRequestRequestTypeDef",
-    "GetAuthorizersRequestGetAuthorizersPaginateTypeDef",
     "GetAuthorizersRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
-    "GetDeploymentResponseTypeDef",
-    "GetDeploymentsRequestGetDeploymentsPaginateTypeDef",
     "GetDeploymentsRequestRequestTypeDef",
     "GetDomainNameRequestRequestTypeDef",
-    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
     "GetDomainNamesRequestRequestTypeDef",
     "GetIntegrationRequestRequestTypeDef",
     "GetIntegrationResponseRequestRequestTypeDef",
-    "GetIntegrationResponseResponseTypeDef",
-    "GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
     "GetIntegrationResponsesRequestRequestTypeDef",
     "IntegrationResponseTypeDef",
-    "GetIntegrationsRequestGetIntegrationsPaginateTypeDef",
     "GetIntegrationsRequestRequestTypeDef",
     "GetModelRequestRequestTypeDef",
-    "GetModelResponseTypeDef",
     "GetModelTemplateRequestRequestTypeDef",
-    "GetModelTemplateResponseTypeDef",
-    "GetModelsRequestGetModelsPaginateTypeDef",
     "GetModelsRequestRequestTypeDef",
     "ModelTypeDef",
     "GetRouteRequestRequestTypeDef",
     "GetRouteResponseRequestRequestTypeDef",
-    "GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
     "GetRouteResponsesRequestRequestTypeDef",
-    "GetRoutesRequestGetRoutesPaginateTypeDef",
     "GetRoutesRequestRequestTypeDef",
     "GetStageRequestRequestTypeDef",
-    "GetStagesRequestGetStagesPaginateTypeDef",
     "GetStagesRequestRequestTypeDef",
     "GetTagsRequestRequestTypeDef",
-    "GetTagsResponseTypeDef",
     "GetVpcLinkRequestRequestTypeDef",
-    "GetVpcLinkResponseTypeDef",
     "GetVpcLinksRequestRequestTypeDef",
     "VpcLinkTypeDef",
     "ImportApiRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "ReimportApiRequestRequestTypeDef",
     "ResetAuthorizersCacheRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiMappingRequestRequestTypeDef",
-    "UpdateApiMappingResponseTypeDef",
     "UpdateDeploymentRequestRequestTypeDef",
-    "UpdateDeploymentResponseTypeDef",
     "UpdateIntegrationResponseRequestRequestTypeDef",
-    "UpdateIntegrationResponseResponseTypeDef",
     "UpdateModelRequestRequestTypeDef",
-    "UpdateModelResponseTypeDef",
     "UpdateVpcLinkRequestRequestTypeDef",
-    "UpdateVpcLinkResponseTypeDef",
-    "GetApiMappingsResponseTypeDef",
     "ApiTypeDef",
+    "AuthorizerTypeDef",
     "CreateApiRequestRequestTypeDef",
+    "UpdateApiRequestRequestTypeDef",
+    "CreateApiMappingResponseTypeDef",
     "CreateApiResponseTypeDef",
+    "CreateAuthorizerResponseTypeDef",
+    "CreateDeploymentResponseTypeDef",
+    "CreateIntegrationResponseResponseTypeDef",
+    "CreateModelResponseTypeDef",
+    "CreateVpcLinkResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportApiResponseTypeDef",
+    "GetApiMappingResponseTypeDef",
+    "GetApiMappingsResponseTypeDef",
     "GetApiResponseTypeDef",
+    "GetAuthorizerResponseTypeDef",
+    "GetDeploymentResponseTypeDef",
+    "GetIntegrationResponseResponseTypeDef",
+    "GetModelResponseTypeDef",
+    "GetModelTemplateResponseTypeDef",
+    "GetTagsResponseTypeDef",
+    "GetVpcLinkResponseTypeDef",
     "ImportApiResponseTypeDef",
     "ReimportApiResponseTypeDef",
-    "UpdateApiRequestRequestTypeDef",
+    "UpdateApiMappingResponseTypeDef",
     "UpdateApiResponseTypeDef",
-    "AuthorizerTypeDef",
+    "UpdateAuthorizerResponseTypeDef",
+    "UpdateDeploymentResponseTypeDef",
+    "UpdateIntegrationResponseResponseTypeDef",
+    "UpdateModelResponseTypeDef",
+    "UpdateVpcLinkResponseTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
-    "CreateAuthorizerResponseTypeDef",
-    "GetAuthorizerResponseTypeDef",
     "UpdateAuthorizerRequestRequestTypeDef",
-    "UpdateAuthorizerResponseTypeDef",
     "CreateDomainNameRequestRequestTypeDef",
     "UpdateDomainNameRequestRequestTypeDef",
     "CreateDomainNameResponseTypeDef",
     "DomainNameTypeDef",
     "GetDomainNameResponseTypeDef",
     "UpdateDomainNameResponseTypeDef",
     "CreateIntegrationRequestRequestTypeDef",
     "UpdateIntegrationRequestRequestTypeDef",
     "CreateIntegrationResultTypeDef",
     "GetIntegrationResultTypeDef",
     "IntegrationTypeDef",
     "UpdateIntegrationResultTypeDef",
     "CreateRouteRequestRequestTypeDef",
     "CreateRouteResponseRequestRequestTypeDef",
+    "UpdateRouteRequestRequestTypeDef",
+    "UpdateRouteResponseRequestRequestTypeDef",
     "CreateRouteResponseResponseTypeDef",
     "CreateRouteResultTypeDef",
     "GetRouteResponseResponseTypeDef",
     "GetRouteResultTypeDef",
     "RouteResponseTypeDef",
     "RouteTypeDef",
-    "UpdateRouteRequestRequestTypeDef",
-    "UpdateRouteResponseRequestRequestTypeDef",
     "UpdateRouteResponseResponseTypeDef",
     "UpdateRouteResultTypeDef",
     "CreateStageRequestRequestTypeDef",
+    "UpdateStageRequestRequestTypeDef",
     "CreateStageResponseTypeDef",
     "GetStageResponseTypeDef",
     "StageTypeDef",
-    "UpdateStageRequestRequestTypeDef",
     "UpdateStageResponseTypeDef",
     "GetDeploymentsResponseTypeDef",
+    "GetApisRequestGetApisPaginateTypeDef",
+    "GetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    "GetDeploymentsRequestGetDeploymentsPaginateTypeDef",
+    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
+    "GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
+    "GetIntegrationsRequestGetIntegrationsPaginateTypeDef",
+    "GetModelsRequestGetModelsPaginateTypeDef",
+    "GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
+    "GetRoutesRequestGetRoutesPaginateTypeDef",
+    "GetStagesRequestGetStagesPaginateTypeDef",
     "GetIntegrationResponsesResponseTypeDef",
     "GetModelsResponseTypeDef",
     "GetVpcLinksResponseTypeDef",
     "GetApisResponseTypeDef",
     "GetAuthorizersResponseTypeDef",
     "GetDomainNamesResponseTypeDef",
     "GetIntegrationsResponseTypeDef",
     "GetRouteResponsesResponseTypeDef",
     "GetRoutesResponseTypeDef",
     "GetStagesResponseTypeDef",
 )
 
+AccessLogSettingsOutputTypeDef = TypedDict(
+    "AccessLogSettingsOutputTypeDef",
+    {
+        "DestinationArn": str,
+        "Format": str,
+    },
+)
+
 AccessLogSettingsTypeDef = TypedDict(
     "AccessLogSettingsTypeDef",
     {
         "DestinationArn": str,
         "Format": str,
     },
     total=False,
 )
 
-_RequiredApiMappingTypeDef = TypedDict(
-    "_RequiredApiMappingTypeDef",
+ApiMappingTypeDef = TypedDict(
+    "ApiMappingTypeDef",
     {
         "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
         "Stage": str,
     },
 )
-_OptionalApiMappingTypeDef = TypedDict(
-    "_OptionalApiMappingTypeDef",
+
+CorsOutputTypeDef = TypedDict(
+    "CorsOutputTypeDef",
     {
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
+        "AllowCredentials": bool,
+        "AllowHeaders": List[str],
+        "AllowMethods": List[str],
+        "AllowOrigins": List[str],
+        "ExposeHeaders": List[str],
+        "MaxAge": int,
     },
-    total=False,
 )
 
-
-class ApiMappingTypeDef(_RequiredApiMappingTypeDef, _OptionalApiMappingTypeDef):
-    pass
-
+JWTConfigurationOutputTypeDef = TypedDict(
+    "JWTConfigurationOutputTypeDef",
+    {
+        "Audience": List[str],
+        "Issuer": str,
+    },
+)
 
 CorsTypeDef = TypedDict(
     "CorsTypeDef",
     {
         "AllowCredentials": bool,
         "AllowHeaders": Sequence[str],
         "AllowMethods": Sequence[str],
         "AllowOrigins": Sequence[str],
         "ExposeHeaders": Sequence[str],
         "MaxAge": int,
     },
     total=False,
 )
 
-JWTConfigurationTypeDef = TypedDict(
-    "JWTConfigurationTypeDef",
-    {
-        "Audience": Sequence[str],
-        "Issuer": str,
-    },
-    total=False,
-)
-
 _RequiredCreateApiMappingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApiMappingRequestRequestTypeDef",
     {
         "ApiId": str,
         "DomainName": str,
         "Stage": str,
     },
@@ -278,25 +292,34 @@
 
 class CreateApiMappingRequestRequestTypeDef(
     _RequiredCreateApiMappingRequestRequestTypeDef, _OptionalCreateApiMappingRequestRequestTypeDef
 ):
     pass
 
 
-CreateApiMappingResponseTypeDef = TypedDict(
-    "CreateApiMappingResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ApiId": str,
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
-        "Stage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
+JWTConfigurationTypeDef = TypedDict(
+    "JWTConfigurationTypeDef",
+    {
+        "Audience": Sequence[str],
+        "Issuer": str,
+    },
+    total=False,
+)
+
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalCreateDeploymentRequestRequestTypeDef = TypedDict(
@@ -311,27 +334,14 @@
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
 
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
-    {
-        "AutoDeployed": bool,
-        "CreatedDate": datetime,
-        "DeploymentId": str,
-        "DeploymentStatus": DeploymentStatusType,
-        "DeploymentStatusMessage": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DomainNameConfigurationTypeDef = TypedDict(
     "DomainNameConfigurationTypeDef",
     {
         "ApiGatewayDomainName": str,
         "CertificateArn": str,
         "CertificateName": str,
         "CertificateUploadDate": Union[datetime, str],
@@ -350,22 +360,37 @@
     {
         "TruststoreUri": str,
         "TruststoreVersion": str,
     },
     total=False,
 )
 
+DomainNameConfigurationOutputTypeDef = TypedDict(
+    "DomainNameConfigurationOutputTypeDef",
+    {
+        "ApiGatewayDomainName": str,
+        "CertificateArn": str,
+        "CertificateName": str,
+        "CertificateUploadDate": datetime,
+        "DomainNameStatus": DomainNameStatusType,
+        "DomainNameStatusMessage": str,
+        "EndpointType": EndpointTypeType,
+        "HostedZoneId": str,
+        "SecurityPolicy": SecurityPolicyType,
+        "OwnershipVerificationCertificateArn": str,
+    },
+)
+
 MutualTlsAuthenticationTypeDef = TypedDict(
     "MutualTlsAuthenticationTypeDef",
     {
         "TruststoreUri": str,
         "TruststoreVersion": str,
         "TruststoreWarnings": List[str],
     },
-    total=False,
 )
 
 TlsConfigInputTypeDef = TypedDict(
     "TlsConfigInputTypeDef",
     {
         "ServerNameToVerify": str,
     },
@@ -395,33 +420,19 @@
 class CreateIntegrationResponseRequestRequestTypeDef(
     _RequiredCreateIntegrationResponseRequestRequestTypeDef,
     _OptionalCreateIntegrationResponseRequestRequestTypeDef,
 ):
     pass
 
 
-CreateIntegrationResponseResponseTypeDef = TypedDict(
-    "CreateIntegrationResponseResponseTypeDef",
-    {
-        "ContentHandlingStrategy": ContentHandlingStrategyType,
-        "IntegrationResponseId": str,
-        "IntegrationResponseKey": str,
-        "ResponseParameters": Dict[str, str],
-        "ResponseTemplates": Dict[str, str],
-        "TemplateSelectionExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TlsConfigTypeDef = TypedDict(
     "TlsConfigTypeDef",
     {
         "ServerNameToVerify": str,
     },
-    total=False,
 )
 
 _RequiredCreateModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelRequestRequestTypeDef",
     {
         "ApiId": str,
         "Name": str,
@@ -440,46 +451,52 @@
 
 class CreateModelRequestRequestTypeDef(
     _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
 ):
     pass
 
 
-CreateModelResponseTypeDef = TypedDict(
-    "CreateModelResponseTypeDef",
+ParameterConstraintsTypeDef = TypedDict(
+    "ParameterConstraintsTypeDef",
     {
-        "ContentType": str,
-        "Description": str,
-        "ModelId": str,
-        "Name": str,
-        "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Required": bool,
     },
+    total=False,
 )
 
-ParameterConstraintsTypeDef = TypedDict(
-    "ParameterConstraintsTypeDef",
+ParameterConstraintsOutputTypeDef = TypedDict(
+    "ParameterConstraintsOutputTypeDef",
     {
         "Required": bool,
     },
-    total=False,
 )
 
 RouteSettingsTypeDef = TypedDict(
     "RouteSettingsTypeDef",
     {
         "DataTraceEnabled": bool,
         "DetailedMetricsEnabled": bool,
         "LoggingLevel": LoggingLevelType,
         "ThrottlingBurstLimit": int,
         "ThrottlingRateLimit": float,
     },
     total=False,
 )
 
+RouteSettingsOutputTypeDef = TypedDict(
+    "RouteSettingsOutputTypeDef",
+    {
+        "DataTraceEnabled": bool,
+        "DetailedMetricsEnabled": bool,
+        "LoggingLevel": LoggingLevelType,
+        "ThrottlingBurstLimit": int,
+        "ThrottlingRateLimit": float,
+    },
+)
+
 _RequiredCreateVpcLinkRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcLinkRequestRequestTypeDef",
     {
         "Name": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -495,30 +512,14 @@
 
 class CreateVpcLinkRequestRequestTypeDef(
     _RequiredCreateVpcLinkRequestRequestTypeDef, _OptionalCreateVpcLinkRequestRequestTypeDef
 ):
     pass
 
 
-CreateVpcLinkResponseTypeDef = TypedDict(
-    "CreateVpcLinkResponseTypeDef",
-    {
-        "CreatedDate": datetime,
-        "Name": str,
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-        "Tags": Dict[str, str],
-        "VpcLinkId": str,
-        "VpcLinkStatus": VpcLinkStatusType,
-        "VpcLinkStatusMessage": str,
-        "VpcLinkVersion": Literal["V2"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAccessLogSettingsRequestRequestTypeDef = TypedDict(
     "DeleteAccessLogSettingsRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
     },
 )
@@ -649,22 +650,14 @@
         "AutoDeployed": bool,
         "CreatedDate": datetime,
         "DeploymentId": str,
         "DeploymentStatus": DeploymentStatusType,
         "DeploymentStatusMessage": str,
         "Description": str,
     },
-    total=False,
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 _RequiredExportApiRequestRequestTypeDef = TypedDict(
     "_RequiredExportApiRequestRequestTypeDef",
     {
         "ApiId": str,
         "OutputType": JSONYAMLType,
@@ -684,41 +677,22 @@
 
 class ExportApiRequestRequestTypeDef(
     _RequiredExportApiRequestRequestTypeDef, _OptionalExportApiRequestRequestTypeDef
 ):
     pass
 
 
-ExportApiResponseTypeDef = TypedDict(
-    "ExportApiResponseTypeDef",
-    {
-        "body": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetApiMappingRequestRequestTypeDef = TypedDict(
     "GetApiMappingRequestRequestTypeDef",
     {
         "ApiMappingId": str,
         "DomainName": str,
     },
 )
 
-GetApiMappingResponseTypeDef = TypedDict(
-    "GetApiMappingResponseTypeDef",
-    {
-        "ApiId": str,
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
-        "Stage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetApiMappingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetApiMappingsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalGetApiMappingsRequestRequestTypeDef = TypedDict(
@@ -740,18 +714,20 @@
 GetApiRequestRequestTypeDef = TypedDict(
     "GetApiRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 
-GetApisRequestGetApisPaginateTypeDef = TypedDict(
-    "GetApisRequestGetApisPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetApisRequestRequestTypeDef = TypedDict(
     "GetApisRequestRequestTypeDef",
     {
@@ -765,36 +741,14 @@
     "GetAuthorizerRequestRequestTypeDef",
     {
         "ApiId": str,
         "AuthorizerId": str,
     },
 )
 
-_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
-    "_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
-    "_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetAuthorizersRequestGetAuthorizersPaginateTypeDef(
-    _RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-    _OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetAuthorizersRequestRequestTypeDef = TypedDict(
     "_RequiredGetAuthorizersRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetAuthorizersRequestRequestTypeDef = TypedDict(
@@ -817,49 +771,14 @@
     "GetDeploymentRequestRequestTypeDef",
     {
         "ApiId": str,
         "DeploymentId": str,
     },
 )
 
-GetDeploymentResponseTypeDef = TypedDict(
-    "GetDeploymentResponseTypeDef",
-    {
-        "AutoDeployed": bool,
-        "CreatedDate": datetime,
-        "DeploymentId": str,
-        "DeploymentStatus": DeploymentStatusType,
-        "DeploymentStatusMessage": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetDeploymentsRequestGetDeploymentsPaginateTypeDef(
-    _RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-    _OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeploymentsRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetDeploymentsRequestRequestTypeDef = TypedDict(
@@ -881,22 +800,14 @@
 GetDomainNameRequestRequestTypeDef = TypedDict(
     "GetDomainNameRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-GetDomainNamesRequestGetDomainNamesPaginateTypeDef = TypedDict(
-    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetDomainNamesRequestRequestTypeDef = TypedDict(
     "GetDomainNamesRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -915,50 +826,14 @@
     {
         "ApiId": str,
         "IntegrationId": str,
         "IntegrationResponseId": str,
     },
 )
 
-GetIntegrationResponseResponseTypeDef = TypedDict(
-    "GetIntegrationResponseResponseTypeDef",
-    {
-        "ContentHandlingStrategy": ContentHandlingStrategyType,
-        "IntegrationResponseId": str,
-        "IntegrationResponseKey": str,
-        "ResponseParameters": Dict[str, str],
-        "ResponseTemplates": Dict[str, str],
-        "TemplateSelectionExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
-    "_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
-    {
-        "ApiId": str,
-        "IntegrationId": str,
-    },
-)
-_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
-    "_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef(
-    _RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
-    _OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetIntegrationResponsesRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntegrationResponsesRequestRequestTypeDef",
     {
         "ApiId": str,
         "IntegrationId": str,
     },
 )
@@ -975,61 +850,26 @@
 class GetIntegrationResponsesRequestRequestTypeDef(
     _RequiredGetIntegrationResponsesRequestRequestTypeDef,
     _OptionalGetIntegrationResponsesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredIntegrationResponseTypeDef = TypedDict(
-    "_RequiredIntegrationResponseTypeDef",
-    {
-        "IntegrationResponseKey": str,
-    },
-)
-_OptionalIntegrationResponseTypeDef = TypedDict(
-    "_OptionalIntegrationResponseTypeDef",
+IntegrationResponseTypeDef = TypedDict(
+    "IntegrationResponseTypeDef",
     {
         "ContentHandlingStrategy": ContentHandlingStrategyType,
         "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
         "ResponseParameters": Dict[str, str],
         "ResponseTemplates": Dict[str, str],
         "TemplateSelectionExpression": str,
     },
-    total=False,
 )
 
-
-class IntegrationResponseTypeDef(
-    _RequiredIntegrationResponseTypeDef, _OptionalIntegrationResponseTypeDef
-):
-    pass
-
-
-_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
-    "_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
-    "_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetIntegrationsRequestGetIntegrationsPaginateTypeDef(
-    _RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
-    _OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetIntegrationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntegrationsRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetIntegrationsRequestRequestTypeDef = TypedDict(
@@ -1052,64 +892,22 @@
     "GetModelRequestRequestTypeDef",
     {
         "ApiId": str,
         "ModelId": str,
     },
 )
 
-GetModelResponseTypeDef = TypedDict(
-    "GetModelResponseTypeDef",
-    {
-        "ContentType": str,
-        "Description": str,
-        "ModelId": str,
-        "Name": str,
-        "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetModelTemplateRequestRequestTypeDef = TypedDict(
     "GetModelTemplateRequestRequestTypeDef",
     {
         "ApiId": str,
         "ModelId": str,
     },
 )
 
-GetModelTemplateResponseTypeDef = TypedDict(
-    "GetModelTemplateResponseTypeDef",
-    {
-        "Value": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
-    "_RequiredGetModelsRequestGetModelsPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
-    "_OptionalGetModelsRequestGetModelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetModelsRequestGetModelsPaginateTypeDef(
-    _RequiredGetModelsRequestGetModelsPaginateTypeDef,
-    _OptionalGetModelsRequestGetModelsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetModelsRequestRequestTypeDef = TypedDict(
     "_RequiredGetModelsRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetModelsRequestRequestTypeDef = TypedDict(
@@ -1124,36 +922,25 @@
 
 class GetModelsRequestRequestTypeDef(
     _RequiredGetModelsRequestRequestTypeDef, _OptionalGetModelsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredModelTypeDef = TypedDict(
-    "_RequiredModelTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalModelTypeDef = TypedDict(
-    "_OptionalModelTypeDef",
+ModelTypeDef = TypedDict(
+    "ModelTypeDef",
     {
         "ContentType": str,
         "Description": str,
         "ModelId": str,
+        "Name": str,
         "Schema": str,
     },
-    total=False,
 )
 
-
-class ModelTypeDef(_RequiredModelTypeDef, _OptionalModelTypeDef):
-    pass
-
-
 GetRouteRequestRequestTypeDef = TypedDict(
     "GetRouteRequestRequestTypeDef",
     {
         "ApiId": str,
         "RouteId": str,
     },
 )
@@ -1163,37 +950,14 @@
     {
         "ApiId": str,
         "RouteId": str,
         "RouteResponseId": str,
     },
 )
 
-_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
-    "_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
-    {
-        "ApiId": str,
-        "RouteId": str,
-    },
-)
-_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
-    "_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef(
-    _RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
-    _OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetRouteResponsesRequestRequestTypeDef = TypedDict(
     "_RequiredGetRouteResponsesRequestRequestTypeDef",
     {
         "ApiId": str,
         "RouteId": str,
     },
 )
@@ -1209,36 +973,14 @@
 
 class GetRouteResponsesRequestRequestTypeDef(
     _RequiredGetRouteResponsesRequestRequestTypeDef, _OptionalGetRouteResponsesRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
-    "_RequiredGetRoutesRequestGetRoutesPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
-    "_OptionalGetRoutesRequestGetRoutesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetRoutesRequestGetRoutesPaginateTypeDef(
-    _RequiredGetRoutesRequestGetRoutesPaginateTypeDef,
-    _OptionalGetRoutesRequestGetRoutesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredGetRoutesRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetRoutesRequestRequestTypeDef = TypedDict(
@@ -1261,36 +1003,14 @@
     "GetStageRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
     },
 )
 
-_RequiredGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
-    "_RequiredGetStagesRequestGetStagesPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
-    "_OptionalGetStagesRequestGetStagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetStagesRequestGetStagesPaginateTypeDef(
-    _RequiredGetStagesRequestGetStagesPaginateTypeDef,
-    _OptionalGetStagesRequestGetStagesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetStagesRequestRequestTypeDef = TypedDict(
     "_RequiredGetStagesRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetStagesRequestRequestTypeDef = TypedDict(
@@ -1312,80 +1032,45 @@
 GetTagsRequestRequestTypeDef = TypedDict(
     "GetTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetTagsResponseTypeDef = TypedDict(
-    "GetTagsResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetVpcLinkRequestRequestTypeDef = TypedDict(
     "GetVpcLinkRequestRequestTypeDef",
     {
         "VpcLinkId": str,
     },
 )
 
-GetVpcLinkResponseTypeDef = TypedDict(
-    "GetVpcLinkResponseTypeDef",
-    {
-        "CreatedDate": datetime,
-        "Name": str,
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-        "Tags": Dict[str, str],
-        "VpcLinkId": str,
-        "VpcLinkStatus": VpcLinkStatusType,
-        "VpcLinkStatusMessage": str,
-        "VpcLinkVersion": Literal["V2"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetVpcLinksRequestRequestTypeDef = TypedDict(
     "GetVpcLinksRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredVpcLinkTypeDef = TypedDict(
-    "_RequiredVpcLinkTypeDef",
+VpcLinkTypeDef = TypedDict(
+    "VpcLinkTypeDef",
     {
+        "CreatedDate": datetime,
         "Name": str,
         "SecurityGroupIds": List[str],
         "SubnetIds": List[str],
-        "VpcLinkId": str,
-    },
-)
-_OptionalVpcLinkTypeDef = TypedDict(
-    "_OptionalVpcLinkTypeDef",
-    {
-        "CreatedDate": datetime,
         "Tags": Dict[str, str],
+        "VpcLinkId": str,
         "VpcLinkStatus": VpcLinkStatusType,
         "VpcLinkStatusMessage": str,
         "VpcLinkVersion": Literal["V2"],
     },
-    total=False,
 )
 
-
-class VpcLinkTypeDef(_RequiredVpcLinkTypeDef, _OptionalVpcLinkTypeDef):
-    pass
-
-
 _RequiredImportApiRequestRequestTypeDef = TypedDict(
     "_RequiredImportApiRequestRequestTypeDef",
     {
         "Body": str,
     },
 )
 _OptionalImportApiRequestRequestTypeDef = TypedDict(
@@ -1400,24 +1085,14 @@
 
 class ImportApiRequestRequestTypeDef(
     _RequiredImportApiRequestRequestTypeDef, _OptionalImportApiRequestRequestTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 _RequiredReimportApiRequestRequestTypeDef = TypedDict(
     "_RequiredReimportApiRequestRequestTypeDef",
     {
         "ApiId": str,
         "Body": str,
     },
 )
@@ -1441,25 +1116,14 @@
     "ResetAuthorizersCacheRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalTagResourceRequestRequestTypeDef = TypedDict(
@@ -1505,25 +1169,14 @@
 
 class UpdateApiMappingRequestRequestTypeDef(
     _RequiredUpdateApiMappingRequestRequestTypeDef, _OptionalUpdateApiMappingRequestRequestTypeDef
 ):
     pass
 
 
-UpdateApiMappingResponseTypeDef = TypedDict(
-    "UpdateApiMappingResponseTypeDef",
-    {
-        "ApiId": str,
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
-        "Stage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDeploymentRequestRequestTypeDef",
     {
         "ApiId": str,
         "DeploymentId": str,
     },
 )
@@ -1538,27 +1191,14 @@
 
 class UpdateDeploymentRequestRequestTypeDef(
     _RequiredUpdateDeploymentRequestRequestTypeDef, _OptionalUpdateDeploymentRequestRequestTypeDef
 ):
     pass
 
 
-UpdateDeploymentResponseTypeDef = TypedDict(
-    "UpdateDeploymentResponseTypeDef",
-    {
-        "AutoDeployed": bool,
-        "CreatedDate": datetime,
-        "DeploymentId": str,
-        "DeploymentStatus": DeploymentStatusType,
-        "DeploymentStatusMessage": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateIntegrationResponseRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIntegrationResponseRequestRequestTypeDef",
     {
         "ApiId": str,
         "IntegrationId": str,
         "IntegrationResponseId": str,
     },
@@ -1579,27 +1219,14 @@
 class UpdateIntegrationResponseRequestRequestTypeDef(
     _RequiredUpdateIntegrationResponseRequestRequestTypeDef,
     _OptionalUpdateIntegrationResponseRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateIntegrationResponseResponseTypeDef = TypedDict(
-    "UpdateIntegrationResponseResponseTypeDef",
-    {
-        "ContentHandlingStrategy": ContentHandlingStrategyType,
-        "IntegrationResponseId": str,
-        "IntegrationResponseKey": str,
-        "ResponseParameters": Dict[str, str],
-        "ResponseTemplates": Dict[str, str],
-        "TemplateSelectionExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelRequestRequestTypeDef",
     {
         "ApiId": str,
         "ModelId": str,
     },
 )
@@ -1617,26 +1244,14 @@
 
 class UpdateModelRequestRequestTypeDef(
     _RequiredUpdateModelRequestRequestTypeDef, _OptionalUpdateModelRequestRequestTypeDef
 ):
     pass
 
 
-UpdateModelResponseTypeDef = TypedDict(
-    "UpdateModelResponseTypeDef",
-    {
-        "ContentType": str,
-        "Description": str,
-        "ModelId": str,
-        "Name": str,
-        "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateVpcLinkRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVpcLinkRequestRequestTypeDef",
     {
         "VpcLinkId": str,
     },
 )
 _OptionalUpdateVpcLinkRequestRequestTypeDef = TypedDict(
@@ -1650,277 +1265,519 @@
 
 class UpdateVpcLinkRequestRequestTypeDef(
     _RequiredUpdateVpcLinkRequestRequestTypeDef, _OptionalUpdateVpcLinkRequestRequestTypeDef
 ):
     pass
 
 
-UpdateVpcLinkResponseTypeDef = TypedDict(
-    "UpdateVpcLinkResponseTypeDef",
+ApiTypeDef = TypedDict(
+    "ApiTypeDef",
     {
+        "ApiEndpoint": str,
+        "ApiGatewayManaged": bool,
+        "ApiId": str,
+        "ApiKeySelectionExpression": str,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
+        "Description": str,
+        "DisableSchemaValidation": bool,
+        "DisableExecuteApiEndpoint": bool,
+        "ImportInfo": List[str],
         "Name": str,
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
+        "ProtocolType": ProtocolTypeType,
+        "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
-        "VpcLinkId": str,
-        "VpcLinkStatus": VpcLinkStatusType,
-        "VpcLinkStatusMessage": str,
-        "VpcLinkVersion": Literal["V2"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Version": str,
+        "Warnings": List[str],
     },
 )
 
-GetApiMappingsResponseTypeDef = TypedDict(
-    "GetApiMappingsResponseTypeDef",
+AuthorizerTypeDef = TypedDict(
+    "AuthorizerTypeDef",
     {
-        "Items": List[ApiMappingTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "Name": str,
     },
 )
 
-_RequiredApiTypeDef = TypedDict(
-    "_RequiredApiTypeDef",
+_RequiredCreateApiRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateApiRequestRequestTypeDef",
     {
         "Name": str,
         "ProtocolType": ProtocolTypeType,
-        "RouteSelectionExpression": str,
     },
 )
-_OptionalApiTypeDef = TypedDict(
-    "_OptionalApiTypeDef",
+_OptionalCreateApiRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateApiRequestRequestTypeDef",
     {
-        "ApiEndpoint": str,
-        "ApiGatewayManaged": bool,
-        "ApiId": str,
         "ApiKeySelectionExpression": str,
         "CorsConfiguration": CorsTypeDef,
-        "CreatedDate": datetime,
+        "CredentialsArn": str,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
-        "ImportInfo": List[str],
-        "Tags": Dict[str, str],
+        "RouteKey": str,
+        "RouteSelectionExpression": str,
+        "Tags": Mapping[str, str],
+        "Target": str,
         "Version": str,
-        "Warnings": List[str],
     },
     total=False,
 )
 
 
-class ApiTypeDef(_RequiredApiTypeDef, _OptionalApiTypeDef):
+class CreateApiRequestRequestTypeDef(
+    _RequiredCreateApiRequestRequestTypeDef, _OptionalCreateApiRequestRequestTypeDef
+):
     pass
 
 
-_RequiredCreateApiRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateApiRequestRequestTypeDef",
+_RequiredUpdateApiRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateApiRequestRequestTypeDef",
     {
-        "Name": str,
-        "ProtocolType": ProtocolTypeType,
+        "ApiId": str,
     },
 )
-_OptionalCreateApiRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateApiRequestRequestTypeDef",
+_OptionalUpdateApiRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateApiRequestRequestTypeDef",
     {
         "ApiKeySelectionExpression": str,
         "CorsConfiguration": CorsTypeDef,
         "CredentialsArn": str,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
+        "Name": str,
         "RouteKey": str,
         "RouteSelectionExpression": str,
-        "Tags": Mapping[str, str],
         "Target": str,
         "Version": str,
     },
     total=False,
 )
 
 
-class CreateApiRequestRequestTypeDef(
-    _RequiredCreateApiRequestRequestTypeDef, _OptionalCreateApiRequestRequestTypeDef
+class UpdateApiRequestRequestTypeDef(
+    _RequiredUpdateApiRequestRequestTypeDef, _OptionalUpdateApiRequestRequestTypeDef
 ):
     pass
 
 
+CreateApiMappingResponseTypeDef = TypedDict(
+    "CreateApiMappingResponseTypeDef",
+    {
+        "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
+        "Stage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateApiResponseTypeDef = TypedDict(
     "CreateApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAuthorizerResponseTypeDef = TypedDict(
+    "CreateAuthorizerResponseTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "AutoDeployed": bool,
+        "CreatedDate": datetime,
+        "DeploymentId": str,
+        "DeploymentStatus": DeploymentStatusType,
+        "DeploymentStatusMessage": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIntegrationResponseResponseTypeDef = TypedDict(
+    "CreateIntegrationResponseResponseTypeDef",
+    {
+        "ContentHandlingStrategy": ContentHandlingStrategyType,
+        "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
+        "ResponseParameters": Dict[str, str],
+        "ResponseTemplates": Dict[str, str],
+        "TemplateSelectionExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateModelResponseTypeDef = TypedDict(
+    "CreateModelResponseTypeDef",
+    {
+        "ContentType": str,
+        "Description": str,
+        "ModelId": str,
+        "Name": str,
+        "Schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVpcLinkResponseTypeDef = TypedDict(
+    "CreateVpcLinkResponseTypeDef",
+    {
+        "CreatedDate": datetime,
+        "Name": str,
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "Tags": Dict[str, str],
+        "VpcLinkId": str,
+        "VpcLinkStatus": VpcLinkStatusType,
+        "VpcLinkStatusMessage": str,
+        "VpcLinkVersion": Literal["V2"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportApiResponseTypeDef = TypedDict(
+    "ExportApiResponseTypeDef",
+    {
+        "body": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApiMappingResponseTypeDef = TypedDict(
+    "GetApiMappingResponseTypeDef",
+    {
+        "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
+        "Stage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApiMappingsResponseTypeDef = TypedDict(
+    "GetApiMappingsResponseTypeDef",
+    {
+        "Items": List[ApiMappingTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApiResponseTypeDef = TypedDict(
     "GetApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAuthorizerResponseTypeDef = TypedDict(
+    "GetAuthorizerResponseTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeploymentResponseTypeDef = TypedDict(
+    "GetDeploymentResponseTypeDef",
+    {
+        "AutoDeployed": bool,
+        "CreatedDate": datetime,
+        "DeploymentId": str,
+        "DeploymentStatus": DeploymentStatusType,
+        "DeploymentStatusMessage": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIntegrationResponseResponseTypeDef = TypedDict(
+    "GetIntegrationResponseResponseTypeDef",
+    {
+        "ContentHandlingStrategy": ContentHandlingStrategyType,
+        "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
+        "ResponseParameters": Dict[str, str],
+        "ResponseTemplates": Dict[str, str],
+        "TemplateSelectionExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetModelResponseTypeDef = TypedDict(
+    "GetModelResponseTypeDef",
+    {
+        "ContentType": str,
+        "Description": str,
+        "ModelId": str,
+        "Name": str,
+        "Schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetModelTemplateResponseTypeDef = TypedDict(
+    "GetModelTemplateResponseTypeDef",
+    {
+        "Value": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagsResponseTypeDef = TypedDict(
+    "GetTagsResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVpcLinkResponseTypeDef = TypedDict(
+    "GetVpcLinkResponseTypeDef",
+    {
+        "CreatedDate": datetime,
+        "Name": str,
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "Tags": Dict[str, str],
+        "VpcLinkId": str,
+        "VpcLinkStatus": VpcLinkStatusType,
+        "VpcLinkStatusMessage": str,
+        "VpcLinkVersion": Literal["V2"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportApiResponseTypeDef = TypedDict(
     "ImportApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReimportApiResponseTypeDef = TypedDict(
     "ReimportApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateApiRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateApiRequestRequestTypeDef",
+UpdateApiMappingResponseTypeDef = TypedDict(
+    "UpdateApiMappingResponseTypeDef",
     {
         "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
+        "Stage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateApiRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateApiRequestRequestTypeDef",
-    {
-        "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
-        "CredentialsArn": str,
-        "Description": str,
-        "DisableSchemaValidation": bool,
-        "DisableExecuteApiEndpoint": bool,
-        "Name": str,
-        "RouteKey": str,
-        "RouteSelectionExpression": str,
-        "Target": str,
-        "Version": str,
-    },
-    total=False,
-)
-
-
-class UpdateApiRequestRequestTypeDef(
-    _RequiredUpdateApiRequestRequestTypeDef, _OptionalUpdateApiRequestRequestTypeDef
-):
-    pass
-
 
 UpdateApiResponseTypeDef = TypedDict(
     "UpdateApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAuthorizerTypeDef = TypedDict(
-    "_RequiredAuthorizerTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalAuthorizerTypeDef = TypedDict(
-    "_OptionalAuthorizerTypeDef",
+UpdateAuthorizerResponseTypeDef = TypedDict(
+    "UpdateAuthorizerResponseTypeDef",
     {
         "AuthorizerCredentialsArn": str,
         "AuthorizerId": str,
         "AuthorizerPayloadFormatVersion": str,
         "AuthorizerResultTtlInSeconds": int,
         "AuthorizerType": AuthorizerTypeType,
         "AuthorizerUri": str,
         "EnableSimpleResponses": bool,
         "IdentitySource": List[str],
         "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+UpdateDeploymentResponseTypeDef = TypedDict(
+    "UpdateDeploymentResponseTypeDef",
+    {
+        "AutoDeployed": bool,
+        "CreatedDate": datetime,
+        "DeploymentId": str,
+        "DeploymentStatus": DeploymentStatusType,
+        "DeploymentStatusMessage": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class AuthorizerTypeDef(_RequiredAuthorizerTypeDef, _OptionalAuthorizerTypeDef):
-    pass
+UpdateIntegrationResponseResponseTypeDef = TypedDict(
+    "UpdateIntegrationResponseResponseTypeDef",
+    {
+        "ContentHandlingStrategy": ContentHandlingStrategyType,
+        "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
+        "ResponseParameters": Dict[str, str],
+        "ResponseTemplates": Dict[str, str],
+        "TemplateSelectionExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+UpdateModelResponseTypeDef = TypedDict(
+    "UpdateModelResponseTypeDef",
+    {
+        "ContentType": str,
+        "Description": str,
+        "ModelId": str,
+        "Name": str,
+        "Schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVpcLinkResponseTypeDef = TypedDict(
+    "UpdateVpcLinkResponseTypeDef",
+    {
+        "CreatedDate": datetime,
+        "Name": str,
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "Tags": Dict[str, str],
+        "VpcLinkId": str,
+        "VpcLinkStatus": VpcLinkStatusType,
+        "VpcLinkStatusMessage": str,
+        "VpcLinkVersion": Literal["V2"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAuthorizerRequestRequestTypeDef",
     {
         "ApiId": str,
         "AuthorizerType": AuthorizerTypeType,
         "IdentitySource": Sequence[str],
@@ -1944,50 +1801,14 @@
 
 class CreateAuthorizerRequestRequestTypeDef(
     _RequiredCreateAuthorizerRequestRequestTypeDef, _OptionalCreateAuthorizerRequestRequestTypeDef
 ):
     pass
 
 
-CreateAuthorizerResponseTypeDef = TypedDict(
-    "CreateAuthorizerResponseTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetAuthorizerResponseTypeDef = TypedDict(
-    "GetAuthorizerResponseTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAuthorizerRequestRequestTypeDef",
     {
         "ApiId": str,
         "AuthorizerId": str,
     },
 )
@@ -2011,32 +1832,14 @@
 
 class UpdateAuthorizerRequestRequestTypeDef(
     _RequiredUpdateAuthorizerRequestRequestTypeDef, _OptionalUpdateAuthorizerRequestRequestTypeDef
 ):
     pass
 
 
-UpdateAuthorizerResponseTypeDef = TypedDict(
-    "UpdateAuthorizerResponseTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateDomainNameRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainNameRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCreateDomainNameRequestRequestTypeDef = TypedDict(
@@ -2079,64 +1882,53 @@
 
 
 CreateDomainNameResponseTypeDef = TypedDict(
     "CreateDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDomainNameTypeDef = TypedDict(
-    "_RequiredDomainNameTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalDomainNameTypeDef = TypedDict(
-    "_OptionalDomainNameTypeDef",
+DomainNameTypeDef = TypedDict(
+    "DomainNameTypeDef",
     {
         "ApiMappingSelectionExpression": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "DomainName": str,
+        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-
-class DomainNameTypeDef(_RequiredDomainNameTypeDef, _OptionalDomainNameTypeDef):
-    pass
-
-
 GetDomainNameResponseTypeDef = TypedDict(
     "GetDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainNameResponseTypeDef = TypedDict(
     "UpdateDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIntegrationRequestRequestTypeDef",
     {
         "ApiId": str,
@@ -2230,15 +2022,15 @@
         "PayloadFormatVersion": str,
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntegrationResultTypeDef = TypedDict(
     "GetIntegrationResultTypeDef",
     {
         "ApiGatewayManaged": bool,
@@ -2257,15 +2049,15 @@
         "PayloadFormatVersion": str,
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IntegrationTypeDef = TypedDict(
     "IntegrationTypeDef",
     {
         "ApiGatewayManaged": bool,
@@ -2285,15 +2077,14 @@
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
     },
-    total=False,
 )
 
 UpdateIntegrationResultTypeDef = TypedDict(
     "UpdateIntegrationResultTypeDef",
     {
         "ApiGatewayManaged": bool,
         "ConnectionId": str,
@@ -2311,15 +2102,15 @@
         "PayloadFormatVersion": str,
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRouteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRouteRequestRequestTypeDef",
     {
         "ApiId": str,
@@ -2372,218 +2163,196 @@
 class CreateRouteResponseRequestRequestTypeDef(
     _RequiredCreateRouteResponseRequestRequestTypeDef,
     _OptionalCreateRouteResponseRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredUpdateRouteRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRouteRequestRequestTypeDef",
+    {
+        "ApiId": str,
+        "RouteId": str,
+    },
+)
+_OptionalUpdateRouteRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRouteRequestRequestTypeDef",
+    {
+        "ApiKeyRequired": bool,
+        "AuthorizationScopes": Sequence[str],
+        "AuthorizationType": AuthorizationTypeType,
+        "AuthorizerId": str,
+        "ModelSelectionExpression": str,
+        "OperationName": str,
+        "RequestModels": Mapping[str, str],
+        "RequestParameters": Mapping[str, ParameterConstraintsTypeDef],
+        "RouteKey": str,
+        "RouteResponseSelectionExpression": str,
+        "Target": str,
+    },
+    total=False,
+)
+
+
+class UpdateRouteRequestRequestTypeDef(
+    _RequiredUpdateRouteRequestRequestTypeDef, _OptionalUpdateRouteRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateRouteResponseRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRouteResponseRequestRequestTypeDef",
+    {
+        "ApiId": str,
+        "RouteId": str,
+        "RouteResponseId": str,
+    },
+)
+_OptionalUpdateRouteResponseRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRouteResponseRequestRequestTypeDef",
+    {
+        "ModelSelectionExpression": str,
+        "ResponseModels": Mapping[str, str],
+        "ResponseParameters": Mapping[str, ParameterConstraintsTypeDef],
+        "RouteResponseKey": str,
+    },
+    total=False,
+)
+
+
+class UpdateRouteResponseRequestRequestTypeDef(
+    _RequiredUpdateRouteResponseRequestRequestTypeDef,
+    _OptionalUpdateRouteResponseRequestRequestTypeDef,
+):
+    pass
+
+
 CreateRouteResponseResponseTypeDef = TypedDict(
     "CreateRouteResponseResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
-        "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
+        "ResponseParameters": Dict[str, ParameterConstraintsOutputTypeDef],
         "RouteResponseId": str,
         "RouteResponseKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRouteResultTypeDef = TypedDict(
     "CreateRouteResultTypeDef",
     {
         "ApiGatewayManaged": bool,
         "ApiKeyRequired": bool,
         "AuthorizationScopes": List[str],
         "AuthorizationType": AuthorizationTypeType,
         "AuthorizerId": str,
         "ModelSelectionExpression": str,
         "OperationName": str,
         "RequestModels": Dict[str, str],
-        "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
+        "RequestParameters": Dict[str, ParameterConstraintsOutputTypeDef],
         "RouteId": str,
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResponseResponseTypeDef = TypedDict(
     "GetRouteResponseResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
-        "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
+        "ResponseParameters": Dict[str, ParameterConstraintsOutputTypeDef],
         "RouteResponseId": str,
         "RouteResponseKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResultTypeDef = TypedDict(
     "GetRouteResultTypeDef",
     {
         "ApiGatewayManaged": bool,
         "ApiKeyRequired": bool,
         "AuthorizationScopes": List[str],
         "AuthorizationType": AuthorizationTypeType,
         "AuthorizerId": str,
         "ModelSelectionExpression": str,
         "OperationName": str,
         "RequestModels": Dict[str, str],
-        "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
+        "RequestParameters": Dict[str, ParameterConstraintsOutputTypeDef],
         "RouteId": str,
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRouteResponseTypeDef = TypedDict(
-    "_RequiredRouteResponseTypeDef",
-    {
-        "RouteResponseKey": str,
-    },
-)
-_OptionalRouteResponseTypeDef = TypedDict(
-    "_OptionalRouteResponseTypeDef",
+RouteResponseTypeDef = TypedDict(
+    "RouteResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
-        "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
+        "ResponseParameters": Dict[str, ParameterConstraintsOutputTypeDef],
         "RouteResponseId": str,
+        "RouteResponseKey": str,
     },
-    total=False,
 )
 
-
-class RouteResponseTypeDef(_RequiredRouteResponseTypeDef, _OptionalRouteResponseTypeDef):
-    pass
-
-
-_RequiredRouteTypeDef = TypedDict(
-    "_RequiredRouteTypeDef",
-    {
-        "RouteKey": str,
-    },
-)
-_OptionalRouteTypeDef = TypedDict(
-    "_OptionalRouteTypeDef",
+RouteTypeDef = TypedDict(
+    "RouteTypeDef",
     {
         "ApiGatewayManaged": bool,
         "ApiKeyRequired": bool,
         "AuthorizationScopes": List[str],
         "AuthorizationType": AuthorizationTypeType,
         "AuthorizerId": str,
         "ModelSelectionExpression": str,
         "OperationName": str,
         "RequestModels": Dict[str, str],
-        "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
+        "RequestParameters": Dict[str, ParameterConstraintsOutputTypeDef],
         "RouteId": str,
-        "RouteResponseSelectionExpression": str,
-        "Target": str,
-    },
-    total=False,
-)
-
-
-class RouteTypeDef(_RequiredRouteTypeDef, _OptionalRouteTypeDef):
-    pass
-
-
-_RequiredUpdateRouteRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRouteRequestRequestTypeDef",
-    {
-        "ApiId": str,
-        "RouteId": str,
-    },
-)
-_OptionalUpdateRouteRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRouteRequestRequestTypeDef",
-    {
-        "ApiKeyRequired": bool,
-        "AuthorizationScopes": Sequence[str],
-        "AuthorizationType": AuthorizationTypeType,
-        "AuthorizerId": str,
-        "ModelSelectionExpression": str,
-        "OperationName": str,
-        "RequestModels": Mapping[str, str],
-        "RequestParameters": Mapping[str, ParameterConstraintsTypeDef],
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
     },
-    total=False,
-)
-
-
-class UpdateRouteRequestRequestTypeDef(
-    _RequiredUpdateRouteRequestRequestTypeDef, _OptionalUpdateRouteRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateRouteResponseRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRouteResponseRequestRequestTypeDef",
-    {
-        "ApiId": str,
-        "RouteId": str,
-        "RouteResponseId": str,
-    },
-)
-_OptionalUpdateRouteResponseRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRouteResponseRequestRequestTypeDef",
-    {
-        "ModelSelectionExpression": str,
-        "ResponseModels": Mapping[str, str],
-        "ResponseParameters": Mapping[str, ParameterConstraintsTypeDef],
-        "RouteResponseKey": str,
-    },
-    total=False,
 )
 
-
-class UpdateRouteResponseRequestRequestTypeDef(
-    _RequiredUpdateRouteResponseRequestRequestTypeDef,
-    _OptionalUpdateRouteResponseRequestRequestTypeDef,
-):
-    pass
-
-
 UpdateRouteResponseResponseTypeDef = TypedDict(
     "UpdateRouteResponseResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
-        "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
+        "ResponseParameters": Dict[str, ParameterConstraintsOutputTypeDef],
         "RouteResponseId": str,
         "RouteResponseKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRouteResultTypeDef = TypedDict(
     "UpdateRouteResultTypeDef",
     {
         "ApiGatewayManaged": bool,
         "ApiKeyRequired": bool,
         "AuthorizationScopes": List[str],
         "AuthorizationType": AuthorizationTypeType,
         "AuthorizerId": str,
         "ModelSelectionExpression": str,
         "OperationName": str,
         "RequestModels": Dict[str, str],
-        "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
+        "RequestParameters": Dict[str, ParameterConstraintsOutputTypeDef],
         "RouteId": str,
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateStageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStageRequestRequestTypeDef",
     {
         "ApiId": str,
@@ -2609,228 +2378,411 @@
 
 class CreateStageRequestRequestTypeDef(
     _RequiredCreateStageRequestRequestTypeDef, _OptionalCreateStageRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredUpdateStageRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateStageRequestRequestTypeDef",
+    {
+        "ApiId": str,
+        "StageName": str,
+    },
+)
+_OptionalUpdateStageRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateStageRequestRequestTypeDef",
+    {
+        "AccessLogSettings": AccessLogSettingsTypeDef,
+        "AutoDeploy": bool,
+        "ClientCertificateId": str,
+        "DefaultRouteSettings": RouteSettingsTypeDef,
+        "DeploymentId": str,
+        "Description": str,
+        "RouteSettings": Mapping[str, RouteSettingsTypeDef],
+        "StageVariables": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class UpdateStageRequestRequestTypeDef(
+    _RequiredUpdateStageRequestRequestTypeDef, _OptionalUpdateStageRequestRequestTypeDef
+):
+    pass
+
+
 CreateStageResponseTypeDef = TypedDict(
     "CreateStageResponseTypeDef",
     {
-        "AccessLogSettings": AccessLogSettingsTypeDef,
+        "AccessLogSettings": AccessLogSettingsOutputTypeDef,
         "ApiGatewayManaged": bool,
         "AutoDeploy": bool,
         "ClientCertificateId": str,
         "CreatedDate": datetime,
-        "DefaultRouteSettings": RouteSettingsTypeDef,
+        "DefaultRouteSettings": RouteSettingsOutputTypeDef,
         "DeploymentId": str,
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
-        "RouteSettings": Dict[str, RouteSettingsTypeDef],
+        "RouteSettings": Dict[str, RouteSettingsOutputTypeDef],
         "StageName": str,
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStageResponseTypeDef = TypedDict(
     "GetStageResponseTypeDef",
     {
-        "AccessLogSettings": AccessLogSettingsTypeDef,
+        "AccessLogSettings": AccessLogSettingsOutputTypeDef,
         "ApiGatewayManaged": bool,
         "AutoDeploy": bool,
         "ClientCertificateId": str,
         "CreatedDate": datetime,
-        "DefaultRouteSettings": RouteSettingsTypeDef,
+        "DefaultRouteSettings": RouteSettingsOutputTypeDef,
         "DeploymentId": str,
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
-        "RouteSettings": Dict[str, RouteSettingsTypeDef],
+        "RouteSettings": Dict[str, RouteSettingsOutputTypeDef],
         "StageName": str,
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStageTypeDef = TypedDict(
-    "_RequiredStageTypeDef",
+StageTypeDef = TypedDict(
+    "StageTypeDef",
     {
+        "AccessLogSettings": AccessLogSettingsOutputTypeDef,
+        "ApiGatewayManaged": bool,
+        "AutoDeploy": bool,
+        "ClientCertificateId": str,
+        "CreatedDate": datetime,
+        "DefaultRouteSettings": RouteSettingsOutputTypeDef,
+        "DeploymentId": str,
+        "Description": str,
+        "LastDeploymentStatusMessage": str,
+        "LastUpdatedDate": datetime,
+        "RouteSettings": Dict[str, RouteSettingsOutputTypeDef],
         "StageName": str,
+        "StageVariables": Dict[str, str],
+        "Tags": Dict[str, str],
     },
 )
-_OptionalStageTypeDef = TypedDict(
-    "_OptionalStageTypeDef",
+
+UpdateStageResponseTypeDef = TypedDict(
+    "UpdateStageResponseTypeDef",
     {
-        "AccessLogSettings": AccessLogSettingsTypeDef,
+        "AccessLogSettings": AccessLogSettingsOutputTypeDef,
         "ApiGatewayManaged": bool,
         "AutoDeploy": bool,
         "ClientCertificateId": str,
         "CreatedDate": datetime,
-        "DefaultRouteSettings": RouteSettingsTypeDef,
+        "DefaultRouteSettings": RouteSettingsOutputTypeDef,
         "DeploymentId": str,
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
-        "RouteSettings": Dict[str, RouteSettingsTypeDef],
+        "RouteSettings": Dict[str, RouteSettingsOutputTypeDef],
+        "StageName": str,
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeploymentsResponseTypeDef = TypedDict(
+    "GetDeploymentsResponseTypeDef",
+    {
+        "Items": List[DeploymentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApisRequestGetApisPaginateTypeDef = TypedDict(
+    "GetApisRequestGetApisPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
+    "_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
+    "_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-class StageTypeDef(_RequiredStageTypeDef, _OptionalStageTypeDef):
+
+class GetAuthorizersRequestGetAuthorizersPaginateTypeDef(
+    _RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+    _OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+):
     pass
 
 
-_RequiredUpdateStageRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateStageRequestRequestTypeDef",
+_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
     {
         "ApiId": str,
-        "StageName": str,
     },
 )
-_OptionalUpdateStageRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateStageRequestRequestTypeDef",
+_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
     {
-        "AccessLogSettings": AccessLogSettingsTypeDef,
-        "AutoDeploy": bool,
-        "ClientCertificateId": str,
-        "DefaultRouteSettings": RouteSettingsTypeDef,
-        "DeploymentId": str,
-        "Description": str,
-        "RouteSettings": Mapping[str, RouteSettingsTypeDef],
-        "StageVariables": Mapping[str, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class UpdateStageRequestRequestTypeDef(
-    _RequiredUpdateStageRequestRequestTypeDef, _OptionalUpdateStageRequestRequestTypeDef
+class GetDeploymentsRequestGetDeploymentsPaginateTypeDef(
+    _RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+    _OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
 ):
     pass
 
 
-UpdateStageResponseTypeDef = TypedDict(
-    "UpdateStageResponseTypeDef",
+GetDomainNamesRequestGetDomainNamesPaginateTypeDef = TypedDict(
+    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
     {
-        "AccessLogSettings": AccessLogSettingsTypeDef,
-        "ApiGatewayManaged": bool,
-        "AutoDeploy": bool,
-        "ClientCertificateId": str,
-        "CreatedDate": datetime,
-        "DefaultRouteSettings": RouteSettingsTypeDef,
-        "DeploymentId": str,
-        "Description": str,
-        "LastDeploymentStatusMessage": str,
-        "LastUpdatedDate": datetime,
-        "RouteSettings": Dict[str, RouteSettingsTypeDef],
-        "StageName": str,
-        "StageVariables": Dict[str, str],
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-GetDeploymentsResponseTypeDef = TypedDict(
-    "GetDeploymentsResponseTypeDef",
+_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
+    "_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
     {
-        "Items": List[DeploymentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApiId": str,
+        "IntegrationId": str,
+    },
+)
+_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
+    "_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef(
+    _RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+    _OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
+    "_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
+    "_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetIntegrationsRequestGetIntegrationsPaginateTypeDef(
+    _RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+    _OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
+    "_RequiredGetModelsRequestGetModelsPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
+    "_OptionalGetModelsRequestGetModelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetModelsRequestGetModelsPaginateTypeDef(
+    _RequiredGetModelsRequestGetModelsPaginateTypeDef,
+    _OptionalGetModelsRequestGetModelsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
+    "_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
+    {
+        "ApiId": str,
+        "RouteId": str,
+    },
+)
+_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
+    "_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef(
+    _RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+    _OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
+    "_RequiredGetRoutesRequestGetRoutesPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
+    "_OptionalGetRoutesRequestGetRoutesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetRoutesRequestGetRoutesPaginateTypeDef(
+    _RequiredGetRoutesRequestGetRoutesPaginateTypeDef,
+    _OptionalGetRoutesRequestGetRoutesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
+    "_RequiredGetStagesRequestGetStagesPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
+    "_OptionalGetStagesRequestGetStagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetStagesRequestGetStagesPaginateTypeDef(
+    _RequiredGetStagesRequestGetStagesPaginateTypeDef,
+    _OptionalGetStagesRequestGetStagesPaginateTypeDef,
+):
+    pass
+
+
 GetIntegrationResponsesResponseTypeDef = TypedDict(
     "GetIntegrationResponsesResponseTypeDef",
     {
         "Items": List[IntegrationResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetModelsResponseTypeDef = TypedDict(
     "GetModelsResponseTypeDef",
     {
         "Items": List[ModelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVpcLinksResponseTypeDef = TypedDict(
     "GetVpcLinksResponseTypeDef",
     {
         "Items": List[VpcLinkTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApisResponseTypeDef = TypedDict(
     "GetApisResponseTypeDef",
     {
         "Items": List[ApiTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAuthorizersResponseTypeDef = TypedDict(
     "GetAuthorizersResponseTypeDef",
     {
         "Items": List[AuthorizerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainNamesResponseTypeDef = TypedDict(
     "GetDomainNamesResponseTypeDef",
     {
         "Items": List[DomainNameTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntegrationsResponseTypeDef = TypedDict(
     "GetIntegrationsResponseTypeDef",
     {
         "Items": List[IntegrationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResponsesResponseTypeDef = TypedDict(
     "GetRouteResponsesResponseTypeDef",
     {
         "Items": List[RouteResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoutesResponseTypeDef = TypedDict(
     "GetRoutesResponseTypeDef",
     {
         "Items": List[RouteTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStagesResponseTypeDef = TypedDict(
     "GetStagesResponseTypeDef",
     {
         "Items": List[StageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2/type_defs.pyi` & `mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for apigatewayv2 service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_apigatewayv2.type_defs import AccessLogSettingsTypeDef
+    from mypy_boto3_apigatewayv2.type_defs import AccessLogSettingsOutputTypeDef
 
-    data: AccessLogSettingsTypeDef = {...}
+    data: AccessLogSettingsOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -40,35 +40,37 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AccessLogSettingsOutputTypeDef",
     "AccessLogSettingsTypeDef",
     "ApiMappingTypeDef",
+    "CorsOutputTypeDef",
+    "JWTConfigurationOutputTypeDef",
     "CorsTypeDef",
-    "JWTConfigurationTypeDef",
     "CreateApiMappingRequestRequestTypeDef",
-    "CreateApiMappingResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "JWTConfigurationTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
-    "CreateDeploymentResponseTypeDef",
     "DomainNameConfigurationTypeDef",
     "MutualTlsAuthenticationInputTypeDef",
+    "DomainNameConfigurationOutputTypeDef",
     "MutualTlsAuthenticationTypeDef",
     "TlsConfigInputTypeDef",
     "CreateIntegrationResponseRequestRequestTypeDef",
-    "CreateIntegrationResponseResponseTypeDef",
     "TlsConfigTypeDef",
     "CreateModelRequestRequestTypeDef",
-    "CreateModelResponseTypeDef",
     "ParameterConstraintsTypeDef",
+    "ParameterConstraintsOutputTypeDef",
     "RouteSettingsTypeDef",
+    "RouteSettingsOutputTypeDef",
     "CreateVpcLinkRequestRequestTypeDef",
-    "CreateVpcLinkResponseTypeDef",
     "DeleteAccessLogSettingsRequestRequestTypeDef",
     "DeleteApiMappingRequestRequestTypeDef",
     "DeleteApiRequestRequestTypeDef",
     "DeleteAuthorizerRequestRequestTypeDef",
     "DeleteCorsConfigurationRequestRequestTypeDef",
     "DeleteDeploymentRequestRequestTypeDef",
     "DeleteDomainNameRequestRequestTypeDef",
@@ -78,188 +80,202 @@
     "DeleteRouteRequestParameterRequestRequestTypeDef",
     "DeleteRouteRequestRequestTypeDef",
     "DeleteRouteResponseRequestRequestTypeDef",
     "DeleteRouteSettingsRequestRequestTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DeleteVpcLinkRequestRequestTypeDef",
     "DeploymentTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportApiRequestRequestTypeDef",
-    "ExportApiResponseTypeDef",
     "GetApiMappingRequestRequestTypeDef",
-    "GetApiMappingResponseTypeDef",
     "GetApiMappingsRequestRequestTypeDef",
     "GetApiRequestRequestTypeDef",
-    "GetApisRequestGetApisPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetApisRequestRequestTypeDef",
     "GetAuthorizerRequestRequestTypeDef",
-    "GetAuthorizersRequestGetAuthorizersPaginateTypeDef",
     "GetAuthorizersRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
-    "GetDeploymentResponseTypeDef",
-    "GetDeploymentsRequestGetDeploymentsPaginateTypeDef",
     "GetDeploymentsRequestRequestTypeDef",
     "GetDomainNameRequestRequestTypeDef",
-    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
     "GetDomainNamesRequestRequestTypeDef",
     "GetIntegrationRequestRequestTypeDef",
     "GetIntegrationResponseRequestRequestTypeDef",
-    "GetIntegrationResponseResponseTypeDef",
-    "GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
     "GetIntegrationResponsesRequestRequestTypeDef",
     "IntegrationResponseTypeDef",
-    "GetIntegrationsRequestGetIntegrationsPaginateTypeDef",
     "GetIntegrationsRequestRequestTypeDef",
     "GetModelRequestRequestTypeDef",
-    "GetModelResponseTypeDef",
     "GetModelTemplateRequestRequestTypeDef",
-    "GetModelTemplateResponseTypeDef",
-    "GetModelsRequestGetModelsPaginateTypeDef",
     "GetModelsRequestRequestTypeDef",
     "ModelTypeDef",
     "GetRouteRequestRequestTypeDef",
     "GetRouteResponseRequestRequestTypeDef",
-    "GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
     "GetRouteResponsesRequestRequestTypeDef",
-    "GetRoutesRequestGetRoutesPaginateTypeDef",
     "GetRoutesRequestRequestTypeDef",
     "GetStageRequestRequestTypeDef",
-    "GetStagesRequestGetStagesPaginateTypeDef",
     "GetStagesRequestRequestTypeDef",
     "GetTagsRequestRequestTypeDef",
-    "GetTagsResponseTypeDef",
     "GetVpcLinkRequestRequestTypeDef",
-    "GetVpcLinkResponseTypeDef",
     "GetVpcLinksRequestRequestTypeDef",
     "VpcLinkTypeDef",
     "ImportApiRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "ReimportApiRequestRequestTypeDef",
     "ResetAuthorizersCacheRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiMappingRequestRequestTypeDef",
-    "UpdateApiMappingResponseTypeDef",
     "UpdateDeploymentRequestRequestTypeDef",
-    "UpdateDeploymentResponseTypeDef",
     "UpdateIntegrationResponseRequestRequestTypeDef",
-    "UpdateIntegrationResponseResponseTypeDef",
     "UpdateModelRequestRequestTypeDef",
-    "UpdateModelResponseTypeDef",
     "UpdateVpcLinkRequestRequestTypeDef",
-    "UpdateVpcLinkResponseTypeDef",
-    "GetApiMappingsResponseTypeDef",
     "ApiTypeDef",
+    "AuthorizerTypeDef",
     "CreateApiRequestRequestTypeDef",
+    "UpdateApiRequestRequestTypeDef",
+    "CreateApiMappingResponseTypeDef",
     "CreateApiResponseTypeDef",
+    "CreateAuthorizerResponseTypeDef",
+    "CreateDeploymentResponseTypeDef",
+    "CreateIntegrationResponseResponseTypeDef",
+    "CreateModelResponseTypeDef",
+    "CreateVpcLinkResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportApiResponseTypeDef",
+    "GetApiMappingResponseTypeDef",
+    "GetApiMappingsResponseTypeDef",
     "GetApiResponseTypeDef",
+    "GetAuthorizerResponseTypeDef",
+    "GetDeploymentResponseTypeDef",
+    "GetIntegrationResponseResponseTypeDef",
+    "GetModelResponseTypeDef",
+    "GetModelTemplateResponseTypeDef",
+    "GetTagsResponseTypeDef",
+    "GetVpcLinkResponseTypeDef",
     "ImportApiResponseTypeDef",
     "ReimportApiResponseTypeDef",
-    "UpdateApiRequestRequestTypeDef",
+    "UpdateApiMappingResponseTypeDef",
     "UpdateApiResponseTypeDef",
-    "AuthorizerTypeDef",
+    "UpdateAuthorizerResponseTypeDef",
+    "UpdateDeploymentResponseTypeDef",
+    "UpdateIntegrationResponseResponseTypeDef",
+    "UpdateModelResponseTypeDef",
+    "UpdateVpcLinkResponseTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
-    "CreateAuthorizerResponseTypeDef",
-    "GetAuthorizerResponseTypeDef",
     "UpdateAuthorizerRequestRequestTypeDef",
-    "UpdateAuthorizerResponseTypeDef",
     "CreateDomainNameRequestRequestTypeDef",
     "UpdateDomainNameRequestRequestTypeDef",
     "CreateDomainNameResponseTypeDef",
     "DomainNameTypeDef",
     "GetDomainNameResponseTypeDef",
     "UpdateDomainNameResponseTypeDef",
     "CreateIntegrationRequestRequestTypeDef",
     "UpdateIntegrationRequestRequestTypeDef",
     "CreateIntegrationResultTypeDef",
     "GetIntegrationResultTypeDef",
     "IntegrationTypeDef",
     "UpdateIntegrationResultTypeDef",
     "CreateRouteRequestRequestTypeDef",
     "CreateRouteResponseRequestRequestTypeDef",
+    "UpdateRouteRequestRequestTypeDef",
+    "UpdateRouteResponseRequestRequestTypeDef",
     "CreateRouteResponseResponseTypeDef",
     "CreateRouteResultTypeDef",
     "GetRouteResponseResponseTypeDef",
     "GetRouteResultTypeDef",
     "RouteResponseTypeDef",
     "RouteTypeDef",
-    "UpdateRouteRequestRequestTypeDef",
-    "UpdateRouteResponseRequestRequestTypeDef",
     "UpdateRouteResponseResponseTypeDef",
     "UpdateRouteResultTypeDef",
     "CreateStageRequestRequestTypeDef",
+    "UpdateStageRequestRequestTypeDef",
     "CreateStageResponseTypeDef",
     "GetStageResponseTypeDef",
     "StageTypeDef",
-    "UpdateStageRequestRequestTypeDef",
     "UpdateStageResponseTypeDef",
     "GetDeploymentsResponseTypeDef",
+    "GetApisRequestGetApisPaginateTypeDef",
+    "GetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    "GetDeploymentsRequestGetDeploymentsPaginateTypeDef",
+    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
+    "GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
+    "GetIntegrationsRequestGetIntegrationsPaginateTypeDef",
+    "GetModelsRequestGetModelsPaginateTypeDef",
+    "GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
+    "GetRoutesRequestGetRoutesPaginateTypeDef",
+    "GetStagesRequestGetStagesPaginateTypeDef",
     "GetIntegrationResponsesResponseTypeDef",
     "GetModelsResponseTypeDef",
     "GetVpcLinksResponseTypeDef",
     "GetApisResponseTypeDef",
     "GetAuthorizersResponseTypeDef",
     "GetDomainNamesResponseTypeDef",
     "GetIntegrationsResponseTypeDef",
     "GetRouteResponsesResponseTypeDef",
     "GetRoutesResponseTypeDef",
     "GetStagesResponseTypeDef",
 )
 
+AccessLogSettingsOutputTypeDef = TypedDict(
+    "AccessLogSettingsOutputTypeDef",
+    {
+        "DestinationArn": str,
+        "Format": str,
+    },
+)
+
 AccessLogSettingsTypeDef = TypedDict(
     "AccessLogSettingsTypeDef",
     {
         "DestinationArn": str,
         "Format": str,
     },
     total=False,
 )
 
-_RequiredApiMappingTypeDef = TypedDict(
-    "_RequiredApiMappingTypeDef",
+ApiMappingTypeDef = TypedDict(
+    "ApiMappingTypeDef",
     {
         "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
         "Stage": str,
     },
 )
-_OptionalApiMappingTypeDef = TypedDict(
-    "_OptionalApiMappingTypeDef",
+
+CorsOutputTypeDef = TypedDict(
+    "CorsOutputTypeDef",
     {
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
+        "AllowCredentials": bool,
+        "AllowHeaders": List[str],
+        "AllowMethods": List[str],
+        "AllowOrigins": List[str],
+        "ExposeHeaders": List[str],
+        "MaxAge": int,
     },
-    total=False,
 )
 
-class ApiMappingTypeDef(_RequiredApiMappingTypeDef, _OptionalApiMappingTypeDef):
-    pass
+JWTConfigurationOutputTypeDef = TypedDict(
+    "JWTConfigurationOutputTypeDef",
+    {
+        "Audience": List[str],
+        "Issuer": str,
+    },
+)
 
 CorsTypeDef = TypedDict(
     "CorsTypeDef",
     {
         "AllowCredentials": bool,
         "AllowHeaders": Sequence[str],
         "AllowMethods": Sequence[str],
         "AllowOrigins": Sequence[str],
         "ExposeHeaders": Sequence[str],
         "MaxAge": int,
     },
     total=False,
 )
 
-JWTConfigurationTypeDef = TypedDict(
-    "JWTConfigurationTypeDef",
-    {
-        "Audience": Sequence[str],
-        "Issuer": str,
-    },
-    total=False,
-)
-
 _RequiredCreateApiMappingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApiMappingRequestRequestTypeDef",
     {
         "ApiId": str,
         "DomainName": str,
         "Stage": str,
     },
@@ -273,23 +289,32 @@
 )
 
 class CreateApiMappingRequestRequestTypeDef(
     _RequiredCreateApiMappingRequestRequestTypeDef, _OptionalCreateApiMappingRequestRequestTypeDef
 ):
     pass
 
-CreateApiMappingResponseTypeDef = TypedDict(
-    "CreateApiMappingResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ApiId": str,
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
-        "Stage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+JWTConfigurationTypeDef = TypedDict(
+    "JWTConfigurationTypeDef",
+    {
+        "Audience": Sequence[str],
+        "Issuer": str,
     },
+    total=False,
 )
 
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "ApiId": str,
     },
@@ -304,27 +329,14 @@
 )
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
-    {
-        "AutoDeployed": bool,
-        "CreatedDate": datetime,
-        "DeploymentId": str,
-        "DeploymentStatus": DeploymentStatusType,
-        "DeploymentStatusMessage": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DomainNameConfigurationTypeDef = TypedDict(
     "DomainNameConfigurationTypeDef",
     {
         "ApiGatewayDomainName": str,
         "CertificateArn": str,
         "CertificateName": str,
         "CertificateUploadDate": Union[datetime, str],
@@ -343,22 +355,37 @@
     {
         "TruststoreUri": str,
         "TruststoreVersion": str,
     },
     total=False,
 )
 
+DomainNameConfigurationOutputTypeDef = TypedDict(
+    "DomainNameConfigurationOutputTypeDef",
+    {
+        "ApiGatewayDomainName": str,
+        "CertificateArn": str,
+        "CertificateName": str,
+        "CertificateUploadDate": datetime,
+        "DomainNameStatus": DomainNameStatusType,
+        "DomainNameStatusMessage": str,
+        "EndpointType": EndpointTypeType,
+        "HostedZoneId": str,
+        "SecurityPolicy": SecurityPolicyType,
+        "OwnershipVerificationCertificateArn": str,
+    },
+)
+
 MutualTlsAuthenticationTypeDef = TypedDict(
     "MutualTlsAuthenticationTypeDef",
     {
         "TruststoreUri": str,
         "TruststoreVersion": str,
         "TruststoreWarnings": List[str],
     },
-    total=False,
 )
 
 TlsConfigInputTypeDef = TypedDict(
     "TlsConfigInputTypeDef",
     {
         "ServerNameToVerify": str,
     },
@@ -386,33 +413,19 @@
 
 class CreateIntegrationResponseRequestRequestTypeDef(
     _RequiredCreateIntegrationResponseRequestRequestTypeDef,
     _OptionalCreateIntegrationResponseRequestRequestTypeDef,
 ):
     pass
 
-CreateIntegrationResponseResponseTypeDef = TypedDict(
-    "CreateIntegrationResponseResponseTypeDef",
-    {
-        "ContentHandlingStrategy": ContentHandlingStrategyType,
-        "IntegrationResponseId": str,
-        "IntegrationResponseKey": str,
-        "ResponseParameters": Dict[str, str],
-        "ResponseTemplates": Dict[str, str],
-        "TemplateSelectionExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TlsConfigTypeDef = TypedDict(
     "TlsConfigTypeDef",
     {
         "ServerNameToVerify": str,
     },
-    total=False,
 )
 
 _RequiredCreateModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelRequestRequestTypeDef",
     {
         "ApiId": str,
         "Name": str,
@@ -429,46 +442,52 @@
 )
 
 class CreateModelRequestRequestTypeDef(
     _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
 ):
     pass
 
-CreateModelResponseTypeDef = TypedDict(
-    "CreateModelResponseTypeDef",
+ParameterConstraintsTypeDef = TypedDict(
+    "ParameterConstraintsTypeDef",
     {
-        "ContentType": str,
-        "Description": str,
-        "ModelId": str,
-        "Name": str,
-        "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Required": bool,
     },
+    total=False,
 )
 
-ParameterConstraintsTypeDef = TypedDict(
-    "ParameterConstraintsTypeDef",
+ParameterConstraintsOutputTypeDef = TypedDict(
+    "ParameterConstraintsOutputTypeDef",
     {
         "Required": bool,
     },
-    total=False,
 )
 
 RouteSettingsTypeDef = TypedDict(
     "RouteSettingsTypeDef",
     {
         "DataTraceEnabled": bool,
         "DetailedMetricsEnabled": bool,
         "LoggingLevel": LoggingLevelType,
         "ThrottlingBurstLimit": int,
         "ThrottlingRateLimit": float,
     },
     total=False,
 )
 
+RouteSettingsOutputTypeDef = TypedDict(
+    "RouteSettingsOutputTypeDef",
+    {
+        "DataTraceEnabled": bool,
+        "DetailedMetricsEnabled": bool,
+        "LoggingLevel": LoggingLevelType,
+        "ThrottlingBurstLimit": int,
+        "ThrottlingRateLimit": float,
+    },
+)
+
 _RequiredCreateVpcLinkRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcLinkRequestRequestTypeDef",
     {
         "Name": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -482,30 +501,14 @@
 )
 
 class CreateVpcLinkRequestRequestTypeDef(
     _RequiredCreateVpcLinkRequestRequestTypeDef, _OptionalCreateVpcLinkRequestRequestTypeDef
 ):
     pass
 
-CreateVpcLinkResponseTypeDef = TypedDict(
-    "CreateVpcLinkResponseTypeDef",
-    {
-        "CreatedDate": datetime,
-        "Name": str,
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-        "Tags": Dict[str, str],
-        "VpcLinkId": str,
-        "VpcLinkStatus": VpcLinkStatusType,
-        "VpcLinkStatusMessage": str,
-        "VpcLinkVersion": Literal["V2"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAccessLogSettingsRequestRequestTypeDef = TypedDict(
     "DeleteAccessLogSettingsRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
     },
 )
@@ -636,22 +639,14 @@
         "AutoDeployed": bool,
         "CreatedDate": datetime,
         "DeploymentId": str,
         "DeploymentStatus": DeploymentStatusType,
         "DeploymentStatusMessage": str,
         "Description": str,
     },
-    total=False,
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 _RequiredExportApiRequestRequestTypeDef = TypedDict(
     "_RequiredExportApiRequestRequestTypeDef",
     {
         "ApiId": str,
         "OutputType": JSONYAMLType,
@@ -669,41 +664,22 @@
 )
 
 class ExportApiRequestRequestTypeDef(
     _RequiredExportApiRequestRequestTypeDef, _OptionalExportApiRequestRequestTypeDef
 ):
     pass
 
-ExportApiResponseTypeDef = TypedDict(
-    "ExportApiResponseTypeDef",
-    {
-        "body": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetApiMappingRequestRequestTypeDef = TypedDict(
     "GetApiMappingRequestRequestTypeDef",
     {
         "ApiMappingId": str,
         "DomainName": str,
     },
 )
 
-GetApiMappingResponseTypeDef = TypedDict(
-    "GetApiMappingResponseTypeDef",
-    {
-        "ApiId": str,
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
-        "Stage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetApiMappingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetApiMappingsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalGetApiMappingsRequestRequestTypeDef = TypedDict(
@@ -723,18 +699,20 @@
 GetApiRequestRequestTypeDef = TypedDict(
     "GetApiRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 
-GetApisRequestGetApisPaginateTypeDef = TypedDict(
-    "GetApisRequestGetApisPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetApisRequestRequestTypeDef = TypedDict(
     "GetApisRequestRequestTypeDef",
     {
@@ -748,34 +726,14 @@
     "GetAuthorizerRequestRequestTypeDef",
     {
         "ApiId": str,
         "AuthorizerId": str,
     },
 )
 
-_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
-    "_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
-    "_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetAuthorizersRequestGetAuthorizersPaginateTypeDef(
-    _RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-    _OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-):
-    pass
-
 _RequiredGetAuthorizersRequestRequestTypeDef = TypedDict(
     "_RequiredGetAuthorizersRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetAuthorizersRequestRequestTypeDef = TypedDict(
@@ -796,47 +754,14 @@
     "GetDeploymentRequestRequestTypeDef",
     {
         "ApiId": str,
         "DeploymentId": str,
     },
 )
 
-GetDeploymentResponseTypeDef = TypedDict(
-    "GetDeploymentResponseTypeDef",
-    {
-        "AutoDeployed": bool,
-        "CreatedDate": datetime,
-        "DeploymentId": str,
-        "DeploymentStatus": DeploymentStatusType,
-        "DeploymentStatusMessage": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetDeploymentsRequestGetDeploymentsPaginateTypeDef(
-    _RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-    _OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeploymentsRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetDeploymentsRequestRequestTypeDef = TypedDict(
@@ -856,22 +781,14 @@
 GetDomainNameRequestRequestTypeDef = TypedDict(
     "GetDomainNameRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-GetDomainNamesRequestGetDomainNamesPaginateTypeDef = TypedDict(
-    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetDomainNamesRequestRequestTypeDef = TypedDict(
     "GetDomainNamesRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -890,48 +807,14 @@
     {
         "ApiId": str,
         "IntegrationId": str,
         "IntegrationResponseId": str,
     },
 )
 
-GetIntegrationResponseResponseTypeDef = TypedDict(
-    "GetIntegrationResponseResponseTypeDef",
-    {
-        "ContentHandlingStrategy": ContentHandlingStrategyType,
-        "IntegrationResponseId": str,
-        "IntegrationResponseKey": str,
-        "ResponseParameters": Dict[str, str],
-        "ResponseTemplates": Dict[str, str],
-        "TemplateSelectionExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
-    "_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
-    {
-        "ApiId": str,
-        "IntegrationId": str,
-    },
-)
-_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
-    "_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef(
-    _RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
-    _OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetIntegrationResponsesRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntegrationResponsesRequestRequestTypeDef",
     {
         "ApiId": str,
         "IntegrationId": str,
     },
 )
@@ -946,57 +829,26 @@
 
 class GetIntegrationResponsesRequestRequestTypeDef(
     _RequiredGetIntegrationResponsesRequestRequestTypeDef,
     _OptionalGetIntegrationResponsesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredIntegrationResponseTypeDef = TypedDict(
-    "_RequiredIntegrationResponseTypeDef",
-    {
-        "IntegrationResponseKey": str,
-    },
-)
-_OptionalIntegrationResponseTypeDef = TypedDict(
-    "_OptionalIntegrationResponseTypeDef",
+IntegrationResponseTypeDef = TypedDict(
+    "IntegrationResponseTypeDef",
     {
         "ContentHandlingStrategy": ContentHandlingStrategyType,
         "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
         "ResponseParameters": Dict[str, str],
         "ResponseTemplates": Dict[str, str],
         "TemplateSelectionExpression": str,
     },
-    total=False,
 )
 
-class IntegrationResponseTypeDef(
-    _RequiredIntegrationResponseTypeDef, _OptionalIntegrationResponseTypeDef
-):
-    pass
-
-_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
-    "_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
-    "_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetIntegrationsRequestGetIntegrationsPaginateTypeDef(
-    _RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
-    _OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetIntegrationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntegrationsRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetIntegrationsRequestRequestTypeDef = TypedDict(
@@ -1017,62 +869,22 @@
     "GetModelRequestRequestTypeDef",
     {
         "ApiId": str,
         "ModelId": str,
     },
 )
 
-GetModelResponseTypeDef = TypedDict(
-    "GetModelResponseTypeDef",
-    {
-        "ContentType": str,
-        "Description": str,
-        "ModelId": str,
-        "Name": str,
-        "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetModelTemplateRequestRequestTypeDef = TypedDict(
     "GetModelTemplateRequestRequestTypeDef",
     {
         "ApiId": str,
         "ModelId": str,
     },
 )
 
-GetModelTemplateResponseTypeDef = TypedDict(
-    "GetModelTemplateResponseTypeDef",
-    {
-        "Value": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
-    "_RequiredGetModelsRequestGetModelsPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
-    "_OptionalGetModelsRequestGetModelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetModelsRequestGetModelsPaginateTypeDef(
-    _RequiredGetModelsRequestGetModelsPaginateTypeDef,
-    _OptionalGetModelsRequestGetModelsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetModelsRequestRequestTypeDef = TypedDict(
     "_RequiredGetModelsRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetModelsRequestRequestTypeDef = TypedDict(
@@ -1085,34 +897,25 @@
 )
 
 class GetModelsRequestRequestTypeDef(
     _RequiredGetModelsRequestRequestTypeDef, _OptionalGetModelsRequestRequestTypeDef
 ):
     pass
 
-_RequiredModelTypeDef = TypedDict(
-    "_RequiredModelTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalModelTypeDef = TypedDict(
-    "_OptionalModelTypeDef",
+ModelTypeDef = TypedDict(
+    "ModelTypeDef",
     {
         "ContentType": str,
         "Description": str,
         "ModelId": str,
+        "Name": str,
         "Schema": str,
     },
-    total=False,
 )
 
-class ModelTypeDef(_RequiredModelTypeDef, _OptionalModelTypeDef):
-    pass
-
 GetRouteRequestRequestTypeDef = TypedDict(
     "GetRouteRequestRequestTypeDef",
     {
         "ApiId": str,
         "RouteId": str,
     },
 )
@@ -1122,35 +925,14 @@
     {
         "ApiId": str,
         "RouteId": str,
         "RouteResponseId": str,
     },
 )
 
-_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
-    "_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
-    {
-        "ApiId": str,
-        "RouteId": str,
-    },
-)
-_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
-    "_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef(
-    _RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
-    _OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetRouteResponsesRequestRequestTypeDef = TypedDict(
     "_RequiredGetRouteResponsesRequestRequestTypeDef",
     {
         "ApiId": str,
         "RouteId": str,
     },
 )
@@ -1164,34 +946,14 @@
 )
 
 class GetRouteResponsesRequestRequestTypeDef(
     _RequiredGetRouteResponsesRequestRequestTypeDef, _OptionalGetRouteResponsesRequestRequestTypeDef
 ):
     pass
 
-_RequiredGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
-    "_RequiredGetRoutesRequestGetRoutesPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
-    "_OptionalGetRoutesRequestGetRoutesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetRoutesRequestGetRoutesPaginateTypeDef(
-    _RequiredGetRoutesRequestGetRoutesPaginateTypeDef,
-    _OptionalGetRoutesRequestGetRoutesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredGetRoutesRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetRoutesRequestRequestTypeDef = TypedDict(
@@ -1212,34 +974,14 @@
     "GetStageRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
     },
 )
 
-_RequiredGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
-    "_RequiredGetStagesRequestGetStagesPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
-    "_OptionalGetStagesRequestGetStagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetStagesRequestGetStagesPaginateTypeDef(
-    _RequiredGetStagesRequestGetStagesPaginateTypeDef,
-    _OptionalGetStagesRequestGetStagesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetStagesRequestRequestTypeDef = TypedDict(
     "_RequiredGetStagesRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetStagesRequestRequestTypeDef = TypedDict(
@@ -1259,78 +1001,45 @@
 GetTagsRequestRequestTypeDef = TypedDict(
     "GetTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetTagsResponseTypeDef = TypedDict(
-    "GetTagsResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetVpcLinkRequestRequestTypeDef = TypedDict(
     "GetVpcLinkRequestRequestTypeDef",
     {
         "VpcLinkId": str,
     },
 )
 
-GetVpcLinkResponseTypeDef = TypedDict(
-    "GetVpcLinkResponseTypeDef",
-    {
-        "CreatedDate": datetime,
-        "Name": str,
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-        "Tags": Dict[str, str],
-        "VpcLinkId": str,
-        "VpcLinkStatus": VpcLinkStatusType,
-        "VpcLinkStatusMessage": str,
-        "VpcLinkVersion": Literal["V2"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetVpcLinksRequestRequestTypeDef = TypedDict(
     "GetVpcLinksRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredVpcLinkTypeDef = TypedDict(
-    "_RequiredVpcLinkTypeDef",
+VpcLinkTypeDef = TypedDict(
+    "VpcLinkTypeDef",
     {
+        "CreatedDate": datetime,
         "Name": str,
         "SecurityGroupIds": List[str],
         "SubnetIds": List[str],
-        "VpcLinkId": str,
-    },
-)
-_OptionalVpcLinkTypeDef = TypedDict(
-    "_OptionalVpcLinkTypeDef",
-    {
-        "CreatedDate": datetime,
         "Tags": Dict[str, str],
+        "VpcLinkId": str,
         "VpcLinkStatus": VpcLinkStatusType,
         "VpcLinkStatusMessage": str,
         "VpcLinkVersion": Literal["V2"],
     },
-    total=False,
 )
 
-class VpcLinkTypeDef(_RequiredVpcLinkTypeDef, _OptionalVpcLinkTypeDef):
-    pass
-
 _RequiredImportApiRequestRequestTypeDef = TypedDict(
     "_RequiredImportApiRequestRequestTypeDef",
     {
         "Body": str,
     },
 )
 _OptionalImportApiRequestRequestTypeDef = TypedDict(
@@ -1343,24 +1052,14 @@
 )
 
 class ImportApiRequestRequestTypeDef(
     _RequiredImportApiRequestRequestTypeDef, _OptionalImportApiRequestRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 _RequiredReimportApiRequestRequestTypeDef = TypedDict(
     "_RequiredReimportApiRequestRequestTypeDef",
     {
         "ApiId": str,
         "Body": str,
     },
 )
@@ -1382,25 +1081,14 @@
     "ResetAuthorizersCacheRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalTagResourceRequestRequestTypeDef = TypedDict(
@@ -1442,25 +1130,14 @@
 )
 
 class UpdateApiMappingRequestRequestTypeDef(
     _RequiredUpdateApiMappingRequestRequestTypeDef, _OptionalUpdateApiMappingRequestRequestTypeDef
 ):
     pass
 
-UpdateApiMappingResponseTypeDef = TypedDict(
-    "UpdateApiMappingResponseTypeDef",
-    {
-        "ApiId": str,
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
-        "Stage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDeploymentRequestRequestTypeDef",
     {
         "ApiId": str,
         "DeploymentId": str,
     },
 )
@@ -1473,27 +1150,14 @@
 )
 
 class UpdateDeploymentRequestRequestTypeDef(
     _RequiredUpdateDeploymentRequestRequestTypeDef, _OptionalUpdateDeploymentRequestRequestTypeDef
 ):
     pass
 
-UpdateDeploymentResponseTypeDef = TypedDict(
-    "UpdateDeploymentResponseTypeDef",
-    {
-        "AutoDeployed": bool,
-        "CreatedDate": datetime,
-        "DeploymentId": str,
-        "DeploymentStatus": DeploymentStatusType,
-        "DeploymentStatusMessage": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateIntegrationResponseRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIntegrationResponseRequestRequestTypeDef",
     {
         "ApiId": str,
         "IntegrationId": str,
         "IntegrationResponseId": str,
     },
@@ -1512,27 +1176,14 @@
 
 class UpdateIntegrationResponseRequestRequestTypeDef(
     _RequiredUpdateIntegrationResponseRequestRequestTypeDef,
     _OptionalUpdateIntegrationResponseRequestRequestTypeDef,
 ):
     pass
 
-UpdateIntegrationResponseResponseTypeDef = TypedDict(
-    "UpdateIntegrationResponseResponseTypeDef",
-    {
-        "ContentHandlingStrategy": ContentHandlingStrategyType,
-        "IntegrationResponseId": str,
-        "IntegrationResponseKey": str,
-        "ResponseParameters": Dict[str, str],
-        "ResponseTemplates": Dict[str, str],
-        "TemplateSelectionExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelRequestRequestTypeDef",
     {
         "ApiId": str,
         "ModelId": str,
     },
 )
@@ -1548,26 +1199,14 @@
 )
 
 class UpdateModelRequestRequestTypeDef(
     _RequiredUpdateModelRequestRequestTypeDef, _OptionalUpdateModelRequestRequestTypeDef
 ):
     pass
 
-UpdateModelResponseTypeDef = TypedDict(
-    "UpdateModelResponseTypeDef",
-    {
-        "ContentType": str,
-        "Description": str,
-        "ModelId": str,
-        "Name": str,
-        "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateVpcLinkRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVpcLinkRequestRequestTypeDef",
     {
         "VpcLinkId": str,
     },
 )
 _OptionalUpdateVpcLinkRequestRequestTypeDef = TypedDict(
@@ -1579,269 +1218,515 @@
 )
 
 class UpdateVpcLinkRequestRequestTypeDef(
     _RequiredUpdateVpcLinkRequestRequestTypeDef, _OptionalUpdateVpcLinkRequestRequestTypeDef
 ):
     pass
 
-UpdateVpcLinkResponseTypeDef = TypedDict(
-    "UpdateVpcLinkResponseTypeDef",
+ApiTypeDef = TypedDict(
+    "ApiTypeDef",
     {
+        "ApiEndpoint": str,
+        "ApiGatewayManaged": bool,
+        "ApiId": str,
+        "ApiKeySelectionExpression": str,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
+        "Description": str,
+        "DisableSchemaValidation": bool,
+        "DisableExecuteApiEndpoint": bool,
+        "ImportInfo": List[str],
         "Name": str,
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
+        "ProtocolType": ProtocolTypeType,
+        "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
-        "VpcLinkId": str,
-        "VpcLinkStatus": VpcLinkStatusType,
-        "VpcLinkStatusMessage": str,
-        "VpcLinkVersion": Literal["V2"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Version": str,
+        "Warnings": List[str],
     },
 )
 
-GetApiMappingsResponseTypeDef = TypedDict(
-    "GetApiMappingsResponseTypeDef",
+AuthorizerTypeDef = TypedDict(
+    "AuthorizerTypeDef",
     {
-        "Items": List[ApiMappingTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "Name": str,
     },
 )
 
-_RequiredApiTypeDef = TypedDict(
-    "_RequiredApiTypeDef",
+_RequiredCreateApiRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateApiRequestRequestTypeDef",
     {
         "Name": str,
         "ProtocolType": ProtocolTypeType,
-        "RouteSelectionExpression": str,
     },
 )
-_OptionalApiTypeDef = TypedDict(
-    "_OptionalApiTypeDef",
+_OptionalCreateApiRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateApiRequestRequestTypeDef",
     {
-        "ApiEndpoint": str,
-        "ApiGatewayManaged": bool,
-        "ApiId": str,
         "ApiKeySelectionExpression": str,
         "CorsConfiguration": CorsTypeDef,
-        "CreatedDate": datetime,
+        "CredentialsArn": str,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
-        "ImportInfo": List[str],
-        "Tags": Dict[str, str],
+        "RouteKey": str,
+        "RouteSelectionExpression": str,
+        "Tags": Mapping[str, str],
+        "Target": str,
         "Version": str,
-        "Warnings": List[str],
     },
     total=False,
 )
 
-class ApiTypeDef(_RequiredApiTypeDef, _OptionalApiTypeDef):
+class CreateApiRequestRequestTypeDef(
+    _RequiredCreateApiRequestRequestTypeDef, _OptionalCreateApiRequestRequestTypeDef
+):
     pass
 
-_RequiredCreateApiRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateApiRequestRequestTypeDef",
+_RequiredUpdateApiRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateApiRequestRequestTypeDef",
     {
-        "Name": str,
-        "ProtocolType": ProtocolTypeType,
+        "ApiId": str,
     },
 )
-_OptionalCreateApiRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateApiRequestRequestTypeDef",
+_OptionalUpdateApiRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateApiRequestRequestTypeDef",
     {
         "ApiKeySelectionExpression": str,
         "CorsConfiguration": CorsTypeDef,
         "CredentialsArn": str,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
+        "Name": str,
         "RouteKey": str,
         "RouteSelectionExpression": str,
-        "Tags": Mapping[str, str],
         "Target": str,
         "Version": str,
     },
     total=False,
 )
 
-class CreateApiRequestRequestTypeDef(
-    _RequiredCreateApiRequestRequestTypeDef, _OptionalCreateApiRequestRequestTypeDef
+class UpdateApiRequestRequestTypeDef(
+    _RequiredUpdateApiRequestRequestTypeDef, _OptionalUpdateApiRequestRequestTypeDef
 ):
     pass
 
+CreateApiMappingResponseTypeDef = TypedDict(
+    "CreateApiMappingResponseTypeDef",
+    {
+        "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
+        "Stage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateApiResponseTypeDef = TypedDict(
     "CreateApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAuthorizerResponseTypeDef = TypedDict(
+    "CreateAuthorizerResponseTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "AutoDeployed": bool,
+        "CreatedDate": datetime,
+        "DeploymentId": str,
+        "DeploymentStatus": DeploymentStatusType,
+        "DeploymentStatusMessage": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIntegrationResponseResponseTypeDef = TypedDict(
+    "CreateIntegrationResponseResponseTypeDef",
+    {
+        "ContentHandlingStrategy": ContentHandlingStrategyType,
+        "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
+        "ResponseParameters": Dict[str, str],
+        "ResponseTemplates": Dict[str, str],
+        "TemplateSelectionExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateModelResponseTypeDef = TypedDict(
+    "CreateModelResponseTypeDef",
+    {
+        "ContentType": str,
+        "Description": str,
+        "ModelId": str,
+        "Name": str,
+        "Schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVpcLinkResponseTypeDef = TypedDict(
+    "CreateVpcLinkResponseTypeDef",
+    {
+        "CreatedDate": datetime,
+        "Name": str,
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "Tags": Dict[str, str],
+        "VpcLinkId": str,
+        "VpcLinkStatus": VpcLinkStatusType,
+        "VpcLinkStatusMessage": str,
+        "VpcLinkVersion": Literal["V2"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportApiResponseTypeDef = TypedDict(
+    "ExportApiResponseTypeDef",
+    {
+        "body": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApiMappingResponseTypeDef = TypedDict(
+    "GetApiMappingResponseTypeDef",
+    {
+        "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
+        "Stage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApiMappingsResponseTypeDef = TypedDict(
+    "GetApiMappingsResponseTypeDef",
+    {
+        "Items": List[ApiMappingTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApiResponseTypeDef = TypedDict(
     "GetApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAuthorizerResponseTypeDef = TypedDict(
+    "GetAuthorizerResponseTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeploymentResponseTypeDef = TypedDict(
+    "GetDeploymentResponseTypeDef",
+    {
+        "AutoDeployed": bool,
+        "CreatedDate": datetime,
+        "DeploymentId": str,
+        "DeploymentStatus": DeploymentStatusType,
+        "DeploymentStatusMessage": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIntegrationResponseResponseTypeDef = TypedDict(
+    "GetIntegrationResponseResponseTypeDef",
+    {
+        "ContentHandlingStrategy": ContentHandlingStrategyType,
+        "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
+        "ResponseParameters": Dict[str, str],
+        "ResponseTemplates": Dict[str, str],
+        "TemplateSelectionExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetModelResponseTypeDef = TypedDict(
+    "GetModelResponseTypeDef",
+    {
+        "ContentType": str,
+        "Description": str,
+        "ModelId": str,
+        "Name": str,
+        "Schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetModelTemplateResponseTypeDef = TypedDict(
+    "GetModelTemplateResponseTypeDef",
+    {
+        "Value": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagsResponseTypeDef = TypedDict(
+    "GetTagsResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVpcLinkResponseTypeDef = TypedDict(
+    "GetVpcLinkResponseTypeDef",
+    {
+        "CreatedDate": datetime,
+        "Name": str,
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "Tags": Dict[str, str],
+        "VpcLinkId": str,
+        "VpcLinkStatus": VpcLinkStatusType,
+        "VpcLinkStatusMessage": str,
+        "VpcLinkVersion": Literal["V2"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportApiResponseTypeDef = TypedDict(
     "ImportApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReimportApiResponseTypeDef = TypedDict(
     "ReimportApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateApiRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateApiRequestRequestTypeDef",
+UpdateApiMappingResponseTypeDef = TypedDict(
+    "UpdateApiMappingResponseTypeDef",
     {
         "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
+        "Stage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateApiRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateApiRequestRequestTypeDef",
-    {
-        "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
-        "CredentialsArn": str,
-        "Description": str,
-        "DisableSchemaValidation": bool,
-        "DisableExecuteApiEndpoint": bool,
-        "Name": str,
-        "RouteKey": str,
-        "RouteSelectionExpression": str,
-        "Target": str,
-        "Version": str,
-    },
-    total=False,
-)
-
-class UpdateApiRequestRequestTypeDef(
-    _RequiredUpdateApiRequestRequestTypeDef, _OptionalUpdateApiRequestRequestTypeDef
-):
-    pass
 
 UpdateApiResponseTypeDef = TypedDict(
     "UpdateApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAuthorizerTypeDef = TypedDict(
-    "_RequiredAuthorizerTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalAuthorizerTypeDef = TypedDict(
-    "_OptionalAuthorizerTypeDef",
+UpdateAuthorizerResponseTypeDef = TypedDict(
+    "UpdateAuthorizerResponseTypeDef",
     {
         "AuthorizerCredentialsArn": str,
         "AuthorizerId": str,
         "AuthorizerPayloadFormatVersion": str,
         "AuthorizerResultTtlInSeconds": int,
         "AuthorizerType": AuthorizerTypeType,
         "AuthorizerUri": str,
         "EnableSimpleResponses": bool,
         "IdentitySource": List[str],
         "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class AuthorizerTypeDef(_RequiredAuthorizerTypeDef, _OptionalAuthorizerTypeDef):
-    pass
+UpdateDeploymentResponseTypeDef = TypedDict(
+    "UpdateDeploymentResponseTypeDef",
+    {
+        "AutoDeployed": bool,
+        "CreatedDate": datetime,
+        "DeploymentId": str,
+        "DeploymentStatus": DeploymentStatusType,
+        "DeploymentStatusMessage": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateIntegrationResponseResponseTypeDef = TypedDict(
+    "UpdateIntegrationResponseResponseTypeDef",
+    {
+        "ContentHandlingStrategy": ContentHandlingStrategyType,
+        "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
+        "ResponseParameters": Dict[str, str],
+        "ResponseTemplates": Dict[str, str],
+        "TemplateSelectionExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateModelResponseTypeDef = TypedDict(
+    "UpdateModelResponseTypeDef",
+    {
+        "ContentType": str,
+        "Description": str,
+        "ModelId": str,
+        "Name": str,
+        "Schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVpcLinkResponseTypeDef = TypedDict(
+    "UpdateVpcLinkResponseTypeDef",
+    {
+        "CreatedDate": datetime,
+        "Name": str,
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "Tags": Dict[str, str],
+        "VpcLinkId": str,
+        "VpcLinkStatus": VpcLinkStatusType,
+        "VpcLinkStatusMessage": str,
+        "VpcLinkVersion": Literal["V2"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAuthorizerRequestRequestTypeDef",
     {
         "ApiId": str,
         "AuthorizerType": AuthorizerTypeType,
         "IdentitySource": Sequence[str],
@@ -1863,50 +1748,14 @@
 )
 
 class CreateAuthorizerRequestRequestTypeDef(
     _RequiredCreateAuthorizerRequestRequestTypeDef, _OptionalCreateAuthorizerRequestRequestTypeDef
 ):
     pass
 
-CreateAuthorizerResponseTypeDef = TypedDict(
-    "CreateAuthorizerResponseTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetAuthorizerResponseTypeDef = TypedDict(
-    "GetAuthorizerResponseTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAuthorizerRequestRequestTypeDef",
     {
         "ApiId": str,
         "AuthorizerId": str,
     },
 )
@@ -1928,32 +1777,14 @@
 )
 
 class UpdateAuthorizerRequestRequestTypeDef(
     _RequiredUpdateAuthorizerRequestRequestTypeDef, _OptionalUpdateAuthorizerRequestRequestTypeDef
 ):
     pass
 
-UpdateAuthorizerResponseTypeDef = TypedDict(
-    "UpdateAuthorizerResponseTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateDomainNameRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainNameRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCreateDomainNameRequestRequestTypeDef = TypedDict(
@@ -1992,62 +1823,53 @@
     pass
 
 CreateDomainNameResponseTypeDef = TypedDict(
     "CreateDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDomainNameTypeDef = TypedDict(
-    "_RequiredDomainNameTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalDomainNameTypeDef = TypedDict(
-    "_OptionalDomainNameTypeDef",
+DomainNameTypeDef = TypedDict(
+    "DomainNameTypeDef",
     {
         "ApiMappingSelectionExpression": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "DomainName": str,
+        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-class DomainNameTypeDef(_RequiredDomainNameTypeDef, _OptionalDomainNameTypeDef):
-    pass
-
 GetDomainNameResponseTypeDef = TypedDict(
     "GetDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainNameResponseTypeDef = TypedDict(
     "UpdateDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIntegrationRequestRequestTypeDef",
     {
         "ApiId": str,
@@ -2137,15 +1959,15 @@
         "PayloadFormatVersion": str,
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntegrationResultTypeDef = TypedDict(
     "GetIntegrationResultTypeDef",
     {
         "ApiGatewayManaged": bool,
@@ -2164,15 +1986,15 @@
         "PayloadFormatVersion": str,
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IntegrationTypeDef = TypedDict(
     "IntegrationTypeDef",
     {
         "ApiGatewayManaged": bool,
@@ -2192,15 +2014,14 @@
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
     },
-    total=False,
 )
 
 UpdateIntegrationResultTypeDef = TypedDict(
     "UpdateIntegrationResultTypeDef",
     {
         "ApiGatewayManaged": bool,
         "ConnectionId": str,
@@ -2218,15 +2039,15 @@
         "PayloadFormatVersion": str,
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRouteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRouteRequestRequestTypeDef",
     {
         "ApiId": str,
@@ -2275,210 +2096,192 @@
 
 class CreateRouteResponseRequestRequestTypeDef(
     _RequiredCreateRouteResponseRequestRequestTypeDef,
     _OptionalCreateRouteResponseRequestRequestTypeDef,
 ):
     pass
 
+_RequiredUpdateRouteRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRouteRequestRequestTypeDef",
+    {
+        "ApiId": str,
+        "RouteId": str,
+    },
+)
+_OptionalUpdateRouteRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRouteRequestRequestTypeDef",
+    {
+        "ApiKeyRequired": bool,
+        "AuthorizationScopes": Sequence[str],
+        "AuthorizationType": AuthorizationTypeType,
+        "AuthorizerId": str,
+        "ModelSelectionExpression": str,
+        "OperationName": str,
+        "RequestModels": Mapping[str, str],
+        "RequestParameters": Mapping[str, ParameterConstraintsTypeDef],
+        "RouteKey": str,
+        "RouteResponseSelectionExpression": str,
+        "Target": str,
+    },
+    total=False,
+)
+
+class UpdateRouteRequestRequestTypeDef(
+    _RequiredUpdateRouteRequestRequestTypeDef, _OptionalUpdateRouteRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateRouteResponseRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRouteResponseRequestRequestTypeDef",
+    {
+        "ApiId": str,
+        "RouteId": str,
+        "RouteResponseId": str,
+    },
+)
+_OptionalUpdateRouteResponseRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRouteResponseRequestRequestTypeDef",
+    {
+        "ModelSelectionExpression": str,
+        "ResponseModels": Mapping[str, str],
+        "ResponseParameters": Mapping[str, ParameterConstraintsTypeDef],
+        "RouteResponseKey": str,
+    },
+    total=False,
+)
+
+class UpdateRouteResponseRequestRequestTypeDef(
+    _RequiredUpdateRouteResponseRequestRequestTypeDef,
+    _OptionalUpdateRouteResponseRequestRequestTypeDef,
+):
+    pass
+
 CreateRouteResponseResponseTypeDef = TypedDict(
     "CreateRouteResponseResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
-        "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
+        "ResponseParameters": Dict[str, ParameterConstraintsOutputTypeDef],
         "RouteResponseId": str,
         "RouteResponseKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRouteResultTypeDef = TypedDict(
     "CreateRouteResultTypeDef",
     {
         "ApiGatewayManaged": bool,
         "ApiKeyRequired": bool,
         "AuthorizationScopes": List[str],
         "AuthorizationType": AuthorizationTypeType,
         "AuthorizerId": str,
         "ModelSelectionExpression": str,
         "OperationName": str,
         "RequestModels": Dict[str, str],
-        "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
+        "RequestParameters": Dict[str, ParameterConstraintsOutputTypeDef],
         "RouteId": str,
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResponseResponseTypeDef = TypedDict(
     "GetRouteResponseResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
-        "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
+        "ResponseParameters": Dict[str, ParameterConstraintsOutputTypeDef],
         "RouteResponseId": str,
         "RouteResponseKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResultTypeDef = TypedDict(
     "GetRouteResultTypeDef",
     {
         "ApiGatewayManaged": bool,
         "ApiKeyRequired": bool,
         "AuthorizationScopes": List[str],
         "AuthorizationType": AuthorizationTypeType,
         "AuthorizerId": str,
         "ModelSelectionExpression": str,
         "OperationName": str,
         "RequestModels": Dict[str, str],
-        "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
+        "RequestParameters": Dict[str, ParameterConstraintsOutputTypeDef],
         "RouteId": str,
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRouteResponseTypeDef = TypedDict(
-    "_RequiredRouteResponseTypeDef",
-    {
-        "RouteResponseKey": str,
-    },
-)
-_OptionalRouteResponseTypeDef = TypedDict(
-    "_OptionalRouteResponseTypeDef",
+RouteResponseTypeDef = TypedDict(
+    "RouteResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
-        "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
+        "ResponseParameters": Dict[str, ParameterConstraintsOutputTypeDef],
         "RouteResponseId": str,
+        "RouteResponseKey": str,
     },
-    total=False,
 )
 
-class RouteResponseTypeDef(_RequiredRouteResponseTypeDef, _OptionalRouteResponseTypeDef):
-    pass
-
-_RequiredRouteTypeDef = TypedDict(
-    "_RequiredRouteTypeDef",
-    {
-        "RouteKey": str,
-    },
-)
-_OptionalRouteTypeDef = TypedDict(
-    "_OptionalRouteTypeDef",
+RouteTypeDef = TypedDict(
+    "RouteTypeDef",
     {
         "ApiGatewayManaged": bool,
         "ApiKeyRequired": bool,
         "AuthorizationScopes": List[str],
         "AuthorizationType": AuthorizationTypeType,
         "AuthorizerId": str,
         "ModelSelectionExpression": str,
         "OperationName": str,
         "RequestModels": Dict[str, str],
-        "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
+        "RequestParameters": Dict[str, ParameterConstraintsOutputTypeDef],
         "RouteId": str,
-        "RouteResponseSelectionExpression": str,
-        "Target": str,
-    },
-    total=False,
-)
-
-class RouteTypeDef(_RequiredRouteTypeDef, _OptionalRouteTypeDef):
-    pass
-
-_RequiredUpdateRouteRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRouteRequestRequestTypeDef",
-    {
-        "ApiId": str,
-        "RouteId": str,
-    },
-)
-_OptionalUpdateRouteRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRouteRequestRequestTypeDef",
-    {
-        "ApiKeyRequired": bool,
-        "AuthorizationScopes": Sequence[str],
-        "AuthorizationType": AuthorizationTypeType,
-        "AuthorizerId": str,
-        "ModelSelectionExpression": str,
-        "OperationName": str,
-        "RequestModels": Mapping[str, str],
-        "RequestParameters": Mapping[str, ParameterConstraintsTypeDef],
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
     },
-    total=False,
 )
 
-class UpdateRouteRequestRequestTypeDef(
-    _RequiredUpdateRouteRequestRequestTypeDef, _OptionalUpdateRouteRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateRouteResponseRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRouteResponseRequestRequestTypeDef",
-    {
-        "ApiId": str,
-        "RouteId": str,
-        "RouteResponseId": str,
-    },
-)
-_OptionalUpdateRouteResponseRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRouteResponseRequestRequestTypeDef",
-    {
-        "ModelSelectionExpression": str,
-        "ResponseModels": Mapping[str, str],
-        "ResponseParameters": Mapping[str, ParameterConstraintsTypeDef],
-        "RouteResponseKey": str,
-    },
-    total=False,
-)
-
-class UpdateRouteResponseRequestRequestTypeDef(
-    _RequiredUpdateRouteResponseRequestRequestTypeDef,
-    _OptionalUpdateRouteResponseRequestRequestTypeDef,
-):
-    pass
-
 UpdateRouteResponseResponseTypeDef = TypedDict(
     "UpdateRouteResponseResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
-        "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
+        "ResponseParameters": Dict[str, ParameterConstraintsOutputTypeDef],
         "RouteResponseId": str,
         "RouteResponseKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRouteResultTypeDef = TypedDict(
     "UpdateRouteResultTypeDef",
     {
         "ApiGatewayManaged": bool,
         "ApiKeyRequired": bool,
         "AuthorizationScopes": List[str],
         "AuthorizationType": AuthorizationTypeType,
         "AuthorizerId": str,
         "ModelSelectionExpression": str,
         "OperationName": str,
         "RequestModels": Dict[str, str],
-        "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
+        "RequestParameters": Dict[str, ParameterConstraintsOutputTypeDef],
         "RouteId": str,
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateStageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStageRequestRequestTypeDef",
     {
         "ApiId": str,
@@ -2502,224 +2305,393 @@
 )
 
 class CreateStageRequestRequestTypeDef(
     _RequiredCreateStageRequestRequestTypeDef, _OptionalCreateStageRequestRequestTypeDef
 ):
     pass
 
+_RequiredUpdateStageRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateStageRequestRequestTypeDef",
+    {
+        "ApiId": str,
+        "StageName": str,
+    },
+)
+_OptionalUpdateStageRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateStageRequestRequestTypeDef",
+    {
+        "AccessLogSettings": AccessLogSettingsTypeDef,
+        "AutoDeploy": bool,
+        "ClientCertificateId": str,
+        "DefaultRouteSettings": RouteSettingsTypeDef,
+        "DeploymentId": str,
+        "Description": str,
+        "RouteSettings": Mapping[str, RouteSettingsTypeDef],
+        "StageVariables": Mapping[str, str],
+    },
+    total=False,
+)
+
+class UpdateStageRequestRequestTypeDef(
+    _RequiredUpdateStageRequestRequestTypeDef, _OptionalUpdateStageRequestRequestTypeDef
+):
+    pass
+
 CreateStageResponseTypeDef = TypedDict(
     "CreateStageResponseTypeDef",
     {
-        "AccessLogSettings": AccessLogSettingsTypeDef,
+        "AccessLogSettings": AccessLogSettingsOutputTypeDef,
         "ApiGatewayManaged": bool,
         "AutoDeploy": bool,
         "ClientCertificateId": str,
         "CreatedDate": datetime,
-        "DefaultRouteSettings": RouteSettingsTypeDef,
+        "DefaultRouteSettings": RouteSettingsOutputTypeDef,
         "DeploymentId": str,
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
-        "RouteSettings": Dict[str, RouteSettingsTypeDef],
+        "RouteSettings": Dict[str, RouteSettingsOutputTypeDef],
         "StageName": str,
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStageResponseTypeDef = TypedDict(
     "GetStageResponseTypeDef",
     {
-        "AccessLogSettings": AccessLogSettingsTypeDef,
+        "AccessLogSettings": AccessLogSettingsOutputTypeDef,
         "ApiGatewayManaged": bool,
         "AutoDeploy": bool,
         "ClientCertificateId": str,
         "CreatedDate": datetime,
-        "DefaultRouteSettings": RouteSettingsTypeDef,
+        "DefaultRouteSettings": RouteSettingsOutputTypeDef,
         "DeploymentId": str,
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
-        "RouteSettings": Dict[str, RouteSettingsTypeDef],
+        "RouteSettings": Dict[str, RouteSettingsOutputTypeDef],
         "StageName": str,
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStageTypeDef = TypedDict(
-    "_RequiredStageTypeDef",
+StageTypeDef = TypedDict(
+    "StageTypeDef",
     {
+        "AccessLogSettings": AccessLogSettingsOutputTypeDef,
+        "ApiGatewayManaged": bool,
+        "AutoDeploy": bool,
+        "ClientCertificateId": str,
+        "CreatedDate": datetime,
+        "DefaultRouteSettings": RouteSettingsOutputTypeDef,
+        "DeploymentId": str,
+        "Description": str,
+        "LastDeploymentStatusMessage": str,
+        "LastUpdatedDate": datetime,
+        "RouteSettings": Dict[str, RouteSettingsOutputTypeDef],
         "StageName": str,
+        "StageVariables": Dict[str, str],
+        "Tags": Dict[str, str],
     },
 )
-_OptionalStageTypeDef = TypedDict(
-    "_OptionalStageTypeDef",
+
+UpdateStageResponseTypeDef = TypedDict(
+    "UpdateStageResponseTypeDef",
     {
-        "AccessLogSettings": AccessLogSettingsTypeDef,
+        "AccessLogSettings": AccessLogSettingsOutputTypeDef,
         "ApiGatewayManaged": bool,
         "AutoDeploy": bool,
         "ClientCertificateId": str,
         "CreatedDate": datetime,
-        "DefaultRouteSettings": RouteSettingsTypeDef,
+        "DefaultRouteSettings": RouteSettingsOutputTypeDef,
         "DeploymentId": str,
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
-        "RouteSettings": Dict[str, RouteSettingsTypeDef],
+        "RouteSettings": Dict[str, RouteSettingsOutputTypeDef],
+        "StageName": str,
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeploymentsResponseTypeDef = TypedDict(
+    "GetDeploymentsResponseTypeDef",
+    {
+        "Items": List[DeploymentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApisRequestGetApisPaginateTypeDef = TypedDict(
+    "GetApisRequestGetApisPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
+    "_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
+    "_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class StageTypeDef(_RequiredStageTypeDef, _OptionalStageTypeDef):
+class GetAuthorizersRequestGetAuthorizersPaginateTypeDef(
+    _RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+    _OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+):
     pass
 
-_RequiredUpdateStageRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateStageRequestRequestTypeDef",
+_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
     {
         "ApiId": str,
-        "StageName": str,
     },
 )
-_OptionalUpdateStageRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateStageRequestRequestTypeDef",
+_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
     {
-        "AccessLogSettings": AccessLogSettingsTypeDef,
-        "AutoDeploy": bool,
-        "ClientCertificateId": str,
-        "DefaultRouteSettings": RouteSettingsTypeDef,
-        "DeploymentId": str,
-        "Description": str,
-        "RouteSettings": Mapping[str, RouteSettingsTypeDef],
-        "StageVariables": Mapping[str, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class UpdateStageRequestRequestTypeDef(
-    _RequiredUpdateStageRequestRequestTypeDef, _OptionalUpdateStageRequestRequestTypeDef
+class GetDeploymentsRequestGetDeploymentsPaginateTypeDef(
+    _RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+    _OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
 ):
     pass
 
-UpdateStageResponseTypeDef = TypedDict(
-    "UpdateStageResponseTypeDef",
+GetDomainNamesRequestGetDomainNamesPaginateTypeDef = TypedDict(
+    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
     {
-        "AccessLogSettings": AccessLogSettingsTypeDef,
-        "ApiGatewayManaged": bool,
-        "AutoDeploy": bool,
-        "ClientCertificateId": str,
-        "CreatedDate": datetime,
-        "DefaultRouteSettings": RouteSettingsTypeDef,
-        "DeploymentId": str,
-        "Description": str,
-        "LastDeploymentStatusMessage": str,
-        "LastUpdatedDate": datetime,
-        "RouteSettings": Dict[str, RouteSettingsTypeDef],
-        "StageName": str,
-        "StageVariables": Dict[str, str],
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-GetDeploymentsResponseTypeDef = TypedDict(
-    "GetDeploymentsResponseTypeDef",
+_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
+    "_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
     {
-        "Items": List[DeploymentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApiId": str,
+        "IntegrationId": str,
+    },
+)
+_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
+    "_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+class GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef(
+    _RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+    _OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+):
+    pass
+
+_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
+    "_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
+    "_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
+class GetIntegrationsRequestGetIntegrationsPaginateTypeDef(
+    _RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+    _OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
+    "_RequiredGetModelsRequestGetModelsPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
+    "_OptionalGetModelsRequestGetModelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetModelsRequestGetModelsPaginateTypeDef(
+    _RequiredGetModelsRequestGetModelsPaginateTypeDef,
+    _OptionalGetModelsRequestGetModelsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
+    "_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
+    {
+        "ApiId": str,
+        "RouteId": str,
+    },
+)
+_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
+    "_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef(
+    _RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+    _OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+):
+    pass
+
+_RequiredGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
+    "_RequiredGetRoutesRequestGetRoutesPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
+    "_OptionalGetRoutesRequestGetRoutesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetRoutesRequestGetRoutesPaginateTypeDef(
+    _RequiredGetRoutesRequestGetRoutesPaginateTypeDef,
+    _OptionalGetRoutesRequestGetRoutesPaginateTypeDef,
+):
+    pass
+
+_RequiredGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
+    "_RequiredGetStagesRequestGetStagesPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
+    "_OptionalGetStagesRequestGetStagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetStagesRequestGetStagesPaginateTypeDef(
+    _RequiredGetStagesRequestGetStagesPaginateTypeDef,
+    _OptionalGetStagesRequestGetStagesPaginateTypeDef,
+):
+    pass
+
 GetIntegrationResponsesResponseTypeDef = TypedDict(
     "GetIntegrationResponsesResponseTypeDef",
     {
         "Items": List[IntegrationResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetModelsResponseTypeDef = TypedDict(
     "GetModelsResponseTypeDef",
     {
         "Items": List[ModelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVpcLinksResponseTypeDef = TypedDict(
     "GetVpcLinksResponseTypeDef",
     {
         "Items": List[VpcLinkTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApisResponseTypeDef = TypedDict(
     "GetApisResponseTypeDef",
     {
         "Items": List[ApiTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAuthorizersResponseTypeDef = TypedDict(
     "GetAuthorizersResponseTypeDef",
     {
         "Items": List[AuthorizerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainNamesResponseTypeDef = TypedDict(
     "GetDomainNamesResponseTypeDef",
     {
         "Items": List[DomainNameTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntegrationsResponseTypeDef = TypedDict(
     "GetIntegrationsResponseTypeDef",
     {
         "Items": List[IntegrationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResponsesResponseTypeDef = TypedDict(
     "GetRouteResponsesResponseTypeDef",
     {
         "Items": List[RouteResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoutesResponseTypeDef = TypedDict(
     "GetRoutesResponseTypeDef",
     {
         "Items": List[RouteTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStagesResponseTypeDef = TypedDict(
     "GetStagesResponseTypeDef",
     {
         "Items": List[StageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2.egg-info/PKG-INFO` & `mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigatewayv2
-Version: 1.28.0
-Summary: Type annotations for boto3.ApiGatewayV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.10
+Summary: Type annotations for boto3.ApiGatewayV2 1.28.10 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigatewayv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigatewayv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-apigatewayv2?color=blue)](https://pypistats.org/packages/mypy-boto3-apigatewayv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApiGatewayV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
+[boto3.ApiGatewayV2 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-apigatewayv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,35 +368,37 @@
 ### Typed dictionaries
 
 `mypy_boto3_apigatewayv2.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apigatewayv2.type_defs import (
+    AccessLogSettingsOutputTypeDef,
     AccessLogSettingsTypeDef,
     ApiMappingTypeDef,
+    CorsOutputTypeDef,
+    JWTConfigurationOutputTypeDef,
     CorsTypeDef,
-    JWTConfigurationTypeDef,
     CreateApiMappingRequestRequestTypeDef,
-    CreateApiMappingResponseTypeDef,
+    ResponseMetadataTypeDef,
+    JWTConfigurationTypeDef,
     CreateDeploymentRequestRequestTypeDef,
-    CreateDeploymentResponseTypeDef,
     DomainNameConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
+    DomainNameConfigurationOutputTypeDef,
     MutualTlsAuthenticationTypeDef,
     TlsConfigInputTypeDef,
     CreateIntegrationResponseRequestRequestTypeDef,
-    CreateIntegrationResponseResponseTypeDef,
     TlsConfigTypeDef,
     CreateModelRequestRequestTypeDef,
-    CreateModelResponseTypeDef,
     ParameterConstraintsTypeDef,
+    ParameterConstraintsOutputTypeDef,
     RouteSettingsTypeDef,
+    RouteSettingsOutputTypeDef,
     CreateVpcLinkRequestRequestTypeDef,
-    CreateVpcLinkResponseTypeDef,
     DeleteAccessLogSettingsRequestRequestTypeDef,
     DeleteApiMappingRequestRequestTypeDef,
     DeleteApiRequestRequestTypeDef,
     DeleteAuthorizerRequestRequestTypeDef,
     DeleteCorsConfigurationRequestRequestTypeDef,
     DeleteDeploymentRequestRequestTypeDef,
     DeleteDomainNameRequestRequestTypeDef,
@@ -406,140 +408,144 @@
     DeleteRouteRequestParameterRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
     DeleteRouteResponseRequestRequestTypeDef,
     DeleteRouteSettingsRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeleteVpcLinkRequestRequestTypeDef,
     DeploymentTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportApiRequestRequestTypeDef,
-    ExportApiResponseTypeDef,
     GetApiMappingRequestRequestTypeDef,
-    GetApiMappingResponseTypeDef,
     GetApiMappingsRequestRequestTypeDef,
     GetApiRequestRequestTypeDef,
-    GetApisRequestGetApisPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetApisRequestRequestTypeDef,
     GetAuthorizerRequestRequestTypeDef,
-    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
     GetAuthorizersRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
-    GetDeploymentResponseTypeDef,
-    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDomainNameRequestRequestTypeDef,
-    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
     GetDomainNamesRequestRequestTypeDef,
     GetIntegrationRequestRequestTypeDef,
     GetIntegrationResponseRequestRequestTypeDef,
-    GetIntegrationResponseResponseTypeDef,
-    GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
     GetIntegrationResponsesRequestRequestTypeDef,
     IntegrationResponseTypeDef,
-    GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
     GetIntegrationsRequestRequestTypeDef,
     GetModelRequestRequestTypeDef,
-    GetModelResponseTypeDef,
     GetModelTemplateRequestRequestTypeDef,
-    GetModelTemplateResponseTypeDef,
-    GetModelsRequestGetModelsPaginateTypeDef,
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetRouteRequestRequestTypeDef,
     GetRouteResponseRequestRequestTypeDef,
-    GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
     GetRouteResponsesRequestRequestTypeDef,
-    GetRoutesRequestGetRoutesPaginateTypeDef,
     GetRoutesRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
-    GetStagesRequestGetStagesPaginateTypeDef,
     GetStagesRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
-    GetTagsResponseTypeDef,
     GetVpcLinkRequestRequestTypeDef,
-    GetVpcLinkResponseTypeDef,
     GetVpcLinksRequestRequestTypeDef,
     VpcLinkTypeDef,
     ImportApiRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ReimportApiRequestRequestTypeDef,
     ResetAuthorizersCacheRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiMappingRequestRequestTypeDef,
-    UpdateApiMappingResponseTypeDef,
     UpdateDeploymentRequestRequestTypeDef,
-    UpdateDeploymentResponseTypeDef,
     UpdateIntegrationResponseRequestRequestTypeDef,
-    UpdateIntegrationResponseResponseTypeDef,
     UpdateModelRequestRequestTypeDef,
-    UpdateModelResponseTypeDef,
     UpdateVpcLinkRequestRequestTypeDef,
-    UpdateVpcLinkResponseTypeDef,
-    GetApiMappingsResponseTypeDef,
     ApiTypeDef,
+    AuthorizerTypeDef,
     CreateApiRequestRequestTypeDef,
+    UpdateApiRequestRequestTypeDef,
+    CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
+    CreateAuthorizerResponseTypeDef,
+    CreateDeploymentResponseTypeDef,
+    CreateIntegrationResponseResponseTypeDef,
+    CreateModelResponseTypeDef,
+    CreateVpcLinkResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportApiResponseTypeDef,
+    GetApiMappingResponseTypeDef,
+    GetApiMappingsResponseTypeDef,
     GetApiResponseTypeDef,
+    GetAuthorizerResponseTypeDef,
+    GetDeploymentResponseTypeDef,
+    GetIntegrationResponseResponseTypeDef,
+    GetModelResponseTypeDef,
+    GetModelTemplateResponseTypeDef,
+    GetTagsResponseTypeDef,
+    GetVpcLinkResponseTypeDef,
     ImportApiResponseTypeDef,
     ReimportApiResponseTypeDef,
-    UpdateApiRequestRequestTypeDef,
+    UpdateApiMappingResponseTypeDef,
     UpdateApiResponseTypeDef,
-    AuthorizerTypeDef,
+    UpdateAuthorizerResponseTypeDef,
+    UpdateDeploymentResponseTypeDef,
+    UpdateIntegrationResponseResponseTypeDef,
+    UpdateModelResponseTypeDef,
+    UpdateVpcLinkResponseTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
-    CreateAuthorizerResponseTypeDef,
-    GetAuthorizerResponseTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
-    UpdateAuthorizerResponseTypeDef,
     CreateDomainNameRequestRequestTypeDef,
     UpdateDomainNameRequestRequestTypeDef,
     CreateDomainNameResponseTypeDef,
     DomainNameTypeDef,
     GetDomainNameResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     CreateIntegrationRequestRequestTypeDef,
     UpdateIntegrationRequestRequestTypeDef,
     CreateIntegrationResultTypeDef,
     GetIntegrationResultTypeDef,
     IntegrationTypeDef,
     UpdateIntegrationResultTypeDef,
     CreateRouteRequestRequestTypeDef,
     CreateRouteResponseRequestRequestTypeDef,
+    UpdateRouteRequestRequestTypeDef,
+    UpdateRouteResponseRequestRequestTypeDef,
     CreateRouteResponseResponseTypeDef,
     CreateRouteResultTypeDef,
     GetRouteResponseResponseTypeDef,
     GetRouteResultTypeDef,
     RouteResponseTypeDef,
     RouteTypeDef,
-    UpdateRouteRequestRequestTypeDef,
-    UpdateRouteResponseRequestRequestTypeDef,
     UpdateRouteResponseResponseTypeDef,
     UpdateRouteResultTypeDef,
     CreateStageRequestRequestTypeDef,
+    UpdateStageRequestRequestTypeDef,
     CreateStageResponseTypeDef,
     GetStageResponseTypeDef,
     StageTypeDef,
-    UpdateStageRequestRequestTypeDef,
     UpdateStageResponseTypeDef,
     GetDeploymentsResponseTypeDef,
+    GetApisRequestGetApisPaginateTypeDef,
+    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
+    GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+    GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+    GetModelsRequestGetModelsPaginateTypeDef,
+    GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+    GetRoutesRequestGetRoutesPaginateTypeDef,
+    GetStagesRequestGetStagesPaginateTypeDef,
     GetIntegrationResponsesResponseTypeDef,
     GetModelsResponseTypeDef,
     GetVpcLinksResponseTypeDef,
     GetApisResponseTypeDef,
     GetAuthorizersResponseTypeDef,
     GetDomainNamesResponseTypeDef,
     GetIntegrationsResponseTypeDef,
     GetRouteResponsesResponseTypeDef,
     GetRoutesResponseTypeDef,
     GetStagesResponseTypeDef,
 )
 
 
-def get_structure() -> AccessLogSettingsTypeDef:
+def get_structure() -> AccessLogSettingsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-apigatewayv2-1.28.0/mypy_boto3_apigatewayv2.egg-info/SOURCES.txt` & `mypy-boto3-apigatewayv2-1.28.10/mypy_boto3_apigatewayv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.0/setup.py` & `mypy-boto3-apigatewayv2-1.28.10/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-apigatewayv2",
-    version="1.28.0",
+    version="1.28.10",
     packages=["mypy_boto3_apigatewayv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ApiGatewayV2 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.ApiGatewayV2 1.28.10 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

