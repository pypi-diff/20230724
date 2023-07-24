# Comparing `tmp/cow_api-0.1.0.tar.gz` & `tmp/cow_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cow_api-0.1.0.tar", last modified: Sun Jul 23 14:49:58 2023, max compression
+gzip compressed data, was "cow_api-0.1.1.tar", last modified: Mon Jul 24 09:32:09 2023, max compression
```

## Comparing `cow_api-0.1.0.tar` & `cow_api-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 falkolavitt   (501) staff       (20)        0 2023-07-23 14:49:58.821909 cow_api-0.1.0/
--rw-r--r--   0 falkolavitt   (501) staff       (20)       17 2023-07-23 14:43:30.000000 cow_api-0.1.0/MANIFEST.in
--rw-r--r--   0 falkolavitt   (501) staff       (20)      284 2023-07-23 14:49:58.821600 cow_api-0.1.0/PKG-INFO
--rw-r--r--   0 falkolavitt   (501) staff       (20)      794 2023-07-23 14:48:02.000000 cow_api-0.1.0/README.md
-drwxr-xr-x   0 falkolavitt   (501) staff       (20)        0 2023-07-23 14:49:58.818211 cow_api-0.1.0/cow_api/
--rw-r--r--   0 falkolavitt   (501) staff       (20)        0 2023-07-23 14:34:28.000000 cow_api-0.1.0/cow_api/__init__.py
--rw-r--r--   0 falkolavitt   (501) staff       (20)     4211 2023-07-23 14:29:21.000000 cow_api-0.1.0/cow_api/main.py
-drwxr-xr-x   0 falkolavitt   (501) staff       (20)        0 2023-07-23 14:49:58.820320 cow_api-0.1.0/cow_api.egg-info/
--rw-r--r--   0 falkolavitt   (501) staff       (20)      284 2023-07-23 14:49:58.000000 cow_api-0.1.0/cow_api.egg-info/PKG-INFO
--rw-r--r--   0 falkolavitt   (501) staff       (20)      257 2023-07-23 14:49:58.000000 cow_api-0.1.0/cow_api.egg-info/SOURCES.txt
--rw-r--r--   0 falkolavitt   (501) staff       (20)        1 2023-07-23 14:49:58.000000 cow_api-0.1.0/cow_api.egg-info/dependency_links.txt
--rw-r--r--   0 falkolavitt   (501) staff       (20)       31 2023-07-23 14:49:58.000000 cow_api-0.1.0/cow_api.egg-info/requires.txt
--rw-r--r--   0 falkolavitt   (501) staff       (20)       14 2023-07-23 14:49:58.000000 cow_api-0.1.0/cow_api.egg-info/top_level.txt
--rw-r--r--   0 falkolavitt   (501) staff       (20)       38 2023-07-23 14:49:58.822002 cow_api-0.1.0/setup.cfg
--rw-r--r--   0 falkolavitt   (501) staff       (20)      508 2023-07-23 14:43:31.000000 cow_api-0.1.0/setup.py
-drwxr-xr-x   0 falkolavitt   (501) staff       (20)        0 2023-07-23 14:49:58.820950 cow_api-0.1.0/tests/
--rw-r--r--   0 falkolavitt   (501) staff       (20)        0 2023-07-23 14:34:45.000000 cow_api-0.1.0/tests/__init__.py
--rw-r--r--   0 falkolavitt   (501) staff       (20)     2266 2023-07-23 14:36:27.000000 cow_api-0.1.0/tests/test_main.py
+drwxr-xr-x   0 falkolavitt   (501) staff       (20)        0 2023-07-24 09:32:09.277974 cow_api-0.1.1/
+-rw-r--r--   0 falkolavitt   (501) staff       (20)       17 2023-07-23 14:43:30.000000 cow_api-0.1.1/MANIFEST.in
+-rw-r--r--   0 falkolavitt   (501) staff       (20)     1234 2023-07-24 09:32:09.277559 cow_api-0.1.1/PKG-INFO
+-rw-r--r--   0 falkolavitt   (501) staff       (20)      914 2023-07-23 15:02:12.000000 cow_api-0.1.1/README.md
+drwxr-xr-x   0 falkolavitt   (501) staff       (20)        0 2023-07-24 09:32:09.274825 cow_api-0.1.1/cow_api/
+-rw-r--r--   0 falkolavitt   (501) staff       (20)        0 2023-07-23 14:34:28.000000 cow_api-0.1.1/cow_api/__init__.py
+-rw-r--r--   0 falkolavitt   (501) staff       (20)     3934 2023-07-24 09:23:00.000000 cow_api-0.1.1/cow_api/main.py
+-rw-r--r--   0 falkolavitt   (501) staff       (20)     1777 2023-07-24 08:58:28.000000 cow_api-0.1.1/cow_api/models.py
+drwxr-xr-x   0 falkolavitt   (501) staff       (20)        0 2023-07-24 09:32:09.276450 cow_api-0.1.1/cow_api.egg-info/
+-rw-r--r--   0 falkolavitt   (501) staff       (20)     1234 2023-07-24 09:32:09.000000 cow_api-0.1.1/cow_api.egg-info/PKG-INFO
+-rw-r--r--   0 falkolavitt   (501) staff       (20)      275 2023-07-24 09:32:09.000000 cow_api-0.1.1/cow_api.egg-info/SOURCES.txt
+-rw-r--r--   0 falkolavitt   (501) staff       (20)        1 2023-07-24 09:32:09.000000 cow_api-0.1.1/cow_api.egg-info/dependency_links.txt
+-rw-r--r--   0 falkolavitt   (501) staff       (20)       31 2023-07-24 09:32:09.000000 cow_api-0.1.1/cow_api.egg-info/requires.txt
+-rw-r--r--   0 falkolavitt   (501) staff       (20)       14 2023-07-24 09:32:09.000000 cow_api-0.1.1/cow_api.egg-info/top_level.txt
+-rw-r--r--   0 falkolavitt   (501) staff       (20)       38 2023-07-24 09:32:09.278079 cow_api-0.1.1/setup.cfg
+-rw-r--r--   0 falkolavitt   (501) staff       (20)      680 2023-07-24 09:30:29.000000 cow_api-0.1.1/setup.py
+drwxr-xr-x   0 falkolavitt   (501) staff       (20)        0 2023-07-24 09:32:09.277086 cow_api-0.1.1/tests/
+-rw-r--r--   0 falkolavitt   (501) staff       (20)        0 2023-07-23 14:34:45.000000 cow_api-0.1.1/tests/__init__.py
+-rw-r--r--   0 falkolavitt   (501) staff       (20)     2410 2023-07-24 08:52:42.000000 cow_api-0.1.1/tests/test_main.py
```

### Comparing `cow_api-0.1.0/README.md` & `cow_api-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 
 ### Installation
 
 Install the package using pip:
 
 `pip install cow_api`
 
+Alternatively, you can clone the repository and install the requirements using pip:
+
+`pip install -r requirements.txt`
+
 ### Usage
 
 After installation, you can run the application using uvicorn:
 
 `uvicorn cow_api.main:app --reload`
 Then navigate to http://localhost:8000/docs in your web browser to access the API.
```

### Comparing `cow_api-0.1.0/cow_api/main.py` & `cow_api-0.1.1/cow_api/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,146 +1,101 @@
+from cow_api.models import Cow
 from fastapi import FastAPI, HTTPException
-from faker import Faker
+from fastapi.encoders import jsonable_encoder
+from fastapi.responses import JSONResponse
+from loguru import logger
 from typing import List, Optional
-from pydantic import BaseModel
-import uuid
-import json
-
-fake = Faker()
-Faker.seed(1)
-
 
-class Weight(BaseModel):
-    mass_kg: float
-    last_measured: str
-
-
-class Feeding(BaseModel):
-    amount_kg: float
-    cron_schedule: str
-    last_measured: str
-
-
-class MilkProduction(BaseModel):
-    last_milk: str
-    cron_schedule: str
-    amount_l: float
-
-
-class Cow(BaseModel):
-    id: str
-    name: str
-    sex: str
-    birthdate: str
-    condition: str
-    weight: Weight
-    feeding: Feeding
-    milk_production: MilkProduction
-    has_calves: bool
-
-    @classmethod
-    def generate_fake(cls):
-        return cls(
-            id=str(uuid.uuid4()),
-            name=fake.first_name(),
-            sex=fake.random_element(elements=["Male", "Female"]),
-            birthdate=str(fake.date_time()),
-            condition=fake.random_element(elements=["Healthy", "Sick"]),
-            weight=Weight(
-                mass_kg=fake.random_int(min=1000, max=1500),
-                last_measured=str(fake.date_time()),
-            ),
-            feeding=Feeding(
-                amount_kg=fake.random_int(min=1, max=10),
-                cron_schedule="0 */6 * * *",
-                last_measured=str(fake.date_time()),
-            ),
-            milk_production=MilkProduction(
-                last_milk=str(fake.date_time()),
-                cron_schedule="0 8,12,16,20 * * *",
-                amount_l=fake.random_int(min=1, max=10),
-            ),
-            has_calves=fake.random_element(elements=[True, False]),
-        )
+import json
 
+logger.add("cow_api.log", rotation="500MB")
 
 all_cows: List[Cow] = [Cow.generate_fake() for _ in range(100)]
 
-
-app = FastAPI()
+app = FastAPI(title="Cow API", version="0.1.0")
 
 
 @app.get("/cows", status_code=200, response_model=List[Cow])
 async def get_cows() -> List[Cow]:
     """
     Get all cows.
 
     Returns:
         list: List of cows."""
+    logger.success("Successfully retrieved all cows.")
     return all_cows
 
 
 @app.get("/cows/{cow_id}", status_code=200, response_model=Cow)
 async def get_single_cow(cow_id: str) -> Cow | None:
     """
     Get single cow based on id.
 
     Returns:
         Single Cow."""
 
     for cow in all_cows:
         if cow.id == cow_id:
+            logger.success("Successfully retrieved single cow.")
             return cow
 
 
 @app.post("/cows/", status_code=201)
-async def add_cow(cow: Cow):
+async def add_cow(cow: Cow) -> Cow:
     """
     Add a cow.
 
     Returns:
         Dict: same payload as the one sent with 201 status code on success.
     """
     all_cows.append(cow)
+    logger.success("Successfully added cow.")
     return cow
 
 
 @app.put("/cows/{cow_id}", status_code=200, response_model=Cow)
 async def update_cow(cow_id: str, cow: Cow) -> Cow:
     """
     Update a cow.
 
     Returns:
         Dict: same payload as the one sent with 200 status code on success.
     """
     for i, existing_cow in enumerate(all_cows):
         if existing_cow.id == cow_id:
             all_cows[i] = cow
+            logger.success("Successfully updated cow.")
             return cow
+    logger.error("Cow not found.")
     raise HTTPException(status_code=404, detail="Cow not found")
 
 
 @app.delete("/cows/{cow_id}", status_code=200)
 async def delete_cow(cow_id: str) -> Cow:
     """
     Delete a cow.
 
     Returns:
         Dict: same payload as the one sent with 200 status code on success.
     """
     for i, existing_cow in enumerate(all_cows):
         if existing_cow.id == cow_id:
             del all_cows[i]
+            logger.success("Successfully deleted cow.")
             return existing_cow
+    logger.error("Cow not found.")
     raise HTTPException(status_code=404, detail="Cow not found")
 
 
-def filter_cow(cow: Cow, field: str, value: str):
+def filter_cow(cow: Cow, field: str, value: str) -> bool:
+    # This assumes that the field is a nested field using '.', e.g. "weight.mass_kg"
     fields = field.split(".")
     temp_value = cow
+
+    # Traverse the nested fields and check if the value matches.
     for f in fields:
         if hasattr(temp_value, f):
             temp_value = getattr(temp_value, f)
         else:
             return False
     try:
         # Attempt to convert the value to json. This will handle boolean and numeric values correctly.
@@ -148,20 +103,34 @@
     except json.JSONDecodeError:
         # If the value cannot be converted, leave it as is. It is likely a string.
         pass
     return temp_value == value
 
 
 @app.get("/cows/filter/{field}", response_model=List[Cow])
-async def filter_cows(field: str, value: Optional[str] = None):
+async def filter_cows(field: str, value: Optional[str] = None) -> List[Cow]:
     """
     Filter cows based on the field and value provided.
 
     Returns:
         list: List of filtered cows.
     """
     if not value:
+        logger.warning("Found no value to filter by. Returning all cows.")
         return all_cows
 
     filtered_cows = [cow for cow in all_cows if filter_cow(cow, field, value)]
 
+    if len(filtered_cows) == 0:
+        logger.warning(
+            f"Found no cows matching the filter, based on {field}. Returning all cows."
+        )
+        return all_cows
+
+    logger.success("Successfully filtered cows.")
     return filtered_cows
+
+
+@app.get("/healthcheck", status_code=200)
+def healthcheck() -> JSONResponse:
+    logger.success("Successfully healthchecked.")
+    return JSONResponse(content=jsonable_encoder({"status": "Ok"}))
```

### Comparing `cow_api-0.1.0/tests/test_main.py` & `cow_api-0.1.1/tests/test_main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from fastapi.testclient import TestClient
-from cow_api.main import app, Cow, Weight, Feeding, MilkProduction
+from cow_api.main import app, Cow
 
 client = TestClient(app)
 
 
 class TestAPI:
+    def test_api_healthcheck(self):
+        response = client.get("/healthcheck")
+        assert response.status_code == 200
+        assert response.json() == {"status": "Ok"}
+
     def test_cows_endpoint_returns_200(self):
         response = client.get("/cows")
         assert response.status_code == 200
 
     def test_get_cows_endpoint_returns_nonempty_list(self):
         response = client.get("/cows")
         assert response.json() != []
```

