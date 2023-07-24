# Comparing `tmp/microlearn_gen_course-0.0.1.tar.gz` & `tmp/microlearn_gen_course-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microlearn_gen_course-0.0.1.tar", last modified: Thu Jul 20 08:48:43 2023, max compression
+gzip compressed data, was "microlearn_gen_course-0.0.2.tar", last modified: Mon Jul 24 06:33:02 2023, max compression
```

## Comparing `microlearn_gen_course-0.0.1.tar` & `microlearn_gen_course-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:48:43.955001 microlearn_gen_course-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:48:43.951001 microlearn_gen_course-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:48:43.955001 microlearn_gen_course-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-20 08:48:33.000000 microlearn_gen_course-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-20 08:48:33.000000 microlearn_gen_course-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-20 08:48:43.955001 microlearn_gen_course-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-20 08:48:33.000000 microlearn_gen_course-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-20 08:48:33.000000 microlearn_gen_course-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-20 08:48:43.955001 microlearn_gen_course-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:48:43.955001 microlearn_gen_course-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:48:43.955001 microlearn_gen_course-0.0.1/src/gen_course/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:48:33.000000 microlearn_gen_course-0.0.1/src/gen_course/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-20 08:48:33.000000 microlearn_gen_course-0.0.1/src/gen_course/gen_answer_to_article_ques.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-20 08:48:33.000000 microlearn_gen_course-0.0.1/src/gen_course/gen_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-20 08:48:33.000000 microlearn_gen_course-0.0.1/src/gen_course/gen_course_article_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-20 08:48:33.000000 microlearn_gen_course-0.0.1/src/gen_course/gen_course_articles_titles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-20 08:48:33.000000 microlearn_gen_course-0.0.1/src/gen_course/gen_course_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:48:43.955001 microlearn_gen_course-0.0.1/src/microlearn_gen_course.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-20 08:48:43.000000 microlearn_gen_course-0.0.1/src/microlearn_gen_course.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-20 08:48:43.000000 microlearn_gen_course-0.0.1/src/microlearn_gen_course.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:48:43.000000 microlearn_gen_course-0.0.1/src/microlearn_gen_course.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 08:48:43.000000 microlearn_gen_course-0.0.1/src/microlearn_gen_course.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 08:48:43.000000 microlearn_gen_course-0.0.1/src/microlearn_gen_course.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:48:43.955001 microlearn_gen_course-0.0.1/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-20 08:48:33.000000 microlearn_gen_course-0.0.1/src/tests/test_answer_to_article_ques.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-20 08:48:33.000000 microlearn_gen_course-0.0.1/src/tests/test_gen_course_article_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-20 08:48:33.000000 microlearn_gen_course-0.0.1/src/tests/test_gen_course_articles_titles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-20 08:48:33.000000 microlearn_gen_course-0.0.1/src/tests/test_gen_course_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:33:02.366232 microlearn_gen_course-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:33:02.362232 microlearn_gen_course-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:33:02.362232 microlearn_gen_course-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-24 06:32:50.000000 microlearn_gen_course-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 06:32:50.000000 microlearn_gen_course-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-24 06:33:02.366232 microlearn_gen_course-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 06:32:50.000000 microlearn_gen_course-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-24 06:32:50.000000 microlearn_gen_course-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-24 06:33:02.366232 microlearn_gen_course-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:33:02.362232 microlearn_gen_course-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:33:02.366232 microlearn_gen_course-0.0.2/src/gen_course/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:32:50.000000 microlearn_gen_course-0.0.2/src/gen_course/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-24 06:32:50.000000 microlearn_gen_course-0.0.2/src/gen_course/gen_answer_to_article_ques.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-24 06:32:50.000000 microlearn_gen_course-0.0.2/src/gen_course/gen_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-24 06:32:50.000000 microlearn_gen_course-0.0.2/src/gen_course/gen_course_article_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-24 06:32:50.000000 microlearn_gen_course-0.0.2/src/gen_course/gen_course_articles_titles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-24 06:32:50.000000 microlearn_gen_course-0.0.2/src/gen_course/gen_course_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:33:02.366232 microlearn_gen_course-0.0.2/src/microlearn_gen_course.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-24 06:33:02.000000 microlearn_gen_course-0.0.2/src/microlearn_gen_course.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-24 06:33:02.000000 microlearn_gen_course-0.0.2/src/microlearn_gen_course.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:33:02.000000 microlearn_gen_course-0.0.2/src/microlearn_gen_course.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-24 06:33:02.000000 microlearn_gen_course-0.0.2/src/microlearn_gen_course.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 06:33:02.000000 microlearn_gen_course-0.0.2/src/microlearn_gen_course.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:33:02.366232 microlearn_gen_course-0.0.2/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-24 06:32:50.000000 microlearn_gen_course-0.0.2/src/tests/test_answer_to_article_ques.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-24 06:32:50.000000 microlearn_gen_course-0.0.2/src/tests/test_gen_course_article_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-24 06:32:50.000000 microlearn_gen_course-0.0.2/src/tests/test_gen_course_articles_titles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-24 06:32:50.000000 microlearn_gen_course-0.0.2/src/tests/test_gen_course_metadata.py
```

### Comparing `microlearn_gen_course-0.0.1/.github/workflows/publish.yml` & `microlearn_gen_course-0.0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.1/PKG-INFO` & `microlearn_gen_course-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microlearn_gen_course
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package for generating microlearn course content
 Home-page: https://github.com/AIprojectflow/gen_course
 Project-URL: Bug Tracker, https://github.com/AIprojectflow/gen_course/issues
 Project-URL: Changelog, https://github.com/AIprojectflow/gen_course/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
```

### Comparing `microlearn_gen_course-0.0.1/setup.cfg` & `microlearn_gen_course-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.1/src/gen_course/gen_answer_to_article_ques.py` & `microlearn_gen_course-0.0.2/src/gen_course/gen_answer_to_article_ques.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.1/src/gen_course/gen_base.py` & `microlearn_gen_course-0.0.2/src/gen_course/gen_base.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.1/src/gen_course/gen_course_article_content.py` & `microlearn_gen_course-0.0.2/src/gen_course/gen_course_article_content.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.1/src/gen_course/gen_course_articles_titles.py` & `microlearn_gen_course-0.0.2/src/gen_course/gen_course_articles_titles.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.1/src/gen_course/gen_course_metadata.py` & `microlearn_gen_course-0.0.2/src/gen_course/gen_course_metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,37 +3,35 @@
 from pydantic import BaseModel, Field
 
 from .gen_base import GenBase
 
 
 class CourseMetadataModel(BaseModel):
     title: str = Field(
-        description="title of the course, where the length of the title is between 2 and 4 words")
+        description="title of the course of only 3 words")
     description: str = Field(
-        description="description of the course, where the length of the description is maximum of 150 words")
+        description="description of the course which is an introduction article of maximum 40 words")
 
 
 class GenCourseMetadata(GenBase):
     """
-    Generator class for course metadata(title, description, etc.).
+    Generator class for course metadata(title, description, etc.) using the description as text.
     """
-    HUMAN_PROMPT = """I'm developing a micro learning course about the following:
+    SYSTEM_PROMPT = """Act like a copywriter expert in course editing"""
+    HUMAN_PROMPT = """Write a title of only 3 words and an introduction article to a course of maximum 40 words based on the following:
 ---
-Title: {course_title}
 Description: {course_description}
 ---
-Rewrite the title and description for the course."""
+"""
 
     def __init__(self, llm, verbose: bool = False):
         super().__init__(llm, verbose)
 
     def get_output_parser(self):
         return PydanticOutputParser(pydantic_object=CourseMetadataModel)
 
     def generate(self,
-                 course_title: str,
                  course_description: str,
                  ) -> CourseMetadataModel:
         return self.generate_output(
-            course_title=course_title,
             course_description=course_description,
         )
```

### Comparing `microlearn_gen_course-0.0.1/src/microlearn_gen_course.egg-info/PKG-INFO` & `microlearn_gen_course-0.0.2/src/microlearn_gen_course.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microlearn-gen-course
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package for generating microlearn course content
 Home-page: https://github.com/AIprojectflow/gen_course
 Project-URL: Bug Tracker, https://github.com/AIprojectflow/gen_course/issues
 Project-URL: Changelog, https://github.com/AIprojectflow/gen_course/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
```

### Comparing `microlearn_gen_course-0.0.1/src/microlearn_gen_course.egg-info/SOURCES.txt` & `microlearn_gen_course-0.0.2/src/microlearn_gen_course.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.1/src/tests/test_answer_to_article_ques.py` & `microlearn_gen_course-0.0.2/src/tests/test_answer_to_article_ques.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.1/src/tests/test_gen_course_article_content.py` & `microlearn_gen_course-0.0.2/src/tests/test_gen_course_article_content.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.1/src/tests/test_gen_course_articles_titles.py` & `microlearn_gen_course-0.0.2/src/tests/test_gen_course_articles_titles.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.1/src/tests/test_gen_course_metadata.py` & `microlearn_gen_course-0.0.2/src/tests/test_gen_course_metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """
 Test GenCourseMetadata
 
 Usage:
     pytest src/tests/test_gen_course_metadata.py -v --log-cli-level INFO
 """
-import logging
 import sys
 from pathlib import Path
 sys.path.insert(0, str(Path(__file__).parent.parent))
 
-from dotenv import load_dotenv
-from gen_course.gen_course_metadata import GenCourseMetadata
-
 from llm_factory.llm_factory import LLMFactory
+from gen_course.gen_course_metadata import GenCourseMetadata
+from dotenv import load_dotenv
+import logging
 
 
 load_dotenv(override=True)
 
 logger = logging.getLogger(__name__)
 
 
@@ -25,14 +24,13 @@
         llm_type=LLMFactory.LLM_OPENAI_CHAT_NAME,
         model_name="gpt-4",
         temperature=0.0,
         max_tokens=256,
     )
     gen = GenCourseMetadata(llm=llm, verbose=True)
     output = gen.generate(
-        course_title="Python for Beginners",
-        course_description="Learn Python from scratch.",
+        course_description="Generate a course about Python programming language for beginners.",
     )
     logger.info(f"course's title: {output.title}")
     logger.info(f"course's description: {output.description}")
     assert len(output.title) >= 2 and len(output.title.split()) <= 4
-    assert len(output.description) <= 150
+    assert len(output.description.split()) <= 40
```

