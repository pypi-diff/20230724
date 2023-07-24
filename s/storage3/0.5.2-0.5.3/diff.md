# Comparing `tmp/storage3-0.5.2.tar.gz` & `tmp/storage3-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storage3-0.5.2.tar", max compression
+gzip compressed data, was "storage3-0.5.3.tar", max compression
```

## Comparing `storage3-0.5.2.tar` & `storage3-0.5.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1147 2022-10-28 11:19:58.756229 storage3-0.5.2/LICENSE
--rw-r--r--   0        0        0      613 2022-10-28 11:19:58.756641 storage3-0.5.2/README.md
--rw-r--r--   0        0        0     1788 2023-03-05 15:07:14.498196 storage3-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      894 2023-03-05 15:06:46.561906 storage3-0.5.2/storage3/__init__.py
--rw-r--r--   0        0        0       61 2022-10-28 11:19:58.759300 storage3-0.5.2/storage3/_async/__init__.py
--rw-r--r--   0        0        0     3198 2022-10-28 11:19:58.759455 storage3-0.5.2/storage3/_async/bucket.py
--rw-r--r--   0        0        0     1367 2023-03-05 15:06:46.562247 storage3-0.5.2/storage3/_async/client.py
--rw-r--r--   0        0        0     8192 2023-02-05 14:06:53.343501 storage3-0.5.2/storage3/_async/file_api.py
--rw-r--r--   0        0        0       59 2023-02-21 06:31:46.000000 storage3-0.5.2/storage3/_sync/__init__.py
--rw-r--r--   0        0        0     3117 2023-03-05 15:05:45.260745 storage3-0.5.2/storage3/_sync/bucket.py
--rw-r--r--   0        0        0     1324 2023-03-05 15:06:46.562510 storage3-0.5.2/storage3/_sync/client.py
--rw-r--r--   0        0        0     8080 2023-03-05 15:05:45.261258 storage3-0.5.2/storage3/_sync/file_api.py
--rw-r--r--   0        0        0      288 2023-03-05 15:06:46.562727 storage3-0.5.2/storage3/constants.py
--rw-r--r--   0        0        0     1336 2023-03-05 15:06:46.563576 storage3-0.5.2/storage3/types.py
--rw-r--r--   0        0        0      308 2023-03-05 15:07:23.620039 storage3-0.5.2/storage3/utils.py
--rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 storage3-0.5.2/setup.py
--rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 storage3-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1147 2023-07-24 20:22:34.982546 storage3-0.5.3/LICENSE
+-rw-r--r--   0        0        0      909 2023-07-24 20:22:34.982777 storage3-0.5.3/README.md
+-rw-r--r--   0        0        0     1859 2023-07-24 20:23:13.116881 storage3-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      894 2023-07-24 20:22:34.984482 storage3-0.5.3/storage3/__init__.py
+-rw-r--r--   0        0        0       61 2023-07-24 20:22:34.984598 storage3-0.5.3/storage3/_async/__init__.py
+-rw-r--r--   0        0        0     3984 2023-07-24 20:22:34.984701 storage3-0.5.3/storage3/_async/bucket.py
+-rw-r--r--   0        0        0     1367 2023-07-24 20:22:34.984776 storage3-0.5.3/storage3/_async/client.py
+-rw-r--r--   0        0        0    12745 2023-07-24 20:22:34.984896 storage3-0.5.3/storage3/_async/file_api.py
+-rw-r--r--   0        0        0       59 2023-07-24 20:22:34.985012 storage3-0.5.3/storage3/_sync/__init__.py
+-rw-r--r--   0        0        0     3891 2023-07-24 20:22:34.985100 storage3-0.5.3/storage3/_sync/bucket.py
+-rw-r--r--   0        0        0     1324 2023-07-24 20:22:34.985173 storage3-0.5.3/storage3/_sync/client.py
+-rw-r--r--   0        0        0    12597 2023-07-24 20:22:34.985259 storage3-0.5.3/storage3/_sync/file_api.py
+-rw-r--r--   0        0        0      288 2023-07-24 20:22:34.985338 storage3-0.5.3/storage3/constants.py
+-rw-r--r--   0        0        0     1828 2023-07-24 20:22:34.985412 storage3-0.5.3/storage3/types.py
+-rw-r--r--   0        0        0      308 2023-07-24 20:23:28.507758 storage3-0.5.3/storage3/utils.py
+-rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 storage3-0.5.3/PKG-INFO
```

### Comparing `storage3-0.5.2/LICENSE` & `storage3-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `storage3-0.5.2/pyproject.toml` & `storage3-0.5.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,35 +14,38 @@
 description = "Supabase Storage client for Python."
 documentation = "https://supabase-community.github.io/storage-py"
 homepage = "https://supabase-community.github.io/storage-py"
 license = "MIT"
 name = "storage3"
 readme = "README.md"
 repository = "https://github.com/supabase-community/storage-py"
-version = "0.5.2"
+version = "0.5.3"
 
 [tool.poetry.dependencies]
-httpx = "^0.23"
+httpx = ">=0.23,<0.25"
 python = "^3.8"
 typing-extensions = "^4.2.0"
 python-dateutil = "^2.8.2"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "^7.33.2"
-black = "^23.1.0"
+black = "^23.3.0"
 isort = "^5.12.0"
-pre-commit = "^3.1.1"
-pytest = "^7.2.0"
-pytest-asyncio = "^0.20.3"
-pytest-cov = "^4.0.0"
+pre-commit = "^3.3.3"
+pytest = "^7.4.0"
+pytest-asyncio = "^0.21.0"
+pytest-cov = "^4.1.0"
 python-dotenv = "^1.0.0"
-Sphinx = "^6.1.3"
+Sphinx = "^7.0.1"
 sphinx-press-theme = "^0.8.0"
 unasync-cli = "^0.0.9"
 
+[tool.poetry.group.dev.dependencies]
+sphinx-toolbox = "^3.4.0"
+
 [tool.semantic_release]
 version_variable = "storage3/utils.py:__version__"
 version_toml = "pyproject.toml:tool.poetry.version"
 major_on_zero = false
 commit_subject = "chore(release): bump version to v{version}"
 build_command = "curl -sSL https://install.python-poetry.org | python - --preview && export PATH=\"/github/home/.local/bin:$PATH\" && poetry install && poetry build"
 upload_to_repository = true
```

### Comparing `storage3-0.5.2/storage3/__init__.py` & `storage3-0.5.3/storage3/__init__.py`

 * *Files identical despite different names*

### Comparing `storage3-0.5.2/storage3/_async/bucket.py` & `storage3-0.5.3/storage3/_async/bucket.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import Any, Optional
 
 from httpx import HTTPError, Response
 
-from ..types import RequestMethod
+from ..types import CreateOrUpdateBucketOptions, RequestMethod
 from ..utils import AsyncClient, StorageException
 from .file_api import AsyncBucket
 
 __all__ = ["AsyncStorageBucketAPI"]
 
 
 class AsyncStorageBucketAPI:
@@ -48,34 +48,58 @@
             The unique identifier of the bucket you would like to retrieve.
         """
         res = await self._request("GET", f"/bucket/{id}")
         json = res.json()
         return AsyncBucket(**json, _client=self._client)
 
     async def create_bucket(
-        self, id: str, name: Optional[str] = None, public: bool = False
+        self,
+        id: str,
+        name: Optional[str] = None,
+        options: Optional[CreateOrUpdateBucketOptions] = None,
     ) -> dict[str, str]:
         """Creates a new storage bucket.
 
         Parameters
         ----------
         id
             A unique identifier for the bucket you are creating.
         name
             A name for the bucket you are creating. If not passed, the id is used as the name as well.
-        public
-            Whether the bucket you are creating should be publicly accessible. Defaults to False.
+        options
+            Extra options to send while creating the bucket. Valid options are `public`, `file_size_limit` and
+            `allowed_mime_types`.
         """
+        json: dict[str, Any] = {"id": id, "name": name or id}
+        if options:
+            json.update(**options)
         res = await self._request(
             "POST",
             "/bucket",
-            json={"id": id, "name": name or id, "public": public},
+            json=json,
         )
         return res.json()
 
+    async def update_bucket(
+        self, id: str, options: CreateOrUpdateBucketOptions
+    ) -> dict[str, str]:
+        """Update a storage bucket.
+
+        Parameters
+        ----------
+        id
+            The unique identifier of the bucket you would like to update.
+        options
+            The properties you want to update. Valid options are `public`, `file_size_limit` and
+            `allowed_mime_types`.
+        """
+        json = {"id": id, "name": id, **options}
+        res = await self._request("PUT", f"/bucket/{id}", json=json)
+        return res.json()
+
     async def empty_bucket(self, id: str) -> dict[str, str]:
         """Removes all objects inside a single bucket.
 
         Parameters
         ----------
         id
             The unique identifier of the bucket you would like to empty.
```

### Comparing `storage3-0.5.2/storage3/_async/client.py` & `storage3-0.5.3/storage3/_async/client.py`

 * *Files identical despite different names*

### Comparing `storage3-0.5.2/storage3/_async/file_api.py` & `storage3-0.5.3/storage3/_sync/file_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,38 +8,41 @@
 
 from httpx import HTTPError, Response
 
 from ..constants import DEFAULT_FILE_OPTIONS, DEFAULT_SEARCH_OPTIONS
 from ..types import (
     BaseBucket,
     CreateSignedURLOptions,
+    CreateSignedURLsOptions,
+    FileOptions,
     ListBucketFilesOptions,
     RequestMethod,
+    SignedUploadURL,
     TransformOptions,
 )
-from ..utils import AsyncClient, StorageException
+from ..utils import StorageException, SyncClient
 
-__all__ = ["AsyncBucket"]
+__all__ = ["SyncBucket"]
 
 
-class AsyncBucketActionsMixin:
+class SyncBucketActionsMixin:
     """Functions needed to access the file API."""
 
     id: str
-    _client: AsyncClient
+    _client: SyncClient
 
-    async def _request(
+    def _request(
         self,
         method: RequestMethod,
         url: str,
         headers: Optional[dict[str, Any]] = None,
         json: Optional[dict[Any, Any]] = None,
         files: Optional[Any] = None,
     ) -> Response:
-        response = await self._client.request(
+        response = self._client.request(
             method,
             url,
             headers=headers or {},
             json=json,
             files=files,
         )
         try:
@@ -47,111 +50,235 @@
         except HTTPError:
             raise StorageException(
                 {**response.json(), "statusCode": response.status_code}
             )
 
         return response
 
-    async def create_signed_url(
+    def create_signed_upload_url(self, path: str) -> SignedUploadURL:
+        """
+        Creates a signed upload URL.
+
+        Parameters
+        ----------
+        path
+            The file path, including the file name. For example `folder/image.png`.
+        """
+        _path = self._get_final_path(path)
+        response = self._request("POST", f"/object/upload/sign/{_path}")
+        data = response.json()
+        full_url: urllib.parse.ParseResult = urllib.parse.urlparse(
+            str(self._client.base_url) + data["url"]
+        )
+        query_params = urllib.parse.parse_qs(full_url.query)
+        if not query_params.get("token"):
+            raise StorageException("No token sent by the API")
+        return {
+            "signed_url": full_url.geturl(),
+            "token": query_params["token"][0],
+            "path": path,
+        }
+
+    def upload_to_signed_url(
+        self,
+        path: str,
+        token: str,
+        file: Union[BufferedReader, bytes, FileIO, str, Path],
+        file_options: Optional[FileOptions] = None,
+    ) -> Response:
+        """
+        Upload a file with a token generated from :meth:`.create_signed_url`
+
+        Parameters
+        ----------
+        path
+            The file path, including the file name
+        token
+            The token generated from :meth:`.create_signed_url`
+        file
+            The file contents or a file-like object to upload
+        file_options
+            Additional options for the uploaded file
+        """
+        _path = self._get_final_path(path)
+        _url = urllib.parse.urlparse(f"/object/upload/sign/{_path}")
+        query_params = urllib.parse.urlencode({"token": token})
+        final_url = f"{_url.geturl()}?{query_params}"
+
+        if file_options is None:
+            file_options = {}
+
+        cache_control = file_options.get("cache-control")
+        if cache_control:
+            file_options["cache-control"] = f"max-age={cache_control}"
+
+        headers = {
+            **self._client.headers,
+            **DEFAULT_FILE_OPTIONS,
+            **file_options,
+        }
+        filename = path.rsplit("/", maxsplit=1)[-1]
+
+        if (
+            isinstance(file, BufferedReader)
+            or isinstance(file, bytes)
+            or isinstance(file, FileIO)
+        ):
+            # bytes or byte-stream-like object received
+            _file = {"file": (filename, file, headers.pop("content-type"))}
+        else:
+            # str or pathlib.path received
+            _file = {
+                "file": (
+                    filename,
+                    open(file, "rb"),
+                    headers.pop("content-type"),
+                )
+            }
+        return self._request(
+            "PUT",
+            final_url,
+            files=_file,
+            headers=headers,
+        )
+
+    def create_signed_url(
         self, path: str, expires_in: int, options: CreateSignedURLOptions = {}
     ) -> dict[str, str]:
         """
         Parameters
         ----------
         path
             file path to be downloaded, including the current file name.
         expires_in
             number of seconds until the signed URL expires.
+        options
+            options to be passed for downloading or transforming the file.
         """
+        json = {"expiresIn": str(expires_in)}
+        if options.get("download"):
+            json.update({"download": options["download"]})
+        if options.get("transform"):
+            json.update({"transform": options["transform"]})
+
         path = self._get_final_path(path)
-        response = await self._request(
+        response = self._request(
             "POST",
             f"/object/sign/{path}",
-            json={"expiresIn": str(expires_in)},
+            json=json,
         )
         data = response.json()
         data[
             "signedURL"
         ] = f"{self._client.base_url}{cast(str, data['signedURL']).lstrip('/')}"
         return data
 
-    async def get_public_url(self, path: str, options: TransformOptions = {}) -> str:
+    def create_signed_urls(
+        self, paths: list[str], expires_in: int, options: CreateSignedURLsOptions = {}
+    ) -> list[dict[str, str]]:
+        """
+        Parameters
+        ----------
+        path
+            file path to be downloaded, including the current file name.
+        expires_in
+            number of seconds until the signed URL expires.
+        options
+            options to be passed for downloading the file.
+        """
+        json = {"paths": paths, "expiresIn": str(expires_in)}
+        if options.get("download"):
+            json.update({"download": options["download"]})
+
+        response = self._request(
+            "POST",
+            f"/object/sign/{self.id}",
+            json=json,
+        )
+        data = response.json()
+        for item in data:
+            item[
+                "signedURL"
+            ] = f"{self._client.base_url}{cast(str, item['signedURL']).lstrip('/')}"
+        return data
+
+    def get_public_url(self, path: str, options: TransformOptions = {}) -> str:
         """
         Parameters
         ----------
         path
             file path, including the path and file name. For example `folder/image.png`.
         """
         render_path = "render/image" if options.get("transform") else "object"
         transformation_query = urllib.parse.urlencode(options)
         query_string = f"?{transformation_query}" if transformation_query else ""
         _path = self._get_final_path(path)
         return f"{self._client.base_url}{render_path}/public/{_path}{query_string}"
 
-    async def move(self, from_path: str, to_path: str) -> dict[str, str]:
+    def move(self, from_path: str, to_path: str) -> dict[str, str]:
         """
         Moves an existing file, optionally renaming it at the same time.
 
         Parameters
         ----------
         from_path
             The original file path, including the current file name. For example `folder/image.png`.
         to_path
             The new file path, including the new file name. For example `folder/image-copy.png`.
         """
-        res = await self._request(
+        res = self._request(
             "POST",
             "/object/move",
             json={
                 "bucketId": self.id,
                 "sourceKey": from_path,
                 "destinationKey": to_path,
             },
         )
         return res.json()
 
-    async def copy(self, from_path: str, to_path: str) -> dict[str, str]:
+    def copy(self, from_path: str, to_path: str) -> dict[str, str]:
         """
         Copies an existing file to a new path in the same bucket.
 
         Parameters
         ----------
         from_path
             The original file path, including the current file name. For example `folder/image.png`.
         to_path
             The new file path, including the new file name. For example `folder/image-copy.png`.
         """
-        res = await self._request(
+        res = self._request(
             "POST",
             "/object/copy",
             json={
                 "bucketId": self.id,
                 "sourceKey": from_path,
                 "destinationKey": to_path,
             },
         )
         return res.json()
 
-    async def remove(self, paths: list) -> dict[str, str]:
+    def remove(self, paths: list) -> dict[str, str]:
         """
         Deletes files within the same bucket
 
         Parameters
         ----------
         paths
             An array or list of files to be deletes, including the path and file name. For example [`folder/image.png`].
         """
-        response = await self._request(
+        response = self._request(
             "DELETE",
             f"/object/{self.id}",
             json={"prefixes": paths},
         )
         return response.json()
 
-    async def list(
+    def list(
         self,
         path: Optional[str] = None,
         options: Optional[ListBucketFilesOptions] = None,
     ) -> list[dict[str, str]]:
         """
         Lists all the files within a bucket.
 
@@ -160,24 +287,28 @@
         path
             The folder path.
         options
             Search options, including `limit`, `offset`, and `sortBy`.
         """
         extra_options = options or {}
         extra_headers = {"Content-Type": "application/json"}
-        body = {**DEFAULT_SEARCH_OPTIONS, **extra_options, "prefix": path or ""}
-        response = await self._request(
+        body = {
+            **DEFAULT_SEARCH_OPTIONS,
+            **extra_options,
+            "prefix": path or "",
+        }
+        response = self._request(
             "POST",
             f"/object/list/{self.id}",
             json=body,
             headers=extra_headers,
         )
         return response.json()
 
-    async def download(self, path: str, options: TransformOptions = {}) -> bytes:
+    def download(self, path: str, options: TransformOptions = {}) -> bytes:
         """
         Downloads a file.
 
         Parameters
         ----------
         path
             The file path to be downloaded, including the path and file name. For example `folder/image.png`.
@@ -185,74 +316,91 @@
         render_path = (
             "render/image/authenticated" if options.get("transform") else "object"
         )
         transformation_query = urllib.parse.urlencode(options)
         query_string = f"?{transformation_query}" if transformation_query else ""
 
         _path = self._get_final_path(path)
-        response = await self._request(
+        response = self._request(
             "GET",
             f"{render_path}/{_path}{query_string}",
         )
         return response.content
 
-    async def upload(
-        self, path: str, file: Union[str, Path], file_options: Optional[dict] = None
+    def upload(
+        self,
+        path: str,
+        file: Union[BufferedReader, bytes, FileIO, str, Path],
+        file_options: Optional[FileOptions] = None,
     ) -> Response:
         """
         Uploads a file to an existing bucket.
 
         Parameters
         ----------
         path
             The relative file path including the bucket ID. Should be of the format `bucket/folder/subfolder/filename.png`.
             The bucket must already exist before attempting to upload.
         file
             The File object to be stored in the bucket. or a async generator of chunks
         file_options
-            HTTP headers. For example `cache-control`
+            HTTP headers.
         """
         if file_options is None:
             file_options = {}
-        headers = {**self._client.headers, **DEFAULT_FILE_OPTIONS, **file_options}
+        cache_control = file_options.get("cache-control")
+        if cache_control:
+            file_options["cache-control"] = f"max-age={cache_control}"
+
+        headers = {
+            **self._client.headers,
+            **DEFAULT_FILE_OPTIONS,
+            **file_options,
+        }
         filename = path.rsplit("/", maxsplit=1)[-1]
 
         if (
             isinstance(file, BufferedReader)
             or isinstance(file, bytes)
             or isinstance(file, FileIO)
         ):
             # bytes or byte-stream-like object received
             files = {"file": (filename, file, headers.pop("content-type"))}
         else:
             # str or pathlib.path received
-            files = {"file": (filename, open(file, "rb"), headers.pop("content-type"))}
+            files = {
+                "file": (
+                    filename,
+                    open(file, "rb"),
+                    headers.pop("content-type"),
+                )
+            }
 
         _path = self._get_final_path(path)
 
-        return await self._request(
+        return self._request(
             "POST",
             f"/object/{_path}",
             files=files,
             headers=headers,
         )
 
     def _get_final_path(self, path: str) -> str:
         return f"{self.id}/{path}"
 
 
 # this class is returned by methods that fetch buckets, for example StorageBucketAPI.get_bucket
 # adding this mixin on the BaseBucket means that those bucket objects can also be used to
 # run methods like `upload` and `download`
 @dataclass(repr=False)
-class AsyncBucket(BaseBucket, AsyncBucketActionsMixin):
+class SyncBucket(BaseBucket, SyncBucketActionsMixin):
     """Represents a storage bucket."""
 
-    _client: AsyncClient = field(repr=False)
+    _client: SyncClient = field(repr=False)
 
 
 @dataclass
-class AsyncBucketProxy(AsyncBucketActionsMixin):
+class SyncBucketProxy(SyncBucketActionsMixin):
     """A bucket proxy, this contains the minimum required fields to query the File API."""
 
     id: str
-    _client: AsyncClient = field(repr=False)
+    _client: SyncClient = field(repr=False)
```

### Comparing `storage3-0.5.2/storage3/_sync/bucket.py` & `storage3-0.5.3/storage3/_sync/bucket.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import Any, Optional
 
 from httpx import HTTPError, Response
 
-from ..types import RequestMethod
+from ..types import CreateOrUpdateBucketOptions, RequestMethod
 from ..utils import StorageException, SyncClient
 from .file_api import SyncBucket
 
 __all__ = ["SyncStorageBucketAPI"]
 
 
 class SyncStorageBucketAPI:
@@ -48,34 +48,58 @@
             The unique identifier of the bucket you would like to retrieve.
         """
         res = self._request("GET", f"/bucket/{id}")
         json = res.json()
         return SyncBucket(**json, _client=self._client)
 
     def create_bucket(
-        self, id: str, name: Optional[str] = None, public: bool = False
+        self,
+        id: str,
+        name: Optional[str] = None,
+        options: Optional[CreateOrUpdateBucketOptions] = None,
     ) -> dict[str, str]:
         """Creates a new storage bucket.
 
         Parameters
         ----------
         id
             A unique identifier for the bucket you are creating.
         name
             A name for the bucket you are creating. If not passed, the id is used as the name as well.
-        public
-            Whether the bucket you are creating should be publicly accessible. Defaults to False.
+        options
+            Extra options to send while creating the bucket. Valid options are `public`, `file_size_limit` and
+            `allowed_mime_types`.
         """
+        json: dict[str, Any] = {"id": id, "name": name or id}
+        if options:
+            json.update(**options)
         res = self._request(
             "POST",
             "/bucket",
-            json={"id": id, "name": name or id, "public": public},
+            json=json,
         )
         return res.json()
 
+    def update_bucket(
+        self, id: str, options: CreateOrUpdateBucketOptions
+    ) -> dict[str, str]:
+        """Update a storage bucket.
+
+        Parameters
+        ----------
+        id
+            The unique identifier of the bucket you would like to update.
+        options
+            The properties you want to update. Valid options are `public`, `file_size_limit` and
+            `allowed_mime_types`.
+        """
+        json = {"id": id, "name": id, **options}
+        res = self._request("PUT", f"/bucket/{id}", json=json)
+        return res.json()
+
     def empty_bucket(self, id: str) -> dict[str, str]:
         """Removes all objects inside a single bucket.
 
         Parameters
         ----------
         id
             The unique identifier of the bucket you would like to empty.
```

### Comparing `storage3-0.5.2/storage3/_sync/client.py` & `storage3-0.5.3/storage3/_sync/client.py`

 * *Files identical despite different names*

### Comparing `storage3-0.5.2/storage3/types.py` & `storage3-0.5.3/storage3/types.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Optional, Union
 
 import dateutil.parser
 from typing_extensions import Literal, TypedDict
 
@@ -14,38 +16,63 @@
 
     id: str
     name: str
     owner: str
     public: bool
     created_at: datetime
     updated_at: datetime
-    file_size_limit: int
-    allowed_mime_types: str
+    file_size_limit: Optional[int]
+    allowed_mime_types: Optional[list[str]]
 
     def __post_init__(self) -> None:
         # created_at and updated_at are returned by the API as ISO timestamps
         # so we convert them to datetime objects
         self.created_at = dateutil.parser.isoparse(self.created_at)  # type: ignore
         self.updated_at = dateutil.parser.isoparse(self.updated_at)  # type: ignore
 
 
 # used in bucket.list method's option parameter
 class _sortByType(TypedDict):
     column: str
     order: Literal["asc", "desc"]
 
 
+class SignedUploadURL(TypedDict):
+    signed_url: str
+    token: str
+    path: str
+
+
+class CreateOrUpdateBucketOptions(TypedDict, total=False):
+    public: bool
+    file_size_limit: int
+    allowed_mime_types: list[str]
+
+
 class ListBucketFilesOptions(TypedDict):
     limit: int
     offset: int
     sortBy: _sortByType
 
 
-class TransformOptions(TypedDict):
-    height: Optional[float]
-    width: Optional[float]
-    resize: Optional[Union[Literal["cover"], Literal["contain"], Literal["fill"]]]
+class TransformOptions(TypedDict, total=False):
+    height: int
+    width: int
+    resize: Literal["cover", "contain", "fill"]
+    format: Literal["origin", "avif"]
+    quality: int
+
+
+class CreateSignedURLOptions(TypedDict, total=False):
+    download: Union[str, bool]
+    transform: TransformOptions
+
+
+class CreateSignedURLsOptions(TypedDict):
+    download: Union[str, bool]
 
 
-class CreateSignedURLOptions(TypedDict):
-    download: Optional[Union[str, bool]]
-    transform: Optional[TransformOptions]
+FileOptions = TypedDict(
+    "FileOptions",
+    {"cache-control": str, "content-type": str, "x-upsert": str},
+    total=False,
+)
```

### Comparing `storage3-0.5.2/PKG-INFO` & `storage3-0.5.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: storage3
-Version: 0.5.2
+Version: 0.5.3
 Summary: Supabase Storage client for Python.
 Home-page: https://supabase-community.github.io/storage-py
 License: MIT
 Author: Joel Lee
 Author-email: joel@joellee.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: httpx (>=0.23,<0.24)
+Requires-Dist: httpx (>=0.23,<0.25)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: typing-extensions (>=4.2.0,<5.0.0)
 Project-URL: Documentation, https://supabase-community.github.io/storage-py
 Project-URL: Repository, https://github.com/supabase-community/storage-py
 Description-Content-Type: text/markdown
 
 # Storage-py
@@ -42,7 +41,14 @@
 
 # pass in is_async=True to create an async client
 storage_client = create_client(url, headers, is_async=False)
 
 storage_client.list_buckets()
 ```
 
+### Uploading files
+When uploading files, make sure to set the correct mimetype by using the `file_options` argument:
+```py
+storage_client.from_("bucket").upload("/folder/file.png", file_object, {"content-type": "image/png"})
+```
+If no mime type is given, the default `text/plain` will be used.
+
```

