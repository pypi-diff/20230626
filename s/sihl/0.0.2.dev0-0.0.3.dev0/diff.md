# Comparing `tmp/sihl-0.0.2.dev0.tar.gz` & `tmp/sihl-0.0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sihl-0.0.2.dev0.tar", max compression
+gzip compressed data, was "sihl-0.0.3.dev0.tar", max compression
```

## Comparing `sihl-0.0.2.dev0.tar` & `sihl-0.0.3.dev0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1063 2023-05-20 16:08:12.727536 sihl-0.0.2.dev0/LICENSE
--rw-r--r--   0        0        0      897 2023-05-20 16:08:25.023681 sihl-0.0.2.dev0/README.md
--rw-r--r--   0        0        0     1334 2023-05-20 16:08:25.027681 sihl-0.0.2.dev0/pyproject.toml
--rw-r--r--   0        0        0      233 2023-05-20 16:08:25.027681 sihl-0.0.2.dev0/src/sihl/heads/__init__.py
--rw-r--r--   0        0        0     2237 2023-05-20 16:08:25.027681 sihl-0.0.2.dev0/src/sihl/heads/binary_classification.py
--rw-r--r--   0        0        0     2832 2023-05-20 16:08:25.027681 sihl-0.0.2.dev0/src/sihl/heads/multiclass_classification.py
--rw-r--r--   0        0        0     2630 2023-05-20 16:08:25.027681 sihl-0.0.2.dev0/src/sihl/heads/multilabel_classification.py
--rw-r--r--   0        0        0     2936 2023-05-20 16:08:25.027681 sihl-0.0.2.dev0/src/sihl/lightning_module.py
--rw-r--r--   0        0        0     6170 2023-05-20 16:08:25.027681 sihl-0.0.2.dev0/src/sihl/torchvision_backbone.py
--rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 sihl-0.0.2.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-26 10:00:27.512373 sihl-0.0.3.dev0/LICENSE
+-rw-r--r--   0        0        0      894 2023-06-26 10:00:44.648576 sihl-0.0.3.dev0/README.md
+-rw-r--r--   0        0        0     1487 2023-06-26 10:00:44.652576 sihl-0.0.3.dev0/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-06-26 10:00:44.652576 sihl-0.0.3.dev0/src/sihl/__init__.py
+-rw-r--r--   0        0        0   402648 2023-06-26 10:00:44.656576 sihl-0.0.3.dev0/src/sihl/heads/NotoSansMono-Bold.ttf
+-rw-r--r--   0        0        0      233 2023-06-26 10:00:27.520373 sihl-0.0.3.dev0/src/sihl/heads/__init__.py
+-rw-r--r--   0        0        0     3148 2023-06-26 10:00:44.656576 sihl-0.0.3.dev0/src/sihl/heads/binary_classification.py
+-rw-r--r--   0        0        0     3802 2023-06-26 10:00:44.656576 sihl-0.0.3.dev0/src/sihl/heads/multiclass_classification.py
+-rw-r--r--   0        0        0     4658 2023-06-26 10:00:44.656576 sihl-0.0.3.dev0/src/sihl/heads/multilabel_classification.py
+-rw-r--r--   0        0        0     3424 2023-06-26 10:00:44.656576 sihl-0.0.3.dev0/src/sihl/lightning_module.py
+-rw-r--r--   0        0        0     6156 2023-06-26 10:00:44.656576 sihl-0.0.3.dev0/src/sihl/torchvision_backbone.py
+-rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 sihl-0.0.3.dev0/PKG-INFO
```

### Comparing `sihl-0.0.2.dev0/LICENSE` & `sihl-0.0.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sihl-0.0.2.dev0/README.md` & `sihl-0.0.3.dev0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Simple Image Heads and Layers
 
 [![PyPI](https://img.shields.io/pypi/v/sihl.svg)][pypi_]
 [![python versions](https://img.shields.io/pypi/pyversions/sihl)][python version]
 [![coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/jonregef/c203d6bce2a485ab49d1814ff3218a06/raw/covbadge.json)][coverage]
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+[![ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)][ruff]
 
 [pypi_]: https://pypi.org/project/sihl/
 [python version]: https://pypi.org/project/sihl
 [coverage]: https://coverage.readthedocs.io/en/7.2.5/
-[pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
+[ruff]: https://github.com/astral-sh/ruff
 
 ## Installation
 
 ```console
 pip install sihl
 ```
```

### Comparing `sihl-0.0.2.dev0/pyproject.toml` & `sihl-0.0.3.dev0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 [tool.poetry]
 name = "sihl"
-version = "0.0.2-dev"
+version = "0.0.3-dev"
 description = "Simple Image Heads and Layers"
 authors = ["jonregef <jon.regef@pm.me>"]
 readme = "README.md"
 license = "MIT"
 # homepage = "https://github.com/sihlAI/sihl"
 # repository = "https://github.com/sihlAI/sihl"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 torch = "^2.0.0"
 torchvision = "^0.15.1"
 torchmetrics = "^0.11.4"
-lightning = {version = "^2.0.2", optional = true}
+lightning = { version = "^2.0.2", optional = true }
+timm = { version = "^0.9.2", optional = true }
+importlib-resources = { version = "==5.12.0", markers = "python_version < '3.9'" }
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mypy = "^1.2.0"
 ruff = "^0.0.264"
 pytest = "^7.3.1"
 coverage = "^7.2.5"
-pre-commit = "^3.3.1"
-pre-commit-hooks = "^4.4.0"
 isort = "^5.12.0"
 pyupgrade = "^3.3.2"
 kaggle = "^1.5.13"
 torchinfo = "^1.7.2"
 lightning = "^2.0.2"
 tensorboard = "^2.13.0"
 
 [tool.poetry.extras]
 lightning = ["lightning"]
+timm = ["timm"]
+all = ["lightning", "timm"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
@@ -58,7 +60,8 @@
 strict = true
 warn_unreachable = true
 pretty = true
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 ignore_missing_imports = true
+warn_unused_ignores = true
```

### Comparing `sihl-0.0.2.dev0/src/sihl/heads/multiclass_classification.py` & `sihl-0.0.3.dev0/src/sihl/heads/binary_classification.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,78 @@
 from __future__ import annotations
 
+try:
+    from importlib_resources import files, as_file
+except ImportError:
+    from importlib.resources import files, as_file  # type: ignore
+
 import torch
+import torchmetrics
 from torch import Tensor
 from torch import nn
-from torchmetrics.classification import MulticlassAccuracy
-from torchmetrics.classification import MulticlassPrecision
-from torchmetrics.classification import MulticlassRecall
+from torchvision.utils import draw_bounding_boxes
 
 
-class MulticlassClassification(nn.Module):
+class BinaryClassification(nn.Module):
     def __init__(
-        self,
-        in_channels: int,
-        num_classes: int,
-        level: int = -1,
-        label_weights: list[float] | None = None,
-        label_smoothing: float = 0.0,
+        self, in_channels: int, level: int = -1, question: str = "true?"
     ) -> None:
         super().__init__()
-        self.num_classes = num_classes
-        self.level = level
-        self.label_weights = torch.tensor(label_weights) if label_weights else None
-        self.label_smoothing = label_smoothing
         self.net = nn.Sequential(
-            nn.AdaptiveAvgPool2d(1), nn.Flatten(), nn.Linear(in_channels, num_classes)
+            nn.AdaptiveAvgPool2d(1), nn.Flatten(), nn.Linear(in_channels, 1)
         )
+        self.level = level
+        self.question = question
 
     def forward(self, inputs: list[Tensor]) -> tuple[Tensor, Tensor]:
-        scores, classes = torch.max(
-            torch.nn.functional.softmax(self.net(inputs[self.level]), dim=1), dim=1
-        )
-        return scores, classes
+        scores = torch.sigmoid(self.net(inputs[self.level])).squeeze(-1)
+        return scores, scores > 0.5
 
     def training_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
-        logits = self.net(inputs[self.level])
-        loss = torch.nn.functional.cross_entropy(
-            logits,
-            labels,
-            weight=self.label_weights,
-            label_smoothing=self.label_smoothing,
-        )
+        logits = self.net(inputs[self.level]).squeeze(-1)
+        targets = labels.to(logits.dtype).to(logits.device)
+        loss = torch.nn.functional.binary_cross_entropy_with_logits(logits, targets)
         return loss, {}
 
     def on_validation_start(self) -> None:
-        self.accuracy_computer = MulticlassAccuracy(num_classes=self.num_classes)
-        self.precision_computer = MulticlassPrecision(num_classes=self.num_classes)
-        self.recall_computer = MulticlassRecall(num_classes=self.num_classes)
+        self.accuracy_computer = torchmetrics.classification.BinaryAccuracy()
+        self.precision_computer = torchmetrics.classification.BinaryPrecision()
+        self.recall_computer = torchmetrics.classification.BinaryRecall()
 
     def validation_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
         input = inputs[self.level]
-        self.accuracy_computer = self.accuracy_computer.to(input.device)
-        self.precision_computer = self.precision_computer.to(input.device)
-        self.recall_computer = self.recall_computer.to(input.device)
-        logits = self.net(input)
-        loss = torch.nn.functional.cross_entropy(
-            logits,
-            labels,
-            weight=self.label_weights,
-            label_smoothing=self.label_smoothing,
-        )
-        self.accuracy_computer.update(logits, labels)
-        self.precision_computer.update(logits, labels)
-        self.recall_computer.update(logits, labels)
+        logits = self.net(input).squeeze(-1)
+        targets = labels.to(logits.dtype).to(logits.device)
+        loss = torch.nn.functional.binary_cross_entropy_with_logits(logits, targets)
+        self.accuracy_computer.to(input.device).update(logits, targets)
+        self.precision_computer.to(input.device).update(logits, targets)
+        self.recall_computer.to(input.device).update(logits, targets)
         return loss, {}
 
     def on_validation_end(self) -> dict[str, float]:
         return {
             "accuracy": self.accuracy_computer.compute().item(),
             "precision": self.precision_computer.compute().item(),
             "recall": self.recall_computer.compute().item(),
         }
+
+    def visualize(self, inputs: list[Tensor], labels: Tensor) -> list[Tensor]:
+        scores, classes = self.forward(inputs)
+        visualizations: list[Tensor] = []
+        with as_file(files(__package__) / "NotoSansMono-Bold.ttf") as font:
+            for batch, image in enumerate(inputs[0]):
+                visualizations.append(
+                    draw_bounding_boxes(
+                        (image * 255).to(torch.uint8),
+                        torch.zeros((1, 4)),
+                        [self.question + (" Yes" if classes[batch] else " No")],
+                        colors="green" if classes[batch] == labels[batch] else "red",
+                        width=0,
+                        font=str(font),
+                        font_size=15,
+                    )
+                )
+        return visualizations
```

### Comparing `sihl-0.0.2.dev0/src/sihl/lightning_module.py` & `sihl-0.0.3.dev0/src/sihl/lightning_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """Lightning module wrapper for conveniently training Sihl models."""
 
     def __init__(
         self,
         backbone: nn.Module,
         neck: nn.Module | None,
         head: nn.Module,
-        optimizer: type[Optimizer] = torch.optim.AdamW,
+        optimizer: type[Optimizer] = torch.optim.Adam,
         optimizer_kwargs: dict[str, Any] | None = None,
         scheduler: type[Scheduler] | None = None,
         scheduler_kwargs: dict[str, Any] | None = None,
     ):
         super().__init__()
         self.optimizer = optimizer
         self.optimizer_kwargs = optimizer_kwargs or {}
@@ -38,24 +38,33 @@
 
     def training_step(self, batch: tuple[Tensor, Any], batch_idx: int) -> Tensor:
         x, *y = batch
         head_inputs = self.neck(self.backbone(x))
         loss, metrics = self.head.training_step(head_inputs, *y)  # type:ignore
         self.log("train/loss", loss, on_epoch=False, on_step=True, prog_bar=True)
         self.log_dict(metrics, on_epoch=False, on_step=True, prog_bar=True)
-        scheduler = self.lr_schedulers()
+        scheduler: Scheduler = self.lr_schedulers()  # type: ignore
         if scheduler:
             scheduler.step()
             lr = scheduler.get_last_lr()[0]
             self.log("lr", lr, on_epoch=False, on_step=True, prog_bar=True)
         return loss  # type:ignore
 
     def validation_step(self, batch: tuple[Tensor, Any], batch_idx: int) -> Tensor:
         x, *y = batch
         head_inputs = self.neck(self.backbone(x))
+        if batch_idx == 0 and self.logger and hasattr(self.logger, "experiment"):
+            try:
+                images = self.head.visualize(head_inputs, *y)  # type: ignore
+                for sample_idx, image in enumerate(images):
+                    self.logger.experiment.add_image(
+                        f"eval/{sample_idx}", image, global_step=self.global_step
+                    )
+            except Exception as e:
+                logging.warn(e)
         loss, metrics = self.head.validation_step(head_inputs, *y)  # type:ignore
         return loss  # type:ignore
 
     def configure_optimizers(
         self,
     ) -> Optimizer | tuple[list[Optimizer], list[Scheduler]]:
         optimizer = self.optimizer(self.parameters(), **self.optimizer_kwargs)
```

### Comparing `sihl-0.0.2.dev0/src/sihl/torchvision_backbone.py` & `sihl-0.0.3.dev0/src/sihl/torchvision_backbone.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,9 +133,8 @@
         setattr(self, name, torchvision_model)
         self.dummy_input = torch.empty((1, input_channels, 64, 64))
         self.output_channels = [input_channels] + [
             _.shape[1] for _ in getattr(self, name)(self.dummy_input).values()
         ]
 
     def forward(self, x: Tensor) -> list[Tensor]:
-        x = self.normalize(x)
-        return [x] + list(getattr(self, self.name)(x).values())
+        return [x] + list(getattr(self, self.name)(self.normalize(x)).values())
```

### Comparing `sihl-0.0.2.dev0/PKG-INFO` & `sihl-0.0.3.dev0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 Metadata-Version: 2.1
 Name: sihl
-Version: 0.0.2.dev0
+Version: 0.0.3.dev0
 Summary: Simple Image Heads and Layers
 License: MIT
 Author: jonregef
 Author-email: jon.regef@pm.me
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Provides-Extra: all
 Provides-Extra: lightning
-Requires-Dist: lightning (>=2.0.2,<3.0.0) ; extra == "lightning"
+Provides-Extra: timm
+Requires-Dist: importlib-resources (==5.12.0) ; python_version < "3.9"
+Requires-Dist: lightning (>=2.0.2,<3.0.0) ; extra == "lightning" or extra == "all"
+Requires-Dist: timm (>=0.9.2,<0.10.0) ; extra == "timm" or extra == "all"
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: torchmetrics (>=0.11.4,<0.12.0)
 Requires-Dist: torchvision (>=0.15.1,<0.16.0)
 Description-Content-Type: text/markdown
 
 # Simple Image Heads and Layers
 
 [![PyPI](https://img.shields.io/pypi/v/sihl.svg)][pypi_]
 [![python versions](https://img.shields.io/pypi/pyversions/sihl)][python version]
 [![coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/jonregef/c203d6bce2a485ab49d1814ff3218a06/raw/covbadge.json)][coverage]
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+[![ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)][ruff]
 
 [pypi_]: https://pypi.org/project/sihl/
 [python version]: https://pypi.org/project/sihl
 [coverage]: https://coverage.readthedocs.io/en/7.2.5/
-[pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
+[ruff]: https://github.com/astral-sh/ruff
 
 ## Installation
 
 ```console
 pip install sihl
 ```
```

