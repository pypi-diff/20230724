# Comparing `tmp/commonbase-0.1.0.tar.gz` & `tmp/commonbase-0.1.1.tar.gz`

## Comparing `commonbase-0.1.0.tar` & `commonbase-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 commonbase-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 commonbase-0.1.0/commonbase/__init__.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 commonbase-0.1.0/commonbase/completion.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 commonbase-0.1.0/commonbase/completion_response.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 commonbase-0.1.0/commonbase/exceptions.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 commonbase-0.1.0/commonbase/tests/__init__.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 commonbase-0.1.0/commonbase/tests/test_completion.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 commonbase-0.1.0/examples/completion.ipynb
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 commonbase-0.1.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 commonbase-0.1.0/LICENSE
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 commonbase-0.1.0/README.md
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 commonbase-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 commonbase-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 commonbase-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 commonbase-0.1.1/commonbase/__init__.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 commonbase-0.1.1/commonbase/completion.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 commonbase-0.1.1/commonbase/completion_response.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 commonbase-0.1.1/commonbase/exceptions.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 commonbase-0.1.1/commonbase/tests/__init__.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 commonbase-0.1.1/commonbase/tests/test_completion.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 commonbase-0.1.1/examples/completion.ipynb
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 commonbase-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 commonbase-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 commonbase-0.1.1/README.md
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 commonbase-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 commonbase-0.1.1/PKG-INFO
```

### Comparing `commonbase-0.1.0/.github/workflows/python-publish.yml` & `commonbase-0.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `commonbase-0.1.0/commonbase/completion_response.py` & `commonbase-0.1.1/commonbase/completion_response.py`

 * *Files identical despite different names*

### Comparing `commonbase-0.1.0/commonbase/tests/test_completion.py` & `commonbase-0.1.1/commonbase/tests/test_completion.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,7 +40,20 @@
 def test_completion_response():
     result = commonbase.Completion.create(
         project_id=os.getenv("CB_PROJECT_ID"),
         prompt="Please return the string '123abc' to me without the quotes.",
     )
 
     assert result.completed and result.choices[0].text.strip() == "123abc"
+
+
+def test_completion_stream():
+    response_count = 0
+
+    for response in commonbase.Completion.stream(
+        project_id=os.getenv("CB_PROJECT_ID"),
+        prompt="Tell me about artificial intelligence.",
+    ):
+        assert len(response.choices) > 0 and response.choices[0].text is not None
+        response_count += 1
+
+    assert response_count > 0
```

### Comparing `commonbase-0.1.0/examples/completion.ipynb` & `commonbase-0.1.1/examples/completion.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9541666666666666%*

 * *Differences: {"'cells'": "{3: {'execution_count': None, 'outputs': []}, insert: [(4, OrderedDict([('cell_type', "*

 * *            "'markdown'), ('metadata', OrderedDict()), ('source', ['Use `Completion.stream` to "*

 * *            "stream a completion response.'])])), (5, OrderedDict([('cell_type', 'code'), "*

 * *            "('execution_count', None), ('metadata', OrderedDict()), ('outputs', []), ('source', "*

 * *            '[\'import commonbase\\n\', \'\\n\', \'project_id="<YOUR PROJECT_ID>"\\n\', \'\\n\', '*

 * *            '\'result =  […]*

```diff
@@ -29,36 +29,49 @@
                 "A project ID is required for all Commonbase requests. You can find your project ID in the [Commonbase Dashboard](https://commonbase.com/test-50727/project/test/overview).\n",
                 "\n",
                 "To create a completion, provide your project ID and prompt to the `Completion.create` class method."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "\n",
-                        "\n",
-                        "It was nice to meet you. It is always nice to make new connections. I hope you have a great day!\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "import commonbase\n",
                 "\n",
                 "project_id=\"<YOUR PROJECT ID>\"\n",
                 "\n",
                 "result = commonbase.Completion.create(project_id=project_id, prompt=\"Hello!\")\n",
                 "\n",
                 "print(result.choices[0].text)"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Use `Completion.stream` to stream a completion response."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "import commonbase\n",
+                "\n",
+                "project_id=\"<YOUR PROJECT_ID>\"\n",
+                "\n",
+                "result = commonbase.Completion.stream(project_id=project_id, prompt=\"Write me a short essay about artificial intelligence.\")\n",
+                "\n",
+                "for completion in result:\n",
+                "    print(completion.choices[0].text, end=\"\")"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `commonbase-0.1.0/.gitignore` & `commonbase-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `commonbase-0.1.0/LICENSE` & `commonbase-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commonbase-0.1.0/PKG-INFO` & `commonbase-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonbase
-Version: 0.1.0
+Version: 0.1.1
 Summary: Commonbase Python SDK
 Project-URL: Homepage, https://github.com/commonbaseapp/commonbase-python
 Project-URL: Source, https://github.com/commonbaseapp/commonbase-python
 Project-URL: Tracker, https://github.com/commonbaseapp/commonbase-python/issues
 License: MIT License
         
         Copyright (c) 2023 Commonbase
@@ -25,30 +25,51 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: requests>=2.31.0
+Requires-Dist: sseclient-py>=1.7.2
 Description-Content-Type: text/markdown
 
 # Commonbase Python SDK
 
 Commonbase allows developers to integrate with any popular LLM API provider without needing to change any code. The SDK helps with collecting data and feedback from the users and helps you fine-tune models for your specific use case.
 
 ## Installation
 
 ```
 pip install commonbase
 ```
 
 ## Usage
 
+A project ID is required for all Commonbase requests. You can find your project ID in the [Commonbase Dashboard](https://commonbase.com/test-50727/project/test/overview).
+
+To create a completion, provide your project ID and prompt to the `Completion.create` class method.
+
 ```py
 import commonbase
 
 project_id="XXXXXXXX-XXXXXXXX-XXXXXXXX-XXXXXXXX"
 
 result = commonbase.Completion.create(project_id=project_id, prompt="Hello!")
 
 print(result.choices[0].text)
 ```
+
+Use `Completion.stream` to stream a completion response.
+
+```py
+import commonbase
+
+project_id="XXXXXXXX-XXXXXXXX-XXXXXXXX-XXXXXXXX"
+
+result = commonbase.Completion.stream(
+    project_id=project_id,
+    prompt="Write me a short essay about artificial intelligence."
+)
+
+for completion in result:
+    print(completion.choices[0].text, end="")
+```
```

