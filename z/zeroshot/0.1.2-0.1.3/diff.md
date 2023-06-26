# Comparing `tmp/zeroshot-0.1.2.tar.gz` & `tmp/zeroshot-0.1.3.tar.gz`

## Comparing `zeroshot-0.1.2.tar` & `zeroshot-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeroshot-0.1.2/.git
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 zeroshot-0.1.2/requirements.txt
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 zeroshot-0.1.2/requirements_dev.txt
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 zeroshot-0.1.2/.github/workflows/integration_python.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 zeroshot-0.1.2/.github/workflows/lint_python.yml
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 zeroshot-0.1.2/.github/workflows/test_python.yml
--rw-r--r--   0        0        0   650834 2020-02-02 00:00:00.000000 zeroshot-0.1.2/examples/run_classification.ipynb
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 zeroshot-0.1.2/scripts/integration_test.py
--rw-r--r--   0        0        0   448620 2020-02-02 00:00:00.000000 zeroshot-0.1.2/scripts/test_files/giraffe.png
--rw-r--r--   0        0        0    33317 2020-02-02 00:00:00.000000 zeroshot-0.1.2/scripts/test_files/test_model.json
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 zeroshot-0.1.2/zeroshot/__init__.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 zeroshot-0.1.2/zeroshot/classifier.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 zeroshot-0.1.2/zeroshot/classifier_test.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 zeroshot-0.1.2/zeroshot/downloader.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 zeroshot-0.1.2/zeroshot/downloader_test.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 zeroshot-0.1.2/zeroshot/feature_extractor.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 zeroshot-0.1.2/zeroshot/feature_extractor_test.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 zeroshot-0.1.2/zeroshot/logistic_regression.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 zeroshot-0.1.2/zeroshot/logistic_regression_test.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 zeroshot-0.1.2/zeroshot/preprocessing.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 zeroshot-0.1.2/zeroshot/utils.py
--rw-r--r--   0        0        0    40312 2020-02-02 00:00:00.000000 zeroshot-0.1.2/zeroshot/test_files/test_model.json
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 zeroshot-0.1.2/.gitignore
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 zeroshot-0.1.2/README.md
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 zeroshot-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 zeroshot-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeroshot-0.1.3/.git
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 zeroshot-0.1.3/requirements.txt
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 zeroshot-0.1.3/requirements_dev.txt
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 zeroshot-0.1.3/.github/workflows/integration_python.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 zeroshot-0.1.3/.github/workflows/lint_python.yml
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 zeroshot-0.1.3/.github/workflows/test_python.yml
+-rw-r--r--   0        0        0   651012 2020-02-02 00:00:00.000000 zeroshot-0.1.3/examples/run_classification.ipynb
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 zeroshot-0.1.3/scripts/integration_test.py
+-rw-r--r--   0        0        0   448620 2020-02-02 00:00:00.000000 zeroshot-0.1.3/scripts/test_files/giraffe.png
+-rw-r--r--   0        0        0    33317 2020-02-02 00:00:00.000000 zeroshot-0.1.3/scripts/test_files/test_model.json
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/__init__.py
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/classifier.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/classifier_test.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/downloader.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/downloader_test.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/feature_extractor.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/feature_extractor_test.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/logistic_regression.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/logistic_regression_test.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/preprocessing.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/utils.py
+-rw-r--r--   0        0        0    40312 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/test_files/test_model.json
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 zeroshot-0.1.3/.gitignore
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 zeroshot-0.1.3/README.md
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 zeroshot-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 zeroshot-0.1.3/PKG-INFO
```

### Comparing `zeroshot-0.1.2/.github/workflows/integration_python.yml` & `zeroshot-0.1.3/.github/workflows/integration_python.yml`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.2/.github/workflows/lint_python.yml` & `zeroshot-0.1.3/.github/workflows/lint_python.yml`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.2/.github/workflows/test_python.yml` & `zeroshot-0.1.3/.github/workflows/test_python.yml`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.2/examples/run_classification.ipynb` & `zeroshot-0.1.3/examples/run_classification.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9149725274725274%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(3, 'model = "*

 * *            'zeroshot.Classifier("d2570afb-2be7-4798-8931-ed62a5340fff")\\n\'), (5, \'# Run the '*

 * *            "model! The result is the index of the prediction.\\n'), (6, 'result = "*

 * *            "model.predict(dog_url)\\n'), (7, 'class_name = model.classes[result]\\n')], delete: "*

 * *            "[7, 6, 5, 3]}}, 6: {'source': {insert: [(7, 'classifier = zeroshot.Classifier(\\n'), "*

 * *            '(8, \'    "d2570afb-2be7-4798-8931-ed62a5340fff", preprocessor=N […]*

```diff
@@ -52,19 +52,19 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import zeroshot\n",
                 "\n",
                 "# Create the classifier with the model we've created on usezeroshot.com\n",
-                "classifier = zeroshot.Classifier(\"d2570afb-2be7-4798-8931-ed62a5340fff\")\n",
+                "model = zeroshot.Classifier(\"d2570afb-2be7-4798-8931-ed62a5340fff\")\n",
                 "\n",
-                "# Run the model!\n",
-                "prediction = classifier.predict(dog_url)\n",
-                "class_name = classifier.class_list[prediction]\n",
+                "# Run the model! The result is the index of the prediction.\n",
+                "result = model.predict(dog_url)\n",
+                "class_name = model.classes[result]\n",
                 "print(f'The image is class \"{class_name}\"')"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -82,28 +82,35 @@
                 "import zeroshot\n",
                 "\n",
                 "# You can pull out the pre-processing function. This is useful in case your\n",
                 "# images are already in a ImageNet standardized format or something similar.\n",
                 "preprocess_fn = zeroshot.create_preprocess_fn()\n",
                 "\n",
                 "# Create the classifier and preprocessing function.\n",
-                "classifier = zeroshot.Classifier(\"d2570afb-2be7-4798-8931-ed62a5340fff\", preprocessor=None)\n",
+                "classifier = zeroshot.Classifier(\n",
+                "    \"d2570afb-2be7-4798-8931-ed62a5340fff\", preprocessor=None\n",
+                ")\n",
                 "\n",
                 "# Get predictions.\n",
+                "image = zeroshot.numpy_from_url(dog_url)\n",
                 "prediction = classifier.predict_proba(preprocess_fn(image))\n",
-                "classes = classifier.class_list\n",
+                "classes = classifier.classes\n",
                 "\n",
                 "print(\"Probabilities:\")\n",
                 "for pred, cls in zip(prediction, classes):\n",
                 "    print(f\"\\t{cls}: {pred:.2%}\")"
             ]
         }
     ],
     "metadata": {
+        "kernelspec": {
+            "display_name": "Python 3 (ipykernel)",
+            "language": "python",
+            "name": "python3"
+        },
         "language_info": {
             "name": "python"
-        },
-        "orig_nbformat": 4
+        }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `zeroshot-0.1.2/scripts/integration_test.py` & `zeroshot-0.1.3/scripts/integration_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 def run_test(target: str, classifier: Any) -> None:
     # Run the classifier.
     prediction = classifier.predict(target)
     prediction_probs = classifier.predict_proba(target)
 
     # Print the results.
-    prediction_str = classifier.class_list[prediction]
+    prediction_str = classifier.classes[prediction]
     print(f"Predicted class: {prediction_str}")
 
-    probabilities_str = zip(classifier.class_list, prediction_probs)
+    probabilities_str = zip(classifier.classes, prediction_probs)
     print(f"Predicted probabilities:")
     for class_name, probability in probabilities_str:
         if prediction_str == class_name:
             print("\033[1m", end="")
         print(f"\t{class_name}: {probability:.2%}")
         if prediction_str == class_name:
             print("\033[0m", end="")
```

### Comparing `zeroshot-0.1.2/scripts/test_files/giraffe.png` & `zeroshot-0.1.3/scripts/test_files/giraffe.png`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.2/scripts/test_files/test_model.json` & `zeroshot-0.1.3/scripts/test_files/test_model.json`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.2/zeroshot/classifier.py` & `zeroshot-0.1.3/zeroshot/classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 class Classifier(object):
     def _load_from_data(self, data: dict) -> None:
         # Load the model
         self.linear_model = LogisticRegression(
             coefs=np.array(data["coefficients"]), intercept=np.array(data["intercepts"])
         )
-        self.class_list = data["class_list"]
+        self.classes = data["class_list"]
         self.feature_extractor_name = data["feature_extractor"]
 
         self.feature_extractor = DINOV2FeatureExtractor(self.feature_extractor_name)
 
     def _features_from_str(self, image: Union[str, np.ndarray]) -> np.ndarray:
         """Generate feature vector from a string."""
         if isinstance(image, str) and image.startswith("http"):
```

### Comparing `zeroshot-0.1.2/zeroshot/classifier_test.py` & `zeroshot-0.1.3/zeroshot/classifier_test.py`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.2/zeroshot/downloader.py` & `zeroshot-0.1.3/zeroshot/downloader.py`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.2/zeroshot/downloader_test.py` & `zeroshot-0.1.3/zeroshot/downloader_test.py`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.2/zeroshot/feature_extractor.py` & `zeroshot-0.1.3/zeroshot/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.2/zeroshot/feature_extractor_test.py` & `zeroshot-0.1.3/zeroshot/feature_extractor_test.py`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.2/zeroshot/logistic_regression.py` & `zeroshot-0.1.3/zeroshot/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.2/zeroshot/logistic_regression_test.py` & `zeroshot-0.1.3/zeroshot/logistic_regression_test.py`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.2/zeroshot/preprocessing.py` & `zeroshot-0.1.3/zeroshot/preprocessing.py`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.2/zeroshot/utils.py` & `zeroshot-0.1.3/zeroshot/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Optional, Union
 
 import numpy as np
 import requests
 from PIL import Image
 
 
-def _from_data_or_path(input: Union[str, bytes]) -> dict[str, Any]:
+def _from_data_or_path(input: Union[str, io.BytesIO]) -> np.ndarray:
     """Loads the model from either a path or data."""
     img = Image.open(input)
     img = img.convert("RGB")
     img_data = np.array(img)
 
     return img_data
```

### Comparing `zeroshot-0.1.2/zeroshot/test_files/test_model.json` & `zeroshot-0.1.3/zeroshot/test_files/test_model.json`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.2/.gitignore` & `zeroshot-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.2/README.md` & `zeroshot-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.2/pyproject.toml` & `zeroshot-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zeroshot"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     {name = "Zeroshot Maintainers", email = "hello@usezeroshot.com"},
 ]
 description = "Image classifier with zero-shot learning."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `zeroshot-0.1.2/PKG-INFO` & `zeroshot-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroshot
-Version: 0.1.2
+Version: 0.1.3
 Summary: Image classifier with zero-shot learning.
 Project-URL: Homepage, https://github.com/moonshinelabs/zeroshot-python
 Author-email: Zeroshot Maintainers <hello@usezeroshot.com>
 Keywords: classifier,cv,zeroshot
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

