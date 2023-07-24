# Comparing `tmp/megaladon-0.0.1.tar.gz` & `tmp/megaladon-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megaladon-0.0.1.tar", max compression
+gzip compressed data, was "megaladon-0.0.2.tar", max compression
```

## Comparing `megaladon-0.0.1.tar` & `megaladon-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0     3050 2023-07-24 20:45:14.833748 megaladon-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-24 20:21:50.706201 megaladon-0.0.1/megaladon/__init__.py
--rw-r--r--   0        0        0     2375 2023-07-24 21:02:53.857130 megaladon-0.0.1/megaladon/math.py
--rw-r--r--   0        0        0     7364 2023-07-24 20:34:39.913321 megaladon-0.0.1/megaladon/models.py
--rw-r--r--   0        0        0      841 2023-07-24 21:02:41.372183 megaladon-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3812 1970-01-01 00:00:00.000000 megaladon-0.0.1/setup.py
--rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 megaladon-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-24 20:21:50.706201 megaladon-0.0.2/Megaladon/__init__.py
+-rw-r--r--   0        0        0     2375 2023-07-24 21:04:28.565996 megaladon-0.0.2/Megaladon/math.py
+-rw-r--r--   0        0        0     7364 2023-07-24 20:34:39.913321 megaladon-0.0.2/Megaladon/models.py
+-rw-r--r--   0        0        0     3050 2023-07-24 21:04:28.565834 megaladon-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-24 20:21:50.706201 megaladon-0.0.2/megaladon/__init__.py
+-rw-r--r--   0        0        0     2375 2023-07-24 21:04:28.565996 megaladon-0.0.2/megaladon/math.py
+-rw-r--r--   0        0        0     7364 2023-07-24 20:34:39.913321 megaladon-0.0.2/megaladon/models.py
+-rw-r--r--   0        0        0      841 2023-07-24 21:05:02.259202 megaladon-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3812 1970-01-01 00:00:00.000000 megaladon-0.0.2/setup.py
+-rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 megaladon-0.0.2/PKG-INFO
```

### Comparing `megaladon-0.0.1/README.md` & `megaladon-0.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-# Megalodon
+# Megaladon
 Sail the Seas of Data and Dive into the Depths of Computation!  
-![Megalodon](megaladon.jpeg)
+![Megaladon](megaladon.jpeg)
 
-## _Megalodon: The Orca is no match._
+## _Megaladon: The Orca is no match._
 
-Welcome aboard, shipmates! Let Megalodon be your steadfast vessel on the uncharted ocean of Big Data and Machine Learning. With our rich datasets and detailed mathematical models, there's no computational storm we can't weather together! 
+Welcome aboard, shipmates! Let Megaladon be your steadfast vessel on the uncharted ocean of Big Data and Machine Learning. With our rich datasets and detailed mathematical models, there's no computational storm we can't weather together! 
 
-> "We didn't name it 'Megalodon' for nothing. It's big, it's powerful, and it's got a heck of a bite when it comes to data crunching!" - Captain Codebeard
+> "We didn't name it 'Megaladon' for nothing. It's big, it's powerful, and it's got a heck of a bite when it comes to data crunching!" - Captain Codebeard
 
 ## Navigation Chart
 
 ```python
 Dataset Sample (Row by Row) [Input] --(Feeds into)--> [Model] --(Outputs)--> Dataset Sample (Row by Row)
 ```
 
 # Deck Logs (Changelog)
 
 - **v2.0.0 - The Leviathan Update** - We've surfaced some serious computational power in this one! Modular integration of HuggingFace and OpenAI models.
 - **v1.5.0 - The Kraken Patch** - Tightened up the tentacles of the code. Fewer bugs will be slipping through!
-- **v1.0.0 - Maiden Voyage** - Initial launch! The Megalodon sets sail!
+- **v1.0.0 - Maiden Voyage** - Initial launch! The Megaladon sets sail!
 
 # Shipwright's Guide (Installation)
 
-Batten down the hatches and ready your terminal, it's time to summon the Megalodon:
+Batten down the hatches and ready your terminal, it's time to summon the Megaladon:
 
 ```bash
-git clone https://github.com/megalodon-ds/megalodon.git
-cd megalodon
+git clone https://github.com/Megaladon-ds/Megaladon.git
+cd Megaladon
 pip install -r requirements.txt
 ```
 
 # Navigational Tools (Usage)
 
 1. **Start your voyage with a good map.** (Load your dataset)
 
 ```python
-from megalodon import Megalodon
+from Megaladon import Megaladon
 
 # Using OpenAI model
-megalodon = Megalodon(model_id="gpt-3", api_key="your-api-key", dataset="flax-sentence-embeddings/stackexchange_math_jsonl")
+Megaladon = Megaladon(model_id="gpt-3", api_key="your-api-key", dataset="flax-sentence-embeddings/stackexchange_math_jsonl")
 
 # Using Hugging Face model
-megalodon = Megalodon(model_id="gpt2", dataset="flax-sentence-embeddings/stackexchange_math_jsonl")
+Megaladon = Megaladon(model_id="gpt2", dataset="flax-sentence-embeddings/stackexchange_math_jsonl")
 ```
 
 2. **Set sail!** (Generate explanations)
 
 ```python
-explanations = megalodon.run()
+explanations = Megaladon.run()
 ```
 
 3. **Return to port.** (Save your results)
 
 ```python
-megalodon.save_to_huggingface(explanations, 'hf_output_dir')
+Megaladon.save_to_huggingface(explanations, 'hf_output_dir')
 ```
 
 Please replace `"your-api-key"` with your actual OpenAI API key, and `'hf_output_dir'` with your desired output directory for the Hugging Face datasets.
 
 # Lifeboats (Support)
 
 If you find yourself overboard in a sea of confusion, don't panic! Shoot a flare to our issue tracker on Github, and our dedicated crew will row to your rescue. 
 
-[Create New Issue](https://github.com/megalodon-ds/megalodon/issues/new)
+[Create New Issue](https://github.com/Megaladon-ds/Megaladon/issues/new)
 
 # Crow's Nest (Future Plans)
 
-1. **New Species Detection** - We're constantly exploring unknown waters to find and integrate new algorithms and data models into Megalodon. 
-2. **Crew Training** - Comprehensive documentation and examples are on the horizon to help you get the most out of your voyage with Megalodon.
+1. **New Species Detection** - We're constantly exploring unknown waters to find and integrate new algorithms and data models into Megaladon. 
+2. **Crew Training** - Comprehensive documentation and examples are on the horizon to help you get the most out of your voyage with Megaladon.
 
-Thank you for choosing to sail with Megalodon. May fair winds and calm seas guide your data journey!
+Thank you for choosing to sail with Megaladon. May fair winds and calm seas guide your data journey!
 
 Happy Sailing!
 
-The Megalodon Team
+The Megaladon Team
 
 
 
 # Todo:
 
 * Better prompt
 * More seamless model handling, plug and play with any model from OpenAI or HuggingFace.
```

### Comparing `megaladon-0.0.1/megaladon/math.py` & `megaladon-0.0.2/Megaladon/math.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from datasets import load_dataset
 from datasets import load_dataset, DatasetDict, Dataset
 
 from Megaladon.models import OpenAILanguageModel, HuggingFaceLLM
 
-class Megalodon:
+class Megaladon:
     def __init__(self, model_id: str, api_key: str = None, dataset: str = None, prompt: str = None):
         self.api_key = api_key
 
         api_key = api_key or os.getenv("OPENAI_API_KEY") 
 
         self.dataset = load_dataset(dataset) if dataset else None
         self.prompt = prompt if prompt else "This text: {text} was upvoted/downvoted. Explain why in a simple, comprehensive manner."
@@ -50,15 +50,15 @@
 # TODO: Make it modular to plug in and play with any model openai or huggingface
 # TODO: Save to huggingface after each iteration is labelled
 # TODO: Potentially use parquet for optimized storage
 # TODO: Add in polymorphic or shape shifting preprocesing logi 
 
 
 # # Using OpenAI model
-# megalodon = Megalodon(model_id="gpt-3", api_key="your-api-key", dataset="flax-sentence-embeddings/stackexchange_math_jsonl")
-# explanations = megalodon.run()
-# megalodon.save_to_huggingface(explanations, 'hf_output_dir')
+# Megaladon = Megaladon(model_id="gpt-3", api_key="your-api-key", dataset="flax-sentence-embeddings/stackexchange_math_jsonl")
+# explanations = Megaladon.run()
+# Megaladon.save_to_huggingface(explanations, 'hf_output_dir')
 
 # # Using Hugging Face model
-# megalodon = Megalodon(model_id="gpt2", dataset="flax-sentence-embeddings/stackexchange_math_jsonl")
-# explanations = megalodon.run()
-# megalodon.save_to_huggingface(explanations, 'hf_output_dir')
+# Megaladon = Megaladon(model_id="gpt2", dataset="flax-sentence-embeddings/stackexchange_math_jsonl")
+# explanations = Megaladon.run()
+# Megaladon.save_to_huggingface(explanations, 'hf_output_dir')
```

### Comparing `megaladon-0.0.1/megaladon/models.py` & `megaladon-0.0.2/Megaladon/models.py`

 * *Files identical despite different names*

### Comparing `megaladon-0.0.1/pyproject.toml` & `megaladon-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "Megaladon"
-version = "0.0.1"
-description = "Megalodon - Pytorch"
+version = "0.0.2"
+description = "Megaladon - Pytorch"
 authors = ["Kye Gomez <kye@apac.ai>"]
 license = "MIT"
 readme = "README.md"  # assuming you have a README.md file
-homepage = "https://github.com/Agora-X/Megalodon"
+homepage = "https://github.com/Agora-X/Megaladon"
 keywords = ["artificial intelligence", "attention mechanism", "transformers"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.6",
 ]
 
-include = ["megalodon/**/*"]
+include = ["Megaladon/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 transformers = "*"
 datasets = "*"
 deepspeed = "*"
 openai = "*"
```

### Comparing `megaladon-0.0.1/setup.py` & `megaladon-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 {'': ['*']}
 
 install_requires = \
 ['datasets', 'deepspeed', 'openai', 'transformers']
 
 setup_kwargs = {
     'name': 'megaladon',
-    'version': '0.0.1',
-    'description': 'Megalodon - Pytorch',
-    'long_description': '# Megalodon\nSail the Seas of Data and Dive into the Depths of Computation!  \n![Megalodon](megaladon.jpeg)\n\n## _Megalodon: The Orca is no match._\n\nWelcome aboard, shipmates! Let Megalodon be your steadfast vessel on the uncharted ocean of Big Data and Machine Learning. With our rich datasets and detailed mathematical models, there\'s no computational storm we can\'t weather together! \n\n> "We didn\'t name it \'Megalodon\' for nothing. It\'s big, it\'s powerful, and it\'s got a heck of a bite when it comes to data crunching!" - Captain Codebeard\n\n## Navigation Chart\n\n```python\nDataset Sample (Row by Row) [Input] --(Feeds into)--> [Model] --(Outputs)--> Dataset Sample (Row by Row)\n```\n\n# Deck Logs (Changelog)\n\n- **v2.0.0 - The Leviathan Update** - We\'ve surfaced some serious computational power in this one! Modular integration of HuggingFace and OpenAI models.\n- **v1.5.0 - The Kraken Patch** - Tightened up the tentacles of the code. Fewer bugs will be slipping through!\n- **v1.0.0 - Maiden Voyage** - Initial launch! The Megalodon sets sail!\n\n# Shipwright\'s Guide (Installation)\n\nBatten down the hatches and ready your terminal, it\'s time to summon the Megalodon:\n\n```bash\ngit clone https://github.com/megalodon-ds/megalodon.git\ncd megalodon\npip install -r requirements.txt\n```\n\n# Navigational Tools (Usage)\n\n1. **Start your voyage with a good map.** (Load your dataset)\n\n```python\nfrom megalodon import Megalodon\n\n# Using OpenAI model\nmegalodon = Megalodon(model_id="gpt-3", api_key="your-api-key", dataset="flax-sentence-embeddings/stackexchange_math_jsonl")\n\n# Using Hugging Face model\nmegalodon = Megalodon(model_id="gpt2", dataset="flax-sentence-embeddings/stackexchange_math_jsonl")\n```\n\n2. **Set sail!** (Generate explanations)\n\n```python\nexplanations = megalodon.run()\n```\n\n3. **Return to port.** (Save your results)\n\n```python\nmegalodon.save_to_huggingface(explanations, \'hf_output_dir\')\n```\n\nPlease replace `"your-api-key"` with your actual OpenAI API key, and `\'hf_output_dir\'` with your desired output directory for the Hugging Face datasets.\n\n# Lifeboats (Support)\n\nIf you find yourself overboard in a sea of confusion, don\'t panic! Shoot a flare to our issue tracker on Github, and our dedicated crew will row to your rescue. \n\n[Create New Issue](https://github.com/megalodon-ds/megalodon/issues/new)\n\n# Crow\'s Nest (Future Plans)\n\n1. **New Species Detection** - We\'re constantly exploring unknown waters to find and integrate new algorithms and data models into Megalodon. \n2. **Crew Training** - Comprehensive documentation and examples are on the horizon to help you get the most out of your voyage with Megalodon.\n\nThank you for choosing to sail with Megalodon. May fair winds and calm seas guide your data journey!\n\nHappy Sailing!\n\nThe Megalodon Team\n\n\n\n# Todo:\n\n* Better prompt\n* More seamless model handling, plug and play with any model from OpenAI or HuggingFace.\n* Save to HuggingFace after each iteration is labeled\n* Potentially use Parquet for optimized storage\n* Add in polymorphic or shape shifting preprocessing logic\n',
+    'version': '0.0.2',
+    'description': 'Megaladon - Pytorch',
+    'long_description': '# Megaladon\nSail the Seas of Data and Dive into the Depths of Computation!  \n![Megaladon](megaladon.jpeg)\n\n## _Megaladon: The Orca is no match._\n\nWelcome aboard, shipmates! Let Megaladon be your steadfast vessel on the uncharted ocean of Big Data and Machine Learning. With our rich datasets and detailed mathematical models, there\'s no computational storm we can\'t weather together! \n\n> "We didn\'t name it \'Megaladon\' for nothing. It\'s big, it\'s powerful, and it\'s got a heck of a bite when it comes to data crunching!" - Captain Codebeard\n\n## Navigation Chart\n\n```python\nDataset Sample (Row by Row) [Input] --(Feeds into)--> [Model] --(Outputs)--> Dataset Sample (Row by Row)\n```\n\n# Deck Logs (Changelog)\n\n- **v2.0.0 - The Leviathan Update** - We\'ve surfaced some serious computational power in this one! Modular integration of HuggingFace and OpenAI models.\n- **v1.5.0 - The Kraken Patch** - Tightened up the tentacles of the code. Fewer bugs will be slipping through!\n- **v1.0.0 - Maiden Voyage** - Initial launch! The Megaladon sets sail!\n\n# Shipwright\'s Guide (Installation)\n\nBatten down the hatches and ready your terminal, it\'s time to summon the Megaladon:\n\n```bash\ngit clone https://github.com/Megaladon-ds/Megaladon.git\ncd Megaladon\npip install -r requirements.txt\n```\n\n# Navigational Tools (Usage)\n\n1. **Start your voyage with a good map.** (Load your dataset)\n\n```python\nfrom Megaladon import Megaladon\n\n# Using OpenAI model\nMegaladon = Megaladon(model_id="gpt-3", api_key="your-api-key", dataset="flax-sentence-embeddings/stackexchange_math_jsonl")\n\n# Using Hugging Face model\nMegaladon = Megaladon(model_id="gpt2", dataset="flax-sentence-embeddings/stackexchange_math_jsonl")\n```\n\n2. **Set sail!** (Generate explanations)\n\n```python\nexplanations = Megaladon.run()\n```\n\n3. **Return to port.** (Save your results)\n\n```python\nMegaladon.save_to_huggingface(explanations, \'hf_output_dir\')\n```\n\nPlease replace `"your-api-key"` with your actual OpenAI API key, and `\'hf_output_dir\'` with your desired output directory for the Hugging Face datasets.\n\n# Lifeboats (Support)\n\nIf you find yourself overboard in a sea of confusion, don\'t panic! Shoot a flare to our issue tracker on Github, and our dedicated crew will row to your rescue. \n\n[Create New Issue](https://github.com/Megaladon-ds/Megaladon/issues/new)\n\n# Crow\'s Nest (Future Plans)\n\n1. **New Species Detection** - We\'re constantly exploring unknown waters to find and integrate new algorithms and data models into Megaladon. \n2. **Crew Training** - Comprehensive documentation and examples are on the horizon to help you get the most out of your voyage with Megaladon.\n\nThank you for choosing to sail with Megaladon. May fair winds and calm seas guide your data journey!\n\nHappy Sailing!\n\nThe Megaladon Team\n\n\n\n# Todo:\n\n* Better prompt\n* More seamless model handling, plug and play with any model from OpenAI or HuggingFace.\n* Save to HuggingFace after each iteration is labeled\n* Potentially use Parquet for optimized storage\n* Add in polymorphic or shape shifting preprocessing logic\n',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://github.com/Agora-X/Megalodon',
+    'url': 'https://github.com/Agora-X/Megaladon',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.6,<4.0',
 }
```

### Comparing `megaladon-0.0.1/PKG-INFO` & `megaladon-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: megaladon
-Version: 0.0.1
-Summary: Megalodon - Pytorch
-Home-page: https://github.com/Agora-X/Megalodon
+Version: 0.0.2
+Summary: Megaladon - Pytorch
+Home-page: https://github.com/Agora-X/Megaladon
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -22,90 +22,90 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: datasets
 Requires-Dist: deepspeed
 Requires-Dist: openai
 Requires-Dist: transformers
 Description-Content-Type: text/markdown
 
-# Megalodon
+# Megaladon
 Sail the Seas of Data and Dive into the Depths of Computation!  
-![Megalodon](megaladon.jpeg)
+![Megaladon](megaladon.jpeg)
 
-## _Megalodon: The Orca is no match._
+## _Megaladon: The Orca is no match._
 
-Welcome aboard, shipmates! Let Megalodon be your steadfast vessel on the uncharted ocean of Big Data and Machine Learning. With our rich datasets and detailed mathematical models, there's no computational storm we can't weather together! 
+Welcome aboard, shipmates! Let Megaladon be your steadfast vessel on the uncharted ocean of Big Data and Machine Learning. With our rich datasets and detailed mathematical models, there's no computational storm we can't weather together! 
 
-> "We didn't name it 'Megalodon' for nothing. It's big, it's powerful, and it's got a heck of a bite when it comes to data crunching!" - Captain Codebeard
+> "We didn't name it 'Megaladon' for nothing. It's big, it's powerful, and it's got a heck of a bite when it comes to data crunching!" - Captain Codebeard
 
 ## Navigation Chart
 
 ```python
 Dataset Sample (Row by Row) [Input] --(Feeds into)--> [Model] --(Outputs)--> Dataset Sample (Row by Row)
 ```
 
 # Deck Logs (Changelog)
 
 - **v2.0.0 - The Leviathan Update** - We've surfaced some serious computational power in this one! Modular integration of HuggingFace and OpenAI models.
 - **v1.5.0 - The Kraken Patch** - Tightened up the tentacles of the code. Fewer bugs will be slipping through!
-- **v1.0.0 - Maiden Voyage** - Initial launch! The Megalodon sets sail!
+- **v1.0.0 - Maiden Voyage** - Initial launch! The Megaladon sets sail!
 
 # Shipwright's Guide (Installation)
 
-Batten down the hatches and ready your terminal, it's time to summon the Megalodon:
+Batten down the hatches and ready your terminal, it's time to summon the Megaladon:
 
 ```bash
-git clone https://github.com/megalodon-ds/megalodon.git
-cd megalodon
+git clone https://github.com/Megaladon-ds/Megaladon.git
+cd Megaladon
 pip install -r requirements.txt
 ```
 
 # Navigational Tools (Usage)
 
 1. **Start your voyage with a good map.** (Load your dataset)
 
 ```python
-from megalodon import Megalodon
+from Megaladon import Megaladon
 
 # Using OpenAI model
-megalodon = Megalodon(model_id="gpt-3", api_key="your-api-key", dataset="flax-sentence-embeddings/stackexchange_math_jsonl")
+Megaladon = Megaladon(model_id="gpt-3", api_key="your-api-key", dataset="flax-sentence-embeddings/stackexchange_math_jsonl")
 
 # Using Hugging Face model
-megalodon = Megalodon(model_id="gpt2", dataset="flax-sentence-embeddings/stackexchange_math_jsonl")
+Megaladon = Megaladon(model_id="gpt2", dataset="flax-sentence-embeddings/stackexchange_math_jsonl")
 ```
 
 2. **Set sail!** (Generate explanations)
 
 ```python
-explanations = megalodon.run()
+explanations = Megaladon.run()
 ```
 
 3. **Return to port.** (Save your results)
 
 ```python
-megalodon.save_to_huggingface(explanations, 'hf_output_dir')
+Megaladon.save_to_huggingface(explanations, 'hf_output_dir')
 ```
 
 Please replace `"your-api-key"` with your actual OpenAI API key, and `'hf_output_dir'` with your desired output directory for the Hugging Face datasets.
 
 # Lifeboats (Support)
 
 If you find yourself overboard in a sea of confusion, don't panic! Shoot a flare to our issue tracker on Github, and our dedicated crew will row to your rescue. 
 
-[Create New Issue](https://github.com/megalodon-ds/megalodon/issues/new)
+[Create New Issue](https://github.com/Megaladon-ds/Megaladon/issues/new)
 
 # Crow's Nest (Future Plans)
 
-1. **New Species Detection** - We're constantly exploring unknown waters to find and integrate new algorithms and data models into Megalodon. 
-2. **Crew Training** - Comprehensive documentation and examples are on the horizon to help you get the most out of your voyage with Megalodon.
+1. **New Species Detection** - We're constantly exploring unknown waters to find and integrate new algorithms and data models into Megaladon. 
+2. **Crew Training** - Comprehensive documentation and examples are on the horizon to help you get the most out of your voyage with Megaladon.
 
-Thank you for choosing to sail with Megalodon. May fair winds and calm seas guide your data journey!
+Thank you for choosing to sail with Megaladon. May fair winds and calm seas guide your data journey!
 
 Happy Sailing!
 
-The Megalodon Team
+The Megaladon Team
 
 
 
 # Todo:
 
 * Better prompt
 * More seamless model handling, plug and play with any model from OpenAI or HuggingFace.
```

